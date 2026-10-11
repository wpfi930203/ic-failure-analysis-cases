---
title: "ISTFA-2010.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_c96412a3bdf9889a9efec0f9fb0d7d217295230462135641
file_size: 68919102
---

ISTFA  2010   Conference Proceedings from the


36th International Symposium


for Testing and Failure Analysis


November 14 –18, 2010  InterContinental Hotel Dallas  Dallas, Texas, USA


Sponsored by


www.asminternational.org/istfa


www.asminternational.org


Published by


ASM International®


Materials Park, Ohio 44073-0002


TM


Copyright  © 2010


by


All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any  means, electronic, mechanical, photocopying, recording, or otherwise, without the written permission of  the copyright owner.


First printing, November 2010


Great care is taken in the compilation and production of this Volume, but it should be made clear that NO  WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES  OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN  CONNECTION WITH THIS PUBLICATION. Although this information is believed to be accurate by  ASM, ASM cannot guarantee that favorable results will be obtained from the use of this publication alone. This publication is intended for use by persons having technical skill, at their sole discretion and risk. Since  the conditions of product or material use are outside of ASM's control, ASM assumes no liability or  obligation in connection with any use of this information. No claim of any kind, whether as to products or  information in this publication, and whether or not based on negligence, shall be greater in amount than the  purchase price of this product or publication in respect of which damages are claimed. THE REMEDY  HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND SOLE REMEDY OF BUYER, AND IN NO  EVENT SHALL EITHER PARTY BE LIABLE FOR SPECIAL, INDIRECT OR CONSEQUENTIAL  DAMAGES WHETHER OR NOT CAUSED BY OR RESULTING FROM THE NEGLIGENCE OF  SUCH PARTY. As with any material, evaluation of the material under end-use conditions prior to  specification is essential. Therefore, specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or  reproduction, in connection with any method, process, apparatus, product, composition, or system, whether  or not covered by letters patent, copyright, or trademark, and nothing contained in this book shall be  construed as a defense against any alleged infringement of letters patent, copyright, or trademark, or as a  defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN-13:978-1-61503-041-5


ISBN-10: 0-61503-041-7


SAN: 204-7586


Materials Park, OH 44073-0002


Printed in the United States of America


Multiple copy reprints of individual articles available from Technical Department, ASM International.


iii


EDFAS 2010-2011 BOARD OF DIRECTORS


EDFAS President                                                EDFAS Vice President  Dr. Thomas Moore                                                 Jeremy Walraven


OmniProbe                                                   Sandia National Labs


|Board Members |Position |Affiliation |
|---|---|---|

|Dr. Thomas Moore |EDFAS President |OmniProbe |

|Mr. Jeremy A. Walraven |EDFAS Vice President |Sandia National Laboratories |

|Mr. David P. Vallett |Secretary |IBM Systems and Technology |

|Ms. Sandra Delgado |Finance Officer |Nanolab Technologies |

|Mr. Tracy D. Myers |Past President |ON Semiconductor |

|Mr. Randall S. Barnes |Executive Director |EDFAS |

|Ms. Susan Li |Member at Large |Spansion |

|Dr. Philippe Perdu |Member at Large |CNES |

|Mr. Matthew Thayer |Member at Large |Advanced Micro Devices |

|Ms. Cheryl Hartfield |Member at Large |OmniProbe |

|Mr. Christopher L. Henderson |Member at Large |Semitracks, Inc. |

|Board Committees |Position |Affiliation |
|---|---|---|

|Prof. Christopher C. Berndt, FASM |ASM BOT Liaison |Swinburne University of Technology |

|Ms. Rosalinda M. Ring |EDFA Chair |SMSC Austin |

|Mr. Thomas Zanon |Education Chair |PDF Solutions Inc. |

|Mr. Jeremy Walraven |Events Chair |Sandia National Laboratories |

|Mr. John West |Membership Chair |Texas Instruments |

|Mr. Tracy D. Myers |Nominating Chair |ON Semiconductor |

|Mr. Jeremy Walraven |Website Chair |Sandia National Laboratories |

iv


ORGANIZING COMMITTEE


William E. Vanderlinde      Jeremy Walraven               Philippe Perdu                    Dan Bodoh                        Sam Subramanian


General Chair               Vice General Chair               Technical Chair                  Tutorial Chair                      Tutorial Vice Chair


IARPA                       Sandia National Labs                        CNES                        Freescale Semiconductor              Freescale Semiconductor


Nicholas Antoniou


Immediate Past General Chair


Center for Nanoscale Systems (CNS), Harvard University


Activities Chairs


James Demarest


Local Arrangements/Publicity  Chair


IBM


Becky Holdford


Local Arrangements/Publicity  Co-Chair


Texas Instruments, Inc.


Martin Keim


AV Chair


Mentor Graphics Corporation


Ed Keyes


User’s Group Chair


Independent Consultant


Susan Li


EDFAS Liaison


Spansion


Efrat Raz-Moyal


Expo Chair


Omniprobe, Inc


David Su


International Chair


TSMC


Zhiyong Wang


Panel Discussion  Chair


Intel Corporation


Thomas Zanon


Education Short Course Chair  PDF Solutions, Inc.


v


ISTFA 2010 TUTORIAL COMMITTEE


ISTFA 2010


Tutorial Program Chair


Dan Bodoh


Freescale Semiconductor


|Tutorial Committee Chair |Topic |Affiliation |
|---|---|---|

|Dan Bodoh |Technology-Specific Failure Analysis |Freescale Semiconductor |

|Sam Subramanian (Vice Chair) |Technology-Specific Failure Analysis |Freescale Semiconductor |

|Susan Li |Fault Isolation |Spansion |

|Randy Mulder (Vice Chair) |Fault Isolation |Silicon Laboratories |

|Chris Richardson |Die and Defect Access |Abound Solar |

|Bobby Hooghan |Microscopy and FIB |FEI |

|Jeremy Walraven (Vice Chair) |Microscopy and FIB |Sandia National Laboratories |

|Dick Ross |The Periphery of FA |Consultant |

|James Demarest |Lab Management |IBM |

vi


ISTFA 2010 SYMPOSIUM COMMITTEE


Technical Program Chair


Philippe Perdu


CNES


|Alternative Energy |Alternative Energy |Counterfeit Electronics Risks |Counterfeit Electronics Risks |FA Process Case Studies |FA Process Case Studies |
|---|---|---|---|---|---|

|OTWIN BREITENSTEIN (CHAIR), |OTWIN BREITENSTEIN (CHAIR), |and Mitigations |and Mitigations |ROSE RING (CHAIR), SMSC |ROSE RING (CHAIR), SMSC |

|Max Planck Institute of |Max Planck Institute of |BHANU SOOD (CHAIR), Center for |BHANU SOOD (CHAIR), Center for |LEO G. HENRY (CO-CHAIR), |LEO G. HENRY (CO-CHAIR), |

|Microstructure Physics |Microstructure Physics |Advanced Life Cycle Engineering |Advanced Life Cycle Engineering |ESD/TLP Consulting |ESD/TLP Consulting |

|DAVID NILES (CO-CHAIR), |DAVID NILES (CO-CHAIR), |GARY SHADE (CO-CHAIR), |GARY SHADE (CO-CHAIR), |Dave Burgess, Accelerated Analysis |Dave Burgess, Accelerated Analysis |

|Avago Technologies |Avago Technologies |Insight Analytical Labs |Insight Analytical Labs |Michael Campin, Advanced Micro Devices |Michael Campin, Advanced Micro Devices |

|Christian Boit, University of Berlin |Christian Boit, University of Berlin |David Cheek,Quantum Corporation,|David Cheek,Quantum Corporation,|Taylor Cavanah, DCG Systems |Taylor Cavanah, DCG Systems |

|Stephan Gall, CSG |Solar AG |Kundan Malik, |Hamilton Sundstrand Corp. |Robert Champaign, Raytheon |Inc. |

|Jerry Kukulka , |Spectrolab |Ramesh Varma, Corporation |Northrop Grumman |Yu-Chang Lin, TSMC Vijay Chowdhury, Evans Jan Gaudestad, Neocera |Analytical Group LLC |

|Board and System |Level FA |||Antonio Orozco, Neocera |LLC |

|APEK MULAY |(CHAIR), |Defect Characterization |and |Chris O'Connor, RTI Ted Kolasa, Superior |Robson Technologies Technical Services |

|Texas |Instruments |Metrology ||JH Li, TSMC ||

|ROGER |STEIRMAN (CO-CHAIR), |PHIL KASZUBA |(CHAIR), IBM |Tim McGrady, ATMEL |Corporation Technologies |

|Omniprobe |Inc. |TERRY KANE (CO-CHAIR), |IBM |David Niles, Avago Ohnmar Nyi, |WaferTech |

|Carlos Arroyave, Peregrine |Semiconductor |Daminda |Dahanayaka, University of Oklahoma |John Olson, MAL ||

|David Burgess, Accelerated |Analysis |Don Scansen, |SemiconDR |Paiboon |Tangyunyong, Sandia National |

|Joe Colangelo, |Raytheon Inc. |Jim Slinkman, IBM ||Laboratories ||

|Bob Davis, Texas |Instruments |Pai Tangyunyong, |Sandia National Laboratories |Martin Versen, Martin Villafana, |University of Rosenheim Qualcomm Laboratories |

|Circuit Edit ||||Peter Yuen, Intel |Corporation |

|TED LUNDQUIST |(CHAIR), |Emerging Conc ||||

|DCG Systems||MIKE BRUCE |(CHAIR), |MEMS, |Discrete and |

|DCG Systems ||Independent |Consultant |Optoelectronic |Device FA |

|MIKE PHANEUF |(CO-CHAIR), |||JIM COLVIN (CHAIR),||

|||AVID ALLETT |COCHAIR |IM OLVIN |CHAIR |

|Fibics, Inc.||IBM ||FA Instruments, |Inc. |

|Marsha Abramo, |Independent Consultant |||DAVID BURGESS |(CO-CHAIR), |

|Mike DiBattista, Qualcomm, |Inc |Dan Bodoh, |Freescale Semiconductor, Inc. |Accelerated |Analysis |

|Yuval Greenzweig, |Intel Corporation-Israel |Rama Goruganthu, Advanced |Micro Devices |||

|Bob Pajak, LSI |Corporation |Selim  Unlu, Boston |University |Vijay Chowdhury, Evans Carl Nail, Failure Analysis |Analytical Group Engineer |

Fibics, Inc.


David Cheek, Quantum Corporation,


epts


D


V


(-


),


Inc


JC


(


vii


Nanoprobing and Nanoscale


|Electronic Characterization |Electronic Characterization |AARON FALK (CHAIR), |
|---|---|---|

|TAYLOR CAVANAH (CHAIR), |TAYLOR CAVANAH (CHAIR), |QFI/Optometrix |

|DCG Instruments, Inc. |DCG Instruments, Inc. |WINFIELD SCOTT (CO-CHAIR), |

|ANTON RILEY (CO-CHAIR), |ANTON RILEY (CO-CHAIR), |MEFAS |

|Multiprobe Inc. |Multiprobe Inc. ||

|||Vijay Chowdhury, Evans Analytical Group |

|Dave Albert, IBM |Dave Albert, IBM |Brennan Davis, Silicon Labs |

|CJ Bonifas , Cypress |CJ Bonifas , Cypress |Joe Patterson, Independent Consultant |

|Randy Mulder, Silicone Laboratories |Randy Mulder, Silicone Laboratories |Zhongling Qian, Infineon Technologies David Vallett, IBM Michael Woo, Raytheon Inc. |

|Packaging/Assembly Level FA |Packaging/Assembly Level FA ||

|JAMES DEMAREST (CHAIR), IBM |JAMES DEMAREST (CHAIR), IBM |Posters |

|CAROL BOYE(CO-CHAIR), IBM |CAROL BOYE(CO-CHAIR), IBM |ALAN STREET (CHAIR), Inscopelabs |

|Chris Hyoung Kang,  IBM |Chris Hyoung Kang,  IBM |MARTIN VERSEN (CO-CHAIR), |

|Ted Levin, IBM |Ted Levin, IBM |University of Rosenheim |

|Jessica Tucker, The Aerospace Corporation |Jessica Tucker, The Aerospace Corporation ||

||Tim McGrady, ATMEL Corporation |Tim McGrady, ATMEL Corporation |

||Tom Paquette, Insight Analytical Labs |Tom Paquette, Insight Analytical Labs |

|Photon Based Techs.  1 |Photon Based Techs.  1 |Peter Yuen , Intel Corporation |

|FELIX BEAUDOIN (CHAIR),IBM|FELIX BEAUDOIN (CHAIR),IBM||

|HERVE DESLANDES (CO-CHAIR), |HERVE DESLANDES (CO-CHAIR), |Sample Preparation For Chip |

|DCG Systems |DCG Systems |Access and De-Processing |

|||BECKY HOLDFORD (CHAIR), |

|Kent Erington, Freescale Semiconductor, Inc. William Lo, Nvidia |Kent Erington, Freescale Semiconductor, Inc. William Lo, Nvidia |Texas Instruments |

|JeromeTouzel, Infineon Technologies |JeromeTouzel, Infineon Technologies |ROBERT CHAMPAIGN (CO-CHAIR), |

|Frank Zachariasse, NXP |Frank Zachariasse, NXP |Raytheon |

|||Jake Klein , Texas Instruments Stan Silvus, Southwest Research Institute David Su, TSMC |

FELIX BEAUDOIN (CHAIR), IBM


Photon Based Techs. 2


Sample Preparation For


.


2010 ISTFA Photo Contest winner: “A Star is Born”, Christophe DeNardi, Thales and Philippe Perdu, CNES


 is Born”, Christophe DeNardi, Thales and Philippe Perdu, CNES


|Be a Star in 37th International Symposium for |the Industry. • MEMS, Discretes and |
|---|---|

|Testing and Failure Analysis |Optoelectronic Device FA |

|November 13-17, 2011 |• Electronic Device Materials |

|McEnery Convention Center|Characterization (SIMS, |

|McEnery Convention Center |RBS, XPS, Auger, etc...) |

|San Jose, California USA |Technical symposia, user |

|Share your experiences and advance the industry |groups, seminars, short |

|and your career at 37th International Symposium for |courses, and the largest “Window View”, |

|Testing and Failure Analysis (ISTFA), the premier event |equipment exposition in the Thomas Zirilli, |

|for the microelectronics failure analysis community. |industry make ISTFA the best Freescale Semiconductor |

|Finding the Invisible Defect is the theme for 2011. |place to learn, network, and further your career! |

|Topic include: |Don’t be invisible. Stand out. |

|• Non-visible Defect (NVD) Failure Analysis |Submit your abstract and plan to attend ISTFA 2011. |

|• Detecting Counterfeit Microelectronics ||

|• Alternative Energy (Photovoltaics, Solid State |Abstract Submission Deadline: March 25, 2011. |

|Lighting, etc...) |ISTFA Exposition |

|• FA Techniques Addressing the Challenges of the |Companies interested in exhibiting and sponsoring |

|22nm Node and Beyond ||

|Emerging FA Techniques and Concepts|contact Kelly Thomas, National Account Manager at |

|• Emerging FA Techniques and Concepts |440.338.1733 or Kelly.Thomas@asminternational.org. |

|• FA Process |Custom packages available. |

|• Packaging and Assembly Level FA ||

|• Diagnostic Testing, Scanning and Debug |ASM International® |

|• Board and System Level FA |9639 Kinsman Road |

|• Metrology and In-line Device Characterization |Materials Park, Ohio 44073-0002 |

|• Fault Isolation |800.336.5152 |

||www.asminternational.org |

Don’t be invisible. Stand out.


Submit your abstract and plan to attend ISTFA 2011.


Abstract Submission Deadline: M


Don't be invisible. Stand out.arch 25, 2011.


Go to www.istfa


March 25, 2011.


.org.


ix


Contents


IPFA 2010 Best Paper


# Contents


Combining High-Resolution Pulsed TIVA and Nanoprobing Techniques to


Identify Drive Strength Issues in Mixed-Signal Circuits........................................................1


V.K. Ravikumar1, M.Y. Ho1, R.R. Goruganthu2, S.L. Phoa1, V. Narang1, and J.M. Chin1


(1) Advanced Micro Devices Singapore Pte Ltd., Singapore;


(2) Advanced Micro Devices, Inc., Austin TX, USA


Session 1: Emerging FA Techniques and Concepts


Laser Voltage Imaging: A New Perspective of Laser Voltage Probing................................5


Yin S. Ng1, Ted Lundquist1, Dmitry Skvortsov1,  Joy Liao2, Steven Kasapi2, and Howard Marks2


(1) DCG Systems, Inc., Fremont, CA, USA;


(2) NVIDIA Corporation, Santa Clara, CA, USA


Two-Photon X-Variation Mapping Based on a


Diode-Pumped Femtosecond Laser......................................................................................14


K.A. Serrels1, D.T. Reid1, T.R. Lundquist2, and P. Vedagarbha2


(1) Heriot-Watt University, Edinburgh, UK;


(2) DCG Systems Inc, Fremont, CA, USA


Quantitative, Nanoscale Free-Carrier Concentration Mapping


Using Terahertz Nearfield Nanoscopy..................................................................................20


J. Wittborn1, R. Weiland1, A.J. Huber2, F. Keilmann3, and R. Hillenbrand4


(1 )Infineon Technologies AG, Munich, Germany;


(2) Neaspec GmbH, Martinsried, Germany;


(3 )Max Planck Institut of Quantum Optics and Center for NanoScience, Garching, Germany;


(4) CIC nanoGUNE Consolider, Donostia – San Sebastian, Spain


Laser-Thermal Imaging .........................................................................................................27


R. Aaron Falk and Tram Pham  QFI, Tukwila, WA, USA


Mobile Diffractive Solid Immersion Lens Design for


Backside Laser Based Fault Localization ............................................................................32


S.H. Goh1, J.Y. Cho1, Jeffrey Lam1, J.C.H. Phang2


(1) Global Foundries Singapore, Singapore;


(2) National University of Singapore, Singapore


x


Session 2: FA Process/Case Studies


Volume Electrical Failure Analysis for Product-Specific Yield Enhancement .................38


Steven Kasapi1, Joy Liao1, Bruce Cory1, Izak Kapilevich2, Richard Portune2,  Yin Shyang Ng2, Cathy Kardach2, and Elaine Cheng2


(1) NVIDIA, Santa Clara, CA, USA;


(2) DCG Systems, Fremont, CA, USA


Case Study in Fault Isolation of a Metal Short for Yield Enhancement ............................49


Sarven Ipek and David Grosjean


Analog Devices Inc., Wilmington MA, USA


Inter Layer Dielectric Defect Induced High Contact Resistance .......................................54


Re-Long Chiu, Jason Higgins, Toby Kinder, Juha Tyni, Sharon Ying, and Jones Chung  WaferTech LLC CAMAS, Washington, USA


Failure Analysis Methodology on Systematic Defect in


ADC_PLL Ring Pattern Due to Plasma De-Chuck Process ................................................58


Ang Ghim Boon, Chen Changqing, Alfred Quah, Magdeliza, Indahwan Jony,  Lee Mern Tat, David Zhu, and Neo Soh Ping


Failure Analysis Group, QRA, Global Foundries


Fault Isolation of Sub-Surface Leakage Defects Using


Electron Beam Induced Current Characterization in


Next-Generation Flash Memory Technology Development ...............................................62


Go Nagatani1, Kenneth Yu1, Amalia Del Rosario1, Max Sidorov1,  Richard E. Stallcup II2, and Joel-Anthony Gray2


(1) Spansion Inc., Sunnyvale, CA, USA;


(2) DCG Systems Inc., Dallas, TX, USA


A Case Study: Observation of Counter Doping of Gate Poly and


Its Validation in High Density 90nm CMOS SRAM Bitcell ..................................................66


Yuk Tsang, Xiang-Dong Wang, Michael Mendicino, and Andrew Blankenship  Freescale Semiconductor Inc., Austin, TX, USA


Session 3: Packaging and Assembly Level FA I


Magnetic Microscopy for 3D Structures: Use of the Simulation Approach


for the Precise Localization of Deep Buried Weak Currents .............................................71


Fulvio Infante 1,2, Rodolphe Gomes2, Philippe Perdu2, Fabien Battistella3, Sebastien Annereau3, and Dean Lewis4


(1) FAST, Toulouse, France;


(2) CNES, Toulouse, France;


(3) Thales IT, Toulouse, France;


(4) Université Bordeaux, Talence, France


xi


Advanced Sample Preparation Method for Lead Free Bump IMC and


Solder Grain Image Enhancement .......................................................................................79


Ming-Song Sheu, Yian-Liang Kuo, Jeng-Hun Lee, Yu-Ting Lin,


Hui-Chen Chu, Tsung-Fu Tsai, and Chih-Horng Chang


Taiwan Semiconductor Manufacturing Company, Ltd., Hsin-Chu, Taiwan


Extending Acoustic Microscopy for


Comprehensive Failure Analysis Applications....................................................................84


Sebastian Brand1, Matthias Petzold1, Peter Czurratis2, and Peter Hoffrogge2


(1) Fraunhofer Institute for Mechanics of Materials, Halle, Germany;


(2) PVA TePla Analytical Systems GmbH, Aalen, Germany


Session 4: Sample Preparation for Technological Analysis


Process Induced Defects in the Silicon Substrate:


Approaches for Successful Failure Analysis ......................................................................92


J.G. van Hassel and Xiao-Mei Zhang


NXP Semiconductors, Nijmegen, The Netherlands


X-Sectional Scanning Capacitance Microscopy (SCM) Applications on


Deep Submicron Devices at Specific Sites .........................................................................98


Xiang-Dong Wang, Yuk Tsang, and Clifford Howard  Freescale Semiconductor Inc. Tempe, AZ, USA


High Volume and Fast Turnaround Automated Inline TEM


Sample Preparation for Manufacturing Process Monitoring ...........................................102


Hyoung H. Kang1, John F. King1, Oliver D. Patterson1, Steven B. Herschbein1,  James P. Nadeau2, and Scott E. Fuller2


(1) IBM Microelectronics, Hopewell Junction, NY, USA;


(2) FEI Company, Hillsboro, OR, USA


Session 5: Defect Characterization and Metrology I


Backscattered Electron Imaging for Embedded Subtle Defects in


32nm Processes ..................................................................................................................108


Z.G. Song1, H.S. Song2, J. Yu3, and T. Su1


(1) IBM, Samsung Electronics Co., Singapore;


(2) IBM STG-MD, Hopewell Junction, NY, USA;


(3) Global Foundries, Singapore


Semi-Automated Full Wafer In-Line SRAM Failure Analysis by


Dual Beam Focused Ion Beam (FIB) ..................................................................................113


Steven B. Herschbein1, Hyoung H. Kang1, Harvey E. Berman1,  Carmelo F. Scrudato1, Aaron D. Shore1, and Bing Dai2


(1) IBM Systems & Technology, Hopewell Junction, NY, USA;


(2) Stanford University, Stanford, CA, USA


xii


Simulation Studies of Fluorine-Induced Corrosion and Defects on


Microchip Al Bondpads in Wafer Fabrication ...................................................................117


Hua Younan and Nistala Ramesh Rao


Globalfoundries Singapore Pte. Ltd., Singapore


Session 6: Sample Prep for Chip Access and Device Deprocessing


A Novel Wet Etch In-situ Decapsulation of Devices on Boards ......................................122


Michael A. Gonzales and Joanna Kiljan  Qualcomm, Inc., San Diego, CA, USA


Low Temperature Plasma Decapsulation of Copper-Wire-Bonded and


Exposed Copper Metallization Devices .............................................................................127


Kristopher D. Staller


Texas Instruments, Tucson, AZ, USA


Decapsulation of Copper Bonded Plastic Encapsulated Integrated Circuits


Utilizing Laser Ablation and Mixed Acid Chemistry .........................................................133


Jake E. Klein and Lucas Copeland


Texas Instruments Inc., Tucson, AZ, USA


Session 7: Alternative Energy (Photovoltaics, Solid State Lighting, etc.)


Photoluminescence and EBIC for Process Control and


Failure Analysis in Si-Based Photovoltaics  .....................................................................137


Martin Kittler1, Tzanimir Arguirov1, Reiner Schmid1,  Winfried Seifert1, and Teimuraz Mchedlidze2


(1) IHP, Frankfurt (Oder), Germany;


(2) Joint Lab IHP / BTU Cottbus, Cottbus, Germany


Quality Evaluation Techniques of Solar Cell Module .......................................................143


Daisuke Murahara, Wataru Shimizu, Hidehisa Kubota,  Tamiko Oda, and Kazuhiro Yabe


Oki Engineering Co., Ltd., Tokyo, Japan


Combined Electron Beam Induced Current Imaging (EBIC) and


Focused Ion Beam (FIB) Techniques for


Thin Film Solar Cell Characterization ................................................................................151


Frank Altmann1, Jan Schischka1, Vinh Van Ngo2, Stacey Stone2,


Laurens F. Tz. Kwakman3, and Ralf Lehmann4


(2) FEI Company, Hillsboro, OR, USA;


This study used a scanning electron microscope (SEM)-based nanoprobing system. This system provides the capability  of maneuvering the probe tips by nanometer range to land  exactly on top of the individual source, drain, and gate  tungsten contact (Fig. 7). The SEM provides a high-resolution  real-time image that facilitates locating the device and placing


the probe tips. The SEM is operated at 1 keV to ensure there is  no transistor degradation [5].


Based on the level restorer layout and information from  electrical fault isolation described in Section II, our first  approach was to perform layer-by-layer inspection using SEM. This traditional PFA technique failed to reveal any obvious  anomalies from metal 4 down to contact level. This is not  surprising, since this is a temperature-sensitive failure (soft  failure).


Inputs from


电1


other circuits


Feeds into Failing Signal中lNMOS


nvol


Gate


DEH


PMOS1


Fig. 7: SEM image (right) showing three tungsten probes (black  arrows) landing on tungsten contacts of the NMOS transistor in the  inverter image on the left.


With the individual transistor isolated at contact level, nanoprobing is the one of the best way to obtain full-transistor  electrical characterization. Families of current versus voltage (I/V) curves are collected on multiple transistors on the good  and failing level restorer. Basic transistor parameters such as  threshold voltage (Vt), saturation drive current (Isat), and N/P  ratio can be extracted with ease. N/P ratio is the value of Nchannel Isat divided by P-channel Isat. A higher N/P ratio means  the NMOS drive strength is higher than the PMOS drive  strength. Mixed-signal circuits need tight control of this ratio  since they operate in the analog domain of the IV curve.


Data analysis


There are five PMOS and five NMOS transistors in each  level restorer identified as the failing circuit during fault  isolation, four of those inverters in parallel and grouped into  D1 in Fig. 6 while the last one, D2, is used to hold the state of  the restorer like a latch.


Fig. 8(a) shows the one of the five PMOS IDSAT curves  obtained from the failing and good level restorer with the gate  voltage set at -1V. Almost 20% deviation is observed in the  drive current of the good and bad PMOS transistor, with the  bad circuitry showing lower drive strength. Fig. 8(b) shows the  NMOS IDSAT curve with the gate voltage at 1V. The NMOS  transistor does not show a significant deviation between the  good and bad curves.


中国


Fig. 8(a):  PMOS transistor in the failing site exhibits 20-30% lower drive current (see comparison red line) compared to the good  level restorer.


vontge (up


Fig. 8(b):  NMOS transistor in the failing site shows comparable  drive current compared to the good level restorer.


This measurement is repeated in the other four PMOS and  NMOS transistors, which showed a similar response of lower  PMOS drive strength. It is therefore obvious that the failing  area exhibited weak PMOS I/V characteristics with acceptable  NMOS characteristics. This, in turn, drove the N/P ratio of the  bad transistors significantly higher than the good transistors. To validate this result, a similar experiment is conducted on a  second bad DUT (not shown here), and the results are found to  be repeatable.


Defect Identification


After the exact failing transistor is successfully identified  using nanoprobing, defect identification techniques like  focused ion beam (FIB) and scanning tunneling electron  microscopy (STEM) are used, but revealed no physical  defects. A transmission electron microscopy (TEM) sample is  then prepared to understand the low drive current behavior. The result of TEM, however, revealed no defects, and  construction analysis did not show any difference between  good and bad transistors. While TEM is a proven powerful  tool in FA [6], it has some shortcomings, like the difficulty of  quantifying the extent of implantation.


With the feedback of drive strength non-conformance and


LF好山-23


the lack of physical defects, the fabrication facility had


>FO-X


increased confidence in its identification of the failure


-+T0


Falling choultry


mechanism, and it corrected the process to increase the drive


, Dood aouby


strength of the PMOS transistor, resulting in a 100% fix.


-I0-0oh-004


IV. Conclusion


a国


This paper discussed the creative use of pulsed TIVA with


10


SIL to obtain increased sensitivity and resolution during static


404


fault isolation. This is the first report of this technique being  applied to mixed-signal circuitry to detect drive strength- and  N-P ratio-related failure mechanisms. Fig. 5 clearly highlight  of the capabilities of this technique.


306-04


A fault isolation image that resulted from the combination


Failing circuitry


of pulsed TIVA with SIL resulted in faster identification of the


25E-04


. Good circuitry


root cause and, therefore, its fix. The paper also highlights the  importance of nanoprobing to identify non-visual defects and


C


T206-04


characterize the electrical performance of circuits.


1


MMOE 156-04W=10V


n


V. References


110E-04


50E-05


[1] Phang, JCH et al., “A Review of Laser Induced


Techniques for Microelectronic Failure Analysis,” Proc


0.DE+00


Int Symp Physical & Failure Analysis of Integrated


100.2040.608101.214


Circuits (IPFA 2004), 5-8 Jul 04, pp. 255-261, 2004.


[2] Phang, JCH  et al., "Resolution and Sensitivity


Enhancements of Scanning Optical Microscopy


Techniques for Integrated Circuit Failure Analysis,” Int


Symp Physical and Failure Analysis of Integrated Circuits (IPFA 2009), 6-10 Jul 09, pp. 11-18, 2009.


[3] Quah, ACT et al., “Combining Refractive Solid


Immersion Lens and Pulsed Laser Induced Techniques for  Effective Defect Localization on Microprocessors,” Proc  International Symposium for Testing & Failure Analysis  2008, pp. 402-406.


[4] Faure, D and Waggoner, CA, “A New Sub-micron


Probing Technique for Failure Analysis in Integrated


Circuits,” ESREF 2002.


[5] Mizuno, T et al., “Maximum Permissible EB Acceleration  Voltage for SEM-Based Inspection before Electrical


Characterization of Advanced MOS,” IEEE 45th Annual  International Reliability 2007.


[6] Williams, DB and Carter, CB, Transmission Electron


Microscopy: A Textbook for Materials Science, Vols. 1-4 (Plenum Press, New York, 1996).


Copyright ©  2010 ASM International®


Proceedings from the 36th International Symposium for Testing and Failure Analysis


November 14–18, 2010, Addison, Texas, USA


# Laser Voltage Imaging: A new Perspective of Laser Voltage Probing


Laser Voltage Imaging: A new Perspective of Laser Voltage Probing


Yin S Ng, Ted Lundquist, Dmitry Skvortsov


DCG Systems, Inc., 45900 Northport Loop East, Fremont, CA 94538, USA


Joy Liao, Steven Kasapi, Howard Marks


NVIDIA Corporation, 2701 San Tomas Expressway, Santa Clara, CA 95050, USA


Abstract


Laser Voltage Imaging (LVI) is a new application developed  from Laser Voltage Probing (LVP). Most LVP applications  have focused on design debug or design characterization, and  are seldom used for global functional failure analysis. LVI  enables the failure analysis engineer to utilize laser probing  techniques in the failure analysis realm. In this paper, we  present LVI as an emerging FA technique. We will discuss  setting up an LVI acquisition and present its current  challenges. Finally, we will present an LVI application in the  form of a case study.


Introduction


Within the failure analysis community, Laser Voltage Probing (LVP) is now a well-known method of extracting signals  through the backside of silicon ICs.  LVP systems have been  available commercially for nearly 15 years and have found  their greatest application in the design debug and in the  characterization of ICs rather than for general failure analysis (FA).  There are several reasons why LVP has not been the  tool of first resort in FA, including:


1. Focus on node level probing: Typical fault isolation  processes begin with a relatively large region of interest (ROI) that may contain the suspect failing circuitry.  This ROI is  usually identified by failure data log from Automated Test  Equipment (ATE) or System Level Testing (SLT). Failure  localization is achieved by further reducing the ROI with FA  diagnostics techniques. Not being a global technique, LVP  generally becomes the tool of last resort because it is focused  on node-level probing.


2.  Time consuming: To localize a failure using LVP, the FA  engineer generally needs to search from transistor to transistor  to identify the failing transistor or logic state.  With an ever  increasing number of transistors in new designs, even with a  smart binary search, this approach can become time  consuming1.


1 With scan Design-for-Test (DFT) implementation, the FA  problem does not necessarily scale with transistor count. A  compressed scan chain with approximately 500 flops requires  at least 8 LVP measurements to identify the failing flop.


3. Limited design knowledge2: FA is driven by the failure and  not the design which is a fundamental difference between  general FA and design debug.  For DFT-related failures the  design is often relatively straightforward to understand. However, for more complex circuit types successful probing  requires help from a designer intimate with the circuit before  probing can begin. IC designers are usually preoccupied with  new designs as the former designs reach high-volume  production.


Global methods of examining an IC are always preferred and  widely utilized. These readily available methods include  photon emission microscopy which can readily reveal an Iddq  failure, as well as variations of static/dynamic laser  stimulation (SLS/DLS).  However, there are limitations with  these techniques.  Emission microscopy is challenged with an  exponential dependence on the power supply voltage, exacerbated with the continued trend of dropping core  voltages.  SLS and DLS require external signals from the  power supply or tester, both of which can be challenging to  obtain for large, complex IC’s. Additionally, both emission  microscopy and laser stimulation techniques do not provide  direct measurements of the dynamic behavior of the IC.


Laser Voltage Imaging (LVI) [1], developed as a general  extension of the LVP [2-4] technologies, has now emerged as  a candidate to complement present failure analysis techniques. Rather than acquire data at a single point on an IC in the timedomain, LVI extracts data from numerous points within an IC. Fast acquisition is required to collect a multitude of data over  varying fields-of-view (FOVs) within the IC; hence data is  acquired in the frequency-domain.  LVI can then be used to  study frequency characteristics of the IC.


This paper discusses the implementation of LVI, and its  current and potential applications. LVI application enables the  visualization of transistor activity, but more importantly can  significantly reduce electrical failure analysis time.


2 Global techniques do not imply that design information is  not needed as many global techniques are of limited  usefulness without design information.


Laser Voltage Imaging


The LVI technique (Fig. 1) uses a laser beam to raster-scan *拓芬NI准0#across a field of view.  At any point in the FOV that the laser beam interacts with a switching transistor, that transistor 28 modulates the laser beam at its switching frequency.


，图异


Consequently, the reflected light is modulated (both in  amplitude and phase) at that switching frequency.


The modulated reflected light is then converted into a  modulating electrical signal by a detector module consisting of  a photo detector, a trans-impedance amplifier and RF  amplifiers. This amplified modulating electrical signal is then  analyzed by a spectrum analyzer.


The spectrum analyzer receives the modulating electrical  signal and the output is an electrical signal that is proportional  to the intensity of the detected modulation. This signal from  the spectrum analyzer is then digitized and displayed as a  grayscale value in the LVI image.


LVI image of transistors


operating at a specific frequency


Figure 1: Laser Voltage Imaging


串


This modulation in the frequency domain is only detected on  the transistors that have frequency components at the  frequency of interest, and the modulation is mapped as the  laser is scanned over the FOV.  Transistors switching at  frequency components other than the frequency of interest are  not detected, hence ‘masked’. Concurrently, the reflected light  is also converted into an image grayscale value for each pixel  in the FOV. Consequently, both LSM image and LVI  acquisition are captured simultaneously. Fig. 2 below shows  an LSM image and the LVI acquisition taken at the clocking  frequency.


Figure 2: Laser Scanning Microscope Image and Laser  Voltage Imaging Acquisition


LVI Spectrum Analysis parameters


Acquiring LVI data requires some knowledge of the spectrum  analyzer parameters. While there are 2 types of spectrum  analyzers: super-heterodyne swept-tuned spectrum analyzer  and FFT spectrum analyzer, the discussion here focuses on the  super-heterodyne swept-tuned spectrum analyzer.


Center Frequency


The center frequency is the frequency of interest to which the


Electrical Signal


spectrum analyzer is tuned. The resolution bandwidth (RBW)


-9


determines how accurately the center frequency must be tuned.


GND


Vout


A small RBW, of say 100 Hz, requires the center frequency to  be ± 25 Hz. Though one may program an ATE or a function  generator to drive a signal of say 11 MHz, the frequency of the  actual signal could be say 10.999948 MHz. With the spectrum  analyzer tuned to 11 MHz, this would be 52 Hz off the actual  center frequency. This is significantly large error for a 100 Hz  RBW, but is acceptable for a 1 kHz RBW.


Resolution Bandwidth (RBW)


The resolution bandwidth (RBW) determines the noise floor  of the spectrum, which in turn represents the background


nLensObjective


na


2


s9nA


Modulated


2m


Analyzer


Signal In


(grayscale) level of the LVI image. The lower the RBW, the  smaller the noise floor and this result in a darker LVI


Returming Signal


background as shown in Fig. 4. However, the RBW also


Beam


affects the response time of the spectrum analyzer. In Fig.3


Splitter


Detector


below, the time response of a spectrum analyzer was captured  using an oscilloscope.


Laser Source


Figure 3: Response time of a Spectrum Analyzer with different  RBW


十


30 Hz RBW


3 kHz RBW


20 ms/div


tD +4


HtR


Note that with a smaller RBW,


there is a certain amount of delay (tD) before the  spectrum analyzer responds


the spectrum analyzer rise time (tR) is slower.


Consequently, the scan dwell time of the laser-beam while it  raster scans across an FOV has to be slowed down to the total  response time of the spectrum analyzer (which is  approximately 28 ms for the 30 HZ RBW). If the scan dwell  time is too short, the LVI data would be shifted and would  have ‘streaking’ effect in the direction of the scan. Fig. 4  illustrates these effects.


Figure 4: LVI acquisition with different RBWs and scan dwell  times. (A) Scan dwell time of 3.5 ms at 30 Hz RBW, (B) Scan  dwell  time of 28 ms at 30 Hz RBW, (C) Scan dwell time of 28  ms at 3 kHz RBW, (D) Scan dwell  time of 3.5 ms at 3 kHz  RBW


From Fig. 4, there is an obvious shift when the scan dwell  time of 3.5 ms is too fast for the spectrum analyzer’s response  time of ~ 28 ms (A). Lengthening the dwell time to 28 ms (B) corrects for the LVI shift. Since the response time of the  spectrum analyzer at 3 kHz is approximately 2.7 ms, there is  no shift and no difference in the LVI image at both 28 ms (C) and 3.5 ms (D) scan dwell time.


Video Bandwidth (VBW)


The video bandwidth (VBW) determines the noise of the  spectrum analyzer’s output to digitizer. This represents the  noise of the digitized grayscale LVI image. The lower the  VBW, the less the noise. However, like RBW, the VBW also  affects the response time of the spectrum analyzer.  In Fig 5  below, the time response of a spectrum analyzer was captured  using an oscilloscope.


Figure 5: Response time of a Spectrum Analyzer with different  VBW. RBW was set to 30 Hz


Note that with a smaller VBW,


there is no difference in the amount of delay (tD) before the spectrum analyzer responds


As with RBW, the scan dwell time of the laser-beam while it  raster scans across an FOV has to be slowed down to the total  respond time of the spectrum analyzer; which is determine by  both the RBW and VBW. Fig. 6 illustrates these effects, where  the scan dwell time was set to be very short at 870 µs to  clearly illustrate the ‘streaking’ effect of a slow rise time.


Figure 6: LVI acquisition with different VBW. The ‘streaking’ effect is caused by the spectrum analyzer’s slow rise time at  larger VBW.


Zero Span


At zero span, the local oscillator is tuned to the center  frequency and is not swept. Therefore, sweep time is not a  factor in the spectrum analyzer’s response time. This leaves  the resolution bandwidth and the video bandwidth as factors  that affect the spectrum analyzer’s response time.


Most spectral analyses involve looking at a range of  frequencies, or a frequency span. The spectrum analyzer  sweeps its local oscillator over this span while updating the  display of the spectrum analyzer. It takes time for the  spectrum analyzer to sweep across a range of frequencies, and  the minimum sweep time depends on the resolution bandwidth (RBW) and video bandwidth (VBW) of the spectrum analyzer. For example, the minimum sweep time is 200 ms for a  particular spectrum analyzer when the RBW=VBW=1 kHz. In  LVI acquisition, modulation information is to be extracted  over a large number of pixels; a 256x256 scan resolution  would result in 65,536 pixels. At 200 ms, this is more than 3½  hours! Therefore, one desires the acquisition for each pixel to  be a fast as possible.


Understanding LVP origins


LVI was first developed during the process to understand the  origins of Laser Voltage Probing (LVP) and for the most part  has only been documented in research papers [5-7]. Fig 7  shows the origin of the LVP modulation on a single FET  transistor. These results have been published and will not be  repeated in this paper.


Scan direction


主


10 Hz VBW


100 Hz VBW


tD


10 Hz VBW 100 Hz VBW


(B) (C) (D) (A)


SGD


Figure 7: Origin of LVP signal on an NFET with Gate & Drain pulsed at nominal device operating voltage.


Given a certain focus on the active layer, LVI is able to  determine the areas of LVP modulation. However, LVP  modulation and thus LVI are sensitive to focus. Fig 8 shows  several LVI images which were acquired as focus is changed.


Figure 8: Detected LVP modulation changes with focus


The experiment was conducted on a 2-gate inverter fabricated  in 180 nm process technology to enable discrimination of  modulation from the gate and drain regions. When the laser  beam is in focus (center image in Fig 8), the origin of the LVP  modulation is as expected; coming from both the drain and  gate regions. However, when the laser beam is under focused


(focused in the bulk silicon before the active layer) or over  focused (focused further into the contact layer), the  modulation seems to originate from the source region. This is  because at these foci, the beam spot size at the active & poly  layer is large and covers the entire 2-gate transistor. As a  result, the modulation detected by this laser beam is the  summation of several sources of modulation. Thus when the  laser beam is scanned over the source region, the resulting  summation produces a non-zero LVI value at this area.


The same 2-gate inverter is used to study the polarity of the  LVP modulation from the gate and drain regions using Logic


0


State LVI (patent pending). Similar studies were previously


100


conducted and its results published [7]. Further details on


90


Logic State LVI implementation warrants an entirely separate  article, and is not discussed here. Fig. 9 shows the Logic State


2O


200


LVI image, which clearly shows that the modulation from the


. .


gate and drain of a PFET transistor in a CMOS pair are of


>300


岁0


opposite polarity.


30


400


20 10


500


500400300x[pixe]2001000


Figure 9: Logic State LVI on a PFET


The hypotheses of the above observation is based on the prior  research work done on LVP origins [5-7], in which it is  reported that the LVP modulation comes from the timevarying changes in the depletion region under the gate and


1111111111


drain changes as the transistor switches between “OFF” and “ON” states.


VDD


0V


0VVDD


G


s


DS


pp


p


n-well


Figure 10: Simplified illustration of a simple CMOS inverter’s  PFET when the PFET is in the “OFF” state (left) and in the “ON” state (right)


As illustrated in Fig. 10, when the PFET of a simple CMOS  inverter is in the “OFF” state, there is no p-channel region  under the gate. Consequently, there is little or no depletion  region under the gate.  In the meantime, the P-N junction  between the P-drain and the N-well is not forward-biased; hence there is substantial depletion region under the gate.


Under   focus


In...   focus


Over


focus


ID G S G D D G S G D


D G S G D


D  G  S G  D


When the PFET is in the “ON” state, a p-channel is formed  under the gate. Since VDS = 0V when the PFET is “ON”, the pchannel is even across the gate. This p-channel forms a P-N  junction with the n-well, hence a depletion region is formed. The drain now is at VDD, and hence causes a forward bias  between the P-drain and the N-well. The depletion region  under the drain now is significantly reduced.


Therefore, when the PFET turns from “OFF” to “ON”, the  depletion region under the gate increases, while the depletion  region under the drain decreases, and vice versa. This is a  hypothesis as to the reason behind the opposite polarity seen  between the gate and drain of a CMOS inverter’s PFET. It is  to be noted that a CMOS inverter’s NFET would behave  differently, and so would PFET and NFET in NAND or NOR  gates.


These two experiments above are important in understanding  the reason LVP signals may sometimes come inverted. Depending on the lateral probe placement, LVP signals would  invert if one probes at the gate as compared to the drain. With  65nm process technology and below, there is very high  probability that the laser beam would cover both gate and  drain, and the resulting modulation would be the summation  between the 2 sources of modulation.


Current Application – Scan Chain Analysis


LVI is being currently utilized for several applications. One of  them is a stuck-at failure analysis on a compressed scan chain


[8]. It is typical that software-based ATPG diagnostics are not  able to identify the defective scan cell within the failing scanchain. A common electrical failure analysis method like  Photoemission microscopy has significant challenges with  dropping core voltages (non-detectable emission) and the  inability to discriminate timing information (emission from  huge multitude of transistors). LVI is now emerging as a  technique to debug stuck-at scan chain failures due to its  unique ability to distinguish transistor toggling at a specific  frequency, and its low core voltage probing capabilities.


Fig. 11 compares the LVI images of a good unit and a failing  unit at the scan data frequency and scan clock frequency.  LVI  images were acquired using a 0.5 NA 50x objective lens. Abnormally large LVI signals were observed on the failing  unit at both data and clock frequencies. Scan cell boundaries  of the failing scan chain were superimposed on the LVI  images and illustrated in Fig. 12. It is worth noting that the  strong modulation locations at the lower part of the images (at  and near Location 2) are not part of the failing scan chain, therefore revealing possible root-cause locations; locations  that would have taken node-level probing techniques a much  longer time to localize


Figure 11: 50x LVI images of good die (left) and bad die (right) at scan data frequency (top) and scan clock frequency (bottom).


Figure 12: CAD cell boundaries superimposed on 50x LVI  images of the failing unit at data frequency (left) and clock  frequency (right).  Note the strong modulation locations at the  lower part of the images are not part of the failing scan chain.


Fig. 13 and 14 show LVI images acquired using a 2.45 NA  220x SIL. The SIL images show the same excessive  modulation on the failing unit, and the increased spatial  resolution enabled identification the exact cells of interest.


Data Freq   Good Die


Data Freq  Bad Die


Clk Freq   Good Die


Clk Freq   Bad Die


Data Freq   Bad Die


Figure 13: 4X LSM zoom SIL LVI  images of the good die (left) and bad die (right) at the clock frequency (top) and  data  frequency (bottom) at the excessive modulation location in  the  failing scan chain (highlighted Location 1 in Fig. 12).  The red  circle in the top-right image indicates the anomalous clock  signal mixing with the data signal.


Figure 14: 4X LSM zoom SIL LVI images of the good die (left) and bad die (right) at the clock frequency (top) and  data  frequency (bottom) at the excessive modulation location  highlighted Location 2 in Fig. 12.


SIL LVI images clearly show that the clock signals were  mixing with the data signals at the gates of Location 2, indicating anomalous signal crosstalk.  LVI acquired at the  buffer that directly drives the gates at Location 2 revealed  normal activities.  Waveforms extracted at these gates with  laser probing confirm the observation.


Figure 15: Net trace and connectivity of the excessive LVI  signals: Location 1 (upper), and Location 2 (lower right).


Fig. 15 shows the net-tracing of the cells with excessive  modulation. The results of the net-tracing show that the  abnormal activities at Location 2 would result in the anomaly  at Location 1 (located in the scan chain), hence scan chain  failure.  Bridging between data and clock signals is a likely  failure mechanism.


LVI challenges


A couple of the few challenges the LVI faces today are  detecting signals with short pulses (short duty-cycle) and  signals that are non-periodic. In the frequency domain, a  periodic square wave with 50% duty cycle has discrete  spectrum peaks at


⎟⎠⎞


⎜⎝⎛


=


)


sin(


2 ππ


A


an


-- (1)


Where  n is the nth harmonic; n = 1 is the fundamental  frequency


an  is the intensity of the discrete spectrum peak at  the nth harmonic


A is the peak-to-peak amplitude of the square wave  in the time domain


(3) FEI France, SAS., Lyon, France;


(4) FEI Deutschland GmbH, Frankfurt Main, Germany


Activation Energy Analysis of Dark and Laser Illuminated I-V Characteristics of


Thin-Film Poly Silicon Solar Cells ......................................................................................158


M. Boostandoost, U. Kerst, and C. Boit


Berlin University of Technology, Berlin, Germany


xiii


Session 8: Sample Prep for Chip Access and Device Deprocessing II


Characterization and Failure Analysis of 3D Integrated


Semiconductor Devices Novel Tools for Fault Isolation,


Target Preparation and High Resolution Material Analysis .............................................163


Frank Altmann1, Matthias Petzold1, Christian Schmidt1, Roland Salzer1,  Cathal Cassidy2, Paul Tesch3, and Noel Smith3


(2) austriamicrosystems AG, Unterpremstaetten, Austria;


(3) Oregon Physics, Hillsboro, OR, USA


A Novel Junction Profiling Methodology ...........................................................................171


Tomokazu Nakai


Micron Japan, Ltd., Hyogo, Japan


Improvement of Optical Resolution through


Chip Backside Using FIB Trenches ...................................................................................176


Arkadiusz Glowacki1, Clemens Helfmeier1, Uwe Kerst1,  Christian Boit1, and Philippe Perdu2


(1) Berlin University of Technology, Berlin, Germany;


(2) CNES, Toulouse, France


Copper to Aluminum Bonding: IMC Characterization through


New Mechanical Sectioning Methods ................................................................................181


Lucas Copeland1 and Mukul Saran2


(1) Texas Instruments, Tucson, AZ, USA;


(2) Texas Instruments, Dallas, TX, USA


Sample Preparation and Analysis on Full-Thickness Silicon Wafers for


Wafer-to-Wafer Bonding Process Development ...............................................................186


Richard J. Young1, Alex Buxbaum1, Corey Senowitz1, C. Deeb2, and W.H. Teh3


(1) FEI Company, Hillsboro, OR, USA;


(2) International SEMATECH Manufacturing Initiative, Albany, NY, USA;


(3) SEMATECH, Albany, NY, USA


Session 9: Board and System Level FA


Application of Lock-in Thermography on PCB for


Fault Localization and Validation of Failure Mechanism Due to


External Discrete Component Variation ............................................................................191


William Ng1, Kevin Weaver1, Zachary Gemmill1,


Herve Deslandes2, and Rudolf Schlangen2


(1) National Semiconductor, Santa Clara, CA, USA;


System Level FA on Transmission Line Issues ................................................................196


Nicholas Konkol


Intel Corporation, Hillsboro, OR, USA


xiv


Fault Localization of Power-Ground Short via Signal Injection and


Oscilloscope Technique .....................................................................................................202


Binh Nguyen


Session 10: Photon Based Techniques I


Product Debug: Speed Problem Related to Unexpected RC Delay ................................206


J.G. van Hassel and F. Zachariasse


Timing Characterization of a Tester Operated Integrated Circuit by


Continuous and Pulsed Laser Stimulation ........................................................................211


Tuba Kiyan1, Christof Brillert2, and Christian Boit3


(1) Yildiz Technical University, Istanbul, Turkey;


(2) Infineon Technologies AG, Munich, Germany;


(3) Berlin University of Technology, Berlin, Germany


Dynamic Power Analysis under Laser Stimulation:


A New Dynamic Laser Simulation Approach ....................................................................217


A. Deyine1, P. Perdu1, K. Sanchez1, J.C. Courrège1, and Dean Lewis2


(1) THALES & CNES, Toulouse, France


(2) University Bordeaux, Talence, France


Two-Photon Absorption Laser Assisted Device Alteration Using


1340nm CW Laser: Critical Timing Fault Isolation & Localization for


32nm MPU and Beyond .......................................................................................................224


Baohua Niu, Pat Pardy, Joe Davis, Mel Ortega, and Travis Eiles  Intel Corporation, Hillsboro, OR, USA


Session 11: Posters


Failure Analysis Power Cycling Tool – FAPCT .................................................................231


Yi Yun Chua


Intel Production, Malaysia


Advanced IR-OBIRCH Analysis Technique for High Isb Failure Analysis ......................233


Kuo Hsiung Chen, Wen Sheng Wu, Yu Hsiang Shu, and Jian Chan Lin  United Microelectronics Corporation, Tainan, Taiwan, ROC


Using Nano-Probing Technique to Clarify Nickel Silicide beyond


Process Window Causing Device Failure ..........................................................................236


Jian-Chang Lin and Wen-Sheng Wu


United Microelectronics Corporation, Tainan, Taiwan, ROC


Fault Isolation on High Resistance Failure of 45nm ET Via


Chains Using Combined Technique of SEM PVC and Nanoprobing ..............................239


P.K. Tan, Z.H. Mai, Y.W. Goh, L. Zhu, S.L. Toh, Q. Deng, R. He, H. Tan,  H.L. Li, Q.F. Wang, Y.Z. Ma, W.Y. Lee, G.R. Low, and Jeffrey Lam


xv


Detecting Internal “ESD-Like” Damage on CMOS Gates .................................................243


M. Gores1 and H. Dicken2


(1) Hi-Rel Laboratories, Inc, Spokane, WA, USA;


(2) DM Data, Inc, Scottsdale, AZ, USA


Design Rule of Microchip Al Bond Pad and Optimization of


Bonding Process in Wafer Fabrication ..............................................................................249


Hua Younan, Nistala Ramesh Rao, Ang Ghim Boon, and Chen Shuting  GlobalFoundries Singapore Pte Ltd., Singapore


Backside Infrared Imaging Using Improved Refraction-Assisted


Illumination Methods ...........................................................................................................254


Terence Yeoh, Stephen LaLumondiere, Neil Ives, and Martin Leung  The Aerospace Corporation, El Segundo, CA, USA


The Novel Dopant Profile Inspection Methodology by FIB ..............................................257


Po Fu Chou and Li Ming Lu


United Microelectronics Corporation, Ltd., Taiwan, R.O.C.


Design Diagnosis with E-Beam Probing to Improve Reliability Issue


Due to Competitive Signal Error ........................................................................................261


T.C. Chuang, C.M. Shen, L.F. Wen, S.C. Lin, C.M. Huang, and Jon C. Lee  Taiwan Semiconductor Manufacture Company, Ltd., Tainan, Taiwan, R.O.C.


Application to Non Destructive Physical Analysis Method Using


X-ray CT Imaging .................................................................................................................265


Akira Mizoguchi, Minoru Sugawara, Masahide Nakamura, and Koichiro Takeuchi  Mitsubishi Electric Corporation, Kamakura City, Kanagawa pref., Japan


Fundamental Study of Al Pad Grain Size Measurement and Its Effectiveness ..............271


Yaobin Zhao, Haibo Dai, Baolin Gao, Linfeng Wu, Sanan Liang,


Chorng Niou, and Qiang Guo


Semiconductor Manufacturing International (Beijing) Corp, Beijing, P.R. China


Session 12: MEMs, Discretes and Optoelectronic Device FA


Characterization of Green and Ultraviolet LEDs by


Laser-Based FA Techniques ..............................................................................................275


M.A. Miller, E.I. Cole Jr., and P. Tangyunyong


Sandia National Laboratories, Albuquerque, NM, USA


Advanced Laser Preparation of Microsystems for Further FIB Processing ...................281


Juergen Walter, Stefan Martens, and Walter Mack  Infineon Technologies AG, Regensburg, Germany


Fast Turn-around Failure Analysis of Metal Interconnection Using


FIB and LA ICP-MS ..............................................................................................................285


Zixiao Pan1, Wei Wei1, and Fuhe Li2


(1) Exponent Failure Analysis Associates, Menlo Park, CA, USA;


(2) Air Liquide – Balazs NanoAnalysis, Fremont, CA, USA


xvi


A Novel Non-Destructive Approach to Deprocess the Sealing Cap from


MEMS Device for Failure Analysis .....................................................................................290


Hsien-Wen Liu, King-Ting Chiang, Tao-Chi Liu, Ming-Lun Chang, and Jandel Lin  Integrated Service Technology Inc., Hsin-chu, Taiwan, R.O.C.


A Novel Technique for Localization of Low Level Leakage in


Integrated Circuits ...............................................................................................................297


A. Chiang, H. Wu, H. Nguyen, W. Pratchayakun, and P. Le  Vishay Siliconix, Santa Clara, CA, USA


Session 13: Defect Characterization and Metrology – II


Energy-Dispersive X-ray Spectrometry Performance on


Multiple Transmission Electron Microscope Platforms ...................................................301


James Demarest1, Chris Deeb2, Thomas Murray3, and Hong-Ying Zhai4


(1) IBM, Albany, NY, USA;


(2) SEMATECH, Albany, NY, USA;


(3) CNSE SUNY Albany, Albany, NY, USA;


(4) Gonzer, Albany, NY, USA


Highly Resistive AlN Formation in TiN / AlCu / TiN Stack Evidenced by


EELS TEM and XPS .............................................................................................................304


B. Delahaye1, H. Fray1, J.P. Brun1, N. Guilbaud1, P. Tabary1, S. Lariviere1,  D. Basso1, M. Modi2, and M. Idir2


(1) Altis Semiconductor, Corbeil-Essonnes, France;


(2) Synchrotron Soleil, Gif-Sur-Yvette, France


Scanning Capacitance Microscopy for Failure Analysis of SOI- Based


Advanced Microprocessors ................................................................................................309


Lim Soon Huat, Lwin Hnin-Ei, Vinod Narang, and J.M. Chin  Device Analysis Lab, Singapore


Wafer Level Atomic Force Probing ....................................................................................317


Terence Kane, Sweta Pendyala, and Michael P. Tenney


IBM Systems and Technology Group, Hopewell Junction, NY, USA


Session 14: Test and Diagnostic, Test and Debug


Systematic Defect Identification through Layout Snippet Clustering .............................320


Wing Chiu Tam, Osei Poku and R.D. (Shawn) Blanton  Carnegie Mellon University, Pittsburgh, PA, USA


High Volume Scan FA for Yield Enhancement at the 90nm Node ...................................330


Ryan Ross and Gil Garteiz


Freescale Semiconductor, Tempe AZ, USA


xvii


Tester-Driven Dynamic Laser Stimulation for Hard Functional Failure ..........................332


S.H. Goh1, Y.H. Chan1, F. Zheng1, H. Tan1, J.W. Ting1, Robin Chen1, Z.H. Mai1,  Jeffrey Lam1, L.C. Hsia1, C.M. Chua2, and J.C.H. Phang2


(2) SEMICAPS Pte Ltd, Singapore


Leveraging the Power Grid for Localizing Trojans and Defects ......................................338


Jim Plusquellic1 and Dhruva Acharyya2


(1) University of New Mexico, NM, USA;


(2) Verigy Inc., Santa Clara, CA, USA


Session 15: Circuit Edit I


Success! > 90% Yield for 65nm/40nm Full-Thickness Backside Circuit Edit .................348


David W. Niles and Ronald W. Kee


Avago Technologies, Fort Collins, CO, USA


Innovative Methodologies of Circuit Edit on


Wafer-Level Chip Scale Package (WLCSP) Devices .........................................................359


Shih-Ting Liu, Tao-Chi Liu, Ming-Lun Chang, and Jandel Lin  Integrated Service Technology Inc., Hsin-chu, Taiwan, R.O.C.


Session 16: Counterfeit Electronics—Risks and Mitigation


Counterfeit Parts Recognition and Detection for Failure Analysts .................................364


Katherine V. Whittington


California Institute of Technology, Pasadena, CA, USA


Case Studies of Counterfeit Part Detection in Assembled Products ..............................369


Daniel P. Hartgerink


National Aeronautics and Space Administration, Houston TX, USA


Session 17: Photon Based Techniques II


Differential and Lockin Imaging of Dynamic Photon Emission and


Applications in Failure Analysis ........................................................................................373


Zhongling Qian1, Christof Brillert1, Christian Burmer1, and Yoshiyuki Yokoyama2


(1) Infineon Technologies AG, Munich, Germany;


(2) Hamamatsu Photonics Deutschland GmbH, Herrsching, Germany


Application of Lock-in Thermography for Backside Failure Localization


Using Solid Immersion Lenses ..........................................................................................378


Christian Schmidt1, Christian Große1, Frank Altmann1,  Jürgen Schulz2, and Alexander Seibt2


(2) Melexis GmbH, Erfurt, Germany


xviii


Combining Time Resolved Emission and Analog Simulation for


Fault Localization ................................................................................................................384


Christian Burmer1, Fabian Hopsch2, and Wolfgang Vermeiren2


(1) Infineon Technologies, Munich, Germany;


(2) Fraunhofer IIS/EAS Dresden, Germany


Developing a Chemistry-Assisted Focused Ion Beam Process for


‘On-Demand’ Solid Immersion Lenses in Silicon .............................................................389


P. Scholz1, U. Kerst1, C. Boit1, T. Kujawa2, and T. Lundquist2


Infrared and Visible—Near Infrared Electroluminescence Developments for


FA in AlGaN/GaN HEMTS on SiC .......................................................................................393


M. Bouya1,2, D. Carisetti1, J.C. Clement1, N. Malbert2, N. Labat2, and P. Perdu3


(1) THALES Research and Technology, Palaiseau, France;


(2) University Bordeaux, Talence, France;


(3) CNES Laboratory, Toulouse, France


Session 18: Nanoprobing and Nano Scale Electronic Characterization


Characterizing Gate Disturb Embedded Flash Memory Cells by


Atomic Force Probing .........................................................................................................398


M. Hoffmann, C. Nowak, A. Haase, and S. Eckl


Infineon Technologies Dresden GmbH, Dresden, Germany


Identification of a Non-LDD Induced Vt Shift Failure Mechanism via


Nano-Probe Characterization .............................................................................................403


Randal Mulder1 and Yuk Tsang2


(1) Silicon Laboratories, Inc.;Austin, TX, USA;


(2) Freescale Semiconductor, Inc.;Austin, TX, USA


Characterization of a Resistive Path to a Gate Node


Using Tunneling Current Measurements ...........................................................................409


Clifford Howard, Sam Subramanian, Kent Erington,  Randall Mulder, Yuk Tsang, and John Bartlett


Freescale Semiconductor, Inc., Austin, TX, USA


Electron Beam Absorbed Current as a Means of Locating


Metal Defectivity on 45nm SOI Technology ......................................................................413


K. Dickson, G. Lange, K. Erington and J. Ybarra  Freescale Semiconductor, Inc. Austin, TX, USA


Frequency Sensitive Soft Fails in SRAM Arrays ...............................................................423


Sweta Pendyala, Terence Kane, Michael Tenney, Richard Oldrey,  Manuel Villalobos, and John Sylvestri


xix


Session 19: Circuit Edit II (Laser, FIB, etc.)


Pulsed Spot Milling and Deposition to Enable Next Generation


Circuit Edit Via Development ..............................................................................................426


Dane Scott1, Ted Lundquist2, and Tahir Malik2


(1) Intel Corporation, Folsom, CA, USA;


(2) DCG Systems, Inc., Fremont, CA, USA


Novel Circuit Edit Solution for Bulk Copper Milling .........................................................431


Tahir Malik1, Rajesh Jain1, Ferdi Meijer2, and Tim Velthof2


(1) DCG Systems, Fremont, CA, USA;


(2) MASER Engineering, Enschede, The Netherlands


Fast Mixed Field Material Removal Using New Dielectric Etch Solution ........................440


Vladimir V. Makarov1, Leo Krasnobayev1, and James Hahn2


(1) Tiza Lab, LLC, Milpitas, CA, USA;


(2) Altera Corp., San Jose, CA, USA


Session 20: Packaging and Assembly Level FA II


Root-Cause Investigations of Stitch Bond – Shearing by Means of


3D-X-ray Computer Tomography (XCT),


Metallographic Polishing and FIB ......................................................................................444


Peter Jacob, Iwan Jerjen, and Giovanni Nicoletti


EMPA Swiss Federal Labs for Materials Testing and Research, Duebendorf, Switzerland


Methodology for Analysis of Schottky Diode Failures .....................................................449


Bhanu P. Sood1, Michael Pecht1, John Miker2, and Tom Wanek2


(1) University of Maryland, College Park, MD, USA;


(2) Emerson Network Power, Lorain, OH, USA


Resolving the Failure Analysis Challenges on Stacked Die Structure in


Lead Frame Chip Scale Package ........................................................................................457


Raymond G. Mendaros and Jon Carlo P. Salimbangon  Analog Devices Inc., Cavite, Philippines


Author Index ........................................................................................................................465


# Combining High-Resolution Pulsed TIVA and Nanoprobing Techniques to Identify Drive Strength Issues in Mixed-signal Circuits


Combining High-Resolution Pulsed TIVA and  Nanoprobing Techniques to Identify Drive


Strength Issues in Mixed-signal Circuits


Ravikumar VK1, Ho MY1, Goruganthu RR2, Phoa SL1, Narang V1, Chin JM1   Advanced Micro Devices Singapore Pte Ltd1, 508 Chai Chee Lane, Singapore 469032,  Advanced Micro Devices, Inc.2, 5900 E Ben White Blvd, Austin TX 78741, USA


Phone: (65) 679698888 Fax: (65) 62339080 Email: venkat-krishnan.ravikumar@amd.com


Abstract - This paper uses an interesting case study to  highlight high-resolution pulsed thermal-induced voltage  alteration (TIVA) with solid immersion lens (SIL) as a  technique to isolate a temperature-sensitive failure in  mixed-signal circuitry, followed by circuit analysis and  nanoprobing to confirm a drive strength issue caused by a  process change.


I. INTRODUCTION


Fault isolation for failure analysis (FA) has become  increasingly challenging with technology scaling and devices  growing more sensitive to smaller defects and process changes. This pushes the need for substantial improvements in  conventional FA techniques.


Thermal-Induced Voltage Alteration (TIVA) is a popular  fault isolation technique for detecting temperature-sensitive  defects [1]. The technique involves biasing the device under  test (DUT) with constant current and monitoring changes in  voltage. A 1340-nm near-infrared (NIR) laser is used to target  specific areas in DUT that cause localized heating and helps  isolate defects or thermally sensitive circuitries. Pulsed TIVA  is essentially similar to TIVA technique. The main  modification in pulsed TIVA is in using a pulsed laser with a  lock-in phase detection system, which improves signal-to-noise  ratio (SNR) and helps remove TIVA artifacts [2]. When  pulsed TIVA is coupled with SIL, it can result in highmagnification, high-resolution imaging, resulting in increased  accuracy in signal detection [3].


The SIL used for this analysis is made of silicon and is set  to work at a super-hemispherical focus, giving a magnification  of around 240x when combined with a backing 20x lens. It has  an effective numerical aperture (NA) greater than 2.4, which  boosts the resolution of laser imaging significantly. To `use the  SIL effectively, the units are thinned until around 100 um of  silicon remains, then mirror polished with 10 um of tolerance. Care is taken during polishing to ensure the sample preparation  requirements.


After a site has been successfully isolated using nondestructive fault isolation techniques, the DUT is de-processed  from the front side, layer by layer, and every metal layer is  thoroughly checked for anomalies. Once the top-most metal  layer of the circuitry of interest is reached, physical fault  isolation (PFI) techniques like AFM and Nanoprobing are  popularly used. PFI helps confirm the presence of the defect  electrically and isolate the defect to a much smaller area of  interest. This process is crucial for the identification and  characterization of the defect, which usually is the final step in  understanding the failure.


In this paper, we discuss a temperature-sensitive failure  case study that utilizes pulsed TIVA with SIL for fault  isolation and subsequent nanoprobing and circuit analysis to  detect a drive strength-related failure in mixed-signal circuitry.


II. FAULT ISOLATION


Failing Signature


The analysis is conducted on failing samples containing  mixed-signal circuitry with limited DFT access to the area  causing the failure.


Tests revealed the samples are temperature-sensitive and  passed more often at elevated temperature. Curve tracing (Fig. 1) showed the faulty signal (solid red) pulled to a high state  instead of remaining at a low state like the good signal (dotted  blue) when the system voltage VDD (pink dashed) is ramped. Soft defect localization, the popular technique for isolating  temperature-sensitive defects, is rendered unusable because it  is limited in design for test (DFT) features to exercise the  failure continuously. Tests showed that the part is stuck in its  state unless the supply voltage is turned down and ramped  again.


TIVA Analysis


TIVA analysis is performed by biasing the supply and  monitoring the failing signal. The supply voltage is held close  to the voltage at which the failing signal latches into a high


instead of a low state. The analysis showed a strong  disturbance at specific mixed-signal circuitry (Fig. 2).


Time (ms)


Fig.1: Curve tracing shows that the bad signal was abnormally  pulled high during power supply ramp.


40um


12um


2(a)


2(b)


Fig. 2(a): Conventional TIVA image; 2(b) is the overlay image. Streaking makes it impossible to isolate the failing circuitry.


The high sensitivity of the circuit to laser effects caused  streaking, and a change of state in the TIVA image in Fig. 2  made it difficult to isolate the actual part of the circuitry that is  sensitive. To obtain a better isolation, pulsed TIVA (Fig. 3) is  used which showed improvements over conventional TIVA.


3(a)


3(b)


Fig. 3(a): Pulsed TIVA image; 3(b) is the overlay image.


Streaking is substantially reduced.


Using pulsed TIVA, the laser is pulsed and using phase  lock detection, the streaks are effectively reduced to enable


isolation of the actual circuits that are sensitive to laser  stimulation (Fig. 3). To improve the isolation further, the  supply voltages are tweaked and the bad signal is monitored


---.....GodSignal-8ad Signal


through an oscilloscope when pulsed TIVA is performed.


The laser power is also reduced substantially to cause  minimum artifacts. As seen in Fig. 4(a), the number of TIVA  sites decreased to one, which correlated well to the failing  signature. Fig. 4(b) is a snapshot while the laser scanned the


Voltage (V)


Bad Signal


sensitive circuitry. A dip in the voltage is observed at the  location highlighted by pulsed TIVA.


Good Signal


However, the pulsed TIVA overlay image still pointed to  multiple instances in the area of interest that could potentially  cause the failure. The magnification is not high enough to  isolate the circuitry to a particular instance.


VDD1


****bad signaVDP2


oop5 8ue


4(a)


4(b)


Fig. 4(a): Pulsed TIVA image with reduced laser power and


optimized supply; 4(b) is the oscilloscope monitor of signal.


The unit is further thinned for imaging using the SIL, which  provides a magnification improvement of a 2.5x in addition to  a 5x resolution improvement compared to the state-of-the-art  air-gap lens. When combining pulsed TIVA with SIL, a higher  resolution image and more accurate fault isolation results are  obtained (Fig. 5).


5(a)


5(b)


Fig. 5(a): Image of the pulsed TIVA with SIL overlay; 5(b) is  the overlay of pulsed TIVA on digitally zoomed and cropped 0.85-NA 100x air-gap lens.


This is evident when comparing Fig. 5(b), a digitally zoomed  overlay image obtained using a 0.85-NA 100x NIR lens, to  Fig. 5(a), the overlay image obtained by using a SIL in superhemispherical mode and a 20x NIR backing lens.


Circuit Analysis


The CAD navigation tool showed that the site highlighted  by pulsed TIVA with SIL pointed to a particular transistor. On  circuit analysis and layout tracing, it is unambiguous that the  TIVA signal came from an input to a level restorer circuit that  fed to the failing signal (Fig. 6).


Draintane


Fig. 6: Block diagram of circuitry of interest. Circled transistor  T1 is highlighted by high-resolution pulsed TIVA.


Transistor T1, a PMOSFET, is the input of a level restorer  circuitry made up of two inverters: the larger D1, which feeds  forward, and the smaller D2, which helps to hold the state. A  wrong input from either a leaky or a slow PMOS T1 could  change the state of the restorer, causing the signal to flip and  the reported failure. The level restorer is powered by the  voltage supplies VDD1 and VDD2, which also supported the  observed failure.


III. Physical Failure Analysis


PFI and PFA approach


As mentioned earlier, with technology scaling of ICs, nonvisible defects have become common phenomena in FA. On  top of this challenge, the electrical failure signature for many  of the failures is soft, as presented in this study. Therefore, the  utilization of non-destructive PFI is essential to indicate the  exact failing location before attempting PFA. This section  demonstrates the successful use of nanoprobing to reveal faults  in the level restorer. The theory of nanoprobing [4] has been  adequately described in the literature.


Location 1  Clk Freq   Bad Die


Location 1  Clk Freq   Good Die  Location 1  Data Freq   Good Die


Location 1  Data Freq  Bad Die


Location 2  Clk Freq   Bad Die


Location 2  Clk Freq   Good Die


Location 2  Data Freq   Good Die


Location 2  Data Freq   Bad Die


At even harmonics (n = 2, 4, 6..), the sine value would be zero, therefore, a periodic square wave with 50% consists of  discrete spectrums at the fundamental and at the odd multiples  of the fundamental frequency. The bulk of the signal’s power


a


is at the fundamental frequency, with the power decreasing at


e ! ^


its harmonics by a factor of n at each nth harmonic (Fig 16). In  LVI, we tuned in to this fundamental frequency in order to


N V


acquire maximum intensity of the signal’s spectrum.


C E N T E R ↓ 1 2 5 _ 0 ↓ H H z


S d Y N ↓ Z S O _ O ↓ M H Z


C E N T E R ↓ 1 2 5 _ 0 ↓ M H z


S P A N ↓ 2 5 0 _ 0 ↓ M H z


Figure 16: Frequency spectrum of a 25 MHz 50% duty cycle  square wave (top) and a 25MHz 30% duty cycle wave (bottom).


Duty Cycle


However, the power of the fundamental frequency drops as  the signal’s duty cycle changes. In a frequency domain, a  square pulse wave has discrete spectrum peaks at


壹( ))sin(2dnnA


π


e 福


-- (2)


8 p  p a


Where  d is the duty cycle.


Using equation (2), the intensity of the fundamental frequency  a1 is plotted across several different duty cycles (Fig. 17)


Amplitude vs Duty Cycle @ Fundamental Freq


0.0


0.2


0.4 0 u l u d


0.6 n Z p


0.8 p a


1.0


0.1


0.3


0.4


0.5


M A R K E R


2 4 _ 8 ↓ M H z


Figure 17: The intensity of the fundamental decreases in a  logarithmic manner in relation to the duty cycle.


Fig. 16 showed the comparison of the 50% duty cycle square  wave versus a 30% duty cycle pulse. Note that for a pulsed  signal, discrete spectrum peaks now appear at the even  harmonics. The fundamental frequency loses some of its  intensity.


A drop in the fundamental frequency’s intensity reduces the  SNR of the LVI signal. The ability to capture LVI data on  these signals is diminish as fundamental frequency’s intensity  in the modulated reflected light drops towards the noise floor


of the acquisition system.


Non-Periodic Signal


As signals become slightly non-periodic, a gated clock for  example, the intensity of the periodic signal decreases as well. For the sake of simplicity, we use the term ‘periodicity’ to  define the duration of the periodic signal, as illustrated in Fig.


18.


Figure 18: Definition of ‘periodicity’


Results show the intensity of the fundamental frequency as ‘periodicity’ is varied (Fig. 19).


Amplitude vs Periodicity @ Fundamental Freq


0.6


0.7 J 0 W w  d


0.8 n Z


0.9


0.7


0.8


Periodicity


Figure 19:  The intensity of the fundamental decreases  linearly with ‘periodicity’.


10101010101010101010 100% periodicity  10101010101010100000 80% periodicity  10101010101000000000 60% periodicity  10101010001000000000 40% periodicity  10100000000000100000 20% periodicity


Figure 20: Frequency spectrum of a 25 MHz 100% periodic  signal (top) and a 25MHz 90% periodic signal (bottom).


Fig. 20 shows the comparison of the 100% periodic signal  versus a 90% periodic signal, both with 50% duty cycle. Note  discrete spectrum peaks now appear at non-harmonic  frequencies.


As the signal becomes more non-periodic, the energy of the  spectrum peaks start to spread across the spectrum, and this  reduces the intensity of the spectrum peak at the fundamental  frequency and harmonics. As in the duty cycle discussion, drop in the fundamental frequency’s intensity diminishes the  acquisition system’s capability to acquire LVI data.


Conclusion


LVI is a useful extension of LVP into the frequency and  imaging space. Specifically, we have shown that it is practical  and useful technique for measuring time-varying signals in an  IC. LVI does not require any special hardware setup, aside  from setting up the stimulus in a continuous loop. Unlike SLS  and DLS techniques, it does not require any signal to be  extracted from the tester power supply or a dedicated pass/fail  indicator. From the point of view the simplicity of the setup it


is a closer cousin to static emission than to the other laserbased techniques.


The global, image-based nature of the measurements makes it  much easier to discover phenomena which were unexpected  from the initial test results but are nonetheless critical to  understanding the root cause of the failure. This was  illustrated in the Scan Chain Analysis example, in which  possible root cause location(s) are revealed.


LVI is not applicable to all FA problems.  Some part of the IC  must be functioning and it must be possible to stimulate the  defective area in a continuous loop. In principle LVI can be  applied to any failure analysis problem in which a timevarying signal can be used to localize and identify the defect. We are currently investigating applications of LVI to memory  debug and ATPG scan capture failure analysis.


LVI also does not replace final PFA. By providing better  defect localization and identification we believe that LVI will  significantly improve PFA hit rate and throughput. We need to  perform more real-world case studies to defend this claim, but  our results so far are very promising.


Acknowledgement


We want to acknowledge our reviewer, Dan Bodoh, in helping  us to improve this paper through his comments and  encouragement.


References


[1] S. Kasapi, U.S. Patent 7,733,100 B2


[2] H. K. Heinrich, D. M. Bloom, B. R. Hemenway, K. McGroddy, and U. Keller, “Noninvasive Optical Sheet  Charge Density Probe for Silicon Integrated Circuits”, IEEE Transactions on Electron Devices vol. 33 (11), 1987, p 1860.


[3] M. Paniccia, T. Eiles, V.R.M. Rao, and W.M.Yee, “Novel Optical Probing Technique for FlipChip  Packaged Microprocessors”, International Test  Conference (ITC), 1998, p 740


[4] Yin S Ng, W Lo, K Wilsher, “Next Generation Laser  Voltage Probing”, ASM-ISTFA 2008, p. 249


[5] U Kindereit, G Woods, J Tian, U Kerst, C Boit, “Investigation of Laser Voltage Probing Signals in  CMOS Transistors”, IEEE-IRPS 45 (2007) 526.


[6] U Kindereit, G Woods, J Tian, U Kerst, R Leihkauf, C  Boit, “Quantitative Investigation of Laser Beam  Modulation in Electrically Active Devices as Used in  Laser Voltage Probing”, IEEE Trans Dev Mater Reliab  7 (2007)19


[7] U Kindereit, C Boit, U Kerst, S Kasapi, R Ispasoiu, R  Ng, W Lo, “Comparison of laser voltage probing and  mapping results in oversized and minimum size devices  of 120 nm and 65 nm technology”, Micro Rel 48 (2008) 1322


[8] J. Liao, S. Kasapi, B. Cory, H. Marks and Y Ng, “Scan  Chain Failure Analysis using Laser Voltage Imaging”, to be presented at  ESREF 2010


# Two-Photon X-Variation Mapping Based on a Diode-Pumped Femtosecond Laser


Two-Photon X-Variation Mapping Based on a Diode-Pumped  Femtosecond Laser


K. A. Serrels, D. T. Reid


School of Engineering and Physical Sciences, Heriot-Watt University,Edinburgh,EH14 4AS, UKSchool of Engineering and Physical Sciences, Heriot-Watt University, Edinburgh, EH14 4AS, UK k.a.serrels@hw.ac.ukk.a.serrels@hw.ac.uk


T. R. Lundquist, P. Vedagarbha


DCG Systems Inc, 45900 Northport Loop East, Fremont, CA 94538, USADCG Systems Inc, 45900 Northport Loop East, Fremont,CA 94538, USA


AbstractAbstract


By inducing two-photon absorption within the device layer  of a proprietary silicon test chip, the first nonlinear variant  of X-variation mapping is reported by demonstrating  frequency mapping of a ring oscillator circuit at 1.55µm.


The microelectronics industry is characterized by the  exponential rate at which its products increase in  performance, transistor count, integration density and  functionality - all trends that adhere to the demands of  Moore’s Law. Gordon E. Moore’s prognostic prediction  has held true for almost half a century and will continue  over the next decade and beyond. The semiconductor  integrated-circuit (IC) industry is therefore in constant  pursuit of the latest cutting-edge technologies in order to  address this requirement. As a result, the level of  complexity required to fabricate these devices is elevated  to such a degree that previously rare failure modes are  becoming significant and difficult to avoid. The current  state-of-the-art in IC design relies on a fusion of  sophisticated materials engineering, dense threedimensional multilayer architectures and innovative  multiprocessing schemes; therefore the characterization  capabilities of the failure analyst must be expanded in  order to maintain a state of parallel progress.


Laser signal injection microscopy covers an extensive range  of possible device probing configurations and technologies  for advanced device failure analysis (FA). Recent  developments in this regime of semiconductor device FA  have exploited the use of laser scanning near infrared (NIR) microscopy for the purposes of surface and sub-surface  fault localization and defect characterization. Fault  localization techniques generally rely on either laserinduced thermal or power alteration schemes such as  optical beam-induced resistance change (OBIRCH) [1], resistive interconnect localization (RIL) [2] and soft defect  localization (SDL) [3]; whereas defect characterization is  typically based on laser-induced carrier generation  techniques such as optical beam-induced current (OBIC) imaging [4] and laser-assisted device alteration (LADA)


[5]. Therefore, through extrapolation and amalgamation of  the traditional OBIC technique we investigate the feasibility  of two-photon LADA (2p LADA)1.


Two-photon absorption (TPA) is a nonlinear effect and, although it is difficult to observe using continuous-wave  laser sources, it can be easily demonstrated with a few  milliwatts of light using femtosecond pulses from a  modelocked laser. The main requirement for inducing  observable TPA in a semiconductor sample is to ensure that  the incident laser photon energy is exactly equal to, or  greater than, half the material bandgap energy. This is  characteristic of TPA since no carriers will be generated at  these photon energies at low intensities – i.e. no optical  absorption. The absorption spectrum of silicon exhibits  extremely low absorption values at sub-bandgap (< 1.1 eV) energies; however, it is possible for the semiconductor  material to simultaneously absorb two, or more, photons at  sufficiently high optical intensities. When this event takes  place a single electron-hole pair is generated within the  material. This unique multi-photon absorption process  addresses the contradictory requirements encountered using  traditional linear methodologies of focusing through thick  substrates while maintaining sufficient absorption at the  focus of a laser beam to produce a strong signal. Furthermore, it has already been exploited in several novel  semiconductor IC studies [6], including state-of-the-art  polarization-sensitive and pupil-function engineering  super-resolution techniques [7, 8] as well as 3D imaging


[9]. Consequently, 2p LADA2 has the potential to become a


1 There is an additional consideration when using a  femtosecond laser to induce LADA—the timing of the  laser pulse with respect to the transition of the transistor. In traditional LADA, the laser is always on so this issue


does not arise; however, in the case of a pulsed laser, it is  imperative that the transition happens when the laser is  active and parked on the transistor of interest.   The  lifetime of electron-hole pairs is short compared to the  time between laser pulses.


2 In particular 2p LADA may prove to be more sensitive  than single-photon LADA as any invasiveness would be  decreased due to the reduced laser injection time.


powerful technique for determining critical timing paths at  ultra-high-resolution within a silicon IC.


Two-Photon Absorption in Semiconductor  Integrated-Circuits


There are many benefits to be gained through the  exploitation of TPA over single-photon absorption in the  context of silicon IC characterization and debug; therefore, it is important to consider the physical and optical  parameters behind such a technique before effective  implementation can be achieved. Since silicon is  transparent to the incident laser radiation in the linear  regime, the conventional single-photon exponential  attenuation within the sample (Beer’s Law) due to such a  condition can no longer be applied. The generation of  electron-hole pairs (carriers) through the TPA process is  proportional to an intensity-squared relationship with the  incident laser pulse. This indicates that there will only be  significant nonlinear absorption within the high-intensity  focal-volume of the focused beam. This unique property  allows for the injection of carriers to occupy any region  within the sample, ultimately providing the option to  generate a 3D map of absorption sensitivity sites on a  device through the backside illumination of ICs which  have been fabricated using silicon or even gallium arsenide (GaAs) or indium phosphide (InP) wafers for that matter. In addition, the generated charge trail – i.e. the level of  carriers generated as a function of laser intensity –produced through the TPA process differs in appearance to  that generated through single-photon absorption.


Ramsay et al [10] described these processes in detail with  an emphasis on understanding the focal dependence of a  nonlinear signal in the presence of strong linear signal  within a semiconductor device. This simple numerical  simulation models the depletion of laser power of a  converging beam as it enters a silicon IC that exhibits both  linear and nonlinear absorption. We note here that, although sometimes overlooked, residual single-photon  absorption at wavelengths longer than the bandgap  wavelength of silicon is, and must always be, included in  this, or any other, model for completeness – silicon IC  substrates are often highly doped, resulting in a significant  single-photon absorption coefficient beyond the silicon  band-edge. The progression of the model considers the  case of a focused Gaussian-profiled beam as it enters a  silicon IC which contains, at a depth of 100 µm, a thin  device layer that is responsible for electron-hole pair  generation and collection. At relatively low intensities the  overall absorption is dominated by linear absorption; however, as the intensity increases towards the focus, the  TPA contribution to the overall absorption increases since  TPA is nonlinearly proportional to the intensity of the  beam. After the focal region of the beam has been  traversed, the TPA contribution decreases again and the  single-photon absorption begins to dominate once more.


The model described above was obtained by numerically  solving the differential equation:


where P is the peak optical power in the beam at z, α is the  linear absorption coefficient, β is the TPA coefficient and  a is the area of the beam at point z, where    and is the Gaussian beam radius, which is defined by:


here,  is the size of the focused spot, z is the distance propagated from the focus λ is the free space laser  wavelength of the excitation beam and n is the refractive  index of silicon.


Figure 1 plots the overall absorption signal generated, as  expressed in the Ramsay et al [10] numerical model, as a  function of focal position through the silicon IC.


Figure 1 – Total absorption signal generated as a function  of focal position. The active device layer is situated 100µm  from the surface of the silicon substrate (i.e. z=100) [10].


Note here that an extended focal range, beyond the device  layer, has been simulated in order to demonstrate that even  when the effective focal spot of the laser has travelled  beyond the device layer there still remains a considerable  level of signal observed. Therefore, it is also important to  note that since the magnitude of induced TPA depends  nonlinearly on the power in the beam, if a considerable  level of single-photon absorption takes place before the  device layer, the overall beam power will be significantly  depleted. This will result in a lower TPA signal being  generated and, ultimately, a lower signal-to-noise ratio  than that possible when TPA is dominant. As a result, it is  useful to stress here that one can minimize this effect (i.e. unwanted residual single-photon absorption) when probing  semiconductor microelectronic circuits by preparing a


thinned device substrate.  Thus thinning the substrate to  100 μm or less has become standard practice for various  optical FA techniques.  For probing full thickness die (780 µm), the doping levels will be critical to success.  (Note: Even in heavily doped IC substrates the doping levels are  much less than the doping of the N/P wells and less again  than the S and D regions.)


The expressions presented above provide the necessary  details required to understand the advantages of TPA in  semiconductor device studies. One main property that has  been derived is that for single-photon absorption (abovebandgap excitation) there will be an exponential decrease  in carrier generation as a function of depth within a  material. This property results in an exponential optical  absorption throughout the volume of the beam within the  sample due to intrinsic optical attenuation that is linear  with respect to laser irradiance; however, in a TPA  arrangement, the absorption follows an intensity-squared  relationship which ultimately provides an ability to inject  carriers at any given depth within the sample. This  approach is analogous to the practice of optical sectioning  in two-photon confocal fluorescent microscopy where an  intensity-squared fluorescence relationship alleviates the  issues of excessive sample absorption, sample damage  through photo-bleaching and limited optical probing  performance since a signal is only generated throughout  the focal-volume of the incident beam. When this process  takes place the resulting fluorescence can be detected at  any location surrounding the sample due to its isotropic  emission (i.e. 3D detection). These advanced nonlinear  probing techniques have already been adopted from the  biological sciences and applied to the investigation and  analysis of silicon ICs [9].


Results and Discussion


The circuit under investigation was a ring oscillator  located 100 µm through the substrate of a proprietary chip  fabricated by DCG Systems for the evaluation of advanced  optical diagnostic platforms. The 500 MHz ring oscillator  structure was used to evaluate laser-induced frequency  variations. The output of this circuit was accessible  through a divide-by-32 stage which resulted in a 15.625  MHz signal at the appropriate output pin of the DUT. This  output was then connected to an RF spectrum analyzer as  in X-Variation mapping [11, 12, 13, 14].  An experimental  test procedure was conceived to measure the variations in  frequency of the ring oscillator at every pixel position as  the laser raster scanned across the device. This was  achieved through the construction of a custom 1.55 µm  laser scanning microscope (LSM) that incorporated a fibercoupled ultrafast erbium-doped fiber laser, whose design  has been reported previously [15], and a near-IR objective  lens (NA=0.8).  The acquisition software scan resolution  was selected to be 512 × 512 pixels. The experimental  arrangement is illustrated in Figure 2 and the results from  the experiment are shown in Figures 3 (a) and (b).


Figure 2 – Schematic of experimental configuration for  two-photon frequency variation mapping.


Figures 3 (a) and (b) were acquired with a laser power of


4.45mW (0.35mW delivered) and a dwell time of 3.4µs.  Figure 3 (a) shows the confocal reflection image of the  area of interest that includes the ring oscillator structure at  100× magnification. The effect of the 1.55 µm wavelength  laser on the ring oscillator structure can be clearly seen as  the darker areas in Figure 3 (b). The dark areas on the  image indicate that the laser has induced a reduction of the  output operating frequency from the ring oscillator as a  result of the nonlinear laser stimulation of the active  inverter stages. This reduction is a standard LADA  characteristic which illustrates that the low-to-high  transition times of a switching PMOS transistor are  decreased whereas the high-to-low transition times are  increased – with the change in the high-to-low transition  times dominating over low-to-high transition times [16]. This timing mismatch results in a decrease of the output  frequency when the laser stimulates the inverter structure. It is natural to assume that the darker region should  therefore consume the entire feature of interest; however, to serve as a reference marker, this particular ring  oscillator had its stages configured to be deliberately  redundant after the 37th stage – which is evident on Figure  3 (b). Furthermore, on closer inspection, it is clear that the  modulated contrast within the darker region is not random  and actually follows the intricate stage features of the ring  oscillator.


The benefits that two-photon stimulation processes hold  over conventional single-photon techniques can be clearly  seen when the nonlinear image presented in Figure 3 (b) is  compared and contrasted against previously obtained  linear data of the same 500-MHz ring oscillator circuit


[16]. The images illustrated in Figure 4 (a) and (b) were  obtained using a 100mW continuous-wave 1064 nm  excitation laser source at magnifications of 20×  and 100×, respectively. The dwell time was 1.63ms and the testing  configurations employed were similar to that adopted for  the nonlinear frequency variation probing scheme. The  first notable characteristic is the difference between the  magnitudes of the absorption-sensitive areas of both the


two-photon and single-photon induced map proportional to the square of the optical i highly localized region of interest will be st incident 1.55 µm radiation. This is clearl comparing Figure 3 (b) with both Figure 4 Figure 4 (a), the larger field-of-view confir absorption-sensitive zone for single-ph spans a significant portion of the chip’s  exponentially from the centre of the feat Figure 4 (b) further supports this trait; how the map contains only the localized feature


(a)


Figure 3 – (a) Confocal LSM image of  frequency variation image of the same feat from top to bottom, left to right.  Darker  vertical lines that are observable on this f with ring oscillator circuits; they are not ob


Figure 4 – (a) Single-photon frequency var resolution and 20× magnification and (b) S 512 scan resolution and 100× magnificatio


s. Since TPA is  ntensity, only a  imulated by the  y illustrated by


(a) and (b). In  ms that the total  oton processes  area, decaying  ure of interest. ever, this time, s of interest that


are influenced by the incid single-photon absorption le circuit features to reveal th adjacent 1 GHz ring os interconnecting tracks) as  elements of the functiona individual stages of the 50 hand, the two-photon map displays only the active frequ from the functional circuit fe


(b)


the 500-MHz ring oscillator circuit at 100× magn ure (also at 100×  magnification) simultaneously ac regions denote a lower output frequency as the lase requency variation image are a result of the frequen served in the CW image because of its much shorter a


iation image of the 500MHz ring oscillator circuit tak ingle-photon frequency variation image of the same f n [16].


ent laser light. Here we see  aking across to neighboring  eir general structure (e.g. an  cillator circuit and some  well as the more detailed  l circuit features (i.e., the  0MHz circuit). On the other   presented in Figure 3 (b) ency perturbations emanating  atures.


ification and (b) Two-photon  quired as the laser is scanned  r is scanned.  The granulated  cy drift commonly associated  cquisition time.


en at 1064nm, 512 x 512 scan  eature taken at 1064nm, 512 x


Furthermore, in support of a consistent comparison


between the two probing configurations, it is important to


note the correspondence between the extent of both the


single-photon and two-photon circuit functionality


sensitivity across the entire 500 MHz ring oscillator


structure. As previously stated, to serve as a reference


marker, this structure had been deliberately restricted to


contain only 37 active stages over its active area. This


premeditated constraint is clearly observable on both


Figure 3 (b) and Figure 4 (b), providing confirmation that


the two probing schemes are accessing the correct device


operating parameters for accurate frequency variation


mapping.


Finally, it is important to note that although TPA provides


an improvement in resolution over conventional singlephoton procedures due to its nonlinearity (i.e. the fullwidth half-maximum reduction of a squared Gaussian


point-spread function is by a factor of 2, the result


presented in this work has not yet been fully optimized and counterparts. This suggests that the expected √2 exposed. It is clear from both Figure 3 (b) and 4 (b) that


the individual stages of the ring oscillator circuit can be


resolved using both techniques; however, the TPA image


is, first of all, visually limited by the frequency drift


commonly associated with ring oscillator circuits and,


secondly, quantitatively limited by the laser wavelength


employed. For an equal comparative analysis to take place,


the experimental parameters of both technologies must be


identical or held as close as that allowable. The


preliminary nature of this investigation therefore satisfies  to serves as a successful example of the benefits to be  gained through the utilization of TPA; however, it does not  demonstrate in its entirety an optimum performance. To  begin with, the granulated vertical lines on Figure 3 (b) impede a true qualitative evaluation of the resolution  performance to take place and therefore must be  suppressed. This may be achieved by increasing the  incident 1.55µm laser power (i.e. above 4.45mW) in order  to enhance the nonlinear interaction with the circuit since  at low powers the only observable effect will be the  drifting ring oscillator frequency. By increasing the power  and hence the TPA signal, and averaging over several  frames, the interesting fluctuations of the nonlinear signal  will dominate over additional unwanted noise/circuit  variations. At present however, under closer examination, it does appear that the widths of the vertically displaced, horizontally configured ring oscillator stages in the TPA


point-spread function is by a factor of √2), the result


image are of an equal magnitude to their linear  counterparts. This suggests that the expected 2  improvement in TPA-enhanced resolution did contribute  yet remains visually suppressed by these fluctuating  frequency variations. Therefore, once this has been  remedied an improved visualization will be gained. In a  simplified approach, we altered both the contrast and  brightness of the TPA image in an attempt to further  support this statement. These results are presented in  Figure 5 (a) and (b).


(a)(a)


(b)(b)


2-


Figure 5 – (a) Image-processed two-photon frequency variation map displaying simulated contrast and brightness adjustments  and (b) its hybrid confocal overlay to serve as an alternative for improved visualization and discussion clarity.


Furthermore, since different laser wavelengths have been  used for the two techniques, an inequitable quantitative  comparison will exist. It is accurate to state that in this  example the two methodologies share a similar  performance since it suggests so both qualitatively and


quantitatively; however, if the two-photon laser  wavelength were brought closer to the silicon band-edge (all the while satisfying the energy-dependent conditions  of TPA), its resolution-enhancing performance would  dominate. For example, the lateral resolution of an


imaging system is approximately defined as Δx=λ/2NA, where λ represents the laser wavelength and NA the  numerical aperture of the system. Therefore, in this study, for a single-photon wavelength of 1.064µm and a TPA  wavelength of 1.55µm, the corresponding resolution  performance is 665nm and 685nm (including the factor of  2), respectively. This confirms the stated comparable  performance. On the other hand, for a single-photon  wavelength of 1.064µm and an adjusted TPA wavelength  of 1.2µm, the corresponding resolution performance would  be 665nm and 530nm (including the factor of 2), respectively. Therefore, after applying the appropriate  experimental conditioning to fully optimize both  techniques, it is clear that a TPA-enhanced system will  out-perform its linear alternative as a consequence of its  nonlinearity as well as its superior optoelectronic  properties.


Conclusions


In summary, we demonstrated the first observation of  nonlinear X-variation effects inside a silicon IC by  inducing TPA in the device layer of a proprietary silicon  microelectronic DUT. By monitoring the magnitude of  transistor switching time variations we were able to obtain  a frequency variation map of a 500 MHz ring oscillator  circuit. These preliminary results highlight the feasibility  of developing 2p LADA into an advanced diagnostic and  debug tool with the potential to obtain higher lateral  resolution through the utilization of TPA.


The authors would like to thank Dmitry Skvortsov and  Roy Ng of DCG Systems Inc for both helpful technical  discussions and valuable contributions towards the  experimental implementation of this work.


ReferencesReferences


[1] K. Nikawa and S. Inoue, "New laser beam testing  methods applicable to fault localization and defect  detection in VLSI devices", IEEE International  Reliability Physics Proceedings, 34th Annual, 346-354 (1996).


[2] E.I. Cole, P. Tangyunyong, C.F. Hawkins, M.R. Bruce, V.J. Bruce, R.M. Ring, and W.L. Chong, “Resistive Interconnection Localization”, ASM  International Symposium for Testing and Failure  Analysis - 27th Annual, 43-50 (2001).


[3] M. R. Bruce, V. J. Bruce, D. H. Eppes, J. Wilcox, E. I. Cole Jr., P. Tangyunyong, C. F. Hawkins, “Soft  Defect Localization (SDL) on ICs”, ASM  International Symposium for Testing and Failure  Analysis - 28th Annual, 21 (2002).


[4] E.I. Cole, J.M. Soden, J.L. Rife, D.L. Barton, and  C.L. Henderson, "Novel Failure Analysis Techniques  Using Photon Probing with a Scanning Optical  Microscope", IEEE International Reliability Physics  Proceedings - 32nd Annual, 388-398 (1994).


[5] J. Rowlette and T. Eiles, “Critical timing analysis in


V2), respectively. This confirms the stated comparable


microprocessors using near-IR laser assisted device  alteration (LADA)”, Proceedings of international test  conference, vol. 1, p.264–273 (2003).


[6] E. Ramsay, N. Pleynet, D. Xiao, R.J. Warburton, and


be 665nm and 530nm (including the factor of √2),


D.T. Reid, "Two-photon optical-beam-induced  current solid-immersion imaging of a silicon flip chip  with a resolution of 325 nm", Optics Letters 30, 26-28 (2005).


[7] K.A. Serrels, E. Ramsay, R.J. Warburton, and D.T. Reid, "Nanoscale optical microscopy in the vectorial  focusing regime", Nature Photonics 2, 311-314 (2008).


[8]  K.A. Serrels, E. Ramsay, and D.T. Reid, "70 nm  resolution in subsurface optical imaging of silicon  integrated-circuits using pupil-function engineering”, Applied Physics Letters 94, 073113 (2009).


[9] E. Ramsay, K.A. Serrels, M.J. Thomson, A.J. Waddie, M.R. Taghizadeh, R.J. Warburton, and D.T. Reid, "Three-dimensional nanoscale subsurface  optical imaging of silicon circuits", Applied Physics  Letters 90, 131101 (2007).


[10] E. Ramsay and D.T. Reid, “Investigation of the twophoton optical beam induced current effect in silicon  integrated circuits”, Optics Communications 221, 427-433 (2003).


[11] G. Woods, H. Koike, P. Vedagarbha, K. Wilsher, K. Sanchez, and R. Desplats,  “Laser-Induced Timing  Alteration in Integrated Circuits”, LSI Testing  Symposium, Osaka, Japan, 297-302 (2004).


[12] K. Sanchez, R. Desplats, F. Beaudoin, P. Perdu, S. Dudit, G. Woods, and D. Lewis, “Dynamic Laser  Delay Variation Mapping (DVM) implementation  and Applications” ASM International Symposium for  Testing and Failure Analysis -31st  Annual, 106-114 (2005).


[13] P. Perdu, R. Desplats, K. Sanchez, F. Beaudoin, D  Lewis, V. Pouget, A. Douin, and P. Fouillat, “Identification of some key parameters for  photoelectric laser stimulation of  ICs: an  experimental approach”,  IEEE International  Symposium on the Physical and Failure Analysis of  Integrated Circuits – 12th  Annual, 21-26 (2005).


[14] K. Sanchez, R. Desplats, F. Beaudoin, P. Perdu, J.P. Roux, G. Woods, and D. Lewis, “NIR laser  stimulation for dynamic timing analysis”,  Microelectronics Reliability 45, 1459-1464 (2005).


[15] K. Tamura, E. P. Ippen, H. A. Haus, and L. E. Nelson, "77-fs pulse generation from a  stretchedpulse mode-locked all-fiber ring laser," Optics Letters  18, 1080 - 1082 (1993)


[16] P. Vedagarbha, G. Woods, H. Koike, and K. Sanchez, “Laser-Induced Debug and Failure Analysis”, in  Semiconductor


Clearly these background signals represent a practical  limitation on the laser power density that can be used in the  Raman probe. Excessive heating not only produces an optical  background that competes with the Raman signal, but also  induces leakage currents that can adversely affect normal  device operation.


Theory of Laser-Thermal Imaging


The exponential signal-to-power relationship of the  background radiation was input for a model to determine the  expected signal point response. The laser input is assumed to  produce an Airy pattern appropriate for an input wavelength  of 1342 nm and a 200X objective with NA of 1.2 as utilized in  our experiments.


u n


The laser-thermal effect model assumes that the locally  induced temperature rise will be proportional to the laser


e


power density, i.e. it is assumed that thermal spreading is


S


relatively small [6]. Results for an assumed temperature rise of  200 oC indicate a factor of 3 reduction in point response width  for the laser-thermal effect as shown in Fig. 3.


0.6 Normalized Intensity0.8 1


1.2


-1


-0.5


Position (um)


Airy


Two-Photon Laser-Thermal


Figure 3:  Spot size of three image signals for a diffraction  limited input spot (1342 nm with a 1.2 NA oil immersion  objective). Airy represents reflected light signal. Two-Photon  is two-photon absorption OBIC response for high pulse power  laser. Laser-Thermal is laser induced thermal emission  response.


In imaging, the point response function is connected to image  resolution via a Fourier transform1. Thus as the point response  narrows, the image resolution improves proportionally. To  fully appreciate what this result means in terms of image  quality, our model was extended to produce the relative image  intensity for a target spatial pattern for each of the cases of a  standard (linear) reflectance imaging, a two-photon imaging, and a laser-thermal imaging. A target pattern of two closely  spaced stripes is shown in Fig. 4. Linear reflectance shows no  modulation in the response signal, i.e. the response is  1 The Fourier transform actually couples to the imaging spatial  frequency response or modulation transfer function (MTF). The common term “image resolution” loosely relates to the  MTF cut-off frequency. Other issues such as side lobes can  significantly affect image quality.


indistinguishable from that of a single wide stripe. The twophoton signal response shows a very small modulation (~10%), i.e. a vigilant observer could just discern the presence  of a pair of stripes. The modulation in the laser-thermal signal  response (~ 95%) produces an easily discernable pair of strips.


0.00


0.10


0.20


a y0.30]


0.40 a0.50 u


a 1


0.60


0.70


0.80


0.90


1.00


Two-Photon Laser Thermal Pattern


Figure 4:  Intensity versus position of three image signals as  diffraction limited spot is scanned over a pair of closely  spaced lines. Airy represents reflected light signal. TwoPhoton is two-photon absorption OBIC response for high  pulse power laser. Laser-Thermal is thermal emission  response.


-


n m


DAQ Electronics


4 3 1


a y0.2 e0.3


a八0.4


PBS


Imaging


□0.5


Optics Relay


Optics


a0.6u


Relay


p!M0.7


q0.8


Scan Mirror


Color Beam


Detector InGaAs


300


ObjectiveL


Delta Temperature (K)


「e S


Test Circuit


Lock-In Amplifier


Figure 5: Graph of improved resolution versus delta  temperature.


The analysis in Figs. 3 and 4 utilized a fixed laser-induced  temperature rise of 200 oC. Additional analysis was performed  to determine the amount of point response reduction that  occurs with variation in the change in laser induced  temperature rise or delta. Of not is that the point response


reduction only depends on the temperature delta and not the  base temperature. The analysis results are shown in Fig. 5. The point response reduces with increasing delta temperature  until it reaches a shallow minimum around a 300 oC and then  slowly rises.


Experimental Results


Figure 6 shows the basic optical and electronic configuration  used to validate the theoretical predictions. The core


人


configuration consists of our standard laser scanning


microscope system with a 1342 nm source laser, scanner,


u


imaging detector and DAQ electronics for capturing signals as


the laser is scanned along the test circuit. A 200X, NA of 1.2  oil immersion objective was used, which produced a  diffraction spot of ~ 1.0 micron at FWHM and an effective  pixel size of 0.12 micron.


The additional optical components include utilization of low  pass color filters to separate the laser and thermal optical  components and an uncooled InGaAs IR detector. The  detector aperture is defined by the detector size, ~ 1mm. The  nominal bandpass of the system is ~ 1400 to 1650 nm – limited on the lower end by the low pass filters and on the  upper end by the detector response. Currents developed in the  test circuit are sent through a lock-in amplifier to improve  SNR and collected by the DAQ electronics. Alternatively, the  InGaAs detector signal is passed through the lock-in and  detected.


Figure 6:  Block diagram of system for performing backside  laser thermal.


A first experiment test of laser–thermal imaging was  performed by using a black ceramic target. This target exhibits  strong absorption of the laser radiation, minimal thermal  spreading, strong emission of thermal radiation and resistance  to damage when heated to high temperatures. This  combination created sufficient thermal radiation that it could  be detected by the un-cooled InGaAs detector with the aid of  chopping the laser beam and a lock-in amplifier. In fact, sufficient heating occurred at some locations that the thermal  emission could be seen by eye in a darkened room.


The result is shown in Figure 7 below. The fuzzy spots in this  image correspond to high points (peaks) on the rough target  surface. We expect these locations to become hottest as they  have the lowest thermal conductivity. Hottest translates to  brightest. Several spots are observed in the image that are  approximately 1/3 of the size of the laser beam. Features  which are smaller than the diffraction limit cannot exist in a  linear, reflected-light image. Their presence clearly  demonstrates the improved resolution produced by laserthermal imaging.


0.36 um


Figure 7:  Laser- thermal image of ceramic surface. Red  circle indicates size of laser spot and contains one subdiffraction sized feature. Scale is placed around a second subdiffraction feature.


As a second experimental test, the induced leakage current in  the IC was simultaneously imaged along with a reflected light  image as the laser was scanned over the device [7]. The  experimental results are shown in Fig. 8. A very faint white  line can be seen running vertically down the center of a dark  vertical bar in the reflected light image on the right. The dark  bar is ~ 2 microns wide, so this white line is just at the  expected resolution limit of our laser scanning microscope  with the objective used.


The laser-thermal induced photocurrent image shows clearly  resolved vertical lines - two black around a white, with the  location of the white line corresponding to the location of the  white line in the reflected light image. The improved


resolution is obvious. The black lines are only 3 image pixels  wide corresponding to ~ 0.36 micron. Again, observation of  sub-diffraction sized features is consistent with the predicted  resolution improvement of laser-thermal imaging.


Faint white line


Same white line


Figure 8:  Demonstration of improved image resolution using  laser-thermal technique.


Future Efforts


The current analysis and experimental results clearly indicate  significant improvement in imaging using the laser-thermal  effect. The 1342 nm source laser used in these experiments  was dictated by application of the Raman system to imaging  through silicon devices. Clearly shorter wavelengths will  result in even better resolution, although thermal spreading  should produce a lower limit. Pulsed laser sources might be  used to overcome these limits.


Signal strength represents a limiting factor in image  acquisition times (minutes for the images shown). Use of  longer wavelength, cooled detectors should improve  acquisition times by orders of magnitude.


Finally we note that these techniques can be applied to any  laser response of an exponential character. Expansions into  chemical and biological imaging represent potential  application arenas.


Laser-thermal non-linear imaging produces a remarkable  three-fold increase in image resolution over linear, diffractionlimited imaging. The results presented in this paper are a long  distance from a practical FA tool. However, backside imaging  through silicon disallows use of shorter wavelengths for  improved image resolution. Difficult as it may be, non-linear  imaging represents one of the few options for keeping up with  ever shrinking feature sizes.


Acknowledgments


The authors would like to acknowledge their spouses and  families; some of the few people who would put up with our  unintelligible mumblings about DAQ, MTF, Airy discs and  other technical singularities.


[1] W. Denk, J. Strickler, W. Webb, Science 248 (1990) 73–


76.


[2] E. Ramsay, D.T. Reid, Optics Communications 221 (2003) 427-433


[3] V. Pouget, et al., 35th ISTFA, (2009) 268-71


[4] R. A. Falk, T. Pham, G. Albright, Proc. 35th ISTFA, (2009) 65-72


[5] S.L.Tan, et al., Proc. 33rd ISTFA, (2007) 81-85


[6] P. Tangyunyong, D. Benson, E.I. Cole, Jr., J. Vac. Sci. Technol. B 18(2000) 2820-2825


[7] B.P. Richards, P.K. Footner, The Role of Microscopy in  Semiconductor Failure Analysis, Oxford University  Press, Oxford, 1992.


# Mobile Diffractive Solid Immersion Lens Design for Backside Laser Based Fault Localization


Mobile Diffractive Solid Immersion Lens Design for   Backside Laser Based Fault Localization


SH Goh1, JY Cho2, Jeffrey Lam1


1GLOBAL FOUNDRIES Singapore, Technology Development, New Technology Prototyping   2GLOBAL FOUNDRIES Singapore, Quality and Reliability Assurance, Failure Analysis


JCH Phang


Centre for Integrated Circuits Failure Analysis, National University of Singapore


In this paper, a mobile Diffractive Solid Immersion Lens (mDSIL) design is proposed to enhance spatial resolution for  backside laser fault isolation techniques. By allowing for  multiple failure sites analysis using a single DSIL, this design  improves conventional static DSIL directly fabricated on  silicon substrate. The feasibility of mDSIL is demonstrated  experimentally and the resolution performance is shown to be  comparable to a static DSIL.


Backside laser based fault isolation techniques have been  adopted widely as mainstream methods for electrical failure  analysis (EFA) [1, 2, 3]. To ensure localization effectiveness  for 45 nm and below technologies, there are strong  motivations to scale down optical spatial resolution [4, 5]. In  principle, far field optical resolution is limited by diffraction  and the achievable spatial resolution using typical NearInfrared (NIR) wavelength laser is approximately 1 m. This is  far larger than the critical defect size of 22.5 nm at 45 nm  technology node [6].


Solid Immersion lens (SIL) technology has proven to be an  effective solution. There are two main categories of SIL  technology, namely Refractive solid immersion lens (RSIL) [7, 8] and Diffractive solid immersion lens (DSIL) [9, 10]. RSIL  enhances collection efficiency and numerical aperture (NA) through favorable light refraction on the spherical interface of  the lens. Unlike RSIL, DSIL works by the principle of  diffractive optics. It involves creating concentric patterns on  silicon (Si) substrate to control the bending of light to enhance  collection efficiency. Although RSIL is more adopted by  industry, DSIL has its advantages. Unlike RSIL which is  usually 1- 2 mm in height, DSIL has a small thickness. This  allows the use of a high NA, short working distance objective  lens. Therefore, a higher effective NA can potentially be  achieved.  Another advantage of DSIL lies in its fabrication. DSIL can be fabricated conveniently using readily available  Focused Ion Beam (FIB) and Reactive Ion Etcher (RIE) found  in a typical FA laboratory [10].


However, a major drawback of a conventional DSIL is its  immobility. A separate DSIL has to be created either when the  existing DSIL is fabricated in the wrong location due to  alignment errors or when there are multiple failing sites for  analysis. The resolving power of DSIL is proportional to its  diameter. Since a larger diameter DSIL requires longer  fabrication time, it is usually not practical to spend an hour to  create a large DSIL just for a single analysis. Furthermore, the  optical quality is not guaranteed, especially when the FIB and  RIE tools are poorly maintained.


To overcome these limitations, we propose a mobile DSIL  design in which case, a high performance DSIL only requires  to be fabricated once and it can be reusable. In this paper, we  demonstrate the feasibility of mDSIL for laser imaging and  investigate its optical performance qualitatively.


Basic DSIL design parameters


A binary-phase DSIL which consists of two-level profile  works similar to a Fresnel Phase plate. Unlike a Fresnel zone  plate where rays that will cause destructive interference are  blocked so as to ensure only constructive interference at the  focus, a fresnel Phase plate introduces a π phase change to the  destructive rays. Although a binary- phase DSIL is usually  created due to fabrication simplicity, the tradeoff is diffraction  efficiency of approximately 40% [11]. The remaining 60% of  incident light is not transmitted to the focal focus. The  diffraction efficiency can be increased by increasing the  number of levels.


There are two main design parameters that determine the  concentric profile of DSIL, namely lens diameter D and focal  depth kd where k is an arbitrary constant and d is the substrate  thickness as shown in Fig. 1. It can be seen from Fig. 1(a) that  as D increases, the semi-collection angle  increases. Therefore, D directly affects resolution. Diffraction at the lens  interface results in a virtual focus at depth k1d. The semiaperture angle  determines the minimum required matching  objective NA for reflected light collection. For k=1, 1 =1‟. This is similar to a centric RSIL design. Fig. 1(b) illustrates  further that under the same substrate thickness d, for a larger k  value such that k2 > k1, 2‟ < 1‟and a smaller matching  objective NA is required. Therefore, k determines the focal


an68


SarAe


Fig. 1. Schematic design of a DSIL with designed focal point  at (a) k1d and (b) k2d where k2 > k1 and d is the thickness of  silicon substrate.


depth and backing objective NA. By using a suitable k, the  DSIL can perform similar to an aplanatic RSIL design. However, unlike an RSIL, every designed focus is SA-free in a  DSIL.


Mobile DSIL (mDSIL) Design


The top side of a 1 mm x 1 mm blanket Si is polished to a  roughness of approximately 0.25 m using mechanical


lapping. Subsequently, the method of Gallium (Ga) implantation to form a mask pattern and differential CHF3 ion  etching [10] is used to fabricate the DSIL. Fig. 2 shows the


DSIL0


reflected laser image of the binary lens under 50X objective


Sample


lens.  For the IC sample, the back Si substrate is polished to a  thickness such that the total height d, comprising of IC and  DSIL sample thickness equals the designed focal plane at A as


kd


shown in Fig. 3. k is designed to be 1.


For optical coupling and navigation of mDSIL, a clear aperture  structure attached to a micromanipulator is used. The backing  objective lens and mDSIL are decoupled in this configuration. Optical oil (Refractive Index: ~1.515) is used in between the


-Foam


lens and sample interface to enhance optical coupling.  Fig. 4  shows a schematic of mDSIL attached on the aperture


Clear aperture structure


structure using epoxy wax. The clear aperture is larger than the


Smpl DSU


Wax


diameter of DSIL for maximum collection efficiency. In order  to avoid lens crack, foam is used in the structure design for  gradual compression. This method is effective to a Si thickness  as thin as 60 m.


Besides attaching an mDSIL to a micromanipulator, it can also  be used as a standalone which we term a „stick-on-mDSIL‟ in  this paper. In this case, it makes use of the natural adhesion  force between the non-volatile liquid and flat Si surfaces. Although there are tradeoffs in reduced optical coupling, it is  an economical way to implement mDSIL for quick resolution  enhancement on an existing optical system.


70um


Fig. 2. Reflected laser image of a fabricated DSIL on blanket  silicon.


Fig. 3. Schematic of mDSIL design with virtual focus at kd  where d is the total thickness of DSIL and sample substrate.


Fig. 4. Schematic design of an mDSIL attached to an aperture  structure.


A commercial scanning laser optical microscope system and  1340 nm wavelength laser is used in all the experiments. It  should be noted that the micron bars in the reflected laser  images do not apply for features within DSIL.


A.  Feasibility of mDSIL concept


A 170 m diameter DSIL is fabricated on a 130 m thick, 1.3  mm x 2 mm blanket Si. It is designed for a device substrate


thickness of 95 m at k=1.  At this design, the effective NA  achievable is approximately the product of objective NA and  refractive index of Si (nSi). The theoretical achievable NA and  resolution is 1.24 and 660 nm respectively using a minimum  backing objective NA of 0.35. Fig. 5(a) shows a laser reflected  image of mDSIL on top of a backside IC sample. There are six  other DSIL on the same DSIL sample but they can be ignored  in this work. The DSIL of interest is indicated by an arrow. The DSIL sample is approximately 95-100 m thick. Fig. 5(b) shows a schematic of the dummy features of interest in the IC  sample. In this experiment, a „stick-on-mDSIL‟ is applied.


Fig. 6(a) shows the backside reflected laser images at the  device focal plane captured using 20X objective lens (0.25  NA) at location A which is near the edge of die.


Fig. 5. (a)Reflected laser image of mDSIL placed on top of  backside IC sample and (b) schematic of dummy structure of  interest.


(c)


(d)


Fig. 6. Backside reflected laser image at (a), (b) device and (c), (d) DSIL focal planes. (a) ,(c) is at location A and (b), (d) is at location B. 20X objective lens is used. Location A is at  edge of die and location B is away from the edge.


Fig. 7. Backside reflected laser image (a) without DSIL at  digital zoom 3 and with DSIL  using 50X objective lens (0.4  NA) at (b) digital zoom 1 and (c) digital zoom 2


Fig. 6(b) shows the image at location B which is away from  the edge. The features underneath the DSIL are not resolvable. Fig. 6(c) and 6(d) shows the images at the DSIL focal plane at  location A and B respectively. The spatial resolution of the  images is enhanced and the dummy features clearly resolved. There is also additional magnification of approximately 3.5  times.


Fig. 7(a) shows a reflected laser image of the dummy  structures captured on a 50X objective lens (0.4 NA). It is  obvious that the structures cannot be resolved. The structures  can be clearly resolved using stick-on-mDSIL as shown in Fig. 7(b) and 7(c). This is expected because the 1.32 m pitch is  well within the theoretical resolving power of the DSIL design.


B.  Static DSIL and mDSIL


The same dimension DSIL is used to compare the optical  performance between a static DSIL and stick-on-mDSIL. Fig. 8(a) and 8(b) shows the case of a DSIL directly formed on Si  substrate and mDSIL respectively imaging on the same  dummy structures. It is evident that in both lenses, the results  are similar although there are slight differences in  magnification due to deviations in sample thicknesses. However, it should be noted mDSIL requires about 30% more  laser power for imaging. This is mainly due to poorer optical  coupling and possible difference in lens quality. Using the  clear aperture structure, this degradation is reduced to about


Fig. 8. Backside reflected laser image using (a) DSIL directly  fabricated on IC sample and (b) mDSIL at 50X digital zoom 2.


20%. This might pose challenges for laser stimulation  techniques. However, the issues of poor transmission through  DSIL can be overcome by using either blazed DSIL [12].


C.  Qualitative Analysis of optical performance


Fig. 9(a) shows the schematic of a backside Si resolution target  sample which has line/ space pitch structures ranging from 400  nm to 2000 nm with 200 nm increments. These are 50% line  and space pitch. The sample thickness is about 85 m. The  smallest resolvable pitch structure is commonly used as a  figure of merit for the qualitative analysis of the resolution  performance of a microscope system. Fig. 9(b) shows the  reflected laser image using 1340nm wavelength laser and high  NA 100X objective lens (0.7 NA). The smallest resolvable  pitch is 1200 nm. Fig. 9(c) and 9(d) show that the 170 m  diameter mDSIL can easily resolved the 1000 nm pitch  features (indicated by a box). This is expected because the  theoretical resolution achievable is approximately 660 nm. Fig. 9(d) also shows that with the clear aperture, there is slight  enhancement in image contrast due to reduced glare with  better optical coupling. The laser power required is about 10% lower in the case of Fig. 9(d) as compared to Fig. 9(c). The  overall quality of images is poorer in both cases because of  increased spherical aberrations at 10 m away from intended  focal plane.


Another mDSIL is fabricated on a 1 mm x 1 mm blanket Si. The diameter is 150 m. It is designed for a device


Fig. 9. (a)Schematic of features on backside Si resolution


target. Backside reflected laser image using (b) 100X


objective lens (0.7NA) without DSIL at digital zoom 8, 50X  objective lens (0.4NA) at digital zoom 2 with (c) stick-onmDSIL and (d) mDSIL with clear aperture. The boxed up  region indicates 1000 nm pitch structures.


substrate and mDSIL thickness of 120 m and focal plane at  k=1. A theoretical spatial resolution of 410 nm can be  achieved in this configuration. The better resolution compared  to the 170 m diameter DSIL comes from the reduced  designed focal plane such that collection angle is larger. Fig. 10(a) and 10(b) show the results captured using the 50X  objective lens (0.4 NA) without DSIL and with mDSIL  respectively. The mDSIL is compressed with the clear aperture  structure. The 0.3/0.4 m line/space structures can be resolved  clearly. In this experiment, the final thickness is approximately  15 m lower than designed focal plane.


Fig. 10. Reflected laser image captured using 50X objective (0.4 NA) (a) without DSIL at digital zoom 4 and with mDSIL  and clear aperture at (b) digital zoom 1and (c) digital zoom 2


Future potential of mDSIL


A DSIL with good resolving power of 0.4 μm has been  reported on a diameter of 200 m [10]. Further resolution  enhancement has been demonstrated by fabricating and  distributing appropriately a large number of pinholes over the  DSIL [13, 14]. These pinholes are known as photon sieves. In  general, the enhancement factor is d/ w where d is the diameter  of the pinhole and w is the Fresnel zone width. A resolution of  200 nm resolution was reported. These advanced innovations  can be leveraged by mDSIL for better performance.


Besides optical performance, there is another potential  advantage for mDSIL over RSIL. For example, stick-onmDSIL allows access to die corners which is difficult using a  commercial RSIL. This is illustrated previously in Fig.6 (a) where the lens is so close to the edge that a small part of it is  not covering the device (portion with darker shade). For better  field of view coverage, an array of DSIL can be created and be  simply „pasted‟ on the Si substrate for enhanced resolution as  shown in Fig. 11. This is extremely useful for scanning optical  microscope with inverted optics. Taking into account that a 3  X 3, 200 m diameter mDSIL array, a 1 mm blanket Si sample  is sufficient. In this way, navigation of mDSIL to the intended  region is easier. Minimal interfacial issues are expected based  on previous experimental data presented.


Practical Challenges of mDSIL


RSIL technology has been optimized for laser based FA tools  applications and the best achievable theoretical resolution at  the aplanatic configuration (~nSi2 enhancement factor) is  approximately 220 nm based on 1340 nm wavelength laser. This is equivalent to an effective NA of close to 2.9 based on  backing objective of 0.24 NA.


Fig. 11. Schematics of mDSIL array concept.


The performance of mDSIL is not competitive to that of RSIL  at the moment due to physical constraints in creating an  equivalent large lens of approximately 1 mm in diameter. Firstly, using the current method of fabrication, this will take  hours on the FIB. The reason is because of beam current drift  and spot size limitation to create the fine outer rings of DSIL  that can potentially affect the symmetry of DSIL. For the  latter, publications have reported the potential of using  picoseconds (ps) and femtoseconds (fs) pulsed lasers for  nanomachining materials [15]. By optimizing wavelength and  pulse width, sub-100 nm range features can be created. Common continuous wave or long-pulsed microsecond lasers  are unfavourable because of the extensive heat diffusion into  the material.


Both resolution and sensitivity are critical in fault localization  tools using laser stimulation. Although the sensitivity of laser  induced signals have not been characterized in this work, poor  laser transmission is evident as one of the key challenges of  mDSIL based on the increased laser power of 10-30% required  for imaging compared to conventional DSIL. One effective  solution is the use of blazed instead of a binary DSIL design. This can increase the diffraction efficiency from approximately  40% to 88% [12].


The other challenge lies in the fabrication of DSIL using  current dual process. The optical quality of the lens heavily  depends on the consistency and precision of FIB and RIE. Often in FA laboratories, ion beam stability and etch  consistency are not critical as long as the physical failure  analysis (PFA) objectives are achievable. Fig. 12 shows a   portion of a DSIL profile. The lens surface quality shown in  Fig. 12(a) is more uniform and less rough than that shown in  Fig. 12(b). There are two reasons for this. Firstly, in the Ga  implantation process, the ion beam fluctuates as it scans. This  is evident by the horizontal non-continuous lines observed in  Fig. 12(b). More frequent maintenance might be required in  order to ensure consistent DSIL optical quality. Secondly, the  sample etch time could be too long and coupled with the nonuniform implantations, the surface roughness becomes worse. Process optimization might resolve this part.


200μm


1mm


-of tam(a)


Fig. 12. SEM image between stable and unstable system.


→


In this work, we show that it is possible to create a workable  mDSIL whose resolution can be comparable to a conventional  static DSIL. It can be used for multiple failing sites analysis  and is reusable. mDSIL can either be used as a standalone lens  sample or be incorporated into a clear aperture structure for  better optical coupling. The best resolvable resolution  achieved based on a small diameter DSIL design of 150 m  and 0.4 NA backing objective is about 400 nm.


International


(2004)


# Quantitative, nanoscale free-carrier concentration mapping using terahertz near-field nanoscopy


Quantitative, nanoscale free-carrier concentration mapping using terahertz nearfield nanoscopy


J. Wittborn and R. Weiland


Infineon Technologies AG, Munich, Germany


A. J. Huber


Neaspec GmbH, Martinsried, Germany


F. Keilmann


Max Planck Institut of Quantum Optics and Center for NanoScience, Garching, Germany


R. Hillenbrand


CIC nanoGUNE Consolider, Donostia – San Sebastian, Spain  Ikerbasque, Basque Foundation for Science, Bilbao, Spain


We use ultra-resolving terahertz (THz) near-field microscopy  based on THz scattering at atomic force microscope tips to  analyze 65-nm technology node transistors. Nanoscale  resolution is achieved by THz field confinement at the very tip  apex to within 30 nm. Images of semiconductor transistors  provide evidence of 40 nm (λ/3000) spatial resolution at 2.54  THz (wavelength λ = 118µm) and demonstrate the  simultaneous THz recognition of materials and mobile carriers  in a single nanodevice. The mobile carrier contrast can be  clearly related to near-field excitation of THz-plasmons in the  semiconductor regions. The extraordinary high sensitivity of  our microscope provides THz near-field contrasts from less  then 100 mobile electrons in the probed volume.


Background


Measurement of carrier- or doping-concentration of  nanostructured devices still remains a challenge for the  semiconductor industry. Secondary ion mass spectroscopy (SIMS) and spreading resistance profiling (SRP) are useful  methods for measuring dopant concentration and carrier  concentration, respectively, but are limited to 1-dimensional  depth profiles. In addition, both these methods require  relatively large, laterally homogenous sample areas. Atom  probe microscopy faces the opposite problem; it yields 3-dimensional measurements of the nanoscale dopant  concentration [1] but the maximum sample size limits its use  for many failure analysis applications. Scanning probe  microscopy (SPM) based methods [2] such as scanning  capacitance microscopy (SCM) [3, 4, 5, 6, 7], scanning  spreading resistance microscopy (SSRM) [8, 9] and scanning  microwave microscopy (SMM) utilizes different tip-sample  interaction mechanisms to yield 2-dimensional doping maps.


Spatial resolution and detectable doping range varies between  the methods.


Here we demonstrate the benefits of near-field nanoscopy. We  use laser light at 2.54 THz (wavelength λ = 118µm) scattering  at metallised atomic force microscope tips to achieve 2-dimensional, quantitative mapping of carrier concentration in  the range 1016 to 1019 carriers/cm3 at a spatial resolution of 40  nm (λ/3000). Nanoscale resolution is achieved by THz field  confinement at the very tip apex to within 30 nm. Images of  65-nm technology node CMOS transistors demonstrate the  simultaneous THz recognition of materials and mobile carriers  in a single nanodevice.


Electromagnetic radiation at THz frequencies addresses a rich  variety of light-matter interactions because photons in this low  energy range can excite molecular vibrations and phonons, as  well as plasmons and electrons of non-metallic conductors [10, 11, 12, 13]. Consequently, THz radiation offers intriguing  possibilities for material characterization currently motivating  major efforts in the development of THz imaging systems [14, 15]. Diffraction unfortunately limits the spatial resolution to  about half the wavelength which is in the order of 100 μm. For  this reason, THz mapping of micro- or nanoelectronic devices  could not be attained. A promising route to break the  diffraction barrier and to enable sub-wavelength scale imaging  is based on fine-focusing of THz radiation by millimeter-long  tapered metal wires [16, 17, 18, 19]. Acting as antennas, the  wires capture incident THz waves and convert them into  strongly confined near fields at the wire tip apex [20]. When  this confined field becomes modified by a close-by scanned  sample, the scattered radiation carries information on the local  dielectric properties of the sample [18, 21, 22]. THz images  can be obtained by recording the scattered radiation by a  distant THz receiver. Attempts of realizing such THzscattering near-field optical microscopy (THz-SNOM), however, suffered from extremely weak signals and faint  material contrasts owing to strong background scattering.


Novel probes for THz focusing are thus a subject of current  interest [23, 24]. In 2008, Huber et al. [25, 26] introduced THz  near-field microscopy achieving unprecedented resolution of  about 40 nm, paired with extraordinarily high image contrast  and acquisition speed. This is enabled by interferometric  detection of THz radiation scattered from cantilevered atomicforce-microscope (AFM) tips. Building on this pioneering  work we demonstrate THz mapping of mobile carriers within a


single nano-device and its relevance for semiconductor


θ 2


technology.


mirrord↑M


parabolic


beamTheory


splitter


The optical near-field scattering, depending on refractive index


mirror


and absorption of the sample, can be enhanced by phonon  polaritons in polar dielectrics or plasmon polaritons in metals


c.w.THz laser


and doped semiconductors [27]. Using a wavelength near the  polariton resonance of the material of interest thus causes  sharp contrast between this and other materials.


bolometer


A dipole model for the field scattered by the tip that has  proven to agree well with experimental results has been  developed and is thoroughly described in a paper by Keilmann  and Hillenbrand [21].


The essential ingredient to nanoscale resolved THz near-field  microscopy is a strongly confined THz near field for  generating highly localized scattering. Nanoscale near-field  confinement can be achieved by plane-wave illumination of a  conical metal tip, similar to visible [28] and infrared [29] frequencies. Strong confinement as well as an about 25-fold  field enhancement (compared to the incident field) are  essentially caused by the lightning-rod effect [30]. We note  that because of the short tip length (L << λ), geometrical  antenna resonances [16, 23] can be neglected. Also, dielectric  plasmon resonances of a metal tip are absent at THz  frequencies.


The experimental set-up


Our experimental set-up basically consists of a home-built  AFM combined with a THz laser light source and  interferometric detection of the scattered light.


We use AFM-tips (L  20 μm) with a Pt metallization of about  20 nm thickness (Mod. CSC37/Ti-Pt, Mikromasch). While the  sample is scanned in conventional AFM mode, both the tip (with curvature radius of about 30 nm) and the cantilever are  illuminated with a focused laser beam at a frequency of 2.54  THz from a continuous-wave CH3OH gas laser (Mod. SIFIR50, Coherent), at a power of about 5 mW (Fig. 1). THz  imaging is performed by collecting the back-scattered  radiation with a parabolic mirror. For detection we use a  Michelson interferometer featuring a 23 µm thick polyethylene  beam splitter at 45° incidence. Interferometric detection offers  the advantage of signal amplification which is crucial for  measuring the back-scattered THz radiation with a high signalto-noise ratio at reasonable integration times less than 100 ms  per pixel. As THz detector we use a hot-electron bolometer (Mod. RS1-5T, Scontel). In order to eliminate background


scattering the AFM is operated in dynamic mode where the  cantilever oscillates at its mechanical resonance frequency Ω,here at 35 kHz, with amplitude of about 100 nmpp. The  bolometer signal is subsequently demodulated at harmonic  frequencies nΩ (with n = 2 or 3) yielding a background-free  THz signal amplitude sn [21, 31].


Figure 1: Scheme of our experimental setup based on an  AFM: A laser emitting a monochromatic beam at 2.54 THz is  used for illuminating a cantilevered AFM tip and  interferometric detection is used for recording the  backscattered THz radiation simultaneously with the AFM  topography.


Sample preparation


Samples were prepared for imaging by cleaving and  mechanical polishing to the cross-section of interest. No  further sample preparation such as etching or metal-coating  was necessary [32].


Terahertz near-field nanoscopy


By imaging a polished cross section through a 65-nm  technology node CMOS transistor we demonstrate the  simultaneous recognition of materials and free carriers by THz  near-field microscopy. While the AFM topography (Fig. 2a) only shows some depressions where metal contacts (Cu, W) were differently polished than SiO2, the THz image (Fig. 2b)


We use AFM-tips (L≈20 um) with a Pt metallization of about


clearly recognizes seven transistors manufactured in Si, with  polycrystalline Si gates, and with SiO2 as insulating material. The THz contrast can be clearly related to the different  materials composing the transistors as we verify by scanning  electron microscopy (SEM) of a similar sample where  decoration etching was employed to highlight the different  materials (Fig. 2d). We find that regions with metals or highly  conductive semiconductors appear brightest in the THz image, the lowly doped semiconductors darker, and the lowrefractive-index oxides darkest, similar to earlier findings of  scattering near-field microscopy at optical and infrared  frequencies [21, 33]. This near-field contrast can be explained  by dipolar near-field coupling between tip and sample which  predicts higher signals s2 for materials with higher dielectric  values.


Near-field microscopy at THz frequencies particularly enables d


us to recognize mobile carriers and their distributions, in a


concentration range centrally important for semiconductor


science and technology (n = 1016 to 1019 carriers/cm3) where


visible and infrared methods lack sensitivity. This sensitivity


can be clearly seen from the strong THz signal variations Cusib2w Sisingle transistor within the Si substrate of the device structure shown in Fig. 2a. e


THz


IR


We observe a decreasing THz signal just below the transistors


T1.0 and a local maximum at 500 nm depth. After passing a second 6u


n=1019cm-3


minimum at about 900 nm depth, the THz signal reaches a


IS constant level on intrinsically doped Si. A comparison with the HZ


1018


nominal mobile carrier concentrations (the numbers in Fig. 2b 10.5-1017 and c are from device simulations) provides clear evidence 01016wthat the THz contrast maps the mobile carrier distribution with u


nanoscale resolution. For comparison we also show an infrared


near-field image taken with a CO2 laser at λ near-field image taken with a CO2 laser at λ≈11 um (Fig. 2c). 11 μm (Fig. 2c).


一2.545102850


It does not exhibit signal variations below the transistors.


frequency (THz)


To explain the THz contrast in the theoretical framework


mentioned above, we calculate the frequency-dependent THz


signal s2 (Fig. 2e), between a metallic sphere and an extended


Si surface where the mobile carrier response is described by a


Drude term which depends on the mobile carrier concentration


n [34, 35]. The calculated spectra have highest THz signals at


low frequencies and a shape which can be assigned to the nearfield coupling between the tip and the mobile carrier plasmons image (c) (2 ≈ 11 um; taken for comparison) clearly in the Si sample.


Figure 2: THz near-field microscopy of a polished cut through  a multiple-transistor device structure. AFM topography (a) and simultaneously acquired THz near-field image (b). The  varying THz signal within the Si substrate reveals the different  mobile carrier concentrations n indicated by numbers  obtained from device simulations. The infrared near-field  image (c) (λ  11 μm; taken for comparison) clearly  demonstrates that only with THz illumination the varying freecarrier concentration can be recognized. The SEM image (d)


of a similar but decoration-etched sample validates that the  THz image distinguishes different materials and the single


100nm


transistors. The rectangle in 2a and b marks the zoom-in area  depicted in Fig. 4a. In 2e the THz signal amplitude s2 calculated for n-doped Si as a function of the illumination  frequency is shown.


With increasing n, the spectral signature shifts to higher


500 nm


frequencies. Interestingly, a minimum near the plasma


0nm


frequency is predicted, which occurs at 2.54 THz (red line in


b


Fig. 2e) for n Fig.2e) for n≈2.1017cm3. A minimum is indeed observed in 2·1017cm-3. A minimum is indeed observed in


max


the THz image (Fig. 2b), at a depth of 900 nm below the  transistors where the designed concentration gradient assumes  a value of n


1018a value of n≈2.1017cm-3. 2·1017cm-3.


In Fig. 3 a comparison between a simulation of the transistors  1017


net doping and a terahertz near-field nanoscopy image is  shown, as well as a line profile through the center of the gate


n≈1016cm-3


min


(along the white, dashed line) showing the normalized THz


signal. It can be noted that the image and line profile both  correspond well to the carrier concentrations given by the


simulation. This good agreement between design, experiment  and theory enables immediate applications of THz near-field


microscopy in semiconductor science and technology. Owing  to the distinct relation between THz-plasmons and carrier


1017


concentration, our results open the door to quantitative mobile  carrier profiling at the nanometer scale. The capability of


n=1016cm-3


quantifying relevant mobile-carrier distributions with


nanoscale lateral resolution could be augmented by improving  the model and by employing broadband THz spectroscopy


[36].


b c


Figure 3: Comparison of the THz near-field nanoscopy image  with simulation. Please note that the carrier concentrations  indicated by the simulation (a) can be clearly resolved in both  the THz image (b) and in the line profile (c) through the center  of the gate, as marked by the dashed white line.


Further evidence of the values of THz near-field microscopy is  provided by scanning a single transistor (marked in Fig. 2a and  b) at reduced pixel size. Figure 4 shows a 65-nm technology


40 nm


node transistor. In (a) a terahertz near-field nanoscopy image  is shown. Note that the poly-Si gates, NiSi metallization, as


1021


well as the source- and drain-diffusions can be clearly outlined! In (b) a line profile along the dashed, black line in (a) through the center of the gate shows a sharp signal increase  from the low-refractive-index material SiO2 to the metallic


NetDeping


NiSi gate contact. Due to the smooth sample surface (see Fig.


Segned Log (ern-30 32


2a) we can exclude any topography-related artifact and also


142


prove the pure dielectric origin of the THz contrast. This


8


2.10


allows us to unambiguously determine a near-field optical


6.84-5-4长%


resolution of about 40 nm (λ/3000), defined as the distance


-12.00


between 20% and 80% of the increase from minimum to


-15.2-非放


maximum THz signal. In (c) a transmission electron


-21.4


microscopy (TEM) image of a transistor from the same device


1016cm-3


is shown for comparison. The component material and an outline of the source- and drain-diffusions are indicated in the  image. The comparison between TEM and high-resolution  THz image clearly verifies the capability of THz near-field  microscopy to map the basic entities of the transistor: source, drain and gate. The metallic NiSi is more or less opaque to the  electron beam, and thus appears as black areas in this high  contrast TEM image.


c


100 nm


40 nm↓


poly-SiSiN


siO2


200 nm


300 nm


SourceDrain Si


TEM


0.51.0


NiSi


SiO2


Figure 4: 65-nm technology node CMOS transistor: (a) THz near-field nanoscopy image. (b) Line profile demonstrating the 40 nm


norm. THz signal


resolution, defined as the 20% to 80% signal increase distance. (c) TEM image of a transistor from the same device as shown in the  THz near-field nanoscopy image.


In the THz image on the other hand, a gradient in signal within  the NiSi layer can be observed. This is probably caused by the  interaction depth of the THz nanoscopy of about 40 nm which  averages the signal from the relatively rough Si-NiSi interface. Furthermore, we find that between the NiSi source and drain  contacts (black parts in the TEM image) the THz signal level  reaches an intermediate value. According to our calculation in  Fig. 2e, this indicates a mobile carrier concentration in the  order of 1018 cm-3 which is in good agreement with results  from device simulations. Obviously, THz near-field  microscopy allows for quantitative probing of mobile carriers  in the 65 nm wide region between source and drain. In  combination with future spectroscopic extensions [17, 18, 19, 22, 36, 37, 38] ,this possibility could open the door to even  measure the carrier mobility in this most important part of  nanoscale semiconductor devices.


Comparison with SCM and SSRM


For comparison, the same sample was imaged using SSRM  and SCM, the two most widely used, SPM based methods for  2-dimensional carrier concentration mapping. In Fig. 5a a  SSRM image is shown, demonstrating the excellent spatial  resolution achievable [9]. However, it also shows the lack of  sensitivity at lower carrier concentration, as well as its  completely missing material contrast. Moreover, even though  SSRM in principle can give quantitative results, it is for real  failure analysis samples seldom possible to achieve this due to  sample preparation complications. The SCM image in Fig. 5b  demonstrates the capability of SCM of differentiation between  p- and n-doped areas, and even though its spatial resolution is  limited compared to SSRM it is comparable to that achieved  using THz or IR s-SNOM. Moreover, sub-10 nm resolution as  well as quantitative measurement using SCM has been  reported [7].


Figure 5: In (a) an SSRM image is shown, demonstrating its  high spatial resolution. In (b) an SCM image is shown – demonstrating its p- and n- doping differentiation.


Discussion


An intriguing consequence follows from the sensitivity of our  setup to mobile carrier concentrations in the range 1017 - 1018 cm-3, evident from the THz contrast shown in Fig. 4a. Since  the spatial resolution of 40 nm infers [30] that the volume  probed by the THz near-field is about (40 nm) [12], we  conclude that an average of less than 100 electrons in the  probed volume suffices to evoke significant THz contrast. This  opens the fascinating perspective that straightforward  improvements of the current setup could master THz studies of  single electrons - and in conjunction with ultrafast techniques  even their dynamics. Moreover, THz near-field microscopy  seems predestined to study also other charged particles and  quasiparticles in condensed matter—for example in  superconductors, low-dimensional electron systems or  conducting biopolymers—which possess intrinsic excitations  at THz quantum energies and thus should exhibit resonantly  enhanced THz contrast. Also biological molecules and cellular  entities may be possible to investigate using THz nanoscopy.


We succeeded in quantitative mapping areas with various  materials, as well as free carrier concentrations between 1016 and 1019 carriers/cm3. The capacity of THz near-field


nanoscopy to perform quantitative studies of local carrier  concentration and mobility at the nanometer scale gives it the  potential to find many applications within semiconductor  industry and research.


Financially supported by BMBF within the NanoFutur  program,


grant


no.


03N8705,


Deutsche  Forschungsgemeinschaft Clusters of Excellence “Nanosystems  Initiative Munich (NIM)” and “Munich-Centre for Advanced  Photonics (MAP)”, and Etortek Nanotron project from the  Government of the Basque Country. Angela Collantes (Infineon) is acknowledged for TEM imaging, and Stephan  Schömann (Infineon) is acknowledged for SSRM imaging.


[1] Alvis, R. and Kelly, T. F., Microscopy Today, September  2008, pp. 6-11.


[2] Schweinböck, T., Schömann, S., Alvarez, D., Buzzo, M., Frammelsberger, W., Breitschopf, P., and Benstetter, G. “New trends in the application of Scanning Probe


Techniques in Failure Analysis”, Microelectronic


reliability, Vol. 44, (2004), pp. 1541-1546.


[3] Born, A. and Wiesendanger, R., “Scanning capacitance  microscope as a tool for the characterization of


integrated circuits”, Applied Physics A, Vol. 66, (1998), pp. 421-426.


[4] Anand, S., “Another Dimension in Device


Characterization – Scanning Capacitance Microscopy of  InP-Based Laser Structures”, Circuits & Devices, March, (2000), pp. 12-18.


[5] Zimmerman, G., Born, A., Ebernsberger, B., and Boit,


C., “Application of SCM for the microcharacterization  of semiconductor devices”, Applied Physics A, Vol. 76, (2003), pp. 885-888.


[6] Benstetter, G., Breitschopf, P., Frammelsberger, W.,


Ranzinger, H, Reislhuber, P., and Schweinböck, T.,


“AFM-based scanning capacitance techniques for deep  sub-micron semiconductor failure analysis”,


Microelectronic reliability, Vol. 44, (2004) pp. 1615-


1619.


[7]  Kikuchi, Y., Kubo, T., and Kase, M., “Quantitative Ultra  Shallow Dopant Profile Measurement by Scanning


Capacitance Microscope”, FUJITSU Sci. Tech. J., Vol. 38, No. 1, (2002) pp. 75-81.


[8] De Wolf, P., Clarysse, T., Vandervorst, W., Hellemans, L., Niedermann, Ph., and Hänni, W., “Cross-sectional


nano-spreading resistance profiling”, J. Vac. Sci.


Technol. B, Vol. 16(1), (1998), pp. 355-361.


[9] Schömann, S. and Alvarez, D., “Doping mapping by


SSRM – reaching maturity and sub-10nm resolution”,


Proceedings from the 30th International Symposium for  Testing and Failure Analysis, (2004), pp. 346-349.


[10] Kuzmany, H., Solid-State Spectroscopy. Springer:


Berlin, 1998


[11] Ferguson, B.; Zhang, X. C. Nature Materials (2002), 1, pp. 26-33.


[12] Mittleman, D., Sensing with Terahertz Radiation.


Springer: Berlin, 2003.


[13] Tonouchi, M. Nature Photonics (2007), 1, pp. 97-105.


[14] Chan, W. L.; Deibel, J.; Mittleman, D. M. Reports on


Progress in Physics (2007), 70, 1325-1379.


[15] Withayachumnankul, W.; Png, G. M.; Yin, X. X.;


Atakaramians, S.; Jones, I.; Lin, H. Y.; Ung, B. S. Y.;


Balakrishnan, J.; Ng, B. W. H.; Ferguson, B.; Mickan, S. P.; Fischer, B. M.; Abbott, D. Proceedings of the IEEE (2007), 95, pp. 1528-1558.


[16] Matarrese, L. M.; Evenson, K. M. Applied Physics


Letters 1970, 17, pp. 8-9.


[17] van der Valk, N. C. J.; Planken, P. C. M. Applied


Physics Letters (2002), 81, pp. 1558-1560.


[18] Chen, H. T.; Kersting, R.; Cho, G. C. Applied Physics


Letters (2003), 83, pp 3009-3011.


[19] Chen, H. T.; Kraatz, S.; Cho, G. C.; Kersting, R.


Physical Review Letters (2004), 93, 267401.


[20] Planken, P. C. M.; van der Valk, N. C. J. Optics Letters (2004), 29, pp. 2306-2308.


[21] Keilmann, F. and Hillenbrand, R., “Near-field


microscopy by elastic light scattering from a tip”


Philosophical Transactions of the Royal Society London. A, Vol. 362 (2004), pp. 787–805.


[22] Buersgens, F.; Kersting, R.; Chen, H. T. Applied Physics  Letters (2006), 88, 112115.


[23] Wang, K. L.; Mittleman, D. M.; van der Valk, N. C. J.; Planken, P. C. M. Applied Physics Letters (2004), 85,


pp. 2715-2717.


[24] Maier, S. A.; Andrews, S. R.; Martin-Moreno, L.;


Garcia-Vidal, F. J. Physical Review Letters (2006), 97,


176805.


[25]  Huber, A. J., Keilmann, F., Wittborn, J., Aizpurua, J.


and Hillenbrand, R., Nano Letters, (2008), 8 (11), pp.


3766-3770.


[26] Highlighted by "A terahertz nanoscope", Nature 456,


(2008), pp. 454-455.


[27] Ocelic, N., Hillenbrand, R., “Subwavelength-scale


tailoring of surface phonon polaritons by focused ionbeam implantation”, Nature Materials, Vol. 3, (2004),


pp. 606-609.


[28] Novotny, L.; Sanchez, E. J.; Xie, X. S. Ultramicroscopy (1998), 71, pp. 21-29.


[29] Cvitkovic, A.; Ocelic, N.; Aizpurua, J.; Guckenberger,


R.; Hillenbrand, R. Physical Review Letters (2006), 97,


60801.


[30] Novotny, L.; Hecht, B., Principles of Nano-Optics.


Cambridge University Press (Cambridge, 2007).


[31] Ocelic, N.; Huber, A.; Hillenbrand, R. Applied Physics  Letters (2006), 89, 101124.


[32] Wittborn, J., Weiland, R., Kazantsev, D., Huber, A.,


Keilmann, F. and Hillenbrand, R., “Material and doping


contrast in semiconductor devices at nanoscale


resolution using scattering-type scanning near-field


optical microscopy”, Proceedings of the 32nd


International Symposium for Testing and Failure


Analysis, Austin, Texas, USA, November, (2006), pp. 98-101.


[33] Taubner, T.; Hillenbrand, R.; Keilmann, F. Journal of  Microscopy-Oxford (2003), 210, pp. 311-314.


[34] Huber, A. J.; Kazantsev, D.; Keilmann, F.; Wittborn, J.; Hillenbrand, R. Advanced Materials (2007), 19, pp.


2209-2212.


[35] Knoll, B.; Keilmann, F. Applied Physics Letters (2000),77, pp. 3980-3982.


[36] von Ribbeck, H. G.; Brehm, M.; van der Weide, D. W.; Winnerl, S.; Drachenko, O.; Helm, M.; Keilmann, F.


Opt. Express (2008), 16, pp. 3430-3438.


[37] Zhan, H.; Astley, V.; Hvasta, M.; Deibel, J. A.;


Mittleman, D. M.; Lim, Y. S. Applied Physics Letters (2007), 91, 162110.


[38] Naftaly, M.; Miles, R. E. Proceedings of the IEEE


(2007), 95, pp. 1658-1665.


# Laser-Thermal Imaging


Laser-Thermal Imaging


R. Aaron Falk and Tram Pham


QFI, OptoMetrix Division, Tukwila, WA, USA


Laser induced emission and photocurrents with exponential  power scaling were discovered using a near IR Raman laser  scanning microscope. The potential for utilizing these highly  non-linear effects for sub-diffraction limited imaging has been  explored both theoretically and experimentally. A three-fold  improvement over the linear diffraction limit was predicted  and experimentally validated.


Improvement in image resolution with non-linear signal


response has been investigated through the square law power


scaling of two-photon absorption in biological [1] and IC (applications [2]. The square power dependence of the twoU S


photon signal narrows the image point response by square root  of two. Image resolution is improved over the diffraction limit


V C


by the same factor.


6


Two-photon absorption in silicon is produced using a near IR


wavelength pulsed laser (1275 nm). The peak pulse power is  sufficiently high to observe second order absorption of two  photons at once. The combined energy is equivalent to a  single photon at 637.5 nm, well above that silicon bandgap  energy. The resultant photo-carriers are collected as the laser  is scanned. Recent efforts have demonstrated both increased  transverse and axial resolution. This combination has  produced dramatic 3-D images of the junction areas of various  devices [3]


Even higher peak laser powers can induce absorption of three  photons, four photons, and so on. The related image resolution  would improve as square root of the number of photons  absorbed for each created photo-carrier. However, the  required laser powers become somewhat problematic from a  practical standpoint.


Serendipitous background signals that occurred in our IR  Raman studies proved to have an exponential scaling with  laser power. Although these background signals prove to be a  nuisance for Raman imaging, the high order non-linearity  sparked an immediate investigation into their potential  application to non-linear imaging. Theoretical modeling  predicted a three-fold improvement in image resolution over  the diffraction limit. Experimental results using two different  approaches have confirmed these predictions.


Recent experiments in backside IR Raman imaging of silicon  ICs [4] produced an unexpected broadband background signal  when illuminated with focused, high-intensity (~ 10MW/cm2) laser radiation at 1342 nm (see Fig 1). This optical  background only occurred at certain locations in the device  that often correlated to an induced ‘photocurrent’ on the order  of 0.1 microamp.


-500


e u


n 0 0


1000 1500 2000


Pixel


Laser Line


Unknown


Background  Raman Line


Figure 1: IR Raman spectrum with background ‘fluorescence’. Pixel scale is ~ 1330 to 1580 nm.


The illumination photons are not sufficiently energetic to  expect fluorescent excitation. In addition, the silicon target  contained no materials that are expected to fluoresce at the  1342 nm pump wavelength. Test of signal variation versus  laser power established an exponential variation (see Fig. 2)


Two models were proposed for this laser effect that involved  laser heating of highly absorptive areas in the IC well above  ambient room temperature. In the first model, laser heating  induces thermal emissions. This model is sufficient to explain  the broadband emission detected by the Raman spectrometer, but did not adequately explain the induced leakage currents.  In the second model laser heating in the IC induces increased  leakage currents. A small portion of the generated carriers


recombine in photon emission to produce the detected  broadband background.


0 200 400


U 6600 0


0800 S1000


1200


1400


60


65


70


75


80


Laser Power (mW)


Data---Fit


Figure 2:  Exponential scaling of broadband emission with  laser power. Fit of Plank’s law (Eq. 1) is consistent with ~ 210 oC peak temperature rise for induced thermal radiation.


Plank’s equation describes the expected power scaling for the  first hypothesis. However in this temperature range, an  exponential approximation is highly accurate. The exponential  approximation can be recast into the same form as current  scaling with temperature of a pn junction, with an effective  junction energy of ~ 0.2 eV for this wavelength range (1.4 to


1.6 micron) as shown in Eq. 1.


( )


[


] (


W


C T


EkT


λλ λ=−≅ −15201expexp Δ )  (1)


Thus, the two effects cannot be distinguished by simple power  scaling. In addition, the spectral characteristics of the two  effects [5] are not readily distinguishable over the relatively  narrow Raman signal bandpass, 1380 to 1580 nm, into our  spectrometer.


Although performance of mDSIL is not competitive to current  static DSIL performance, one of the aims in this work is to  regenerate interest in DSIL application for far field laser fault  isolation diagnostic tools. Gradually, existing DSIL  technologies to improve the laser spot size further can be  implemented to overcome current limitations. mDSIL offers an  alternative to RSIL. It is believed that DSIL can eventually be  as good, yet a more economical option than RSIL since it can  be fabricated in typical FA laboratories.


The main author would like to acknowledge Frank Zachariasse  of NXP Semiconductors for his time and discussion on  fabrication of DSIL in the course of his post graduate degree.


[1] Bruce MR, Bruce VJ, Prejean S, Huynh J, "Failure  Analysis Turned Upside Down:  A Review of Backside  Analysis Techniques", Electronic Device Failure  Analysis, Vol 5, No 4, pg 13-24, 2003.


[2] Phang JCH, Chan DSH, Palaniappan M, Chin JM, Davis  B, Bruce M, Wilcox J, Gilfeather G, Chua CM, Koh LS, Ng HY, Tan SH, “A Review of Laser Induced Techniques  for Microelectronic Failure Analysis”, Proc Int Symp  Physical & Failure Analysis of Integrated Circuits (IPFA  2004), pg 255-261, 2004.


[3] Bruce M, Bruce M, Eppes D, Wilcox J, Cole E, Tangyuanyong P, Hawkins C, “Soft Defect  Localization(SDL) on ICs”. Proc Int Symp Testing & Failure Analysis (ISTFA 2002), pg 21-27, 2002.


[4] Wagner  LC,” Failure analysis challenges”, Proc Int Symp  Physical & Failure Analysis of Integrated Circuits (IPFA  2001),  pg 36-41, 2001.


[5] Vallett DP, “Failure analysis requirements for  nanoelectronics,” IEEE Trans. Nanotechnol., Vol 1, No 3, pg. 117–121, 2002.


[6] Semiconductor Industry Association, “International  Technology Roadmap for Semiconductors”, 2008 Edition


[7] Ippolito SB, Goldberg BB, and Ünlü  MS, “Highresolution Subsurface Microscopy Technique”, Appl Phys  Lett, Vol. 78, No. 26, pg 4071-4073, 2001.


[8] Goh SH, Quah ACT, Sheppard CJR, Chua CM, Koh LS, Phang JCH, “Effect of Refractive Solid Immersion Lens  Parameters on the Enhancement of Laser Induced Fault  Localization Techniques”, Proc Int Symp Physical & Failure Analysis of Integrated Circuits (IPFA 2008), pg 1-6, 2008.


[9] Brunner R, Burkhardt M, Pesch A, and Sandfuchs O, Ferstl M, Hohng S and White JO, “Diffraction-based solid  immersion lens”, J Opt Soc. Am A, Vol 21, No 7, pg  1186-1191, 2004.


[10] Zachariasse F, Goossens Martijn, “Diffractive Lenses for  High Resolution Laser Based Failure Analysis”, Proc Int  Symp Testing & Failure Analysis (ISTFA 2005), pg.1-7,


2005.


[11] Donald C O‟Shea, Thomas J Suleski, Alan D Kathman, Dennis W Prather, “Diffractive Optics- Design, Fabrication, and Test”, Tutorial Texts in Optical  Engineering, TT62, SPIE publication, 2004.


[12] Edward Coyne and Frank Zachariasse, “A working  method for prototyping solid immersion blazed-phase  diffractive optics for near-infrared laser microscopy”, J  Micromec Microeng, Vol 18, 045016, pg. 1-9, 2008.


[13] Kipp L et al., “Sharper images by focusing soft X-rays  with photon sieves” Nature Vol  414, pg 184-188, 2001.


[14] Cao Q and Jahns J, “Modified Fresnel zone plates that  produce sharp Gaussian focal  spots”, J Opt Soc Am A, Vol. 20, No. 8, pg 1576-1581, 2003.


[15] Ali M, Wagner  T, Shakoor  M, and Molian PA, “Review  of laser nanomachining”, J Laser Appl, Vol 20, No 3, pg  169-184, 2008.


# Volume Electrical Failure Analysis for Product-Specific Yield Enhancement


Volume Electrical Failure Analysis


for Product-Specific Yield Enhancement


Steven Kasapi, Joy Liao, Bruce Cory


NVIDIA, 2701 San Tomas Expressway, Santa Clara, CA 95050 USA


Izak Kapilevich, Richard Portune, Yin Shyang Ng, Cathy Kardach and Elaine Cheng


DCG Systems, 45900 Northport Loop East, Fremont, CA 94538 USA


Contact: skasapi@nvidia.com


Yield on specific designs often falls far short of predicted  yield, especially at new technology nodes. Product-specific  yield ramp is particularly challenging because the defects are, by definition, specific to the design, and often require some  degree of design knowledge to isolate the failure.


Despite the wide variety of advanced electrical failure analysis (EFA) techniques available today, they are not routinely  applied during yield ramp. EFA techniques typically require a  significant amount of test pattern customization, fixturing  modification, or design knowledge. Unless the problem is  critical, there is usually not time to apply advanced EFA  techniques during yield ramp, despite the potential of EFA to  provide valuable defect insight.


We present a volume-oriented workflow integrating a limited  set of electrical failure analysis (EFA) techniques. We believe  this workflow will provide significant benefit by improving  defect localization and identification beyond what is available  using test-based techniques.


Current Product-Specific Yield-Ramp Workflow


Figure 1:  Typical workflow for product-specific yield ramp


Figure 1 shows a typical product-specific yield-ramp  workflow. A production tester logs the pin and cycle failure  information, usually from die on an entire wafer or set of  representative wafers. Fault diagnosis software attempts to  identify the root cause of the failure from the tester failure logs – which specific fault diagnosis is performed depends on  which test pattern is failing. For example, a bitmap failure  leads to mapping of the physical location of which bit has  failed, whereas a scan capture failure would lead to scan  capture diagnosis.


Failing devices for which fault diagnosis is able to localize a  candidate defect region are submitted for physical failure  analysis (PFA). During PFA the part is de-processed to look  for physical evidence of the defect. If an underlying process  issue is found a corrective action is implemented, if possible.


The root-causes of some test failures are relatively easy to find  with this approach. For example, if an embedded SRAM fails  a bitmap pattern the physical location of the failing bit cell can  be identified easily from the tester failure output. SRAM  arrays are popular vehicles for process development and  monitoring because of the high degree of localization possible  from test results alone.


Defects which occur in areas covered by logic are harder to  diagnose. The design of logic is nearly always product-specific  and does not have nearly the same external visibility as  memory arrays.


Design-for-test (DFT) scan methodologies help make intralogic defect localization more systematic. The scan chain  architecture provides a means of viewing the values on the  outputs of any flop included in the DFT design from the  external pins and software simulation models certain classes of  defects, usually hard stuck-at defects and bridges.


There are a number of scenarios in which DFT diagnosis does  not perform well. Scenarios include ones in which:


• The failure is parametric, or shows frequency, voltage, or temperature dependency.


• Scan chain shift fails;


Data logging at wafer sort


Fault diagnosis


Root Cause (Physical  Failure Analysis)


Corrective Action


• The diagnosis software fails to find a sufficiently  localized root cause;


• There are multiple failures;


• There are failures in the clock tree or control logic;


The final outcome of each root-cause analysis is PFA. In order  to be successful, PFA requires a relatively small area at the  outset. If DFT cannot sufficiently isolate the location of the  defect the chances of getting a PFA result are slim.


Our volume EFA workflow builds upon DFT scan analysis, in  particular DFT scan shift and scan capture analysis. EFA  techniques enable circuit visibility beyond the flops included  in the DFT design. EFA, applied appropriately, can overcome  many of the limitations of DFT-based yield ramp.


Incorporating EFA into Yield Ramp


Electrical failure analysis (EFA) tools are used by many FA  labs to determine root-causes of DFT failures in low volume. The quantity of die to be analyzed during yield ramp makes it  impractical for a conventional FA lab to have significant  impact during yield ramp. In our experience the FA lab only  becomes involved to help solve the most critical issues  because of the cycle time involved in EFA work.


In order to be effective during high-volume yield ramp, EFA  techniques must meet several basic requirements:


• The cycle times must be short;


• The measurements must use production testers, probe  cards, and test patterns;


• The techniques must work on full-thickness wafers  with minimal (preferably no) surface preparation;


• The techniques must be robust enough for automation  and fast cycle times;


We have surveyed available EFA techniques and focused on  the ones which are best suited to volume yield ramp.


Many of common EFA techniques are not well-suited to  volume work:


• Static laser techniques (OBIRCH, TIVA, etc.) require accessing the power supply of the tester which  is impractical when using production testers on highcurrent devices. Static laser techniques are also  difficult to automate because there are many  parameters that need adjustment (laser power, scan  speed, power supply noise gain, etc.)


• Dynamic laser techniques (LADA, SDL, etc.) are  more suited to marginal failures than yield-related  defects. Our emphasis is currently on hard (voltage  and frequency insensitive) failures. We may introduce  dynamic laser techniques in the future but the bulk of  yield ramp work is to find and fix hard failures.


Dynamic laser techniques also suffer from a large  range of parameters which need adjustment.


• Thermal emission techniques do not have sufficient  spatial resolution to localize single-gate failures.


• Probing techniques (TRE, LVP, etc.) require  considerable design knowledge and in their current  form are not well-suited to automation.


After our survey only two EFA techniques stood out as wellsuited to automation.


The first and most mature technique is static emission  microscopy (EMMI). EMMI is simple to perform and is wellsuited to automation because it only requires collecting  photons from a region-of-interest (ROI). Taking a difference in  the photon emission rate between a passing and failing die can  indicate gates connected to a defective regioni.


The second technique, modulation mapping, is relatively new. Like static emission microscopy, it does not require special  tester setup and only requires navigation to the ROI in order to  perform a measurement. We will review modulation mapping  later in this paper during the case study.


EFA Yield Ramp Workflow


Simon et al. have already demonstrated that EFA techniques  are beneficial for yield enhancementii. The main conceptual  difference between our work and theirs is the degree of  automation and throughput targets we are trying to achieve. Our goal is to achieve a similar workflow as theirs but with  high throughput driven by volume automated DFT analysis.


The workflow was originally developed for EMMI  measurements. As already mentioned, there is significant value  to expanding it to include modulation mapping. For the sake of  clarity we will refer to EMMI measurement, but will present  modulation mapping results as part of the case study to show  how it fits naturally with the EMMI workflow.


Our volume EFA workflow, starting from the DFT analysis  already established is as follows:


• Select failing die for further analysis based on failure  information and DFT analysis;


• Determine the appropriate EMMI measurement  regions, pattern, and tester condition (loop or hold-atvector) for the failure condition;


• Perform the prescribed measurements on the selected  failing die and a passing reference die and store all  the resulting data in a database;


• Analyze the data to identify candidate failing nets for  PFA;


do not support high throughput. The hardware is designed for  manual control by a single, skilled operator. The fixturing is


usually designed for packaged die, not whole wafers and  production testers. The software has little or no ability to  catalog and analyze data across multiple signal acquisitions, let  alone die spanning many wafers as required for yield ramp.


To realize the EFA yield ramp workflow we had to develop  both new EFA hardware and software.


Hardware


The basic hardware requirements to enable this workflow  included:


• Compatible with full-thickness wafers without  thinning or polishing;


• Compatible with > 10,000 die bumps for large IC’s;


• Mechanism for loading a wafer within a few minutes;


• Probe-to-pad alignment with step-and-repeat  navigation to any die on the wafer;


• Less than 0.5 um drift in a half-hour measurement  time;


• Integrated-resolution optics and IR photon imaging  detector;


• Controllable through external communications  interface (preferably a network-accessible API);


The hardware we used (WaferScan from DCG Systems) met  most of these requirements. It was still at a prototype stage and  did not include a software API, hence requiring significant  manual control. However, the core hardware supported the  yield-ramp application well.


Using this HW, switching from die-to-die on a wafer was  limited by the time it took to do a “step-and-repeat” process (retract the probe card, move the wafer, and land the probe  card). The “step-and-repeat” process took approximately 10-30 seconds per die, depending on the distance between the die. In contrast, changing die in a typical lab-based FA  environment can take several hours, including DUT prep, fixturing, and alignment.


Landing and retracting the probe card from the wafer was  performed by raising and lowering the probe card. In a  conventional production probe system the wafer is raised and  lowered while the probe card is stationary, so the vendor  introduced a flexible interface between the probe card and the  test head to allow for movement of the probe card. The delay  introduced by the cable interface requires a simple timing  calibration to compensate for the additional cable length  between the pin driver and the device pin. In practice the extra  cable length presented no difficulties beyond this initial  calibration.


The WaferScan system also included an InGaAs EMMI  camera with a very sensitive LN2-cooled 1024x1024 pixel  array and a variety of air-coupled lenses.


Software


We developed an in-house software tool set at NVIDIA to  enable data collection, cataloging, and analysis across multiple  die. The tool screens the DFT diagnosis output, prescribes the  appropriate EFA measurement based on the failure type, identifies the measurement regions and lens types, catalogs the  data as it is collected, and presents the results in a CAD  coordinate space for analysis.


All relevant information is stored in an XML-based file. We  refer to the XML-based markup language as Circuit Analysis  Markup Language, or CAML for short.


Determining the measurement to be performed


Figure 2. Data flow for determining what and where to  measure


Figure 2 shows the flow of information leading to the  measurements. DFT shift failures are those in which the data  cannot be loaded and unloaded from the scan chain correctly. DFT capture failures are those in which the part passes shift,


Fault  Diagnosis


DFT Capture  Fail


DFT Shift Fail


Other


MBIST, etc.


Identify & Locate Failing  Chains


Identify & Locate  Callouts


Stop


Choose Test  Vectors within  Pattern


Choose


Measurement


Regions


Submit


Analysis


Instructions for  Measurement


but a defect in the inter-connecting logic causes a failure when  the data is captured.


A standard scan chain consists of a set up flops which can be  configured as a shift register. A 2-input MUX determines  whether the flop is fed by logic or by a previous flop. In shift  mode, each flop receives data from the previous flop in the  chain. A single input pin feeds data into the scan chain and the  output is sent to a single output pin. In designs with millions of  transistors the number of flops in a single scan chain can easily  number in the thousands.


A compressed scan chain is a sub-chain of a compressed scan  chain. It is formed by dividing the standard scan chain into  smaller scan chains. The number of compressed scan chains  usually far exceeds the number of I/O pins, so a single pin  drives multiple compressed scan chains, and combinational  logic mixes data from multiple compressed scan chains onto  the output pins.


For EFA, compressed scan chains have the benefit of being  much shorter than standard scan chains. Using compressed  chain shift failures provides a valuable first step of isolation. A  compressed scan chain typically covers less than 300 x


mµ , significantly less than area of several square


millimeters that a conventional scan chain can cover. We work  exclusively with compressed shift test patterns and on die with  a small number (usually less than three) of failing compressed  scan chains.


We chose to focus on scan chain shift failures because  software solutions have only marginally effective. Scan shift  debug represents a significant unsolved challenge for the  industry.


The relationship between pin/cycle failures and failing  compressed scan chains can be complex. An automated  software tool converts the compressed shift failure log data  into failing compressed scan chains. Another software tool  analyzes chain flop and logic in the Q fanout logic to  determine the locations at which EMMI data (or other FA  data, such as modulation mapping) should be collected. Both  the flops and the fanout are considered because a defect in the  fanout logic net can prevent data from propagating between  the flops.


Another software tool determines the best acquisition regions  to cover the candidate logic as efficiently as possible. To cover  an entire scan chain several images may be required. We store  the physical description of the circuit in the CAML file to  facilitate subsequent analysis without requiring access to a full  design database.


As each EMMI image is captured, all the relevant information  about how the image was acquired is logged into the CAML  file. Some of the information stored includes:


• Design name, wafer, and die location;


• EFA tool name, serial number, operator, and location;


• CAD location of the image;


• Lens, acquisition time, camera, etc.


• Test pattern and stimulus conditions (looping or  holding at a cycle);


• Link to failure log, diagnosis result, and measurement  data;


To ensure the image-to-CAD alignment we also store the  following:


• Mapping between image-space and device (or stage)-space;


• Mapping between stage coordinates and CAD  coordinates;


• Reference images to enable post-processing fine  alignment;


In an EMMI image, the image-to-device mapping is mainly  affected by the magnification of and aberrations in the lens  used as well as any rotation of the camera. The image-todevice mapping does not change unless the camera is moved  within its mount.


The image-to-device mapping can be calibrated once and  remains valid until the camera mounting is changed, such as  during service. After calibration, for a particular measurement, all that is needed to map every pixel in the image to an  absolute coordinate on the DUT is the mapping of a single  point. However, in very dense logic, aligning a single point  can be challenging. Reference images of identifiable structures  are needed because in very dense logic regions there are no  identifying structures with which to confirm the alignment.


The basic scheme of the EMMI measurements is to acquire  photon emission signals from the failing die and a good  reference die under exactly the same input stimulus conditions  and look for any significant differences coinciding with the  scan chain and any associated logic. The associated logic  includes buffers between flops during shift and the fan out  logic one level deep from the Q output of the flops. The  defects are usually in the logic feeding the cells showing  anomalous EMMI, although it could also be in the cells  themselves, either in the metal inter-connects or in the  transistors.


Once the data is logged into the CAML file, another software  module renders all the captured images in a CAD coordinate  system and searches for anomalies between the good and bad  die.


The in-house software system can be linked to a CAD viewer (in our case NEXS from DCG Systems) for net tracing from  cell ports and for comparison to the GDS information. NEXS  also enables identification of cells not pre-determined by our  automated software flow during manual post-processing.


One benefit of the systematic data logging at each step of the  process is that it is suitable for an extended environment. We  have successfully implemented the workflow with data  collection in Taiwan and analysis of the collected data in  California. We have studied several dozen die using this  hardware and software combination.


To clarify the workflow, we present a typical case study.


Case Study


The device for this case study is a commercial 40-nm bulk  CMOS GPU operated at its nominal voltage of 0.95 V. It  failed a compressed shift test and the failure was insensitive to  frequency and voltage. In order to perform additional electrical  analysis this die was packaged but was kept full-thickness and  without any anti-reflection (AR) coating to replicate the  measurements we would normally perform on a wafer during  yield ramp.


From the wafer test failure log we identified a single failing  chain on this device. As outlined above, our software  automatically identified the bounding boxes of every flop in  the chain and calculated the location of the lens required to  observe the relevant flops and Q fanouts.


Figure 3. Failing scan chain (in red) superimposed on a  reflected-light image (top) and on an EMMI image (bottom) using an air-coupled 50x, 0.5 NA lens.


The pattern used during shift is a 11001100… data sequence. We ran the pattern up to the cycle when the chain of interest  was loaded with the 11001100… shift pattern and stopped. We  also ran two cycles later, when the chain was loaded with a  00110011… pattern and stopped.


We used a 50x, 0.5 NA air-coupled lens to perform all the  measurements. The field-of-view was 296 x 296 µm2 and  almost completely enclosed the scan chain.


Figure 3 shows the entire scan chain superimposed on a  reflected light image (top) and on a photon-emission (EMMI) image (bottom) when the chain is loaded with a 11001100… pattern. The images were rendered from the data in the CAML  file and are displayed in a CAD coordinate system. The  software filters the images displayed by image type (EMMI or  reflected light, good die, bad die, test conditions, etc.)


We calibrated the lens field-of-view and image rotation to  achieve image-to-CAD accuracy of +/- 0.5 um across the field  of view. The reflected-light image is centered away from the  scan chain onto a distinct structure to facilitate alignment, as  outlined above. Subsequent EMMI images were referenced to  this alignment image, within the accuracy of the mechanical  stage. With reasonable thermal control the stage drift in the  WaferScan was < 0.5 um over the 10 minutes duration of the  measurements.


We took EMMI images from the failing device and a passing  reference device at exactly the same location and tester  stimulus. On each die, we took an image when the chain was  fully loaded (with the 11001100… vector) and two cycles  before (with the complementary 00110011… vector on the  output of the flops). The EMMI exposure time was 60s for  each image. In total 8 images were collected, including the  four EMMI images and four reflected-light reference images.


The average EMMI levels in the two devices were different  because the devices had different average current leakage  rates. After adjusting the mean signal levels and taking the  difference between the failing die and good die a single point  in the chain stood out as anomalous.


①


o0d=5.0mm


D.00m


0224


Figure 4. EMMI image on at fixed cycle on failing device (left) and passing device (center).


C234


Figure 5. Difference between the EMMI images on the good  and bad die. The anomalous EMMI occurs at the input to flop


48.


Figure 4 shows EMMI from a good reference device (top) and


cuntarg (310269. 5239.88)mm 10E


the failing device (bottom). Figure 5 shows the difference  between the two images. Zooming into the anomaly we could  see that it coincided with the input to flop 48 in the scan chain  which was fed by the output from flop 49 (the chain is fed in  reverse order – flop N feeds flop N-1 etc.).


est


Figure 6. Outline of flop 49 (red) and flop 48 (blue) showing  interconnecting nets and logic


02


982


Figure 6 shows a close-up of flops 49 and 48 (the figure also  shows flops 50 and 47 (top and bottom respectively, in white,


Du


for completeness). The output of flop 49 (shown in red) also  drives 3 other gates. The signal from flop 49 to flop 48 passes


C204


through a buffer (shown in purple).


o


The EMMI signal suggested a defect in the net (shown in blue) connecting a buffer (show in purple) to flop 48. The total  length of the next is approximately 1 µm.


Limitations of EMMI


C221


986C


0274


This case study produced a single significant anomalous


C220


ban


emission spot and indicated a single failure location. In  general, EMMI results can be complicated to interpret because


a single defect can cause anomalous emission from several


5001


52H


cells. Tracing the nets back from multiple cells can be time065


gzEG


consuming. Instead, we have chosen to adopt an additional


c30


EFA technique, modulation mapping, into the workflow.


DoC


oro


029


5C92


s*9


Modulation Mapping


As discussed in the introduction, we strictly limited ourselves  to techniques which could be applied in volume at wafer level.


P


C264


Modulation mapping, as discussed in the introduction, is


OtD


CD68


another candidate yield-ramp EFA technique. The modulation


as


C4


mapping hardware we used was a prototype, integrated into  our in-house Meridian system, but has since been integrated  into the WaferScan system.


Modulation mapping (also known as laser signal imaging (LSI)) is a technique for imaging circuit activity at specific  frequencies rates. Kindereit et al. have already presented the


49 48 oa wDZL


47


49 48 OTIS


49 48


49


48


中


50


canlerg (310269.5239.88)mm


EMMI  Anomaly


physical basis of the techniqueiii. A separate abstract,


concnt(310208 5240.05


C2Z)


C274


submitted to ISTFA 2010, covers details of the technique so  we will only briefly review it here.


Analysis:  Electrical Probing


The delay circuitry block is shown schematically in Fig. 5, with the probe points labeled corresponding to those in Fig. 4. The clock signal inputs at each branch are 180° out of phase  with one another. The delay block supplies different parts of  the chip with clock signals of different delays, and the probe  pads are located to probe those clock signals. Each delay is  much shorter than the input signal period, so all points on one  leg are out of phase with all points on the other leg.


Delay  Element


F


B


E


Figure 5:  Schematic diagram of the delay circuitry with the  probe points labeled. Note that the clock signals going into  each branch are 180° out of phase.


Manual probing of the test points labeled in Fig. 4 and Fig. 5  was performed in order to check for anomalous signals in the  delay circuitry. It was confirmed that there was no clock  signal present for points B & C when the die was drawing 2 current draw, and no clock signal for point B, C, E, & F when  the die had 3 current draw. When probing these same test  points on a known good device, strong clock signals were  seen. Probing all the delay circuitry probe points confirmed  that when an LSIM signature was present, there was no clock  signal present at the probe points connected to that signature  area. See Fig. 6 for the tabulated results. This anomalous  behavior was confirmed on several other die as well.


Figure 6: Clock frequency (kHz) at all probe points. The "Master" clock was measured to verify that the clock was  working. The clock frequency is halved before entering the  delay circuitry block.


The traces were electrically isolated with a laser to separate  the downstream PEM sites from the delay circuitry block and  to see if the clock signal was being sapped by some shunt  downstream. This was done at numerous locations  concentrating on the circuitry downstream of test points B and  C, starting far downstream and moving progressively closer. When points H & J (in Fig. 3) were cut, there was no change  in current draw or clock signal. In fact, no disconnections  downstream of any of the probe points corrected the problem  in the delay circuitry, indicating that the failure was located  within the delay circuitry.


Directly measuring the resistance between test-points B & C, as well as test-points E & F discovered a resistive path of ~400Ω for both. The same measurements were performed on a  known good device resulting in electrical opens (>10MΩ).


Looking more closely at the probe points at B & C in Fig. 5, there are two inverters right before the probe points. One  hypothesis was that a short existed somewhere between them, and we started by considering the outputs. Figure 7 shows the  two inverters at B & C, and note that the input signals are  shown to be out of phase as mentioned before. Thus, when the  input signal to the inverter at B is low, its output is connected  to Vdd, and at the same time, the input to C is high, connecting its output to ground. In this way, if the outputs  were electrically connected, the result is a connection from  Vdd through the resistive short to ground. When the input  clock cycles flip, the same thing happens, but now the path is  from Vdd in C to ground in B through the resistive short. A  resistive short was thus consistent with the current flow in the  current imaging maps and the functioning of the circuit.


We attempted to create the excess current draw on a known  good die by applying a resistive path of 400Ω between testpoints B & C using probes; the current of the known good die  went from 1 to 2. A second test was conducted where testpoints B & C as well as E & F both had resistive paths across  them, and the total current consumption was confirmed to  jump from 1 to 3. When the resistive paths were removed, the current consumption went back down to the normal 1 level.


Vdd


|Probe  point |Good Device  1x current |Failing Device  2x current |Failing Device  3x current |
|---|---|---|---|

|Master |693 |698 |698 |

|A B |346 |349 |349 |

|A B |346 |‐‐‐ |‐‐‐ |

|C |346 |‐‐‐ |‐‐‐ |

|D E |346 |349 |349 ‐‐‐ |

|F |346 |349 |‐‐‐ |

|G |346 |349 |349 |

-b0


Output B=Vdd


Input


GND Vdd


-dl


Output C= GND


Figure 7: Behavior of inverters at points B & C with  suspected short included between the outputs. Since the  signals are 180° out of phase, the result would be a  connection of Vdd to ground through the resistive short.


As further verification, LSIM was performed on a known  good die with a resistive path between test-points B & C, and  the same LSIM signature as in Fig. 1a was reproduced (see  Fig. 8a). To locate the resistive path between these points on a  known failing die, LSIM was performed in which the bias was  applied directly to points B & C on a failing die. This analysis  further identified a small signature site between MET2 lines  which connect to the delay circuitry of the die (Fig. 8b).


a)


b)


Figure 8: a) LSIM bias is applied to a known good die  between VDD and GND while a resistive path is applied  between test points B & C, recreating the signature observed  on a 2 current draw die. b) LSIM bias is then applied  directly between points B & C on a failing die which revealed  a signature site as shown in yellow circle.


Analysis:  FIB cross sections


The spot located in Fig. 8b is shown on a layout diagram  below in Fig. 9, which also shows the direction of the FIB cut  done to look for the short.  Figure 10 shows three successive  FIB cuts through the MET2 lines at the site. There is clearly  residual barrier metal layer connecting the two traces. The  connection goes diagonally across from one trace to the next, so the successive cuts help visualize it “moving” from the  right line to the left line.


Figure 9: Schematic of FIB cross section through the  signature shown in Fig. 8b.


Residual metal


extending from base  of right interconnect


Residual metal no  longer connected to  right interconnect…


but is continuing to left  interconnect.


Higher kV electrons image  below the surface, revealing  residual metal extending to  neighboring line.


1kV


28kV


Residual metal  connected to left


interconnect


Figure 10: FIB cross section through the LSIM spot found  between two interconnects in Fig. 8b. The residual barrier  metal was verified to be the cause of the extra current draw  originally observed.


Imaging with both low and high energy electrons (1kV and  28kV) in the SEM enables imaging slightly below the surface  of the cut and gives an indication of how quickly the feature is  changing so that we can adjust the FIB cut steps accordingly.  This is a useful technique to help avoid cutting all the way  past the feature of interest by accident, which sometimes  happens, especially when the size of the feature is unknown.


In this area of the two MET2 lines that are perpendicularly  running over two MET1 lines, the topography created a slight  bowl shape that made clearing out the metal a bit more  difficult. In this particular topographical feature, the aluminum  was not being completely cleared, masking the etch of the  barrier metal and leaving it behind. A slightly longer etch time  at the aluminum etch step was shown to clear it completely, allowing the barrier metal etch to remove the barrier metal, and the yield recovered on the subsequent lots.


Localizing strong metal shorts is often difficult because PEM  and LSIM can identify effects rather than causes of defects, especially when the bias is applied to an entire die rather than  subsections. Furthermore, for a strong metal short, the  scanning laser may have only a small effect in changing the  resistance of the short, making the difference in the circuit  performance undetectable. Weak metal shorts where the laser  can modify the resistance of the defect are easier to identify. In this case, the LSIM found the structures that were being  driven hard as a result of the strong shorts elsewhere in the  circuitry.


Current mapping showed where the current was flowing in the  circuit which indicated the correct circuit block to focus on. By combining probing of that circuit block with the current  mapping and emission results, we were able to understand the  photon emission spots and the LSIM signatures to be effects  of the defect. It also helped us narrow down the search for the  defect so that LSIM on a small part of the circuit could lead us  to the actual defect.


A few other points in this work are noteworthy from a failure  analysis perspective:


1. Having probe points located at a variety of locations  throughout the circuit significantly helped make probing  easier. We did not have to deposit probe pads with a FIB, and  that made our cycles of learning much faster. This is a nice  feature to include when designing for FA.


2. Using higher energy electrons when imaging during the  FIB cross sectioning helped us see below the surface to make  sure we did not cut too aggressively and miss the defect.


The authors acknowledge the help of M. O’Kane, T. Kelly, J. Long, R. Mhatre, A. Saxonis, F. Vazaghoo, B. Wachtmann of  ADI, and M. Carter and G. Xiao of Micro Magnetics.


[1] L. A. Knauss, et al, Microelectronics Failure Analysis


|Desk Reference, 5th edition, ASM International (Materials |96. |
|---|---|

|Park, OH, 2005), pp. 303-11. ||

|[2] C. Hillman, “A Novel Approach to identifying and Validating Electrical leakage in Printed Circuit Boards through Magnetic Current Imaging,” Proc 30th Int’l Symp for Testing and Failure Analysis, Worcestor, MA, November 2004, pp 82-87. [3] O. Crepel, et al, “Magnetic Current Imaging Techniques: Comparative Case Studies,” Proc 30th Int’l Symp for Testing and Failure Analysis, Worcestor, MA, November 2004, pp 29-32. |Ma Ana [6] C. Sili Ref [7] R. Pr San |

[4] D. Vallett, “Scanning SQUID Microscopy for Die Level  Fault Isolation,” Proc 28th Int’l Symp for Testing and  Failure Analysis, Phoenix, AZ, November 2002, pp. 391-[5] B. D. Schrag, et al, “Scanning Magnetoresistive  Microscopy for Die-Level Sub-Micron Current Density  pping”, Proc 29th Int’l Symp for Testing and Failure  lysis, Santa Clara, CA, November 2003, pp. 2-5.


Boit, “Fundamentals of Photon Emission (PEM) in  con,” Microelectronics Failure Analysis Desk  erence, 2005, pp. 356-68.


Aaron Falk, “Advanced LIVA/TIVA Techniques," oc 27th Int’l Symp for Testing and Failure Analysis, ta Clara, CA, November 2001, pp. 59-65.


Inter Layer Dielectric Defect Induced High Contact Resistance


Re-Long Chiu, Jason Higgins, Toby Kinder, Juha Tyni, Sharon Ying and Jones Chung


WaferTech LLC CAMAS Washington rchiu@wafertech.com  360-817-3364


High contact resistance can be caused by moisture absorption in low phosphorus content BPTEOS. Moisture diffused  through the TiN glue layer is absorbed by the BPTEOS during  subsequent thermal processes resulting in increased contact  resistance. This failure mode was studied by combining


4-


different failure analysis methods and was confirmed by  duplication on experimental wafers.


Contact resistance is a critical parameter of semiconductor  devices since it can significantly affect product performance.


0.


Abnormally low contact resistance can result in low yield and  possibly decreased reliability.  The potential origins of this  problem are numerous, including insufficient contact etching, particle blocking, Ti/TiN glue layer anomalies [1], improper


-2


tungsten plug deposition, or chemical mechanical polish


(CMP) clean issues.  Failure analysis (FA) work may provide


misleading information if it is based solely upon interpretation


of diagnostic images of the structures in question.  This could 4 hinder correct identification of the root cause of the failure and


delay corrective action.


-20


m4


In this paper, we report on a novel failure mechanism that


=caused high contact resistance induced by inter-layer dielectric 20%日(ILD) defects.  The failures were revealed by an in line wafer


0 acceptance test (WAT) monitor on a Metal-1 layer test 20%036%si-structure.  The analysis of the failure used a number of 60%0 techniques including  passive voltage contrast (PVC) imaging,


scanning electron microscope (SEM) inspection, focused ion


beam (FIB) cross sectioning, transmission electron microscope


70%器 20%0非


diePercentage of all


(TEM) imaging, energy dispersive X-ray (EDX) spectroscopy,and secondary ion mass spectroscopy (SIMS).


Experimental Details


In this case study, the ILD layer is formed by using silicon


汾100150206客om点骞岑宏患660700750R00


oxygen nitride (SiON) as a barrier layer to the polysilicon gate electrodes, followed by boron and phosphorus doped  tetraethyl orthosilicate (BPTEOS) layer for satisfactory reflow, then topped with a deposited tetraethyl ortho-silicate (TEOS) layer and planarized using CMP. One 0.18 um CMOS wafer  failed Metal-1 WAT monitor tests for excessive active and


poly contact resistance. The contact resistance test on the  WAT structures showed a random distribution as seen in the


(a) wafer map and (b) contact resistance distribution shown in  Figure 1 with the bad devices having contact resistance  between 20Ω and 500Ω compared to normal values of  <10Ω.


||||8.257|8.079|8.183||||
|---|---|---|---|---|---|---|---|---|

||9.267|9.758|2.483|1559|369|2016|8231||

||1125|139.2|61-42|2658|58:91|9.341|7.7E+06||

|75,42|9.303|X317|902 7||26n|被安|85|31.2)|

|3.029|3083|377|1596|8.198|15.28|13.37|383|156 3|

|2929|12|3.218|3817|719|TT0|11.43|182)|124B|

||1774|8.143|8.351|0013|1665|10,15|38.63||

|||JBAS|48|1138|4957|1175|8172||

||||13.68|3627|7697|(a) |(a) |(a) |

Figure 1: Contact resistance (a) wafer map with failing region indicated and (b) distribution.


Corrtact Resistance Ghm


One test unit, highlighted on the wafer map, was measured at  around 1MΩ but is not shown in the distribution graph.  A failure site was isolated on the highest resistance failed die


AI


using PVC.  FIB and SEM inspection revealed a hollow  tungsten contact.  However, this did not explain the failure  resistance distribution symptom so TEM/EDX examination


W-plugTEOG


was performed on a marginal failure site.  TEM sample


BPTEOG


preparation was done using FIB milling and lift out was  achieved by triboelectric charge.


.SION


Poly-Si


TEM analysis was performed using a TECNAI F20 instrument


↑


Ox


equipped with EDX and a scanning transmission electron  microscope (STEM).  An anomaly in the ILD film was  observed, so the sample was submitted for a more detailed


Si-sub


ILD film composition analysis which was performed by taking  a SIMS depth profile using a CAMECA IMS instrument.


TEOS


No physical anomalies were observed by FIB cross section  and SEM inspection of the marginally failing unit. The failure


Gap


site in the highest resistance unit was isolated by PVC as  shown in Figure 2.


Figure 2:  Passive voltage contrast of test structure at metal-1.  The failure site is indicated by the arrow.


The sample was de-layered to reveal the surface of Metal-1  using chemical and mechanical processes.  Low kV PVC  imaging shows good grounded contacts as bright areas and  open or high resistance contacts as dark areas.  This isolated  the failure site, which was then cross sectioned by an FIB and  examined.


SEM inspection of the sample after highlighting using a slope


BPTEOS


etch showed a hollow Tungsten plug, as shown in Figure 3.


The tungsten plug defect could have been caused by particle W-plug,blocking, tungsten deposition anomalies, CMP anomalies,


improper post-CMP clean, or poor coverage of the next metal


Cosi


layer causing tungsten corrosion during photoresist removal. The zoom-in view shows that the contact glue layer was well  formed, but not enough tungsten was deposited into the gap


within BPTEOS and TEOS interface.  No particles were  observed within the tungsten contact and the contact was fully  covered by the overlying Metal-1 layer so both the particle  blocking and corrosion issues were ruled out.


Figure 3: A FIB cross section of the failing test structure  showing an abnormality in a tungsten plug (arrow).


PVC examination indicated no abnormal sites in the  marginally failing test structure where the resistance was only  a couple of ohms above normal. Nevertheless, TEM  inspection of the active and poly contact areas in the structure  was performed.  The TEM image shows that the tungsten plug  was fully deposited. However, a low mass-density, porous interface layer was found to be present between the TEOS and  BPTEOS layers as shown in Figure 4. The porous layer could


Failed Test StructurePVC Inspection


50.0um


correspond to the gap at the BPTEOS to TEOS interface seen  in Figure 3, which was subjected to a slope etch treatment.


The ILD layer from a good wafer shown in Figure 5 shows a  normal interface structure for comparison.


Figure 4: A low mass-density, porous type interface layer is  present between TEOS and BPTEOS layers.


Fail Contact Zoom-In View


400n'm(b)


PVC Isolation Site FIB Cut SEM Image


1.doum1(a)


1E+16 1E+17


niw


1E+18 1E+19 1E+20


1E+21


Approximate Concentration (Atoms/cm3)


0 0


poosy


d 18 p


1E+22 1E+23


150


250


Depth (nm)


1E+00


1E+01


1E+02inu 1E+0385 1E+04


1E+05


N->11B


P-Good Sample


0 u


SION


BPSG


P-Bad Sample


B-Good Sample


B-Bad Sample


Figure 5: The ILD layer from a good wafer shows a normal  PETEOS/BPTEOS interface for comparison.


SIMS depth profile comparison of good and bad wafers shows  the same boron concentration trend but the failing sample  showed abnormally low phosphorus content, decreasing  dramatically with increasing depth as shown in Figure 6.  Adding phosphorus dopant to silicon dioxide forms  phosphosilicate glass, which is a diffusion barrier to moisture, gathers alkali ions, and increases flow characteristics [3]. The  lightly P-doped material makes it easy to absorb moisture on  the BPTEOS film surface in the following processes [4].  This  moisture absorption, which revealed itself as a porous type  layer in the TEM image, could occur during the time between  BPTEOS densification and TEOS deposition. The water will  be desorbed during the subsequent high temperature processes


Figure 6: SIMS depth profile comparison of good and bad  wafer shows low P content on the failing unit.


of rapid thermal annealing (RTA) or tungsten deposition.


Thus the moisture diffused during the Ti/TiN glue RTA could be the cause of high contact resistance [1,2].  Water vapor  diffused through the TiN glue layer form s  a columnar structure during tungsten deposition, a phenomenon which is similar to the processes that occur during polysiloxane based  spin-on-glass (SOG) outgas that cause hollow via symptoms


[5].


To verify the failure mechanism, one partially fabricated test  wafer processed through contact etching with a thin layer of  Ti/TiN barrier metal deposited was annealed in the RTA  chamber.  After the clean process a small amount of water was  left on the surface of the wafer.  The wafer then underwent  standard processing through Metal-1 layer formation.  Subsequent WAT electrical tests showed increased contact  resistance.


TEM inspection of the contact test structure showed one  anomalous layer present between Ti silicide and TiN glue  layer as shown in Figure 7. An EDX line scan depth profiles  were conducted to detect the presence of O, Ti, Si, and W.  The results confirmed that the composition of the anomalous  layer is TiOx, which is the cause of high contact resistance.


Figure 7: TEM and EDX analysis of a high moisture test  wafer showed oxide growth between TiN and Silicide.


Ti


Si/W


O


W-plug


Si-sub TiN


TiSi


oxide layer


High moisture test wafer


In conclusion, not detailed enough FA data might cause  misinterpretation of the images, resulting in longer cycle times  and potentially more defective wafers. We have shown that by  combining different analysis tools such as SEM, FIB, TEM/EDX and SIMS analysis the root cause of high contact  resistance contacts can easily be determined.  This was further  confirmed by duplicating the failure mechanism using an  experimental wafer and recreating the atmosphere that created  the resistivity change.


The authors would like to acknowledge the members of  Failure Analysis and Product Engineering at WaferTech LLC.


[1] W. Qin, D. Alldredge, D. Heleotes, A. Elkin, M. Vadipour, B. Godek, N. Lerner, P. Fejes and N.D. Theodore. Microscopy and Microanalysis 13 (Suppl  2):1134-1135 CD 2007.


[2] H.Y. Chen and F.H. Lu,  J. Vac. Sci. Technol. A 23(4), pp. 1006-1009 Jul /Aug 2005.


[3] Peter, V. Z., Microchip Fabrication 5th ed. The  McGrawHill Companies., Inc. (2004), pp. 397-398.


[4] A. G. Thorness and A. J. Muscat , J. Electrochem. Soc., 150 (12) F219-F228 (2003).


[5] J.D. Romero, M. Khan, H. Fatemi and J. Turlo J. Mater. Res., Vol. 6, No. 9, pp. 1996-2003 Sep.1991.


# Failure Analysis Methodology on Systematic defect in ADC_PLL Ring Pattern due to Plasma De-chuck Process


Failure Analysis Methodology on Systematic defect in ADC_PLL Ring  Pattern due to Plasma De-chuck Process


Ang Ghim Boon, Chen Changqing, Alfred Quah, Magdeliza, INDAHWAN Jony, Lee Mern Tat, David Zhu, Neo Soh Ping  Failure Analysis Group, QRA, Global Foundries


Email Address: anggb@globalfoundries.com


In this paper, a low yield case relating to a systematic array of  failures in a ring pattern due to ADC_PLL failures on low  yielding wafers will be studied. A systematic problem solving  process based on the application of a variety of FA techniques  such as TIVA, AFP current imaging, layout path tracing, PVC  and XTEM together with Fab investigation is used to  understand the root cause as well as failure mechanism  proposed. This process is particularly critical in a wafer  foundry in which there is minimal available data on the test  condition setup to duplicate the exact failure. The ring pattern  was due to systematically open via as a result of polymer  built-up from plasma de-chuck issue. It would serve as a good  reference for a wafer Fab that encounters such an issue


In the wafer foundry industry, it is often quite tedious and time  consuming to perform failure analysis on Automatic Test  Pattern Generation (ATPG) and scan, BIST or functional  failure relating to low yield issue. This is due to the fact that  there is minimal available data on the test condition setup to  replicate the exact failure. For the scan/ATPG failure, TetraMax diagnosis followed by Laker software has been one  of the key diagnostic tools currently in the industry to debug  and analyze such failure [1]. This has greatly increased the  success rate of analyzing such failure contributing to the low  yield issue especially on logic circuitry. However, other types  of failure such as Analog circuitry malfunction is still one of  the big challenges for foundry FA engineers to work on.


One of the typical failure analysis approaches to work on  analog failures such as ADC_PLL without any available data  is to power up the chip using general Analog VDD and check  for any leakage or high resistance issue. In cases where I-V  curve tracing reveals presence of leakage or high resistance, further electrical fault localization by TIVA analysis will be  performed. Thermal Induced Voltage Altering (TIVA) is  considered as a powerful electrical fault isolation tool that has  been widely used in conductivity related failure analysis [2].


Another advanced FA technique that was engaged in this low  yield issue is Atomic Force Probing (AFP).  The AFP included  both the current imaging mode as well as nano-probing mode  for electrical characterization of the family of I-V curves for  probed transistors. It has been proved to be very useful as


compared to the traditional Passive Voltage Contrast (PVC) technique. This AFP current imaging mode is used to scan  across large poly capacitors for this low yield issue to check  for any leaky poly issue.


Figure 1: Example of the leaky poly capacitors identified from  AFP current imaging mode


Result and Discussion


A low yield issue was encountered in wafer fabrication with  the main failure relating to ADC_PLL circuitry. All the low  yielding wafers revealed a signature of a ring shaped pattern  of failures with different severity as shown in Figure 2. Based  on the wafer sort map, it was observed that not all the die in  the ring had failed. There were some passing die randomly  located in the ring. Besides that, according to typical test  sequence in the foundry industry, analog test such as ADC  was normally performed after all the continuity, power short, scan and BIST (logic and memory) test. In other words, all  these ADC failed die have passed the scan and memory test.


Figure 2: Wafers with failing ring pattern signature of  different severity


Both these two observed key symptoms of passing die in the  ring as well as failing at the later test stage suggested that the  issue may not be related to CMP but more prone to process  flaw related to specific structure or layout.


Typical failure analysis flow was first engaged in this low  yield issue. Being a foundry with minimal available data on  test condition setup, initial electrical fault localization  approach was to bias the general AVDD and AVSS to identify  any defective site. Unfortunately, TIVA / PEM analysis did  not show any TIVA/emission spots (Figure 2).


Figure 3: TIVA analysis by biasing the general Analog VDD  and VSS showed no distinct TIVA spot


Random top down SEM inspection on every layer in the  ADC_PLL block also did not show any physical evidence of  anomaly. Based on some preliminary Fab investigation and  equipment commonality between failed wafers, it was  theorized that the possible root cause could be due to charging  issues resulting from plasma de-chuck (This is the process of  removing the wafer from the ESC chuck)


Th knds d Tim


31x


K


Figure 4: AFP current Imaging on the poly capacitors in the  PLL block showed no leaky poly (i.e. the gate oxide of the


狁证


poly capacitor remained intact


With this equipment commonality data of plasma de-chuck  resulted charging issue that could directly damaged the gate  oxide in the capacitor structure, detailed AFP (Atomic Force  probing) current imaging was engaged to scan through the


poly capacitors in the ADC_PLL circuitry which was typically  more prone to damage under plasma charging issue. However,  no leaky poly was observed suggesting the gate oxide of the  poly capacitor remained intact (Figure 4)


Thereafter, a failing region of the PLL block was provided for  further analysis. Based on the provided diagram, it was  observed that there was some circuitry connecting both  capacitors as highlighted in Figure 5.


Poly Capacitors


PLL Block


Figure 5:  A failing region of the PLL block was provided for  further analysis.


Typically, for scan failures, TetraMax diagnosis followed by  Laker software can be used to debug such failures [1]. However, for this particular low yield case, there was no  Design Netlist, STIL and Library available for this device at  the time of analysis. This is also a scenario faced in foundry  industries due to lack of such critical information. In order to  resolve such problem, detailed manual circuit tracing was  engaged to understand the circuitry connecting to the poly  capacitors. A certain level of experiences within an engineer is  required for such a tracing task (Figure 6).


Manual Tracing


组


Poly


H


Caps


瑜


生


Figure 6: Manual Tracing was then engaged to understand the  circuitry connecting to the poly capacitors


Guided by manually traced failure path, layer by layer  deprocessing followed by PVC analysis showed a systematic  open Via3 on an M3 island (Figure 7).


Figure 7:  PVC analysis showed open Via3 on a systematic M3  island.


Further analysis by TEM revealed an unlanded Via3 with  embedded polymer found and Si Nitride that was already  etched (Figure 8). Further analysis on several other failing die  in the ring also revealed similar defect of unlanded Via3 at the  particular metal island.


Figure 8: XTEM revealed unlanded Via3 with embedded  polymer found and Si Nitride that was already etched


Thus, all these FA findings suggested that the cause of the  ADC_PLL failure was due to the open Via3 which resulted in  a disconnection between the 2 capacitors. The failure was very  systematic as it was located at a single specific structure. This  also explained why there was no failure of continuity, power


Metal 42


short, scan and BIST (logic and memory) tests. There was  bound to be some design sensitivity issue that easily results in


failure whenever there is a specific process malfunction.


Upon finding that the unlanded Via3 was due to the presence  of polymer through systematic failure analysis, there were  several questions relating to the wafer failure signature and its  actual failure mechanism.


Via3/Metal 3


Bad


1). Why does the wafer map reveal a ring signature?


2). Why is the unlanded Via mainly on Via3 and at a particular


>*


structure?


3). How does the plasma de-chuck process result in the defects  as seen?


4).What is the failure mechanism behind this effect?


Good


Based on the wafer sort map, the failing ring was actually not  directly at the edge. Instead, there was some distance away  from it. A detailed check on the wafer temperature distribution  showed that it is also has a ring pattern and lower temperature  at the ring location. In other words, it was observed that the  failing ring pattern exhibited on the wafer sort map correlated  to the lower temperature distribution ring (Figure 9). Cooling  effects will result in higher CxFy rich polymer generation and  build-up.


***


c*


471


425


**


收素


exE


Ch


Figure 9:  Wafer temperature distribution correlated to failing  ring pattern


Another key mystery linked to this low yield issue was the  systematic open Via3 observed at a particular metal3 island.  Based on the detailed GDS layout study (Figure 10), it was  observed that for this ADC_PLL structure, there were multiple  small poly capacitors on this block. These small poly  capacitors were connected together only at Metal 3. Thus, for  the Via3, it is considered to be connected to a much larger  poly capacitor as compared to Via1 and Via2. The much larger  poly capacitor also suggested that it will serve as a much  larger charge reservoir. The negative charge on the large poly  capacitor will in turn attract excessive polymer (positively  charged) back into the vias.


N2/H2NH3)(NH3)NH3


Figure 10:  A drawn layout to illustrate why the failed via is


Plasma


always at Via3


Failure Mechanism


Hydrophobic


Hydrophilic


As seen from the XTEM in Figure 5, the polymer was found  with the silicon nitride already etched away. This XTEM


H2/N2


O2/Ar


result suggested that after the Metal4 and Via3 trench etch 0s with the silicon nitride etch stop layer removed, there was


some polymer that was trapped back into the via hole from the


environment. The polymer build-up was the result of the


plasma de-chuck process.  Generally, during the plasma dechuck, the ESC chuck was at 0V while the plasma was still on.


The large poly capacitor on the wafer was negatively charged.


The positively charged plasma environment will first repel the


positively charged polymer from itself and toward the wafer


surface. Concurrently, the negatively charged poly capacitor


will serve as an attractive force and further attract the


positively charged polymer into via hole. Thus, this type of


repel and attract forces acting concurrently on the positively


charge polymer was suspected to result in excessive polymer


build up into the particular via 3 (Figure 11).


Figure 11:  A drawn diagram showing the large poly capacitor  is negatively charged together with the plasma environment  will result positively charged polymer to be attracted to Via  hole and leading to excessive polymer build up into the  particular Via 3


Further Fab Investigation and Corrective Actions


Besides the layout and plasma de-chuck process that resulted  in the polymer build-up on the particular via, further Fab  investigation showed that there are also other potential factors  that would result in polymer build-up. These factors include  the queue time as well as the gases used during the post etch  deplapA L


treatment (PET). During PET step, N2/H2 reacts with CxFy to  form an NHx polymer that reacts readily with moisture to  grow under atmosphere condition. It was observed that by


FF


using O2/Ar, inline scan showed that the polymer has been  reduced significantly (Figure 12). Besides that, the queue time


POLY CAPPOLY CAPPOLY CAPPOLY CAP


between etch to clean is also critical as the longer the queue


Wafor


time between these two process steps, the higher the  possibility of polymer build-up.


ESC


Figure 12: Reaction of N2/H2 and O2/Ar during the post etch  treatment (PET) step


A low yield issue relating to a systematic ring pattern due to  the ADC_PLL failure was discussed. Systematic problem  solving process based on the application of a variety of FA  techniques such as TIVA, AFP current Imaging, layout path  tracing, PVC and XTEM together with Fab investigation was


+ve charges


used to understand the root cause as well as the failure  mechanism proposed.


Polymer Repel


The ring pattern of failed die was due to a systematically open  via that was the result of polymer built-up from plasma dePolymer Attract


chuck issue. This example should serve as a good reference to


-ve charges


Large Poly Capacitoe


wafer Fabs that encounter similar issues. A good Design


WILL Wafer


robustness is critical to “withstand” process drift as seen from  this low yield case. Continuous adjustment of manufacturing


parameters as directed by FA findings has improved the yield


OV


of manufactured die which reduces overall production cost.


Plasma De-chuck


The authors would like to thank the EFA/ XTEM team for  the FA data and Ng Wee Loon for the failure mechanism  discussion


[1] GB Ang, CK Chan, KK Chua and CK Oh “TetraMax  Diagnosis and Laker Software on Failure Analysis  ForATPG/Scan Failures”, IPFA2006, pp217-221


[2] R. Ross, K. Ly, M. de la Bardonnie, L.F.tz. Kwakman, F.Lorut, M. Lamy, C. Wyon, “OBIRCH driven Failure  Analysis for Process Development of 120nm to 65nm  technology nodes” ISTFA 2004, pp.447-450


# Fault Isolation of Sub-surface Leakage Defects Using Electron Beam Induced Current Characterization in Next-Generation Flash Memory Technology Development


Fault Isolation of Sub-surface Leakage Defects Using Electron Beam Induced Current  Characterization in Next-Generation Flash Memory Technology Development


Go Nagatani, Kenneth Yu, Amalia Del Rosario, Max Sidorov


Spansion Inc., Sunnyvale, California U.S.A. Go.Nagatani@Spansion.com


Richard E. Stallcup II, Joel-Anthony Gray


DCG Systems Inc., Dallas, Texas U.S.A. Richard_Stallcup@dcgsystems.com


Electrically testable (end-of-line) scribe line monitors are key  tools for yield enhancement allowing isolation of yield  limiting sources to a smaller set of process modules. These  monitors are often laid out in non-addressable large arrays to  enhance the failure signatures without occupying substantial  real estate in the scribe lines. [1] This method of signal  enhancement allows detection of soft failures or low defect  density failures even in scribe line monitors, but at the cost of  making fault isolation significantly more difficult. Rapid  identification of the failure root cause in such scribe line  monitors can further accelerate the overall yield improvement.


This paper covers methods used to isolate single leaky  junctions in a test structure designed for Flash memory  technology development. The end-of-line Wafer Electrical  Test (WET) identified a population of test sites with high  leakage. It may be possible to isolate this failure through  micro probing or a combination of electrical testing and  physical structure modification by FIB, but at the expense of  spending numerous days. It will be shown that a combination  of Emission Microscopy (EMMI), Electron Beam Induced  Current (EBIC) characterization and a SEM nano probing can  drastically simplify the fault isolation process. Results of  nano-probing will also be shown to prove the level of leakage  detected in the faulty junction.


Electrical Failure Signature


A scribe line electrical test structure was designed to monitor  leakage failures of critical transistors. In order to maximize the  number of transistors that can be monitored in the limited real  estate available in scribe lines, various nodes of the transistors  were tied together during testing. Source side junctions, drain  side junctions, and gates were tied together respectively across  roughly 2500 transistors per test structure. This allowed ppm  level failures in such transistors to be monitored.


Figure 1 shows an electrical result from this test structure. Based on the analysis of all available data from this test  structure, the primary mode of leakage failure was identified  to be junction leakage. The high leakage sites exhibited microamps of current while nominal sites reported 10’s of nanoamps of current.


Figure 1: Electrical test results from the leakage monitor  showing delta of several magnitudes in leakage between the  nominal and outlier sites.


cp


We used a conventional laser scanning microscope embedded  in the Meridian FA system to raster scan a 1340 nm laser beam  across the device in the region of interest. An avalanche  photodiode (APD) converted the reflected light into a DC


C2m


signal (for imaging) and an RF signal at a selectable frequency


C21


办强


(for detecting circuit activity). The RF signal on the laser beam  amplitude is induced by time-varying voltage biases inside a


34


transistor causing free-carrier density changes in the depletion  region of the transistor. This reflected-light RF signal was


C22


amplified by a series of low-noise RF amplifiers and


Cat


monitored by a spectrum analyzer with real-time analog 0 output.


Modulation mapping gave us a direct view of every location in


the field-of-view the circuit that is active at a chosen


frequency. For our scan chain shift analysis, modulation


mapping clearly showed us both the data shifting through the


scan chain as well as the clock driving the flops.


Like EMMI, modulation mapping is well-suited to automation


because it does not require any modification of the test pattern


or hardware, aside from adding a loop command into the shift


pattern to keep it running. Unlike static and dynamic laser


techniques (OBIRCH, TIVA, SDL, LADA, etc.) it does not


require any special signals from the tester power supply or


pins.


Performing a measurement consists of navigating to the region


of interest, focusing the image, and acquiring the modulation


mapping signal. The LSM we used allowed simultaneous


reflected-light and RF measurements. Aligning the reflectedlight image to the associated CAD data thus also aligned the


MM image to the CAD.


The measurement was not strongly affected by laser power,


although we tended to operate with the maximum power the


detector could handle to optimize the SNR.


Figure 7. SIL reflected-light LSM image with FOV = 40x30 µm2 and scan chain cell boundaries superimposed.


We first performed a global CAD alignment between the stage  CAD coordinates and the CAD coordinate space using an aircoupled lens. The highest resolution air-coupled lens we used  was a 50x, 0.5 NA Mitutoyo IR objective. The modulation  mapping signal with this 50x lens did not have sufficient  resolution to localize circuit activity, but it was sufficient to  perform CAD-to-image alignment within approximately 1 µm.


We ultimately used a solid-immersion lens (SIL) for the MM  measurements of the circuit. The SIL provided sufficient  spatial resolution (approximately 0.25 mµ ) to observe activity


inside flops.


After aligning the CAD to the device, we navigated to the  location of the EMMI anomaly. Figure 7 shows the SIL  reflected-light image in this region. The image was taken at a  4x LSM hardware zoom and covers approximately 40x30 µm2.  The red boxes are the bounding-boxes of the flops in the scan  chain. The red cross-hair in the center of the image is the  location of the anomalous EMMI discussed earlier.


We acquired modulation-mapping images at both the data (at


2.75 MHz) and the clock (at 11.0 MHz) frequencies. As for  the EMMI measurements, all the data was logged and rendered  in CAD coordinates using in-house software described earlier  in this article.


0250


srL


DC


00


OCer


89


ox8


CO


C41


Figure 8. 11 MHz clock activity in the passing (top) and  failing (bottom) devices.


Figure 8 shows the 11 MHz clock activity in the passing (top) and failing (bottom) devices. The white regions roughly in the  center of the flops are created by transistors switching at the  clock frequency. The gray areas between the flops are noise. In  both the passing and failing devices we saw clock activity in  the flops, so it is unlikely the defect is in the clock distribution  network. This insight was not immediately obvious from the  EMMI data presented earlier.


08UEL02 2 52


5 009酸


说


92#00


trpa


ou


"


Figure 9. Data activity in the passing (top) and failing (bottom) devices.


Figure 9 shows the 2.75 MHz data activity in the passing (top) and failing (bottom) devices. Note that the data activity stops  in the failing device at flop 48 (indicated by the cursor in the  center of the image) and is not present for all following flops. In the passing device the activity is present in all flops, confirming our hypothesis from the EMMI data that the defect  is between flop 49 and 48.


oauj030(310206.5240.051um


cont


cas


026


贷粥


08


(3102 06. 5240 05Tum


cs


0t


2K


OK


49 48 0


DOL


R


CH


D830


39


0tda


861


O9


D9


农


证


OC


nDN


21


2C0


022


C25


CT


C2OCm


DaoC29


C289


C200


Cz


也


口重


OCD


25


C销


oe


Figure 10. Clock activity in the passing device (top) and


62


failing device (bottom). can


C272


Figure 11. Data activity in the passing device (top) and failing  device (bottom)


Figure 10 and Figure 11 show the clock and data activity, respectively, in the passing and failing devices with SIL at 8x  zoom. We see clearly that the data signal failed to propagate  from flop 49 to flop 48 and all subsequent flops.


Figure 12. Circuit layout superimposed on the modulation  mapping signal.


Figure 12 shows the circuit layout superimposed on the data  modulation mapping signal. Notice also that there is no  activity in the buffer between the output of flop 49 and the  input of flop 48. Two of the gates (shown in green) in the fan  out of flop 49 show data activity, but the lower one does not,.


C制


The lower gate receives data exclusively from flop 49, suggesting that there is a defect in the sub-net from the output  of flop 49 feeding the lower two gates, or in flop 49 itself.


The modulation mapping signal was consistent with the EMMI  signal, but provided significantly more insight into the exact  location of the defect.


contes


Car2


cN


conteor


ocb


hot


The modulation-mapping data was collected using our current  SIL which required thinning the device to 100 um. For wafer  work we would require a SIL compatible with a 700 um fullthickness wafer. Such a SIL is currently under development.


Physical failure analysis (PFA) was performed on the region  around flop 49. PFA confirmed that an open contact inside  flop 49 was causing it to fail, consistent with our analysis.


Throughput Considerations


Table 1. Additional time for EFA yield workflow for analyzing  shift failures (not including tester data logging and  processing)


|Activity (per die) |Actual Time |Target Time w/ Automation |
|---|---|---|

|Failure log anaysis |5 mins |5 mins |

|CAML file preparation (EFA measurement instructions) |5 mins |5 mins |

|Load wafer into system (one time) |2 hours |10 mins |

|Pin-to-pad alignment (one time) |10 mins |5 mins |

|Navigation to die |10 mins |2 mins |

|EMMI measurements |60 mins |10 mins |

|MM measurements |n/a |10 mins |

|Analysis |3 hours |10 mins |

Turn-around time is critical for yield ramp. A typical PFA  might take a few days, so to be useful the process of EFA in  yield ramp should be significantly less than that.


Table 1 shows the target throughput of each of the key steps in  the volume EFA workflow.  The CAML file is automatically  created and its generation will probably not become  significantly faster. Wafer loading and alignment has to date  been performed manually, but new software to integrate  several components significantly improves the loading time. 0


The EMMI measurement time should also improve  significantly with automation by elimination the need to  manually enter navigation coordinates and repeat  measurements because of human error. Most significantly the  data analysis time should be significantly reduced with better  net back-tracing. We are currently investigating several  approaches.


Summary and Future Work


We have shown how the combination of EMMI with  modulation mapping is a powerful scan chain shift failure  localization technique. Both techniques are well-suited to  automation because they require only a description of what  regions to measure. The test patterns and tester hardware are  the same as we use for production. All that is required is the  insertion of stop and loop commands in the production test  patterns.


However, there are still several challenges in the current  workflow.


The fundamental pieces of the workflow are in place, and we  have demonstrated that the measurements can be prescribed  automatically. However, current hardware tools do not allow  control by external software, so automation is limited. A  technician must read the measurements instructions from the  database application, collect the data, and enter it into the  database manually. This process is time-consuming and can  lead to errors. We are currently working with system vendors  to include an API to enable automation of the data equipment. Even with automation a technician will most likely be required  to load wafers, monitor the system, and perform other tasks, but the task of cataloging the collected data is best performed  by a machine.


The most important metric of success is how much the  workflow improves PFA hit rate and throughput, and  ultimately how much it shortens yield ramp. It is too early to  make any quantitative predictions. This work is ongoing and  will depend on a close collaboration with our vendors and  foundries in order to be successful.


Despite these and other challenges, we believe that combining  EFA with existing yield ramp activities is an important next  step for yield enhancement.


Acknowledgements


The authors would like to thank M. S. Chuang of TSMC for  his helpful insights and assistance.


i Stellari, F., P. Song, et al. (2004). Broken Scan Chain  Diagnostics based on Time-Integrated and Time-Dependent  Emission Measurements. ISTFA 2004, Worcester, MA.


ii Simon, P., M. Thétiot, et al. (2008). Yield enhancement  using a combination of wafer level Failure Analysis and defect  isolation software: case studies. ISTFA 2008: Proceedings  from the 34th International Symposium for Testing and Failure  Analysis, Portland, Oregon USA.


iii Kindereit, U., G. Woods, et al. (2007). "Quantitative  Investigation of Laser Beam Modulation in Electrically Active  Devices as Used in Laser Voltage Probing." IEEE  Transactions on Device and Materials Reliability 7(1): 19-30.


# Case Study in Fault Isolation of a Metal Short for Yield Enhancement


Case Study in Fault Isolation of a Metal Short for Yield Enhancement


Sarven Ipek, David Grosjean


Analog Devices Inc., 831 Woburn St. MS-511, Wilmington MA 01887, USA


The application of an individual failure analysis technique  rarely provides the failure mechanism. More typically, the  results of numerous techniques need to be combined and  considered to locate and verify the correct failure mechanism. In this paper we describe a particular case in which different  microscopy techniques (photon emission, laser signal  injection, current imaging) each gave clues to the problem, which then needed to be combined with manual probing and a  thorough understanding of the circuit to locate the defect.


Magnetic current imaging--either SQUID (Superconducting  Quantum Interference Device) or MR (Magnetoresistive or  GMR Giant Magnetoresistive Microscopy)--has been growing  steadily in importance and usage for integrated circuits [1]. SQUID can be used for PCB-level, package-level, and dielevel current mapping [2]-[4], while MR is better suited to dielevel imaging because of the smaller sensors [5]. For fault  isolation of electrical shorts, current mapping is often useful  by itself, but it can be even more powerful when combined  with the results of other techniques.


During the qualification process of transferring the production  of a part using a standard 0.5m CMOS process from one  fabrication site to another, a large yield loss was experienced  due to excessive current draw.   Several wafers with probe  maps were analyzed; the failing die exhibited excessive  current draw which was not only too high, but was observed  to be in integral multiples (2, 3, 4) of the nominal current  as specified by the data sheet. Optimistically, this suggested  that a single defect type was responsible and was causing  successive portions of the circuit to be activated. This paper  describes the thought processes and actions taken in  determining the failure mechanism and finding the defect, which involved the combination of various analysis  techniques and a detailed understanding of the circuit.


Analysis:  Defect Localization


The first steps in this analysis were the straightforward


investigation of any anomalies found with standard


inspections. Optical inspection of the failing die did not show rLany gross visual anomalies. Photon Emission Microscopy (PEM) analysis [6] of a known good die exhibited no emission


spots, while that of a known bad die exhibited numerous


spots, an example of which is shown in Fig. 1. Each of the


spots was examined optically, and a few of them were cross


sectioned with a Focused Ion Beam (FIB). No anomalies were


observed in any of the cross sections.


Figure 1. Example of photoemission spots on failing die.


Laser Signal Injection Microscopy (LSIM) using a 1340-nm  laser [7] was performed with the die biased between Vdd (supply voltage) and GND (ground). On the failing die, LSIM  revealed extra locations not present on the good die:  a single  signature and a double signature, corresponding to 2 and 3 current draws in the delay circuitry block (Fig. 2). These sites  were not present on any of the known good devices. FIB cross  sections of these sites yielded no anomalies.


Figure 2: LSIM signature sites correlating to a) 2 current  draw and b) 3 current draw. The yellow box denotes the  delay circuit block.


Continuing on the path of straightforwardly investigating any  sites noted by PEM or LSIM, several failing die were  deprocessed down to silicon using hydrofluoric (HF) acid and  then highlighted using a Wright etch. Optical inspection and  Scanning Electron Microscopy (SEM) inspection of the PEM  and LSIM sites yielded no abnormalities at the silicon level, ruling out silicon point defects or ESD.


These results by themselves were not useful in localizing the  issue; however, they helped by indicating that the emission  spots and LSIM signatures were not located at defects, but  were likely the effects of defects located elsewhere.


Analysis:  Current Imaging


The technique of magnetic current imaging [5] was essential  to the fault localization, since the data collected thus far  indicated only effects of the defect, not the defect itself. The  magnetic current imaging was performed on the  MicroMagnetics CS1000 on both known good and known  failing die. Compared to the current map of the good die, the  failing die showed extra current going to different locations. For example, Fig. 3 shows the current map around the PEM  spot (black arrows) from the top right of Fig. 1. We expect to  see current there, but the map is nevertheless informative.


Figure 3: Current mapping (red) superimposed on a few of  the photoemission spots (black arrows) found earlier (compare to top spot in Fig. 1). The yellow arrows point to  probe pads.


Other magnetic current imaging results pointed to high  currents going through the delay circuitry block where LSIM  signatures were found before. By overlaying the LSIM results  from Fig. 2 with the magnetic current imaging results as  shown in Fig. 4, it is clear that the excess current was going  from Vdd through the LSIM signatures to ground.


The large amount of current going through the delay circuitry  correlating with the LSIM signatures turned our focus to that  block, but it was still not clear that the problem lay there. In  Fig. 3, two probe points are labeled which are downstream of  points B & C in the delay circuitry block (Fig. 2b). The other  PEM sites were similarly downstream of the delay circuitry. Thus, since the delay block and the PEM sites were  connected, it was still not possible to separate the cause from  the effect. To do this required understanding the inputs and  outputs of the delay block and how it works internally.


E Vdd


F GND G


Figure 4: Magnetic current imaging results (red) superimposed on the LSIM signature spots (circled) recorded  in Fig. 2a & b signature sites. The yellow box labels the test  points under passivation connecting to the delay circuitry.


Emission Microscopy (EMMI)


EMMI was used as the first method, which is typical for  leakage failures of the type described in this paper. [2] This  method was expected to be a challenge for this failure mode  due to the low level of leakage detected in these structures. As  seen in Fig. 1, the leakage levels were on the order of microamps, and the power output was on the order of micro-watts  with only a few volts applied during testing. Considering the  upper limit of applicable bias to be gated by junction  breakdown, the measured leakage during WET was bordering  on the EMMI detection limit.


A site with the highest leakage level measured during WET  was selected for EMMI, and as Fig. 2 shows, a photon  emission spot was successfully identified. This EMMI result  was vital to this investigation as it proved the failure to be  driven by a point defect rather than a global increase in  leakage across the entire structure.


Figure 2: Emission microscopy image showing a hot spot  several microns in diameter located in the failing test  structure (white arrow pointing to red dot).


Although the presence of an emission hot spot significantly  reduced the failure area of interest, the lack of resolution of  the EMMI became an apparent problem. In this structure, the  hot spot that is several microns in diameter can easily cover  more than 40 junctions. The number of possible failure sites  was therefore too high for blind physical failure analysis to  confidently identify the root cause.


Electron Beam Induced Current (EBIC) Characterization


Electrical test and optical techniques failed to pinpoint the  defect in this scribe line test monitor. As a result another  technique, EBIC characterization, was needed to better  localize the fault. The structure was deprocessed to remove all  metal traces that connect the active contacts. Additional top  down optical and SEM inspection post deprocessing did not  yield any indicators that could further localize the failure  within the EMMI hot spot.


A SEM was equipped with a nano-probing system capable of  placing tungsten nano-probe tips on any of the exposed active  contacts enabling local signal injection or extraction. In  addition, the SEM beam was used as a moving stimulus probe  that produced electron hole pairs (EHPs) at each of the active  PN junctions. The SEM beam energy needed to be high  enough, 6keV and 100pA in this case, to allow the electrons to  penetrate the insulating material above the PN junctions and  stimulate EHPs within the PN junctions. With 2 nano-probe  tips connected across the PN junction, EBIC was collected and  amplified. [3] An EBIC image was generated by correlating


the EBIC signal with the SEM beam location shown in Fig.3. At defects in each local PN junction, the EHPs quickly  recombine before they can separate and reach the probe tips. This decreases the collected EBIC signal at that location, resulting in a corresponding dark spot in the EBIC image. Together, the SEM and the nano-prober form a system that  can make connections to isolated PN junctions and visualize  defects deep within the junctions.


Utilizing the data obtained from the EMMI, subsurface areas  surrounding the EMMI hot spot was the focus of EBIC  characterization. As shown in Fig. 2, nano-probe P1, connected to the EBIC amplifier ground, was landed on the  well contact at the right end of the line corresponding to the  EMMI hot spot. Nano-probe P2, connected to the EBIC  amplifier input, was then landed on the first active contact  near the well contact, diode D1 row 2. Simultaneous EBIC  and SEM images were captured and then overlaid to produce  the false color composite of Fig. 3.  The EBIC image was  collected with the amplifier gain of 109 volts per amp. In the  lower right hand corner of Fig. 3 probe P1 and probe P2 are  visible.


The third probe shown in Fig. 3 is one of 6 other spares, totaling 8 probes, which could be used for electrical  characterization of more complex circuits. Since probe P2 is  directly connected to diode D1, the EBIC signal at that  location is very large and is represented by the very bright  oval region surrounding probe tip P2 and D1 row 2. The signal  at the center of the oval is so large that the EBIC amplifier is  saturated and is represented by the black spot in the center.


Figure 3: A false color composite of EBIC image in blue and  SEM image in grey showing the local failure sites at D44 and  D15. The EBIC amplifier is connected between the probes P1  and P2.


Since the upper layer metal lines were removed, the  conductive path between all of the other diodes along the  active contact line was poor. As a result the EBIC signal  coming from the other diodes that reached probe P2 and the  EBIC was decades lower. This is the reason why the EBIC  amplifier gain needed to be set to 1 volt per nano amp.


At locations D15 row 1 and D44 row 2, a clear reduction in  the EBIC signals was observed and shown in Fig. 3. There is  good correlation between the EMMI hot spot data of Fig. 2, which points to the general area and the decreased EBIC  signal at location D44. There is no EMMI data that correlates


1E-4


to D15 row 1 as this junction was connected to a node that was


1E-5


not evaluated for EMMI. A weak EBIC signal generally could


d1E-6


mean open or short to the well or irregularities in the implants,


however, based on the WET results, a leaky defect is expected


u 9


-鲁-D14


1E-7


for this particular sample.


d1E-8


--D15


5


---D16


01E-9 8


61E-10


Nano-Probing IV Characterization


1E-11


1 o


1E-12


SEM based nano-probing has become an invaluable technique


-1.2-1-0.8-0.6-0.4-0.20


for locating soft fails by extracting parametric data directly


Active Contact Voltage (Volts)


from isolated devices of 90nm process and below. [4] With  extra nano-probe tips already near the test structure and  connected to a Keithley 4200 parametric analyzer, further  characterization of the suspect diodes was possible without the  need to stop and re-cable. The two extra probes needed for  two point diode measurements were connected to the analyzer  preamps via triaxial cables. One probe was moved to the  location of the active contact corresponding to the low EBIC  signal and a second probe to the corresponding row well  contact. For reference, IV curves were collected from active  contacts immediately left and right of the low EBIC signal.


Fig. 4 shows the current vs. voltage (IV) curves of D45, D44, D43 and D1 of row 2. The voltage sweep was initiated at 0  volts to minimize the possibility of altering the defective  diodes. The IV curves from D44 corresponding to the low  EBIC signal did not remotely resemble their neighboring  diodes. The defective junction behaved ohmic rather than  diode and confirmed that the active contact is shorted to the  well.


w


---D43*1E-8n


-044 0


1E-9


M


-1.2-1-0.8-0.6-0.4


-0.20


1E-10


--045-D1


Figure 4: Nano-probing current vs. voltage curves of failed  diode, D44, and reference diodes D1, D43, and D45. Diode 44  corresponds to the weak EBIC signal of active contact row 2.


Fig. 5 shows the IV curves of D16, D15, and D14 of row 1. Similar to D44, D15 behaved ohmic unlike its surrounding  junctions proving to be yet another shorted junction. The


EBIC technique proved to be more versatile than EMMI as it  was able to detect failures in all PN junctions located within  the same well, while EMMI was restricted to the test structure  node that was under bias.


Figure 5: Nano-probing current vs. voltage curves of failed  diode, D15, and reference diodes D14, and D16. Diode 15  corresponds to the weak EBIC signal of active contact row 1.


Physical Failure Analysis


With the identification of a single faulty junction by EMMI  and EBIC characterizations, a targeted physical failure  analysis would most certainly identify the root cause of the  failure. Fig. 6 shows the cross-sectional TEM (XTEM) result  of a cut made at the junction of interest. A silicide  encroachment growing at 45º towards the channel region was  found to be the culprit behind the junction leakage seen in  WET during early stage of technology development. It has  been reported by others that such silicide encroachment to be  causes of off-state leakage-current in MOSFETs. [5]


Figure 6: XTEM of the EMMI and EBIC isolated failure  location shows silicide encroachment to be the source of  junction leakage in the test structures during the development  stage of technology development.


This paper successfully demonstrated the sequence of failure  analysis methodologies used to identify the cause of junction  leakage in a test structure where fault isolation was difficult  during early technology development. A combination of  EMMI and EBIC characterization was able to pinpoint the  problematic junction from approximately 2500 junctions in the  structure. Furthermore, the nano-probing IV characterization  proved the identified junction to be indeed high in leakage  current, providing further confidence for physical failure  analysis. Finally, XTEM of the area of interest identified  silicide encroachment from the source-drain region towards  the channel region to be the physical source of the leakage  allowing the technology development team to address and  eliminate the defects.


The authors of this paper would like to acknowledge the  contribution by Bryan Tracy of Spansion Inc. and Glenn  Maley of DCG Systems Inc. for bringing the team together for  this collaboration.


1. C. Hess, et al, “Scribe Characterization Vehicle Test Chip  for Ultra Fast Product Wafer Yield Monitoring”, Proceedings of International Conference on  Microelectronic Test Structures, IEEE, p110 (2006)


2. JCH Phang, et al, “Review of Near Infrared Photon  Emission Microscopy and Spectroscopy”, Proceedings of  the 12th International Symposium on the Physical and  Failure Analysis of Integrated Circuits, IEEE, p275 (2005)


3. H. J. Leamy, “Charge Collection Scanning Electron  Microscopy,” Journal of applied Physics, V53(6), 1982, P. R51


4. L. Liu, Y. Wang, H. Edwards, D. Sekel and D. Corum, “Combination of SCM/SSRM analysis and Nanoprobing  technique for soft single bit failure analysis”, in Proc Int  Symp Testing & Failure Analysis (ISTFA 2004), 14-18  Nov 2004, Boston, MA, USA, 2004, pp. 38-41.


5. T. Yamaguchi, et. al, “A Novel Low Leakage-Current Ni  SALICIDE process in nMOSFET on Si(110) Substrate”, Electron Device Meeting 2007, IEDM 2007, pp. 139-142.


# A case study: Observation of counter doping of gate poly and its validation in high density 90nm CMOS SRAM Bitcell


A case study: Observation of counter doping of gate poly and its   validation in high density 90nm CMOS SRAM Bitcell


Yuk Tsang*, Xiang-Dong Wang, Michael Mendicino, Andrew Blankenship


Freescale Semiconductor Inc. 6501 W. WM Cannon Drive  Austin, TX 78735


(*) Corresponding author: ra0149@freescale.com (512)-895-3905


Threshold voltage (Vt) shift was measured, using atomic force  probing (AFP) technique, in the pullup PFETs of high density  SRAM bitcell arrays in 90nm CMOS bulk technology.  This  shift caused catastrophic yield loss. The direct measurements  of dopant distribution both in plan view and x-section using  Scanning Capacitance Microscopy (SCM) technique  suggested counter doping of the P-poly had occurred. A single  mask modification was shown to validate the observation and  eliminated the counter doping resulting in drastic yield  enhancement to about 60% from nearly no yield.


High density CMOS devices have presented a constant  challenge for technologists to achieve consistent high yield. To facilitate fast feedback for process corrections, built-in  SRAM arrays have been routinely utilized for defect  identification. Due to its high density and design, single bit  fails are typically at the top of the bitfail Pareto. Therefore, the  understanding of single bit fails is very important for process  corrective actions. For standard 6-transistor bitcell arrays, the  defect is most likely embedded in the layers below the second  metal level. The analysis could be rather simple for single bit  failures. Advanced focused ion beam (FIB) systems with dual  beam and ultra high resolution capability have been routinely  used to find the physical defects with a high success rate. Transmission electron microscopy (TEM) analysis is used to  analyze subtle defects once the defect site is isolated by other  techniques. However, significant numbers of single bit fails  are “soft” fails that pass certain voltage levels but fail the  others. These voltage sensitive bits (VSB) typically lack  visible physical defects, and thus FIB, TEM analyses will fail  to find the defects. We have experienced the VSB fail type  that caused catastrophic yield loss during the development and  manufacturing of a 90nm node bulk CMOS technology. While   the electrical signature was high Vt as measured in the PFETs  by Atomic Force Probing (AFP) at the contact level, the origin  of the problem was unknown as the sources for high Vt could  be numerous, such as random defective channel implant, poly


grain size [1], and thus requires thorough investigation to  pinpoint the root cause for corrective actions.


In this paper, we discuss the analytical approach that  successfully determined the invisible defect. We first  postulated counter doping of the P-poly as the cause for the  high Vt. Then, we probed the failing PFETs for direct  evidence of dopant anomaly in the Poly using SCM technique. We subsequently performed a controlled split experiment  using a single mask modification to validate the observation  and prediction.


EXPERIMENT


The layout design of the standard 6-transistor bitcell is shown  in Fig. 1. A known single bit fail in the SRAM array was  unlayered down to the contact level from the top metal using a  combination of wet, dry, and polishing techniques. An AFP  system [2] was used to electrically characterize each of the six  transistors. Four heads were utilized to access the drain, source, gate and substrate of each transistor.


Pass gate NFET


Pullup PFET


Pulldown NFET


Pass gate NFET  Pullup PFET


Phosphorus implant opening (05N)


Boron implant opening


(05P)


Phosphorus implant opening


(05N)


Fig. 1  6-transistor SRAM bitcell at first metal. Green=poly, yellow=active, gray=contact. Poly implant masks in dashed  boxes are also super imposed. The other back-end levels are  not labeled


SCM was employed to directly image the dopant regions and  types. The SCM measurements were done on a DI3100 system  with the SCM module [3]. The detailed description of the  SCM technique can be found elsewhere [4]. The tool is setup  to measure the derivative of capacitance (dC/dV) between the  conducting probe and silicon (with a thin oxide in between) while a small modulation voltage is applied to the probe.  The  amplitude of dC/dV is related to carrier concentration (smaller  amplitude for higher concentration in most cases), while the  dopant type can be obtained from the phase shift. In this study, p-type carrier is imaged brighter than the background (metal  or insulator), while n-type carrier is imaged darker. However, the contrast variation can be complicated near the junction  areas where carrier depletion occurs.


To prepare x-section surface for SCM, the samples were  polished with diamond lapping films and colloidal silica. Prior  to polishing, the top surface was coated with metal to short all  the contacts so that they are in the same potential level. FIB  marks were also made on the sample for x-section polishing. During FIB marking, care was taken to minimize the beam  exposure to avoid damage to the devices or to alter electrical  properties. Finally, the samples were exposed to UV light  while baking at ~300°C to grow a thin but robust oxide and to  remove the charges on the surface.


To prepare the surface for backside plan-view SCM imaging, the front of the sample (at contact level) was first coated with  metal and glued to a conducting plate with silver epoxy. The  backside was then polished down with diamond lapping films  and colloidal silica until the poly is reached.


RESULTS


AFP measurements were performed with substrate and source  biased at 0v, while the drain and gate voltage was swept from  0v to -1.8v independently, as illustrated in the insert in Fig. 2. It was observed that only the pullup PFET was abnormal  while the other transistors were normal. A typical PFET I-V  characteristic plot is shown in Fig. 2a. The abnormal PFET  shows a higher turn-on voltage as shown in Fig. 2b. The Vt  determined from the Id-Vg plot, shown in Fig. 2, taken at Vd=-0.2v is -0.5v and -1.2v for the normal PFET and the abnormal  PFET respectively. The Vt shift for the failed PFET is 0.7V  more negative in this case.


SCM analysis was subsequently performed in both x-section  and plan view to investigate any dopant issues. Fig. 3 shows xsection SCM images obtained as a function of sample bias Vb. The images contain four PFETs in two adjacent bit cells. The  overall implant regions can be best illustrated in the SCM  image taken at 0V, where S/D, S/D extension, channel regions  can be well identified. The top of the channel regions of the  three good transistors is used here to serve as the reference  location of the gate oxide. Due to high p-type concentration in  the gate poly, the SCM signal has very little contrast and does  not change noticeably as sample bias changes. In contrast, the  poly area of the high Vt PFET shows that the poly is lightly


Vd=-.2v


Vd=-1.8v


-1.7 -1.6 -1.5 -1.4 -1.3 -1.2 -1.1 -1.0 -0.9 -0.8 -0.7 -0.6 -0.5 -0.4 -0.3 -0.2 -0.1 0.0


2.0


-2.0


-4.0-6.0-8.0-10.0-12.0-14.0-16.0-18.0-20.0-22.0


、


-24.0


-26.0


-28.0


-30.0


-1.8


-32.0


d


g


4


-.2v


-1.8v


-1.9-1.8-1.7-1.6-1.5-1.4-1.3-1.2-1.1-1.0-0.9-0.7


-0.8


-0.6


-0.4


-0.3


-0.2


-0.1


-1.8 -1.7 -1.6 -1.5 -1.4 -1.3 -1.2 -1.1 -1.0 -0.9 -0.8 -0.7 -0.6 -0.5 -0.4 -0.3 -0.2 -0.1 0.0


Vg (V)


Fig. 2 Bitcell Pulldown PFET Id-Vg characteristic plots  measured by AFP microprobing: (a) Typical, (b) Anomalous. Vd and Vg was each swept from 0 to -1.8v @-0.2v/step, and  Vs=Vsub=0v. Typical Vt = -0.5v and the anomalous Vt =-1.2v  was determined from the curve at Vd=-0.2v


doped, evidenced by the significant contrast change as sample  bias changes.


c) Vb = -2.0V a) Vb = +1.0V


b) Vb = 0V


Fig. 3 Cross-section SCM images. The series of bias  dependent SCM images show that high Vt PFET has much  lower p-type concentration as its contrast has large swing as a  function of sample bias. The other good gates do not show any  noticeable contrast due to very high p-type level. The high Vt  PFET is circled in red. (Dashed lines indicate the expected  gate oxide location. Image size is 4umx1um.)


P+ poly


P+


P+D


Sub


N


Backside plan view SCM images further confirmed the  abnormal poly-doping issue. Fig. 4 shows backside SCM  image of another high Vt sample, along with topographic  image for bit cell registration. In these images, the p-type poly  areas are imaged brighter. Again, the poly on the failed bit has  p-n junction moved well into the channel area, as highlighted


with the dashed black lines.  At this point, while the doping  concentration level was not quantified, it was clear that the  high Vt PFET gate poly was lacking in P+ dopant  concentration.


N-type poly


P-type poly


source


drain


ox


Reference center line


Top view


Cross-section


Fig. 4 Backside plan view SCM images. a) Topographic image with superimposed bit cell (green-poly, purple-active, pink-contact), b) SCM image of the same area. The high Vt PFET is circled. Dashed lines represent the center of the channel regions. The insert shows  the extent of the counter doped region in planar and cross-sectional views. Note that the cross-section is a reconstruction of the PFET  transistor structure by adding P+, substrate and gate oxide to the backside that was removed.


HYPOTHESIS and DISCUSSIONS


Failure with high PFET Vt has been particularly alarming in  recent years due to process complexity and design  requirements in ever decreasing CMOS device dimensions.


More recently, high PFET Vt due to the formation of large  poly grains was reported [1], and rapid thermal anneal  treatment was employed to solve the problem. As mentioned  before, causes for high Vt are many. Therefore, it is of utmost  importance to identify the most probable cause to set for the


best solution path. In our case, in light of the AFP electrical  and SCM physical characterization information, we evaluate  PFET gate poly counter-doping as one of the most plausible  causes as outlined below.


1. Analytical assessment


Threshold voltage, Vt, of MOSFET is given by


Vt = Vfb - QB/Cox + φs                 (1)


and


Vfb = ΦMS  -  Qo/Cox ~ ΦMS           (2)


where Vfb is flatband voltage, QB is induced charge in silicon,  Cox is gate oxide capacitance, φs is surface potential, ΦMS  is the  work function, Qo is surface state charge. Note that charges  and oxide capacitance are per unit area.


In the case of P+poly, Vfb is ~ΦMS ~0.9V [5-6] whereas in the  case of counter doped poly, Vfb can be determined by the  measured Vt mismatch between the normal PFET and the  counter doped PFET. Vfb in the counter doped PFET is  determined to be ~0.2v using Equations (1) and (2). Therefore, ΦMS is changed from about 0.9v to 0.2v. This means that the  total oxide voltage would be lower in the counter doped PFET.


2. Root cause postulate


The basic 6-transistor SRAM bitcell is shown in Fig. 1 with  the poly implant masks superimposed. Design rule check  verified there was no design rule violation in the bitcell layout, and thus eliminated the mask error as the problem source. The  N+poly is achieved with N-type implant through window  opening mask (05N). The P+poly is achieved with P-type  implant through window opening mask (05P) which is the  inverse of mask 05N. The latch pair shares the same gate poly  line with the pullup PFET. Since the pullup PFET size is  noticeably much smaller than the pulldown NFET, the  phosphorous can counter dope the PFET poly entirely if the  implant opening window (05N) is too close to the PFET gate  region without allowing for adequate margin for process  defect, such as photoresist patterning edge roughness. When  this happens the work function will be changed, resulting in  higher Vt as described above in this discussion section.


Another possible cause is the formation of large poly grain at  the PFET resulting in dopant loss through diffusion into grain  boundaries. It will be shown that this was not the cause in our  case.


VERIFICATION and SOLUTION


To verify the counter doping mechanisms described above had  occurred, a controlled split experiment was performed by  changing mask dimensions related to poly implant. For half of


bits failing singleNumber of die


the lot, the 05N mask implant window opening was decreased  by 125nm at the edge toward the PFET, as shown in Fig. 5. This will move the phosphorous implant farther away from the  PFET gate area. The 05N mask for the other half of the lot  remains unchanged. There was no other process change for  both halves. The test results are shown in Figs. 6-7 and Table


1.  The bitmap signature for the control was characterized by


Reduced by 125nm


Fig. 5 Phosphorus implant window opening change: Blue  shape is original size; Slashed yellow shape is new size  reduced by 125nm at the PFET side.


single bit fails that were extremely voltage sensitive as shown  in Fig. 6, and the yield was low as shown in Fig. 7. However, the yield was drastically improved in wafers with implant  moved by 125nm away from the P-gate. The corresponding  VSB bitfails were also reduced to essentially none as shown in  Fig. 6. The contrasting test results clearly verified the  Phosphorus counter doping theory.  Implementation of the  05N modification in ensuing wafer lots had consistently  yielded good results as shown in Fig. 8. It is noted in Fig. 6  that after removing the systematic counter doping failure  mechanism, voltage insensitive bit fails remained. These hard  bit fails were due to baseline random defectivities. These  defects, usually visible, had limited the yield to reach its full  potential. Since the analytical and experimental results  presented here had successfully solved our high Vt issue, the  plan to attempt the rapid thermal anneal to minimize poly  grain size and enhance uniformity [1] was not carried out.


0 100 200 300 400 500 600


W#7


W#9


W#8


W#10


Wafer ID


Hi Vdd Lo Vdd


05N-not modified


05N modified


Fig. 6 Single bit fail comparison between the control wafers  without 05N modification and the experimental wafers with  05N modification. The results show the control group suffers  high single bit fail and extremely voltage sensitive.


Dare I


Fig. 7  Final test wafer map showing the 05N modified portion  yielded 55-60% (group at top) while the control portion  without 05N modification <2% (group at bottom). Each wafer  received identical processing, except the 05N mask sizing  difference. Color code: green is good die, all others are bad  die.


TOARS


Eowor


Fig. 8 Final test wafer map where green is good die: (a) full  lot with original phosphorus implant mask 05N, (b) full lot  with modified 05N mask.


Table 1   Controlled split experiment yield and VSB results


|Poly implant mask |# of |die/wafer with single bit fail |Yield |
|---|---|---|---|

|Poly implant mask ||Low Vdd                  High Vdd |Yield |

|Original 05N |400+/-60 |400+/-60 |150+/-5 |

|Modified 05N |67+/-2 |67+/-2 |56+/-3 |

Bual: 39:45


Bin1:54


482 06 839


434 of 839


DD17854_08


DD17854_10


CONCLUSION


Birc 1


Ban: 1


In high density SRAM bitcells with minimum design rules, a  conventional CMOS platform process was found to be very  susceptible to poly counter doping. The counter doping had  resulted in work function change resulting in Vt shift, and thus  seriously degraded yield. A simple one-mask modification had  eliminated counter doping resulting in drastic yield  enhancement. Thus, a unique and vital process integration  solution was implemented. The work presented here should be  useful for more aggressive and complex IC device


8m1:19


8nl:199国


manufacturing.


10 of839


13 of839


DD17854_07


DD17854_09


The authors wish to thank B. Winstead for technical  discussions and the Freescale Semiconductor Technology and  Manufacturing Center, Austin, for providing the samples.


REFERENCES


[1]    S. Ikeda, Y. Yoshida, K. Ishibashi, and Y. Mitsui ‘Failure analysis of 6T SRAM on low-voltage and


high-frequency operation,’ IEEE Transactions on


Electron Devices, Vol. 50, No. 5, May 2003


[2]     Multiprobe Atomic Force Probing System manuals on


facility requirements and specification, installation,


maintenance, and user guide


[3]       Digital Instruments, Veeco Metrology Group.


[4]       C. C. Williams, ‘Two-dimensional dopant profiling by


scanning capacitance microscopy’, Annual Review of


Materials Science, Vol. 29: 471-504 (1999)


[5]    A. Gupta, P. Feng, M. Song, M. Lin, D. Wollesen, K.


Chen, and C. Hu, ‘Accurate determination of Ultrathin


gate oxide thickness and effective Polysilicon doping


of CMOS devices,’ IEEE Electron Device Letters, Vol.


18, No. 12, December 1997


[6]    C.Y. Wong, J. Sun, Y. Taur, C. Oh, R. Angelucci, and          B. Davari, ‘Doping of N+ and P+ polysilicon in a dualgate CMOS process,’ IEDM p 238, 1988


# Magnetic Microscopy for 3D structures: use of the Simulation Approach for the precise localization of deep buried weak currents


Magnetic Microscopy for 3D structures: use of the Simulation Approach for the  precise localization of deep buried weak currents


Fulvio Infante1,2, Rodolphe Gomes2, Philippe Perdu21FAST, Toulouse, France 2CNES, Toulouse, France  fulvio.infante@cnes.fr


Fabien Battistella, Sebastien Annereau


Thales IT, Toulouse, France


Dean Lewis


Université Bordeaux 1, Talence, France


With the innovations in packaging technologies which have  taken place over the last decade, new assemblies often include  an increasing number of dies inside a single package. This is  exactly what was predicted by the More than Moore’s  paradigm: as the integration of ICs increases, the  heterogeneity of the devices found in a single package  increases. As a result, the number of potential failures which  can appear at assembly level has increased exponentially. At  present, no technique has been able to precisely localize  defects which are deep inside a complex package. For this  reason, a new technique for failure localization for threedimensional structures is needed. In this paper the technique  proposed, based on the coupling of magnetic measurements  and simulations, is applied to a three-dimensional structure to  precisely localize the current path which is buried deep inside  it. A new method, based on parameters fittings of magnetic  simulations, is then applied in order to accurately evaluate the  distance between the current and the sensor.


Over the years, Failure Analysis has provided the solutions  needed by designers to improve the quality of electronic  devices. This has allowed industry both to save the money  which would have been needed for customer returns of failed  systems, and to keep increasing system performances by


pinpointing and improving the weak points of the devices. However, with the coming of System in Package technologies


[1], the old techniques for failure localization can no longer  be used. More and more new devices are being developed in  three dimensions [2], where the complexity of the assemblies  make the task of the failure analyst increasingly difficult. At  present, all the techniques which can be used to localize a  defect in such systems require preventive depackaging. However, the analyst must already have quite a precise idea  where the defect lies. Without this knowledge, there is a very  high risk of destroying the defect and therefore losing all its  information while opening the package. The example which  will be shown in the present paper is one such case: if we had


proceeded to open the component, we would have lost the  defect. We developed a technique which is able to pre-localize  current leakages in a contact-less way without opening the  circuit. This technique is therefore able to respond to the need  for failure localization of three-dimensional components.


In this paper we will show the advances we have made with  the magnetic microscopy technique and apply them to a fully  three-dimensional case study.


Magnetic Microscopy


Magnetic Microscopy is a non-invasive contactless technique  for defect localization. It uses the effects of the Biot-Savart  law to precisely localize current leaks at die and at assembly  levels. This law gives the distribution of the static Magnetic  Induction Field generated by a current flow:


ˆ


4 r


r


l


I


ddB


×


πμ


(1)


We know that when a current flows inside an electrical  conductor, it generates a magnetic induction field according  to this law. This is shown in figure 1:


Figure 1: Magnetic Induction Field generated by a current  line


From this diagram we can see that the z component of B is  zero at all the points which are directly above the current line. If we acquire the field on a line perpendicular to the current, we obtain a curve similar to one of those in figure 2. The  actual shape of the curve will depend on the ratio between the  current amplitude and the Working Distance (WD), i.e., the


distance between the magnetic source (the current in this  case) and the measurement plane. As this ratio decreases we  lose the two peaks of the curve. These peaks carry the  information about the WD. This means that as the sensor gets  further from the current, obtaining information about the z  values becomes increasingly difficult.


Figure 2: Magnetic acquisition curves for a current of  500mA at a distance of respectively 5µm (blue), 10 µm (green), 50 µm (red) and 100 µm (purple).


The two unknowns of the Biot-Savart law are the magnetic  induction field and the current vector. The law provides a  solution for evaluating B once the current distribution is  known. For our purposes we need to do the opposite: evaluate  the current distribution from the measurement of the z  component of B. This is what is referred to as the Magnetic  Inverse Problem.  Its solution has been demonstrated under  some hypotheses [3][4]: the current distribution was evaluated  from measurements of the z component of the field on a  constant x-y plane.


Magnetic Current Imaging


The technique which applies the solution to the inverse  problem is called Magnetic Current Imaging (MCI). This  technique has been developed and implemented by Neocera in  the Magma C20/C30 magnetic microscope. This tool can  produce very precise current cartographies by measuring the  magnetic field above the device. The tool used is shown in  figure 3.


A range of sensors can be used to pick up the magnetic field; the one most often used is the SQUID. This is also the sensor  which is used in the Magma systems. The SQUID is the most  sensitive magnetic sensor, and allows the mapping of very  weak currents from a large distance [5][6]. The drawback is  that it uses superconducting Josephson junctions to pick up  the magnetic flux: this means that the equipment must work  at very low temperatures. The other sensors which are used  are the GMR and the MTJ. These allow for better spatial  resolution, but need a shorter distance between the sensor and  the current in order to give meaningful solutions [7].


The MCI technique has also been developed to localize highly  resistive opens by carrying out a difference analysis between  magnetic scans performed on faulty and reference devices


[8][9].


Figure 3: Neocera Magnetic Microscope


Technique Limitations


Whilst the MCI technique is extremely useful, it does have  various limitations. The spatial resolution of the technique  can be affected by several factors. Not only does this depend  on the sensor type, as explained above, but also on the  distance from the current to the sensor (the working  distance): the larger this distance, the worse the resolution. The spatial resolution also depends on the magnetic noise, as  explained in [10].


Another limitation is that the magnetic inversion algorithm  can only process two-dimensional current distributions. The z  component of the current distribution does not generate any  contribution to the z component of the magnetic induction  field, as they are always perpendicular to each other. Therefore it is impossible to map vertical currents.


Finally, if the currents flow on different x-y planes, the  solution of the inversion is not unique. This means that the  result of the MCI algorithm will present some artifacts: the  currents which flow closer to the sensor will be shown as  stronger, while those which flow further from it will be  shown as weaker.


The Simulation Approach


In order to overcome these limitations, the MCI technique has  been developed further in a number of ways. One of these is  the simulation approach. It consists in generating a set of  magnetic simulations based on hypotheses of the layout of the  currents; the simulations are then compared to the  acquisitions. The hypothesis which has the highest  correlation to the field measured gives the precise location of  the current. To maximize the localization accuracy of the  current, it can be divided into simple straight lines which are  simulated separately using the superposition principle. By  working on each single part of the current it is therefore


possible to maximize the correlation by performing a certain  number of geometrical transformations: translations, rotations  or extension/shortening. We have proven that with the  simulation approach, it is possible to generate a very precise  current map, even when the standard MCI algorithm does not  produce good enough results [11]. This is because the  simulation approach allows us to retain the valuable  information about the data which is lost when performing the  calculations and filtering needed for the MCI algorithm.


We have also shown how the technique resolution can be  increased with this approach, so that it is possible to map  currents flowing up to a few centimeters away from the probe  with a resolution as low as 1µm [12].


Finally, with the simulation approach, we have been able to  add another dimension to the scope of the technique: the DUT  can be fully three-dimensional, and with a combination of  tilted and flat scans it is possible to generate a full 3D  reconstruction of the current path [13].


The Simulation Approach for 3D devices


The use of the MCI technique for three-dimensional System  in Package devices has already been documented[14]. However, in that particular case studied all the currents were  flowing on the external part of the package. Therefore it was  possible to perform the measurements at a short distance from  the currents. In this paper we propose a case where the simple  application of the MCI algorithm was not able to give the  desired results. This was because some of the currents were  flowing as far as one centimeter away from the package’s  external surface. Consequently the MCI technique was not  able to generate a full currents map.


In such cases it is possible to find the current leak by using  the simulation approach. We were therefore able to  reconstruct the current path with enough precision to isolate  the defect. To measure the precise value of the working  distance, we applied a fitting algorithm using knowledge of  the shape of the magnetic acquisition curve. This new  methodology helped us to find those parameters which  previously could not be found with sufficient accuracy.


A 3D Case Study


The failed component we studied was a memory stack from  3D-Plus. A certain percentage of the manufactured  components all presented the same type of defect: abnormal  behavior observed during electrical tests. For our analyses we  only had access to one failed device.


Sample Background


Figure 4 shows optical images of the DUT. It is an eight layer  flash memory stack. Each layer is composed of a strap board  which connects the two sides of the component which have  the vertical connections, and a flexible PCB connected via  bond wires to the memory chips.


Figure 4: Optical views of the DUT: the top of the component (top left), the bottom (top right), one of the plain sides (middle) and the two sides with the vertical connections  between different layers (bottom). The coordinates indicate  orientation of the device.


During the electrical characterization of the module  performed with ATE (Automatic Test Equipment), an  abnormal current value was detected on the Write Enable pin  of the 8th level (WE7). The test showed a current of 65mA on  this pin, which was only limited by the compliance of the  equipment. However, despite this faulty behaviour, the device  was fully functional.


As only the 8th level of the component presented an anomaly, comparative tests between the 7th (the reference device) and  8th (the faulty device) levels were performed. We then verified  that all the other levels (from the 1st to the 6th) behaved  exactly as the 7th.


The tracks under investigation can be seen in the pin-out in  figure 5. Here we have the complete layout of the external  connections which are used to electrically link the different  layers of the circuit.


Electrical tests


Electrical tests performed on the sample showed a current  leak on the Write Enable pin of the 8th level (WE07). The  electrical signature of the defective pin was acquired and  compared with that of the 7th layer pin (WE6). The module  presented two VCC pins which were not connected internally (VCC and VCC1). We therefore proceeded to the acquisition  of the current/voltage characteristic between the WE pins  and, respectively, the ground (GND), VCC and VCC1. The  results are shown in figure 6. Here we can see that, as


expected, there is no current flowing between the WE06 and  the VCC, VCC1 or GND pins.


Figure 5: Layout of the lateral connections of the sample: all  the layers are connected to the external pins by the lateral  metallic tracks. The tracks under investigation are those  which relate to the WE07 and VCC pins.


Figure 6: Differences in the electrical signatures between  WE06 and WE07 pins versus GND, VCC1 and VCC. WE06 vs  GND, WE06 vs VCC1 and WE06 vs VCC produced the same  results and are therefore all represented by the same line on  the graph.


The two curves relating to WE07 versus GND and VCC1 are  very similar. In both cases, a small amount of current (approximately 5µA) starts to flow if we apply a high enough  bias. Finally, we can see that there is a very high current leak  flowing between the WE7 and VCC pins. The compliance we  used for this measurement was 50µA, and it saturated before  we could reach the 3V measurement limit. The current  flowing between the WE7 and VCC pins is a lot higher than  the current on the reference device. This signature does not  show a direct short circuit, but a current leakage at some  point in the device. The fact that the signature of the failure  showed on the WE07 pin, could easily have led to the  conclusion that the defect was on the top layer of the sample. We later proved, by using magnetic techniques, that the  defect was in fact very deep inside the device and not on this  layer.


Optical and X-Ray inspection


Figure 7: X-Ray acquisitions of the sample: top view (left)and  side view (right) .


The external optical inspection of the sample showed no sign  of defects. We therefore proceeded to the X-Ray inspection of  the sample.


In figure 7 the X-Ray acquisitions of the sample are shown. Due to the complex nature of the assembly, it is not possible  to see any defects in these images. In the side view we can see  how complex the assembly of the device is: we have eight  separated layers composed of a lead frame, a strap board and  the die. By acquiring an X-Ray image from above the DUT it  is therefore not possible to focus on a particular layer or to  obtain sufficient information about the internal layout.


At this point in the analysis, we still thought that the defect  was most probably situated on the 8th layer. We tried to focus  the X-Ray image on this layer with no results.


Magnetic Microscopy analysis


Electrical setup


The best way to localize a defect without risk of destroying it  is to use a non-invasive contactless technique, such as  Magnetic Microscopy. We therefore proceeded to put in place  an electrical setup which permitted the use of this technique. To avoid applying too high a voltage on the pins, the  maximum current allowed on the WE07 pin was around  100µA. In order to get the best signal to noise ratio, magnetic


Tracks under investigation


acquisitions are usually performed through an AC bias. The  acquisitions are then filtered through a lock-in amplifier  working at the same frequency of the injected AC current. This makes it possible to filter out all the background  magnetic noise, which is mostly due to the DC fields  generated by ferromagnetic materials and the 50Hz field  generated by the system currents.


We therefore set the DC bias to 2.5V to activate the defect  and then added a 1Vpp AC voltage. The resulting current Ipp  was approximately 100µA. For currents of this amplitude, the  MCI technique is the best solution for working distances of  up to a few hundred micrometers, which was the distance we  had estimated from the top of the package to the 8th layer.


Magnetic analysis


Figure 8: Magnetic acquisition (left) and overlay of the  results of the MCI calculations with the optical acquisition (right).


A first scan showed no signal at all above the DUT. This was  the first sign that the overcurrent was not flowing in the 8th layer. The lack of signal was also due to the package  metallization, as part of this metal layer can become partially  magnetized and prevent the magnetic acquisition from giving  meaningful results in terms of MCI analysis.


We therefore tried to acquire the magnetic signal from  backside, which was not covered in metal. The result was a  very noisy acquisition, but one which still provided some  information that we could analyze. We therefore performed  an MCI calculation to get an initial idea of the current  distribution. The results can be seen in figure 8. We can see  that the output current map is not very precise. To localize the  current on the x-y axes with greater precision we performed a  magnetic simulation of a current line. We started from the  hypothesis that there was a current line on one of the layers. We then generated a set of simulations by varying the current  direction and position. The results are shown in figure 9. The  thin blue line represents the position of the simulated line  which had the highest correlation to the measurement. We


then superposed this result to an X-Ray image in order to  obtain information about the current’s position in the circuit  layout.


Figure 9: Superposition of the MCI results, the current  localization by simulation and the X-Ray image.


As this step was not conclusive, we decided to perform  magnetic acquisitions followed by MCI analyses on the sides  of the sample, where there are all the connections between the  pins of the device and the different layers of the stack. The  MCI results are shown in figure 10.


Figure 10: MCI results for the sides of the sample.


These results showed that the current was not flowing on the  top layer, but that it was buried deep inside the package. Surprisingly, the vertical currents stopped at the 5th level on  both sides. This is the reason why the acquisition taken above  the sample did not give any results: the current was flowing  too far from the surface.


Thanks to this last step, we were finally able to verify that the  defect was on the 5th layer. To obtain more detailed results it  was necessary to decrease the working distance. We therefore  proceeded to perform physical deprocessing of the package by  cutting the device just above the fifth layer. The results of the  cross section are shown in figure 11. We then repeated the  electrical tests performed earlier to be sure that we had not  destroyed the defect.


After this step, the bi-dimensional layout of the current was  obtained by performing a magnetic scan followed by an MCI  analysis. The resulting current layout is shown in figure 12. In this image we can clearly see that there is a current


flowing in the middle of the sample. However, we still do not


6e-003


know on which exact z plane the current is flowing. Therefore a further magnetic simulation was performed.


40-009-


26-002


0*+000-


(T) Field Magnetic


2-006


-46-009


Figure 11: Side view (left) and top view (right) of the


D300100015002000250030003500-6e-003-


deprocessed sample.


Distance on the y axis


Figure 12: MCI results on the top side


To evaluate the z plane on which the current was flowing  with precision, we generated a magnetic curve fitting. This


Vcc1


methodology was used in [15] to extract very useful  parameters such as the z distance and the current amplitude.


WE07


The results of our analysis are shown in figure 13. The red  curve is the acquisition of the magnetic field on the y axis, while the blue curve is our fitting. The two curves are very  similar, showing that the output parameters of the fitting are  extremely precise.


Figure 13: Fitting of the magnetic field.


The fitting gave a z distance of 834µm from the probe. As the  package was now already partially deprocessed, we were able


SBlsD


to acquire an X-Ray image of only the 5th layer. By  superposition of this image to the simulation it was then  possible to precisely localize the exact z plane inside the layer  on which the current was flowing.


Now that we had found the vertical localization of the  current, we were able to superpose the X-Ray acquisition of  that layer to the current layout, as shown in figure 14. This  figure shows the exact track where the current was flowing.


1003


Figure 14: Superposition of the MCI results to the X-Ray  acquisition of the 5th layer


Defect Localization


On the fifth level of the sample, the WE7 pin should not be  connected to the flex board. However, we can clearly see in  figure 14 that there is an electrical connection on that pin. In  order to validate the results, we did a comparison study


between the 8th and 5th levels of the sample.


Figure 15: Electrical contacts on the 8th layer


In figure 15 the electrical contacts of the 8th layer are shown  and enlarged. The two tracks which are highlighted in the  image are clearly open, so there is no contact with the  external tracks which connect the vertical layers to the pins of  the component. These two lines need to be left open and not  connected to the external vertical tracks; as the dies are  reported on these lines through bond wires, the tracks were  cut at this level. This same cut was performed on all the other  layers in order to leave these pins unconnected for all the  dies.


In figure 16, the X-ray images of the 5th layer are shown. Here we can see that one of the two pins still makes a short  circuit with the external connections.


Figure 16: Electrical contacts on the 5th layer


This defect was due to a misalignment of the layers. While  the 8th layer board had been correctly placed, the 5th layer  board had been slightly shifted to the right. An enlarged view  of the left-hand side of the two layers is shown in figure 17.


Figure 17: Connections on the 8th layer (left) and on the 5th layer (right).


Here we can see that on the 5th layer there is still a part of the  external lead frame due to a misalignment of the component  during production.  Not all the layers of the component had  been placed and cut in the same way. On the left-hand side  parts of the lead frame which should have been cut out were  still present,  as the 5th layer was shifted to the right. This is  shown in figure 17. Meanwhile, on the right-hand side of the  layer the cut was performed further over to the left than it  should have been. Therefore parts of the lead frame which  should not have been removed were cut out. In this case, the  track which should have been left open was short-circuited to  the external vertical lines.


MCI techniques are able to map currents which flow close to  the probe. When this is the case, as we have seen in [14], it is  possible to reconstruct a 3D current path from the magnetic  acquisitions. However, if the currents flow deep inside the  sample, it is not possible to generate any results with MCI. In  this paper we have shown a case like this, where the only way  to generate a map of the currents was to use other  methodologies like magnetic simulations. We were then able  to precisely reconstruct the current path inside the sample. In  addition, a methodology for the evaluation of z was used, so  that it was possible to precisely evaluate the z plane of the  layer in which the currents were flowing. It consisted in  fitting the measured data to a pre-calculation of the  theoretical magnetic field in order to extract the desired  parameters (in our case the z distance).


The analysis performed on the case study shows how  magnetic microscopy can be a very powerful tool for defect  localization even for large three-dimensional structures. The  initial electrical tests, in this case, could have brought us to  the false conclusion that the defect was on the 8th level of the  sample; in reality, these results occurred because the track  connecting the WE of that layer was mistakenly connected to  the 5th layer too. That is why the component was still  functional, even though the current leak on that pin was so  high that the component was not fit for use.


No contact with  the external tracks


Contact with the  external tracks


No contact with


the external tracks


No external lead  frame visible


Part of the lead  frame still present


Thanks to the magnetic technique, we were therefore able to  first identify the correct layer of the defect, and then pinpoint  the exact short circuit which created the defect.


We would like to thank Antonio Orozco and Jan Gaudestad  from Neocera for their invaluable help and for sharing their  knowledge about Magnetic Microscopy. We would also like to  thank Nicolas Fiant and Christian Val from 3D-Plus for all  their support and guidance regarding the case study.


[1] Zhang GQ, Graef M, van Roosmalen F. The rationale and  Paradigm of ”More than Moore”. Proceedings of 56th  ETCT, IEEE, 2006; p. 151-157.


[2] Goldstein H. Packages go Vertical. IEEE Spectrum, August 2001; p. 46-51


[3] Roth BJ, Sepulveda NG, Wikswo Jr JP. Using a  magnetometer to image a two-dimensional current  distribution. Journal of Applied Physics 65, 1 January  1989; p. 361-372.


[4] Wikswo Jr JP. The magnetic inverse problem for NDE. In  Weinstock H, editor. SQUID Sensors: Fundamentals, Fabrication and Applications, Kluwer Academic  Publishers; 1996, p.629-695.


[5] Knauss LA, Cawthorne AB, Lettsome N, Kelly S, Chatrephorn S, Fleet EF, et al. Scanning SQUID  Microscopy for Current Imaging. Microelectronics  Reliability no. 41, February 2001; p.1211-1229.


[6] Knauss LA, Frazier BM, Christen HM, Silliman SD, Harshavardhan KS, Fleet EF, et al. Detecting power  shorts from front and backside of IC packages using  scanning SQUID microscopy. Proceedings of 25th ISTFA, 1999; p.11-6.


[7] Crepel O, Poirier P, Descamps P, Desplats R, Perdu P, Haller G, Firiti A. Magnetic Microscopy for ICs Failure  Analysis: Comparative Case Studies using SQUID, GMR  and MTJ Systems. Proceedings of 11th IPFA, 2004; p.45-8.


[8] Knauss LA, Orozco A,Woods SI, ZhiyongWang. Advances  in Magnetic-Based Current Imaging for High Resistance  Defects and Sub-Micron Resolution. Proceedings of 11th IPFA, 2004; p. 267-270.


[9] Hsiung S, Tan KV, Komrowski AJ, Sullivan DJD, Gaudestad J, Orozco A, et al. Failure Analysis on  Resistive Opens with Scanning SQUID Microscopy. 42nd  Annual international Reliability Physics Symposium,IEEE, 2004; p. 611-2.


[10] Chatraphorn S, Fleet EF, Wellstood FC, Knauss LA. Noise and Spatial Resolution in SQUID Microscopy. IEEE Transactions on Applied Superconductivity, March  2001; vol. 11, No. 1, p. 234-7.


[11] Infante F, Perdu P, Petemont S, Lewis D. A new  Methodology for Short Circuit Localization on Integrated  Circuits using Magnetic Microscopy Technique coupled  with Simulations. Proceedings of 16th IPFA, 2009; p.208-212.


[12] Infante F, Gabarrot M, Perdu P, Lewis D. Ultimate  Resolution for Current Localization by means of Magnetic  techniques. Proceedings of 35th ISTFA, 2009; p.314-318.


[13] Infante F, Perdu P, Lewis D. Magnetic microscopy for 3D  devices: Defect localization with high resolution and long  working distance on complex system in package. Proceedings of 20th ESREF, 2009; p. 1169-1174.


[14] Felt F, Knauss LA, Gilbertson A, Orozco A. Construction  of a 3-D Current Path using Magnetic Current Imaging. Proceedings of 33th ISTFA, 2007; vol.33, p. 197-205.


[15] Schrag BD, Liu X, Hoftun SH, Klinger PL, Levin TM, Vallett D. Quantitative Analysis and Depth Measurement  via Magnetic Field Imaging. EDFA Magazine, November  2005; vol.7, issue 4, p. 24-31.


# Advanced Sample Preparation Method for Lead Free Bump IMC and Solder Grain Image Enhancement


Advanced Sample Preparation Method for Lead Free Bump IMC and Solder Grain  Image Enhancement


Ming-Song Sheu, Yian-Liang Kuo, Jeng-Hun Lee, Yu-Ting Lin, Hui-Chen Chu, Tsung-Fu Tsai, and Chih-Horng Chang.  Failure Analysis Division, Taiwan Semiconductor Manufacturing Company, Ltd., Hsin-Chu, Taiwan


mssheu@tsmc.com


An advanced method for LF (Lead Free) bump sample  preparation to improve the surface of sample that can enhance  the image of IMC (Inter Metallic Compound), solder grain  boundary and micro-crack after TC (thermal cycle) reliability  test is proposed. By this advanced method application, LF  bump micro-crack location and propagation path can be  observed easily for the reliability test fracture failure  mechanism study and LF bump crack improvement further.


For the purpose of saving our environment and adhering to the  RoHS (Restriction of Hazardous Substances) guidelines, LF (Lead Free) solder bump material is now frequently used in the  semiconductor industry. Due to the brittle material  characteristic of SnAg LF bump, cracking on SnAg LF bumps  occurred easily during the TC (Thermal Cycle) test. [1] Different LF bump crack behaviors, such as bump crack  location and propagated path or direction, may indicate  different fracture modes [2,3,4]. However, the micro-crack and  its propagation path are usually difficult to observe by the  standard sample preparation method. Therefore, a new method  for sample preparation is required and essential. In this paper, a low angle ion-milling based technique is proposed to  advance the LF bump sample preparation method - providing  an excellent and clear image of micro-cracks as well as the  grain boundary of LF bumps for the reliability test fracture  failure study


Ion milling surface treatment


For the former cross-section sample preparation method, the  sample was polished directly without any additional surface  treatment. Hence, the LF bump surface was almost flat and the  grain boundary could not be observed easily. The surface  treatment in this advanced sample preparation method utilized  the BAL-TEC RES101 (Rapid Etching System), a low angle  ion milling instrument. A clear LF bump grain boundary image  can be observed by applying this instrument.  Fig. 1 shows the  LF bump cross-section-polished SEM (Scanning Electron  Microscope) images. The same bump images without the  surface treatment process and with the surface treatment


process are shown in Fig. 1a and Fig. 1b, respectively.  The  Fig. 1b reveals a better bump surface profile and grain  boundary image than does Fig. 1a. This result indicates the  surface profile of bumps could be improved by using this  surface treatment method.


Figure  1a: SEM of a LF bump without surface treatment.


Figure 1b: The same bump as Fig. 1a following the  application of ion milling surface treatment.


Cu


Ni


LF solder


For example, the trans-granular crack and inter-granular crack  denoted different fracture mechanisms. Therefore, the  observation of bump cracking behavior is important and  helpful to understand the bump crack failure mechanism. Fig. 2 demonstrates crack propagation of a LF bump sample that  underwent the ion milling surface treatment method. Fig. 2a  shows the image of the full crack of a LF bump; the cracking  path of that bump was mostly propagated along the grain  boundary. A partial crack of the bump was shown in Fig. 2b, and the short column grain stopped the crack.


Figure 2a: Example of the full crack propagation path of a LF  bump.


Figure 2b: Example of the partial crack propagation path of a  LF bump


The grain size of LF bump would also influence crack  behavior. Fig.3 show the images of LF bumps, which samples  had subjected to the low angle ion milling surface treatment, and the various grain sizes of that bump can be seen. The  crack was propagated easily in the small grain bump, as shown  in Fig 3a. In the contrast, as shown in Fig 3b, the large size  grains reveal a good cracking resistance. The advance of the


low angle ion milling method can be interpreted by above  observations.


Figure 3a: SEM of LF bump with low angle ion milling  surface treatment. The bump with smaller size grain tended to  crack easily.


Figure 3b: SEM of a LF bump had subjected to the low angle  ion milling surface treatment. The grain size of that bump was  larger than the bump in Fig. 3a, and was not as easy to crack.


Bump cracks propagated mostly  along the grain boundary


Cracking was stopped by the short column grain.


Bump crack


Comparison of surface treatment methods


Several surface profile enhancement methods for LF bumps  were also performed in this study, and the results are  demonstrated in Table-1.


Table 1. Summary of various surface treatment methods for  LF bumps.


|Method |No treatment (original) |Chemical (HCl + CH3OH) |Physical |Physical |Physical ||
|---|---|---|---|---|---|---|

|Method |No treatment (original) |Chemical (HCl + CH3OH) |PECS |FIB |Ion milling ||

|Cu/Ni interface |not clear |more clear |very clear |very |very clear ||

|Cu/Ni interface |not clear |more clear |very clear |clear |very clear ||

|IMC |not clear |more clear |more clear |very clear |very clear ||

|Solder grain |X |not clear |X |not clear |very clear ||

|Bump u-crack |not clear |not clear |clear |clear |very clear ||

X : Solder grain cannot be observed.


The argon gas plasma is a favorite working media for surface  treatment. The key factor in surface treatment result is the  angle between the sample surface and the plasma injection  nozzle. Due to different etching rates between different  materials, the high angle nozzle method can create a good  interface image between two different materials. Therefore, the  image of the Sn matrix and IMC can be recognized by the high  angle nozzle method. Unfortunately, for the high nozzle angle  method, it is difficult to enhance the grain boundary of the  solder bump (the material is the same). Low angle nozzle (near  horizontal) surface treatment, however, can provide a good  image between two different materials as well as grain  boundary. The SEM images of the LF bump micro-crack are  shown in Fig. 4.  Fig. 4a demonstrates the bump without  surface treatment, and the micro-crack of bump cannot observe  clearly. Afterward, the same bump was subjected to surface  treatment by the PECS (Precision Etching Coating System, Gatan Model 682), and the result was shown in Fig. 4b. The  image of the bump was improved and the micro-crack of the  bump was visually discernible. However, grain boundary of  the solder bump cannot be observed because the argon plasma  nozzle of PECS is vertical to the sample surface. Thus, it  cannot be judged whether or not cracking is propagating along  the solder grain boundary


The low angle nozzle of the ion milling surface treatment  method can significantly improve such shortage by combining  the advance physical etch (more horizontal direction and less  vertical bombardment) and the thermal etch surface treatment. Fig. 5 shows the SEM images of the LF bump micro-crack  inspection. Fig. 5a reveals the bump without surface treatment, and the micro-crack of the bump was not clear. Afterward, the  same bump was subjected to the low angle nozzle of the ionmilling surface treatment, and the result is shown in Fig. 5b.


The bump image of micro-crack and grain boundary was  improved and visually discernible. Hence, the micro-crack of  the bump mostly propagating along the grain boundary can be  observed.


Figure 4a: SEM of a LF bump without surface treatment. The  bump micro-crack is not clear.


Figure 4b: The same bump as in Fig. 4a following application  of PECS surface treatment. The micro-crack in the bump can  be found after performing the PECS, however, the solder  grain boundary could not be observed. Hence, the crack of  bump could not be judged whether or not cracking is  propagating along the solder grain boundary.


Micro-crack


Figure 5a: SEM image of a LF bump without surface  treatment. The micro-crack image of bump is not clear.


Figure 5b: The same bump, as shown in Fig. 5a, following  application of ion milling surface treatment. The micro-crack  image of bump can be found after performing ion milling, and  the solder grain boundary can be also observed clearly. The  micro-crack of bump propagated mostly along the solder  grain boundary can be seen.


Ion milling demonstrated a good surface treatment capability; however, the operation parameters strongly affect the quality  of the treatment surface. If using the improper parameters (improper plasma nozzle angle, bias voltage, current, sample  position etc.) is difficult to get an excellent surface treatment  effect. [5] Table-2 lists the key parameters for low angle ion  milling surface treatment


Table 2. Key parameters of low angle ion milling surface  treatment.


Gun current:                    3 mA


Acceleration voltage:      6 kV


Angle of incidence:         2.5o


Rotation speed:                3 rpm


Milling time:                   40 min.


The FIB (Focused Ion Beam) is another helpful instrument for  sample preparation and surface treatment. It can create an  excellent surface for morphology observation by SEM or TEM (Transmission Electron Microscope). However, the FIB is  only suitable for a small observation area, such as  100um*100um. In contrast, the low angle nozzle ion milling  method/instrument can easily create a large observation area, such as 20,000um*20,000um. Furthermore, the cost of the FIB  instrument is much higher than that of the ion-milling  instrument.


The ion milling with a low angle nozzle function is proposed  to be an ideal method of surface treatment for LF bumps  cracking failure mechanism study. The micro-cracks of LF  bumps and its crack behaviors, such as cracking location and  propagation path, can be observed easily by this advanced  surface treatment method.  .


The authors would like to appreciate all their colleagues of  package assembly failure analysis (PAFA) in Taiwan  semiconductor manufacturing company (TSMC) for their great  help and support in this work.


[1] H.Y. Lu, H. Balkan, J. Vrtis, and K.Y. Simon Ng,


“Impact of Cu Content on the Sn-Ag-Cu  interconnects”, Electronic Components and  Technology Conference, 2005, pp.113-119.


[2] S.K. Kang, P. Lauro, D.-Y. Shih, D.W. Henderson, T. Gosselin, J. Partelo, S.R. Cain, C. Goldsmith, K,J, Puttlitz, and T.K. Hwang, “Evaluation of Thermal  Fatigue Life and Failure Mechanisms of Sn-Ag-Cu  Solder Joints with Reduced Ag Contents”, Electronic  Components and Technology Conference, 2004, pp.661-667.


[3] J.-W. Jang, A.P.D. Silva, J.-K. Lin, and D.R. Frear,


“Tensile fracture behaviors of solid-state-annealed  eutectic SnPb and lead-free solder flip chip bumps”, Materials Research Society, Vol.19, No.6 (2004), pp.1826-1834.


[4] B. Arfaei, Y. Xing, J. Woods, J. Wolcott, P. Tumne, P. Borgesen, and E. Cotts, “The Effect of Sn Grain  Number and Orientation on the Shear Fatigue Life of  SnAgCu Solder Joints”, Electronic Components and  Technology Conference, 2008, p.459-465.


[5] W. Mack, B. Seidl, R. Fischer, T. Ort, J. Walter, J. Grijnewald, L. Berthold, and M. Petzold, “Ion Beam  Polishing for Embedded Cross-Sections and its  Advantages for FESEM Analysis in Electronic  Packaing”, the 30th International Symposium for  Testing and Failure Analysis, 2004, p.338-345.


# Extending Acoustic Microscopy for Comprehensive Failure Analysis Applications


Extending Acoustic Microscopy for Comprehensive Failure Analysis  Applications


Sebastian Brand, Matthias Petzold


Fraunhofer Institute for Mechanics of Materials, Halle, Germany   Sebastian.Brand@iwmh.fraunhofer.de


Peter Czurratis, Peter Hoffrogge


PVA TePla Analytical Systems GmbH, Aalen, Germany


In industrial manufacturing of microelectronic components, non-destructive failure analysis methods are required for either  quality control or for providing a rapid fault isolation and  defect localization prior to detailed investigations requiring  target preparation. Scanning acoustic microscopy (SAM) is a  powerful tool enabling the inspection of internal structures in  optically opaque materials non-destructively. In addition, depth specific information can be employed for two- and  three-dimensional internal imaging without the need of time  consuming tomographic scan procedures. The resolution  achievable by acoustic microscopy is depending on parameters  of both the test equipment and the sample under investigation. However, if applying acoustic microscopy for pure intensity  imaging most of its potential remains unused.


The aim of the current work was the development of a  comprehensive analysis toolbox for extending the application  of SAM by employing its full potential. Thus, typical case  examples representing different fields of application were  considered ranging from high density interconnect flip-chip  devices over wafer-bonded components to solder tape  connectors of a photovoltaic (PV) solar panel. The progress  achieved during this work can be split into three categories: Signal Analysis and Parametric Imaging (SA-PI), Signal  Analysis and Defect Evaluation (SA-DE) and Image  Processing and Resolution Enhancement (IP-RE). Data  acquisition was performed using a commercially available  scanning acoustic microscope equipped with several ultrasonic  transducers covering the frequency range from 15 MHz to 175  MHz. The acoustic data recorded were subjected to  sophisticated algorithms operating in time-, frequency- and  spatial domain for performing signal- and image analysis. In  all three of the presented applications acoustic microscopy  combined with signal- and image processing algorithms  proved to be a powerful tool for non-destructive inspection.


Inspection methods operating non-destructively are required in  many applications in the field of failure analysis including


quality control and fault localization prior to destructive target  preparation for detailed micro-structural investigations. Providing the option of running multiple tests on the same  sample methods operating non-destructively also extend the  level of investigation and thus, the understanding of defect  formation, failures and their root causes. However, nondestructivity is always connected with a trade-off between  comprehensive destructive preparations and resolution. Scanning acoustic microscopy employing ultrasonic signals  ranging from the MHz- to the GHz-range allow resolutions  from the mm- down to the μm range. The final resolution  achievable however, is depending on various parameters  namely the acoustic frequency, the transducers aperture but  also the sound velocity of the material and the depth of the  structure under investigation. While the aperture of the  inspection transducer can be tailored for specific applications  wave attenuation is inevitably proportional to frequency and  the materials acoustic attenuation [1]. In acoustics, attenuation  covers several phenomena which contribute to a decrease of  the amplitude of the acoustic wave and its spectral content. Major attenuation effects are caused by absorption and  scattering, but also structural and chemical relaxation  processes lead to a decreased acoustic intensity. For increasing  the penetration depth, the acoustic frequency has to be lowered  which is, however, related to a decreased lateral resolution. The interaction of acoustic waves with matter is characterized  by phenomena like reflection, diffraction and scattering caused  by structural, size and mechanical properties of the sample and  its sub-structure. Therefore, echo signals received from a  sample contain characteristic information on the samples  properties. By employing appropriate signal analysis  algorithms to time domain echo signals acquired by the  acoustic microscope, parameters related to structural and  mechanical properties of the inspected sample can be derived. Thus, by analyzing the echo signals comprehensive  information on the samples condition and composition can be  obtained. In situations were acoustic microscopy is applied for  pure qualitative imaging of internal structures, like  delaminated spots in a bonding interface, additional image  processing and analysis can improve resolution and contrast  for revealing and emphasizing various of defects.


The current work is focused on the development of a  comprehensive analysis tool for extending acoustic  microscopy by signal and image processing algorithms, enabling a broad range of applications in the field of failure


analysis. In this paper three case studies representing different


fields of application are described targeting developments in


parametric imaging, defect evaluation and image processing.


Signal analysis and parametric imaging is applied for


estimating the adhesive condition of a solder tape of a PVsolar panel. The flip-chip contacts of a CPU-device were


evaluated and classified employing extended signal analysis.


Finally, delaminated regions in wafer-bonded interfaces were


inspected and images were processed for increasing the


resolution and the contrast. In all three applications the results


were improved providing additional information on the defect


situation.


Materials and Methods


Data Acquisition


Acoustic data acquisition was performed using a fast scanning  acoustic microscope (Evolution II, PVA Tepla Analytical  Systems GmbH, Aalen, Germany) equipped with several  transducers covering a frequency range from 15 MHz up to  175 MHz. The focal length of the transducers also differed  from 5.9 mm @ 175 MHz up to 20 mm @ 15 MHz. Echo  signals were digitized with a sampling rate of 500 MS/s at a  resolution of 8 bit. The unprocessed digital rf-signals were  stored on the microscopes internal hard drive for further offline analysis. During scanning, the samples were submerged in  distilled and degassed water which acted as the coupling  medium for the acoustic wave propagation. Data analysis and  image reconstruction was performed using the MATLAB  acoustic analysis software SAMNALYSIS, developed at the  Fraunhofer Institute for Mechanics of Materials, Halle, Germany.


Signal Processing


Signal processing was developed using MATLAB (The


Mathworks, Natick, USA). The algorithms developed during


this work were combined into the SAMNALYSIS toolbox that IUNIcan be applied for performing comprehensive and complex  analyses on acoustic data and images. The entire software was


bus bar


solder


solder tape


compiled using the MATLAB compiler and thus, can be run  on any Microsoft Windows based computer for off-line  analysis of the recorded rf-ultrasonic signals.


Signal Analysis and Parametric Imaging (SA-PI)


The samples employed for illustrating the application of  parametric imaging combined with signal analysis were


delaminated spot


/ polycrystalline Silicon


photovoltaic (PV) solar cells as shown in figure 1. The  samples consisted of polycrystalline silicon wafers with a  thickness of 220 μm. For electrical connectivity, a tinned  copper interconnect ribbon of 100 μm thickness and 5 mm  width was soldered on top of the solar cell’s bus bar. The  solder had a thickness of approx. 30 μm on each side of the  tape. The acoustic inspection was performed as described  above. For optimizing the acoustic images using appropriate  processing and analysis algorithms, the echo signals were


subjected to a cepstral analysis [2]. Parametric imaging allows  the visualization of parameter changes caused by specific  defects related to characteristic sample properties. The  example shown here employs the transformation of the time  domain signals into the cepstral domain. In the cepstraldomain, features representing the periodicity of the spectra can  be derived which are related to the temporal and thus, the  spatial separation between echo pulses in the time domain  signal. By employing the appropriate sound velocity, the  physical separation between interfaces can be estimated. The  main advantage of using the cepstral domain is the ability to  estimate the pulse separation even when pulses overlap. In  locations where the solder tape is delaminated from the bus bar  of the PV-panel, a strong reflectivity occurs at the interface  tape-coupling fluid, resulting not only in a strong echo at this  interface but also in the occurrence of multiple reflections  which can be observed as a reverberation in the received  acoustic signal. When inspecting a well soldered region, the  acoustic signal obtained is expected to contain echo pulses at  the tape/bus bar interface with a weaker amplitude that is  caused by the lower reflectivity and the higher transmission  coefficient of the soldered interface. The signal obtained here  is also expected to lack a strong reverberation, resulting in a  low number of reoccurring echo pulses.


From the cepstra computed using the time domain signals, the  position index of the first maximum was extracted. The  parametric imaging was then performed by color coding of the  parameter values and mapping as a two dimensional image.


It should be noted that parametric imaging can be performed  using any relevant parameter of the underlying acoustic signal  representing a signal property related to the defect of interest.


wafer


Figure 1: Sample description for signal analysis and  parametric imaging. Illustration of a PV-solar cell with bus  bar and soldeed Cu ribbon for electrically connecting the bus  bar to the external electronics. The cell had a thickness of 220 μm, while the Cu riboon thickness was 1 mm. Approx. 30 μm  of solder was contained on top and beneath the ribbon. The  ribbon width was 5 mm.


For verifying the findings obtained by acoustic microscopy  and subsequent signal analysis complementary x-ray  inspection was performed using a nanomex 180nf CT (Phoenix  x-ray, Wunstorf, Germany).


Signal Analysis and Defect Evaluation (SA-DE)


CPU devices manufactured in flip-chip technology were  investigated for evaluating and classifying the condition of the  solder bump contacts using acoustic microscopy. The samples  used are illustrated in figure 2. The flip-chip contacts  connected the 750 μm thick silicon die with the organic  laminate substrate of the CPU device. The solder bumps had a  lateral diameter of 80 μm and the die size was 20 mm by 30  mm. To support the reliability behavior, a polymeric under fill  was contained.


Signal Analysis and Defect Classification:


The lateral locations of the flip-chip contacts were estimated  by differentiating between the interfaces silicon/solder-contact  and silicon/underfill using characteristic reflective features of  the interfaces as illustrated in figure 3. Figure 3-right shows  the Hilbert transformed acoustic cross section of a CPUsample. Echoes occurring at the silicon/solder-contact  interface were considerably longer than echoes from the  silicon/underfill interface. Parameter values of the backscatter  amplitude integral (BAI) were computed within the time range  between the exit echo of the silicon and the signal peak at the  solder/substrate interface as indicated by the red rectangle in  figure 3. Further analysis was applied to signals of the solder  interconnections exclusively for characterization of the contact  condition. These processing steps included wavelet analysis  employing a Gaussian mother wavelet of the 4th order for  deriving wavelet coefficients versus scaling factors and time. Wavelet analysis is a 2-D redundant signal transformation  which overcomes the main weaknesses of the short-timeFourier-transformation (STFT). The application of a static  window length as used in STFT results in a constant time and  frequency resolution of the transformed signal. In wavelet  analysis, the analyzing wavelet is expanded and compressed in  addition to sliding over the signal analyzed. This adaptation  results in an improved temporal and spectral resolution, which  cannot be obtained by a Fourier transformation [5]. During  scaling of the analyzing wavelet, the number of oscillations of  the wavelet remains constant, resulting in a variation of the  spectral content. Wavelet analysis of a signal computes  coefficients at different scaling factors describing the  correspondence between the analyzing wavelet and the signal. For illustration, a wavelet coefficient corresponds to the area  below the result of the multiplication of the analysis wavelet  and the signal at a particular wavelet scaling. Although the  STFT provides a complex coefficient for one parameter (frequency), the continuous wavelet transform (CWT) computes one coefficient for each combination of the scaling  factor and the temporal position. The wavelet transformation  performed in the current study used the MATLAB functions  for the CWT. A Gaussian wavelet of the fourth order was  chosen because of its similarity to the ultrasonic pulses used in


Figure 2: Sample description for signal analysis and defect  evaluation. The sample was a CPU device manufactured in  flip-chip technology on top of an organic substrate. The dies  thickness was 750 μm, with flip-chip contacts of height 100 μm and diameter 80 μm. The lateral dimension of the die was  20 mm by 30 mm. Acoustic inspection was performed through  the die after the cap of the CPU was removed.


the experiments. Wavelet analysis was applied to the signals  obtained at positions which were detected to be a


flip-chip contact. The distribution (mean and standard  deviation) of the wavelet coefficients were computed versus  scaling factors and as a function of the temporal position.


In addition to wavelet coefficients, the backscatter  amplitude integral (BAI), the relative peak positions, the peak  amplitudes and the corresponding pulse widths at the siliconsolder interface were computed. For estimating the pulse  width, the peak position and the peak amplitudes time signals  were first transformed into the Hilbert domain and the pulse  width was obtained in ns at -6 dB of the peak amplitude. The  BAI can be computed according to [3] as the integral of the  Hilbert transformed absolute values of the time signal prior to  low pass filtering.


Figure 3: Internal sample structure and echo signal  occurrence. The schematic on the left illustrates the 750 μm  silicon layer with the flip-chip contacts underneath. On the  right, an acoustic cross-section image through the CPUdevice is shown. Boundaries and corresponding echoes are  indicated by red lines. The red rectangle shows the time range  for estimating BAI values.


flip-chip contacts


silicon


flip-chip


Due to integrating over time, multiple echoes can be included  in the BAI computation resulting in an improved contrast. Finally, the parameters of the peak position, the BAI and the  wavelet distribution were scaled, thresholded and combined in  a classifier for deriving a binary void-intact decision for each  individual flip-chip contact. To provide an easy-to-handle  visual indication the resulting decision matrix was color coded  and superimposed to the BAI-parametric image.


Si-wafer (500 μm


The signal- and image analysis toolbox developed for  improving the performance of acoustic analysis showed  positive results. It was possible to extend the application of  acoustic microscopy from pure qualitative imaging to  parametric imaging and thus, semi-quantitative parameter  estimation applicable in a broad range of different application  fields. Additionally, an automated operating method for defect  evaluation of interconnects was developed, based on acoustic  microscopy data. Finally, the combination of acoustic imaging  with image analysis and processing also proved successful for  increasing image detail and contrast. Further image processing  filters will be included stepwise into the analysis toolbox in the  near future, for extending the optimization of the acoustic  micrographs.


91。


[1] Briggs, A, Advances in Acoustic Microscopy, Plenum  Press (New York and London, 1995)


[2] Ziegler, K., “Cepstrum Analysis of Voice disturbances” Folia Phoniatrica et Logopaedica”, Vol. 47, No. 4 (1995), pp. 210-217.


[3] Raum, K., et al., “Channel defect detection in food  packages using integrated backscatter ultrasound  imaging”, IEEE Transactions on Ultrasonics  Ferroelectrics and Frequency Control, Vol. 45, No.1 (1998), pp. 30-40.


[4] Cannon, M., “Blind deconvolution of spatially invariant  image blurs with phase”, IEEE Transactions on Acoustics, Speech and Signal Processing, Vol. 24, No. 1 (1976), pp. 58-63.


[5] Graps, A. “An introduction to Wavelets.”, IEEE  Transactions on Comp Sci Eng, Vol 2, No. 2 (1995), pp. 50-61.


Figure 11: Image analysis applied to acoustic micrographs. Top: pure intensity images obtained by an acoustic


microscope. Bottom: processed acoustic images. Image filters for blind-deconvolution and a Gaussian filter were applied  to emphasize the defect and for increasing the resolution. A Sobel filter was applied in the lower left- and right images for  detecting the contour and orientation of the defects.


# Process induced defects in the silicon substrate: Approaches for successful Failure Analysis.


Process induced defects in the silicon substrate:


Approaches for successful Failure Analysis.


NXP Semiconductors, Nijmegen, The Netherlands   Jan.van.hassel@nxp.com


Failures induced in the silicon substrate by process  marginalities or process mistakes need continuous attention in  new as well as established technologies.


Several case studies showing implant related defects and  dislocations in silicon will be discussed. Depending on the  electrical characteristics of the failure the localization method  has to be chosen. The emphasis of the discussion will be on  the importance of the right choice for further physical deprocessing to reveal the defect.


This paper focuses on the localization method, the deprocessing technique and the use of Wright etch for  subsequent TEM preparation.


The intricate failure analysis process can be categorized in two  parts: electrical fault localization to identify the location of the  abnormalities and physical de-processing to reveal the defect  causing the failure. Naturally both steps involve many  different techniques. In the case of functional circuit failure  related to silicon substrate, the abnormality very often exposes  itself as additional leakage current. The approximate location  of such current can be observed using techniques such as  Photo Emission Microscopy (PEM), Optical Beam Induced  Resistance Change (OBIRCH) and Soft Defect Localization (SDL) [1]. In order to further understand the electrical  behavior of the failing component, it is necessary to use local  probing techniques, such as micro-probing, conductive atomic  force microscopy (CAFM) [2], in-SEM Nano probing [3] or  scanning capacitance microscopy (SCM) [4]. When it comes  to physical de-processing, it is vital that correct methods are  selected to proceed since by nature most procedures are  irreversible.


In this paper, several case studies related to anomalies in  silicon, such as incorrect implant, process and stress induced  crystal defects, will be discussed. The focus of the discussion  will be on the appropriate selection of a de-processing method  for successful analysis. In cases where failure analysis is not  able to show a physical root cause, interpretation of the results  from electrical measurement and experimental evidence from


the processing FAB need to be combined to put forward  possible hypotheses.


The root cause of the example defects in silicon substrate  presented below will only be discussed marginally. More  background information about dislocations; their origin, and  simulation studies can be found in reference [5].


Dopant related failures


Dopant related failures rarely originate from the implant  process itself. In most common cases, the implant process is  blocked due to anomalies in preceding steps of the process. Depending on the technology node and the suspected circuitry (analog or digital) failure analysis can be initiated from front  side or backside of the device.


Figure 1a is a laser scan image taken from the backside of a  failing device. The OBIRCH signal (not shown) coincided  with an abnormal pattern seen at the center of the image.


Figure 1a: Defect revealed by backside laser imaging on a  device where additional current was observed. At the same  location an OBIRCH spot was obtained.


The corresponding TEM cross-section through the anomaly, see figure 1b, shows missing drain implant (manifested as  missing implant damage compared to the source side). A thin  layer of nitride residue can be seen above the drain area. Evidently this remaining nitride layer is the cause of this short  failure. In fact, the abnormal pattern shown in Figure 1a was  the area where nitride residue was present. If the analyst had  selected the HF strip method to reveal the defect, the root  cause would have been removed even though the defect itself  was clearly visible.


(p-well)


Figure 1b: TEM cross-section showing missing implant due to  blocked spacer etching on the left side of poly-gate .


intruding n-area


10 μm


3:24:01 PM 1.30kV 10 000x 5.0mm 4.507FA4393:Dev 10 spot 2


Figure 2: Using SEM passive voltage contrast differently  doped areas can be clearly distinguished. In this case, the  dark contrast along the drain contact was n-type, and this was  missing in the defective area highlighted by the oval.


In general, even though PEM or OBIRCH clearly indicates the  site of interest, failures related to missing or lack of implant  are not always easy to reveal physically especially when the  dopant concentration is somewhat low. Under such  circumstances, several techniques can be used. With SEM  passive voltage contrast method using low acceleration energy (< 1.5 kV) and high incident beam angle different doped areas  can be distinguished as shown in figure 2. Due to surface


contamination during scanning only few scans are possible to  identify the incorrectly doped areas.


Alternatively Scanning Capacitance Microscopy (SCM) can  be used to map the doping area [6,7] with high spatial  resolution. This is illustrated in the next example. In this case, two failing devices (channel length 1 µm) were submitted for  analysis. PEM and OBIRCH highlighted the approximate fail  location and local probing results showed a failing Nmostransistor having a source to drain short under normal gate and  well potential. TEM cross-section was performed on the first  sample, but nothing abnormal was found. The second device  was stripped to silicon level using HF. Multiprobe with SCM  option was used to carry out the 2D dopant mapping over the  failing silicon surface.


Figure 3. : SCM 2D dopant distribution map over


(a) The silicon surface/channel area of the failing Nmos, An  intruding n-dopant area cross the channel (green) is clearly  visible, (b) Cross-section through the area with doping defect  shown in a and (c) Cross-section through the channel of an  adjacent identical Nmos. Comparing images 3b and 3c it was  clear that the defective doping was introduced during  extended N-well formation.


Missing


channel


cross section


implant


Spacer Nitride


N+ source


N+ drain


residue


Source  contact


Drain contact


N+


Drain  contact


N- area


3a


Extended NW


P-well


3b


3c


2/28/2008HVmagWDspot


The dopant map from the silicon surface, see figure 3a, showed that the source to drain short was caused by an  intruding n-doped area across the channel. Once the failure  location was clear, cross-section was prepared through the  intruding n-doped area. This is shown in figure 3b. An  adjacent identical Nmos was used as reference, (figure 3c). By  comparing figures 3b and 3c, it was clear that the defective  implantation occurred during the extended N-well formation  process. The incorrect doping areas with very high and very  low concentrations represent two extreme ends of the problem  scale. In the former case, conventional chemical delineation  method [8] can be used to reveal doping differences whereas  in the following case a combination of various techniques and  expertise is necessary. This is demonstrated in the next case.  Product test at wafer level showed a number of failing dies at  the wafer edge. During electrical fault localization of this  yield problem, an additional leakage current in the order of µA was observed in the digital power domain when the IC  was set in standby mode. On each die several PEM spots were  present randomly distributed in the digital part of the circuitry. The number of PEM spots on a die increased with the leakage  current. Cross sections made through the suspected transistors  did not reveal any possible root cause. In the end, AFM  probing was used to measure the I-V characteristics of the  suspected transistors. This is shown in figure 4 where the  characteristics of several Nmos transistor in the suspected area  were compared. It became clear that there was a Vt spread  over the transistors measured with the largest shift  corresponding to the Nmos transistor showing PEM emission.
  Further investigation identified that the LDD implant  channelled though the columnar poly-silicon gate causing  channel degrading and hence Vt shift. This was confirmed by  changing the sequence of poly cap oxidation and implant in  the process.


Id-Vgs curves  NMOST (1/0.25)


1 μm


1.E-13


1.E-12


1.E-11


1.E-10


1.E-09


1.E-08


1.E-07


1.E-06


1.E-05


1.E-04


1.E-03


-1 -0.75 -0.5 -0.25 0 0.25 0.5 0.75 1


Vgs


Figure 4: I-V characteristics of several NMOS transistors  measured by AFM probing. The pink curve corresponded to  the Nmos showing PEM emission.


Dislocation related failures


Among defects in silicon substrate, dislocations are well  known. Dislocations can be introduced during silicon  substrate preparation, e.g. epilayer growth step, or in a later  stage when stress accumulation in a local area becomes too  high. Implant damage in combination with anneal and  oxidation processes in a LOCOS integration scheme can cause  dislocations [9, 10]. In STI integration dislocations can be  induced related to mechanical stress [11]. In both integration  schemes additional current consumption may be observed  when dislocations pass across junction interfaces. For this  kind of dislocations surface analysis like SCM or passive  voltage contrast are not useful. Probing and electrical  characterization give an indication of the possible failure  mechanism.


Figure 5 shows a typical example of dislocations induced after  implantation and anneal in a LOCOS isolation process. In this  case the failure sites were localized after probing and PEM.


Figure 5: Plan view TEM of dislocations in an LOCOS  integration scheme.


In another case where STI isolation was used significant  randomly distributed yield loss was observed at low supply  voltage. Here no additional Iddq leakage currents were  measured.  The Schmoo of the impacted devices showed an  abrupt pass to fail area below a certain supply voltage well  above the required value.


The failing cell of the scan continuity failures was identified  with electrical characterization. This was achieved by  changing the voltage while passing data through the scan  chain and partitioning. After initialization, the data was shifted  in at a functional voltage towards a specific flip-flop and  subsequently shifted out at a lower voltage. The location was  confirmed by LADA using a 1064 nm laser [12, 13]. See also  figure 6.


bonding interface


Complementary Defect Assessment:


During the method development, locations of defective solder  contacts were estimated using x-ray microscopy (XD7600, Dage). From these known void and known intact positions, ultrasonic data were acquired and signal parameters were  computed for comparison to parameter values obtained at  known intact interconnects. Characteristic parameter ranges of  the peak position, pulse length, BAI and the distributions of


un-bonded一bonded structure


the wavelet coefficients versus time and temporal positions  were estimated from the acoustic data and implemented in the  analysis algorithm. Thresholds for the classification were  defined for each of the mentioned parameters using half of the  Euclidic distance between the mean values of the two  categories.


Verification by SEM and X-Ray Microscopy:


For verification of the methods accuracy, the success rate of  the acoustic defect estimation was evaluated using “unknown” samples. Void positions were estimated from the ultrasonic  data and the binary decision matrix was computed. The results  were handed to an experienced technician for verifying the  defects using X-ray microscopy. Finally, the two rows  containing the highest number of defective contacts were  cross-sectioned, polished, and high resolution imaging was  performed by scanning electron microscopy (TM1000, Hitachi).


Image Processing and Resolution Enhancement (IP-RE)


The potential of acoustic image processing and resolution  enhancement is illustrated by inspecting bonding interfaces  between silicon wafers. Acoustic micrographs were recorded  at the interface of two bonded wafers. Both wafers had a  thickness of 500 μm and were originally prepared and  patterned for mechanical strength testing (chevron- and tensile  tests). Bonding was based on a plasma-activated low  temperature silicon direct wafer bonding process. Prior to the  mechanical tests, samples were inspected by acoustic  microscopy to investigate the geometric accuracy of the  bonded structures, which is of major relevance for the  reliability of the mechanical test results. Acoustic micrographs  were computed from the rectified and integrated echo signal at  the bonding interface. Locations of intact bonding contain a  lower reflectivity at the bonding interface compared to  delaminated or non-bonded regions. When passing interfaces  between materials with differing elastic or mechanical  properties, sound waves are partially reflected and transmitted. The degree of reflection strongly depends on the mismatch in  acoustic impedance between the neighboring materials.


Figure 4: Description of samples used for image processing  and resolution enhancement. Samples consisted of patterned  and bonded wafers for additional mechanical strength testing. Both wafers had a thickness of 500 μm and surface area of 1  mm by 1 mm. The red indicated area was the bonded structure  while the blue indication represents un-bonded interfaces. For  mechanical testing, the accuracy of the bonded structure  strongly impacts the test reliability.


Acoustic impedance is defined as the product of sound  velocity and mass density. The case of a delamination  containing a gas filled gap represents an extreme mismatch in  acoustic impedance resulting in a reflectivity of almost 100 %. Thus, delaminated spots are clearly visible and easy to detect  in acoustic micrographs, although the axial dimension of the  delamination is much smaller than the wavelength of the  acoustic wave. This phenomenon can be considered as the  modulation of the surface reflectivity by a thin gaseous layer. Acoustic micrographs were then processed using image  processing filters for blind deconvolution [4], a Gaussian filter  and a Sobel filter for emphasizing the edges of the bonded  structures, enabling the evaluation of the geometric accuracy. Image contrast was adapted manually for matching the gray  levels to the dynamic range of the images appropriately.


The connectivity of a solder tape on top of a solar panel was  assessed by computing the position of the first cepstral  maximum from time domain signals acquired using acoustic  microscopy. The image in figure 5-top shows a regular  acoustic micrograph of the solar panel with the solder tape in  the vertical center. The contrast in that image arises from the  maximum amplitude of the recorded echo signals. In figure 5-bottom the time domain signals are plotted as an acoustic  cross-section. The position of the cross section corresponds to  over the cross section. On the left side the solder tape is  detached (delaminated) from the bus bar of the solar panel the


red-marked line in the acoustic micrograph in figure 5-top. It  can be seen that the echo distribution is not homogeneous  which causes multiple reflections (reverberations) of the  acoustic signal within the tape. By applying a cepstral analysis  the echo separation and periodicity was extracted. The  parameter matrix containing the position of the first cepstral  maximum is plotted in the top-image of figure 6. This  parameter map corresponds well to the location of the defect  positions that can be derived from figure 5 bottom.


Hilbert transformed X-section


10.1


10.2


豆10.3


3


10.4


L 10.5


10.6


10.7


51015


[mm]


Figure 5: Acoustic inspection of the connective properties of a  Cu ribbon soldered on top of a PV solar panel. Top: regular  acoustic micrograph representing the maximum amplitude  values of the acoustic echo signal. Bottom: Acoustic crosssection along the red marker in the acoustic micrograph (top  image). To the left and to the right delaminated areas can be  seen from the reverberating echoes.


silicon/underfill interface


Figure 6: Results of the parametric imaging based on acoustic  microscopy. Top: Parametric image displaying the peak


0.81.01.21.4 time!us]


position of the cepstrum. Blue regions in the image  correspond to intact soldering and thus, good adhesion. Yellow and red pixels indicate disconnected areas. It can be  seen that most of the tape is not connected to the bus-bar of  the PV-panel. Bottom: Complementary X-Ray micrograph of  the same region of the tape. Some delaminations can be seen, although the contrast of is rather poor.


In the top-image in figure 6 regions of well adhesion between  the tape and the bus-bar can be identified. In locations of  adhesion only an entrance and a small exit echo occur, leading  to a low position index of the cepstral maximum. In contrast, delaminated areas lead to reverberations, resulting in an  increased position index of the cepstral peak and the  corresponding amplitude. In this parametric image, complete  adhesion is expressed in blue, wile increasing values of of the  cepstral maximum position index are stained yellow to red. For  verification of these findings, complementary x-ray  microscopy was performed. The image in figure 6 bottom  shows the results of the x-ray microscopy. Although  delaminations only cause limited absorption contrast in x-ray  some, delaminations can be seen. For contrast improvement  the x-ray images were plotted in false-color.


The parametric imaging enables a simplified  assessment of the solder quality of the contact ribbon. Further  thresholding would allow for binary imaging and automated  classification.


Acoustic Analysis: interconnect localization


According to the acoustic cross-section contained in the image  to the right in figure 3, interconnect positions were located  using the pulse length of the echoes obtained at the  silicon/solder contact interface. In presence of a flip-chip


20


contact, the peak amplitude of the echo at the siliconconnector interface was 200% higher compared to the signals  measured at the interface silicon/underfill. The pulse width  obtained from a contact was 30 ns while the echo at the  silicon/underfill interface was only 10 ns long. 7.


0.4-


ude [V]amplit品


Figure 7: Hilbert transformed and low pass filtered signals. The black and red curves were computed from signals  recorded in presence and absence of an interconnect, respectively.


at fc-contact


between fc-contactssilicon/connector interface


Figure 7 shows two Hilbert transformed signals recorded at the  location of a flip-chip interconnect (black) and in between two  contacts (silicon/underfill) (red). The differences in the peak  amplitudes and pulse widths are evident from the signals  plotted in figure


Acoustic Analysis: defect classification


Wavelet analysis was applied to the echo signals recorded at  the silicon/interconnect interface. Significant differences in the  distributions of the wavelet coefficients were observed  between intact and defect flip-chip contacts. Wavelet  coefficients estimated from a void showed a broader  distribution versus scaling factors and wavelet positions  compared to values obtained from an intact contact.


197


655


17


32008703


Figure 8: Wavelet coefficients estimated at the silicon/solder  interfaces of an intact (left) and at a defect interconnect (right).


In case of a void, wavelet coefficients of equal amplitude  occur with a much broader distribution over all wavelet  positions. The average distribution width over the scaling  factors (sf) was 1.7sf for intact connectors and 2.5sf for the  voids. For illustration, figure 8 contains results obtained by  wavelet analysis. The wavelet coefficients computed from the  ultrasonic signals recorded at an intact flip-chip interconnect  are plotted in the left-hand-side image in figure 8, while the  right-hand-side image illustrates the wavelet coefficients  obtained from a defective interconnect. Distributions were  estimated at 70% of the maximum values. Another parameter  included in the classification was the relative position of the  signal peak at the silicon/solder interface. Pulse shifts of up to  20 ns between intact and defect contacts were observed. Both  parameters were combined in a classifier for increasing the  success rate and to optimize for false- positive classifications. Figure 9 shows the results estimated by the classifier. Green


indicated spots in figure 9-left specify positions of intact  solder-connectors. Voids and false-positive contact positions  are marked red. The settings and parameter ranges applied for  computing the results in figure 9-left were optimized for  classification of the flip chip-contacts at the outer rim of the  flip-chip device. For classifying the inner interconnects the  application of adapted settings will be required to obtain a  robust computation and reliable results. The graph on the  right-hand-side in figure 9 illustrates the individual parameter  values at the interconnect-locations. Parameter values were  thresholded, scaled to 255 (8bit) and plotted color specific in  this graph. At locations where all parameters reached the  threshold defined for an intact connector, the pixel in the  image is white, since the values of each color channel is 255. In locations were an intact flip-chip contact has not been  identified (since not all parameters reached the level of 255), the pixel values deviate from white. Green indicated are all  pixels that have been identified not to be a flip-chip


interconnect.


Verification by SEM and X-ray microscopy


For validation of the defect classification based on the acoustic


microscopy data both, scanning electron and x-ray microscopy  were applied to the same CPU device. The decision map


:


03


(figure 9-left) generated by the analysis algorithm developed  here was given to a technical assistant experienced in void  detection using the x-ray microscope. In Figure 9-center all  voids detected based on the acoustic microscopy data are  indicated by a yellow mark. Red indication in Fig. 9-center  corresponds to voids that have been confirmed by x-ray  microscopy. It can be seen that 8 out of 31 voids estimated  from the acoustic data could not be confirmed by x-ray, although they have been pointed out explicitly by the  acoustically based decision map, which was handed to the


43


technician for assisting the x-ray inspection. This leads to an  assumption of 25.8% false-positive classification. However, in  addition to x-ray microscopy scanning electron microscopy  was applied to the two rows of connectors with the highest  number of voids detected acoustically. For acquiring electron  micrographs the CPU device was sequentially polished to the  middle of each interconnect row and then further prepared for  SEM-imaging. Voids revealed by SEM-imaging are indicated  by a white circle in figure 9-center. It can be seen that thirteen  voids detected by analyzing the ultrasonic echo signals could  be verified by SEM imaging. However, it also shows that two  false-positive and one false-negative detections occurred, which corresponds to an overall success rate of 90.3% including both kinds of false detection. Figure 10 contains  electron micrographs of the contacts that could not be verified  by x-ray microscopy, but were revealed when analyzing  ultrasonic signals obtained by scanning acoustic microscopy. It  can be seen that all of the flip-chip-contacts are disconnected  from the substrate. The numbering in figure 9-center  corresponds to the numbering in figure 10 (top-right corner of  each scanning electron micrograph). The electron micrograph  in figure 10-1 reveals that this particular interconnect is only  partially disconnected and also shows a noticeable thinner gap


SOP DHLA8


Figure 10: Scanning electron micrographs of defective flipchip interconnects in the investigated CPU-device. The  numbering corresponds to the numbering in Fig.9-center  which shows the lateral positions of the contacts.


a38


between the contact and its socket compared to the other  voids. This kind of defect will show an electrical connection  during electronic testing. However, in a practical application  this interconnect will definitely fail due to thermal processes  caused by the applied electrical current. It was somewhat  surprising to see this kind of void being detected nondestructively using acoustic microscopy inspection. The


HCa SWW


micrographs 2 – 6 displayed in figure 10 clearly show the flipchip interconnects to be defective. However, none of these  defects has been detected by x-ray microscopy, although they  have been pointed out explicitly by the acoustically based  decision map (except the interconnect in 10-2, which was a  false positive detection of the acoustic analysis).


SOP SHAME


eoae mn


Image processing was applied to acoustic micrographs  recorded at the bonding interface of wafer bonded structures. The acoustic micrographs did not show sufficient contrast and  sharpness to clearly evaluate defects located at the bonding  interface. In figure 11 the acoustic micrographs prior to the  image processing are plotted in the upper row. Performed was  blind-deconvolution for increasing the sharpness of the


vs*S0PDL


images. Additionally, a Sobel filter was applied to the regions  of interest (ROI’s) in the left and right images in figure 11. A  Gaussian filter was applied to the central image in figure 11. The samples shown to the left and right in figure 11 were  prepared for chevron testing of the bonding strength while the  sample in the center was prepared for a tensile test. The ideal  shapes for performing chevron- and tensile mechanical tests on  bonded structures are illustrated in figure 4. Deviations from


Figure 9: Classification results and evaluation of void detection. LEFT: green indicated are extracted flip-chip contacts. Red interconnects were classified as voids based on the wavelet coefficients and pulse separation characteristics at the  interface silicon/ solder. CENTER: BAI-parametric image with indication of detected voids. Yellow marks correspond to  voids detected using acoustic microscopy data. Red marks indicate where voids were confirmed by X-ray microscopy. White circles indicate where defect contacts were verified by cross-sectioning and SEM imaging. SEM investigations were  only performed on column 3 and 4 (counted from the right-hand-side of the device). RIGHT: superimposed parameter  maps. Red indication corresponds to pulse separation in the “void-range”. Blue marks indicate the wavelet coefficients


b1 2


4 5


6 3


this structure will lead to a falsification of the strength values  and thus of the derived adhesive properties of the tested  samples. The application of acoustic microscopy revealed that  none of the samples shown here were suitable for mechanical  testing, since regions outside the intended structure were also  bonded to the substrate, not allowing the estimation of reliable  results. However, in all three cases small defects have also  been discovered along the edges of the intended bonding  structure. The application of the image processing enabled a  resolution and contrast enhancement for emphasizing defect  sizes and orientations and thus, an evaluation of the samples  suitability in a non-destructive test.


9


Figure 6: Shows the LADA result on a digital scan continuity  fail.


0.5 pm


AFM probing measurements additionally confirmed the  presence of a leakage path. The plan view TEM results are  shown in figure 7 and 8. Figure 7 shows a typical TEM image  of a dislocation loop in the gate area. Figure 8 shows a  dislocation across the active area. Such a dislocation can also  be visualized after performing Wright etch. Then only the  intercepts of the dislocation with the silicon surface are  visible. Although this is a quick check to see whether  dislocations are present little additional information is  obtained.


Figure 7: Plan view TEM showing a dislocation loop in  silicon below the gate. The insert shows an overview of the  active area.


Figure 8: Shows the Plan view of a dislocation across the  active area. The site was identified by electrical  characterization and LADA.


TEM technique is used routinely to reveal the nature of the  crystal defect. The choice of plan view or cross-section can be  a dilemma as shown in the next example. Several CCD image  sensor failed due to leakage current. A PEM spot was  observed in the ~50x30um2 photo diode area of one pixel, (figure 9a), with multiple junctions underneath. While a plan  view TEM has a greater chance to capture the dislocation in  the image, it does not allow us to identify exactly which  junctions are affected by the dislocation, because depth  information is missing. On the other hand, a conventional  TEM cross-section risks missing the dislocation, because it is  very thin, and crystal direction of the defect is not known  beforehand. In order to increase the chance of catching the  defect in TEM cross section, the device was de-processed to  silicon level in HF followed by surface decoration using  Wright etch. This allowed us to identify not only the location


0.2 μm


of the end point, but also the direction of travel of the  dislocation, see Figure 9b. The subsequent TEM cross section


was made in the direction indicated by the arrow. The TEM  cross-section shown in Figure 9c captured the dislocation  inside the silicon. The depth information allowed us to judge  which junctions were involved.


The same principle holds for revealing origin of stacking  faults (SF) in epilayers. This is shown in Figure 10 and 11. The traces of SF decorated by Wright etch indicates the best  direction in which TEM cross section should be prepared. .


Figure 9: (a) PEM spot was observed in the sensor pixel  highlighted, (b) leaking photo diode area after HF strip (left) and after surface decoration by Wright etch (right). The arrow  indicates the projected direction of the dislocation and  subsequent TEM cross section was prepared in this direction.


(c) TEM cross-section showing the dislocation lying on


<111> plane with its lower end running out of the cross  section.


Figure 10: Optical image of the failing area after Wright etch  at the location where OBIRCH signal was observed. Stacking  faults are clearly visible.


Figure 11:TEM cross section made through the origin of the  stacking fault.


PEM spot


11a


11b


dislocation


Etch pit  shown in  11b


11c 0.5 μm


Successful failure analysis is based upon the combination of  good electrical fault localization techniques and appropriate  selection of physical de-processing methods, which are often  destructive and irreversible. In this paper, several case studies  related to abnormalities seen in silicon, namely doping and  crystal defects are discussed. It is demonstrated that, for both  parts, many techniques can be used to compliment each other  to increase the chance of success. The Combination of Wright  etch and TEM cross sectioning reveals depth information  about possible dislocation or stacking faults that could not be  obtained by plan view TEM.


[1] M Bruce, V Bruce, D Eppes, J Wilcox, Ecole, P  Tangyunyong, C Hawkins, “Soft defect localization (SDL) on ICs” Proc. 28th International Symposium for  Testing & Failure Analysis, 2002, pp. 21-27.


[2] R. Mulder, S. Subramanian, T Chrastecky, “Atomic force  probe analysis of non-visible defects in sub-100 nm  CMOS technologies”, Proceedings of the 32nd  International Symposium for Testing and Failure  Analysis, 2006.


[3] Chao-Chi Wu, Jon C. Lee, Jung-Hsiang Chuang, TsungTe Li, “Single device characterization by Nano-probing  to identify failure root cause”, Proc of the 31 International  Symposium for Testing and Failure Analysis, 2005, pp  183 - 185.


[4] P. De Wolf, R. Stephenson, T Trenkler, T. Clarysse, T  Hantschel, “Satus and review of two-dimensionsl carrier  and dopant profiling using scanning probe microscopy,” J. Vac. Sci. Technol. B, 2000, Vol. 18, pp. 361-368.


[5] Frank Siegelin, Anton Stuffer, “Dislocations related  leakage in advanced CMOS devices” Proc. 31th


International Symposium for Testing & Failure Analysis, 2005, pp. 59-63.


[6] Tsan-Chang Chuang et all, “Alternating Plan-View and  Cross-Section Scanning Capacitance Microscope  Technique to reveal various implant issue”, Proc. 33rd  International Symposium for Testing & Failure Analysis, 2007, pp. 52-55.


[7] Po Fu Chou, Chun Yen Chen, “Doping profile inspected  by SEM dopant contrast, wet stain and SCM”, Proc. 35th  International Symposium for Testing & Failure Analysis, 2009, pp. 189-191.


[8] Rock_chen et all, “Junction leakage induced by silicon  dislocation in a 0.13 µm logic process”, 43rd annual  international re;iability physics symposium”, 2005, pp  624 - 625


[9] Shuji Ikeda et all, “ Mechanical stress control in a VLSI  fabrication process: A method for obtaining the relation  between stress levels and stress induced failures”, IEDM  1996, pp 696-703.


[10] P Smeys, “ The influence of oxidation induced stress on  the generation current and its impact on scaled device  performance”, IEDM 1996, pp 709-712.


[11] Shuji Ikeda, Hiroyuki Ohta, Hideo Miura, Yasuhide  Hagiwara, “Mechanical stress control in a VLSIFabrication process: A method for obtaining the relation  between stress levels and stress-induced failures” IEEE  Trans. On Semiconductor Manufactoring, Vol 16, 2003  pp. 696- 703.


[12] J.A. Rowlette, T.M. Eiles, “ Critical timing analysis in  microprocessors using near-IR laser assited device  alteration (LADA)”, ITC 2003, pp 264-273


[13] A. Mels, F. Zachariasse, “Reduce of acquisition time for  RIL, SDL and LADA”, Proc. 33rd International  Symposium for Testing & Failure Analysis, 2007, pp 6 –


13.


# X-sectional Scanning Capacitance Microscopy (SCM) Applications on Deep Submicron Devices at Specific Sites


X-sectional Scanning Capacitance Microscopy (SCM) Applications   on Deep Submicron Devices at Specific Sites


Xiang-Dong Wang, Yuk Tsang, and Clifford Howard


Freescale Semiconductor Inc. Tempe, AZ


In this paper, we present our recent applications of  scanning capacitance microscopy (SCM) on specific devices  with sampling window as small as 100nm. The dopant related  root causes were successfully identified on those devices  fabricated with 90nm CMOS technology. The key step in our  approach is the development of a sample preparation  technique that allows us to precisely x-section through a  transistor without being affected by focused ion beam (FIB) artifacts. FIB was used to mark the area of interest with high  precision, but it did not expose the devices of interest. Optical  microscope and atomic force microscope (AFM) were used to  inspect the mechanically polished surface, thus avoiding beam  effects from FIB or SEM.  In the first application, a doping  anomaly was identified in a PFET poly gate, in a single bit  failed SRAM cell. In the second application, an asymmetry of  a PWell implant profile in a window of 150nm was identified  as the cause of leakage in a capacitor array. Our approach may  be applied to other scanning probe microscopy (SPM) techniques in the same category, i.e., scanning spreading  resistance microscopy (SSRM) or scanning microwave  microscopy (SMM).


With ever shrinking device dimensions of CMOS  integrated circuit technology, related failure analysis becomes  more and more challenging. One such problem has been to  find dopant related failures in a single device after all the high  resolution microcopies failed to capture any physical evidence  of the failure mechanism. While microscopic techniques are  capable of imaging physical defects at atomic level, imaging  dopant remains an obstacle on production chips. TEM  holography [1, 2] and scanning probe microscopy (SPM) based techniques, such as SCM [3, 4], scanning spreading  resistance microscopy (SSRM) [5, 6] and scanning microwave  microscopy (SMM) [7] have demonstrated impressive spatial  resolution and dynamic range in test devices, however, the  success was rarely duplicated in production samples. Complicated circumstances and small isolated devices make  sample preparation and optimization of imaging conditions  very difficult. Previously reported techniques to achieve  precise x-sectioning are mainly based on the combination of  FIB and mechanical polishing [8, 9]. To avoid the high ion  beam energy (Ga+ ion of 5KeV-15KeV) and charge effects, a  considerable amount of material has to be removed with  mechanical polishing. Moreover, in samples that have been


polished down to contact level for atomic force probe (AFP) or other types of physical analyses, the effect of FIB artifacts  is more significant as there is only a thin layer of dielectric  material on silicon. This significantly limited the precision  required to achieve x-section of a single transistor that is  typically smaller than 100nm in modern CMOS chips.


Here we report our approach to x-section through a  specific device for SCM analysis, exemplified by addressing  dopant related root causes in devices fabricated with 90nm  CMOS technology. We were able to determine root causes  related to anomalous doping not only in silicon, but also in  poly gate. The key step in our approach is the development of  a sample preparation technique that allows us to precisely xsection through a transistor without being affected by FIB.


Experiment


The SCM measurements were done on a Digital  Instruments Dimension 3100 SPM with SCM module [10].  While the conducting metal probe is scanning the sample  surface and taking a topography image, the MOS capacitance, consisting of metal probe, silicon surface oxide and the carrier  depletion in silicon under the probe, is detected by a  capacitance sensor. This signal is mapped out in the form of  its derivative dC/dV to achieve very high capacitance  sensitivity. The magnitude and phase are correlated with  dopant concentration and type, respectively. Typically, a  larger dC/dV magnitude corresponds to lower dopant  concentration (although there are circumstances that the  correlations are not straight forward). In our instrument  configuration, brighter features with respect to the background (dielectric areas) correspond to p-type carrier, while darker  features are n-type.


The sample mounting and coarse polishing processes  are similar to a standard SCM sample approach. The sample  was coated with metal prior to being glued to a protective  glass slip so that all the electrodes were at the same potential. Electrical contact is then made to a metal mounting piece at a  x-section somewhat away from the area of interest. The target  x-section is approached in the opposite direction by polishing  the sample using diamond lapping films of decreasing size  down to 0.1 m. The final polishing is done with 0.05um  Silica slurry on a polishing pad.


Figure 1.  SEM image of the area of interest with FIB marks  as landmarks for sample x-sectioning. The PFET with high Vt  is not exposed to either e-beam or ion beam


To successfully achieve SCM measurement in such small  devices, not only does the x-section have to be right on the  target, but its surface has to be atomically smooth, free from  contamination, charge or crystal damage, and thus it has to be  polished mechanically. Exposure to FIB or SEM, especially at  the last stage of sample preparation, can significantly distort or  even completely screen an SCM signal. In our sample  preparation procedure, the area of interest was first marked  with FIB in order to identify the x-section location under an  optical microscope. Those FIB marks were fabricated near the  defective device prior to metal coating. The precise x-section  is achieved by recognizing FIB marks or intrinsic patterns  during the final polishing step. A FIB mark with a depth of  about 0.3 m or more can be well identified under an optical  microscope. To ensure better control, the final polishing was  done by manually moving the sample without spinning the  polishing wheel, which allowed us to control the polishing  depth with <10nm accuracy.


Figure 1 shows an example of such FIB marks made  in a SRAM sample, where trenches were fabricated with an  ion beam next to the failed device. The FIB mark pattern is  designed in such a way that one can identify how close the xsection is to the area of interest when the sample x-section is  inspected optically. To avoid FIB damage, the failed bit was  never exposed to the Ga+ ion beam during the whole process. With those FIB trenches, we were able to determine the xsection by optically inspecting the x-section surface itself. In  addition, AFM/SCM examination was also frequently used to  achieve higher precision.


Results


1) PFET  poly doping issue


The failure we encountered in this case is a type of  single bit SRAM failure on a chip fabricated with 90nm  CMOS technology. The schematic of a SRAM bit cell is  shown in Figure 2. Based on AFP measurement, one of the  PFETs was identified as defective with high Vt shift. The  electrical signature of the failure prompted the hypothesis that  the poly gate, S/D or the channel was not properly doped. SPM based doping profile techniques, such as SCM, SSRM  and SMM, are virtually the only techniques available to  address such an issue.


Figure 2.  Schematic of the bit cell. Active areas (yellow), poly  gates (green), and contacts are shown. X-section for SCM is


perpendicular to the poly lines.


With only approximately 120nm sampling window in  the defective PFET, sample preparation is the key for a  successful SCM measurement. Figure 3b shows the optical  image of the x-section through the failed bit. The unique  pattern formed by shallow trench isolation (STI),  contacts of  the PFET row and the FIB notches indicate that the x-section  is on the target. Finally, a quick AFM scan is performed to  determine the exact x-section location, as shown in Figure 3a. The AFM inspection could become more critical for devices  with smaller dimensions.


Figure 4 shows the SCM image of the PFET with  high Vt, together with reference devices nearby. It can be  clearly noted that the poly with high Vt is imaged brightly, which means low p-type doping concentration. Sample bias  dependent SCM images indicated that the poly gate was still  p-type but with low p-type concentration. For comparison, the  reference gates did not show much contrast or variation with  sample bias due to high concentration level.


PFET with high  Vt


10um


Figure 3.  a) AFM image and b) Optical image of the x-section  area.


Figure 4.  SCM image of the area of interest. The gate poly of  the high Vt PFET (in red circle) appears lighter due to lower  doping level. The FIB trench appears deeper in SCM than its  physical appearance due to ion-beam charge, as described in  ref. [9].


Penall


NAll


NWal


2) Capacitor edge leakage


Figure 5. Schematics of a capacitor structure in an array. a) X-section view and b) plan view. The area of interest is in the  middle, where PWell (black) is separated from P+ (red) by  NWell (blue). The x-section view only exists in the narrow  area outside of poly (green box) but within the active area (white box).


Another problem we encountered is leakage in a  particular capacitor structure as shown in Figure 5. The  suspected area is at the edge of an array of capacitors as  identified by AFP and OBIRCH (Optical Beam Induced  Resistance Change). AFP data at contact level suggest that the  leakage has the characteristic of pnp bipolar transistors and  EMMI data show emission sites at the edge of the capacitor  array. Those results suggest that the leakage is between the p+ and p-well regions. To access the area with SCM, the xsection has to go through the area between the edge of the  active and the edge of poly, which has a window of about 150  nm. Fortunately, in this case, the optical contrast between STI  and silicon is sufficient to determine the location in the xsection by using an optical microscope, with AFM only for  final adjustment.


FIB Trench


Figure 6 shows the SCM image of the area of


1.002.00


interest. It can be immediately noticed that the PWell implant  is somewhat asymmetric. The right side of the PWell extends  much closer to the P+ region. The NWell gap separating  PWell and P+ regions is significantly reduced, resulting in  leakage due to a pnp bipolar punch through mechanism.


可


Figure 6.  a) Topography and b) SCM image of the x-section  area shown in Fig. 5. The PWell is shown asymmetric with


right side closer to p+. The NWell gap is too small to prevent  leakage between PWell and P+.


X-section


The results we were able be achieve have been  satisfactory on products with 90nm CMOS technology. While  plenty of products on the market are fabricated with  technologies larger than 90nm, it is very demanding to access  the ultimate limit for smaller dimensions, which is 22nm node


cty


for the current generation. There are several major limiting  factors, such as 1) the intrinsic limit of the SCM technique, 2)


Pwell (black)


the precision of x-sectioning, and 3) the surface topography  effect caused by mechanical polishing. While the resolution  and sensitivity of SCM has been insufficient in the


Nwel


development of state of the art CMOS technologies in the past, for failure analysis the qualitative relative comparison between  reference device and failed device is usually sufficient. Resolution of a few nanometers has been reported by quite a  few groups, therefore, even at the 22nm node, SCM is still a  promising tool for FA applications.


With a slow polishing rate and frequent AFM/SCM  inspections, the x-sectioning can be precise within a few nm. With the projected technology node in the tens of nm, such  precision is still promising. However, the throughput will


likely become the bottleneck if an automated system is not  available in the near future.


The more significant challenge is the uniformity of  the polished surface. Currently, 50nm silica suspension is  widely used for final x-section polishing. It gives a very  smooth silicon surface, however, the polishing rate is  significantly different for different materials used in the gate  stack, especially silicon, nitride and tungsten. The topography  created by uneven polishing can be significant and can create  artifacts due to the size and shape of the probe. A polishing  recipe with a consistent rate for those materials is therefore  highly desired.


In conclusion, we have shown unique applications of  x-sectional SCM to accurately probe specific areas of deep  sub-micron devices. By mechanical polishing assisted with  FIB marks or other landmarks existing on the dies, we were  able to access specific areas of less than 100nm and provide  direct evidence of doping related failure mechanisms. Our  approach may be applied to other SPM techniques in the same  category, i.e., SSRM or SMM.


The authors would like to acknowledge the support from


Freescale Semiconductor Global Yield FA Labs.


[1]  W. D. Rau, P. Schwander, F. H. Baumann, W. Höppner, and A. Ourmazd, “Two-Dimensional Mapping of the


Electrostatic Potential in Transistors by Electron


Holography”, Phys. Rev. Lett. 82, 2614(1999).


[2]  M. A. Gribelyuk, M. R. McCartney, Jing Li, C. S.


Murthy, P. Ronsheim, B. Doris, J. S. McMurray, S.


Hegde, and David J. Smith, “Mapping of Electrostatic


Potential in Deep Submicron CMOS Devices by Electron  Holography”, Phys. Rev. Lett. 89, 25502 (2002)


[3] C. C. Williams, “Two-Dimensional Dopant Profiling by  Scanning Capacitance Microscopy” Annual Review of


Materials Science, 29, 471-504(1999)


[4] F. Giannazzo, D. Goghero, V. Raineri, S. Mirabella, F.


Priolo, “Scanning Capacitance Microscopy on


Ultranarrow Doping Profiles in Si”, Applied Physics


Letters, 83(13), 2659(2003).


[5] P. Eyben, S. Vemula, T. Noda and W. Vandervorst, ”


Two-dimensional Carrier Profiling with Sub-nm


Resolution Using SSRM: From Basic Concept to TCAD  Calibration and Device Tuning”, Ext. Abs. the 9th


International Workshop on Junction Technology 2009,


p24-28.


[6] L. Zhang, K. Ohuchi, K. Adachi, K. Ishimaru, M.


Takayanagi, A. Nishiyama, “High-resolution


characterization of ultrashallow junctions by measuring in  vacuum with scanning spreading resistance microscopy”,  Applied Physics Letters, 90(19), 192103(2007)


[7]  W. Han, “Introduction to Scanning Microwave


Microscopy Application”, Agilent Application Note, June  16, 2008


[8]  K. Jarausch, J.F. Richards, L. Denney, and A. Guichard, “Site specific 2-D implant profiling using FIB assisted


SCM”, Proceedings of the 28th International Symposium  for Testing and Failure Analysis, p467, Phoenix, Arizona,


2002.


[9] D.K. Fillmore, and S. Wang, “Investigation of LowEnergy Focused Ion Beam Milling for Scanning


Capacitance Microscopy Sample Preparation”,


Conference Proceedings from the 30th International


Symposium for Testing and Failure Analysis, p350,


Worcester, Massachusetts, 2004.


[10] Veeco Instrument, Dimension-3100 scanning probe


microscope system with electrical measurement modules.


Contact author information:


Xiang-Dong Wang


Freescale Semiconductor Inc.


2100 E. Elliot Road


Tempe, AZ 85284


Xiang-Dong.Wang@Freescale.com


480-413-2803


# High Volume and Fast Turnaround Automated Inline TEM Sample Preparation for Manufacturing Process Monitoring


High Volume and Fast Turnaround Automated Inline TEM Sample Preparation for  Manufacturing Process Monitoring


Hyoung H. Kang, John F. King, Oliver D. Patterson, and Steven B. Herschbein  IBM Microelectronics, 2070 Route 52, Hopewell Junction, NY, 12533


hhkang@us.ibm.com


James P. Nadeau and Scott E. Fuller


FEI Company, 5350 NE Dawson Creek Drive, Hillsboro, OR  97124


This paper introduces a high volume and fast turnaround TEM  sample preparation method and requirements for a 300 mm  inline DualBeam (FIB/SEM) system with “hands-off” full  automation. It requires a factory automation system, robust  automated recipes, and an ex-situ TEM lamella liftout system. It describes the recipe structure and TEM lamella lift out  procedures.  The focus is on fully automated TEM sample  preparation for process monitoring in manufacturing line. Two  successful examples are described to demonstrate the benefit  of this method. The first one is TEM sample for CA profile at  M1 level. The second is TEM sample for poly crystalline (PC) line profile at post-etch.


Transmission electron microscope (TEM) analysis has become  a key component for manufacturing process monitoring. Due  to tighter design rules, many conventional cross section  scanning electron microscope (SEM) images do not provide  enough information because of the limit of spatial resolution  and material contrast. The most common TEM lamella  preparation is done in the lab by hand polishing or by a  Focused Ion Beam (FIB) system. Wafers to make TEM  lamellae are transferred to the lab from the fabrication line. Throughput and turnaround of current TEM sample  preparation methods in the lab are limited due to the level of  difficulty and process time required for producing TEM  lamellae. To improve TEM sample preparation time, the plan  view sampling techniques as well as cross sectional whole  wafer TEM sample preparation by a DualBeam (FIB/SEM) system were introduced into the manufacturing environment [1, 2, 3]. For steady TEM lamella preparation, we  implemented a DualBeam system with factory automation into  the wafer process flow in the fab. The DualBeam system is  running fully automated recipes to eliminate the variability of  operator skill level. TEM sampling of electrical short or open  defect in contact arrays at tungsten CMP level was introduced  earlier [4].


This paper introduces the basic process of the recipe for TEM  lamella preparation in a DualBeam system (FEI CLM+™) for  process monitoring and the wizard-driven, semi-automated, ex-situ lamella extraction system (TEMLink™ 150).


Inline “Hands-off” TEM Sample Preparation


To enable “hands-off” TEM sample preparation inline, the  FIB system and liftout system should be considered as  manufacturing tools. Three key components have been  identified to achieve high volume TEM sample preparation: 1) Factory automation system, 2) Robust automated recipes, and  3) Ex-situ TEM lamella liftout with site data connectivity to  the lamella production tool.


Figure 1 (page 2) shows the flow of automated TEM sample  preparation in the manufacturing line. The IBM factory  automation system called SiView controls the wafer flow in  the manufacturing line. The pre-built process route enables  SiView to deliver a job to the tool. The factory automation  system delivers the wafer by priority to the DualBeam  automatically and initiates the lamella preparation process  with the associated recipe. When the lamella preparation is  completed at the DualBeam system, the wafer is returned to a  stocker and waits for the lamella liftout process step. The  lamella is removed from the wafer at the ex-situ liftout tool in  the manufacturing line. Then the lamella is transferred on a  mesh type 3 mm TEM grid. The grid goes into a box to be  delivered to the lab for imaging. The wafer now can be  scrapped or sent to the next process step, depending on  products or regulations. This TEM sample preparation flow  allows production of TEM samples in a 7 day/24 hour  manufacturing environment.  We have achieved a throughput  exceeding 500 TEM samples per month utilizing work shifts  of 15 hours (nights) during the week and two 24 hour weekend  shifts.


Automated Recipe


An automated recipe provides the lamella preparation without  any operator. The recipes are product, process step, macro, and die specific. Once a wafer is aligned, the X, Y coordinate  in the site list of the recipe drives to the area of interest. One  of the key features to deliver highly successful lamellae auto  preparation is to optimize image recognition well. Image  recognition tools in a well established recipe not only drive to  the target location but also provide TEM lamellae on an exact  target feature. In addition, a software measurement tool is  another key feature, which enables the preparation of a lamella  in a location where the area of interest is in a previous buried


process level. The contact array at M1 level example uses the  measurement tool.


|Steps |Process |
|---|---|

|Wafer align 1 |wafer at 0 deg. Rotation |

|Step 1 |C dep (optional), Local fiducials, W dep, |

|Step 2 |Bulk mill – side 1 |

|Step 3 |Clean mill – side 1 |

|Wafer align 2 |wafer at 180 deg. Rotation |

|Step 4 |Bulk mill – side 2 |

|Step 5 |Clean mill – side 2, U-shape undercut |

|Wafer align 3 |wafer at 0 deg. Rotation |

|Step 6 |Thinning – side 1 |

|Wafer align 4 |wafer at 180 deg. Rotation |

|Step 7 |Thinning – side 2 |

|Step 8 |5 kV cleaning – side 2 |

|Wafer align 5 |wafer at 0 deg. rotation |

|Step 9 |5 kV cleaning  – side 1 |

Wafer & Recipe


FIB /SEM


sent by Factory


TEM sample prep


TEM lamellae


Automation


by automated recipe


FOUP transport Stocker to Ex-situ liftout


Wafer with


Figure 1. Flow of automated TEM sample preparation in the  manufacturing line. The factory automation and recipe driven  steps at the FIB/SEM tool allow very fast TEM sample  preparation. The ex-situ liftout tool runs parallel to the  FIB/SEM  tool to save FIB/SEM process time.


Automated Recipe Procedures


The recipe includes the process steps of wafer alignment, protective layer deposition, thin lamella preparation, and low  kV cleaning with the FIB. Table 1 shows the process steps in a  typical recipe. The conventional method of TEM sample prep  requires stage tilt to achieve the uniform thickness of the  upper and lower parts of lamella, and to make the undercuts to  enable sample extraction. The undercuts are completed during  steps 2-5 listed in table 1. On the CLM+ it is the ion beam  column, not the stage that is tilted. Because of this and to  improve overall sample preparation efficiency the recipe  includes several global wafer alignments between recipe steps  that involve milling on different sides of the lamellae. In  addition, each recipe step is performed to all sites on the wafer  before moving to the next step to minimize overhead in  changing beam conditions etc. The keen local fiducials in


Ex-Situ Liftout


FOUP transport


Table 1. The process steps in a typical recipe. When preparing


Lift out lamellae


SiView Lot Released Ex-situ liftout to Stocker


multiple samples on a wafer each of the wafer alignment steps


Transfer to TEM grids


are performed once for the wafer, with the interim steps (e.g. steps 1-3) occurring for all sites.


step 1 allow keeping the target location with different beam   conditions during the process. Passes 2 through 8 use fiducials  created in pass 1. Electron beam induced carbon deposition  preserves the surface profile without ion beam damage. An


TEM grid(s) transferred


High resolution TEM


optional deposition step using 400 pA e-beam at 2.5 kV is


to transport box


imaging in lab


used to provide well defined carbon depositions reliably. The


Sample tracking


Image storage / export


current carbon deposition process time is 20 minutes on a 2 µm x 3 µm area for 150 nm thick depositions. Naphthalene is  used for carbon deposition. The lamella preparation time by  the FIB takes approximately 22 minutes per lamella. The good  quality of ion beam images at 5 kV provides high success of  image recognition. The low kV cleaning pattern can be  automatically placed on the surface of thin lamella. The low  kV cleaning steps take about 3 minutes per lamella to run both  sides. The total process time to produce a typical lamella is  about 45 minutes with the carbon deposition step and 25  minutes without the carbon deposition step using a fully  automated recipe run. In comparison, the conventional manual  lab lamella preparation methods took up to ½ a day per sample  on average with additional laser marking and TEOS and/or  chromium deposition processes, but not including additional  other overhead such as wafer scrap procedure and transferring  wafer to lab.


Image recognition is a key component to enable the recipe to  run fully automated. The image recognition features in the  recipe allows driving to the area of interest and locating the  deposition or milling pattern on the target location. Figure 2  shows an example of image recognition steps to place the  carbon deposition by e-beam in (a)-(e) and to place the micro  FIB fiducials on the location in (f)-(g). The structure is  polycrystalline macro array after reactive ion etching. The  image recognition tool compares the newly captured image (a)


and the pre-retrained reference image (b). The tool  superimposes the yellow lines for coarse match and the green  lines for fine match in (b). The result of image matching  between (a) and (b) is shown graphically in (c) with its  numerical score (d) to show the similarity of the two images. It shows one area matched with 99.2% success. The higher  score of the image matching provides a higher success of


(B)


Current Trainlmage


running the automated recipe. In the manufacturing line there


are variations from wafer-to-wafer or die-to-die processes, (especially when running processing experiments with  different conditions), that can cause the failure of image  matching due to the structures being slightly different. To


。


develop highly successful image matching results a large  image sampling is required that take into account these


con


variations.


Once the image matching tool finds the matched image the  stage moves or the beam shift tool is applied to place the  carbon deposition at desired location. After the carbon


e the  carbon deposition at desired location. After the carbon


|D|Scoon|X|丫 0.60|Angle 0.00|Fid Erar 0.120|Coverage 0.963|
|---|---|---|---|---|---|---|

(d)1 Resull


deposition process is completed the exact target location must  be located by FIB. Figure 2 (e) shows the ion beam image


00.99210.60


after the carbon deposition. Similar to SEM image matching, the tool compares the new ion beam image (e) and the saved  reference ion beam image (f). Once the image matching is  successfully completed, the micro FIB fiducial pattern shown  in pink (e) is located within the designated area. It is located 4 µm below from the target area in this recipe. The micro  fiducial is used to locate the larger fiducials used from step 2  in table 1. The image recognition with SEM and FIB is key in  making a “hands-off” fully automated recipe.


Figure 3 shows a typical TEM lamella sample prepared by a


IDSconefully automated recipe driven process on the FIB/SEM tool.


00.993


Lamella Liftout


To maximize the productivity of the sample preparation, the  liftout process is done by an ex-situ liftout tool. The ex-situ


liftout tool runs with automated wafer and TEM grid  alignments and a semi-automated software wizard, which  steps the user through the lamella extraction process using  exported lamella location data from the FIB/SEM tool. The


(e)


Cument Trainlmoge(f)


(g)1 Result


Figure 2. The image recognition process. (a) the captured  image by SEM, (b) the pre-trained reference image, (c) run  image and (d) the result of image matching. (e) FIB image, (f) pre-trained reference image and (g) match score.


Figure 3. Typical TEM lamella prepared by fully automated  recipe driven process (a) SEM images at the end of  automation step and (b) TEM images shows the thin area of  the lamella is approximately 2 um × 2.5 um.


0.036


0.07


P8


Probe approaches lamella. applies vacuum to


attach lamella and retracts, breaking it free


0.08


90.5


0.082


0.084


Figure 4. The lamella  cross section image. The  thickness of the lamella is  70nm at 100 nm below the


Probe with detached lamella rotates to orient the


hmsurface.


lamella for placement on TEM grid


g0


ex-situ liftout tool runs in parallel to the FIB/SEM tool to  maximize available FIB/SEM process tool time.


Liftout Process


Probe places lamella on TEM grid, applies pressure


After the wafers have been processed in the FIB system and


to release, stage retracts, leaving lamella on grid


Factory Automation records updated, the wafers with the  prepared lamellae are queued for ex-situ liftout.


In the described procedures, the ex-situ liftout operator is  notified of the queued liftout job through SiView. The wafer is  requisitioned from the stock and delivered to the workstation. A TEM specimen grid must be loaded into the liftout system. After loading the TEM grid and the wafer, the liftout process  is guided by step-by-step instructions. The system  automatically aligns the grid so the lifted lamella can be  placed onto the grid in predetermined locations for ease in  managing the sample locations later during the TEM imaging  phase.


When the wafer is unloaded from the FIB, an XML report  containing the FIB processing records including Lot, Wafer,  FOUP ID numbers, wafer alignment, and lamella navigation  information is created. The operator is directed to load the  FIB-generated XML navigation file associated with the wafer. To accommodate the many product types that use similar  alignment strategies, the ex-situ liftout system can store  automated alignment recipes. The operator can run either a  saved auto-alignment or automatically drive to alignment  positions and manually align the wafer followed by automatic  navigation to the TEM sample sites for ex-situ lift out. Figures  5 and 6 graphically illustrate the main ex-situ liftout steps, which the operator carries out guided by a series of prompts  from the control software.


Liftout is performed using a hollow quartz probe thinned to a  few microns in diameter with an end cleaved at a 45° angle. The probe is lowered into the lamella site and gently driven to  push against the lamella, breaking the thin tabs holding


Figure 5. Lift out steps are (a) at the lamella site. (b) the  liftout probe is lowered into the milled area. (c) the probe  pushes against the lamella, breaks the tabs holding it in place, and holds the freed lamella to the probe using vacuum. (d) the  probe lifts out of the lamella cavity and rotates 180° in  preparation for placement onto the grid. (e) the probe drops to  the grid and places(f) the lamella. (g) a lamella loaded grid.


Figure 6. (a) the lamella site with probe ready for lift out. (b) lamella on probe. (c) probe with lamella ready for placement  on grid. (d) lamella placed on grid. Images are from the  ex-situ liftout tool.


the lamella in place, as shown in figure 3. Vacuum applied in  the hollow probe holds the freed lamella to the probe face. After liftout of the lamella, the stage drives to the grid location. The probe is rotated 180° facing the lamella downward in  preparation for placement onto the grid. The probe is slowly  lowered to the grid surface where the lamella touches and  attaches to the grid surface. The system indexes to the  remaining sites for liftout and placement onto the grid. A grid  report describing the filled grid locations is generated. The  operator unloads the TEM specimen grid, stores it in a  transportation container, documents the material, updates the  status in the Factory Automation system, and then sends the  material on for TEM analysis. Typical liftout process time is  approximately 2 minutes per lamella.


Examples of Auto TEM Sample Preparation  Contact Array at M1


The first example is a construction analysis of the contact  array at the metal 1 level. The profile and location of contact is  one of the key features to monitor. The dislocation of the  contact array causes an electrical short or open in the device. This construction analysis is performed after the electrical  measurement at the M1 level to correlate the yield. Figure 7


(a) shows the macro design layout information with active  area, poly line, contact array, and M1. Figure 7 (b) and (c) show the images of corresponding TEM samples prepared by  the fully automated recipe in the cross section of area  locations 1 and 2, respectively. The image recognition tool  finds the area with only M1 macro information with strong  contrast. The edge finder tools identify the line boundaries of  M1. The measurement tools locate the target area of lamella at  the exact contact array based on M1 design data. Unique  image recognitions are captured and saved for location 1 and  location 2 during recipe creation. Since the area of interest is  at a contact array, the damage of M1 surface is allowed. Carbon deposition is not necessary in this recipe, resulting in  much faster sample preparation. The lamellae of two different  locations were obtained about 100 µm apart in this example.


Polycrystalline Line CD


The second example is monitoring poly line critical dimension (CD) profiles after reactive ion etching (RIE or dry etching) processing.


The standard FIB based protective layer typically damages the  poly line surface. Therefore, an electron beam induced  deposition is employed to deposit an alternative carbon layer.  This carbon deposition was identified as the best choice for  this step to highlight details and poly line profiles while  maintaining structural integrity. Figure 8 shows example  images from TEM lamella samples prepared by this new inline


Figure 7. The design macro layout information in (a) and  images of corresponding TEM samples prepared by full  automated recipe in (b) and (c).


method and by conventional lab methods. The result shows  the same profile from the samples with the two different  methods. The nitride base hard mask is highlighted on the  image with carbon deposition in figure 8(a). The lamella in  figure 8(b) is deposited TEOS done in the lab with the  conventional method. The poly line examples are from the  same wafer dozens of microns apart.


Figure 8. TEM images of poly line profile at post RIE. Samples are prepared (a) by inline technique with ebeam  induced carbon deposition and (b) by conventional method  with TEOS deposition.


The inline FIB/SEM and ex-situ liftout systems provide high  throughput TEM lamella preparation for key process  monitoring. The factory automation capability, recipe base run  with image recognition and measurement tools allows  generating “hands-off” TEM lamella preparation. Two key  process monitoring works are presented: contact array profile  at M1 and poly line profile at post etch.


The authors wish to thank Mark Hudson, Matthew Lamberti, Lisa Santiago, Darrell Hardy, Jennifer Mierzwa, Richard  Hurley, Keith Nickerson, Marylee Saglibene, Michael   Gribelyuk, and Jinhong Li for providing the sample  preparation work and TEM images, and Chris Marotta and  Judy Green for support with the manuscript. This work was  performed at the IBM Microelectronics Division, Hopewell  Junction, NY 12533.


1. H. Kang, M. Gribelyuk, O. Patterson, S. Herschbein, and  C. Senowitz “A New Method of Wafer Level Plan View  TEM Sample Preparation by DualBeam”, Proceedings of  ISTFA 2008, p168-171


2. J. Demarest, Z DeSouza, ”Start up of a Dual Beam FIB  for Automatic STEM Sample Preparation”, Proceedings  of ISTFA 2009, p334-338


3. N. Bicais-Lepinay, F. Andre, S. Brevers, P. Guyader, C. Trouiller, L.F.Tz. Kwakman, S. Pokrant, D. Verkleij, R. Schampers, L. Ithier, E. Sicurani, C. Wyon, “Inline TEM  Sample Preparation and Wafer Return Strategy for Rapid  Yield Learning” Proc. of SPIE, p.615217, 2006.


4. X. Zhou, O. Patterson, W. Lee, H Kang, R. Hahn, “Characterization of Contact Module Failure Mechanisms  for SOI Technologies Using e-Beam Inspection and Inline  TEM” to be published, ASMC, 2010


# Backscattered Electron Imaging for Embedded Subtle Defects in 32nm Processes


Backscattered Electron Imaging for Embedded Subtle Defects in 32nm  Processes


Z. G. Song1, H. S. Song2, J. Yu3 and T. Su1


1IBM, 2Samsung Electronics Co. and 3GLOBALFOUNDRIES Singapore   1IBM STG-MD, Hopewell Junction, NY


Although the overall spatial resolution of backscattered  electron (BSE) imaging suffers in comparison to secondary  electron (SE) imaging, its superior sensitivity to atomic  number (Z) contrast and ability to image through overlying  insulation levels can provide a complementary approach for  imaging subtle buried defects. BSE enables the localization  and imaging of embedded defects through overlying insulator  levels without the risk of compromising them with reactive  ion etch (RIE) or plasma etch exposure or by anisotropic wet  chemical delayering process steps. Once the embedded defect  is localized with BSE in situ, subsequent imaging by cross  sectional Transmission Electron Microscopy (XTEM) combined with elemental analysis by energy dispersive X-Ray  analysis (EDX) or electron energy loss spectroscopy (EELs) can be performed without the risk of introducing artifacts. In  this work, BSE imaging was successfully employed to image  embedded subtle defects in 32nm node technologies through  overlying insulator films not possible with conventional SE  imaging techniques.


Scanning electron microscopy (SEM) is a fundamental  technique essential to any failure analysis lab for localizing  and imaging defects in semiconductor devices. In most cases, secondary electron (SE) imaging can provide a high resolution  image of a defect if the defect is at or near the surface with  detailed surface morphology [1]. With shrinking device sizes, the implementation of twelve or more copper metallization  levels coupled with low k back end of the line (BEOL) dielectric insulator films , the procedure of topdown  delayering with parallel polish followed by topdown SEM  inspection has been adopted. This approach is especially true  for 32nm node technologies. As a result, parallel topdown  polishing without any anisotropic wet etching followed by  SEM inspection is practiced to expose the desired layer of  interest in the course of performing failure analysis. This  topdown iterative polishing followed by SEM inspection  means that most imaged defects are embedded within the  dielectric films under a planar polished surface. Thus, this  approach places a premium on BSE capability of localizing  and imaging embedded defects as compared to conventional  SE imaging techniques. The SE image signal is dependent


upon the secondary electrons generated within a shallow depth (a few nanometers) below the specimen surface [2]. In  comparison, the backscattered electron (BSE) image signal  emanating  from  below the specimen surface enables BSE  imaging to provide depth information as well as atomic  number information associated with the embedded defect. This also enables the BSE imaging to provide a signal not  only of the surface but also from a significant depth within the  specimen [3]. Furthermore, the interlevel dielectric thickness  is now within the information depth of BSE imaging with  selected beam energies. In advanced semiconductor processes  such as the 32nm technology node, the contact dielectric  thickness (CA) is approximately 200 nm. This thinner  dielectric thickness combined with the superior sensitivity of  BSE in imaging high atomic number contrast materials  provides more application opportunities for BSE imaging in  failure analysis of advanced semiconductor devices.


Comparison of SE Imaging and BSE Imaging


SEM has two basic imaging modes, namely secondary  electron imaging and backscattered electron imaging, based  on the two types of electrons generated from the interaction  between the incident electrons and the specimen. In the mode  of SE imaging, the secondary electrons are generated from  inelastic electron scattering events caused by the interaction  between the specimen's electrons and the incident electrons. The SE usually has less than 50eV of energy so that only the  SEs within few nanometers depth below the specimen surface  can escape from the specimen and reach the detector to form  an image [2]. In comparison, in the mode of BSE imaging, the  backscattered electrons are generated from wide angle  Rutherford scattering events resulting from the interaction  between the incident electrons and the specimen atomic nuclei


[4]. Because the elastic scattering involves only a small  energy exchange, most BSEs have energies not too far below  the incident electron energy and can escape from a depth of up  to about half the penetration depth below the specimen surface


[5]. This fact enables the BSE imaging to have deeper  information depth than SE imaging and permits the imaging of  features from significant depth within the specimen [3]. Another difference between these two imaging modes is the  sources of the image contrast. The secondary electron yield is  greatly influenced by the topography of specimen surface  feature and also the angle of the incident electron beam with


respect to the specimen surface. So, the contrast of  the SE  image is mainly topographical contrast. Another contrast  source for SE image is specimen charging, called voltage  contrast. The number of backscattered electrons ejected from  the specimen is proportional to the specimen material's mean  atomic number. Thus the contrast of BSE image is mainly  atomic number contrast, namely Z contrast [6]. In addition, the “doughnut” type design of BSE detector located  underneath the objective lens further reduces the possible  topographical contrast and makes the Z contrast more  pronounced. These features enable BSE imaging to have more  advantages than SE imaging to localize subtle defects  embedded in dielectric with planar polished surfaces.


BSE Imaging Application


Although the overall spatial resolution of backscattered  electron imaging is not as good as that of secondary electron  imaging, BSE imaging, with its atomic number (Z) contrast  and deep information depth, can provide a better methods for  imaging embedded subtle defects under planar polished  surfaces. For advanced semiconductor integrated circuits, a  significant number of submicron features are composed of  high Z materials, such as Cu with Ta/TaN, W, or NiSi on PC  and active region encapsulated in a low Z matrix, such as  SiCOH, or SiO2, whose thickness is well within the BSE  sampling depth. A tiny defect composed of these high Z  materials  can result in malfunction of the device. BSE  localizing and imaging them avoids the risk of introducing  artifacts by RIE/plasma etching or anisotropic wet chemical  etch delayering techniques. By avoiding these delayering  steps, the embedded defect remains intact, encapsulated in the  insulator film. Subsequent analysis like cross-sectional  Transmission Electron Microscopy (XTEM) analysis followed  by EDX or EELs can be followed without the risk of  compromising the defect. In this work, BSE imaging was  performed to image embedded subtle defects, which were not  visible or clearly seen with SE imaging.


1. Poly Level Defect


A SRAM chip exhibited a local bitline failure with one bit  passing. Following the previously described delayering  procedure, the sample was parallel polished to contact level  and the passive voltage contrast (PVC) technique was  performed at the suspected defect area with beam energy of  1KeV. Figure 1 shows this PVC image, disclosing a wordline  poly contact exhibiting a bright contrast at the pass bit of the  local bitline failure. Then SE imaging with beam energy of  20KeV was tried to capture any defect at this location. The SE  image is shown in Figure 2, but nothing abnormal was  indicated. When BSE imaging was selected, a poly stringer  was clearly visible as  shown in the BSE image of Figure 3. This poly stringer made the wordline poly short to the bitline  contact, leading to the local bitline failure with one bit pass. The fact that BSE image showed up the subtle poly stringer  under interlayer dielectric was benefitted from its two  advantages, namely Z contrast and deep information depth.


The poly stringer, which was likely silicided, had higher mean  atomic number than the surrounding materials so that it  showed bright contrast in the BSE image.   The same type of  defect was also captured in a chip with single bit failure (SCF) by BSE imaging, after both PVC and SE images failed in  capturing any abnormality. Figure 4 and Figure 5 showed the  SE and BSE images at contact level for the singe cell failure, respectively. Again, BSE image clearly showed a poly  stringer, which shorted the local poly to Vdd contact, leading  to a single bit failure, while SE image did not show any  defect. Since the poly stringer happened in PFET for this case, PVC image would not show any abnormal contrast because  PFET contacts were always bright in PVC image.


Figure 1: PVC image showing bright contrast for a wordline  poly contact for bitline failure with one bit pass.


Figure 2: SE image of the area with bright wordline poly  contact showing normal.


S48000kV 6.8mm x130kGBSE


400nm


Figure 3: BSE image of the area with bright wordline poly  contact showing a poly stringer.


20.0kV 4.9mm x15uk SE(U)


''s00mm


Figure 4: SE image at contact level of a SCF showing normal.


||. .|
|---|---|

|20.0kV 7.7mmx200k YA|'200mm'|

S4800 20.0kV 7.2mm x150k


Figure 5: BSE image at contact level of the same SCF  showing a poly stringer.


2. Active Level Defect


Another SRAM chip with single bit failure was de-layered to  contact level after SEM inspection for the cross-coupling  metal 1 did not find any abnormality. PVC image at contact  level was taken at the location of the failing bit and showed in  Figure 6. From Figure 6, one can easily find that a rectangular


contact of the failing bit showed abnormally dark contrast. This indicated that the rectangular contact was open to PFET  active. After the tungsten in contacts was removed chemically, both SE imaging and BSE imaging were tried to capture any  defect underneath the contact. Figure 7 and Figure 8 showed  the SE image and BSE image, respectively. The SE image  showed clear profile of contacts and blurry poly profile, but  no difference underneath the contacts was resolved because  the active was far below the specimen surface. Employing the  BSE superior atomic number Z contrast and greater sampling  depth, the BSE image showed clear pattern of poly, active and  contact. It was found that the PFET active was foreshortening  at the location of the dark rectangular contact. It made the  rectangular contact land on STI instead of active, leading to an  open rectangular contact for the single bit failure.


1.0kV48mmx50OkSE(


Figure 6: PVC image at contact level of a single cell fail  showing dark contrast of a rectangular contact.


300nm


Figure 7: SE image at the dark rectangular contact showing  normal contrast after contact W removal.


S4800 20.0k/ 7.2mmx150k


300mm


S4800 20.0kV 7.2mm x100k


Figure 8: BSE image at the dark rectangular contact showing  the PFET active foreshortening after contact W removal.


3. Metal Level Defect


Another SRAM chip with vertical pair bit failure (VPF) was  parallel polished to Via1 level, and PVC image did not show  any abnormality. SE image was taken at the VPF location and  showed in Figure 9. Figure 9 did not show obvious defect and  just a little dark for the bitline island metal 1. While, BSE  image in Figure 10 clearly showed Cu void in the bitline  island metal 1. Again, it was the Z contrast that enabled BSE  imaging to image the tiny Cu void in Cu line. This hollow  bitline island metal 1 caused high resistance in the bitline  stack, leading to vertical pair bit failure. After localizing the  Cu void embedded in the low-K dielectric, a follow-up XTEM  analysis can be employed to further identify the root cause of  Cu void. Exposing the Cu void for SE imaging by either  RIE/plasma etching or anisotropic wet chemical etch would  compromise the defect and prevent determining root cause .


|理|理|
|---|---|

|S4800 10.0kV 5.1mm x100k|500nm|

Figure 9: SE image at Via 1 level of a vertical pair fail (VPF) showing a slight dark contrast in bitline island metal.


500mm


Figure 10: BSE image at Via 1 level of the same vertical pair  fail (VPF) showing hollow bitline island metal.


The wafers and the fail site location lists were delivered to the  in-line FIB.  The requisite combination of conventional stage  movements and local visual reference marker beam pans were  used to center the exact failing cell under the ion beam.  A  tracking marker was milled a short distance away so that the  cell coordinates could be easily located later.


A pattern box of approximately 10 μm x 10 μm was centered  over the cell, and planar topside milling was performed over  the entire region.  The mill progress was stopped as each layer  came into view, and an inspection image was captured at each  level.  A depth monitor to enable automation was proposed by  running a parallel milling pattern over a metal stack of distinct  shapes added along the array edge.  Pattern recognition could  be taught to “see” and stop, as each layers distinct shape is  uncovered.


M4


Starting Point – SRAM fully  functional at M4.  Outer box  defines mill region.


Figure 3.  Localized FIB milling from M4 down to M1.  Highly planar topside milling can be achieved on thin wire  mixed field layers in the SRAM array with the right beam  conditions.


Block Reference (0,0)


y = 20.3


x = 4.56


(0,0)


V3, M3


M3, V2


V2


M2


Fail bit location


defined by the top


left corner of the cell.


V1


M1


As we were milling a mixed field of copper and dielectric, it  was natural to assume that we would run into a materials and  grain dependent channeling issue.  But we found that in this  relatively dense field of minimum thickness and line width  copper, this was not the case under certain conditions. If we  kept the beam current per unit area fairly high (above 10 picoamperes per square micron), the removal rate across the  region was quite uniform.  The milling quality was so  consistent that passive voltage contrast often revealed the  failure site as the cell circuit elements became electrically  isolated.


Finally, the site was marked for cross-sectioning as shown by  the two mill boxes in the next set of images.  A repetitive FIBSEM cut-and-view technique was used to slice through the  cell structure until the failure site could be photographed and  the failure mechanism determined.  TEM lamella preparation  of more difficult to image defects could also be implemented  with only a modification to the final slice and imaging steps


[6].


Figure 4.  Planar milled down beyond M1 to the tungsten  contact level.  Target cell location (defined as upper left  corner) is reasonably centered, and the defective stud is  visible (dark) with beam induced passive voltage contrast.  Cross-section shows incomplete etch.


Extendibility


After some refinement to the last navigation step we were able  to consistently reduce mill box placement error over the  failing cell to under 100 nanometer.  This is certainly suitable


for use on SRAM arrays at the 65 nanometer node, and maybe  a bit beyond.  We believe that advanced image processing  working in conjunction with better built-in markers could  improve this further.  Finally, a better magnification  calibration routine to work with pattern drawing and/or direct  beam pans (deflection) would reduce the error at this last  critical step.


This work shows the potential of implementing a high  volume, highly automated in-line failure analysis technique.  It enables the accurate localization of prior level defects, as it  is selectively driven by electrical test data and not just by the  typical PLY program visual indicators.  It has the potential to  aid early learning and thus could help drive rapid yield  improvement.  The ability to return unbroken wafers to the  line for further processing is an added bonus of implementing  this methodology [6].


[1] Berndlmaier, Z., et al, “The Grand Pareto: A Methodology  for Identifying and Quantifying Yield Detractors in a  Technology for Volume Semiconductor Manufacturing,” ASMC 2006, The 17th Annual SEMI/IEEE, Boston, MA, May  2006, pp. 405-410.


[2] R. Weiland, et al, “Wafer Conserving Full Range  Construction Analysis for IC Fabrication and Process  Development based on FIB / Dual Beam Inline Application,” Proc. 26th ISTFA, Bellevue WA, Nov. 2000, pp. 393-396.


[3] G. Franco, et al, “An Initial Investigation into the use of  FIB Technology for In-line Process Control of Critical  Dimensions in the FAB,” Proc. Of ISSM 2005, San Jose, CA, Sept. 2005, pp. 394-397.


[4] S. Blanc-Coquand, et al, “Automated Defect Crosssectioning with a In-line Dualbeam,” SPIE Metrology & Inspection Conference 2004, Santa Clara, CA, Sept. 2005, pp. 819-896.


[5] S. Herschbein, et al, “Manufacturing In-Line Whole Wafer  Focused Ion Beam (FIB) Memory Address Descramble  Verification,” Proc. 34th ISTFA, Portland, OR, Nov. 2008, pp. 128-132


[6] N. Bicais-Lepinay, et al, “In-Line TEM Sample  Preparation and Wafer Return Strategy for Rapid Yield  Learning”, Proc. of SPIE, Vol 6152, San Jose, CA, Feb. 2006


# Simulation Studies of Fluorine-induced Corrosion and Defects on Microchip Al Bondpads in Wafer Fabrication


Simulation Studies of Fluorine-induced Corrosion and Defects on Microchip   Al Bondpads in Wafer Fabrication


Globalfoundries Singapore Pte. Ltd.


60 Woodlands Industrial Park D, Street 2  Singapore,738406


Email: huayounan@globalfoundries.com


Fluorine-induced corrosion is one of the well-known  failure modes of Al bondpad leading to non-stick on pad (NSOP) issues. Exposure to moisture (H2O) and atmosphere (O2) play an important role in determining the shape and size  of the Al-F corrosion defects on the Al bondpad surface. In  this paper, we will propose a laboratory simulation  methodology that can reproduce F-induced defects observed  either at the wafer fab or the assembly house. The  methodology, known as SLAT (Shelf Lifetime Acceleration  Test), is used to study the relationship between the F-corrosion  defects and the relative temperature (T) and humidity (RH %). It is observed that Al-F corrosion defects simulated are similar  to the real defects found in wafer fab and assembly house in  our previous studies. A relatively higher T and lower RH % results in the formation of the “crystal-like” defects, but if a  relatively lower T and higher RH % condition is used, the “oxide-like” defects were formed. In this paper, we will  compare the simulation results to the real defects found in the  previous cases and discuss the failure mechanism. From the  present study, the importance of controlling T and RH % during wafer storage to eliminate F-induced defects will be  highlighted.


In wafer fabrication (fab), it is a well known fact that Fluorine (F) contamination may cause F-induced corrosion and defects  on microchip Al bondpads, resulting in bondpad discoloration  or non-stick on pads (NSOP). In authors’ previous studies, the  theory, failure mechanism, characteristics and eliminating  solutions of Fluorine-induced corrosion have been studied [1-2]. In this paper, we will further study the failure mechanism  of the F-induced corrosion on Al bondpads, with emphasis on  the relationship between the defects and the relative humidity, RH %, and temperature, T, using a laboratory simulation  method. It will be shown that RH % and T impact differently  on the F-induced corrosion which is reflected in the  morphology of the defects. The present study highlights the  importance of controlling RH % and T during wafer storage to  eliminate F-induced defects.


According to theoretical models proposed in authors’ previous  studies [1-2], F will chemically react with Al and form Al  fluoride ([AlFx](x-3)-). Moreover, during fab process or wafer  storage, O2 and H2O (moisture) in atmosphere will enhance F  corrosion and cause chemical reactions to generate a more  complex compound, Al fluoride oxide (AlxOyFz). Based on the  defect morphology, the F-induced corrosion defects are  classified as the “flower-like”, “crystal-like”, “oxide-like” and “cloud-like” defects [3].  The defects will be observed on the  Al pad surface in the wafer fab as well as in the assemblyhouse. Based on the qualification methodology proposed by  us, a good bondpad should be free of the above defects [4].


In this paper, we will propose a laboratory simulation  methodology (SLAT–Shelf Lifetime Acceleration Test), which can be used for Al bondpad reliability qualification. Using this methodology, one can simulate different F-induced  defects observed in the wafer fab and assembly house by using  temperature and RH % as the control parameters. From this  simulation test, one can obtain further insights about how the  T and RH % influence the formation of different F-induced  defects. The simulation results in this study correspond to oneyear wafer shelf-life storage under the conditions controlled in  the wafer fab and assembly house.


Introduction of Theoretical Models


Fluorine-Induced Corrosion Model


Fluorine contamination on Al bondpads will cause corrosion  and form the F-induced defects. Fluorine will chemically react  with Al and form Al fluoride:


Al + xF-     [AlFx](x-3)- + 3e-          (1) Where the x in [AlFx](x-3)- could be 3 or 6, depending on the F  contamination level and storage conditions. Based on the  above chemical reactions, the “flower-like” defects would be  formed [1-2]. If x=6, Al-F complex compound is [AlF6]3- :


Al + 6F-  [AlF6]3-  + 3e-           (2)


[AlF6]3- is a chemically stable compound. Once formed, a  normal wafer fab cleaning process cannot remove it.


According to our previous studies [1-3], [AlF6]3- formed may  undergo further chemical reaction in the presence of O2 and  moisture (H2O):


3O2 + 6H2O + 12e- → 12OH-


(3)


12OH- + 4Al           → 4Al(OH)3 + 12e-


↓  - 6H2O


2Al2O3


After some complex chemical reactions, Al fluoride oxideAlxOyFz defects may be formed:


[AlFx](x-3)- + Al2O3    AlxOyFz         (4) Based on the above chemical mechanism, we could  understand that moisture (H2O) and oxygen (O2) from  environment will enhance F-induced corrosion. This means  that different corrosion defects may be formed at the different  conditions of the RH % and T. This is why N2 wafer storage  practice is always recommended in the semiconductor  industry. The main purpose is to reduce or isolate moisture  and O2 from the wafer bondpad surface during wafer storage. We postulate that the RH % and T will influence the formation  of the different F-induced defects. In general, Al fluoride  defects could be simulated, which are similar to the real  defects found in wafer fab and assembly house. Our  simulation results showed that if relatively higher temperature  and lower RH % are used, the “crystalline-like” Al-F defects  will be formed. However if relatively higher RH % and lower   temperature are used, the “oxide-like” Al-F defects will be  formed.


Hallberg-Peck Simulation Model


In wafer fabrication, we have observed that F-induced  corrosion reaction does not take place instantaneously. The  chemical reaction is slow and the defects will be formed over  a certain period of time. The surface F at% contamination  level on the Al pad and the wafer storage conditions are the  two important factors that govern the reaction rate. The  implication of the slow reaction dynamics is that the Finduced defects may still not form before wafer fabout and  thus, the ‘defective’ wafers will appear clean at wafer fab  OQA (out-going quality assurance) inspection. However, after  wafer storage or assembly process, the F-induced defects may  be formed slowly. As such, we have to develop a simulation  methodology to evaluate the reliability of wafer bondpad  integrity.


A wafer shelf lifetime acceleration test (SLAT) simulation  methodology has been developed (a USA and Singapore  patent has been filed). In this methodology, Hallberg-Peck  simulation model is used where both temperature and  humidity (RH %) are treated as two key factors that contribute  to the acceleration factor, which is given by,


AF = (AF, H) × (AF, T)                         (5)


or


AF = (RHu/ RHt)-3 × Exp [(Ea/K)*{1/(Tu)–1/(Tt)}]


(6) Where Ea, the activation energy is 0.7eV; K is Boltzmann’s  constant and Tu and Tt are the storage and simulation  temperatures, respectively, expressed in degree Kelvin. Similarly, RHu and RHt refer to the relative humidity during  the wafer storage and simulation.


All the factors and parameters in Eqn (5-6) can be determined  based on the real wafer storage conditions in wafer fab and  assembly house. The wafer storage conditions may be  different for different fab or assembly house.


A Simulation Methodology - SLAT


SLAT reliability test consists of the following components:


(i) the simulation test itself, (ii) the FA measurements before  and after the SLAT, and (iii) the pass-fail criteria. The  flowchart of the SLAT procedure is shown below.


Figure 1: Flowchart of the SLAT simulation and the FA  methodology. OSAT stands for the FA techniques of Optical, SEM, Auger and TEM. Refer to the text for the wafer pass  criteria.


A wafer subjected to SLAT reliability test is considered to  have ‘passed’ the test if it can meet the FA OSAT  characterization conditions of a good bondpad, both before  and after SLAT. This FA procedure was developed by us for  the bondpad process optimization and published elsewhere


Meet


Pass


criteria?


Processed Wafer


Pre-SLAT FA


(OSAT)


Post-SLAT FA


SLAT


(High T & RH%


Simulation)


Wafer Reject


Wafer Fail


Yes


No


Wafer Pass


[4]. The OSAT conditions are: (i) No discoloration under  optical inspection; (ii) Defect-free bondpad surface under  SEM inspection under high magnifications (at x25k, x50k, x100k and x150k); (iii) Carbon (C) and Fluorine (F) contamination level on the bondpad surface should be within  the control limits by Auger Electron Spectroscopy analysis  and (iv) The Al oxide on the bondpad surface measured using  TEM should be uniform with sufficient thickness, which acts  as a passivation layer to prevent Al pad corrosion [4].


A wafer subjected to SLAT reliability test is considered to  have ‘failed’ the test if the F-induced corrosion defects are  formed on the surface of Al bondpads after simulation test.  In this paper, two successful cases of the simulation study will  be presented and discussed. It will be shown that it is possible  to simulate two kinds of F-induced corrosion defects that are  normally observed in wafer fab and the assembly house in our  previous studies [3].


As the semiconductor device geometries continue to shrink  with multiple low K BEOL dielectric films being employed, there is an increased trend of employing BSE inspection of the  sample just after parallel polish without any etch to expose the  layer of interest during failure analysis. With the help of   atomic number (Z) contrast and deep information depth, backscattered electron imaging (BSE) exhibits superior  sensitivity in imaging embedded subtle defects under planar  polished specimen surface. With the latest process technology, where the contact level (CA) interlevel dielectric film  thickness is within the backscatter electron sampling depth, there are clear advantages of BSE inspection as compared to  secondary electron imaging. BSE also enjoys other advantages  in that it can minimize the risk of compromising a subtle  embedded defect without resorting to RIE/plasma  deprocessing or anisotropic chemical etching for  localization/imaging as compared to secondary electron  surface inspection. By avoiding compromising the embedded  defect, follow-on cross sectional TEM analysis involving  EDX and EELs can be performed.


This work was performed at the IBM Microelectronics, Div. Semiconductor Research & Development Center, Hopewell  Junction, NY 12533.


[1] L. Reimer, “Image Formation in Low-Voltage Scanning  Electron Microscopy”, SPIE Optical Engineering, Bellingham, WA, (1993).


[2] T.E. Everhart, O.C. Wells and C. W. Oatley, “Factors  Affecting Contrast and Resolution in the Scanning  Electron Microscope”, J. Electron Control, 7 (1959), pp.


97.


[3] L. M. Gignac, M. Kawasaki, S. H. Boettcher and O.C. Wells, “Imaging and Analysis of Substrate Cu  Interconnects by Detecting Backscattered Electrons in the


Scanning Electron Microscope”, J. Appl. Physics, 97 (2005), pp. 114506.


[4] Niedrig, “Scanning Electron Microscopy”, SEM Inc., Chicago, IL, (1978), pp. 841.


[5] L. Reimer, “Scanning Electron Microscopy: Physics of  Image Formation and Microanalysis”, Springer Seriers  Optical Sciences, Vol. 45 (Springer Berlin, 1985), pp.


131.


[6] J. L. Abraham and P.B. DeNee, “ Scanning Electron  Microscope Histochemistry sing Backscatter Electrons  and Metal Stains”, Lancet, 19 (1973),  pp. 1125.


# Semi-Automated Full Wafer In-line SRAM Failure Analysis By Dual Beam Focused Ion Beam (FIB)


Semi-Automated Full Wafer In-line SRAM Failure Analysis   By Dual Beam Focused Ion Beam (FIB)


Steven B. Herschbein, Hyoung H. Kang, Harvey E. Berman,  Carmelo F Scrudato, Aaron D. Shore


IBM Systems & Technology, Hopewell Junction, NY  12533


Bing Dai


Stanford University, Stanford, CA  94305


The presence of a full wafer dual-beam FIB on the process  floor gave rise to an environment in which formerly  segregated off-line lab and FAB tasks could be linked.  One  such idea involved a methodology for semi-automated defect  targeting based on the spatial predictions of static random  access memory (SRAM) electrical testing.  The embedded  memory blocks on some processors are fully configured and  probe pad testable as early as the forth metal level.  Using a  unique navigation technique that combines electrically sorted  SRAM bit map data with CAD coordinate information and  stage driven X-Y stepping, the FIB tool was used to locate, section and image prior level defects.  We believe that with  the inclusion of suitable fiducial markers in the chip design  and advanced pattern recognition to aid navigation and guide  depth milling, a fully automated process for electrical yield  detractor diagnosis could be introduced.


Defect detection and control strategies, sometimes referred to  as visual Process Limited Yield (PLY) analysis, are an  integral part of process line management. A variety of light  optical and SEM based inspection tools scan a limited region  in selected spots of the wafer.  A determination and binning of  the defect types based on a library of shapes and sizes are  recorded, and a Pareto generated that reflects on the overall  health of the line.  Unfortunately, due to throughput  limitations, these commonly used methodologies are limited to  a small sampling scan area.  They are mostly, with the  exception of high current e-beam voltage contrast, ‘at level’ techniques, with limited sensitivity to prior level defects.


The eTPLY (electrical PLY) concept takes this to the next  level.  Typically, the electrical bit-fail map (BFM) data from  an intermediate or final test is overlaid with the PLY inline  photo inspection or conventional wafer-breaking laboratory  failure analysis results.  This cross-correlation of electrical  performance to visual findings graphically shows the direct  impact of physical defects [1].  The technique described here  is similar to eTPLY but with a number of key enhancements.  Most notable is the ability to rapidly collect a large amount of  prior level data from multiple sites across a number of


SRAM blocks on various die, while keeping the wafer intact.  Removal from the FAB and wafer breakage is not required per  the traditional methods used in the past.


Lab to FAB Transition


The collection and sorting of large amounts of data is essential  to accurately determining the health of the line.  Post process  laboratory analysis can provide very detailed reports on  failures that are difficult to analyze, but is generally not well  suited to producing a statistically significant volume of  information. Recognizing this need, a few papers have been  published on the value of the in-line FIB as an early learning  tool for construction analysis and defect root-cause  determination [2] [3] [4] and as a supplement to traditional  SEM and optical in-line defect review tools.


The installation of an FEI DA-300hp in-line dual-beam FIB  on the IBM 300mm wafer line in East Fishkill, NY created a  number of opportunities to move traditional failure analysis  tasks out of the lab and onto the process floor.  Navigation on  this tool across the entire wafer to any suspected defect site or  array block can be achieved using an X-Y stepping coordinate  system, or by layout design information. Employing both a  gallium focused ion beam for milling and a high resolution  electron beam for imaging, the tool has the ability to do  precision cross-sections or top-down delayering of selected  features.


Unlike its arguably higher performance small chamber  laboratory counterpart, the in-line dual-beam FIB allows  direct inspection of the site and the preparation and removal of  a TEM lamella without scrapping the wafer from the lot or  removing the wafer from the line.


Determining Defect Location


Many in-line inspection strategies are executed using SRAM  arrays, and this work was no different in that regard.  Arrays  are typically chosen because of their high density repetitive  structures, with each level drawn near or at minimum ground  rules.  Surface pattern recognition using either stored images  or adjacent block image subtraction can be used to find  common at-level defects.


Finding prior level defects takes additional resources.  Assuming that the memory address descramble is correct, a  fully testable array can be bitmapped and used to pinpoint the  physical location of soft and hard electrical failures with high  spatial resolution.  As a basic SRAM build requires all front  end processes and typically only the first 3-4 metal  interconnect levels, it makes a good vehicle for this work.  Unfortunately, many processor designs are not optimized to  allow direct address access to embedded arrays as an early inline test, but require filtering thru core logic on the finished  product.  Furthermore, if the descramble layout accuracy was  not electrically verified, the failing cell called out in a bit map  may not be physically near the suggested location, resulting in  continuous 'no defect found' analyses [5].


Our work was made possible by choosing processors that had  specifically designed embedded SRAM arrays that allowed  full bitmapping at M4 wafer probe.  This was done as part of  an overall ‘Design for Failure Analysis’ strategy to enable  rapid Pareto Analysis.  Bitmap accuracy (address and data  state) had been extensively verified by prior teams, as this was  a popular yield analysis vehicle.


Most of the experimental work in phase one of this study was  performed on 90 nm product.  Compared to processes in  development, this older technology is physically large, mature, and stable with a very low defect density.  We knew  that we needed to refine our targeting strategy beyond what  the basic FIB stage was capable of driving to in a single move, and did not want to be thrown off by false hits from nearby  defects.


As discussed above, 300 mm wafers with specifically  designed in-line probe card testable SRAM arrays were pulled  for evaluation at M4.  Bit map results on these previously  certified arrays identified the X/Y locations of randomly  occurring process defects.  Probable failure mode binning was  then applied to the captured electrical signatures.  Based on a  wealth of historical data, this provided a starting point  prediction of what type of physical failure we could expect to  find at each site.  Further refinement could be obtained by  doing extensive schmoo analysis to eliminate soft or transitory  fails.


In the end, a subset of the failure population was chosen for  detailed in-line FIB failure analysis.  The selected candidates  represented electrical fail modes that had a high probability of  yielding obvious & unique visible defects at lower metal  levels.  The selection of unambiguous sites was done mainly  so that we could test out the validity of the localization  technique and correct for any navigation errors that might be  encountered.


An internally developed algorithm was written to cross-map  the SRAM row and column electrical signature to a physical  X-Y site location in the layout CAD.  This was in turn  translated to a micrometer stepping distance from a known


scribe lane landmark (wafer fiducial).  But given the stage  accuracy/repeatability of a conventional FAB review type  tool, a single step ‘drive to’ instruction could only get us  close.  Typically we landed within a few microns, and  nowhere near the required submicron targeting.


VDD (VP)


GND (VP)


Figure 1.  Basic failure mode and mechanism predictions  based on historical data of a 6T SRAM (layout - top) when  matched with electrical bitmap results.


Obtaining the level of performance needed for a fully  automated data collection process would require the  development of a machine automation recipe and pattern  recognition tools trained to work with a new set of unique, locally distributed die markers.  We simulated this procedure  manually during our work, and believe that it is possible to do  with currently available technology.  In this multi-step  methodology, we began at the wafer alignment fiducial and  initially drove to a target marker at the corner of the  designated SRAM array.  The operator (FIB automation) would identify, lock on and re-center this point in the field of  view, and a second stage move was performed to center a new  target marker in the sub-array block closest to the failing cell. The final ‘move’ from the block marker to the center of the  failing cell requires a different approach to obtain precision  targeting.  We were somewhat surprised during our initial  attempts to find that a stage move of even only a few microns


WL (HP)


BLC (VP)


VDD (SC)


(SC)


(VP)


Structure to Fail  Mode Relationship


Single  Cell (SC)


Quad  Cell


Horizontal  Pair (HP)


Vertical  Pair (VP)


S - D short


X


S - D open


S - D contact open


Poly contact open


Poly short


Poly open


M1 short


M1 open


M1-M2 open


X X


was still subject to a highly variable degree of inaccuracy;  enough to sometime place us on the wrong cell.  To correct  for this, the stage was held constant and the final alignment  targeting was done using a combination of drawn pattern mill  boxes, beam pans and FIB milled markers.  All of this relies  on accurate magnification calibration, but with M4 design  markers in place the tool could conceivably be taught to check  itself and periodically adjust to maintain accuracy.


Figure 2.  Final steps in the relocation process.  A new local  origin nearest the failing cell is defining, and becomes the  reference point for highly accurate mill box placement.  Bottom photo rotated 90’ in relation to the top photo.


Figure 3(a) shows the SEM image at the end of the sample  preparation step. Figure 3(b) shows the low magnification  TEM image. The entire lamella is approximately 8 µm in  width with a central 2 µm thinned window containing the  region of interest for TEM analysis. The thickness of the  lamella is typically 70 nm ± 10 nm, 3 sigma with a lamella cut  placement variation of 10 nm, 3 sigma. The tabs on each side  hold the lamella samples securely while the wafer is  transferring inline.


(8)


Figure 4 shows an example of a lamella cross section. The  thickness is 70 nm and 80 nm at 100 nm and 200 nm in depth, respectively. This image was created using the automated  cross-sectioning, imaging and metrology capabilities of the  CLM+. In this way a large number of automatically prepared  TEM samples can be coated, sectioned and measured to  provide detailed statistics on sample thickness, uniformity and  placement accuracy.


Relat


In ou which


4. Th the S“crys surfac magn defec


if subjecte iments need to


e 3: Post-SLA mination level low F at%. Th  Al-pad and   relatively hig


the above sim tion of such d; (ii) Exposur igh Temperat ll as wafer sto  formation of ust control th as at the asse binets to preve


ively Lower T


r previous stu  was related to ese defects w MIF pods dur tal-like” defec es. One has ifications (> x ts.


A)


B)


d to prolo  be carried out


T SEM images s are shown a e “crystal-lik similar in sha her T and lowe


ulation result,efects requires e to moisture  ure. Therefore rage at the ass  these kinds o e surface F a mbly house th nt exposure to


+ Higher RH


dies [1-3], w


the “oxide-li


ere caused by


ing the fab p


ts, they do no


to perform


50k) in order


nged simula


to test the hyp


of Al pads wi bove, (A) – hi e” defects wer pe to those s r RH % condi


one can unde: (i) Wafer wit(H2O) and ox, wafer proces embly house  f defects. In  t% level on th e wafers shou  moisture (H2O


%


e reported a


ke” defects, as


F cross conta


rocesses [3] a


t have well-d


SEM imagi


to observe th


tion. Further


othesis.


th different Fgh F at% and e observed for hown in Fig.2 tions..


rstand that the h high surface ygen (O2) and sing in the fab will contribute the wafer fab e Al bondpad ld be stored in) and oxygen


bondpad issue  shown in Fig mination from nd, unlike the efined faceted ng at higher e “oxide-like”


,


Figu defec


Figu(B), stora


In th relati proce bond 1). S for th 5(A)


re 4: SEM im ts on the affec


re 5: SEM ima taken after t ge under relat


e second exper vely lower T  ssed with dif pads, referred  EM images of e two wafers, showed defec(A)


age showed  ted Al pad.


ges of high-F  he SLAT sim ively lower T a


iment, simula and higher RH ferent initial F to as high- an  the simulated. The Al pad ts after the sim


wafer, (A), an ulation for o nd higher RH


tion test was c %. Again, tw-contaminatio d low- F at%  results are sh s of wafer wi ulation while


ke” corrosion


d low-F wafer ne-year wafe % conditions.


onducted using o wafers wer n level on th(refer to Tabl own in Fig. 5 th high-F, Fig  the Al pads o


, r


e  e  e . f


low-F wafer continued to be defect-free even after the  simulation, Fig. 5(B).


A comparison of Fig. 4 and Fig. 5(A) would suggest that the  agreement between the two is qualitative; especially the size  of defects is quite different. Moreover, the number density of  the simulated defects appears to be larger compared to the  actual case. These discrepancies are possibly related to the  bondpad surface F-contamination on the actual wafer and the  simulated wafer being not identical.


The dependence of the shape and size of Al-F defects on the  simulation test conditions (T and RH %) can be qualitatively  understood in terms of the F-induced corrosion mechanism  described in the beginning of the paper. As was pointed out, in  the presence of O2 and moisture (H2O) F-induced corrosion  would be enhanced. Thus, simulation under relatively higher  RH % should have more F-corrosion sites (Fig. 5(A)) as  compared to that with lower RH % (Fig. 3(A)). Moreover, the  defects are the “oxide-like” as there was more moisture and  oxygen during chemical reaction.


Wafer Storage


The SLAT simulation test is an effective wafer-level  reliability test to evaluate bondpad integrity. The wafers may  be stored either at a wafer fab or an assembly house. The  SLAT simulation results presented in this paper were obtained  with two different values for the acceleration factor, AF, (eqn. 5, Hallberg-Peck model) using two sets of T and RH %. Finduced corrosion defects were simulated on wafers with high  surface F-contamination (F > 9.0 at%) for the two AF values  studied. It is interesting to note that for the same simulation  condition, wafers with low surface F contamination did not  show any corrosion defects. These results are of significant  importance to fab process of Si wafers and the post-fab wafer  storage as they highlight the importance of temperature and  humidity (RH %) in F-induced corrosion and also the  dependence of the nature of defects (size and shape) on test  conditions – conversely, the shape and size of F-induced  corrosion defects on the field-returned wafers/chips can throw  light on the storage conditions.


The Al pad opening process uses F-based gas chemistry and  therefore, by-products containing F-radicals will be generated. Thus, it is practically impossible to have F-free bondpad  surface. However, based on our study results, a Al pad with  low F-contamination (~3-6 at%, depends on fab process used) would be less susceptible to F-induced corrosion (refer to Fig. 3(B) and Fig. 5(B)). However, one must note that this is based  on the assumption the wafers are stored in controlled  atmosphere, such as wafer boxes/canisters with good vacuum  seal or/and N2 storage cabinets.


A shelf lifetime acceleration test (SLAT) was proposed for  simulating the F-induced corrosion defects on the microchip  Al pads. It was shown that under appropriate conditions of  relatively higher T and RH % (high as compared to ambient  conditions) the laboratory simulation test can reproduce the


real F-induced corrosion defects found in wafer fab and  assembly house. Furthermore, one could study the interplay  between the defect morphology and RH % – the “crystal-like” defects are observed at the simulation conditions of relatively  higher T and lower RH %, while the “oxide-like” defects are  observed for relatively lower T and higher RH %. Thus, it is  very important for wafer fab to control F contamination level  on Al pad surface and for assembly house to control wafer  storage conditions (such as temperature and RH %) to prevent/ eliminate pad corrosion.


The authors would like to thank the GLOBALFOUNDRIES  Singapore Pte Ltd FA Lab SEM (Chen Shuting) and Auger (Yang Yanjing and Long Penny) teams for their contributions  to this technical paper. Also special thanks to Dr Daminda  Dahanayaka from the technical committee of ISTFA 2010  conference for providing technical and professional advice.


[1] Hua, Younan, et al.,  “A study on Non-Stick Aluminum  Bondpads due to Fluorine Contamination using SEM, EDX, TEM, IC, Auger, XPS & TOF-SIMS,” Proc 28th   Int’l Symp for Testing and Failure Analysis, Phoenix, Arizona, November 2002, pp. 494-504.


[2] Hua, Younan, et al., “A Study on Fluorine-Induced  Corrosion on Microchip Aluminum Bondpads,” Proc 29th   Int’l Symp for Testing and Failure Analysis, Santa Clara, CA, November 2003, pp. 249-255.


[3] Hua, Younan, et al., “Studies on Fluorine-Induced  Corrosion and Defects on Microchip Al Bondpads and  Elimination Solutions,” Proc 34th Int’l Symp for Testing  and Failure Analysis, Portland, Oregon, November 2008, pp. 285-290.


[4] Hua, Younan, et al., “Studies on a Qualification Method (OSAT) of Microchip Al Bondpads in Wafer  Fabrication,” Proc 35th Int’l Symp for Testing and Failure  Analysis, San Jose, California, November 2009, pp. 289-292.


# A Novel Wet Etch In-situ Decapsulation of Devices on Boards


A Novel Wet Etch In-situ Decapsulation of Devices on Boards


Michael A. Gonzales, Joanna Kiljan   Qualcomm, Inc., San Diego, CA, U.S.A. michaelg@qualcomm.com, 858 651-8605


This paper presents a novel technique for decapsulation of  integrated circuits (ICs) mounted on printed circuit boards. This  technique overcomes wet etch related sidewall blowouts that  damage or alter the performance of the IC and board under test.  It  also allows well defined etch geometries and better endpoint  detection. This is accomplished by protecting the region of  interest (ROI) with a fast-curing, acid-resistant maskant that peels  off easily.  The technique was successfully utilized on a densely  populated board, which exhibited temperature sensitive failure  mechanism, as discussed in this paper.


Decapsulation is often the first method used in failure analysis  sample preparation [1]. It is an essential technique for removing  the packaging material from an integrated circuit.  Typical  decapsulation of ICs with plastic packages involves directing a  stream of hot fuming acid onto the mold compound to expose the  region of interest.  This area can include the entire die or just a  select area [2].  Best results are achieved when the ROI is  sufficiently masked with rubber gaskets and sealants to prevent  damage to the surrounding surface and bottom of the board.  A  large variety of prefabricated rubber gaskets are available.  With  the proper milling tools or with an X-acto knife, a perfectly sized  gasket can be custom made.


High temperature automated “Jet etchers” were not designed to  decapsulate ICs that are mounted on heavily populated printed  circuit boards (PCBs).  However, if the board dimensions allow  and alignment is not a problem it would work perfectly well. Some failure analysts have been successful but for the most part  have difficulty achieving accurate etch head alignment and  repeatable realignment with board level decapsulations without  some sort of fixture and method of protecting components on  both sides of the board.  A gasket or package sidewall “blowout” would be catastrophic for the entire board unless measures were  taken to protect it from such an event.


Other techniques for removal of the plastic mold compound


used in IC packages include laser ablation [3], milling or dry


chemical etching [4,5].  All of them have their place, but they


can be expensive, time consuming and not practical for IC  decapsulation on a fully populated board.


The rest of this paper describes the procedure of in-situ  decapsulation using a maskant, and follows with a specific  practical example of an application for this technique.


In-situ decapsulation of an on board IC maintains the  conditions and environment of the IC in question and  preserves full functionality (or lack of) as a system.  It allows  for a more thorough and systematic approach to the failure  analysis process prior to any destructive analysis.  Often the  IC is blamed for the system failure without the opportunity to  diagnose the impact of the surrounding components.  For  example,  parts can recover after removal from the board, making it difficult to determine the failure.  This technique  provides opportunities for analysis of surface mount  components at system level.


The method described makes this technique accessible to most  failure analysis chemical laboratories.  Other than a UV  source, the tools needed are common to all IC failure analysis  chemical labs.  This methodology, which is based on selective  masking, preserves the board and package connections yet still  provides access to wire bonded and flip chip devices for  further failure analysis.  Additional benefits of this method  include easy cleanup and no damage to the board and  component connections.


Procedure


Package Analysis


Accurate information regarding the geometry of the die inside  the package is necessary for correct placement of a masking  material.  It can be obtained from bonding diagrams or  radiographic analysis.  A conversion ratio can easily be  determined by comparing the dimensions of the radiograph to  the dimensions of the actual part.


Masking Products


Some of the masking materials include tapes, waxes, and  silicone RTV compounds.  Some tapes and non-adhesive films  provide protection and work well against splash or harsh  vapors.  They can rarely  withstand hot fuming mineral acids.  Curable agents such as silicon RTV provide excellent  protection, but suffer long cure times and are difficult to  remove.  Trying to remove it can result in excessive force that  can stress the components, weaken their connection or pull  them out completely.  The use of mold release can prevent the  necessary adhesion or add other variables that may  compromise the device.


To overcome long cure times and adhesion problems, we use a  single component UV/light curable maskant that cures in  seconds instead of hours.  SpeedMask ®  730-BT Ultra LightWeld ® is a peelable, temporary maskant with a high viscosity  that allows the product to stay in place long enough to cure  under a UV/light source.  The maskant is trimmable after  curing and easily removed by peeling.


Masking Procedure


Package Preparation


Figure 1 shows a typical board having four ROIs on three  different ICs.  In this case, one wire bonded “upside” device  and three flip chip devices were requested by the analyst for  full corner-to-corner die exposure. A fine point scribe enabled  accurate and precise guidelines for the masking agent  application.


Figure 1: Example of a board with four ROI prior to adding  masking agent.


Premilling a cavity into the mold compound of the package  can be done to minimize etch times but is generally not  necessary. Radiographic measurements can guide our  dimensions.  It is useful but not critical to be perfectly flat to  the plane of the ROI.  The milled channel will help guide the  definition of the decapsulation geometry. If it is necessary to  premill we have found it useful to mount the board on  standoffs and secure the base of the standoffs with a UV cure  product (Dymax Speedmask 726) as shown in figure 2.


Figure 2: Example of quick temporary attachment of a board  to a milling tool stage.


The masking product comes in a 30 cc syringe and is   dispensed using an 18 gauge blunt needle. The maskant is  viscous enough to maintain its shape and can easily be nudged  up to the pre-scribed lines.  Capillary action will capture the  maskant along the scribe lines for surprisingly accurate  alignment.  Figure 3 shows the maskant applied directly to a  device and board adjacent to the ROI.  Figure 4 shows a board  with the cured maskant.


Figure 3: Application of the masking agent.


Figure 4: Example of a board after adding and curing the  masking agent.


Determine the shortest path that waste acid will travel as it  rolls off of the board.  Surround the ROI with the masking  agent and continue to protect the components to the edge of  the board.  Create a small wall of maskant around the ROI(s).  This will serve as a small reservoir to allow the acid to stay in  contact with the mold compound.  Mask the edge and part of  the backside to protect these areas from acid.


Curing


A Cure Spot 50 Ultraviolet  source was used.  The intensity  was factory set to maximize bulb life yet allow workable  exposure time.  Newer models have an intensity adjustment  available.  A full cure was defined as giving the proper  adhesion bond strength, hardness and surface tack to resist 75  oC hot fuming nitric acid.  Through several trials, we  determined our minimum lower exposure time to be 10  seconds per cm2 and while no upper limit has been established  there have been no detrimental effects when the exposure time  has been tripled.  The UV source has a fiber optic wand that is  supported by an adjustable stand.  A UV shield for eye and  skin protection, timer and foot control provide a safe and easy  to use environment.  The entire set-up is shown in Figure 3.  Place the board with the maskant under the fiber optic wand  about 5 mm from the surface of the maskant.  Activate the foot  switch and move the board to expose all the maskant while  paying special attention to shaded areas around the  components.


Figure 5: UV source with a fiber optic wand and adjustable  stand.  The shield provides skin and eye protection.


Decapsulation


Chemical Procedure


A mixture containing 30 mL of 90% fuming nitric acid and 10  mL of 20% fuming sulfuric acid is placed in a 100 mL Pyrex  beaker and heated on a hot plate to 70 oC. The sulfuric acid  volume can be reduced to make the nitric acid more  aggressive.  Place the board on the hotplate or hold the board  horizontally in your hand.  Place the acid into the maskant  reservoir using a disposable type glass pipette and latex rubber  bulb to test its reactivity with the mold compound.  Typically  there will be a delayed bubbling which soon subsides after the  acid is consumed. Tip the board and allow the acid to drip  down the short path that is protected with maskant.  Continue  to add the acid more vigorously, directing the stream of acid  into the corners while maintaining a perpendicular approach to  the device.  This will keep the walls steep and follow the


pattern of the maskant.  As shown in Figure 6, the die will  begin to appear.


Figure 6: Applying the acid mix to the device.


Continue the process until the full die emerges.  Some of the  maskant will react and begin to obscure the view.  Quench the  reaction by submerging the board in a beaker of water.  Place  the beaker and the board in an ultrasonic bath for 10 seconds.  Follow this with a spray of acetone to clean up the reacted  maskant and mold compound.  Follow with an N2 blow dry.  Inspect the sample as in Figure 7 and repeat if necessary.


Figure 7: Other than some residual polyimide and loose mold  compound, the sample is ready for final cleaning.


When the sample has been etched to the analysts satisfaction, place the portion of the board being decapped in a beaker of  Dynasolve CU-7 heated to 85 Co. Place the beaker in the  ultrasonic bath for approximately 15 seconds. This will  remove any reacted organic material including residual  polyimide. A final water rinse to remove the Dynasolve CU-7  followed by a quick spray of acetone and N2 to dry the sample  will complete the decapsulation process.  This should result in  a near pristine sample that is functional.  The Dynasolve  product is reusable for many samples.


Alternatively if the sample does not lend itself to ultrasonic  submersion, it is easy to spray water from a water bottle or  dispense hot Dynasolve CU-7 with a pipette and latex rubber  bulb.  Ultrasonic may or may not be desirable depending on


the analyst’s evaluation of the sample (i.e. large exposed bond  wires) but generally produces cleaner results.


This revival of the dropper method brings back the ability to  monitor the endpoint in real time.  Confidence is quickly built  up as the die below the ROI emerges with each stream of acid.  If needed, the process can be quenched for inspection and  repeated as necessary since the maskant will survive repeated  applications.  Near anisotropic etch geometry is achieved by  directing the acid perpendicular to the plane of the device.


Maskant Removal


After providing surface protection to the package and  surrounding components, the mask is carefully peeled off and  inspected as shown in Figure 8.


Figure 8: Maskant peels off easily, yet protects the board.


It is best to nudge it off beginning at the edges and working  toward the center.  Once removed, follow up with a stream of  acetone or isopropyl alcohol as a final rinse.  Blow dry with  clean dry air or nitrogen and inspect.  See Figure 9.


Figure 9: Wet-etch in-situ decapsulation of multiple ICs on  circuit boards can be accomplished with one maskant  application.


During final product testing at the board level, a temperature  sensitive boot-up failure was detected. With additional testing  and probing, a possible failure site was isolated to three  integrated circuit (IC) components on the board.  Due to the  nature of this failure, care was taken to avoid any additional  thermal stress to the board, which could have altered the  reported failure mechanism. Therefore, any further analysis of  the three components had to be performed on the board.  Prior  to decapsulation, X-ray and C-SAM analyses showed no  anomalies. After in-situ decapsulation both a reference and the  failing boards were retested to check if their performance has  changed after the procedure. No change was measured at this  step. Emission microscopy followed the retesting. Both boards  were powered up and initialized into a boot-up mode, at which  point their IC emission sites were recorded. Results of the  emission work are shown in Figure 10. The power  management IC from the failing unit has much fewer emission  sites compared to its counterpart on the reference board. One  of the affected regions on the power management IC  corresponds to internal crystal oscillator circuit block, which  provides reference clock to other circuit blocks and other  components on the board.  Improper functioning of the crystal  oscillator circuit was identified as the root cause for the board  not powering up properly.


Figure 10: Results of the emission work preformed on the  failing unit (left side) and on the reference unit (right side).


Successful in-situ decapsulation allowed for a quick and nondestructive analysis of the on-board ICs. This technique  proved to be the key to isolating the failing component.


We have demonstrated in-situ on board decapsulation with the  capability to preserve the symbiotic nature of the original  failure.  It continues to be a critical tool in decapsulating ICs  while still on the board.  It has provided many more options  and better diagnostic capabilities while allowing the option to  remove the IC if further analysis is necessary.


This procedure has also minimized the number of practice  parts needed.  Once the analyst becomes familiar with the  products and procedures the immediate feedback of exposing  the ROI by directing the stream of hot acid allows for many  one-of-a-kind analyses with a high percentage of success.


This procedure is certainly not designed to replace any of the  laser ablation or dry etch methods in use but rather to  supplement and enhance the variety of techniques currently  available to the failure analyst.


The authors would like to thank Michael DiBattista, Martin  Villafana, George Gaut and Babak Motamedi for their editing  and previewing of this paper. We would also like to thank  Jamie Langley and Sook Sengthean for their support and  continuation of this work.  Also Bernardo Diaz del Castillo for  the photo documentation and composition support.


[1]  T.W.  Lee,  Mechanical and Chemical Decapsulation, Microelectronic Failure Analysis, Desk Reference, 3rd Edition.


[2]  T. Hazeldine, K. Duong, “Microsurgery for Microchips”, Advanced Packaging, December 2003.


[3]  S. Perungulam, K.S. Wills, “Chip Access Techniques”, Microelectronics Failure Analysis Desk Reference Fifth  Edition, ASM International, 312-322(2004).


[4] P. Schwindenhammer, P. Poirier, P. Descamps, “Microelectronics Failure Analysis using Laser Ablation of  Composite Materials in System in Package”, 2006 Electronics  Packaging Technology Conference.


[5] D. Thomasi, “Plasma Decapsulation Techniques”, Microelectronics Failure Analysis, Desk Reference, 3rd  Edition.


Appendix A


Partial List of Equipment and Materials Used for This  Procedure


Material   Vendor


Name/Part. No.


Experimental


In the present study, four wafers with high and low F at% contamination were prepared by tuning the Al bondpad  opening process. The contamination level (C and F) on the Al  pads of the wafers was measured using Auger technique. The  wafers were subsequently subjected to the simulation tests  using a reliability test oven with a controlling function of  relatively higher temperature and humidity (RH %). Two  experiments were conducted by changing the operating  conditions of the oven. In table-1 the F contamination of the  four wafers are listed along with the conditions of temperature (T) and relative humidity (RH %) used during the SLAT  simulation.


Table-1: Auger analysis results on the surface of Al Bondpads  of the four wafers and SLAT experimental conditions


Surface F at% Contamination


(Auger Measurement)


SLAT  Conditions


used


Wafer-1


14.0 at%


High T + Low RH %


Wafer-2


<1.0 at% (detection limit)


Wafer-3


9.0 at%


Low T + High RH %


Wafer-4


2.2 at%


In this section we will present two case studies where we were  able to successfully simulate F-induced corrosion defects  using the SLAT simulation. We have established through our  previous studies that humidity is not only a key parameter in  the reaction mechanism of Fluorine-induced Al pad corrosion, as highlighted in the previous section, it also influences the  physical characteristics of corrosion-defects on the Al pad, namely, their morphology (shape and size of the defects) [3,4]. The shape and size are also dependent on F contamination


level and environmental factors such as moisture or humidity  and temperature. Our simulation results showed that: (i) At  conditions of relatively higher T and lower RH %, the “crystal-like” defects were formed; (ii) At conditions of  relatively lower T and higher RH %, the “oxide-like” defects  were formed.


Relatively Higher T + Lower RH %


In our previous studies, one of the failure modes responsible  for NSOP is the formation of the “crystal-like” defects on the  Al pad due to F-induced corrosion. These defects are  enhanced by the presence of moisture. As the name suggests, these defects have faceted surfaces. For example, Fig. 2 shows  the “crystal-like” defects, which were found after wafer  storage at the assembly house.


For this kind of defects, the physical dimension is typically in  the nanometer range and are, therefore, visible only in high  magnification SEM images (> x25k). In the SEM image in Fig  2, one can clearly see that all the defects have well-faceted  surfaces and are of different sizes (~60-220 nm) [3-4].


Figure 2: Surface SEM image of Al pad with the “crystallike” defects. SEM image was taken at high magnification and  the defects are characterized by faceted surfaces.


In the first experiment, simulation test was done using  relatively higher T and lower RH %. Two wafers were  processed with different initial F-contamination level on the  bondpads, referred to as high- and low- F at%. The Fcontamination level was confirmed using Auger technique, which are listed in Table 1. Both the wafers were then  subjected to the SLAT test in an oven under relatively higher  T and lower  RH % conditions.


SEM imaging was performed on the two wafers after the  simulation test as shown in the Fig. 3. The results of high- F  at% wafer (Fig 3(A)) are interesting as they are similar to the  real “crystal-like” defects shown in Fig 2. On the other hand, for the low-F at% wafer, no defects were observed after the  simulation test as shown in Fig. 3(B).


However, the size of the simulated defects (Fig. 3(A)) is much  smaller than those of the real defects (Fig. 2). This is possibly  related to simulation and real scenario not being exactly  identical conditions. It is also likely that defects may further


grow  exper


Figur conta(B) – high-F under


From forma F at%(iii) H as we to the one m where N2 ca(O2).


As indicated earlier, the devices were rinsed with DI water  followed by acetone.  Although it had been theorized that the  copper areas were being passivated with sulfur from one  component of the acid mix chemistry, empirical data of this  had not yet been collected.  To confirm this theory, additional  devices were decapsulated with the laser/acid mix, but were  not rinsed.  Analysis of the exposed copper bond wires with  Energy Dispersive Spectroscopy (EDS) and X-ray  Photoelectron Spectroscopy (XPS) indicated the presence of  copper sulfide and cupric oxide which passivated the wires to  protect them from degradation during the acid decapsulation  process.  It was also found that an immediate (DI) water rinse  of the decapsulated device would dissolve these residual  copper sulfides since these sulfides were soluble in DI as  opposed to acetone or isopropanol (Figure 8).


Figure 8.  Optical micrograph of laser ablated and acid  decapsulated TI device without rinse showing  extent of copper sulfide formation on the copper  wires.


Figure 9.  XPS spectrum of laser ablated and acid


decapsulated copper wires without rinse showing  the presence of copper sulfide formation.


A combination of laser ablation and acid mix can be a very  effective decapsulation method for plastic encapsulated  devices bonded with copper wire.  The experimentation  performed clearly showed that with the appropriate acid mix  ratio and rinse chemistry, minimal corrosion of the copper  wire will occur without any evidence of damage to the die  circuitry due to the formation of copper sulfides on the  exposed copper.  Additionally, with extended mold compound  baking, the resulting cross linking of the mold compound  chemistry reduces the effectiveness of this etch process.  By  first ablating the mold compound to near the die surface and  then applying the acid mix etch, the decapsulation time will be  dramatically reduced, thereby eliminating the risk of copper  corrosion.


Special thanks to Lucas Copeland for his excellent lab work  and technical assistance in completing this project.


[1]  Murali, S., Srikanth, N., “Acid Decapsulation of Epoxy  Molded IC Packages with Copper Wire Bonds”, IEEE  Transactions on Electronics Packaging Manufacturing, Vol  29, No. 3, July 2006.


# Photoluminescence and EBIC for Process Control and Failure Analysis in Si-Based Photovoltaics


Photoluminescence and EBIC for Process Control and Failure Analysis  in Si-Based Photovoltaics


Martin Kittler, Tzanimir Arguirov, Reiner Schmid, Winfried Seifert


IHP, Im Technologiepark 25, 15236 Frankfurt (Oder), Germany


kittler@ihp-microelectronics.com; phone: +49(0)335-5625130


Joint Lab IHP / BTU Cottbus, Konrad-Wachsmann-Allee 1, 03046 Cottbus, Germany


Teimuraz Mchedlidze


Crystalline silicon used for fabrication of solar cells, such as  multicrystalline silicon (mc-Si), contains a high density of  extended crystal defects. Since grain boundaries and  dislocations restrict the solar cell efficiency, characterization  of the defect properties is essential to upgrade the quality of  the wafers, to control the defect influence on the cell  fabrication process and to understand the defect influence on  the solar cell performance.


Since mc-Si wafers exhibit an inhomogeneous defect  distribution, there is a need to combine the spectral capabilities  with the ability of spatially resolving the defect areas. In this  paper we report application of luminescence and electronbeam-induced current (EBIC) techniques for characterization  of defects in solar Si.


Results about multicrystalline Si produced by block casting, see [1], are reported in detail. In addition, observations for  ribbons made by the technique of edge-defined film fed growth (EFG), see [1], and for crystalline Si thin films on glass, see


[2], are also shown.


In the first part luminescence features of defective Si will be  introduced, followed by discussion of application examples. The second part starts with explanation of the EBIC technique, including details about the temperature dependence of the  EBIC defect contrast c(T). Then application examples of the  c(T) behaviour and the analysis of the ‘interaction’ of grain  boundaries with p-n junctions will be discussed.


Photoluminescence


Luminescence of crystalline Si containing crystal defects


Si is an indirect semiconductor material. Nevertheless, a  radiative band-to-band (BB) transition appears which is  assisted by transversal optical (TO) phonons for momentum  conservation. Fig. 1 shows a typical PL spectrum of dislocated


Si. In addition to the BB line a quartet of the dislocationrelated lines, D1-D4, becomes visible, e.g. [3].


The intensity of the BB line in Si is strongly reduced by nonradiative recombination, i.e. it depends on the Shockley-ReadHall lifetime τSRH. Fig. 2 shows the BB efficiency of Si at 300  K calculated as a function of excess carrier density Δn with τSRH as a parameter [4]. Accordingly, for perfect Si the room  temperature efficiency of the BB line might be larger than  20%. Because crystal defects lower the lifetime they decrease  the BB intensity.


Figure 1: PL spectrum of dislocated Si, measured at 80 K, showing the dislocation lines, D1-D4, and the BB line.


The D line intensity is found to decrease with increasing  temperature. At room temperature only BB and D1 lines can  be observed in defective Si, see Fig. 3.


Electroluminescence of forward biased solar cells, emitting  BB light, is widely used to study the defect distribution in fully  processed solar cells. For mc-Si wafers without p-n junction  instead of EL imaging mapping of the BB light by PL can be  used. Then surface recombination and a longer data  acquisition time are limiting factors. Here we report on a novel  rapid PL imaging technique, for direct observation of D1  radiation in a non-passivated mc-Si wafer providing spatially  resolved images at room temperature [5]. For this technique


we use high injection of excess charge carriers. Rapid BB  imaging is also possible by this new method.


Figure 2: Calculated efficiency of BB line of Si at 300 K as a  function of excess carrier density [cm-3], with Shockley-ReadHall lifetime as parameter.


Figure 3: Spectrum of a mc-Si sample exhibiting BB and D1  lines at room temperature.


PL imaging of defect distribution in mc-Si


In Fig. 4a a D1 image of a 5 x 5 cm2 piece of a non-passivated  mc-Si wafer is shown, which was taken in 5 sec at 300 K. The  spatial resolution is around 130 m. Standard D1 mapping at  300 K yields a similar image (not shown here) but needs a  much longer recording time of about 13 hours. Fig. 4b shows  an enlarged section of Fig. 4a but imaged with BB light. The  dark extended lines, which are visible in the BB image, are  caused most likely by surface damage due to wafer-cutting. In  the D1 image these lines are no longer observed and do not  show any noticeable disturbing effect on the defect-related  radiation. Accordingly, the novel technique which eliminates  surface artifacts can be used as a tool for fast in-line detection  of crystal defects in mc-Si.


The dark defect contrast in the BB images appears because the  lifetime at the defect sites is smaller. Accordingly, the BB light  intensity/efficiency is lowered by the defects, see Fig. 2. However, also other features caused by lifetime variation  become visible in the BB images. Surface artifacts caused by  wafer cutting appear as dark lines, see Fig. 4b. The advantage


of the D1 mapping, where the defects appear as bright  contrasts, is that only the defects are imaged, whereas artifacts  visible in the BB image are eliminated.


Figure 4: Photoluminescence images of a 5 x 5 cm2 piece of a  non-passivated mc-Si wafer taken at 300 K with a novel  imaging technique, showing (a) D1 and (b) BB luminescence  images of the same sample area at 300 K. Spatial resolution is  around 130 m for the large and 60 μm for the small images.


The novel rapid D1 imaging technique can be applied at  different stages of the solar cell process, starting from asgrown wafers till processed solar cells. Because it does not  need a special surface treatment, e.g. passivation, and because  it is resistant against thin layers on top of the wafer surface, it  is a candidate for inline quality control. For further details see


As an example Fig. 5 compares a BB and a D1 image of a full  15 x 15 cm2 wafer after phosphorus diffusion for p-n junction  formation, covered with an inhomogeneous phosphor silicate  glass layer. No noticeable effect of the layer is found on the  D1 image, in contrast to the BB image, which is obscured by a  multitude of white dots and large white blurry areas.


Figure 5: BB (top) and a D1 (bottom) image of a full 15 x 15  cm2 wafer covered with an inhomogeneous phosphor silicate  glass layer. Note the full wafer image is assembled from subimages.


Comparison of BB and D1 luminescence in EFG Si


During growth of about 300 μm thick Si ribbons using the  EFG technique (see e.g. [1]) grain boundaries are formed  parallel to the growth direction. A part of the grains in EFG-Si   contains a high dislocation density. Fig. 6 shows profiles taken  at 300 K perpendicular to the EFG growth direction. It is  found that D1-line intensity can be observed within the  defective regions (Fig. 6a). The BB line intensity shows the  opposite behaviour, i.e. it gets smaller in the defective regions (Fig. 6b). Moreover, BB intensity and minority-carrier  diffusion length / lifetime correlate with the BB intensity,


which is expected according to Fig. 2. The observations for  EFG Si are in complete analogy with results found for the  block-cast Si, shown above. Accordingly, anti-correlation of  BB and D1 intensity exhibit a general behaviour for different  types of solar Si.


Figure 6: Profiles measured at room temperature  perpendicular to the growth direction of an EFG ribbon, taken (a) with D1-line and (b) with BB line, Ibb. The profile of  the minority-carrier diffusion length, L, is also included in (b) by open symbols.


Correlation of D1 luminescence with open circuit voltage  in Si thin film solar cells


An application of the D1 emission is demonstrated for thin Si  solar cells on glass made by CSG Solar AG, see [2]. The  micro-crystalline Si layer, in which the solar cell was  fabricated, is about 1.5 μm thick and exhibits a defect density  around 10E9 cm-2. The layer emits at room temperature strong  D1-like light. The data obtained using PL were compared to  the performance of different solar cells. The intensity of the  D1 line was shown to deliver information about non-radiative  recombination [7]. In Fig. 7 a correlation of the open circuit  voltage (VOC), measured at the solar cells, and the intensity of  D1 line is presented.  The data could be fitted with a line in the  semi-logarithmic scale, suggesting that D1 intensity correlates  with the minority-carrier diffusion length (lifetime) in the  structure.


Vice versa, D1 intensity measured by PL allows prediction of  the important solar cell parameter VOC. Accordingly, PL can  be used as a tool for process control predicting solar cell  parameters in the Si thin film technology.


Figure 7: Correlation observed between open circuit voltage  values (VOC) of Si thin film solar cells normalized on a  maximal value for various illumination conditions and  intensity of the D1 line. All data are measured at room  temperature.


We have shown that PL is a powerful tool for non-destructive  characterization of solar Si, exhibiting potential for in-line  defect detection and process control. It allows defect imaging  using the BB or the D1 line. The latter one has the advantage  that artifacts are eliminated. As a consequence D1 imaging can  be applied at different stages of the solar cell process. Moreover, it was found that the intensity of the D1 emission  correlates with the open circuit voltage of solar cells, at least  for crystalline Si thin films on glass.


EBIC Technique


Application of the technique of the electron-beam-induced  current (EBIC) to Si allows defect analysis with μm resolution. Accordingly, it might be used as a suitable tool for failure  analysis in photovoltaics, e.g. [8]. The principle of EBIC  operation is very similar to the basic process known for solar  cells. For EBIC the excess electron-hole pairs are generated by  a focused electron probe with beam energies up to 30-40 keV, instead of light in case of a solar cell. The excess carriers  interact with a p-n or Schottky junction and the resulting short  circuit current is used as a signal. By scanning of the electron  probe an EBIC map is formed. Recombinative-active crystal  defects appear as dark contrasts because they lower the EBIC  signal. On the other hand, the regions of p-n junctions appear  bright because the carrier drift within the depletion layer  prevents recombination losses.


EBIC imaging of p-n junctions in mc-Si solar cells


Examples demonstrating that EBIC is well suited for failure  analysis in photovoltaics are shown in Figs. 8 and 9. In Fig. 8  the ‘interaction’ of a grain boundary with the p-n junction is  shown. The spike at the p-n junction, which degrades the cell  characteristics, is caused by enhanced diffusion of phosphorus  at the grain boundary during the junction formation. Moreover, EBIC allows one to explain other defect behaviour which may


degrade/affect the solar cell performance, such as existence of  potential barriers at grain boundaries or the presence of    enhanced transport of minority-carriers along grain  boundaries, for details see e.g. [9].


Figure 8: EBIC micrograph of a beveled mc-Si sample  containing a p-n junction formed by phosphorus diffusion of  the emitter into p-type substrate. The spike at the junction - increased junction depth at the grain boundary - is due to  enhanced phosphorus diffusion during junction fabrication. Note, the image of the beveled surface is enlarged (the  junction depth is around 1 μm).


In Fig. 9 a much more dramatic situation is presented. The p-n  junction becomes visible as a bumpy line and at two locations  the spikes caused by grain boundaries exceed the junction  depth by a factor of about 5 or even more.


Figure 9: EBIC micrograph of a beveled sample exhibiting a  p-n junction of a solar cell made from mc-Si. The junction  shows an extremely inhomogeneous shape.


Temperature dependence of EBIC defect contrast c(T)


The recombination behaviour of extended crystal defects in Si  as measured by EBIC is found to depend on sample  temperature T and injection level/beam current, see e.g. [10] and references therein. The T dependence of the EBIC contrast  c(T) analyzed under low injection conditions is mainly  applied. At the first glance c(T) yields information whether  deep or shallow levels dominate the recombination activity of  the defects, e.g. [11]. Fig. 10a shows two different c(T) behaviour of dislocations in Si, denoted type-1 and type-2, respectively. Fig. 10b shows the SRH lifetime calculated as a


function of T for deep and shallow levels, 0.5 eV or 0.08 eV, respectively, above the valence band. Taking into account that  the contrast, c, is inversely proportional to the lifetime at the  defect, τdefect, the type-1 behaviour in Fig. 10a can be related to  deep levels whereas type-2 behaviour appears when shallow  levels dominate the defect recombination.


Figure 10: Temperature behaviour of EBIC contrast c(T) and  of lifetime τ(T).


(a_top) Experimental c(T) data measured for dislocated Si  before (type-1) and after (type-2) phosphorus diffusion  gettering. The solid lines are calculated using the model  described in [12] yielding impurity concentrations, NM , at the  dislocations of  2 x 107 cm-1 and 3 x 105 cm-1, respectively.


(b_bottom) Normalized SRH-lifetime τ calculated as a  function of temperature T under low-injection conditions. Parameter is the trap position above the valence band.


Dislocations in Si are known to be connected with shallow  levels, about 80 meV from the band edges, which are formed  by the elastic strain field around the dislocations, e.g. [12]. The deep levels at dislocations in Si are caused by kinks, jogs  but are mainly formed by impurities/metal atoms which are  accommodated at the dislocations, e.g. [13]. A model taking  into account the recombination paths formed by the shallow  and deep recombination levels at the dislocations [12] allows  to extract  the density of deep levels/metal impurities, NM,


from the EBIC c(T) behaviour. Fig. 11 shows the c(T) behaviour calculated with NM as parameter.


Note that the EBIC c(T) behaviour is extremely sensitive to  defect contamination. For example NM = 10E6 per cm  dislocation length, at which room temperature contrast in  EBIC is clearly visible already, means that only 100  impurity/metal atom per μm dislocation length are needed to  create this visibility. Routine techniques of analytical electron  microscopy do not reach such sensitivity.


Type-1 behaviour in Fig. 10a was measured for dislocations in  Si before thermal treatment. Fitting the experimental data by  the defect recombination model yields a contamination density   NM = 2 x 107 cm-1. Phosphorus diffusion during p-n junction  formation - which supplementary provides an external getter  sink creating the so called phosphorus diffusion gettering (PDG) - changes the defect c(T) behaviour completely, see  type-2 in Fig. 10a. Fitting the experimental data yields NM = 3  x 105 cm-1. Accordingly, PDG during p-n junction formation  cleans the dislocations and reduces the contamination level by  about two orders of magnitude. As a consequence, the solar  cell performance is improved. This example clearly  demonstrates that EBIC is a powerful technique for in-depth  analysis of the recombination behaviour of defects which helps  to understand changes occurring during the cell process.


Figure 11: EBIC contrast behaviour c(T) for different  concentrations NM from 0 to 108 cm-1 of deep level impurities  at the dislocation, calculated by the model described in [12].


Finally, we report an example where EBIC allows detection of   process contamination. Fig. 12 shows EBIC micrographs taken  at 300 K from two adjacent wafers. Circular Al Schottky  contacts of about 5 mm diameter and 100 nm thickness were  evaporated on the p-type Si wafers to allow EBIC imaging. In  the as-grown state, shown on top, the contrasts are very weak. Weak contrasts at 300 K point to a small defect contamination (compare Fig. 11). On the contrary, the EBIC image of the  parallel wafer - which was etched in KOH - exhibits strong  defect contrasts. Strong contrasts at 300 K point to a


type-1


type-2


considerable increase of defect contamination (see Fig. 11). Accordingly, we could observe appearance of defect  contamination by using simple EBIC imaging. We expect that  the observed defect contamination was caused by an impure  KOH etch.


Figure 12: EBIC micrographs of p-type solar Si taken at 300  K. The circular areas represent Al Schottky contacts of about  5 mm diameter prepared by Al evaporation. The upper image  shows only very weak contrast in the as-grown material. The  lower image exhibits strong contrasts caused by defect  contamination due to  etching in impure KOH.


The EBIC technique was demonstrated to display  inhomogenities of p-n junctions formed by crystal defects / grain boundaries during phosphorus diffusion. It was shown  that the temperature dependence of the EBIC defect contrast  c(T) reflects the defect contamination in a sensitive manner. Cleaning of the defects by phosphorus diffusion gettering  and  contamination of defects due to impure KOH etch are shown  as examples.


Summary and Conclusions


We have demonstrated the potential of luminescence for nondestructive characterization of Si wafers and solar cells in  terms of in-line defect detection and process control. The  information contained in the defect-related D1 line appears to  be more powerful than the information which can be extracted  from the Si BB light, which is widely used for this purpose at  present.


EBIC is a suitable tool for failure analysis of Si solar material  and cells. It delivers detailed information about crystal defects  with μm resolution regarding the level of defect  contamination, the influence of defects during the formation of  p-n junctions. Moreover, the existence of potential barriers and  the transport of charge carriers along defects/grain boundaries  can be analyzed by EBIC.


[1] H.J. Möller, Semiconductors for Solar Cells, Artec House  Inc. (Norwood, MA 02062, 1993).


[2] homepage CSG solar company: http://www.csgsolar.com


[3]  N.A. Drozdov, A.A. Patrin, V. D. Tkachev, Pis’ma Zh. Exp. Theor. Fys., 23, 651 (1976).


[4]   M. Kittler, T. Arguirov, A. Fischer, W. Seifert, Optical


Materials 27, 967 (2005).


[5]   R.P. Schmid, D. Mankovics, T. Arguirov, T. Mchedlidze, M. Ratzke, M. Kittler, Physica Status Solidi A (Wiley  Interscience), submitted.


[6]   R.P. Schmid, D. Mankovics, T. Arguirov, T. Mchedlidze,   M. Kittler, “Novel imaging techniques for dislocation related D1-photo-luminescence of multicrystalline Si


wafers – two different approaches”, 10th Int. Workshop


on Beam Injection Assessment of Microstructures in


Semiconductors - BIAMS 2010, Halle, Germany, July


2010, oral presentation, submitted to Physica Status


Solidi C.


[7]   T. Mchedlidze, J. Schneider, T. Arguirov, M. Kittler,


“Characterization of crystalline silicon on glass using


photoluminescence”, 10th Int. Workshop on Beam


Injection Assessment of Microstructures in


[8]    O. Breitenstein, J. Bauer, T. Arguirov, M. Kittler, W.


Seifert, Scanning 30, 331 (2008).


[9]    M. Kittler, M. Reiche, W. Seifert, X. Yu, T. Arguirov,


O.F. Vyvenko, T. Mchedlidze, T. Wilhelm, ECS


Transactions 3 (4), 429 (2006).


[10]  D.B. Holt, Scanning Microscopy 10 (4), 1047 (1996).


[11]  M. Kittler, W. Seifert, Scanning 15, 316 (1993).


[12]  V. Kveder, M. Kittler, W. Schröter, Phys. Rev. B 63,


115208 (2001).


[13]  M. Kittler, C. Ulhaq-Bouillet, V. Higgs, J. Appl. Phys.


78, 4573 (1995).


# Combined electron beam induced current imaging (EBIC) and focused ion beam (FIB) techniques for thin film solar cell characterization


Combined electron beam induced current imaging (EBIC) and focused ion beam (FIB) techniques for thin film solar cell characterization


Frank Altmann, Jan Schischka


Fraunhofer Institute for Mechanics of Materials, Halle, German Frank.Altmann@iwmh.fraunhofer.de; Jan.Schischka@iwmh.fraunh


Vinh Van Ngo, Stacey Stone


FEI Company, Hillsboro, Oregon USA   Vinh.Ngo@fei.com; Stacey.Stone@fei.com


Laurens F. Tz. Kwakman


FEI France, SAS., Lyon, France  Laurens.Kwakman@fei.com


Ralf Lehmann


FEI Deutschland GmbH, Frankfurt Main, Germany  Ralf.Lehmann@fei.com


y


ofer.de


A novel analytical method applying combined electron beam  induced current (EBIC) imaging  based on scanning electron  microscopy (SEM) and focused ion beam (FIB) cross  sectioning in a SEM/FIB dualbeam system is presented. The  method is demonstrated in several case studies for process  characterization and failure analysis of thin film technology  based Solar cells, including Silicon (CSG), Cadmium  Telluride (CdTe) and Copper Indium Selenide (CIS) absorbers. While existing techniques such as electro-, photoluminescence spectroscopy and lock-in thermography  are able to locate the larger, electrically active defects  reasonably fast on a large area, the FIB-SEM EBIC system is  uniquely capable of detecting sub-micron, sub-surface defects  and of analysing these defects in the same system. In  combination with a FIB, the localized region of interest can be  easily cross sectioned and additional EBIC analysis can be  applied for a three dimensional analysis of the p/n junction.


Thin film technology for solar cell fabrication is a promising  alternative to wafer based technologies in terms of  manufacturing cost and scaleability. A variety of technologies  applying amorphous or crystalline silicon, CdTe or CIS/CIGS  absorbers are already being for industrial production. For  large-area devices required for realistic applications, thin-film  device fabrication becomes complex and requires proper  control over the entire production process. Profound  understanding of manufacturing processes and their impact to  the microstructure and local electrical properties can help to  improve the efficiency of thin-film solar cell devices. Advanced PV defect diagnostics comprise methods for defect  localization, preparation methods and marking for tracking  down defect structures to their root causes in the  microstructure. A particular challenge is the correlation of


device yield to local electric properties on a micrometer scale  for a better understanding of defect mechanisms, material and  process-induced origins. In production lines, defects do not  only affect a single cell or device but can affect the output of  the entire line as a result of systematic process or feedstock  issues. Therefore, a near-line tool for process inspection and  defect analysis provides significant values.


Electron beam induced current (EBIC) imaging  is able to  identify the locations of electrical active defects for detailed  examination or further microanalysis using a Focused Ion  Beam (FIB) on the same system. The following three thin film  technologies were chosen for several case studies  demonstrating the application of EBIC/FIB method.


UV spot source Dymax


38905


Maskant


Dymax


BT-730


Rigid adhesive


726


De-flasher


Dynaloy


Dynasolve CU-7


18 gauge  dispensing  needles


Ellsworth  adhesives


EA18FTH1/2


# Low Temperature Plasma Decapsulation of Copper-wire-bonded and Exposed Copper Metallization Devices


Low Temperature Plasma Decapsulation of Copper-wire-bonded  and Exposed Copper Metallization Devices


Texas Instruments, Tucson Device Analysis Operations Laboratory   5411 E. Williams Blvd, Tucson, Arizona 85711 USA


kstaller@ti.com


One method of reducing costs in the packaging sector is to  switch from gold bond wires to copper.  Gold wires provide  excellent reliability and withstand the chemicals used to  decapsulate microelectronic packages for qualification and  failure analysis inspections.  Copper wires, however, are  susceptible to corrosive attack from many of the decapsulation  acids.  Thicker copper wires (over 2 mils) can be safely  decapsulated using a ratio mixture of fuming acids.  Some  surface etching of the copper will occur, but the wire will  remain electrically viable.  Very thin wires (less than 1 mil) cannot be decapsulated reliably without the risk of etchthrough, especially on one-of-a-kind field returns.  Microwave  Plasma can provide a safer alternative for decapsulating  packages with copper bondwires and exposed copper  metallization.


Plastic package decapsulation requires the use of fuming  sulfuric and fuming nitric acids to break down and dissolve  the polymeric compounds in the encapsulation.  Fuming nitric  acid is the primary choice for decapsulation purposes.  It  dissolves the encapsulation rapidly and removes die coat  materials without etching the gold bondwires or aluminum  bondpad metallization.  Typical process temperatures range  from 70°C to 90°C.  Copper is readily consumed in the  presence of nitric acid and any exposed copper wire  interconnects or metallization on top of the passivation will be  rapidly consumed by the nitric acid.


Fuming sulfuric acid is the other option for decapsulation.  It  is used at higher process temperatures (150°C to 300°C) and  takes longer to dissolve the encapsulation.  It is usually more  effective on harder thermoplastic resins that are impervious to  etching from nitric acid.  While it does not etch or attack  copper metallization, it does etch and dissolve exposed  aluminum metallization.


Either acid when used alone is not optimal for decapsulating  devices with copper metallization and aluminum bondpad  structures.  When fuming nitric and fuming sulfuric acids are  used in a mixed ratio at low temperatures (<70°C), moderately  safe decapsulation of copper metal devices can take place.  Some scavenging of the copper metal will take place and a


protective film of copper sulfate will develop on the copper  surfaces which inhibit further etching from the nitric  component (Figure 1).


Ratio fuming acid mixtures have been found to safely expose  2 mil (and larger) bond wires and exposed copper  metallization on top of the passivation layer.  The residual  copper sulfate crystals on the copper structures require  additional chemical clean-up to expose the bare metal.  Any  copper shavings, filaments, or fine shorting defects are often  lost when using fuming acid decapsulation, resulting in failure  modes clearing upon decap.  1 mil copper bond wires, especially those in the package corners that have been  exposed to temperature cycling also tend to fall apart during  fuming acid decapsulation.


Figure 1: Copper sulfate crystals form on copper wires during  decapsulation using a mixture of fuming nitric and fuming  sulfuric.  This coating slightly etches the copper during its  formation, but then inhibits any further corrosion during the  decapsulation process.


One other detrimental effect of acid decapsulation is that it  will attack and deplete circuit board substrates on surface  mount packages, leaving the glass weave filler swollen and  saturated with acid residue and corrosion byproducts that will  continue to leech out and attack exposed copper metal (figure  2).


Figure 2: PWB substrate resin attack from fuming acids.  Residual acid material remains in the FR4 glass weave  strands and can continue to corrode exposed metal surfaces in  a decapsulated device.


Decapsulation Without Fuming Acids


Other methods of decapsulation that do not use fuming acids  are mechanical milling and laser ablation.  Mechanical milling  and polishing can be used to partially open a cavity in devices, but cannot fully expose the die surface without risking  damage to the passivation and bondwires.  It is a blind process  and requires patient, gradual increments of material removal  until the tops of the bondwires are exposed.  Milling too far  can remove some of the bondwire loop material, leaving the  wires mechanically compromised.


Laser ablation is a method that uses a 1064 nm NdYAG laser  beam to melt and eject encapsulation material from a predefined cavity pattern.  The primary advantage of laser  ablation is that the progress can be visually monitored and it  leaves the package metal structures and magnet wire coatings  in microelectronics intact.  Some slight surface pocking takes  place, but leaves the internal interconnects mechanically  sound.  Laser ablation cannot safely expose the die surface  without risk of catastrophic circuit damage.  Some glass  sphere filler material has been found to pass the laser energy  and damage the die surface, even with a thin layer of  encapsulation remaining over the die surface.  In order to  avoid damage to the die, it is often best to stop the ablation  process at a point between the top of the bondwires and top of  the ball bonds (Figure 3).  The laser also tends to ablate in an  isotropic manner, leaving encapsulation material under the  exposed bondwires.


Either method requires a finishing decapsulation step in order  to clear material out from under the bondwires and to safely  expose the die surface.


Figure 3: Laser ablated BGA package with copper wires.  The  ablation process was run until the top of the bondwires were  exposed (left side top of package, right side BGA bottom of  package).  At this point, a finishing step needs to be performed  to expose the die surface.


Plasma Decapsulation


Plasma decapsulation is a logical process step that can be used  to complete the laser ablation or milling decapsulation  process.  The plastic encapsulation is ashed away by  combustion.  Oxygen (O2) is used to convert the organic  hydrocarbons to CO2 and H2O in the same way we combust  gasoline to CO2 and H2O in our cars. The combustion process  is at a relatively much lower temperatures in a plasma system  since a high temperature spark (equilibrium plasma) is not  used to activate the oxygen (spark plug) but instead by  electron collision in the electric field.  Use of oxygen-only for  decapsulation is a very slow process due to the stability of the  epoxy resin and the relatively low concentration of O radicals. The ash rate is greatly accelerated by introducing activated  fluorine (CF4 or SF6). The presence of O2 in CF4 plasma  assists in the decomposition of O2 and CF4 and the  hydrocarbon surface of the plastic package. Mixtures of  approximately 20% CF4 in O2 are optimum for ash rates. These are chemical anisotropic etching processes.  Etchant  species are most likely O, CF2, CF3 CF and F species. Reaction mechanisms are quite complex and involve fluorine  induced radical formation of surface hydrocarbons (HF  byproduct) and hydrocarbon oxidation to form volatiles CO2  and H2O.[2]


Current RIE and ICP plasma systems are not well suited for  decapsulation.  Both technologies run at a process frequency  of 13.56 MHz (High Frequency – HF) and have a process  temperature that is above the reflow temperature of tin-lead  solder.  Etch rates for plastic or epoxy encapsulation can be  very long on 100-300 watt systems (several hours).  Microcircuit passivation will often etch within a few minutes  of exposure, leading to exposed upper level metallization  and/or damaged silicon-level structures.  Bake-recoverable  mechanisms can also heal when decapsulated in HF plasma, due to the high temperature and solder-related defects will  reflow and be altered.


Microwave plasma, on the other hand, is well suited for  finishing decapsulation.  It uses the same chemistry of the RIE  and ICP systems (oxygen and CF4 or SF6).  Commercial  systems aimed at the microcircuit decapsulation market use  this technology and have been available since the late 1980s.  It operates at a process frequency of 2.45 GHz and has a low  process temperature that is below the reflow temperature of  tin-lead solder.  Successful analysis of cracked solder joints in  axial-leaded inductors and encapsulated 10-base-T hybrid  assemblies was being conducted in the mid 1990s[1] using this  technology, as well as circuit board failures due to internal  solder joint shorts in recent years (figure 4).


Figure 4: Microwave plasma deprocessed circuit board  containing solder shorts within the resin-coated-copper layer.  The plasma was able to safely ash away the resin without  reflowing the shorting solder flakes.


Microwave plasma has a slower etch rate on microcircuit  passivation when compared to RIE/ICP plasma. When the  passivation is exposed in microwave plasma, the die can be  processed for an additional 40 to 120 minutes of time before  the passivation is breached and the upper metallization is  exposed.  Plastic resin etching is anisotropic, safely removing  encapsulation material under bondwires (from laser ablation).   Immersion of the microcircuit within the raw microwave  plasma, however, can have detrimental effects.  The RF  energy present in microwave plasma will rapidly ablate and  sputter exposed metal surfaces in the plasma.  Gold leadframe  plating and gold bondwires will etch away rapidly in the  presence of microwave plasma.  The silicon will also absorb  the microwave energy and heat the device up to process  temperatures that are even higher than those experienced in  RIE/ICP plasma.  These effects are eliminated by the removal  of the RF energy from the plasma stream.


A metal cage with openings cut to the wavelength of the  microwave frequency is placed over the chamber platen, enclosing the samples.  The RF energy is blocked by this  cage, but the reactive plasma species are drawn in and around  the samples in the chamber (Figure 5).  This prevents energy  absorption (sample heating) and sputtering of metal surfaces.


Figure 5: Overview of the microwave decapsulation system.  The faraday cage is the key to lowering the process  temperature and preventing heat absorption and metallization  sputtering.


Typical processing times on laser-ablated/milled cavities (to  expose a clean die surface) range from 2 hours on older 300-watt microwave plasma systems, to 20 minutes on the newer  500-watt systems (Figure 6). Without a pre-ablated cavity, the  total process time to expose a die surface can take up to 8  hours.


Figure 6: Decapsulation of laser-ablated PBGA microcircuit  using downstream microwave plasma.  This takes about two  hours on an older 300-watt system, and less than 20 minutes  on the newer 500-watt systems.


While the microwave plasma is able to safely ash the plastic  encapsulation, it is hindered by the eventual build-up of ash  on the sample.  It is necessary to stop and service the devices  every 15 to 30 minutes, blowing off the ash build up with  pressurized air or nitrogen.


Upper Chamber


Faraday Cage


Sample Platen


Supply Gasses O2 and CF4 are fed into upper  chamber.


Microwave RF (2.54GHz) is  beamed into the upper  chamber, generating a plasma  reaction.


A faraday cage is placed over the sample


platen in the lower chamber.  It blocks all


RF from reaching the samples, allowing


only the ionic gasses to flow through.


Samples are placed on the grounded


platen.


The vacuum port at the bottom of the lower


chamber evacuates the ions and reaction


byproducts, pulling new ionic gasses from


the upper chamber.


In the late 1980’s the commercial decapsulation microwave  plasma systems came with an automated blow off system  consisting of in-chamber nozzles that would could be aimed at  the die area of the plastic package.  It was programmed to stop  the plasma process every 3 to 10 minutes, blow compressed  nitrogen gas through the nozzles from 1 to 30 seconds, and  resume the plasma process.  Up to six plastic encapsulated  DIP packages could be loaded in the chamber, run overnight, and be fully decapsulated and ready for analysis at the  beginning of the next days shift.


Silica filler material tended to become more densely packed in  the encapsulation during the 1990s to the point that the blow  off system was not effective enough to fully expose the die  surfaces automatically.  It became necessary to manually clear  off the ash and filler particles using compressed air with  alcohol in a detailers paint brush spray system every 20  minutes of operation.  Recent experiments on a newer 500-watt system found that the encapsulation could be successfully  ashed and removed from the die surface within 20 minutes  without the need for manual ash removal.


The microwave plasma is very efficient at ashing and  removing organic resin material from the samples placed in it.  In order to preserve the integrity of PWB substrates that are  integrated into some microcircuit packages, and to prevent  ashing and removal of the remainder of the plastic package, it  is necessary to mask off the areas of the package that needs to  be retained.  Aluminum tape with a butylene-rubber-basedadhesive was found to provide complete blocking of plasma  gasses and a service life of over 20 hours.  Not only can this  tape mask off and protect an individual microcircuit substrate  during decapsulation, it was found effective at shielding entire  hybrid PWB assemblies as well.  The electronic assembly can  be fully encased in a pouch of aluminum tape with only the  cavity area on the microcircuit of interest being exposed to the  plasma (Figure 7).


Figure 7: In order to preserve PWB substrates or other areas  of the microcircuit package, it is necessary to mask off those  areas using aluminum tape with butylene rubber adhesive.  Only the decapsulation cavity is exposed to the plasma.


Analysis of Copper Bond Wire Devices


Laser pre-ablation and plasma decapsulation was recently  performed on copper wire reliability units that incorporated 1-mil copper wires bonded onto aluminum bondpads, and a  second population which was bonded onto copper  metallization over the die passivation.  Units that were  decapsulated using an older 300-watt microwave plasma  system were found to take 120 to 180 minutes of total plasma  time, with 20 minute manual air/alcohol ash cleaning.  Units  that were decapsulated on a newer 500-watt microwave  plasma system were found to fully expose the die within 20 to  30 minutes with one manual ash cleaning service.


As expected, no etching of the copper was noted.  The  exposed copper wires were shiny and free of residues  normally present following chemical decapsulation (Figure 8).  Encapsulation material left under the bondwires from the laser  ablation process was anisotropically ashed away (Figure 9).


Figure 8: Plasma decapsulation of 1-mil copper bondwires on  aluminum bondpads.  No attack of the bondpads is evident  and the copper wire metal is as clean as when it was bonded.


Figure 9: FE-SEM inspection shows no corrosive attack of the  copper wire metal and clean removal of encapsulation left  under the wires from the laser ablation process..


Examination of the units that were bonded to copper over the  passivation found that the nickel plating over the die metal  was pristine and un-etched (Figure 10).  Typical acid  decapsulation of this technology often strips the nickel plating  and partially etches the surface copper metal (Figure 11).


Figure 10: Plasma decapsulation of 1-mil copper bondwires  on copper metal over the passivation.  The nickel plating layer  over the surface copper metal (silver color) is pristine and  intact.


Figure 11: Typical acid decapsulation removes the nickel  plating and partially etches the copper metal structures.  Any  anomalous shorting defect is often lost using this technique


Examination of the bondwires found that witness marks on the  stitch bonds were well preserved (Figure 12).  Analysis of  broken stitch bonds using plasma decapsulation should  maintain a clean surface that can be inspected for fracture  features.


Figure 12: Collet witness marks are clearly visible on the  stitch bond areas, along with some lifted material in the inner  radius of the compression zone.  Plasma decapsulation can  maintain the surface features of bondwire fractures to allow  for analysis and identification of the root cause.


Analysis of units containing 1 mil copper bond wires that had  been stressed to end-of-life conditions were found to have  wires which fell off during the fuming acid mixture  decapsulation process.  When those units were decapsulated  with microwave plasma, the corner wires remained intact.  FE-SEM inspection of those wires found that they contained  slip plane fractures (Figure 13) that would likely etch rapidly  in the presence of nitric acid and cause the wire to weaken  before the sulfate coating could be fully developed.  Analysis  of any future copper wire field return units with open circuit  conditions on the corner bondwires will require the use of  plasma decapsulation to safely identify the nature of the wire  break.


Figure 13: Corner copper bondwires which fall off during  acid decapsulation likely contain slip plane fractures like  those seen here on a unit that was decapsulated using  microwave plasma.


Experimental deprocessing of copper bond wire and copper  metallization using laser ablation and downstream microwave  plasma has found that 1 mil stressed wires can be safely  exposed and examined, showing slip plane fractures in the  corner wires.  Topside copper metallization remains intact, even the thin protective nickel plating.  Sensitive copper metal  structures on top of the passivation (such as antennas) will  remain electrically viable following decapsulation with  plasma, but are often lost and defective following acid  decapsulation.


Microwave plasma technology is over 25 years old, but is not  a widely known or utilized tool in package deconstruction.  It  makes an ideal companion to complete a laser ablation system.  Once an organization becomes acquainted with it, it becomes  an indispensable capability.


Special thanks are in order to the ITT A/CD Product Analysis  Lab and Medtronic Microelectronics Lab for utilizing  microwave plasma deprocessing in the workplace, allowing  me to grow and develop my knowledge in the field of sample  deconstruction.  Thanks are also in order to Dr Demetrius  Chysostomou PhD for his insights into the plasma chemistry  and to his company for developing and marketing the  microwave plasma systems that make safe decapsulation of  copper devices possible.  Al Zieba of Medtronic also deserves  honorable mention for his ability to modify, maintain and  improve the reliability of these microwave plasma systems.


[1] Work Experience, ITT Aerospace/Communications  Division, Product Assurance Laboratory, 1919 W. Cook  Rd, Fort Wayne, IN 46825


[2] Demetrius Chrysostomou PhD, Director of Technology  PVA Tepla America, 251 Corporate Terrace, Corona CA  92879


# Decapsulation of Copper Bonded Plastic Encapsulated Integrated Circuits Utilizing Laser Ablation and Mixed Acid Chemistry


Decapsulation of Copper Bonded Plastic Encapsulated Integrated Circuits  Utilizing Laser Ablation and Mixed Acid Chemistry


Jake E. Klein


Texas Instruments Inc., 5411 E. Williams Blvd Tucson, Arizona  85711 USA  Klein_jake@ti.com


Lucas Copeland


Texas Instruments Inc., 5411 E. Williams Blvd Tucson, Arizona  85711 USA  l-copeland@ti.com


By utilizing a NdYAG lamp pumped marking laser, along  with unique mixes of specific acids, reproducible  decapsulation of copper bonded devices without damage to  the bond wires, packaging material, or to the silicon die  circuitry itself can be achieved.  With the copper bond wires, die, or substrate exposed, typical failure analysis methodology  can then be applied to drive root cause failure analysis or  device characterization.


Copper wire is beginning to replace gold as the standard  electrical connection from the silicon die to the package  leadframe. The many positive attributes of this metal besides  the obvious cost savings are apparent, but the complications of  etching open plastic encapsulated devices bonded with copper  wire are anything but positive.   The decapsulation of devices  is a critical technique in both device failure analysis practices  as well as device characterizations.  The ability to expose the  die post-mold can allow for die imaging and measurements in  addition to the application of global isolation techniques such  as emission microscopy or liquid crystal analysis.  One issue  seen with standard acid etch chemistries is that depending on  the molding compound type and extent of cure, etch times can  be lengthy, lasting several minutes to reach the die surface[1].  During the etch process, while the mold compound is being  reactively etched, the copper wires are also being exposed to  the acids which can lead to their degradation.  In order to  shorten this etch time, the device can be first exposed to  ablation of the mold compound by a 1064 nm NdYAG lamp  pumped marking laser typically used to ablate molding  compound in specific patterns for labeling or marking the  device name and lot trace codes.  This same process can also  be used to remove more molding compound in any shape or  pattern allowing for subsequent die exposure.  The ablation  process physically removes the mold compound with the  intense concentration of heat from the laser.  Although this  process works very well on all different types of molding  compounds employed by semiconductor manufactures around


the world, the intense focused laser energy will result in  localized heating on the device circuitry once the molding  compound is removed.  This localized heating will cause  varying levels of melted metallization on the die depending on  the circuitry patterning.  Additionally, the 1064 nm  wavelength can damage transistors by injecting charge.  However, since both the laser ablation and the acid etch  techniques are so effective in decapsulation, the limitations of  each can be reduced by combining each technique in  decapsulation. Before the utilization of laser ablation for  decapsulation, multiple recipes for epoxy decapsulation of  copper bonded devices have been observed in multiple labs  across the world with varying success.  The primary recipes  utilize a mixture of nitric and sulfuric acids at various  temperatures in order to remove the epoxy.  However, one  mixture may work on one device type or molding compound  with limited corrosion of the copper bond wires, but may  severely lead to copper corrosion on another.  This varying  success is due to multiple factors which play a significant role  in the decapsulation process including extent of cross linking  in the epoxy chemistry, the extent and size of silica filler, rinse  chemistry after etch, and ultrasonic cleaning following etch.


In this experiment, our goals were to address a few significant  issues by first varying the acid mixture, acid temperatures, and  laser ablation settings if applicable, and then to characterize  the subsequent rinse steps which produced the best results in  terms of both the lack of copper wire degradation and quality  of mold compound removal.  A high volume device utilizing  Shinetsu KMC 3580HB molding compound and 2.0 mil  copper wire was chosen to be the test vehicle.  Two tiers of  experimentation were explored, one facilitating decapsulation  for exposure of the die circuitry and subsequent failure  analysis and global isolation, and the second to allow for  bonding characterization including stitch bond physical  evaluation, wire pull and bond shear.  Each tier also included  molded devices which were exposed to an extended cure  schedule of 21 days at 200°C which added to the overall


hardness of the mold compound material (see Figure 1).  In  each group, the devices were examined following  decapsulation with either acid chemistry alone or a  combination of laser ablation and mixed acid etch.  After  rinsing, the die and wires were rinsed with deionized (DI) water followed by acetone.


Figure 1.  Copper wire decapsulation experimentation plan  indicating two tier approach.


Following the experimentation, the appropriate mixed acid  ratio was found to produce the optimum results for this  material.  Although the etch time for the standard cure mold  compound with only acid decapsulation was acceptable, the  addition of laser ablation reduced the etch time almost by half.  Overall etch times were found to be 300 seconds for die  exposure with only acid, and approximately 180 seconds  utilizing laser ablation.  The surface of the 2 mil copper wire  appeared good, without significant pitting or corrosion (see  Figures 2-3).


Figure 2.  Optical micrograph of a representative standard


mold cure TI device post acid decapsulation only.


Figure 3.  FESEM micrograph of a representative standard


mold cure TI device post acid decapsulation only. Cross section of the device showed only minor pitting of the  surface copper film (Figure 4).  However, decapsulation of the  devices with extended mold cure at 200°C were quite  different.   On these devices, decap with the same acid mix  and etch parameters required 900 seconds to expose the die.  After this extensive exposure time, the copper wires and die  surface copper film showed severe corrosion and pitting (Figure 5).


Figure 4.  FESEM micrographs of a cross-section through a  representative standard mold cure TI device post  acid decapsulation showing only minor


Copper Wire Decapsulation Experimentation


Test Vehicle:  Texas Instruments Operational Amplifier  Device


Etch for Electrical FA


Etch for Wire Pull (Full  Decap)


Chemistry


Only


Laser Abl.


Optimize  Parameters


(Assume  Extended  Cure M/C)


Not an  option due  to known  overetch


(Assume  Extended  Cure Hard


M/C)


Acid Ratio


Ablate and


use


optimized  chemistry


recipe


Requires  Excessive


time


Etch die


with


acid/laser, then ablate stitch bond


areas


Temperature


Frequent  Package


side  blowout


Time


Characterization for each cell:


1. Optical Characterization


2. SEM Characterization


3. Bond pad X-section


4. Wire Pull/Ball Shear


5. Auger/XPS of bond wire


6. ATE (Electrical FA Cells only)


degradation of the plating above the surface  copper film.


Figure 5.  FESEM micrograph of an extended mold cure TI


device showing the copper film and copper wires  after 900 second acid decapsulation.


By using the combination of laser ablation followed by the  same acid etch chemistry, the etch times was reduced to 180  seconds and consequently, the copper wires and surface  copper film appeared nominal, showing little evidence of  corrosion.  Additionally, the unique capability of the laser  patterning by PC control provided for specific decapsulation  of stitch bond areas away from the die without the need for  acid.  The stitch bond areas of the package could be ablated  after the die exposure process and provided for wire pull and  ball shear to be collected.  The data on these laser  ablated/mixed acid etched devices indicated no degradation of  the bonding parameters with a wire pull mean of 45.7g and  ball shear mean of 157.5g.


Figure 6.  FESEM micrograph of an extended mold cure TI


device showing the copper film and copper wires  after 180 second laser/acid decapsulation.


Figure 7.  Optical micrograph of laser ablated and acid  decapsulated TI device showing exposed die and  stitch bonds.


Crystalline Silicon on Glass (CSG)


The CSG thin film technique used by CSG Solar is based on  the PECVD of thin silicon film on top of a module size  textured glass substrate. P and n doping is realized in-situ by  adding dopant gases during the PECVD process.


Figure 1: CSG cell structure


The amorphous Si layer is crystallized and annealed by  subsequent heat treatments and hydrogen passivated.. CSG’s


exclusive technology is in the way the cells are electrically  contacted. The p/n contacts are both made from the silicon  side through contacting holes which are created by etch drops  realized by inkjet printing techniques. The final structure is  shown in figure 1.


Copper Indium Selenide (CIS)


CiS solar cells made by Odersun are produced by creation of a  Copper-Indium-disulphide semiconductor on long reels of  Copper tape. This copper tape is not only used to form the CIS  semiconductor but also acts as the substrate and the carrier  material for the solar cell. The thin active cell layer is created  in three stages using “reel-to-reel” production process, see  figure 2. The first step is a wet electro-chemical deposition of  Indium to generate CuIn. This step is followed by a gaseous  sulfurization of the CuIn to convert part of this film into  CuInS2. Final steps consist of the deposition of a buffer layer  and a transparent conductive oxide (TCO) as front contact  material.


Figure 2 CIS  reel to reel technology


Cadmium Telluride (CdTe)


The CdTe thin film technique, see figure 3, is based on the  deposition of about 1um thick CdS/CdTe film on top of a  glass substrate which has already the final module size and  that is already coated with a transparent conductive oxide. Backside contacts are created via a metal sputtering process.


Figure 3: CdTe module structure


EBIC/FIB technique


EBIC fundamentals


The primary electron beam in a SEM can generate electronhole pairs within the beam's interaction volume in  semiconductor devices. The electron-hole pairs are separated  by the internal electrical field at the p/n- or Schottky junction, called the depletion zone. Electrons will drift to the n-side, and holes to the p-side. If the p- and n-sides are connected in a  circuit, the corresponding EBIC current can be measured  using a suitable current amplifier. The output of the amplifier  can be used as an input to the SEM imaging system  visualizing the EBIC current value related to the position of  the electron beam which is scanned over the sample, figure 4.


Figure 4 working principle of EBIC


Top-down EBIC analysis


EBIC can be performed top-down to the sample surface which   means that the p/n junction is perpendicular to the SEM  electron beam. As the interaction volume in top-down EBIC  extends into or across the p/n junction, the EBIC image will  contain contrast as a result from changes in the diffusion of  minority carriers. Defects in semiconductors, such as  dislocations, tend to strongly decrease the minority carrier  lifetime in their vicinity, resulting in high top-down EBIC  signal in defect-free areas and weak EBIC signals in areas  around defects.  If the p/n-junction or Schottky diode junction  is covered by a top layer that is of non-uniform thickness, which is the typical case for thin film solar cells, the actual  EBIC signal image also contains topography contrast that can  mask the forementioned EBIC defect information.


In figure 5, this situation is depicted. It is thus important to  realize that in order to penetrate sufficiently deep to reach the  p/n-junction depletion zone, a sufficiently high electron beam  energy has to be selected. Depending on layer thickness this  energy may need to be more than 10 keV.


Metal film


N- doped film


Depletion layer P-doped film


E-beam 2-10 KeV


Figure 5: Depending on top layer thickness and electron beam  energy, energetic electrons may arrive at the depletion zone or  not


The electron range depends on electron energy as well as on  mass, density and average Z of the material. For Silicon the  electron range is ~ 0.03 and 3 um for E = 1 and 15 KeV, respectively. But even at sufficiently high energies, the EBIC  signal strength will vary due to the topography of the top layer  as the electrons arriving at the junction vary in density and in  energy. Sample tilt may have also influence on the topography  effects in the EBIC image.


EBIC analysis at FIB cross sections


When performing EBIC analysis at cross sections, the beam  scans across the cut surface of the p/n or Schottky junction. If  the beam is near the depletion zone the EBIC signal is  increased due to more created electron hole pairs get  separated, generating an EBIC current. When the beam  sweeps away from the junction, less electrons or holes can  diffuse to the junction and the EBIC signal is diminished. Thus, the EBIC signal from cross sections is strongly related  to the diffusion length of minority carriers and the location of  the p/n junction. The EBIC analysis allows to identify the p/n  junction as it coincides with the peak of the EBIC signal.  To  be able to locate the p/n-junction within the layer structure of  a thin film solar cell it is necessary to overlay the EBIC signal  image with the regular SEM image. This is best realized if  both images can be recorded simultaneously to avoid shifts  between serial collected images.


In a FIB/SEM dual-beam system, cross sections are obtained  by milling using focused ion beams (FIBs).. Milling boxes  with typical dimensions up to several 10µm is possible within  a reasonable time. The position of the cross section can be  matched very precisely to the region of interest. In  combination with top down EBIC defect areas can be  identified and easily cross sectioned. In a subsequent step  EBIC imaging can be done at the FIB cross section to  investigate the depletion zone of the p/n-junction or a sub  surface defect structure present in the thin film stack. For best  spatial resolution, EBIC imaging at FIB cross sections should  be performed with the acceleration voltage of the primary  electron beam  as low as possible to reduce the interaction  volume of the electrons, see Fig. 6. In addition, applying  combinations of FIB milling and EBIC imaging three


dimensional structures of the depletion zone or defect  structures can be analyzed.


Figure 6: EBIC at FIB cross section at 52 degree sample tilt, left: overlay of gray scaled SEM image with red scaled EBIC  image at 30kV, right: idem but at 5kV


For successful EBIC analysis at cross sections it is essential to  obtain a clean surface and to avoid any preparation induced  defects influencing the EBIC signal. Ga ions strongly interact  with the material during FIB cross sectioning. It is known for  Silicon that Ga ions destroy its crystal structure. The thickness  of the formed amorphous layer is about 60 nm for  perpendicular and 25nm for gracing incident angle of 30kV  Ga ions. Moreover,, due to implanted Ga ions the electrical  behavior of the p and n doped layer near the cross section  surface could be influenced which can distort EBIC results. Therefore EBIC measurements at FIB cross sections need to  be validated e.g. by comparing these measurements with those  obtained on cross sections prepared with alternative methods  like cleaving or mechanically polishing, figure 7. EBIC  artifacts due to Ga implantation can be minimized or avoided  using low energy FIB for final polishing.


Figure 7: EBIC at 5kV at mechanically polished cross section  to verify results on FIB cross section


Experimental setup


A Quanta 3D FEG dualbeam system made by FEI Company is  used for FIB/SEM EBIC investigations. The system is  equipped with a Point Electronic DISS5 EBIC unit.  The  system features a high end amplifier which can handle the full  range of signals for low and high kV EBIC with an excellent  signal to noise ratio. Gain values can be directly controlled, which is important for the repeatability of EBIC  measurements. With this newly developed EBIC amplifier the  DISS 5 EBIC system is able to perform high-end and  quantitative EBIC measurements.


For the described FIB/SEM EBIC experiments, the samples  are mounted on specific holders like that depicted in Fig. 8, enabling local contacting with prober needles.


Figure 8: CSG sample mounted on specific holder and  contacted by probing needles to p and n contacts.


Case study on CSG


For CSG layers a drop in Voc is observed at large absorber  thickness which is stronger than expected from diffusion  length limitations. The first test sample is an experimental run  with unusually thick silicon for FIB-SEM EBIC evaluation.


First, the sample is analyzed by top down EBIC. A high  density of similarly formed defects can be found as dark spots  in the SEM/EBIC overlay as shown in Fig. 9. Microcracks in  the Si absorber are identified in the defect regions, figure 10. These microcracks locally separates the p/n electrodes, thus  preventing the formation of a depletion zone or electrical  contact to the p layer. In addition, we also observed a change  in electrically behavior at these defect areas during SEM or  FIB imaging; the EBIC signal was inverted from a low to high  value. Possibly, this is caused by a contamination layer  deposited on top of the Si absorber during SEM or FIB  imaging. However, the root cause for the observed cracking  should be a high residual stresses in the Si layer stack at larger  thickness.


A second case study is done on CSG material crystallized by a  new laser process which is currently under development. Laser treatment has to be done sequential on a cm-scale. The  sample Si layer in this case study is made in two steps. First, a  200nm n-doped amorphous Si layer is deposited by electron  beam evaporation on top of a SiN coated glass substrate. Then  the Si layer is recrystallized by laser treatment. Following a  cleaning step, a 1.5um, (p-/p+) a-Si is deposited by e-Beam  and crystallized in a solid phase epitaxy process [4].


Figure 9: Overlay of top-down EBIC and SEM images of a  CSG sample, dark spots related to microcracks in the Si  absorber (left), EBIC at FIB cross section of a defect area  visualizing the depletion zone (right)


Figure 10: SEM detail of microcrack in Si layer


One of the test samples was used to locate defective regions  by EBIC imaging and then to perform local FIB cross  sectioning and root cause analysis at individual defects.


Large area EBIC imaging is done to visualize defect  distribution and sizes, figure 11. A variety of large and small  sized defects are found. Most of the defects are easily  identified by SEM imaging as spots in the Si layer or particles  on the surface.


Figure 11: light optical view on the laser crystallized CSG  sample, darker areas correspond to double laser treated  regions (left), large area top down EBIC image shows high  defect density in double laser treated regions (right)


Additionally, circular defect regions are found by EBIC  imaging, figure 12 upper left. The corresponding SEM image  shows only a small sized defect in the centre, figure 12 upper


right as indicated by arrow as indicated by arrow. This is  highly indicative of the presence of a subsurface electrical  defect. Next, FIB cross-sectioning at the centre of this  subsurface defect is performed, and the cause is traced to a  bulge in the p-Si layer. However, the origin of the lost EBIC  signal in the surrounding area could not be found by SEM  imaging alone. Therefore, a thin transmission electron  microscopy (TEM) lamellae sample of this region is prepared  my FIB. TEM analysis of the defect spot shows that the laser  crystallized n-Si layer and the epitaxially grown p-Si on top  have different grain structures, figure 12 lower right. Reference investigation outside the defect shows the same  grain structure in p-Si and n-Si as expected. It is apparent that  the epitaxial Si grown on top of the n-Si is intercepted by an  intermediate layer. This layer is identified by high resolution  TEM as amorphous contamination caused by residues from  wet cleaning process.


Figure 12: EBIC detail of circular formed defects (upper left) and corresponding SEM image (upper right), TEM cross  section analysis of defect centre shows a bulged p-Si layer (lower left) and different grain structure between n-Si and  epitaxial grown p-Si (lower right)


Case study on CIS


Top-down EBIC on a CIS solar cell test sample shows that the  top layers above depletion zone block most of the primary  electrons up to the maximum acceleration voltage of 30kV. Therefore, top-down localization of shunts in the depletion  zone seems unpromising. During these investigations small  spots with locally high EBIC signal are found, figure 13. The  EBIC signal corresponds to small holes in the TCO top layer (figure 14), which the electron beam to access the depletion  zone. So in this case EBIC was useful to identify local layer  defects in the upper metal electrode.


Figure 13: SEM overview of CIS solar cell surface (left), corresponding EBIC image shows small bright spots  correlates to  µm sized holes in TCO layer on top (right)


Figure 14: SEM/EBIC detail of the identified hole in TCO at  52° sample tilt


In a second investigation, the formation of the depletion zone  in the CIS layer stack is analyzed by EBIC imaging of FIB  cross sections, figure 15. First experiments using standard FIB  milling results in a strong interaction between Ga and CIS  material.  At the surface of the cross section, a Ga/CIS  intermixing layer is formed, resulting in little details from  EBIC imaging. Adding XeF2 gas during FIB milling is found  to be effective in minimizing these artifacts, though other  proprietary techniques have been found to completely remove  all physical artifacts of Ga on imaged cross-sections as well.


Figure 15: SEM detail of a FIB cross section through the  metal/CIS/TCO layer stack (left), EBIC on FIB cross section  visualize the depletion zone related to the layer stack (right)


Case study on CdTe


CdTe thin film solar cells with shunt defects are investigated  by the EBIC/FIB method to understand the electrical behavior


in correlation to the local microstructure. The shunts are first  localized by using Lock in Thermography (LIT) which is one  of the standard methods for solar cell module investigation. Then top-down EBIC imaging was applied to localize these  shunts for further FIB-SEM and cross section EBIC analyses.


Figure 16: LIT amplitude image with hot spot marking a shunt  region (left), SEM/EBIC detail of this localized shunt defect (right). The EBIC signal was inverted to better visualize the  shunt region


The first FIB cross-section is done outside the shunt region, figure 17 upper left. Then stepwise FIB cross-sectioning and  EBIC imaging of the tilted sample are performed to  investigate the three dimensional structure of the shunt, see  figure 17.  By using a high acceleration voltage of 30kV, the  depletion zone is fully activated and the shunt can be  visualized simultaneously on top and at the cross section  giving a three dimensional impression of the electrical defect. At the centre of the shunt, an irregularly formed CdS/CdTe  layer containing voids is found. Applying a low acceleration  voltage of 2kV, it can be shown that the depletion zone at the  shunt is localized near the CdS/CdTe interface.


Figure 17 (left), inverted EBIC at 30kV on FIB cross section  through the defect visualizing its 3D shunt formation inside


the layer stack (upper left and right); EBIC at 2kV on FIB  cross section, irregular structure and voids in CdS/ CdTe are  found (lower left and right)


A second FIB-SEM EBIC analysis is done at a reference  position to compare with the undisturbed p/n-junction, figure


18. It is observed that EBIC signals at the FIB cross section  corresponding to the grain structure and the depletion zone  appear smeared-out in the CdS/CdTe layers. EBIC on  metallographically prepared (polished) cross-section also  gives similar results.


Figure 18: SEM/EBIC overlay of FIB cross section through  TCO/CdTe/metal layer stack, the EBIC signal in red  visualizes the depletion zone which in this case could be  affected from Ga implantation and CdTe grain structure


It has been demonstrated that an integrated FIB-SEM EBIC  system is an effective tool for characterization and failure  analysis of solar cells. Depth and dimension of depletion  zones can be visualized and associated to the absorber layer  stacks which can be used to monitor process fluctuations in  production lines. Furthermore, the combined FIB-SEM EBIC  method can be used effectively for the localization and  characterization of recombination centres and shunt defects at  sub-micron level and in three dimensions.


We like to thank our PV partners QCells, Sovello, CSG Solar, Calyxo and Odersun for supporting this work and providing  us with their samples. Many thanks go to Point Electronics for  providing it s new DISS5 EBIC system for evaluation in this  work.


[1] O. Breitenstein, et. al: “Shunt Types in Crystalline Silicon  Solar Cells“, Progress in Photovoltaics: Research and  Applications (2004) ; 12 : 529–538


[2] M. J. Keevers, et. al.: “10% efficient CSG minimodules,” in Proceedings of the 22nd European Photovoltaic Solar  Energy Conference, (2007), pp. 1783–1790


[3] Eiji Yoshida et al, “3-D EBIC Technique using FIB and  EB Double Beam System “, Proceedings of the 31st  International Symposium for Testing and Failure Analysis (2005), 163-168


[4] D. Inns, et. al.: “Localisation of the p-n junction in polysilicon thin-film diodes on glass by high-resolution cross


sectional EBIC imaging,” Thin Solid Films (2007), vol. 515, no. 7-8, pp. 3806–3809,.


[5] M .Werner et. al: “High-Resolution Electron-Beam  Induced Current Imaging of the P-N Junction in  Crystalline Silicon on Glass (CSG) Cells” Proceedings  23rd European Photovoltaic Solar Energy Conference, Valencia (2008), 2217-2220


[6] Falk et al. : “The European Project HIGH-EF: Multicrystalline Silicon Thin Film Solar Cells on Glass  24EUPVSEC”, 24th European Photovoltaic Solar Energy


Conference (2009), 2341 - 2343


# Activation Energy Analysis of Dark and Laser Illuminated I-V Characteristics of Thin-film Poly Silicon Solar Cells


Activation Energy Analysis of Dark and Laser Illuminated I-V Characteristics of Thin-film Poly Silicon Solar Cells


M. Boostandoost, U. Kerst, C. Boit


Berlin University of Technology, Institute of Radio Frequency and Semiconductor System Technologies  Section Semiconductor Devices


Einsteinufer 19, Sekretariat E2, D - 10587 Berlin, Germany


mahb@mikro.ee.tu-berlin.de, Tel.: +49-30-314-29947


The temperature dependence of photocurrent of polycrystalline  Si (poly-Si) thin-film solar cells on glass with interdigitated  mesa structure has been locally investigated using Infrared  Light Beam Induced Current (IR-LBIC) in the temperature  range of -25 to +70 °C. The temperature dependence of  electrical characteristics of poly-Si thin-film solar cells in  reverse bias has been also analysed and compared with the  monocrystalline thin-film solar cells. The poly-Si solar cell  shows a temperature coefficient (TC) for the photocurrent of  around +0.8 and +0.6 %/°C in the grain interior and grain  boundary, respectively. The activation energy of the reverse  current and also the photocurrent due to the IR laser  stimulation has been evaluated, which provide information  about traps and their energy levels in the absorber layer of the  poly-Si thin-film solar cell. The obtained average value of the  activation energy associated with the photocurrent of the    poly-Si cell suggests the existence of a shallow acceptor level  at around 0.045 eV in the grain boundary and 0.062 eV in the  grain interior of the absorber layer of the poly-Si thin-film  solar cell. The activation energies of the reverse current for  poly-Si and monocrystalline cells have been calculated when  the device is biased at -1 and -2 V and the results compared  with the activation energy of the saturation current obtained  from extrapolation of the I-V curve in the SRH (ShockleyRead-Hall) regime. The results show strong voltage  dependence. In both cases the activation energy of the reverse  current decreases in the reverse bias voltage, approaching the  values obtained from the photocurrent.


1) Introduction


Polycrystalline Si thin-film solar cells on glass are promising  candidates for future low-cost photovoltaic energy production


[1]. However, significant progress is still required to improve  the conversion efficiency of these devices, which are to a large  extent limited by microscopic defects (e.g. at grain  boundaries). Thus, in order to gain deeper insights in the  mechanisms dominating the losses in poly-Si solar cells, microscopic methods like Light Beam Induced Current (LBIC) techniques are needed.


In this paper, IR-LBIC (Infrared Light Beam Induced Current), which is well established technique in the community of  microelectronic devices, is applied to the investigation of polySi thin-film solar cells on glass.


In LBIC, a laser beam is scanned over the device and the  photocurrent induced by the laser beam is monitored. The  variations in the current collection are correlated with the  position of the laser, leading to a current map (LBIC map). In  the solar cell community, LBIC measurement is used to  investigate the cell performance.


For IR-LBIC measurements a laser beam with the wavelength  in the IR range, a little shorter than the wavelength of the  bandgap energy of silicon (1.1 eV), is used. We have  implemented the IR-LBIC measurement using the wavelength  of 1064 nm. The IR-LBIC measurement provides the  information about the solar cell spectral response for photon  energy close to the silicon bandgap energy, which is especially  interesting in thin-film cells because of the low absorption rate. The advantage of low absorption rate can be used for many  applications like extraction of the diffusion length of minority  carrier [2] or for investigating light trapping structures in thinfilm solar cells [3].


2) Setup


IR-LBIC (Infrared Light Beam Induced Current) measurement


has been performed using the laser with the wavelength of


1064 nm to investigate thin-film solar cells and obtain


information about the grain boundaries. The PHEMOS 1000


setup used for the temperature-dependent IR-LBIC


measurement is depicted in figure 1. Main components of


experimental setup include a laser scanning microscope


(LSM), a DC power supply, and a current monitoring unit


including an amplifier, a laser light source, an image processor


and a display. The solar cell sample has been placed on a


thermal chuck and its terminals have been contacted using


microprobe heads and needles.


The TP03000A1 thermo chuck system with a temperature


range of -65 up to 200 °C and a temperature accuracy of


0.5 °C is used to investigate the dark and laser illuminated I-V


characteristics of the poly-Si thin-film solar cell. Temperatures


higher than +80 °C can cause serious damage to the


transparent conductive oxide (TCO) layer. Therefore, for


accurate calculations of activation energies, the measurements


have been implemented in the temperature range of -25 up to          +70 °C to provide a wider range of data. A flow of dry


nitrogen gas is used to act as a shield to prevent ice


accumulation on the sample surface. Therefore, while cooling


down, the sample is insulated from ambient humidity by an


outer layer of nitrogen gas supplied by a high pressure tank.


The nitrogen pressure has to be adjusted manually. The


temperatures have been measured with the digital thermometer


K204 through two channels using two type-K thermocouple


temperature sensors, which were mounted on the surfaces of


the samples.


The PHEMOS 1000 combines laser stimulation and light


emission microscope with a silicon cooled CCD camera as a


detector for acquisition of extremely faint emission within the


broad spectral range including both visible and infrared


regions [2]. The objective with 50X magnification has been


used for IR-LBIC measurements. The laser power can be


adjusted over a continuous range using the PHEMOS control


software. The maximum laser power density using the


objective with 50X magnification is about 20 mW/m2. The


spot size of the laser is calculated numerically, considering the


numerical aperture (N.A.) of the optical system and the laser


wavelength. The laser spot size using the 1064 nm laser and


the objective with 50X magnification is about 1.7 m.


Figure 1: Measurement setup used to perform the


temperature-dependent IR-LBIC technique.


Laser stimulation with 1064 nm wavelength uses the  photovoltaic effect to generate the photocurrent. When the  sample is scanned with the laser beam, primarily photocurrent  is generated in silicon due to the fact that the photon energy is  higher than the indirect bandgap of silicon (1.1 eV). Ideally, absorption of one photon creates one electron-hole pair which  is then separated by pn-junction and increases the current that  can be measured through an external amplifier. The OBIRCH  amplifier amplifies the weak current induced by IR-LBIC. The  PHEMOS 1000 system has the signal amplifying unit  consisting of voltage and current sources and can amplify the  voltage change up to a factor of 100.


The laser scan controller is the basic component of the image  processing unit in the PHEMOS 1000 system and controls the  scanning procedure of the laser beam via line and frame  signals. A laser scanning microscope (LSM) micrograph can  be superimposed on the light emission or laser stimulation  image. Finally, the current change produced by the laser beam (photocurrent) as it scans the sample is converted into  variations in contrast to form the IR-LBIC map.


The IV-characteristics were obtained with a HP4145B  semiconductor parameter analyzer. The same temperature  controller and thermometer have been used to examine the  temperature dependence of the reverse current.


3) Devices


The poly-Si solar cells investigated in this study are composed


of a p-type poly-Si absorber layer with a thickness of about      2 µm that was grown epitaxially by electron-beam evaporation


on a thin, large-grained p+-type poly-Si seed layer (~200 nm).


The seed layer was formed by the aluminium-induced layer


exchange (ALILE) process [5]. On top of the poly-Si absorber


layer a 10 nm thick n+-type amorphous Si emitter was


deposited by plasma-enhanced chemical vapour deposition


(PECVD). Sputtered ZnO:Al was used as transparent


conductive oxide (TCO). After mesa etching interdigitated


contacts were deposited on top of the cell. This device has


been introduced in details elsewhere [2]. As a reference, a


monocrystalline wafer-based Si solar cell with a similar device


structure has been investigated.


4) Results


The laser with the wavelength of 1064 nm is used to perform  the laser stimulation. This laser generates not only electronhole pairs in the silicon via photoelectric laser stimulation (PLS), but also creates some thermal laser stimulation (TLS) effects, especially on the metallic structures.


Pure PLS effect is found at a non biased condition but the TLS  effect on metal interconnects appears with increasing the  current. Since PLS is the primary focus of this work, a region  in the active area of the cell and far from the metal contacts  was chosen to avoid influence from TLS and Seebeck effects. The laser wavelength is much longer than the thickness of the  amorphous silicon emitter layer (~10 nm). Therefore the  activity which is observed provides mainly the information  about p-doped absorber layer.


When implementing the IR-LBIC measurements with the laser  wavelength of 1064 nm, a higher signal response is obtained at  the grain boundaries than the grain interior. Using the high  objective magnification (50X) lens, this difference in signal  response is obviously observed. The darker areas are those  with a higher current change rate. Further measurements are  required to explain IR-LBIC response behaviour in the grain  boundary of the poly-Si thin-film solar cell.


Figure 2 shows the IR-LBIC signal using 1064 nm wavelength  laser with 5% of the maximum laser power. The white band is  the emitter metal contact which shows no signal response. The


Laser Controller


X-Y Scanner


Laser Light


Source


Signal & Image


Processor


Microscope


Current Change   monitor


OBIRCH amplifier  DC Power Supply


DUT


Sample Stage


Temperature Controller


Thermometer


PHEMOS 1000


device is not biased and 20 frames have been integrated to  obtain a sharp and clear image with a high S/N ratio and wide  dynamic range.


The IR-LBIC measurement has been performed in area mode, to avoid any additional effect, such as TLS. Therefore as  figure 3 shows, a 30×30 µm2 window in the active area of  poly-Si cell far from the metal straps has been chosen for the  measurement.


Figure 2: IR-LBIC signal map using objective with 50X


magnification and a laser power of ~0.12 mW/m2. The device  is not biased.


The photocurrent was obtained from the IR-LBIC


measurement with the solar cells biased at 0, -1 and -2 V. To


investigate the temperature dependence of the photocurrent,


generated by IR-LBIC measurement, different areas at the


grain boundaries and grain interiors have been chosen,     figure 3. The IR-LBIC measurement has been performed at


each temperature from -25 up to +70 °C with 5 °C step. The


average IR-LBIC signal response in these areas at each


temperature has been calculated. The contribution of the


shallow defects in recombination is doping concentration


dependent and is higher at lower temperature. Therefore at the


temperature range of our measurement the activity of the


shallow defects with energy level away from midgap can be


obseved [6].


Ea(GB3)=0.0561 eV were also obtained for grain boundaries.


The standard deviation of the activation energy obtained for


the grain boundary and grain interior are 0.0134 and 0.0246


eV, respectively. Therefore, the three activation energies


obtained for the grain boundaries are the same to within the


deviation, and also the results of two activation energies for


the grain interiors lead to the similar values.


As the results show, the activation energy obtained from the


grain boundary is smaller than the one from grain interior


(about 0.0387 eV). The laser wavelength used for the IR-LBIC


measurement which is slightly higher than the bandgap energy


of poly-Si can mainly activate the carriers trapped in subgap


states. There are relatively shallow subgap states at energy   |EC – ET| (defect in the upper half of the bandgap) or |EV – ET| (defect in the lower half of the bandgap) which are acting as  fast minority carrier traps or recombination centers. EC, EV and  ET are the conduction band, valance band and trapping level  energy in eV, respectively [8].


The activation energy of photocurrent has been calculated for  the poly-Si thin-film solar cell, when it is biased at 0, -1 and    -2 V. As the table 1 shows, the activation energy of  photocurrent is almost independent of the applied bias voltage. The standard deviation of activation energy increases with the  reverse bias voltage.


Activation energy of photocurrent [eV]


Applied


Voltage GI1


GI2


GB1


GB2 GB3


0 V


0.0687 0.0602 0.0562 0.0438 0.0306


-1 V


0.0611 0.0506 0.060 0.0428 0.0516


-2 V


0.0768 0.0840 0.0348 0.0341 0.0516


Table1: The activation energies of the photocurrent in grain  boundaries and grain interiors of the poly-Si thin-film solar  cell, when the sample is biased at 0, -1 and -2 V. The results


are not strongly dependent on the applied bias voltage.


The activation energy values from the temperature dependence  of saturation current have been also calculated for both poly-Si  and monocrystalline thin-film solar cells. The temperature  dependence of the saturation current for silicon based pn  junction at temperatures below 100 °C is practically given by  the intrinsic concentration, ni, through the factor exp(Eg/2kT) where Eg is the bandgap energy of the semiconductor (the  generation current component) [10]. Considering the bandgap  energy of monocrystalline silicon in the range of 1.1 to 1.2 eV, activation energy value, Ea = 0.5–0.6 eV at the measurement  temperature range has to be exhibited.


The activation energy of saturation current of the  monocrystalline reference solar cell is determined through  extrapolation of the I-V curve in SRH regime, which is equal  to 0.68 eV. This value is close to that expected from the theory  for monocrystalline solar cells [9].


The activation energy of the saturation current of the poly-Si  thin-film solar cell has been also similarly determined, which  was equal to 0.192 eV. The great difference of the activation  energy obtained from the saturation current of monocrystalline  and poly-Si thin-film solar cells can be interpreted with a  narrower badgap of a later one compared to the  monocrystalline thin-film solar cell and the influence of grain  boundaries on the performance of the poly-Si thin-film solar  cell. The resulting value, which is considerably lower than the  reported value of |EC-EF| in monocrystalline solar cell can not  just be explained with the smaller bandgap in poly-Si, but it  mainly reflects the contribution of traps in the process (|ET-EF|)


[9].


The activation energy of the reverse current has been also  calculated for both of the samples. The activation energy of the  monocrystalline thin-film solar cell reduces in reverse bias to


0.55 and 0.44 eV with the device biased at -1 and -2 V, respectively. The Arrhenius plots for calculations of the  activation energies of the reverse current of the poly-Si thin161


film solar cell are illustrated in figure 5. The extracted  activation energies are equal to 0.061 and 0.030 eV for the  sample biased at -1 and -2 V, respectively.


In both samples the activation energy of the reverse current has  been reduced with increasing the magnitude of reverse bias  voltage. This behavior indicates that the variation in electrical  bias can cause the change in the trap level occupancy in the  absorber layer, which is observable through the activation  energy of reverse current


Figure 5: Arrhenius plot; Activation-energy value derived  from the temperature dependence of the reverse current of  poly-Si thin-film solar cell, when is biased  at -1 and  -2 V and  the saturation current obtained from extrapolation of the I-V  curve in SRH regime.


As mentioned already, poly-Si thin-film solar cells include  many defect energy levels in the bandgap caused by native  defects and impurities. Complex defects, which simultaneously  act as acceptors and donors, are formed during the growth of  the absorber layer. Considering the band diagram of a reverse  biased abrupt n+p junction, the obtained activation energy for  the reverse current is considered to correspond to a shallow  acceptor level (Al or B) [10,11].


We have performed the LBIC measurement in IR range with a


wavelength of 1064 nm on the poly-Si and monocrystalline


thin-film solar cells with same structure. Using the high


resolution (~2 µm) the temperature dependence of the           IR-LBIC signal in the grain boundary and grain interior has


been investigated quantitatively. It has been shown that the


photocurrent of poly-Si thin-film solar cell increased with


increasing the temperature. The activation energies of the


photocurrent and saturation current with samples biased at 0,


-1 and -2 V have been measured spatially at the grain


boundary and grain interior. The results have been used to


introduce the defects and their energy levels at the grain


boundary and grain interior, which is of crucial importance for


analyzing and further optimizing the efficiency of thin-film


solar cells.


The authors would like to thank Hamamatsu KK Japan and  Germany for support; many thanks go to Stefan Gall and Pinar  Dogan from HZB (Helmholtz Zentrum Berlin) for providing  the samples and to Felice Friedrich for helpful discussions  concerning the subject of this paper.


[1] Green, M.; Basore, P.; Chang, N.; Clugston, D.; Egan, R.; Evans, R.; Hogg, D.; Jarnason, S.; Keevers, M.; Lasswell, P.; O'Sullivan, J.; Schubert, U.; Turner, A.; Wenham, S. & Young, T., Crystalline silicon on glass (CSG) thin-film  solar cell modules, Solar Energy, 2004, 77, 857 – 863


[2] Boostandoost, M.; Lin, H.-P.; Kerst U.; Boit C., Analysis  of poly-Si thin-film solar cells by IR-LBIC, ISTFA™ 2009, Conference Proceedings from the 35th International  Symposium for Testing and Failure Analysis, San Jose, California, USA, 2009, 157 – 161


[3] Orton, J.W.; Blood, P. , The Electrical Characterization of  Semiconductors: Measurement of Minority Carrier  Properties, (Techniques of Physics, Vol 13), Academic  Press, 1990, 222 – 225


[4] PHEMOS series General catalogue, Emission Microscope  PHEMOS Series, Cat. No. SSMS0003E07, 2008


[5] Gall, S.; Becker, C.; Conrad, E.; Dogan, P.; Fenske, F.; Gorka, B.; Lee, K.; Rau, B.; Ruske, F. & Rech, B., Polycrystalline silicon thin-film solar cells on glass, Solar  Energy Materials and Solar Cells, 2009, 93, 1004 – 1008


[6] Rein, S.; Rehrl, T.; Warta, W. & Glunz, S. W., Lifetime  spectroscopy for defect characterization: Systematic  analysis of the possibilities and restrictions, Journal of  Applied Physics, 2002, 91, 2059  – 2070


[7] Bube, R. H., Photoconductivity of solids, John Wiley& Sons Ltd., New York, 1960


[8] Sriprapha, K.; Yeop Myong, S.; Yamada, A.; Konagai, M., Temperature dependence of protocrystalline  silicon/microcrystalline silicon double-junction solar cells, Japanese Journal of Applied Physics, 2008, 47, 3, 1496 – 1500


[9] Wong, J.; Huang, J. L.; Kunz, O.; Ouyang, Z.; He, S.; Widenborg, P. I.; Aberle, A. G.; Keevers, M. & Green, M. A., Anomalous temperature dependence of diode  saturation currents in polycrystalline silicon thin-film solar  cells on glass, Journal of Applied Physics, 2009, 105, 103705


[10]Sze, S.M., Semiconductor devices, physics and  technology, John Wiley & Sons, 1985


[11] Buchwald, W.R.; Morath, C.P.; Drevinsky, P.J., Effects of  deep defect concentration on junction space charge  capacitance measurements, Journal of Applied Physics, 2007, 101, 094503


# Characterization and failure analysis of 3D integrated semiconductor devices-novel tools for fault isolation, target preparation and high resolution material analysis


Characterization and failure analysis of 3D integrated semiconductor devicesnovel tools for fault isolation, target preparation and high resolution material  analysis


Frank Altmann, Matthias Petzold, Christian Schmidt, Roland Salzer


Fraunhofer Institute for Mechanics of Materials, Halle, Germany


Frank.Altmann@iwmh.fraunhofer.de, 0049-345-5589-139


Cathal Cassidy


austriamicrosystems AG, Unterpremstaetten, Austria


Cathal.Cassidy@austriamicrosystems.com, 0043 3136 500 5943


Paul Tesch, Noel Smith


Oregon Physics, Hillsboro, OR 97123


p.tesch@oregon-physics.com, 001 503 601 0041


In this paper we will introduce novel methodical approaches  for material and failure analysis of 3D integrated devices. The  potential and advantages of the new concepts and tools will be  demonstrated for flip-chip-like interconnects but in addition, for the first time, for Through Silicon Vias (TSV). The  employed techniques combine non-destructive fault  localization with efficient and accurate target preparation to  get access for following microstructure diagnostics, forming a  subsequent failure analysis workflow. The concept presented  here involves the application of improved Lock-In  Thermography (LIT), and three different innovative concepts  of high rate Focused Ion Beam (FIB) techniques.


During the previous years, technologies for 3D integration of  semiconductor devices have attracted rapidly increasing  attention. Both process step development and reliability  aspects require a precise control of the component  microstructure with particular respect to the involved  interfaces and TSV interconnects. However, the complexity of  three-dimensional high-density integration in terms of novel  designs, processes and materials, and reduced testability pose  severe challenges to the techniques and tools applied for  material characterization and failure analysis. In particular, new fault isolation methods with 3D defect localization  capability are required. Furthermore, the failure analysis needs  more efficient target preparation techniques allowing to  combine a rapid cross sectioning of rather large quantities  with high precision artifact-free access to defective buried  interfaces and interconnects, as well as adapted highresolution microstructure diagnostics methods to understand  interface properties in interconnects.


In this paper, novel methodical approaches for defect  characterization in 3D integrated components are discussed. The potential of the techniques is illustrated for flip-chip-like  and TSV interconnections. The employed techniques combine  non-destructive defect localization with efficient and accurate  target preparation techniques to get access to functional  structures and failure sites on 3D device level. It is  demonstrated that LIT methods provide a superior potential  for analyzing electrically defective interconnects like resistive  opens and shorts. LIT can particularly be applied to isolate  vertical interconnects in high density TSV arrays. Typically, the identified defects traced by LIT require subsequent cross  section target preparation for further failure analysis. It is  shown that different novel high-efficient Focused Ion Beam (FIB) techniques provide excellent erosion rates for silicon  components. As a consequence, FIB milling through the  complete wafer up to several hundreds of micrometers in  depth becomes possible. This enables rapid and precise access  to the fault sites previously localized by LIT. As a result, high  resolution electron microscopy and material diagnostics could  be applied for 3D integration specimens with significantly  improved throughput and efficiency. Thus, the comprehensive  failure diagnostics approach developed here can, in future, support an effective process step development for current 3D  integrated devices. In addition, it may contribute to improve  the reliability properties of the assembled complex devices  and systems.


Sample descriptions


For the 3D integration assembly process, different bonding  technologies have been proposed depending on the specific  boundary conditions with respect to technology and targeted  application [1]. Direct oxide bonding is not only be applied  for mechanically stacking of different components but  supports also the formation of metallic interconnects inside  the bonded interface. Alternatively, Cu thermocompression  bonding provides a feasible technological alternative.


Furthermore, interconnects formed by micro solder bumps  with diameters even significantly below the typical range of  flip-chip interconnects (e.g. < 80 μm) have frequently be used  for 3D integration.


In this paper samples fabricated by a novel Ni microinsert  technology [2] were used. The Ni microinsert technology is a  flip-chip-like process for face-to-face interconnection of  heterogeneously integrated systems. While solder bumps are  used for conventional flip-chip technology in many cases, here small spikes of Ni are formed at the point of  interconnection between the two dies. In terms of bonding  quality and reliability, the choice of glue layer and the deviceto wafer co-planarity are crucial to avoid regions with open  circuits or high-resistance contacts. In the investigated system, 32 contact pads forming a daisy-chain structure were used  with each pad containing 16 isolated microinserts with a  diameter of 5 m. Specimens that showed a significantly  increased ohmic resistance after assembly were analyzed to  detect the failure mechanism involved.


Figure 1. Ni microinserts plated on a metal pad and system  assembly by thermo-compression bonding


A second type of sample has devices with daisy chains of  TSV interconnects with 100μm diameter. The TSVs are made  by Si etching using the Bosch process. Silicon dioxide  deposition was used for isolation, followed by TSV sidewall  metallization with Ti/TiN, W and Al. Finally, the TSVs were  passivated by using a silicon dioxide film and silicon nitride  layers [3]. Specimens with electrical shorts between TSV  metallization and Si substrate were investigated.


Figure 2. Through silicon vias with a diameter of 100μm and  a depth of 250μm with sidewall metallization (unfilled)


Novel failure analysis techniques


Fault isolation by Lock- in Thermography


Lock-in-Thermography (LIT) is a novel technique for thermal  based fault isolation to localize electrically defects like  resistive opens and electrical shorts. The defective circuitry is  stimulated electrically by a periodically pulsed supply voltage  with a certain frequency producing a local thermal heating at  the defect origin. The device under test is measured by a freerunning high sensitive IR camera applying a two channel lock  in image processing. This phase-correlation approach allows  high spatial resolution and sensitivity that is even higher than  the thermal noise of the camera detector itself. The resulting  0° and 90° signals are integrated and make it possible to  derive either the amplitude or the phase image. The amplitude  image has the advantage that the signal to-noise-ratio is  increased and therefore defect-related hot spots are detectable  while the phase image leads to a dynamic suppression and  removes the influence of the material emissivity. By analyzing  the defect’s depth-related phase shift, 3-dimensional defect  localization within fully packaged and complex devices is  possible. The first investigations of this topic were published  in [4,5].


Using both resulting images, the amplitude and the phase  image, it is possible to detect thermally active defects with a  spatial resolution down to approximately 1 m and dissipation  power sensitivity down to a few W. In addition, due to the  fact that silicon is transparent in the infrared range, LIT can  not only be easily applied for IC back side analysis but also to  analyze the interface between vertically stacked Si dies.


Figure 3. Working principle of LIT


New concepts of high rate Focused ion beam milling


In many failure analysis cases, the preparation of  metallographic cross-sections of the localized defect site is  necessary to investigate the mechanism causing the failure. In  addition to the need to remove large quantities of materials, a  typical problem of mechanical cross-sections is the smearing  of soft materials such as tapes, gold metallization, or solder  into cracks and delaminations. This normally requires the  application of ion polishing for a significant increase in  sample quality, and the use of FIB techniques. However, especially for packaged or stacked systems, the time required  for the FIB preparation is the limiting factor due to the  relatively slow ion milling process. The ablation rate of silicon


is typically as low as 2.7 m3/s for a beam current of 10 nA. This is sufficient for target preparations on the processed  semiconductor surface or the Integrated Circuit (IC) level  respectively, but for typical packaging dimensions, or for  stacked Si systems, a huge amount of time is necessary. Up to  now, a so-called High-Current FIB (HC-FIB) can achieve  beam currents up to 100 nA and ablation rates of up to 30  m3/s.


In comparison to this current technique, significant progress  can be achieved by three different approaches.


First, the additional insertion of reactive gases using a GasInjection System (GIS) allows to increase the etch rate by one  or two orders of magnitude [6]. It was shown that bulk Si  trenching can be done using a high gas flux of XeF2. For our  investigations, we used a FEI V600CE+ single beam FIB  equipped with a high current column producing a well shaped  focused ion beam up to 67nA. Bulk silicon trenching can be  performed by a special coaxial gas delivery nozzle that  accelerates silicon etching for faster wafer level cross  sectioning. The capabilities of the system are extended by a  near infrared microscope permits imaging of target structures  through the backside of bulk silicon for fast, accurate  navigation also in 3D integrated devices.


Figure 4. left: Si removal by XeF2 assisted high current FIB  milling (200μmx200μm window through 250μm Si substrate  in about 30min); right: interconnect lines imaged through Si  by using integrated IR microscope


Second, Inductively Coupled Plasma (ICP) ion sources were  applied for target preparation of electron components. Compared to a conventional Liquid Metal Ion Source (LMIS), ICP ion sources have significant higher beam currents in the  A- and even mA-range. We used a new focused ion beam  instrument made by Oregon Physics capable of creating crosssections as large as 1 millimeter in size [7]. In this instrument, a radio frequency plasma ion source with an electrostatic  matching lens has been integrated onto a commercially  available two lens electrostatic FIB column to create a new  FIB tool that can mill structures from less than 100  nanometers to over a millimeter in size. For the plasma, a  variety of different gases including Xenon, Oxygen, Argon  and Helium are applicable depending on the material to be  removed. The ion source provides probe current from tens of  picoamperes to over 2 microamperes. With Xenon at 4  microamperes, the volume removal rate for silicon at normal  incidence is approximately 2000 m3 per second. Mill rates  approaching 6000 m3 have been achieved for producing  cross-sections.


A third possibility is given by the combination of  conventional FIB preparation with a preceding laser ablation  for high rate material removal of parts of the sample. The  feasibility of laser-based target preparation of electronic  components in cross section with a single laser source was  demonstrated recently for molding compound, silicon dies, and metal interconnects in 3D integrated devices. Various  laser technologies such as ultra-short pulse lasers, excimer  lasers, and diode pumped solid state (DPSS) lasers with  different wavelengths and pulse durations were evaluated. For  the target preparation of stacked silicon dies, the laser  wavelength was the most important factor with respect to  artifact-free thinning. With the ultraviolet 355-nm DPSS laser, a distinct ablation also of the stacked silicon dies was possible  with resulting surface roughness of around 5 m [8, 9]. Furthermore, the heat effected zone (HAZ) during laser  preparation was analyzed, which is extremely important to  help determine if visible cracks or delaminations are artifacts  caused by the thermal load during laser preparation, or real  defects in the device. A molten region only 1-2 m thick was  found. After estimation of the amount of absorbed energy, the  spatial and transient temperature profiles were calculated by  finite element simulations. These thermal simulations  confirmed that the molten material, here silicon, cools down to  a few degrees above ambient temperature in the time interval  of tens of s until the next laser pulse is deployed. A  significant temperature increase occurs only within a distance  of 5-6 m close to the laser edge. Therefore, the extension of  the HAZ is limited to the order of the surface roughness [10].
  We used a novel laser-FIB demonstrator made by Zeiss NTS  combining the excellent ablation rates of pulsed laser ablation  with the high accuracy of FIB milling. Therefore, an FIB  device was equipped with a new high current ion-beam  column and a laser ablation device directly attached to the FIB  lock chamber.


Failure analysis case studies


Daisy chain of Ni microinserts


Firstly the high ohmic daisy-chain devices were analyzed by  LIT to locate defective microinsert contacts. LIT  measurements were done at a current of 50 mA producing a  dissipation power of a few mW. It was possible to detect a  thermal signal from the device within a few minutes at a lockin frequency of 25 Hz. In Fig. 5, defect-related thermal  emissions indicating the presence of high ohmic contacts  between the dies can be seen at the spots (1) and (2) compared  to a reference contact (3) which shows no heat dissipation. For  the following target preparation step, high spatial resolution is  required. A resolution improvement for the thermal emission  signal itself can easily be achieved by using a Gaussian fit. However, for a precise allocation of the thermal emission to  the defective structure, a high spatial resolution of the  topography pattern in the sample is also necessary. Therefore, LIT was used with a recently developed high-resolution  infrared objective. Fig. 6 shows that the resulting spatial  resolution allows the identification of single defective Ni


plugs with 5 m diameter inside the chip-to-chip interface. The lower temperature sensitivity of high-resolution imaging  can be compensated for by an increased measurement time. The identified defects traced by lock-in thermography can  now be prepared in cross section by the following efficient  target preparation step. For this purpose, we evaluated a novel  methodical approach combining the excellent erosion rates of  pulsed laser ablation with the high accuracy of focused ion  beam (FIB) milling [11].


Figure 5. LIT amplitude image showing a defect-related  thermal emission at the interconnect areas (1) and (2) between two dies in comparison to a reference contact (3)


Figure 6. High-resolution imaging using LIT of a contact


area allows the exact localization of single defective Ni


plugs


Laser preparation was applied to perform a cross-section  through those Ni microinserts that showed hot spots during  LIT measurements, thus indicating highly resistive contacts. Fig. 7 shows the area of laser preparation, which was a square  of 1 mm2; the depth of the laser cavity was 300 m. Laser  parameters were chosen which resulted in an ablation rate for  the silicon of around 1×106 m3/s. The processing time to  remove the silicon volume of 0.3 mm3 was 300 seconds. An  ablation rate of 6.5×106 m3/s is achievable for silicon with  this laser system. After a processing time of 300 seconds, the  cavity depth is 300m. Fig. 8 shows a more detailed view of a  corner of the laser-prepared cavity. The 4- to 5-m-thick glue  layer between the 180-m-thick upper die and the silicon  substrate is clearly observable. The emerging edges during  laser ablation in silicon are not perpendicular. An edge angle  of around 12 degrees occurs, which is very advantageous  during subsequent FIB polishing. This edge angle has to be  also considered as an offset during laser navigation, which can  currently be done with a position accuracy of around 10 m. Despite the fact that a single laser impact has a diameter of  more than 40 m, due to the mentioned edge angle, the corner  radius decreases down to 2-3 m. The Ni microinserts, the  glue layer, and the metallization are clearly observable  immediately after laser preparation. No cleaning or polishing  has been applied at this stage of preparation. Fig. 9 shows the  corner of the laser cavity after a few minutes of subsequent  FIB polishing with a beam current of 10 nA. In the region of  the Ni microinserts, the material is removed to a depth of 3-4  m. It shows an increased cross-section at the edge of the  laser cavity which is prepared with an ion current of 50 nA  and subsequent polishing at 10 nA and 2 nA.


Figure 7. Overview of laser-prepared Si die to reveal the  interconnects inside the bonded interface


The detailed view of two Ni microinserts in Fig. 10 shows the  root cause of the hot spot signal detected by LIT. A glue-filled  gap is observable between the Ni microinsert and the top die  while the contact between the plated Ni and the bottom die is  intact. The reduced contact area to the top die results in an  increased current density and causes the hot spots observed by  LIT measurements. This result was also confirmed by  conventional mechanical cross-section preparations followed  by FIB analysis.


Figure 8 . Corner of the laser-prepared cavity with the 4- to  5-m-thick glue layer below the 180-m thick upper die


Figure 9. Cross sectioned Ni microinsert interconnects after a  few minutes of additional FIB polishing


Figure 10. Highly resistive Ni microinserts (left) with gluefilled gap (arrow) compared to an electrically intact reference  contact (right), detail


For the same samples, a new plasma FIB system (Hyperion) from Oregon Physics was also used to cross-section a row of  micro-inserts for comparison. Here, a 600nA, xenon focused  ion beam was used to remove 1um slices, across a length of  220um, until the center of a via row was reached. Each slice  took 55seconds, revealing the four vias seen in Figure 11. Here, a second gallium FIB is used to image the plasma FIB  cross-section, allowing the cross-section to be precisely  centered on the micro-insert. Thus, this new system also


provides high additional potential for the considered failure  analysis application.


Figure 11. Ni microinsert interconnects, cross-sectioned by  plasma FIB (left) and imaged with in-situ gallium FIB to show  grain micro structure (right),


TSV with metallized sidewalls


A second case study was performed on TSV with metallized  sidewalls with 100μm . The TSV are connected electrically in  a daisy chain structure. For defective devices, the electrical  measurements performed showed that the TSV metallization  was shorted to the Si substrate and that the I-V curve of the  short had a diode’s characteristic. In a reference analysis, emission microscopy was applied to localize the shorted TSV. Using a high voltage stimulation of 25-30V a defective TSV  could localized. To derive information on defect depth inside  the TSV structure, defocus series were made by emission  microscopy starting at the device surface [12,13].  A local  emission spot could be imaged at 210 μm defocus. The area of  light emission started from the TSV sidewall and reached  several μm into the Si substrate, Figure 12.


Figure 12. Defective TSV localized by Emission Microscopy; austriamicrosystems AG


For comparison applying LIT, similar focus series were


performed on the same sample to investigate the defect origin  again. The defocus could be precisely adjusted by moving the  sample using a stage with μm accuracy. For LIT


measurements the TSVs were electrically stimulated by


probing of bond pads which are connected to TSV


metallization and Si substrate. LIT defocus series were done  applying a supply voltage of 24,5V producing a leakage


current of 80μA. For each measurement, a single IR image


focused on device surface was acquired to provide topography  images as reference. The topography image was overlayed


with the LIT amplitude image taken at different defocus


values to allocate thermal signals to device layout. Then a first  LIT measurement was performed focused at surface of the


Figure 3: IR-LBIC map achieved using 50X objective


magnification and a laser power of ~0.12 mW/m2 in area  mode. The selected areas for investigating the temperature  dependence IR-LBIC measurement are marked. The device is  biased at -2 V.


The results show that photocurrent increased with increasing  the temperature. This phenomenon is what usually observed in  most semiconductors [7]. The reasons for the increase in  photocurrent include the reduction of the bandgap energy, the  increase in the diffusion length of the minority carriers, and the  reduction of the recombination velocity or unfilled localized  states [8].


The temperature coefficient (TC) of photocurrents of the polySi thin-film solar cell, induced through IR laser in the grain  boundary and grain interior has been calculated. The TC has  been calculated considering T0=25 °C as a reference  temperature. The TC of photocurrents in the grain boundary  and grain interior are equal to +0.6 and +0.8 %/°C, respectively. The TCs has been also calculated biasing the  poly-Si thin-film solar cell in 0, -1 and -2 V. The results show  weak dependence on the applied bias voltage.


Figure 4: Arrhenius plot; the straight lines were drawn by


fitting the experimental data for obtaining the activation  energy of the photocurrent of  the poly-Si thin-film solar cell, induced by IR laser in the grain boundary and grain interior. The device is biased at -2 V.


Figure 4 show semilog plots of the photocurrent vs. 1/KT for


the poly-Si thin-film solar cell, when the device is biased at     -2 V. T and K are the temperature in kelvin and Boltzmann’s


constant, respectively. For each area, including GI1, GI2,


GB1, GB2 and GB3, one straight line whose slope is equal to


the activation energy were plotted by fitting the experimental


data. From the illustrated plots, two activation energies


Ea(GI1)=0.0768 eV and  Ea(GI2)=0.0840 eV were obtained


for the grain interior. Three activation energies


Ea(GB1)=0.0348 eV, Ea(GB2)=0.0341 eV and


Figure 6: Resolution of the imaging system calculated based  on images of test structures consisting of metal lines of various  width (0.8 µm, 1 µm, 2 µm and 4 µm) and edge response  methodology (ER). Images were taken using 100x microscope  NIR objective with NA=0.5.


For the narrower metal lines (0.8 µm and 1 µm) the edge  response did not give proper results as the system was not  capable of fully responding to the edge because of its limited  resolving properties. The wider lines (2 µm and 4µm) gave  proper results. First of all, the results are similar, meaning that  the system responds fully to the edges. In addition, the results  lie within the resolution region determined by the well known  microscope empirical formulas (also known as Rayleigh and  Sparrow criteria).


Examples of trenches leaving varying thicknesses of silicon are  presented in Figure 7 for test structure A. The images were  acquired using the full spectrum of the Si CCD detector. As  one can see, for the ultrathin silicon (UTS) case, the structure  of interest can be imaged very well, and the features can be  seen easily. However, the imaging properties degrade rapidly  with increased remaining silicon layer thickness.


Figure 7: Images taken through trenches under structure of  type A with various thicknesses of remaining silicon.


To trace the imaging properties wavelength-wise, images were  also acquired using band-pass interference filters. Depending  on the resolution characterization approach and the structure  type, the reflected light intensity profiles were recorded as  indicated in Figures 2 and 3. In addition, the results obtained  with the LSF method were further normalized to compensate  for the width of the imaged feature. The results of these  measurements for the UTS samples (0-1 µm) are presented in  Figure 8. In addition, one example of the thicker silicon layer  sample is included as well.


Figure 8: Resolution of the imaging system calculated using  the images of test structure A and line spread function (LSF) methodology and using images of  test structure B and edge  response (ER) method. Images were taken using 100x  microscope objective of 0.5 NA for trenches with the  remaining silicon thickness between 0-1 µm and 3 µm.


Image quality is a very strong function of the remaining silicon  thickness.  The range of resolution obtained from the images  acquired for samples with Si thicknesses less than 1 µm ranges


from 400 nm up to 1 µm depending on the exact thickness of  the silicon layer and the wavelength regime chosen for image  acquisition. The resolution dependence on wavelength has a  local minimum that again depends on the Si layer thickness. For the UTS samples a minimum resolution of 400 nm could  be obtained at approximately 600 nm wavelength of the light. For shorter wavelengths the resolution degraded. For thicker Si  layers the resolution was much worse and the minimum existed  at longer wavelengths. For instance, for the sample with a  3-µm thick Si layer inside the trench, the minimum resolution  of 1 µm appeared at around 800 nm wavelength. This behavior  is an effect of the interaction of light with the silicon material. Simple simulations of the first reflection from the air / silicon  interface and the absorption of light in the silicon are presented  in Figure 9. The reflection from the air / Si interface is slightly  dependent on the wavelength in the wavelength regime of the  Si CCD detector. It slightly increases for shorter wavelengths. The exact reflection strongly depends on the quality of the  silicon surface inside the trench and will be worse than the one  shown in the simulations in which the surface non-ideality was  not taken into account. The experiments revealed that  reflection of the light plays no significant role for imaging  through a thin Si layer. For thicker samples (>3 µm) the  amount of reflected light from the imaged structure is small so  that the light reflected from the air / Si interface starts to  dominate, making it difficult to distinguish the features of  interest. In such cases it is necessary to apply an anti-reflective  coating of the proper thickness adjusted to the wavelength  regime of interest.


Figure 9: Simulations of absorption in silicon and the  reflection from the air / silicon interface. The silicon doping  was 1015 cm-3; Si thickness: 1 µm.


Figure 10 shows the simulated ratio of the light coming out of  the structure as a result of transmission into the Si, absorption, reflection from the feature of interest and again absorption to  the light reflected from the air / Si interface before entering the  Si. It is in agreement with the observations. The thicker the Si  layer is, the smaller is the ratio. This is especially the case in  the short wavelength regime where absorption is increasing  exponentially.


Figure 10: Simulation of the ratio of the light transmitted into  the sample, reflected and available for detection to the first  reflection from air / Si interface. The silicon doping was 1015 cm-3.


To show the general average trend of the resolution  dependence on the thickness of the remaining Si layer under  the trench, the resolution calculated from the images acquired  at full spectrum of the detector are shown in Figure 11 as a  function of the Si thickness, separately for the LSF and ER  methods. The smaller the thickness of the silicon is, the better  is the resolution. The resolution here is worse than the best  case seen in Figure 8 as there is no spectrum resolution  performed in this case.


Figure 11: Summary of the resolution measurements obtained  using the entire spectrum of the Si-CCD detector.


Summary and conclusion


A number of trenches were created to check their applicability  for improvement of optical spatial resolution. Various  remaining Si layer thicknesses were achieved. Halogen-lamp  reflected-light images were acquired at various wavelengths, looking at the structures through the remaining silicon in the


created trenches. The improvement in image quality and  resolution improvement were recorded. To get the best  resolving properties of imaging through the backside of the  die, the remaining layer of silicon should be as thin as  possible. The minimum thickness of the silicon is determined  by the device functionality and heat sink issues, as already  studied in [3] and [4]. For samples thicker than approximately  3 µm the reflection from the air / Si interface starts to play  significant role, and deposition of a proper antireflective  coating (ARC) the improve ratio of light coming from the  sample of interest to the reflection from air / silicon interface  should be considered. For thin samples the ARC layer is not  mandatory. The critical thickness depends naturally on the  doping of the substrate and will vary from technology to  technology.  Looking for further resolution improvement, one  has to choose properly the wavelength regime of observation. It should be adjusted to the thickness of the remaining silicon  to perform the imaging in the optimal spectral window.


To summarize, for certain analysis types, device types and  desired resolving properties, parameters such as trench size, remaining Si thickness, trench bottom surface flatness and  quality should be adjusted. In addition, given the thickness of  the remaining Si layer under the trench, deposition of an ARC  layer should be considered and the wavelength regime should  be carefully chosen to get the best resolution, which is a  combined effect of the reflection/transmission, absorption/dispersion and diffraction of light.


We would like to thank Hamamatsu KK, Hamamatsu  Germany, DCG Systems and Infineon Technologies AG for  their support of experiments with equipment, advice and  devices. Special thanks go to Andreas Eckert for device  preparation, Rene Hartmann for bonding, Carlo Pagano for  simulations and discussions and Arkadiusz Jankowski for  helping in data processing and creating the images, all at  Berlin University of Technology.


[1] Jianlei Tao, Peiyuan Fang, Jiaji Wang, “Backside IR  Photon Emission Microscopy (IR-PEM) Observation in  Failure Analysis of the Packaged Devices” ICEPT 2007, pages 1-4


[2] R. Schlangen, R. Leihkauf, U. Kerst, C. Boit, “Functional  IC Analysis Through Chip Backside With Nano Scale  Resolution - E-Beam Probing in FIB Trenches to STI  Level” Proc. ISTFA 2006, pages 376 - 381


[3] R. Schlangen, U. Kerst, A. Kabakow, C. Boit, “Electrical  Performance Evaluation of FIB Edited Circuits Thorugh  Chip Backside Exposing Shallow Trench Isolations” Proc. 16th ESREF (2005) 1544


[4] C. Boit, U. Kerst, R. Schlangen, A. Kabakow, E. Le Roy, R. Lundquist, S. Pauthner, "Impact of Backside Circuit  Edit on Active Device Performance in Bulk Silicon ICs" Proc. 37th ITC (2005) 48.2


# Copper to Aluminum bonding: IMC Characterization through New Mechanical Sectioning Methods


Copper to Aluminum bonding:  IMC Characterization through New Mechanical  Sectioning Methods


Texas Instruments, Tucson, Arizona USA


Dr. Mukul Saran


Texas Instruments, Dallas, Texas USA


Cu wire bonding has had interest in the semiconductor  industry for over two decades [1-7]. Recent increases in the  cost of Gold traditionally used for wire bonding, and advances  in Cu-wire bond technology have driven increasing use of Cu  wire bonds in the semiconductor industry [8-9].  Cu wire  bonding is often stated to be more reliable than Au-bonding  due to very slow intermetallic (IMC) growth with Aluminum  upon aging. This slow IMC growth [11] is due to very low  rates of diffusion of Al and Cu into each other. This is very  different from Au-Al bonding where the intermetallics grow  much more rapidly. Kirkendall voids develop within the AuAl IMC interface due to a difference in the inter-diffusion  rates. Typical estimates of post-assembly intermetallic  thicknesses are ~0.2-0.3µm for Cu-Al bonds. Contrast this  with Au-Al case, where a 1µm thick Al pad is entirely  consumed by the intermetallic formation.


Imaging the intermetallic interface is critical in several areas  including process development, qualification and production  control. For Au wire bonding, this is done routinely.  For Cu  wire bonds the low, Cu-Al intermetallic thickness presents a  challenge in imaging with standard SEM and optical  techniques [10-12]. Accelerated ageing is necessary to  observe the intermetallic formation.  Yet, imaging remains  difficult. Either there is not sufficient contrast to clearly  delineate the growth of the IMC, or worse, sample preparation  artifacts may be misjudged as IMC. Ion-milling the sample  has been used to enhance contrast. However, the degree of  enhancement is rather limited, and depends strongly on the  milling conditions used. Milling artifacts may also confuse the  image interpretation. TEM imaging is possible [11] but can be  complicated and expensive. Additionally, the imaged area is  necessarily limited


This paper presents a new mechanical cross-sectioning  approach that produces an image clarity not yet demonstrated  in published literature. It demonstrates how a critical sequence  of polishing, basic slurry optimization and staining, in  conjunction with correct imaging parameters can be used to  highlight the growth morphology of the IMCs.


Figure 1.  FE-SEM micrograph of CuAl IMC formation  highlighting the detail that can be observed when utilizing the  new sectioning methodology.


Utilizing the above approach, this paper describes the results  of a SEM imaging study of the intermetallic formation & growth at the Cu-Al bond interface during thermal ageing for  up to 4000hrs at 150˚C.  150˚C is a temperature commonly  used to assess reliability of the integrated circuits. Most  previous aging studies have used much higher temperatures (175-250˚C). While these temperatures help accelerate IMC  growth and shorten the duration, the bond interface and its  degradation processes may be non-representative of the  application. Additionally, these studies examine the interface  degradation only indirectly through declining bond-strengths. This paper uses direct SEM imaging to catalog several new  observations which are used to create an initial model for IMC  and void growth at the wire bonded interface.


Another aspect examined in this paper is the effect of  Aluminum splash. It leads to a thinning of Al-pad  metallization under the ball-bond. Since the residual thickness  of Al can be very small (<1000Å) in some regions under the  ball, and with the poor contrast between IMC and Al images, the usual SEM sample preparation techniques are unable to  highlight this interface. A concern exists that the IMC may  debond once it grows down to the barrier-layer underneath the  Al-pad.


Cu Ball Bond


IMC


Al Bond Pad


Cu-wire bonded units were baked in an oven at 150˚C to  create a series of samples representing different durations of  aging, ranging from 0 to 4000 hrs. Multiple units were  decapsulated using an optimized HNO3:H2SO4 acid mix, which avoids damaging the bond-pad metallization and the  Cu-wires. It was verified in other experiments that the use of  this acid mixture does not attack the intermetallics, even after  a several minute long exposure to the mix. Therefore, the  decapsulation process does not affect the conclusions made in  this study.  Ten or more ball bonds on each unit were crosssectioned by chemical mechanical polishing and enhanced for  SEM imaging with the newly developed techniques for  staining and highlighting the intermetallics. Another set of  similar samples were deprocessed to dissolve the bond-pad  Aluminum without attacking the Cu-wire or the IMC. The  under-sides of the lifted ball bonds were examined under the  SEM. IMC morphology, its relationship to Aluminum grain  structure, evolution of the IMC thickness and voids with aging  were studied from both the cross-sectional, and the under  bond images. In addition, the interface between the IMC and  the Al pad barrier-layer under thinned Al bond pad regions  was also examined for evidence of de-bonding.


(a) As-molded Units


Fig 2 shows a highly magnified view of the underside of a Cu  ball. The intermetallics are visible on the surface, with a  morphology that reflects the local growth thickness into the  Aluminum pad. An “island” morphology is evident, with  regions of significant growth separated by flatter regions. Interestingly, island “ring” patterns are seen, which appear to  be imprints of the grain-structure of the Al-pad surface to  which the ball was bonded. The areas enclosed by these ‘rings’ can have an ‘island’ topography or a flat appearance.


Figure 2.  FE-SEM micrograph of the intermetallic formation  as seen on the underside of a Cu bond.


A cross-sectional view in Fig 3, shows that the intermetallic  growth is non-uniform, and there are unalloyed  topographically flat interface regions where Cu and Al do not


intermix at all. However, such areas appear limited in extent. Large areas of the bond show some IMC coverage despite the  variations in thickness.


Figure 3.  Time 0 cross-section of the CuAl IMC interface.


Another feature evident in the pictures is the presence of  vertical grain boundaries in the Aluminum pad. Grainboundaries are generally expected to be paths of rapid  diffusion of Cu in Al. Yet, these images do not show a  preferential Cu diffusion and reaction inside the grain  boundaries. This observation is in apparent contradiction to  the observation of Al grain-boundary imprints under the Cu  balls which suggests a preferential growth of Cu-Al  intermetallics along the grain-boundaries in the Al-pad  surface. Since the samples have seen a only short, hightemperature heat cycle during mold compound cure, there may  be limited diffusion and reaction along the grain-boundaries.  Unbonded Al pads were examined to show the grain-structure  of Aluminum without any wire bond. Figs 4(a) and 4(b) in the  appendix show that the pad-surface contain areas of both  large, columnar grains and smaller, non-columnar grains. This  observation may be relevant to Cu-Al intermetallic growth  topology.


(b) Post-mold Bake Units


Several new features are observed as the samples are baked at  150˚C for 1000 hrs and beyond. After 1000 hrs, no imprints of  Al surface grain-boundary pattern are seen on the underside of  the ball. The IMC at the interface appears less continuous, with an ‘island’ pattern emerging in several areas of the bond. There are visible flat regions where Cu and Al are in intimate  contact but do not show any noticeable IMC growth between  them. A Cu-rich phase becomes evident on the Cu-ball side  where there is a corresponding Al-rich phase growth towards  the Al-pad side. In unbaked samples, this second phase is  barely visible in similar SEM images.  Voids begin to appear  at or above the Cu-Al interface.  Annealing the units to 2000  hrs shows a further growth in the Cu-rich phase thickness; however, the growth stabilizes or may even show a decline at  longer anneal durations.


IMC ring at Al  grain-boundary


“Island structure” grain  consumption


Al grain boundaries


Cu-Ball


Al b/pad


Figure 5.  Graph of the Cu-rich IMC phase thickness in  nm, against time of thermal aging.


Interface voids increase in frequency and size. The islands  observed at 1000 hrs begin to grow laterally and coalesce into  larger islands. Al-rich IMC tends to penetrate deeper into the  Aluminum and maintains its uneven morphology. The balledges tend to form nearly continuous wall of IMC that grows  deep into the Aluminum, ultimately consuming the entire  thickness. In these areas the IMC touches down to the barrier  layers used under Al pad. There is no evidence of de-bonding  to the barrier layer.  See Figures 6(a) 6(b) in the appendix.


DISCUSSION


Based on the observations above, it is possible to construct a  first hypothesis about the processes involved in Cu-Al IMC  growth. The initial bond seems to be a mix of surface weld  regions between Cu and Al and local reactions that lead to  intermetallic formation. It is possible that >170˚C moldcompound curing process used during assembly may add a  diffusion component to IMC growth. Cu tends to diffuse into  Al rapidly along the grain-boundaries, as suggested by the Algrain pattern imprints under the Cu ball. The following figure  shows that IMC formation progresses through complete  consumption of individual Al grains.


Cu diffusion along the grain-boundaries seems to be the  dominant mechanism of transport. Two examples are  presented below that demonstrate IMC growth in regions not  directly accessible to Cu. The first figure shows a ‘boot’


pattern where IMC formation has occurred, leaving out  surrounding Al-grains completely intact.


The second example shows an edge of the Cu ball-bond, where IMC has formed at the base of the Al-splash region, where there is not a direct path for intermetallic growth.


We conclude that growth of intermetallics at the Cu-Al  interface is much more rapid into the bond-pad Aluminum  than into the Cu-ball, but the growth thickness uniformity is  much higher into the Cu-ball. The capability to observe IMC  growth into the Cu-ball is new; TEM images have not readily  highlighted this.


Secondly, we observe that the high non-uniformity of the IMC  thickness into Aluminum pad is related to preferential  conversion of Al grains into IMC’s. The aged ball-bonds  develop an “island” morphology of the intermetallics. With  prolonged bake these islands ultimately coalesce into longer  stretches of continuous IMC.


EDS analysis indicates presence of at least two separate  phases. The Aluminum-rich phase grows unevenly into the  Aluminum bond-pad, while a highly uniform Cu-rich phase  grows into the Cu-ball across the interface. There are regions  where no intermetallics are visible at the interface. A TEM  diffraction analysis is necessary to correctly identify the  various phases.


The SEM x-section images show a slow but clear evolution in  the occurrence of voids at the Cu-Al interface after hightemperature ageing (similar to known Kirkendall voiding in  Au-Al wire bonds).


Cu Bond


Figure 7.  Average number of voids per bond against length of  thermal aging.


Results show that when the intermetallic layer consumes the  entire remaining thickness of the Al-pad and reaches the  barrier metal under the bond, there is no evidence of  debonding at the IMC-to-barrier layer interface. Further  investigation is in progress to see whether the barrier layer  composition would affect the conclusion.


In summary, this new mechanical cross-sectioning approach  has proven to be an effective tool to rapidly study the  formation of Cu wire bonds on Al.  A new level of bond  interface clarity is now available without the cost, size and  cycle-time limitations of TEM.


[1]  Kurtz J, Cousens D, and Dufour M, “Copper wire ball


bonding,”  Proc. 34th Elec Comps Conf, 1984, pp. 1-6.


[2]  Toyozawa K, Oomi S, Minamide S, Wakamoto S, and


Maeda T, “Development technology of copper wire bonding,” Shorp Tech.Journal , vol. 42, pp. 77-80, Sept. 1989


[3]  Hirota J, Machida K, Shimotomai M, and Kawanaka R, “The development of copper wire bonding for plastic molded  semiconductor packages,” in Proc. 35th Electronic


Components Conf., 1985


[4]  Toyozawa K, Fujita K, Minamide S, and Maeda T,


“Development of Copper Wire Bonding Application


Technology” IEEE Trans. On Hybrids and Manuf. Technol


Vol 13, No 4, Dec 1990


[5] Murali S., Srikanth N and Vath C J “ An Analysis of


Intermetallics formation of Gold and Copper Ballbonding on  Thermal Ageing” Mater. Res. Bull.38, 2003, pg 637


[6]  Murali S and Srikanth N, “Acid Decapsulation of Epoxy  Molded IC Packages with Copper Wire bonds,” IEEE


transactions on Electronics and Packaging Manufacturing,


Vol. 29, No. 3, July 2006


[7]  Kim H.J, Lee J Y, Paik K W, Won J, Choe S, Lee J,


Moon J T, Park Y J, “Effects of Cu/Al Intermetallic


Compound (IMC) on Copper Wire and Aluminum Pad


Bondability,” IEEE Transactions on Components and


Packaging Technologies, Vol. 26, No. 2, June 2003


[8]  Deley M and Levine L, “The Emergence of High Volume  Copper Ball Bonding,” KnS Technical Library, 2005


[9] Magno S R C, Ramos J, Pecolera E and Stai C, “Copper


As a Viable Solution for IC Packaging” SMTA International  Conf. 2007


[10] Wulff F W, Breach C.D, Stephan D, Saraswati,, Dittmer  K.J; “Characterisation of intermetallic growth in copper and  gold ball bonds on aluminium metallization “, Proceedings of  6th Electronics Packaging Technology Conference 2004 , pp  348 - 353


[11]  Wulff  F W, Breach C, Stephan D, Saraswati, Dittmer K, Garnier M, “Further Characterization of Intermetallic Growth  in Copper and Gold Ball bonds on Aluminum Metallization,” Semicon Singapore 2005


[12] England L and Jiang T, “Reliability of Cu Wirebonding  to Al Metallization” Electronic Components and Technology  Conference 2007, pp1604-1613


Appendix


Figure 4(a).  T0 Un-bonded Al-pad x-section – Large  columnar grains, with vertical grain boundaries intersecting  the surface are seen, as expected.


Figure 4(b).  T0 Un-bonded Al-pad x-section – Large but  non-columnar grain-structure also exists.


Figure 6(a).  SEM micrograph of an area where the IMC  entirely consumed the Al bond pad.


Figure 6(b).  SEM micrograph of an area where the IMC  entirely consumed the Al bond pad.


# Sample Preparation and Analysis on Full-Thickness Silicon Wafers for Wafer-to-Wafer Bonding Process Development


Sample Preparation and Analysis on Full-Thickness Silicon Wafers for   Wafer-to-Wafer Bonding Process Development


Richard J. Young*, Alex Buxbaum, Corey Senowitz


FEI Company, Hillsboro, Oregon, USA  *email: richard.young@fei.com


C. Deeb


International SEMATECH Manufacturing Initiative, Albany, NY, USA


W.H. Teh


SEMATECH, Albany, NY, USA


Wafer-to-wafer (WtW) bonding is a key capability being  investigated for 3-D integrated circuit (3DIC) technology, the  vertical stacking of multiple processed wafers containing ICs, by electrically connecting them in the z-direction. 3DIC has  been attracting considerable attention because it provides  possible performance improvements by decreasing  interconnect delays and total length, as well as allowing the  opportunity for heterogeneous integration without  compromising form factor. WtW bonding, if optimized  correctly, provides the advantages of a potentially more costeffective process as compared to die-level stacking. In  addition, the use of metallic bonding instead of dielectric  bonding (which requires real-estate for inter-wafer throughsilicon vias connections) allows bonded inter-wafer  connections to have minimal consumption of active device  area [1].


To understand the metallurgy of the bonding and annealing  processes, techniques such as (scanning) transmission electron  microscopy (S/TEM), and electron backscatter diffraction (EBSD) in the scanning electron microscope (SEM), are  commonly employed. However, these electron beam  techniques require direct access to the area to be investigated, which in the WtW samples is buried beneath 750-800 μm of  silicon at the interface of the two wafers. Therefore, extensive  sample preparation is needed to expose the region of interest (and in the case of TEM, thin the sample to electron  transparency, ~100 nm). Using mechanical processes to  section and polish the sample can introduce stresses and  smearing of materials, and so the feasibility of a focused ion  beam (FIB) approach has been investigated.


The focused ion beam (FIB) has become an invaluable tool in  many aspects of semiconductor process development, circuit  edit, low yield analysis, and failure analysis [2]. FIB systems  generally use a gallium liquid metal ion source (Ga-LMIS) as  the source of the ions, providing a typical beam current range  of 1 pA to 20-60 nA. This corresponds to a maximum material  removal rate by sputtering of ~103 μm3/min for silicon at


60 nA of beam current, which enables volumes of a few 10s of μm on a side to be excavated in a reasonable time. Using a  reactive gas (typically halogen based: e.g. I2, XeF2, Cl2) in  addition to the FIB usually enhances the etch rate from 1-15  times [3], but with the combination of XeF2 gas and a silicon  substrate the enhancement can be over 1000 times. This is due  to the reactivity of the gas with Si and enables access trenches  to be drilled even through a full-thickness silicon device for  circuit edit applications [4], or to speed up the sectioning of  large structures such as through-silicon vias (TSV) [5]. Such  an enhancement makes the removal of large volumes of Si  more practical, even with the typical upper end of FIB currents  of 20-60 nA. In this paper we discuss the application of fullthickness silicon trenching to the process development of  WtW bonding.


Wafer-to-Wafer Bonding


The samples investigated consisted of pairs of wafers bonded  face-to-face using an integrated 300 mm bond/align tool. The  make-up of bond/align tool and the details of the bonding  process are described in more detail in Teh et al. [6], and will  just be summarized here.


The 3D fabrication approach starts with M1V1 and M2 copper  metallization process layers completed on two single fullthickness 300 mm bulk-silicon wafers. The V1 and M2  layouts are mirrored to enable these to provide mating  structures for the subsequent Cu-Cu bonding process. The Cu  metallization layers consist of metal lines and vias with ~7kÅ  plated Cu thickness, which was annealed, and then polished  down via CMP to yield a smooth Cu surface prior to bonding. The wafers are then aligned face-to-face and bonded via  thermocompression at ~400°C for 30 mins. The bonding  uniformity was evaluated with scanning acoustic microscopy (SAM), with no evidence of systematic bonding issues  reported. In addition, the overlay alignment accuracy was  measured by IR laser scanning microscopy using a series of  alignment fiducials across the wafers. These results showed a  1 sigma overlay accuracy of ~0.34 μm, resulting in a


corresponding 3 sigma alignment of ~1 μm, meeting ITRS  requirements up until 2012 [6,7].


The bonded wafers included via chain structures, with the Cu  V1 vias ranging from 1 μm to 15 μm in size, mating to M2 Cu  lines with widths ranging from 10 μm to 30 μm. In this paper  we report results on M1V1-to-M2 via chain structures with    3-5 μm size V1 on 30 μm wide M2 lines.


Sample Preparation


The sample preparation within the focused ion beam systems  consisted of four main steps: (1) locating the area of interest;


(2) excavating an access trench; (3) extraction and (4) final  sectioning or thinning of a small piece of sample for  subsequent analysis by TEM or SEM methods.


Equipment Used


While it is possible to imagine steps 1 through 4 (and some  types of final analysis) being carried out in a single tool with  300 mm wafer capability, this proof of concept work was  carried out in two separate preparation systems. Steps 1 and 2  occurred on a V600CE, which is a single-beam FIB system  with 150mm stage, integrated IR and CAD navigation, and  high-speed silicon trenching capability. The trenching used a  patented “co-axial” gas nozzle to provide a high gas flux of  XeF2 at the sample surface to maximize the etch rate. Steps 3  and 4 were then carried out in a Altura™ 855 DualBeam™ FIB-SEM system.


Once the region of interest has been prepared it can then be  transferred to the analysis system for characterization. In this  case, EBSD analysis was performed in a Helios NanoLab™ 600 DualBeam FIB-SEM, and STEM imaging in a Tecnai™ TF20.


Locating and Excavating


The 300 mm sample was first cleaved into a more manageable  size of 30-40 mm on a side, with die close to the center of the  wafer being investigated. The integrated IR camera in the FIB  allowed imaging through the full thickness Si to enable  navigation around the sample based on the metal tracks at the  wafer-wafer interface. A three-point CAD lock was performed  between a CAD database of the layout and IR images in  different parts of the die, enabling CAD polygons to be  overlayed onto the IR images (Fig 1).


device. As a result, a blurred thermal signal emitted from the  TSV sidewall at the opposite site of the defect position found  by emission microscopy could be imaged.  Then, the defocus  was stepwise increased down to 70, 140 and 210μm. The


corresponding LIT results can be seen in Fig. 13.


Figure 13. LIT focus series, upper left: focused on surface, upper right: defocus -70μm, lower left: defocus -140μm, lower right: defocus -210μm


The sharpest hot spot can be seen at 210μm defocus in good  correlation to the result of emission microscopy. The defect is  localized directly at the TSV metallization, Fig. 14. Compared  to emission microscopy, the defect origin could be found more  precisely by high resolution LIT. A further advantage of LIT  in comparison to emission microscopy is that ohmic defects  can also be found. Such defects typically do not produce local  light emission and can not be found by emission  microscopy.


Figure 14 Overlay of LIT topography focused on surface and  LIT amplitude at -210μm defocus, sharp hot spot at  metallization in TSV sidewall indicates the defect position


As a next step in a failure analysis flow, the sidewall of the  defective TSV was investigated by SEM at 36° sample tilt. SEM imaging was performed at 0.8kV acceleration voltage to  avoid sample charging. In agreement with the assumed defect  position, a structural defect could be found at the TSV  sidewall in a depth of 210μm. A detailed SEM image of the  defect visualizes the defect Fig. 15 right.


Figure 15. left: SEM overview of defective TSV at 36° sample  tilt; right: detail of defect located at TSV sidewall


Also for this case we started to evaluate novel preparation  strategies for TSV cross-sectioning. Precise cross-sectioning  is required not only for defect analysis but also for critical  dimension measurements and etch profile characterization. Focused ion beam (FIB) milling is suitable to perform well  aligned target preparation, but standard Ga-FIB is too slow for  cross-sectioning on device level. We present two new  strategies to perform precise cross-sectioning on device level  by enhanced FIB approaches.


In a first approach, we applied Si trenching supported by XeF2  gas chemistry using a new coaxial nozzle design combined  with high current FIB milling at a single beam FIB FEI  V600EC+ system. In a first step, rough milling of a  160μmx120μm box was made using at 65nA ion beam current  and XeF2 gas. Here, the preparation time for rough milling  could be reduced to only 45min. In a second step, polishing  was performed at a maximum current of 67nA for 20min and  finally with 30nA for 5min without using gas injection to  avoid artifacts by chemical reactions and to get a flat surface  of the cross section, Fig. 16.


Figure 16. SEM overview of FIB cross section at 100μm  diameter sidewall-metallized TSV applying Si trench etching


In the second approach, the plasma FIB source from Oregon  Physics was used to perform a top-down cross-sectioning on a  TSV.  The cross-sectioning was made by stepwise slicing with  a extremely high ion beam current of 1μA starting at several  hundred microns from the device edge and using a cleaning  cross-section pattern with 2 min 40 seconds per slice. With  this method, curtaining occurred on the vertical cavity walls, but a smooth wall was received on the bottom. We also tried a  second pattern where we cut a cross-section from the side of  the via using a 150 bias angle with respect to the wafer edge.  After FIB cross sectioning, the TSV sidewall could be imaged  by SEM to investigate its metallization/isolation layer stack. This investigation is only demonstrated for reference TSVs  here, see Figs. 17-18. In future work we will also apply  enhanced FIB cross sectioning to get access to defect sites as  found by emission microscopy or LIT.


Figure 17. SEM overview of TSV cross section made by  plasma FIB, top left: top down milling starting at cleave etch, top  right: Via cut through the perimeter


Figure 18: SEM image of TSV sidewall layer stack taken from  FIB cross section


To improve the quality and reliability properties of 3D  integrated components, it is not only necessary to detect a  failed device or to localize the failed structure, but  determining the detailed root cause of the failure mechanism  is also essential. This paper presents novel tools for the failure  analysis of current silicon integration processes. The  application and beneficial potential is demonstrated for two  different case studies including an interconnecting technology  utilizing Ni microinsert interconnects between two Si dies and  sidewall metalized through silicon vias. In the  first case study  on Ni microinserts, the benefits of using LIT as the first step  of the failure analysis flow for non-destructive defect  localization in 3D integration samples were shown. Even  high-resolution thermal imaging through the top Si die to  detect highly resistive Ni interconnects directly in the bonded  interface was demonstrated. The isolated failed interconnects  were subsequently prepared in cross-section using a currently  developed combination of fast laser-based ablation and highly  accurate FIB technique. This procedure allowed to detect  incomplete bonding between the Ni microinserts and the  metallization of the top Si die and to attribute these defects as  the root cause for the increased ohmic resistance of failing  interconnects. Due to its significantly increased milling rates, the combined laser/ FIB preparation routine offers new  capabilities in terms of speed and efficiency for SEM failure  analysis in such vertical interconnects. As a result, a new FIB  demonstrator with a high-current ion-beam column and  integrated laser ablation is under construction.


In a second case study, sidewall-metalized (unfilled) TSVs  were investigated. Again, LIT was successfully demonstrated  to localize the origin of short defect between TSV  metallization and Si substrate. Thus, it could be shown that  LIT is a powerful technique to localize electrical defects in  TSV structures with high accuracy in x, y and z directions. For target preparation, we applied Si trench etching based on  high current Ga FIB milling cross sections supported by  chemical etching by XeF2 gas injection. Preparation of the   whole TSV structure can be achieved in an acceptable time. In


addition, new plasma FIB sources producing ion beam  currents in μA range provide promising novel techniques for  sample preparation on 3D device level with high potential for  3D integration as an alternative to laser ablation and gas  chemistry etching.


As a result, the novel material diagnostics methods applicable  for 3D integration specimens can, in the future, provide  significantly improved analysis throughput and efficiency. They may be advantageously used with respect to technology  development and reliability issues for 3D integrated devices.


Parts of these results were derived within the FULL  CONTROL research project running within the European  EURIPIDES-EUREKA research program and within the ESIP  project running within the ENIAC initiative. The authors  gratefully acknowledge financial supports by the German  BMBF for both these projects, and a grant from the European  commission for the ESIP collaboration. In addition, the  authors would like to particularly Antoine Nowodzinski from  CEA-LETI for providing the Ni microinsert samples, Stefan  Martens from Infineon Technology AG, Holger Dömer from  Carl Zeiss NTS and Bernard Rasser from Orsay Physics for  their contributions in developing the target preparation  approach based on laser/FIB combination.


[1] L. Di Coccio et al.,  SET Techn. Bullet.,  6-9, (2009)


[2] Mathewson, A., Brun, J., Ponthenier, G., Franiatte, R.Nowodzinski, A., Sillon, N., Poupon, G., “Detailed  characterisation of Ni microinsert technology for flip chip  die on wafer attachment,” Proceedings of the 57th IEEE  Electronic Components and Technology Conference (ECTC), 2007, pp. 616-621.


[3] J. Kraft, A. Hueber, S.Carniello, F.Schrank, E.Wachmann, Passivation Integrity Investigations for  Through Wafer Interconnects, Proceedings – International Reliability Physics Symposium, pp 506-509,


2008.


[4] Schmidt, C., Große, C., Altmann, F., “Lock-inThermography for 3- dimensional localization of  electrical defects inside complex packaged devices,“ Proceedings of the 34th Symposium for Testing and  Failure Analysis (ISTFA), 2008, pp. 102-107


[5] Chr. Schmidt et. al:  “Failure analysis of stacked-die  devices by combining non-destructive localization and  target preparation methods, ISTFA 2009, San Jose USA


[6] Rue, C., Herschbein, S., Scrudato, C., “Backside circuit  edit on full-thickness silicon devices,” Proceedings from  the 34th International Symposium for Testing and Failure  Analysis (ISTFA), 2008, pp. 141-150


[7] Tesch, P., Smith, N., Martin, N., Kinion, D., “High  current focused ion beam instrument for destructive  physical analysis applications,” Proceedings from the 34th


International Symposium for Testing and Failure Analysis (ISTFA), 2008, pp. 7-13.


[8] Martens, S., Mack, W., Courtade, F., Perdu, P., Wilde, J.,Voelklein, F., “Laser-based target preparation in 3D  integrated electronic packages,” ASME Journal of  Electronic Packaging, Vol. 131, No. 3 (2009), 0310061


[9] S. Martens, Ph.D. thesis (to be published in 2010)


[10] Martens, S., Fink, M., Mack, W., Voelklein, F., Wilde, J.,“Simulation-based analysis of the heat-affected zone  uring target preparation by pulsed-laser ablation through  stacked silicon dies in 3D integrated System-inPackages,“ Proceedings of IEEE International Conference  on Thermal, Mechanical and Multiphysics Simulation and  Experiments


in


Micro/Nanoelectronics


Systems(EuroSimE), Bordeaux, France, April 2010.


[11] M. Petzold et. al. “Micro Structure Analysis for System in  Package Components - Novel Tools for Fault Isolation, Target Preparation, and High-resolution Material  Diagnostics”, Proceedings of the 60th IEEE Electronic  Components and Technology Conference (ECTC), (2010) pp. 1296-1302


[12] C. Cassidy et. al: Characterization of wafer bonded  devices and unfilled Through-Silicon-Vias (TSVs), ISTFA 2008, Portland USA


[13] C. Cassidy, F. Renz, J. Kraft, F. Schrank, Depth-resolved  Photoemission Microscopy for Localization of Leakage  Currents in Through Silicon Vias (TSVs), Proceedings - IPFA (2009) 735-740


# A Novel Junction Profiling Methodology


A Novel Junction Profiling Methodology


Micron Japan, Ltd.


302-2. Hirano-cho Nishiwaki-city. HYOGO. 677-0063 JAPAN


Phone: +81.795.23.6621 Fax: +81.795.23.6637 E-mail: tnakai@micron.com


Currently many methods are available to obtain a junction  profile of semiconductor devices, but the conventional  methods have drawbacks, and they could be obstacles for  junction profile analysis. This paper introduces an anodic wet  etching-based two-dimensional junction profiling method, which is practical, efficient, and reliable for failure analysis  and electrical characteristics evaluation.


Two-dimensional junction profiling of semiconductor devices  is needed for failure analysis and electrical characteristics  evaluation, but it becomes very difficult due to continuous  device scale down.


Currently many methods are available to obtain a twodimensional junction profile, but the conventional methods  have drawbacks and advantages. For example, Scanning  Capacitance Microscopy (SCM) is widely used for junction  profiling, and it is a good technique because it can distinguish  between P-type and N-type regions and the carrier  concentration resolution is very high. However, the spatial  resolution is not so good, and it is difficult to see precise  profiles. Moreover, SCM and other scanning probe techniques  like Scanning Spreading Microscopy (SSRM) require good  sample preparation and they lead to low throughput. Wet stain  with TEM is also a general technique and its spatial resolution  is very good. However, the sample-to-sample reproducibility is  bad because the profiling results strongly depend on a variety  of parameters, such as etching time, temperature, chemical  condition, and so on.


Thus, conventional junction profiling methods have some  drawbacks, like low spatial resolution, low throughput, high  cost, and so on. They could be obstacles for junction profile  analysis, therefore we were seeking a good method for twodimensional junction profiling.


In this paper, an anodic wet etching-based junction profiling  method, which is practical, efficient, and reliable for failure  analysis and electrical characteristics evaluation, is reported.


Experiments


Fig. 1 shows a junction delineation flow of the anodic wet  etching-based junction profiling method. In this method, a  common FIB, a micro manipulator, Buffered Oxide Etch (BOE), and a power supply are used for sample preparation.


The use of FIB and micro manipulator enables us to observe a  site specific junction profile with high throughput (about  1h/sample). After sample thinning and bottom cut by FIB (Fig. 2), anodic wet etching is performed (Fig. 3). Anodic wet  etching is destructive so the sample thickness after FIB  thinning needs to be at least 0.1-0.2µm. Tetra-methyl  ammonium hydroxide (TMAH, 20%) treatment is added after  anodic etching, which is the key point of this method.


Fig. 1  Junction delineation flow


Fig. 2  Sample after FIB thinning and bottom cut


Fig. 3  Anodic wet etching


Fig. 4 shows sample images after a side cut. The sample is  picked up by micro manipulator to Cu mesh for STEM  observation (Fig. 5).


This method does not need special equipments so it is very  cost-effective and easy to perform.


Fig. 4  Sample after side cut


Fig. 5  Sample pick up by micro manipulator


Si Etching Mechanism


In aqueous HF solution, various chemical reactions occur  dynamically on Si surface. They are complicated and difficult


to understand. The exact Si etching mechanism is still in  question; however, it is generally accepted that Si etching in  HF(aq) is initiated by hole[1]. One of the main Si dissolution  reactions is shown in Fig. 6.


Fig. 6  Si dissolution in HF


Si surface consists of “SiH” hydride bond in HF(aq) and it  is displaced by “SiF” fluoride bond with electron – hole  exchange first. The subsequent reactions with HF(aq) finally  product H2SiF6 and it dissolves in solution.


Si dissolution oxidation reaction is accelerated on anodic  polarization condition. The reactions on anode and cathode are  written below [1][2].


Anode:   Si + 6HF + 2h+  H2SiF6 + H2 + 2H+


Anode:   Si + 2H2O + 4h+  SiO2 + 4H+


(2)


Anode:   SiO2 + 6HF  H2SiF6 + 2H2O


Anode:   SiO2 + 4HF  SiF4 + 2H2O


(4)


Anode:   SiF4 + 2HF  H2SiF6


(5)


Cathode:   2H+ + 2e-  H2


(6)


As mentioned above, hole initiates Si dissolution reaction in  HF like Eq(1). Si dioxide may be formed with holes and H2O  as in Eq(2), and it can be dissolved by HF like Eq(3) and (4). Eq(4) generates SiF4 and it reacts with HF again and dissolves  in solution as H2SiF6 (Eq(5)).


On cathode, reduction reaction occurs and hydrogen gas is  generated like Eq(6).


Fig. 7 explains Si etch-rate dependency on anodic wet etching


[3]. Si etch-rate is faster at higher carrier concentration region  due to higher conductivity, and P-type Si is usually faster than  N-type because hole is majority carrier on P-type


Fig. 7  Si etch-rate dependency on HF anodic etching [3]


1016


1020


ND


NA


p+


pn


nn+


Fig. 8 compares 90nm DRAM NMOS with and without  TMAH treatment.


Fig. 8  Comparison of w/o TMAH and w/ TMAH


By adding TMAH treatment after anodic wet etching, Si at  S/D region is etched away and a clear junction profile is  obtained. The junction profile is well-matched with the  simulation result (see Fig. 9) On the other hand, a clear  junction profile cannot be obtained without TMAH treatment. As a result of our experiments, the success rate for junction  profiling is about 90% with TMAH and 0% without TMAH. TMAH dip has a strong influence for reproducibility and  carrier concentration resolution.


Fig. 9  Comparison with simulation (90nm DRAM NMOS)


Fig. 10 explains TMAH influence for junction profiling in this  method. After anodic etching, hydride bond is rich on higher  carrier concentration region due to porous Si formation [4]. The hydride bond is very active for chemical reaction, so Si  dissolution is accelerated by TMAH dip at higher carrier  concentration region.


Fig. 10  TMAH influence for junction delineation


Fig. 11 shows a junction profiling result for 90nm DRAM  PMOS. The obtained PMOS junction profile is also wellmatched with simulation result.


Fig. 11  Comparison with simulation (90nm DRAM PMOS)


Fig. 12 is a junction delineation result for 50nm DRAM  NMOS. The profile is very clear, and we can conclude that  this method shows high enough spatial resolution and is  effective even for leading-edge devices.


Fig. 12  S/D  delineation for 50nm DRAM NMOS


This method can delineate Nwell and Pwell profile as well. In  case of well delineation, longer anodic wet etching is  necessary because the carrier concentration of a well is low  and selective Si dissolution reaction hardly occurs at short  time. TMAH dip time is constant regardless of carrier  concentration. Fig. 13 is a result of well delineation. Pwell is  etched deeper than Nwell so the contrast is brighter.


Fig. 13  Well delineation


The anodic etching-based junction profiling method was  actually applied to an implant-related issue of 110nm DRAM. We could narrow down the failing location to a specific  transistor by photo emission microscopy and passive voltage  contrast technique (Fig. 14), but FA resulted in non-visual on  standard SEM/STEM inspection.


As a result of junction profiling analysis, we could find  abnormal N-type region of low carrier concentration between  N+ and Pwell (see Fig. 15). The dopant profile is wellmatched with the SCM result, and this means that the anodic  etching-based junction profiling method has pretty good  performance for carrier concentration resolution.


Fig. 14  PEM and PVC results for 110nm DRAM


Fig. 15  Failure analysis result for 110nm DRAM


Two-dimensional junction profiles of NMOS/PMOS were  successfully obtained by the anodic wet etching-based junction  profiling method, and we succeeded in applying this method to  failure analysis. This junction profiling method shows good  performance for spatial resolution, carrier concentration  resolution, observation capability in the specific site, throughput, reproducibility, and cost. We think that this is the  best method for two-dimensional junction profiling.


I would like to thank Masanobu Kumazaki and Hajime  Furusawa for providing important data.


[1] R. L. Smith and S. D. Collins, “Porous silicon formation  mechanisms”, J. Appl. Phys., Vol. 71, No. 8, 15 April  1992


[2] Ng Sea Chooi and Ng Jou Ching, “Dopant Delineation: Novel Technique For Silicon Dopant Implantation  Defects Identification”, Proceedings of 9th IPFA 2002, Singapore


[3] C. J. M. Eijkel, J. Branebjerg, M. Elwenspoek, and F. C. M. van de Pol, “A NEW Technology for Micromachining  of Silicon: Dopant Selective HF Anodic Etching for the  Realization of Low-Doped Monocrystalline Silicon  Structures”, IEEE ELECTRON DEVICE LETTERS, VOL. 11, NO. 12, DECEMBER 1990


[4] Kimura Yasuo, Hosoi Yoshinobu, Ishii Hisao, Niwano  Michio, “In-situ Observation of Electrochemical Etching  Processes of a Silicon Surface Using Infrared Absorption  Spectroscopy in Multiple Internal Reflection Geometry”, Journal of the Surface Science Society of Japan  25(2)  pp.84-90 20040210


# Improvement of optical resolution through chip backside using FIB trenches


Improvement of optical resolution through chip backside using FIB trenches


Arkadiusz Glowacki, Clemens Helfmeier, Uwe Kerst, Christian Boit


aglowa@mikro.ee.tu-berlin.de, Einsteinufer 19, Sekr. E2, D-10587 Berlin, Germany, phone: +49-30-314-24922  fax: +49-30-314-25526


CNES, Toulouse, France


Optical spatial resolution improvement using local focused ion  beam (FIB) assisted silicon material removal was investigated. Two types of test structures were chosen for imagingresolution characterization to be able to use two ways of  measuring resolution. Samples of various remaining bulk  silicon thicknesses were prepared and characterized in terms of  image quality and spatial resolution. The resulting remaining  bulk Si thickness was measured using reflectance  spectrometry. Images were acquired using halogen-lamp  illumination and reflected light detection using a cooled SiCCD detector. To investigate the image quality at various  wavelengths, a set of interference band-pass filters was  applied.


Nowadays, FA techniques like laser stimulation (LS) and  photon emission microscopy (PEM) are mostly applied through the backside of the chip as a result of common flipchip packaging and presence of many layers of metallization  on the frontside of the chip [1]. The efficiency of optical  techniques such as reflected light imaging, LS or PEM  depends strongly on the thickness of the bulk silicon material, the doping of the substrate and the quality of the back surface. There are three phenomena that affect efficiency of the  analysis from the backside: absorption, dispersion and  reflection of light. Short wavelength light having energy above  the silicon band-gap energy is strongly absorbed through bandto-band absorption. The less energetic photons can penetrate  the material better, but are still being absorbed on free carriers (intra-band absorption). This absorption is a strong function of  the material doping. For modern technologies, the doping is  increased to decrease the short channel effects, which makes  analysis through the backside of the chip more complicated. Light that is not absorbed in the bulk material is dispersed, which in turn degrades the resolving properties of techniques. The last phenomenon determines the amount of light that is  transmitted into the medium where the other two phenomena  are happening, namely the reflection on the air / silicon  interface. This is very much dependent on the quality of the


back surface. It is very important to have a surface that enables  good transmission of light through this interface.


To improve the quality of a particular analysis from the  backside, in terms of resolution and general efficiency, it is  crucial to thin the silicon substrate material as much as  possible to minimize absorption and dispersion effects and at  the same time produce a surface that minimizes reflection of  light. Similar activity aiming at obtaining ultrathin silicon (UTS) has already been performed to enable application of  particle beam techniques like e-beam probing (EBP) [2]. The  aim of this study was to perform local silicon material removal  with special focus on controlling the remaining silicon layer  thickness and good trench bottom planarity and to characterize  qualitatively and quantitatively the properties of reflected light  images acquired through the created trenches.


To enable backside analysis and further processing, the wafer  was diced and the pieces of interest were mounted, bonded and  encapsulated in SBGA packages. Prior to any FIB processing, the dies were mechanically thinned down to approximately 25 µm of remaining bulk silicon material. Further processing was  performed by FIB. The FIB system used in this study was  OptiFIB of DCG systems. The typical procedure consisted of  the steps presented in Table 1.


Table 1: Typical FIB procedure for backside Si removal.


Step #


Activity


Si surface cleaning.


Combination of ion unassisted


and metal (iodine gas assisted) etch steps


Bulk Si removal.


High etch rate process using XeF2 gas


Sample rotation


Bulk Si removal


Final Si removal. Slow etch rate process for  surface quality improvement


ARC deposition (optional)


At first, the location chosen for further trenching was cleaned  using a combination of unassisted ion etch and metal (iodine


gas assisted) etch.  The next step was a high etch rate XeF2 gas  assisted etch. As the OptiFIB system used in the experiments  has one jet for gas delivery, the sample had to be rotated at  some point in the trenching procedure to compensate for  etching inhomogeneity. Another high etch rate was performed  after that. The exact durations of the high etch rate steps before  and after rotation of the sample were adjusted taking into  account the original silicon backside surface slope, and the  desired remaining silicon thickness X, as indicated in Figure 1. The last step was a short slow etch rate XeF2 gas assisted etch  used to improve the silicon surface quality. Optionally, an  antireflective coating (ARC) could be deposited whenever  desired using the endpoint detector to monitor the reflection  from the air / Si interface.


Figure 1: Principle of FIB trenching in the backside of the  silicon die.


Resolution measurement methods


There are several methods one can use to characterize the  resolving properties of an imaging system using the images of  certain features acquired with this system. Among others, there  are line spread function (LSF) and edge response (ER). Line  spread function is the response of the system to a thin line  across the image. Similarly, the edge response shows how the  system responds to a sharp straight discontinuity (an edge). Using LSF, the resolution can be defined as the width at which  the LSF decreases to the half of the maximum value, so called  Full Width at Half Maximum (FWHM). The parameter  characterizing the resolving properties using ER is the distance  required for the edge response to rise from 10% to 90% as also  indicated in Figure 2.


Two types of test structures were used so that both methods  could be applied.


Figure 2: Resolution measurement methods: line spread  function (LSF) and edge response (ER).


Test structures


Two types of test structures were used in the experiments. The  chip was manufactured by Infineon Munich in 120-nm  technology. Test structure A presented in Figure 3 incorporates  numerous repetitive components manufactured as highly doped  diffusions in silicon. The spacing between the diffusions is 440  nm. This structure will be used later to calculate resolution of  the optical images using the line spread function (LSF).


Figure 3: Structure A - very highly doped diffusion regions.


Test structure B consisted of metal lines of various widths  starting from 0.8 µm up to 4 µm as presented in Figure 4.


Figure 4: Structure B – metal lines.


Optical characterization setup


The system used to perform FIB milling was DCG System  OptiFIB. The setup (system) used for characterization of the  optical properties of prepared samples was an LS/PEM  Phemos 1000 system equipped with a halogen lamp having a  broad spectrum ranging from UV to infrared, a microscope  and cooled Si-CCD camera. For inspection at various  wavelengths, a set of band-pass interference filters was used in  the spectral regime of the Si-CCD detector, with the central  wavelength (CWL) ranging from 450 nm to 950 nm and the  bandwidth from 40 nm to 70 nm. In addition, a built-in  backside analysis function of the system was used, which in  turn used a band-pass filter of 1100 nm CWL and bandwidth  of 50 nm. The quantum efficiency of the Si-CCD detector and  the convoluted transmission characteristics of the filters and  detector are presented in Figure 5. The images were taken with  20x and 100x IR microscope objectives, but only 100x images  were used for resolution measurements.


Figure 5: Quantum efficiency of the Si CCD detector and the  convolution of filter transmission characteristics and detector  efficiency.


Experimental results


After the trenches had been created, the remaining bulk Si  thickness was measured using a Filmetrics reflectance  spectroscope and an optical bench equipped with an IR 20x  magnification Mitutoyo microscope objective. To facilitate  measurements inside the trenches, the trenches had to be big  enough to make it possible to focus on the bottom inside of the  trench. Dimensions of the trenches were 200 µm x 200 µm.


However, given the surface flatness of the trench bottom, the  surface quality, and the low level of the reflected-light signal, thickness measurements below 1 µm were not possible. The  summary of trenches used in this study is presented in Table 2. Table 2: Summary of trenches.


Trench #


Remaining  Si thickness


Test  structure


Resolution  measurement


method


1-6


0-1 µm


LSF


7


1.5 µm


ER


8-9


2 µm


2.5 µm


11


3 µm


For reference purposes, the resolving properties of the optical  microscope system were evaluated using test structures  consisting of metal lines having 0.8 µm, 1 µm, 2 µm and 4 µm  widths. Under these structures the silicon was completely  removed by FIB so that there was no additional modulation of  the resolution as a result of the interaction of light with the  silicon material. The images were acquired using the filters for  spectral information resolution. The spatial image resolution  was calculated using the ER method applied to the intensity  profiles read from the detected reflected light images. The  results of these measurements are presented in Figure 6.


The sample can translate between IR position and FIB milling  position with an accuracy of ~3 μm. So, even though the FIB  is effectively blind when it comes knowing its location relative  to the wafer-wafer interface, it can go ahead and create a  trench based on the IR image, confident in the knowledge that  the area of interest will be properly located once all the Si is  removed. To allow for sample extraction in the dual-beam  system it is necessary to provide access onto the wafer-wafer  interface for the SEM, FIB and extraction needle. The  geometry used is shown in Fig 2, which is a 30° tilted view. The total volume removed is estimated at ~2 108 um3.


Figure 1: IR image through full thickness silicon wafer with  CAD polygons overlayed. The area is centered on 5 μm (left) and 3 μm (right) via test structures. Field of view is 96 μm. The red box outlines metal2 (upper wafer), the purple is  metal1 and the blue is the interconnecting via (lower wafer).


Figure 2: SEM image showing the final trench used for the 5 μm via sample. The main trench consists of an access window  of approx 200x200 μm where all the silicon on the upper  wafer has been removed, with two side trenches that provide  access for the FIB and extraction needle in the dualbeam.


The excavation of the trench was performed with an ion beam  current of 21 nA and a chamber pressure rise due to the XeF2  gas of ~2.2 10-5 mbar. The pressure at the sample due to the  confined coaxial nozzle design (Fig. 3) is considerably larger, probably of the order of 10-1 or 10-2 mbar. The hole in the  needle has an inner diameter of 350 μm, so to make such a  large structure the patterning had to be broken down into a  number of individual steps. The patterns were designed such  that the central part of the trench went fully through the  silicon, while the side trenches were more angled to reduce the  amount of material removed.


Figure 3: Coaxial gas nozzle used for fast Si trenching with  XeF2 etch gas. Distance from nozzle to sample is exaggerated  for clarity – typical distance is 50 μm, much less than the 350 μm hole in the nozzle through which the FIB accesses the  sample surface.


The total mill time to create the complete trench was 170  mins, with ~75 mins of additional overhead due to navigation, setup and inspection of the side trenches to determine where  material was obscuring the required angled access into the  main area. Further optimization is certainly possible, reducing  the overhead and fine tuning the milling process to remove the  minimum amount of material to give the required access.


During milling both the specimen current flowing to ground  and the secondary electron signal at the detector are  monitored. Once the passivation below the upper Si substrate  is reached these signal give a characteristic dip (Fig 4), enabling milling to be stopped before any appreciable erosion  of the passivation takes place. During the time spent  completing the side trenches the XeF2 continues to etch the  central area without direct ion beam exposure, resulting in the  central area opening up to a ~200 by 200 μm area (Fig 5). This  figure also shows that passive voltage contrast can be used to  identify the locations of the buried metal lines.


Figure 4: Endpoint trace of the final 9 mins of milling the  main trench – the trace shows detector signal versus time, with a characteristic dip in signal once the silicon dioxide  passivation is reached.


With the trench floor exposed, direct sectioning and imaging  of the interconnects is possible. Results from this will be


covered in the Analysis Results section of the paper, so in this  section we’ll complete the sample preparation for TEM or  EBSD.


Figure 5: FIB image of window opened into silicon dioxide, showing CAD overlay. The secondary electron image shows a  passive voltage contrast effect, enabling the location of the  buried metal traces to be seen.


Final Preparation for TEM or EBSD


Once the access trenches were in place the sample was  transferred to the dual-beam system for a standard sample  extraction and TEM sample preparation.


The only change to normal operation was the re-alignment of  the gas-injection system needle for deposition to be 800 μm  higher than normal, so that the needle could still be inserted  with the wafer-wafer interface positioned at the coincident  point of the FIB and SEM beams. In the standard setup, the  needle is 100-150 μm above the coincident point and so for  this type of sample the upper wafer would have interfered with  it being inserted. In the higher position, the gas flux at the  sample surface is lower than normal, so the deposition  parameters were adjusted to allow more time to build up the  protective layer used during the TEM sample preparation. In  addition, it was important to use the through-the-lens detector (TLD) for secondary electron imaging as the normal inchamber detector was obstructed by the high aspect ratio of  the trench. The preparation for EBSD was similar, but in this  case the sample was not thinning to electron transparency.


Analysis Results and Discussion


FIB and SEM-EBSD Analysis


As noted earlier it is possible to directly inspect the  interconnects at the bottom of the trench using FIB or SEM  imaging. The FIB can be used “top-down” to open up  windows in the trench floor to inspect the relative alignment  of the metal lines and vias [6]. Sections can also be made to  expose the bonded interface. FIB imaging shows strong


channeling contrast that enables the grains in the copper to be  directly observed (Fig. 6).


Figure 6: FIB image of cross-section through 5 μm via  interconnect after bonding (no annealing). Channeling  contrast enables the grain structure of the Cu to be directly  viewed. The red arrows indicate the position of the original  bond interface (in this case the M2 wafer is on the bottom). Sample tilt 42°.


In the SEM, EBSD provides more detail information on the  grain structure than FIB or SEM imaging alone [8]. The  detector geometry required for this technique precludes it from  being used down inside the trench, but using a similar  extraction process as that used for TEM preparation allows a  sample to be oriented in the SEM (or dual-beam) for EBSD  analysis. Results from one of the 5 μm via structures are  shown in Fig 7.


TEM analysis


TEM analysis was carried out on both 3 and 5 μm via  structures with results shown in Figs 8. The EBSD and TEM  data both indicate that some Cu grain growth had taken place  during the bonding/annealing process, with grains now  spanning across the line of the original interface. This can be  contrasted with the M1V1 interface, where there is a distinct  horizontal interface at the barrier interface. In addition, no  voids were observed at the bond interface.


It should also be noted that once the trench has been prepared  it would be possible to do the final sample preparation and  analysis on several locations within the trench.


With the increase in 3DIC it is expected that new process  characterization and failure analysis techniques will be  required. The work presented here shows the feasibility of  extending FIB techniques to the process development of  wafer-to-wafer bonded samples even on full-thickness wafers.


Further optimizations to the process are certainly possible. These could include combining the techniques into a 300 mm  wafer system, so that the full sample preparation process could  be accomplished on a single system. Faster processing times  could also be investigated using larger FIB currents – e.g. by  increasing the current from 21 nA to the 65 nA now available  on some systems, or by utilizing a “plasma FIB” column based  on an inductively coupled plasma (ICP) ion source where  beam currents of 1 μA or more are possible [9]. Alternatively, other techniques such as localized mechanical or laser  chemical etching (LCE) [10] could be employed for the first  part of the trench created thereby reducing the volume of  material needed to be removed by the FIB.


Figure 7: Orientation map obtained using EBSD of 5 μm via after bonding and annealing processes. Each color refers to a particular  Cu grain orientation. The color orientation map is overlayed with the EBSD “image quality” map which highlights the grain  boundaries with darker contrast. The red arrows indicate the position of the original bond interface. (Note - standard EBSD data  cleanup techniques were used to process the raw data to produce this composite image).


Figure 8: STEM image of 3 μm (a & b) and 5 μm (c & d) via  interconnects after bonding and annealing. (b) and (d) are  more detailed views (all images 200 kV HAADF mode). The  red arrows indicate the position of the original bond interface  in the overview images.


Chad Rue and Kimball Skinner (FEI Company) are  acknowledged for their assistance and advice with the  V600CE navigation and trenching. Versions of Figs. 1, 4, 7, 8d appear in Teh et al. [6].


[1] P.R. Morrow et. al., “Three-Dimensional Wafer Stacking  Via Cu-Cu Bonding Integrated With 65-nm StrainedSi/Low-k CMOS Technology,” IEEE Elec. Dev. Lett. 27(5), p. 335, 2006.


[2] For an overview on FIB techniques see, for example, Introduction to Focused Ion Beams: Instrumentation, Theory, Techniques, and Practice, eds. L.A. Giannuzzi  and F.A. Stevie, Springer (New York 2005)


[3] R.J. Young et al., “Characteristics of gas-assisted focused  ion beam etching”, J. Vac. Sci. Technol., B 11 (2), 234 (1993).


[4] C. Rue et al., “Backside Circuit Edit on Full-Thickness  Silicon Devices”, ISTFA 2008: Conference Proceedings  from the 34th International Symposium for Testing and  Failure Analysis, pp141-150 (2008)


[5] P. Gounet et al., “Failure Analysis of Through-SiliconVias Aided by High-Speed FIB Silicon Removal”, Proceedings of 16th IPFA, pp94-99 (2009)


[6] W.H. Teh et al., “Recent Advances in Submicron  Alignment 300 mm Copper-Copper Thermocompressive  Face-to-Face Wafer-to-Wafer Bonding and Integrated  Infrared, High-Speed FIB Metrology”, Proceedings of  13th IEEE International Interconnect Technology  Conference, (2010).


[7] 2007 ITRS Roadmap - Interconnect Emerging  Technologies Section


[8] See for example: Electron Backscatter Diffraction in  Materials Science, eds. A Schwartz et al., Springer (New  York, 2009)


[9] S. M. Kellogg et al., “A system for massive, rapid  material removal for device analysis in monolithic 3D  integrated circuits”, Presented at EIPBN Conference (2009).


[10] M. Paniccia et al., “Novel Optical Probing and  Micromaehining Techniques for Silicon Debug of Flip  Chip Packaged Microprocessors”, Microelectron. Engin. 46, pp27-34 (1999).


# Application of Lock-in Thermography on PCB for Fault Localization and Validation of Failure Mechanism Due to External Discrete Component Variation


Application of Lock-in Thermography on PCB for Fault Localization and


Validation of Failure Mechanism Due to External Discrete Component Variation


William Ng


Kevin Weaver


Zachary Gemmill


National Semiconductor


2900 Semiconductor Drive  Santa Clara, CA 95051


Herve Deslandes  Rudolf Schlangen  DCG Systems


45900 Northport Loop East


Fremont, CA 94538


This paper demonstrates the use of a real time lock-in  thermography (LIT) system to non-destructively characterize  thermal events prior to the failing of an integrated circuit (IC) device. A case study using a packaged IC mounted on printed  circuit board (PCB) is presented. The result validated the  failing model by observing the thermal signature on the  package. Subsequent analysis from the backside of the IC  identified a hot spot in internal circuitry sensitive to varying  value of external discrete component (inductor) on PCB.


The design of an IC must follow a set of specifications. Among other things, the design fulfills product requirement  and operating conditions such as power rating, input  characteristics and output loading etc. External discrete  components are used in conjunction for optimal IC operation  in real life applications. Varying the values of these external  components could adversely affect the operation of the IC and  cause unexpected results.


As it applies to failure analysis (FA) of IC, the scope of the  analysis should include the effect from these discrete  components. For example, when analyzing the root cause of  electrically an overstressed (EOS) IC, massive carbonized  epoxy indicates excessive heat dissipation. The excessive heat  could be the result of non-standard use of external discrete  components on PCB which affect the performance of the  subject IC. The cause of failure is often hypothesized as the  subject device was so severely damaged that the events  happened during the failing condition could hardly be  determined. To validate the hypothesis, a mechanism of failure


and its conditions are established and subsequently applied to  known good devices for information that explains the failure.


This paper describes the use of a lock-in thermography (LIT) system to characterize thermal events prior to the failing of an  IC device. The methodology was applied on an IC installed on  PCB with few other discrete components. The purpose was to  check the effect of using different values of a specific on-board  discrete inductor that would result in any thermal signature of  the IC prior to the failure. As EOS typically closely associates  with thermal events, observing thermal distribution from an  operating IC would provide insight into the cause of failure.


Lock-in Thermography


One of the advantages of a LIT system compared to a  conventional (steady state) thermal detection system is an  improved signal-to-noise ratio of a few orders of magnitude (µK range instead of mK range) [1]. The underlying  methodology of the pixel-wise real-time lock-in is depicted in  Figure 1.


Figure 1: Pixel-wise real-time lock-in methodology


The defect or thermally active circuitry area needs to be  periodically activated with a lock-in frequency (flock-in) to  facilitate the lock-in methodology. The utilized infrared (IR) camera with spectral response ranged between 3µm and 5 µm, continuously captures images which are internally weighted in  accordance to two orthogonal correlation functions (sine & cosine), synchronized to flock-in. The internal “in-phase” result  basically represents the simplest way of doing lock-in, where  the images captured during power off (Vlock-in = 0) are  subtracted from the images during power on. For devices  under test (DUT) without any delay between applied voltage  and detected heat, this is already sufficient for hot-spot  localization. But in case of buried defects leading to noticeable  delay between voltage and heat, only utilizing this  methodology leads to reduced detection efficiency since part  of the detected heat is weighted positively and the other part  negatively. In the extreme case of 90o phase shift between  voltage and heat, this would lead to zero detection, regardless  of the hot-spot temperature. These delayed thermal signatures  are detected by use of the second internal result “out of phase”, based on the orthogonal cosine correlation. For ease of use, both internal results are summarized in the amplitude image, showing the hot-spot regardless of the thermal delay.


Additionally, the ratio between the two orthogonal results can  be used to calculate the phase shift between the excitation  voltage and the thermal response. Knowing the thermal  properties of the DUT materials, this extra piece of  information can be used for determining the depth of a buried  defect, offering sufficient accuracy to discriminate between  individual layers of today’s stacked die architectures [2].


Note that increasing the lock-in frequency can improve the  spatial resolution since less heat is introduced per cycle, leading to a reduced heat dissipation volume, hence allowing  the narrowing of the hot-spot.


The DUT in this discussion was a constant current buck  regulator delivering as much as 1.5A in step down mode. The  device reportedly failed under the absolute maximum rated  condition. It was also reported that the value of the output  inductor used on PCB was not typical.


Visual inspection of the device after decapsulation indicated  the device was severely damaged by EOS as shown in Figure


2. Figure 3 is the application schematic. Under an open load  condition, it was believed that the application overheated due  to the use of an improper L1.


Figure 2: Die picture showing massive carbonized epoxy as a  result of an EOS event. The cause of failure is often


hypothesized due to its extensive damage.


Figure 3: Application schematic of the buck regulator. An  open load condition together with a smaller value of L1 was  believed to have caused the application to overheat.


While the extensive carbonized epoxy was evident of EOS, it  was also indicative of excessive heat generation prior to device  failing. In a product evaluation, it was postulated that a smaller  value of L1 failed to maintain minimum ripple current from the  inductor and prevented the regulator from switching. During  this time, the internal pre-charge FET circuitry turned on to  significantly heat up the device [3].


In order to validate the failing mechanism, it is imperative to  determine if there was any pattern of thermal dissipation prior  to device failing. Any coincidental localization of heat source  with the pre-charge FET circuitry would explain the root cause  of failure.


A conventional thermal camera system was initially used on a  known good packaged device on the application board to look  for any pattern of heat dissipation when operating close to the  maximum rated condition. The resulting image is shown on  Figure 4. As shown the thermal emission from the package  saturated the detector instantly and little information could be  obtained.


Figure 4: Conventional thermal image of a device under the  maximum rated operating condition. Heat dissipation was so  fast that thermal distribution throughout the package revealed  no localization.


LIT Application


The known good device was then subject to the LIT analysis. The application of LIT in this analysis deviated slightly from a  typical application in that the lock-in signal was not applied  directly to the power supply pin but to an enable pin switching  the device between on and off states. This was done to ensure  stable device operation as fast switching of Vin of the buck  regulator was not a typical operation.


The result is shown in Figure 5 and Figure 6 where 6.5Hz  lock-in frequency was used. These were the thermal amplitude  and phase images respectively. The thermal amplitude image  revealed a thermal signature in the area showing massive EOS  damage in Figure 2. See also Figure 7, which is an overlay of  die photo and the thermal image to show the coincidental  location of the heat source and the EOS area. Note that thermal  emission also irradiated sideway out from the left, right and  the leads of the package. The thermal path apparently was  through the silicon substrate, die attach and then to the copper  leadframe. This observation was further substantiated by the  phase image on Figure 6. As can be seen in the phase image, the in yellow region outlines the area of the leadframe under  the silicon in blue. It is evident that the leadframe area radiated  excessive heat. It is empirical that extreme heat was generated  in the region at which massive EOS occurred in Figure 2 and  the heat propagated out through the leadframe.


If the actual phase shift in Figure 6 is analyzed, there was a  169° phase shift on the red spot and 322° on the yellow  emission. By using 3D thermal model [2] software (patent  pending) the phase difference of 153° between the 2 areas  corresponded to a depth difference in mold compound of  396µm was estimated. It indicated that, while the red spot was  coming from the die through mold compound, the yellow  emission was coming from outside of the die area, through an  extra 396µm of mold compound. The cross-section, as shown  in Figure 8, revealed a Si thickness of 390µm confirming that


the area in yellow was at the leadframe level underneath the  silicon.


Figure 5: LIT thermal amplitude. A localized heat source was  revealed near the top right corner on the package coincided


with massive EOS damage on the failing device (see also


Figure 7). The device was operated with a non-typical onboard inductor. Thermal emission also irradiated sideway out  from the left, right and the leads of the package.


Figure 6: LIT thermal phase image. Even displacement of


heat from the leadframe under the die is evident. The numbers  are showing the measured phase shift.


Figure 7: Overlay image of thermal amplitude and the die (overlay digitally processed).


322


169


Figure 8: Cross section of the device showing a silicon


thickness of 390µm. The 2 white dots are wire bonding in a  different plane of the cross-section.


The subject device was next exposed of backside to examine  the exact origin of the heat on silicon. Figure 9 shows the  overview backside image. Figure 10 is a close-up of the  circuitry on silicon that generated excessive heat.


Figure 9: Backside image showing thermal emission sites


coincided with the hot spot found on the package. Note that  the image was flipped in backside orientation.


Figure 10: Close-up of the backside thermal emission.


To verify the thermal signature was related to the value of the  output inductor, L1, the analysis was repeated with a larger  value of L1 so as to maintain a minimal ripple current. Figure  11 is the backside thermal image that shows the absence of the  excessive heat in the area which was believed to have triggered  the EOS condition.


Figure 11: Backside thermal emission on the same device that  used a larger on-board inductor (L1) to maintain a minimal  ripple current. Note the absence of the hot spot.


Discussion and Conclusion


This paper discusses LIT to examine the thermal path and  signature during the event of EOS. The lock-in signal at  frequency provided improved signal-to-noise ratio and  resolution to spatially localize the origin of the hot spot. The  analysis was done first non-destructively on package, and then  from the backside of the silicon. The thermal phase  information provides additional information in z-direction to  better understanding the heat propagation so as to leading to  the next step in the analysis.


Furthermore, since the thermal spectral response of the LIT  camera was between 3µm and 5µm, it would be interesting to  study the part of circuit schematic that was radiating heat. Examination into the pre-charge FET schematic of Figure 12  revealed the serially connected poly resistor and N3, an nchannel FET, were radiating thermally. To further push the  investigation, the backside analysis was repeated with an  InGaAs camera (spectral response: 1µm - 1.5µm). The result is  shown in Figure 13. The photoemissions in both cases were  hardly differentiable at the pre-charge circuitry regardless of  the value of L1. N2, which was configured as a diode, was  emitting as it was always conducting. No photoemission was  observed at other devices. Hence, it is empirical to state that  most of the power was consumed across the poly resistor and  N3.


Figure 12: Schematic of the pre-charge FET.


Figure 13: Photoemission images showing non-differentiable  diagnosis information at the pre-charge FET circuitry that  would (left) and would not (right) maintain a minimal ripple  current with the use of a larger and smaller L1, respectively.


[1] Breitenstein, O. et al., “Developments in IR Lock-in  Thermography”, Proc. 30th Int. Symp. for Testing and  Failure Analysis, ASM Intern. Mat. Park, Ohio November  2004, pp. 595-599


[2] Schmidt C., Altmann F., Schlangen R., Deslandes H. (2010): “Non-destructive defect depth determination at  fully packaged and stacked die devices using Lock-in  Thermography”. IPFA 2010


[3] Internal communication with Longmont Design Center  and Application Group, National Semiconductor Corp.


# System Level FA on Transmission Line Issues


System Level FA on Transmission Line Issues


Intel Corporation Hillsboro, Or U.S.A. nicholas.p.konkol@intel.com


One issue that faces failure analysis at the system level is  impedance mismatched transmission lines resulting from  developers pushing the edge of trace layout recommendations. When transmission lines on printed circuit boards are routed in  such a way as to allow for impedance mismatches, the effects  can be unwanted on the signal that the line carries. Techniques  can be used for discovering if capacitance, resistance, or split  planes are creating the impedance mismatches that are  resulting in the system level failure seen by the customer.


Desktop Mother Board and Server EFA (system level  Electrical Failure Analysis) can involve intermittent failures. An intermittent failure can involve a hang at a P.O.S.T. (power on self test) code, a hang while loading an operating  system, or a hang during typical operating system operation. Various root causes can be attributed to these symptoms such  as software drivers, marginally noisy power rails, signal  timing, signal integrity, or others. The focus here is on signal  integrity and whether or not the cause is due to transmission  line effects. For example, faster switching speeds driven by  signal drivers increase in issues with return currents, crosstalk, and ringing [1]. In the case of a long transmission line (the  time it takes a rising edge to rise at most ¼ of the time it takes  for the signal to fully propagate down the line), return currents  can have adverse effects on signal integrity.


Narrowing the Fault


At the first level of analysis on a desktop printed board  assembly (PBA), server PBA, or add in add PBA, the fault can  be narrowed to a software driver, power supply circuits, the  core chipset and its busses, or other integrated circuits and  their interfaces. If the first level of analysis leads to the core  chipset busses or any other signal interfaces to other integrated  circuits, then the next level of analysis involves narrowing the  fault to a group of signals. After the group of signals or single  signal is determined to be the cause of the fault, signal  analysis can be performed.


Signal Analysis


For example, assume that a 100 MHz clock is the cause of the  fault. A comparison of the clock signal with specifications in  its data sheet is only the beginning, because depending on the  design of the PBA, the clock specifications may be pushed to  the edge of their limits or just beyond. Weather this design


practice is acceptable or not, is not necessarily the focus of the  Failure Analysis Engineer (FAE). If it can be assumed that the  product has been through validation, then the following  technique can be used in determining if a failing product is an  issue despite the fact that its design may be pushing the limits  of its specification. So instead of simply using a data sheet as  the ultimate standard, the FAE can take a screen shot of a  clock signal on a known working PBA, a PBA that has been  tested and does not result in any failures, but may be operating  just outside of its specification or pushing its limits. Once the  screen shot of the clock signal from the known working PBA  is taken, then it becomes the standard that replaces the data  sheet. The reason for this is that if the FAE takes a screen shot  of a clock signal, compares it to a specification, finds the clock  to be operating a little out of specification, and then attributes  the clock to root cause, the FAE can be wrong. But if the FAE  finds that the screen shot of the clock on the failing PBA  matches the screen shot of the clock on the known working  PBA, then the clock can be eliminated as the source of the  failure. However, in this example, the screen shot of the clock  from the failing PBA is different enough to be considered the  source of the fault (Fig. 1, Fig. 2).


Figure 1: 100 MHz clock on a known working PBA. The  signal is measured at the source.


Figure 2. 100 MHz clock on the failing PBA. The signal is  measured at the source. The final voltage (V) is low compared  to the screen shot of the known working PBA (Fig. 1). There is  also more noise on the failing PBA clock  than on  the known  working PBA.


The screen shot of the clock signal in Fig. 2 demonstrates that  the noise and the final voltage are different from the known  good clock signal (Fig. 1). This clock is most likely the cause  of the fault and therefore a good candidate for transmission  line analysis.


Transmission Line Analysis


When signal integrity is an issue with a signal,  there can be  different sources of the issue. For example, if a signal with a  fast edge is routed over a power supply switching node on a  PBA, then this can create a signal integrity problem. But if the  signal trace has significant impedance mismatches, then a  transmission line issue exists. Three effects that can create  transmission line impedance mismatches are capacitance, resistance, and split planes.  How to detect if one of these  three is the cause of impedance mismatches is discussed  in  the section.


Capacitance


The effects of parallel capacitance at both the source and the  destination of a transmission line that carries a signal with a  fast edge can be detected. The next set of figures can be used  as a reference for the general shapes of curves with these  effects (Fig. 3, Fig 4.).


Figure 3. The effects of capacitance at the source. The signal  is measured at the source. Capacitance is added to the source  of the transmission so that the general shape of the curve can  be more easily visualized. This general shape can be used as a  reference for the FAE.


If the FAE measures a signal that resembles that shown in Fig. 3, then the transmission line most likely has too much  capacitance at the source. This can be reasoned from the fact  that the front of the signal appears to have a shape resembling  the effects of an RC time constant. This can been seen on the  slope of the signal in Fig. 3 where it says, 'Capacitor  Charging'.


Figure 4. The effects of capacitance at the destination. The  signal is measured at the source. Capacitance is added to the  destination of the transmission line so that the general shape  of the curve can be more easily visualized. This general shape  can be used as a reference for the FAE.


If the FAE measures a signal that resembles that shown in Fig. 4, then the transmission line most likely has too much  capacitance at the destination. First, it can be seen that the  initial wave propagates to the end of the transmission line and  back at an initial voltage level, as shown in Fig. 4 between the  two blue vertical crosshairs. The sudden drop in voltage is due


to a capacitor at the end of the transmission line that is not yet  charged. Second, the capacitor slowly charges according to the  RC time constant from the transmission line as can be seen by  the signal.


Resistance


The effects of load resistance on a transmission line, which  carries a signal with a fast edge, can be detected. The next set  of figures can be used as a reference for the general shapes of  curves with these effects (Fig. 5, Fig 6.).


Figure 5. The effects of high load resistance. The signal is  measured at the source. This general shape can be used as a  reference for the FAE.


If the FAE measures a signal that resembles that shown in Fig. 5, then the transmission line most likely has too much load  resistance. The wave propagates down the transmission line at  an initial value, but the final value is higher which implies that  the load impedance is higher than the transmission line  impedance.


Figure 6. The effects of low load resistance. The signal is  measured at the source. This general shape can be used as a  reference for the FAE.


If the FAE measures a signal that resembles that shown in Fig. 6, then the transmission line most likely has too little load  resistance. The wave propagates down the transmission line at  an initial value, but the final value is lower which implies that  the load impedance is lower than the transmission line  impedance.


Resistance and Capacitance


The effects of load resistance, parallel capacitance at the  source, and parallel capacitance at the destination of a  transmission line, which carries a signal with a fast edge, can  be detected.


Figure 7. The effects of low load resistance, capacitance at the  source and capacitance at the destination. The signal is  measured at the source. Capacitance is added to the source  and destination of the transmission line so that the general  shape of the curve can be more easily visualized. This general  shape can be used as a reference for the FAE.


If the FAE measures a signal that resembles that shown in Fig. 7, then the transmission line most likely has too much  capacitance at the source, too much capacitance at the  destination, and  too much load resistance.


Confirmation of Impedance Mismatch by R or C


Resistance (R) and capacitance (C) are not the only effects  that can create an unexpected waveform. In order to finally  confirm that R or C is the cause of the unexpected waveform, the FAE can modify the characteristics of the transmission  line. In the case of Fig. 2 - Fig. 7, the same PBA with the same  signal and transmission line is used in every screen shot. This  transmission line on this PBA is modified by placing resistors  at the load for impedance matching and also removing the  effects of the capacitance at both the source and destination.


Figure 8. Here is the effect of removing the impedance  mismatching of the transmission line that carries this signal.


Split Planes


The effects of a split plane under a transmission line that  carries a signal with a fast edge can be detected.


Figure 9. A model of a transmission line routed over a copper  plane compared to a transmission line routed over a split  plane.


Figure 10. The effect of two transmission lines when routed  over a smooth plane as compared to a split plane. The screen  shot is captured from a TDR (Time Domain Reflectometer). The Y-axis on the TDR screen shot in Fig. 10 represents ρ (reflection coefficient) and the x-axis represents t (time).


The gold line on the screen shot in Fig. 10 represents the  transmission line that does not have the split (Fig. 9). The  purple line on the screen shot represents the transmission line  that has the split in the ground plane. The blue line represents  the TDR probe unconnected to any transmission line. The gold  line demonstrates that the impedance of the transmission line  routed over the smooth part of the ground plane is fairly  matched. However, the purple line demonstrates that the  impedance of the transmission line routed over the split part of  the ground plane is inconsistent.


Table 1: TDR Results for two transmission lines, shown in  Fig. 9 and measured in Fig. 10, compared to unconnected  TDR probe unconnected.


TDR Probe  Unconnected


Even  Plane


Split  Plane


TDR Curves  from Fig. 10


Blue


Gold Purple


Transmission  Characteristics


Open Circuit Const. NonC.


*Const. means constant in reference to the slope of the curve, and NonC. means nonconstant in reference to the slope of the  curve.


Referring to both Fig. 19 and Table 1, the blue line is used as a  reference as to the location of the start of the two transmission  lines that are represented by the gold and the purple. The ends  of the transmission lines are represented by the parts of the  curves where they reach their maximum constant values. The  gold curve from the start of the transmission line to the end of  the transmission line is constant relative to the purple curve, except for when they both reach their maximum constant  values.


Even though the TDR along with some PBA analysis are good  tools for determining split planes as the cause of impedance


mismatching, the FAE may want to eliminate the mismatches  on the PBA and then confirm that the failure is eliminated.


Confirmation of Impedance Mismatch by Split Plane


In order to smooth out the purple line in Fig. 10, stitching  capacitors can be placed over the split in the ground plane so  that the signal has a more direct return path. Fig. 11 contains a  model with stitching capacitors and Fig. 12 gives the results of  the transmission line with the stitching capacitors.


Figure 11. Model of stitching capacitors across a split ground  plane.


Figure 12. Effects of a signal with a fast edge propagating  down a transmission line with and without a split in the  ground plane and also with stitching capacitors over the split  plane. The Y-axis on the TDR screen shot in Fig. 12 represents ρ (reflection coefficient) and the x-axis represents t (time).


The gold line on the screen shot in Fig. 12 represents the  transmission line that does not have the split but is routed over  a smooth plane. The purple line on the screen shot represents  the transmission line that has the split in the ground plane. The  blue line represents the TDR probe unconnected to any  transmission line. The green line represents the transmission  line that has the split in the ground plane with stitching  capacitors over the split. The green line demonstrates that ρ


(reflection coefficient) is reduced at the same points of Z (impedance) discontinuity as the purple line. This means that  adding the stitching capacitors over the split plane helps  smooth out the ρ vs. t curve.


When the ρ vs. t curve is smoother, this means that there are  fewer Z discontinuities. This has two desired effects. First, the  return path along the transmission line remains more tightly  bound to the transmission line which results in the reduction  of cross talk. [1] Second, it reduces the effects of unwanted  reflections. [2]


An example of a split plane creating transmission line  problems for a high speed signal was discovered through  electrical failure analysis within Intel on a system. When the  system attempted to load Windows XP, it hung. It did not  always hang and therefore was intermittent. The root cause  was attributed to a high speed differential pair signal routed  over a split plane. In order to eliminate the failure (Windows  Hang Load), stitching capacitors were placed over the plane  split. This can be seen in Fig. 13.


Figure 13. Stitching capacitors over a plane split eliminate a  Windows XP hang failure.


In conclusion, sometimes PCB layout designers may not be  able to follow the best transmission line design practices. If  this is the case, the transmission line problems may be subtle  and result in intermittent system failures, failures that are so  intermittent that they are not caught during the validation of  the product. When this happens, the technique presented here  is one way of determining if the intermittent system failures  are due to some types of transmission line issues.


[1] Johnson, Howard, Graham Martin, High-Speed Digital  Design a Handbook of Black Magic, Prentice-Hall (New  Jersey, 1993), pp. 59-60, 194.


[2] John F. Wakerly, Digital Design Principles & Practices, Prentice Hall p. 788 (1994)


# Fault localization of power-ground short via signal injection and oscilloscope technique


Fault localization of power-ground short


via signal injection and oscilloscope technique


Intel Corporation, Hillsboro, Oregon, USA  Binh.T.Nguyen@intel.com


For those attempting fault isolation on computer motherboard  power-ground short issues, one of the challenges to overcome  is to find the correct tools and techniques for the job. The  optimal technique should utilize existing test equipment  available in the debug facility, requiring no specialty  equipment as well as needing a minimum of training to use  effectively.  The test apparatus should be both easy to set up  and easy to use. The signal injection and oscilloscope  technique described here meets the above requirements. It will  make the task of doing fault isolation on power-ground short  issue both easier and faster.


Test Setup


The signal injection and oscilloscope technique is based on the  application of Ohm’s law in a short-circuit condition. The  highest current will go into the node where the resistance is  lowest, i.e., the short-circuit node. In this event, the shortcircuit node will show the great decrease in voltage.  In other  words, it is the lowest voltage level node. With a proper setup, the oscilloscope is sensitive enough to detect the lowest  voltage level where short-circuit is located. The signal  injection and oscilloscope technique uses the comparative  analysis method. This method compares the amplitudes of all  captured signals along the shorted power rail with the  oscilloscope. The lowest signal amplitude indicates the  location of short-circuit either right at the oscilloscope  measurement location or very close to it. Next, the root cause  of the short-circuit condition can be further identified by other  non-destructive techniques such as optical microscope or Xray. The signal injection and oscilloscope technique works  best for a dead short issue where short-circuit measures less  than 1 Ohm. In this case it will generate the greatest decrease  in voltage at or near the location of the short easily recognized  as lowest signal amplitude. Typical issues that cause dead  shorts are solder bridging, fab defects and electrical overstress (EOS) damaged components.  As mentioned above, the tools  used for this technique are common tools which are readily  available within any debug facility. As shown in Figure 1, they


include an Oscilloscope, a Lab Power Supply and a Push  Button Switch.


Figure 1: Test setup for signal injection and oscilloscope  technique


The process of test setup and measurement is quite simple. As  shown in Figure 1, the power supply is connected to a  suspected short-circuit power rail via the Push Button Switch.  Since the differences among the captured signals along the  suspected short-circuit power rail are very small, the power  generated from the power supply is set at lowest level both in  voltage level and current limit so the voltage drop can be  maximized. The oscilloscope also needs to be set up at the  lowest vertical scale so it can detect even the smallest different  amplitude among captured signals. The offset function can be  used to enhance the capability of the oscilloscope to detect the  smallest change in signal amplitude. To make the measurement  fast and easy, the oscilloscope GND is connected to GND  plane of device under test (DUT) so a return line via the  oscilloscope probes may not necessary. The user may use up to  four oscilloscope probes in conjunction to simultaneously  measure up to four points along the suspected short-circuit  power rails. The end result is the location of short-circuit can  be found faster. Note that if the Lab Power Supply has an  existing standby power button then the Push Button Switch  may not be needed since a sharply rising DC voltage edge can  be applied directly to DUT by using the standby power button


as opposed to a serial Push Button Switch.  If no Lab Power  Supply is available, the Regular Power Supply which is used  to power the motherboard can be used. It has some drawbacks  compared to Lab Power Supply; the user can not control the  voltage level or the current limit level.  The user may need to  set appropriate offset level on the Oscilloscope to get the best  display of voltage change from different test points.


The theory behind the experiments is the application of the  equation for power from Ohm’s law. From Ohm’s law, the  equation for power can be obtained in the form:


Where:


P = power supplied to the resistor from power supply


V = voltage across the resistor


R = resistance


From the power equation, there are two predictions for the two  scenarios in the experiments where a simulation of a shortcircuit VCC3 power rail is used on a good working personal  computer (PC) motherboard.


1. When a no short-circuit VCC3 power rail is applied on a PC


motherboard, there is no change to R leading to no change


of V. We expect almost the same VCC3 voltage values at


different nodes on its power rail.


2. When a short-circuit VCC3 power rail is applied on a PC


motherboard, R, a resistance from VCC3 power rail to


GND, is significantly decreased. That leads to a decrease of


VCC3 voltage since P is considered constant. The closer to


the location of the short-circuit VCC3 power rail the lower


the measured resistance leading to lower the VCC3 voltages.


In fact the measured VCC3 voltage decreases exponentially


with lower resistance. Thus the lowest measured voltage


occurs closest to the short-circuit location.


Two experiments were conducted to prove the effectiveness of  signal injection and Oscilloscope technique. Both experiments  simulate a short-circuit condition on the VCC3 power rail of a  good working PC motherboard then apply the signal injection  and Oscilloscope technique to localize the short. Prior to  detailing the experiments, it is a good idea to give a brief  description on the partial PC motherboard block diagram (Figure 2) that is related to the experiments and test points  where the VCC3 signals are captured by Oscilloscope.


Figure 2: Partial PC motherboard block diagram


The PC power supply provides VCC3 to the PC motherboard  via the Power Supply Connector. VCC3 is power source to a  variety of PC motherboard components such as South Bridge, FWH (Firmware Hub), SIO (Super IO), Clock Generator and  many resistors and capacitors. To simulate a real life condition  where a typical dead short condition often occurs, the Power  Supply Connector, SIO, FWH and South Bridge are used in  the experiments. The Oscilloscope is used to monitor the four  test points (TP1, TP2, TP3 and TP4) which are at or close to  the Power Supply Connector, SIO, FWH and South Bridge  respectively. A solder bridge is used to simulate the shortcircuit condition between VCC3 and GND. It is located  between FWH and South Bridge which are TP3 and TP4  respectively. It is also closer to the South Bridge than the  FWH. The location of all four test points and short-circuit  VCC3 are shown in Figure 3.


The detailed layout section of the PC motherboard for TP3, TP4, and short-circuit VCC3-GND are identified in Figure 4.


Figure 3: Location of four test points and short-circuit on  VCC3 on PC motherboard


Figure 4: Detailed layout of TP3, TP4 and short-circuit VCCGND location


Experiment #1


In this experiment, the Lab Power Supply setting at 4 Amps  current limit is used to inject a 0.7V DC voltage edge through  power supply connector on PC motherboard. An Oscilloscope  with four channels is used to monitor the four test points at the  same time. To show the effect of the short-circuit VCC3 on the  four test points; two Scope snapshots of the four test points are  taken. One snapshot is for the PC motherboard prior to shortcircuit VCC3 simulation. The other snapshot is for the same  PC motherboard after short-circuiting VCC3 to GND. After a  few trials for the best resolution display on Oscilloscope at the  lowest DC voltage, 0.7V DC is selected for injected signal as  shown in Figure 5.


Figure 5: Scope snapshot for the four test points on good nonshort VCC3 motherboard


Figure 5 shows no difference on amplitudes of the four test  points regardless of their positions to signal source (Power  Supply Connector). However, the amplitudes of four test  points change significantly when simulating a short-circuit  condition VCC3-GND between TP3 and TP4. Figure 6 shows  that the closer is the test point to a short-circuit location, the  lower the amplitude of the test point.


Figure 6: Scope snapshot for the four test points on shortcircuit VCC3 motherboard


As shown in Figure 6 above, TP4 is the one that exhibits the  lowest amplitude signal. Since TP4 is the closest to the shortcircuit condition, this illustrates the signal injection and  Oscilloscope technique working in action. Although the shortcircuit location is located outside the South Bridge in this  experiment, a similar result should be expected if the shortcircuit were located inside of the South Bridge component. Figure 6 also shows that the low scale setting of Oscilloscope (20 mV/ Div) gives the user better display resolution to detect  the location of the short-circuit.


Experiment #2


As mentioned earlier, in the case where no Lab Power Supply  is available, the user may use the Regular Power Supply for  the Oscilloscope technique on the condition that the  motherboard is able to power up even momentarily. Except for  the Regular Power Supply, this experiment uses the same  motherboard with the same test points of the Experiment #1. The result is shown in scope snapshot in Figure 7.


Figure 7: Scope snapshot for the four test points when using  Regular Power Supply on shorted VCC3


Experiment #2 gives the identical result as Experiment #1 in  which TP4 is identified as lowest signal amplitude. A Regular  Power Supply still can do a job but much more difficult since  the user cannot control the voltage level or current limit level. There is a potential risk of loss of short-circuit evidence as in  the case of very small-scale solder bridging which can be  easily burnt off by the high current of a Regular Power Supply.  In addition, the user has to spend more time either  manipulating the Oscilloscope offset level or setting up  variable scales to get the better display resolution. It is much  more challenging and difficult with high voltage rails such as  5V or 12V rails. The Regular Power Supply usage is an option  but it is not recommended. By contrast, the external signal  injection is still a preferable technique since it provides the  user with non-destructive, generic and simple method.


The signal injection and oscilloscope technique is a simple, low cost and non-destructive method that greatly helps the user  to find the location of the power-ground short quickly and  more effective.


Chet Lee was very helpful in giving support and guidance. He  also reviewed the manuscript and gave many good


recommendations.


[1] Tektronix TDS 694C Digital Real time Oscilloscope User  Manual, Tektronix Inc July 2000


# Product debug: Speed problem related to unexpected RC delay


Product debug: Speed problem related to unexpected  RC delay


NXP Semiconductors, Nijmegen, The Netherlands   Jan.van.Hassel@nxp.com


In new product designs increasing effort is needed to observe  and prove failure mechanisms or process marginalities. For  advanced failure analysis Soft Defect Localization (SDL) [1] and Time Resolved Emission (TRE) [2,3] have now become a  standard analysis method. Both techniques require a close cooperation between designers and analysts. In this paper we  will discuss a comprehensive study to find the mechanism  behind a speed problem in the digital part of an audio signal  processor. The additional delay was related to unwanted  routing through poly-silicide in timing critical circuitry.


Successful failure analysis in complex and large products  requires throughout knowledge of the product and the failing  conditions. This knowledge is to be combined with the  requirement from failure analysis to stimulate the failing mode  and offer the right output signals to localize the failure. The  failure analysis requirements additionally depend on the tools  used. In this case close co-operation between application and  design engineers and failure analysis was essential in  obtaining adequate FA setup and proper input signals for the  equipment used. On chip CPU programming was performed  to fulfill the requirements for the setup.


During first silicon evaluation of the audio product in 0.15 µm  technology it was observed that the chip failed at speed.  This  reduced speed was observed on only 1 particular Digital  Signal Processor (DSP) implemented in the design. Several  other DSPs were running at speed. These DSPs were designed  in an identical flow and had a similar function for data  processing. Since all samples suffered from the same delay, investigation had to be focused on design rather than process  marginality. First hypothesis was local dynamic voltage drop  in the area of the specific DSP. Although simulation results  confirmed that voltage drop was highest in the suspected area  it could not explain the amount of speed loss that was  observed. Subsequent Soft Defect Localization (SDL) identified a critical path in the DSP of interest. TRE  measurements confirmed that the signal was propagating a


factor 5 too slow in the net.  A closer study of the design  revealed that routing was done through poly instead of  backend metal. Since this particular net used poly routing over  several individual cells in series the additional delay was too  much. In the other DSPs where similar routing through poly  was found the affected nets did not impact the functionality of  the IC since the delay remained within the design margins.


This paper presents the results obtained in different stages of  failure analysis. The paper will start with a functional  description of the device and the information obtained from  the software debug. Subsequently the different FA techniques  and the results will be discussed.


Failure description


Electrical characterization


Figure 1: Die layout of the product involved. The 4 digital  signal processors are indicated in different colors. DSP2 is  labeled “2” and shown in green. This DSP is responsible for  audio processing and shows a speed problem above 150 MHz.


During first silicon evaluation of the audio product in 0.15 µm  technology (64 mm2) it was observed that the chip failed at  speed. Whereas typically 170 MHz was expected the  functionality was lost at 150 MHz. The SOC contains a 32-bit  controller and 4 “identical” digital signal processor (DSP) cores. On the chip, digital inputs are available such as I2S and  SPDIF. Also data from embedded AD converters that digitize  analogue IF frequency signals from a separate tuner device are  possible input signals. Audio processing such as equalizing, tone/volume control is done in the DSPs to be processed on  common audio sample rate. In figure 1 it is shown how the  DSPs are embedded in the chip design. DSP0 and 1 are used  for radio processing and DSP 2 and 3 for audio processing.


Extensive electrical investigation revealed that only one DSP  was responsible for the speed failure. In this specific DSP, digital audio data is filtered using digital filter coefficients as  shown in figure 2.


Figure 2 shows the main functionality of DSP2 that is  involved in the speed problem. Digital audio data and filter  coefficients are brought in the central unit where the filters  are calculated.


The difficulty for failure analysis was that the program control  was run from a ROM thereby limiting the flexibility to run the  sequence step by step. However by altering the input data and  enable/disable instructions the product software engineers  isolated the problem to be located in a multiply accumulate  unit. In this part data from an accumulator register (AR) is  sent to the arithmetic shift unit (ASU). Depending on the  instruction, different shift operations can be selected. After  this operation, the resulting data is combined with a number  from the product register (PR) and stored again in the  accumulate register. This process is schematically shown in  figure 3. Depending on the selected shift operation done by  the ASU, the maximum operational speed of the DSP was  limited. Although the problem looks very localized, an area of >10.000 logic gates could still be part of the critical path.


Figure 3 shows the Multiple Accumulate Unit MAU unit that  was responsible for the speed problem as obtained by  software debug. In this combinatorial logic module data from  the accumulator register (AR) is sent to the shift register (ASU) and combined with the product register. Depending on  the shift operation selected, the failure mode is present or not.


Electrical measurements and simulation


The design team initially pursued a hypothesis that a local, dynamic supply voltage drop was causing the speed problem  since the specific DSP was embedded differently in the design  from power supply point of view. Due to the fact that all  memories were supplied on a separate power domain and that  DSP2 was located in-between several memories, power  supply to DSP2 had to pass over long distances. Additionally, it was observed that decoupling cells were distributed very  irregularly in the design, causing some digital parts up to areas  over 200 µm in size without those cells. This is shown in  Figure 4.


Figure 4 shows an area within the digital part were  decoupling cell are hardly available. The white rectangles  represent the individual decoupling cells.


Decoupling cells are small embedded capacitors placed  between Vdd and ground to smoothen out “glitches” in the  power domain.


The idea of a local dynamic supply voltage drop was  supported by Redhawk [4] simulation. The simulation shows a  time resolved voltage drop map of the chip, over a whole  clock cycle. A screenshot of the simulation is shown in figure


5. This simulation showed that the worst-case supply drop  occurred indeed in the region of the failing DSP. Although the  supply voltage drop was specified at 60 mV, an actual drop of  110 mV was measured. This was measured with probes on  pads made by FIB modification towards the lower metal  layers. However even the measured values could only explain  no more than 4 – 5 Mhz speed loss. It was evident that a more  detailed understanding of the fault location would be needed  to solve the problem.


Figure 5: Screenshot of the Redhawk simulation. The total  simulation shows a time resolved voltage drop map of the  chip, over a whole clock cycle. Worst drop is observed in the  area of DSP2.


Soft defect localization


Since timing problems were considered as another possible  root cause, the failure analysis setup was prepared for  Scanning Optical Microscope (SOM) measurements. For SDL [5.6] a suitable program had to be created to perform these  measurements.


By software debug the DSP product engineer localized the  problem down to a set of 57 instructions in the MAU. For  SDL the identical operation was performed in the functional  DSP3. Comparing the results of the identical calculations in  DSP2 and DSP3 a pass/fail signal was fed into a general  purpose IO pin. By adjusting the digital supply voltage the


device was set to a 50% operational fail/pass mode. Slowing  down the signal in the critical path by laser scanning would  increase the failure rate. In Figure 6 the response of laser  scanning on the sample are shown. Laser scanning is done  from the backside of the sample while the device is in an  application board.


Figure 6: On top the SOM feedback using the 1340 nm laser. Failure rate is increased when passing over a specific area in  DSP2. A zoom is shown in the center image. All spots involved  were linked in one specific net (bottom).


A specific net was identified in DSP2 with the laser. This net  was one of the 3 select paths coming into the ASU (see figure  3). Further it was observed that in the area of the suspected  net, the density of the decoupling cells was minimal. However  this was considered as a second order parameter taking into  account the dynamic voltage drop measurements. Subsequently TRE timing measurements on the suspected net  were initiated to measure the actual delay.


Time Resolved Emission


The TRE measurements were done on various transistors at  intermediate locations from the driver to the end of the  suspected net. Instead of an expected delay of 300 ps for the  signal, 1.5 ns was measured. The TRE measurements along  the chain are shown in figure 7. On top is the net driver.


Figure 7: The TRE measurements on the failing net show that  a total of 1.5 ns is necessary to propagate over the suspected  net. On top is the emission at the driver site and going  towards the bottom emission is measured on various sites  along the net. The shape of the signal varies as different types  of cells are characterized.


The additional 1 ns delay could explain the fail at higher  frequencies. A closer look at the gds finally revealed that  routing was done through poly instead of metal. In Figure 8  the net is shown in highlight with poly switched off. The  measured delay is also shown in this figure. The cell used for  the routing was a multiplexer shown in figure 9.  For design  and layout flexibility the cell has the possibility of 2 inputs  named S0. In the specific net, seven of these cells were  connected in series causing the 1.5 ns delay. Since each poly  adds about 500 Ohm of additional resistance and a load of 500  fF a total RC delay of 1750 ps can be estimated. This agrees  well with the observations done by TRE.


Figure 8: The suspected net and some delay measurements by  TRE at different positions within the chain. Poly is not  highlighted. It shows the gaps were routing is done through  poly silicon.


Figure 9: The multiplexer cell having two S0 inputs for design  and layout flexibility. Since both inputs were used without  additionally connecting them by a metal interconnect, poly  became part of the routing causing the additional delay. In the  net of interest, 7 of these structures were routed in series.


This paper describes the investigation of a speed problem  during the evaluation of an audio IC. It was found that a  combined effect of  “poly routing” and the non-optimal power  grid to supply DSP2 (voltage drop) was the reason for this  failure in the 0.15 µm technology. Intensive collaboration  between designers, software product debug engineers and  failure analysis was necessary to achieve these results.


1.5 ns


The Authors would like to acknowledge Frank Zegers (design) and Alexander van Luijpen (application) and many  others for the discussion and contribution to this work.


[1] M Bruce, V Bruce, D Eppes, J Wilcox, Ecole, P  Tangyunyong, C Hawkins, “Soft defect localization (SDL) on Ics” Proc. 28th International Symposium for  Testing & Failure Analysis, 2002, pp. 21-27.


[2] J.S. Vickers, R. Ispasoiu, D. Cotton, J. Frank, B. Lee, S. Kasapi, “Time-Resolved Photon Counting System based  on a Geiger-mode InGaAs/InP APD and a Solid  Immersion Lens” IEEE 2003, pp 600-601


[3] J.C. Tsang, J.A. Kash, D.P. Vallett, “Time-resolved  Optical Characterization of electrical activity in  Integrated Circuits” Proceedings of IEEE, Vol. 88, 2000,  pp 1440 – 1459


[4] http://www.apache-da.com


[5] J.A. Rowlette, T.M. Eiles, “ Critical timing analysis in  microprocessors using near-IR laser assited device  alteration (LADA)”, ITC 2003, pp 264-273


[6] A. Mels, F. Zachariasse, “Reduce of acquisition time for  RIL, SDL and LADA”, Proc. 33rd International  Symposium for Testing & Failure Analysis, 2007, pp 6 –


# Timing Characterization of a Tester Operated Integrated Circuit by Continuous and Pulsed Laser Stimulation


Timing Characterization of a Tester Operated Integrated Circuit by Continuous  and Pulsed Laser Stimulation


Tuba Kiyan


Yildiz Technical University, Istanbul, Turkey  tkiyan@yildiz.edu.tr


Christof Brillert


Christian Boit


The scope of this work is to investigate the timing  characteristics of a state of the art fully functional IC through  continuous wave (CW) and pulsed laser stimulation. The  propagation delay of a gate depends on the drain current of  nMOS and pMOS transistors, load capacitance and supply  voltage. Localized photocurrent induced by laser beam alters  some of these electrical characteristics, resulting in a change in  the switching time of the gate. In addition to the desired local  timing influence, a global effect on the timing throughout the  full scanning period occurs as secondary phenomenon that - if  not taken into account properly, may mask the local signal.    This effect is strong under CW laser operation and can be  drastically reduced in pulsed laser condition.


Static Photoelectric Laser Stimulation (PLS) and Thermal  laser stimulation (TLS) techniques were introduced in early  1990’s to localize metal shorts/opens, bad contacts/vias, latchup and junction defects. In addition, timing in Integrated  Circuits (ICs) is becoming an important issue in state of the art  technologies. Shrinking geometry and higher clock rate, which  result in speed faults, push failure analysis laboratories more  and more towards delay testing. Therefore, Dynamic Laser  Stimulation (DLS) techniques such as Soft Defect  Localization (SDL) [1], Resistive Interconnect Localization (RIL) [2], Laser Assisted Device Alteration (LADA) [3], Delay Variation Mapping (DVM) techniques [4] were  developed in order to locate dynamic defects, to analyze the  IC performance or to perform timing characterization.


Illuminating the device with a 1.064 μm wavelength laser  beam causes mainly generation of electron-hole pairs and, as  secondary phenomenon, the generation of localized heat  sources and thermal gradients [3,5-7]. Regarding the  magnitude of induced delay shifts, the photoelectric effect of a  1064 nm laser is stronger than the thermal effect [3]. The  generation of electron-hole pairs is related to the interband  absorption of photons (as the energy is greater than the band


gap energy). Induced excess carriers on a semiconductor will  recombine with carrier lifetime as related parameter. However, if the carriers are generated within a space charge region (SCR) or in a distance smaller than the carrier diffusion  length, the carriers will be dissociated and a net photo current  will be generated.


There are two general modes of laser operation: CW and  pulsed. In this investigation, the laser has been operated in    CW and pulsed mode as well. Most of the DLS techniques in  the literature use CW laser. A pulsed laser has lesser overall  power, but the pulse can be set to a specific frame of the test  sequence with the aid of an Automatic Test Equipment (ATE), so that side effects are reduced or suppressed.


Device Under Test


The structure selected for this investigation is a multiplexer as  part of a delay chain. The device under test (DUT) is provided  by Infineon Technology AG, Munich. It is produced in 90 nm  triple well Complementary Metal Oxide Semiconductor (CMOS) technology, packaged in a flip-chip Super Ball Grid  Array (SBGA).


In the triple-well process, a p-well is placed inside a deep nwell, resulting in three types of well structures as shown in  Figure 1. The deep n-well covers all the devices including the  nMOS transistors forming a reversed biased junction between  p-well and deep n-well.


The schematic and the layout of the investigated structure are  shown in Figure 2 while the reflected light image and the  layout of the scanned area are shown in Figure 3.


Figure 1: The cross-section of an nMOSFET and a pMOSFET  for triple well technology


Figure 2: (a) The schematic and (b) the layout of the  investigated structure (Metal1, Contact, Poly, active areas are  highlighted only)


2 um


filling structures


Filling


structures


Multiplexer


Figure 3: (a) The reflected laser micrograph of a 512x512  pixel area on DUT obtained by 50x objective lens (b) The  reflected laser micrograph of the scanned area (32x32 pixel)


(c) The layout of the scanned area


Experimental Setup


The device runs in dynamic mode, which is driven by  automatic test equipment (ATE). ATE produces the pulse  trigger as well. The laser diode emits at the wavelength of  1064 nm. In scan mode, a time measurement tool is employed  while the digital oscilloscope is used in single point mode. In  case the pulsed laser is used, the laser trigger is produced by  tester and fed into the laser diode box. The experimental setup is shown in Figure 4.


Figure 4: Experimental Set-up


Laser Pulse Trigger  output


Image


Processing


Scanner


Unit


ATE


Detector   Laser Diode


Oscilloscope


DALS Kit


input


TAC


A time-to-amplitude converter (TAC) is used to measure the  propagation delay time. We utilized an ORTEC Model 566  TAC unit. It measures the time interval between two pulses  applied to its inputs and generates an output pulse with an  amplitude proportional to the elapsed time. Input and output of  the delay chain drive input terminals of the TAC. When the  delay increases, the output pulse amplitude of the TAC  increases as it is illustrated in Figure 5.


Figure 5: The illustration of the input and output of the delay  chain and the corresponding TAC output


The output of the TAC is fed into Dynamic Analysis of Laser  Stimulation (DALS) Kit, which integrates the signal of  interest. DALS Kit uses an analog integrator to detect the duty  cycle, amplitude or frequency changes in the signal. The  circuitry in the DALS Kit integrates the TAC output signal per  pixel and this integrated signal is used to build up a grayscale  image by the image acquisition card of PHEMOS 1000, while  the laser is scanning the area of interest. If the TAC output  amplitude increases, the output of the DALS kit will increase, too. This change will be detected by the image acquisition  card of the system and the related pixel will be colored in  white. Later on, the gray scale image is overlaid on the  reflected light image for localization.


The set-up with the TAC is very suitable for scanning the  device and grabbing the stimulation images, but it is not  straightforward and accurate for quantitative measurements. Thus, we used a high bandwidth, high sample rate LeCroy  8620A oscilloscope in order to measure the exact delay values. For oscilloscope measurements, the laser is set to point mode. In this mode, the laser does not scan an area, but it is placed on  the investigated structures and the delay chain input-output  delay is measured.


TAC Measurements


The devices can be stimulated with 1064 nm laser in two  ways: either a CW laser or a pulsed laser can be utilized. We  have both continuous and pulsed laser diodes installed in our  system. In case the pulsed laser is used, the laser pulse is  synchronized with the delay chain input stream. The laser  pulse signal in respect to the input and the output signals are  shown in Figure 6. The laser is triggered before the input and


the output signal rising edges and it switches off before the  falling edges.


Figure 6: The laser pulse, the input and the output signals in  time domain (The pulse width of the signals is 200 ns, the  laser pulse and the input signal frequency is 50 kHz)


As shown in Figure 7, laser stimulation appears as a dark spot  on the nMOS transistors and as a bright spot on the pMOS  transistors both for continuous and pulsed laser. It means that  laser stimulation causes speed up for the nMOS transistors and  slow down for the pMOS transistors in the operation speed of  the delay chain. The intensity of the spots decreases with the  increasing supply voltage, requiring slower scanning times or  more integration.


The generated electron-hole pairs in the SCR of the transistors  such as channel, drain/substrate or source/substrate alters the  device characteristics and therefore perturb the switching time  of the delay chain when the laser beam hits. Moreover, as it is  stated in [3], the induced photocurrent in p substrate/n-well  junction of the pMOS transistors changes the bias point of the  pMOS transistor via backgate effect. The threshold voltage  decreases due to potential drop between the n well contact and  the laser spot.


The analysis of the scanned area showed that CW laser  perturbs the speed of the delay chain even when it hits the  filling structures (see Figure 7). As shown in Figure 1, filling  structures are p-implanted areas, which are situated inside the  deep n-well. The filling structures are connected to the ground  line. Therefore, a p-n junction is formed between p-implanted  area and the deep n-well. The generated electron-hole pairs in  the space charge region of these p-n junctions cause a  photocurrent generation, which perturbs the switching time of  the delay chain. The stimulation on the filling structures is not  desired. The analysis with the pulsed laser shows that short  laser pulses can suppress this effect. In pulsed operation, the  laser can be switched on just on the edges of the signals and  thus minimizing the secondary effects. For the supply voltages  higher than nominal voltage, the pulsed laser stimulation on  the filling structures is not detectable anymore. The only


input of the  delay chain  output of the  delay chain


output


visible spots are on the multiplexer. Moreover, in case of CW  laser beam, there is no stimulation detected on the investigated  multiplexer for 1.5 V supply voltage. In pulsed condition  however, laser stimulation is able to localize it.


The grayscale images are overlaid onto the layout of the  scanned area. It showed that the bright and dark spots are  located on the transmission gate and on the first inverter of the  multiplexer. At 0.72 V supply voltage and pulsed laser  condition, the stimulation of the second inverter is (weakly) visible and it gives the opposite type of color. The spots on the  second inverter are not visible for nominal supply voltages or  higher, since the devices are more sensitive to laser  stimulation at lower supply voltages.


Figure 7: Grayscale images showing the delay shifts induced  by CW and pulsed laser illumination (obtained by TAC for  various supply voltages – the scan speed is 1.4 ms/pixel)


Oscilloscope Measurements


The oscilloscope measurements are carried out on the  investigated multiplexer. A line through nMOS and pMOS  transistors is scanned with laser beam (shown in Figure 7) when the device is biased at 1.2 V and the grayscale intensity  values for each pixel are stored in a file. Later, the laser beam  is positioned on different points on the same line and the delay  shifts are measured by oscilloscope. Each measured delay is  assigned to the intensity value of the related pixel. The laser  off delay time is subtracted from laser on delay values and  plotted in a graph for pulsed and CW laser (Figure 8). A laser  pulse width of 200 ns is applied in pulse mode.


Figure 8: The delay shift by continuous and pulsed laser  through a line scan over the multiplexer (The pulse width of  the laser is 200 ns, the laser pulse and the input signal  frequency is 50 kHz)


Two important effects are observed: Once the laser is  triggered, an instantaneous delay level is taken, always higher  for CW (~28 ps) than pulsed laser (~6 ps). This global delay


CW laser


Pulsed laser


pMOS


CW


12 ps


VDD = 0.72 V


VDD = 1.2 V (Nominal Voltage)


VDD = 1.5 V


Scan


direction


28 ps


8 ps


nMOS


Global


delay shift


Laser off


Laser on


Pulsed


4 ps


6 ps


shift is an unwanted overlay or masking effect discussed in a  special chapter. The real investigation of the signal path is  performed with the local delay shifts on the transistors under  test. Local stimulations are relatively small in pulsed mode  since the laser pulse is triggered at the signal edges.


The propagation delay times of an inverter, tPLH and tPHL  determine the input-to-output signal delay during low-to-high  and high-to-low transitions of the output, respectively. The  overall propagation delay of the inverter is defined as the  average of the two values. The propagation delay of the whole  delay chain versus supply voltage graph is shown in Figure 9.


Figure 9: Propagation delay of the delay chain for various  supply voltages


The propagation delay can be expressed as:


DSAT DD


L


tΔΔ∝


Δ


where CL is the load capacitance, VDD is the supply voltage  and IDSAT is the saturation current. Any perturbation on the  power supply or on the saturation current changes the  propagation delay. For a 90 nm technology device, the  parasitic capacitance is in the order of ten fF and the saturation  current is 90 μA for nMOS or 35 μA for pMOS at 1.2 V  supply voltage. As a result, the power supply changes in the  order of hundreds of milivolts cause picosecond global delay  shifts.


The measured delay shift values for various supply voltages  are plotted in a graph. These graphs can be seen in Figure 10  for CW and pulsed laser. The laser beam induced signals are  stronger at lower supply voltages, since the sensitivity of  device dynamics to temperature or additional carriers produce  stronger instabilities in operation. With laser power is kept  constant, the induced delay shift by CW laser is 65 ps and 40  ps for 1.0 V and 1.2 V supply voltages, respectively. The laser  off delays from Figure 9 are 13 ns and 11 ns, respectively.


The device is more immune to the changes in the local power  supply at higher supply voltages.


Figure 10: Delay variations on the multiplexer versus supply  voltage for CW and pulsed laser obtained by oscilloscope in  semi-log scale (the laser beam is positioned on the pMOS  transistors where the bright signals are detected)


Discussion of Global Delay Shift


Stimulating the device with a 1.064 μm wavelength laser  beam causes two effects: electron-hole pair generation (PLS) and temperature rise (Thermal laser stimulation- TLS). This  chapter discusses how these effects can contribute to a global  delay shift.


Filling structures for STI (shallow trench isolation) are pimplanted active areas and they are situated in the deep n-well  forming a p-n junction. Since PLS creates a photocurrent on  all p-n junctions, the filling structures are stimulated as well  influencing the local power supply. These local voltage  changes can cause global delay shifts.


TLS is based on conversion of laser light into heat by  absorption on metal surfaces and by free carriers in silicon.  In  the operating voltage range (0.7 to 1.5V), the limiting factor of


the transistor driving strength is channel carrier mobility [9]. Heat reduces carrier mobility and causes a slow down at both  rising and falling edges for nominal supply voltages. This  effect has mostly been neglected as temperature increases due  to TLS only by few degrees and the timing variation has been  assumed to be weak [3]. The absorbed NIR laser beam heats  mainly IC metallic elements, and to a lesser extent, polysilicon  elements and highly doped substrate areas [10]. Free carrier  absorption coefficient rises when the concentration of charge  carriers is increased [8]. In addition, the generated heat  diffuses in the order of ms. Due to the variety of heat diffusion  paths (silicon, several layers of interconnects), the heat  diffusion length is very hard to estimate. The scanned area of  16x16 µm2 is relatively small and can be diffused by heat in  much less than a ms. In pulsed laser operation, the diffusion  length is depending on the pulse frequency and for 50 kHz in µm order of magnitude, the same as carrier diffusion lengths  in medium doped silicon.


All the discussed properties of TLS fit to the global delay  shift: Immediate onset when chip starts to be exposed by laser (diffusion time short vs. scanning speed), less intense when  pulsed laser is applied (reduced thermal diffusion length). The  PLS-related carrier diffusion length is typically shorter than  100µm and does not vary much with laser pulse durations as  applied in this work. Therefore, the global delay shift can be  caused by PLS only as stimulation of filling diffusion  structures in very large wells. The additional TLS, at 1064 nm  wavelength usually handled as second order effect to PLS, is a  very good candidate to explain the observed global delay shift  effects. Most likely is an add up of the two possible  influences.


Photoelectric laser stimulation technique in CW and pulsed  mode is applied to a triple well technology ‘real’ IC for the  timing characterization. The investigated structure is a  multiplexer in a delay chain. Two measurement units are  employed: TAC in scan mode and high bandwidth  oscilloscope in single point mode.


A number of stimulation effects have been observed that  interfere or even mask the investigation of the desired devices. In order to sort out unwanted and misleading signal sources, the structures that cause a change in the switching speed are  localized and investigated. It is shown that there are some  undesired secondary effects (e.g. the stimulation at filling  structures or global delay shifts) that cause delay change. It is  also demonstrated that pulsed laser operation is able to  minimize these undesired effects.


The best way to avoid these side effects is to pulse the laser at  the switching edges of the investigated signals. It limits the  induced photocurrent or TLS effects on the secondary  structures and therefore the laser perturbations are more  localized.


[1] M.R.Bruce, V.J.Bruce, D.H.Eppes, J.Wilcox, E.I. Cole  Jr., P.Tangyunyong, C.F.Hawkins, Soft defect  localization on ICs, Proceedings of the 28th  International Symposium for Testing and Failure  Analysis (ISTFA), Phoenix, Arizona, pages 21-27,


[2] E. I. Cole Jr., P. Tanyunyong, C.F. Hawkins, M.R. Bruce, V.J. Bruce, R.M. Ring, W. Chong, Resistive  interconnect localization, Proceedings of the 27th  International Symposium for Testing and Failure  Analysis (ISTFA), Santa Clara, California, pages 43-50, 2001.


[3]  J.A. Rowlette and T.M. Eiles, Critical timing analysis  in microprocessors using near-ir laser assisted device  alteration (lada), Proceedings of the IEEE  International Test Conference (ITC), Vol.1, pages  264-73, 2003.


[4] K. Sanchez, R. Desplats, F. Beaudoin, P. Perdu, S. Dudit, G. Woods, D. Lewis, Dynamic laser delay  variation mapping (DVM) implementations and  applications, Proceedings of the 31st International  Symposium for Testing and Failure Analysis (ISTFA), Santa Clara, California, pages 106-114,


[5] E. I. Cole Jr., P. Tangyunyong, D. L. Barton, Backside  localization of open and shorted IC interconnections, 36th Annual IEEE International Reliability Physics  Symposium Proceedings, pages 129-136, 1998.


[6] Kevin Sanchez, Romain Desplats, Félix Beaudoin, Philippe Perdu, Sylvain Dudit, Michel Vallet, Dean  Lewis, Dynamic thermal laser stimulation theory and  applications, 44th Annual IEEE International  Reliability Physics Symposium Proceedings, pages 574-584, 2006.


[7] M.R.Bruce, V.J.Bruce, D.H.Eppes, J.Wilcox, E.I. Cole Jr., P.Tangyunyong, C.F.Hawkins, R. Ring, Soft  defect localization in integrated circuits using  scanning laser microscopy, The 16th Annual Meeting  of the IEEE Lasers and Electro-Optics Society (LEOS), pages 662-663, 2003.


[8]  R. A. Soref and B. R. Bennett, Electrooptical effects  in silicon, IEEE Journal of Quantum Electronics, Vol.23, Issue 1, Pages 123-129, 1987.


[9] Glowacki, A., Brahma, S.K., Suzuki, H., Boit, C., Systematic characterization of integrated circuit  standard components as stimulated by scanning laser  beam, IEEE Transactions on Device and Materials  Reliability, Vol. 7, Issue 1, pages 31-49, 2007.


[10] F. Beaudoin, R. Desplats, P. Perdu, C. Boit, Principles of Thermal Laser Stimulation Techniques, Microelectronic Failure Analysis Desk Reference, Fifth Edition, ASM International, pages 417-425,


2004.


# Dynamic power analysis under laser stimulation: a new Dynamic Laser Simulation approach


Dynamic power analysis under laser stimulation:


a new Dynamic Laser Simulation approach


A. Deyine, P. Perdu, K. Sanchez, J.C. Courrège


THALES & CNES (French Space Agency) Component Expertise Laboratory, Toulouse, France   amjad.deyinebarth@cnes.fr, +33 (0) 5 61 28 14 32


University Bordeaux 1, Talence, France


45            L H L H L L  L L L L L L 46            H H L H L L L L L L L L 47            L H L H L L L L L L L L 48


H L L H L L L L L L L L 49            L H L H L L L L L L L L 50            H H L H L L L L L L L L


H L H H L L L L L L L L


49            L H L H L L L L L L L L


50            H H L H L L L L L L L L


Current (mA)


Time (µs)


Trigger


Current


transition


SCOPE


Hall  Effect  sensor


TESTER


LSM


Conversion


program


embedded into the scope


translates variations into


an analogue signal


The analog signal is


correlated with the laser  beam position by the LSM  acquisition card. Result is a  binary image.


4 mA


0 mA


300ns


0ns


# Two-Photon Absorption Laser Assisted Device Alteration Using 1340nm CW Laser: Critical Timing Fault Isolation & Localization for 32nm MPU and Beyond


Two-Photon Absorption Laser Assisted Device Alteration Using 1340nm CW  Laser: Critical Timing Fault Isolation & Localization for 32nm MPU and Beyond


Baohua Niu, Pat Pardy, Joe Davis, Mel Ortega, Travis Eiles


Intel Corporation, 5200 NE Elam Young Parkway, Hillsboro, OR 97124


Baohua.Niu@Intel.com; Tel. (503)6134915; Patrick.Pardy@Intel.com; Tel. (503)7122834


In this paper, we report on the first observation and study of  two-photon absorption (TPA) based laser assisted device  alteration (LADA) using a continuous-wave (CW) 1340nm  laser. The study was conducted using LADA systems equipped  with high numerical aperture (NA) liquid and solid immersion  lens objectives on Intel’s 45 nm and 32 nm multiprocessor  units (MPU) and test chips. The power densities achievable  using these lenses are similar to those reported in the literature  for TPA in silicon of CW 1455nm light [1]. We show that the  induced photocurrent has a quadratic dependence on the input  laser power, a key indicator of two-photon phenomenon. Our  results imply that even when using 1340nm wavelength CW  lasers, there is a potential for laser invasiveness with the high  power densities achievable using high NA objectives. Laser  induced damage of the DUT is also a possibility at these high  power densities, particularly with the solid immersion lens (SIL). However, we show that the DUT damage threshold can  be increased by reducing the DUT’s temperature. Finally, we  present results demonstrating a >40% improvement in  localization of critical timing faults using TPA based LADA, when compared to traditional 1064nm wavelength (singlephoton absorption) LADA.


In LADA, a CW laser beam is scanned over the DUT to  perturb the timing of internal nodes of an IC through the  localized ‘injection’ of free-carriers [2]. The laser wavelength  of choice for this application has been 1064nm, which has  photon energy above the Si indirect band gap of ~1107nm. The absorption of 1064nm photons by Si generates free  carriers which are then swept into the source and/or drain of  the active CMOS transistors. These free-carriers temporarily  alter the transistor’s I/V characteristics, and therefore, their  switching behavior. When a node is in a critical timing path, the timing perturbation can cause the DUT to transition  between passing and failing modes of operation. The LADA  technique is thus an effective tool for localizing faults or  marginal transistors in critical timing paths that limit the  performance of the DUT.


Soft Defect Localization (SDL) is similar to LADA except that  it uses a longer wavelength laser to locally heat the DUT rather  than inject carriers [3]. A commonly used laser wavelength for


SDL is 1340nm, which has sub-bandgap photon energy. While  SDL can be effective at localizing temperature sensitive, noncatastrophic defects, we don’t find it particularly useful for  localizing circuit marginalities in non-defective DUTs due to  the small timing perturbations caused by temperature changes


[2].


Optical Beam Induced Current (OBIC) is another technique  based on perturbing a DUT with a scanning laser beam to  locate defects [4]. Like LADA, traditional OBIC uses a laser  wavelength capable of generating free carriers in Si through  single-photon absorption. Unlike LADA (and SDL) however, OBIC is a static technique in which the DUT is held in a fixed  state, instead of exercised functionally. TPA based OBIC in Si  has been reported on extensively (see, for example [5-8]). In  two-photon OBIC (TOBIC) a sub-bandgap laser wavelength is  used so that TPA processes are required to generate  appreciable levels of free carriers. A short-pulse mode-locked  laser, with pulse width typically ~100fs, is used to produce the  high peak power densities needed. High power densities (typically >10MW/cm2) are required because of the small TPA  cross section in Si (~1cm/GW [7]). TOBIC in Si using pulsed  lasers demonstrates improved spatial resolution in both the  lateral and longitudinal (along the beam focus) directions [8]. This improvement results from the fact that the required high  laser power densities for TOBIC only occurs at the focus of  the laser beam instead of throughout the whole beam, as in  traditional OBIC. A key distinction between the currents  generated by TOBIC versus OBIC is the quadratic dependence  of the TOBIC photocurrents on laser power, versus the linear  response for OBIC [7].


TPA with pulsed laser sources can also be applied to LADA. However, for a dynamic technique such as LADA, the use of a  pulsed source introduces complexities and limitations: If the  pulsed laser is free-running (pulses not synchronized to the  DUT activity) then the short laser pulses combined with the  relatively long period between pulses (order of 10ns) results in  a greatly reduced duty cycle. As a result, greatly increased  acquisition times are required for complete coverage of the test  pattern. On the other hand, synchronizing the free-running  laser pulses complicates the test setup and may not be possible  in certain test situations. In addition, to make efficient use of  the synchronized laser pulses, the approximate timing of the  problematic clock/data transitions must be known so that they  can be properly targeted (in time).


In this paper, we report, for the first time, the use of a CW  1340nm laser for TPA-based LADA. We show that the power  densities achievable through the use of high NA LIO and SIL  objective lenses is sufficient to produce useful levels of  photocurrent. CW TOBIC measurements on test chips confirm  the expected quadratic dependence of the TPA generated  photocurrent on incident laser power. Performing TPA-based  LADA with a CW laser bypasses the drawbacks of using a  short-pulse laser source while still providing the improved  localization inherent in TPA phenomenon. We demonstrate the  benefits of 1340nm CW TPA based LADA on Intel's 45nm  and 32nm MPUs and test chips.


The experimental setup consisted of the following, as  illustrated in Fig. 1:


• A high speed MPU/Test Chip tester (ATE) with  MPU/Test Chip loadboard and Tester Interface Unit (TIU)


• A LADA system with both LIO and SIL objectives, and  docking interface hardware to the tester


• A workstation to control the tester and the LADA system


• MPU and other test chips


Figure 1: Experimental setup for TPA LADA


a) Photocurrent versus laser power


To measure the photocurrent generated by single- and twophoton absorption in Si, a 32nm technology test chip with  externally accessible thermal diodes was used. The chips were  thinned down to ~50µm to reduce the absorption of near  infrared (NIR) light by the heavily doped Si substrate. The  thermal diodes were connected to a current amplifier in the  LADA system and were biased at 5mV to reduce noise. The  current amplifier used has a noise floor of approximately  10nA. Laser scanning microscope (LSM) reflected light  images of the DUT were first obtained to find the best image  focus position using either the 1064nm or 1340nm wavelength  laser. Then the laser probe beam was parked on the thermal


diode and the DUT refocused to maximize the photocurrent  signal. With the LSM focus fixed, the OBIC or TOBIC  currents were measured as a function of the input laser power. Figures 2-5 show the results of these measurements.


Figures 2 and 3 shows that the photocurrent generated using  the 1064nm CW laser is linearly dependent on the input laser  power. This is true regardless of whether the LIO or the SIL  objective was used. A linear dependence is expected for  single-photon absorption. The OBIC current was found to be  relatively insensitive to the focus settings: Up to a few tenths  of µm focus change produced negligible changes in the  measured current. Typical OBIC currents measured were on  the order of µA. It is also clear from the plots that the total  OBIC currents for the LIO and SIL are nearly the same (within  the measurement error of +/- 5%) for the same input laser  power. This shows that photocurrent generation is independent  of power density, which is also expected for single-photon  absorption.


Figure 2: 1064 nm OBIC photocurrent versus laser power  using the LIO. Note the slope of one in the log/log plot at the  bottom. A slope of one is expected for single-photon  absorption [7].


Figure 3: 1064nm OBIC photocurrent versus laser power  using the SIL. Note the slope of one in the log/log plot at the  bottom.


Figures 4 and 5 are plots of the corresponding TOBIC  photocurrents, generated using the 1340nm CW laser. These  plots clearly show that the generated TOBIC photocurrent is  nonlinear with respect to incident laser power. The log/log  plots show a slope of approximately two for both the LIO and  the SIL objectives, at the higher laser power settings. This  quadratic dependence is strong confirmation of TPA  generation of the measured photocurrents. Typical TOBIC  photocurrents measured are on the order of nanoamperes  which, as expected, are much weaker than the 1064nm OBIC  photocurrents for the same incident laser power.


The slight deviation from the slope of two, especially using the  LIO, is most likely due to DUT heating caused by single  photon absorption of the 1340nm laser beam. It is well known [9, 10] that at higher temperatures, Si absorption of 1340nm  photon increases significantly, which enhances both singlephoton and two-photon absorption by Si. Below, we expand  upon this point further.


Figure 4: 1340nm TOBIC photocurrent versus. laser power  using LIO. Note the slope of two in the log/log plot at the  bottom, which is expected for two-photon absorption  phenomena [7].


We believe that the damage to the thermal diodes is caused by  heating from single-photon absorption of the 1340nm CW  laser beam. As mentioned in the previous section, the  photocurrents generated by the 1340nm CW laser is on the  order of 10 to a few hundred nA. A simple photon flux  calculation shows that only a very small fraction of the  1340nm photons are involved in the actual TOBIC current  generation, as expected. (Out of 1mW of incident laser power,


only ~30nW, or 30ppm, is required to generate 10nA of  photocurrent). The vast majority of the photons are absorbed  by the Si substrate in single-photon processes, generating  localized DUT heating. (This heating process is the basis for  the SDL technique.) Lower temperatures reduces the heating  caused by single-photon absorption of the 1340nm laser beam  and facilitates the removal of any heat generated, by improving  the thermal conductivity of the Si substrate.


# FAILURE ANALYSIS POWER CYCLING TOOL - FAPCT


FAILURE ANALYSIS POWER CYCLING TOOL - FAPCT


Chua, Yi Yun


Intel Production (Malaysia) Sdn. Bhd.


Failure Analysis Power Cycling Tool – FAPCT is a software  tool developed for motherboard FA purpose to replicate a  customer reported failure. One of the major challenges for a  failure analysis engineer is being able to successfully replicate   a customer sighting.  Some customer issues are intermittent  and may only be replicated after a number of AC power  cycles.  Under these circumstances, FAEs (Failure Analysis  Engineers) need to identify differences between the two  environments as well as the customer’s use conditions.  This  information is crucial for the FAE to successfully replicate a  customer failure.


Basically, what the FAE must experiment by stressing the  Unit Under Test (UUT) using  different method in order to  duplicate the failure. One of these  methods to duplicate the  failure is to run AC on/off, in others words, AC cycling. This  is normally done manually which consumes a lot of human  resource time. Due to this overhead, an automatic way was  introduce to perform AC Cycling by using one of the FA  tools.


One of the problems for FA is to perform power cycling to  stress the motherboard in order to duplicate the failure. The  most basic way to perform power cycling is to request a  person to power on and off the board manually. This manual  method is not a good idea as the person has to sit on the same  place for hours or days. Power cycling tool was started to use  in Kulim’s FA Lab on 2007 where the software is running in  DOS mode and Marmitek hardware was purchase to use  together with the software to perform power cycling in the lab  to stress the UUT. There are some problems encountered with  the DOS version software. It is able to do the power cycling, but with two problems for FA.  The 1st problem is that, it did  not have any feedback to the Host PC therefore when there is   a failure occur during power cycle, the UUT  will not halt and  no record was capture  when the failure board is  fail. This will  not able to serve the power cycling purpose as FA engineer  might not know there has been a failure occur during the  power cycle. The second problem is the timing is not  synchronizing correctly. With these 2 reasons above, a user  friendly with extra feature program called FAPCT (Failure  Analysis Power Cycling Tool) was developed to resolve these  2 problems and enhance the AC cycling tools, which is more  suitable for FA purpose, where the software will not continue  to loop if there is any failure occurs on the UUT. Some others  improvement has done on the 1st version of the FAPCT. 2nd  version of the FAPCT improves on the interface and also fixes  some of the software bug which occurs on version 1.


FAPCT basically develop to communicate with Mamitek  CM11 and indirectly to control the UM7206 (Use to control  the front panel) and AM12 (Use to control AC power on and  off). The FAPCT is in GUI (Graphic User Interface) to let user  easier to control and setup the looping and the interface is as  below in Figure 1.


Figure 1:FAPCT Interface.


On occasions the FAPCT has proved to be an effective tool to  replicate customer failures particularly ideal for failures that  are intermittently failing.  These failures concerns (but not  limited to) power cycling failures after 1000 cycles and a  feature of this tool enables the FAE to freeze the failure at its  defective states at anytime during the power cycling process  when the failure suddenly occurs and provides the FAE the 1st  hand account “freeze in time” to performed the necessary  measurements and eventually speed up root cause finding.


With this hardware and software provide FAE one more  option to duplicate intermittent or other issue that need to do  power cycling to capture the failure. The hardware cost is only  about 600 USD which is consider at the lower cost hardware  for a FA tools to do power cycling although there is some  limitation compare to some hardware available in the market.


Have to thanks to Ooi Ping Ping who is providing technical  knowledge on programming and also giving all the  encouragement to start programming in C#. Also have to  thanks to my manager Tan, Chang Teong who always  provides input for improvement on the function of the  program. They are some other Khaw, Boon Chai and Lau, Chong Sheng also provide advice and technical knowledge in  C# programming.


# Advanced IR-OBIRCH Analysis Technique for High Isb Failure Analysis


Advanced IR-OBIRCH Analysis Technique for High Isb Failure Analysis


Kuo Hsiung Chen, Wen Sheng Wu, Yu Hsiang Shu, Jian Chan Lin


United Microelectronics Corporation, Tainan, Taiwan, ROC (kuo_hsiung_Chen@umc.com)


IR –OBIRCH (Infrared Ray – Optical Beam Induced  Resistance Change) is one of the main failure analysis  techniques [1] [2] [3] [4]. It is a useful tool to do fault  localization on leakage failure cases such as poor Via or  contact connection, FEoL or BEoL pattern bridge, and etc… But the real failure sites associated with the above failure  mechanisms are not always found at the OBIRCH spot  locations. Sometimes the real failure site is far away from the  OBIRCH spot and it will result in inconclusive PFA Analysis. Finding the real failure site is what matters the most for fault  localization detection


In this paper, we will introduce one case using deep  sub-micron process generation which suffers serious high Isb  current at wafer donut region. In this case study a BEoL Via  poor connection is found far away from the OBIRCH spots. This implies that layout tracing skill and relation investigation  among OBIRCH spots are needed for successful failure  analysis.


During VLSI (Very Large Scale Integrated circuits) process development, it becomes very important to quickly  find the process defect for yield improvement. The speed is  directly correlated to the yield learning cycle of the factory. Many PFA techniques are useful to inspect process defects  such as SEM (Scanning Electron Microscope), FIB (Focused  Ion Beam), TEM (Transmission Electron Microscope), etc… But how to locate the failure site is the major contributor that  determines the failure analysis success or failure. The  principal failure localization techniques include: SRAM  bitmap analysis, PEM (Photon Emission Microscopy), LCD (Liquid Crystal Detection), IR-OBIRCH, etc... In this paper, we will induce the IR-OBIRCH technique and apply it in deep  sub-micro process failure analysis case.


IR –OBIRCH is a useful tool to do fault localization  technique. But the real failure sites are not always at the  OBIRCH spot locations. Sometimes the real failure site is far  away from the OBIRCH spots location and the fault will be  lost by destructive Physical Failure Analysis (PFA) performed  at the OBIRCH spot positions.


This paper provides an example which combines some  tools such as layout tracing, circuit repair, micro probing, etc… to confirm the real fail location. A detailed analysis of


high Isb current failure at wafer donut region in a deep submicron process is presented.


I. IR-OBIRCH Spot Locations vs Real Failure Sites


A new deep sub-micron pilot product suffered serious  yield loss with the major yield loss being about 60% compared to normal wafers. The major failure modes include  functionality as well as DC failures. By current map analysis, the donut-shape leakage signature is strongly related to Isb  current Two-pin OBIRCH probing method is utilized for fault  localization although no suitable Isb program is available. Five suspicious OBIRCH spots were observed at B/Ds  comparing to G/Ds (see Figure 1-2). But no visible defect can  be found after layer by layer inspection including plain-view  SEM, cross-sectional FIB (X-S FIB), C-AFM, and even nano  probe. This essentially questioned whether the OBIRCH spot  locations are at real failure sites or not.


Figure 1: The I-V characteristic curve shows the difference  between G/Ds and B/Ds


(a)                                              (b)


Figure 2: The backside IR-OBIRCH images show the


difference between G/D and B/D: (a) G/D sample, (b) B/D  sample


II. OBIRCH Spot Investigation by Layout Tracing


Circuit repair by FIB and voltage Layout tracing method  is useful to investigate the relation “among” multiple  OBIRCH spots. In this example, by zooming in the layout  around these five OBIRCH spots, it reveals that all OBIRCH  spots are related to similar CMOS circuits. Utilizing LAKER  software for layout tracing, these OBIRCH spots are  confirmed to be controlled by a series of (M5) signal lines  through layout paths (see Figure 3). Therefore, it is highly  suspected that M5 control line signal loss is the root cause of  high Isb current, and OBIRCH spots are just a phenomenon of  gate floating. CMOS poly gate floating will induce tri-state  and cause a leakage path from VDD to VSS.


III. Signal Level Confirmation by Micro Probe


To confirm the M5 control line signal loss issue, circuit  repair by FIB (see Figure4) and voltage measurement by  micro probe was performed. After parallel lapping to M6  layer, the probe pads of M5 signal lines are pulled out through  the dielectric layer above M5 and through M6 both G/Ds and  B/Ds. The electrical characteristic of suspected failure device  could then be measured by either C-AFM or Nano-Probing  system.


Figure 5: 1340nm TOBIC vs. laser power using SIL. Note the  slope of two in the log/log plot at the bottom.


The TOBIC currents are very sensitive to focus and are orders  of magnitude weaker than the OBIC currents. Both of these  factors contribute to larger measurement errors of the TOBIC  currents. To minimize the effects of focus drift during the  measurements, the focus is adjusted slightly after each change  in power level to maximize the TOBIC current. The current  amplifier noise floor of 10nA sets the limit on the accuracy of  the current measurements at the lowest power settings.


Note that for the same incident laser power, the TOBIC  currents measured when using the SIL are significantly higher  than those measured when using the LIO. This is expected for  TOBIC current generation because the SIL NA is significantly  greater than that of the LIO. Higher NA leads to higher power  densities, and thus, increased TPA photocurrent generation  efficiency.


b) Temperature-dependent laser-induced damage


We did not observe any 1064nm CW laser induced damage to  the diode test structures over the power output range  obtainable from both the LIO and SIL. For LIO this  corresponded to ~50mW, while for the SIL, it corresponded to ~20mW. The SIL has much lower output power due to the low  NIR transmission of the SIL’s backing objective. With the  1340nm CW laser, however, permanent damage to the diode  occurred at ~45mW with the LIO, when the diode was at room  temperature (~25C). With the SIL, damage occurred at ~15mW at the same temperature. When damage occurs, the  diode PN-junction shorts, and even with zero laser power, the  current measured is greater than 200µA (the compliance limit  of the current amplifier.)


Using Intel-developed thermal solutions, we lowered the DUT  temperature to about -10C to investigate the temperature  dependence of the device damage threshold, and of the OBIC  and TOBIC currents. The sample chamber was purged to  prevent frosting, and the DUT temperature was measured with  thermal couples mounted as close to the diode test structures  as practical. At -10C, we did not observe any damage to the  diodes with the 1340nm CW laser using the LIO with up to  100mW power. Using the SIL, no damage was observed up to  the maximum power output of ~20mW.


Figures 6 and 7 shows plots of the measured OBIC and  TOBIC photocurrents as a function of incident laser power at  the two different temperatures, for the SIL. In general, we find  that the OBIC and TOBIC currents generated using the  1064nm and 1340nm CW lasers, respectively, decrease with  temperature.


Figure 6: 1064nm OBIC photocurrent generation using the  SIL at two different temperatures.


Figure 7: 1340nm TOBIC photocurrent generation using the  SIL.at two different temperatures.


c) Single-photon versus two-photon LADA localization


For the data presented in this section, a voltage/frequency “Shmoo” is first run to find the marginal settings of the device  under test (DUT). The DUT’s voltage and frequency is then  fixed at a pass/fail boundary and the pattern is looped  repetitively. The LSM is then used to scan the laser beam over  the region of interest (ROI) and the pass/fail state of each  repetition of the test pattern is plotted as a function of beam  position. The reflected optical images are used to align the  ROI to the CAD database, using the 1064nm CW laser. The  LADA ‘hit-zones’ are then overlaid with the CAD database  and LSM image to localize and identify the failing/marginal  circuits. Then, we switch to the 1340nm CW laser, optimize  focus, based on the LSM image, and slowly increase the laser  power while monitoring the pass/fail condition. Once clear  LADA hits are obtained, they are overlaid with the previously


obtained optical image and CAD overlay to pinpoint the  failing devices. The DUT temperature control is typically set  at 25C for the examples given here.


Figure 8 shows an example ROI for an Intel 45nm MPU, taken  using the 2.45 NA SIL. As can be seen in the LADA maps, the  TPA generated hit-zone, using 5mW of 1340nm CW laser  power, is less than 40% of the area generated using 1.5mW of  1064nm CW power. At the same time, the signal-to-noise ratio  of the LADA map generated using the 1340nm laser is similar  to the 1064nm map. This indicates that the improved  localization obtained by using the 1340nm laser is not simply  due to a reduction in the amount of photocurrent generated [2] but is due to the localized nature of the TPA generated  photocurrent [7].


Figure 8: Comparison of the LADA hit-zone for both the  1064nm CW laser (left side) and 1340nm CW laser (right  side). A 45nm MPU and a 2.45 NA SIL equipped LADA tool  were used for this example.


Figure 9 below shows a second LADA ROI on the same MPU  as in Figure 8. Again the 1340nm TPA-LADA hit-zone is, on  average, <=40% of the area generated using the 1064nm laser. Besides the reduction in hit-zone area, also note the  dramatically improved signal-to-noise ratio (SNR) of the  LADA map generated using the 1340nm laser.


Figure 9: Comparison of a second LADA ROI on the same  MPU and using the same setup as in Figure 8.


Figure 10 below shows the effects of increasing 1340nm laser  power for the ROI shown in Fig 9. It is clear that the SNR  increases dramatically with laser power. The improvement is  even greater than apparent from the images because the  number of accumulated ROI scans is actually reduced at  higher powers: 20 scans were accumulated at 3 mW, 10 scans  at 5 mW, and 5 scans at 10mW. In all cases, the test conditions  were kept the same.


Figure 10: LADA ROI showing effect of increasing the  1340nm laser power. Laser power increases from left to right. A dramatic improvement in LADA hit-zone SNR is apparent at  higher laser power.


Figure. 11 below shows two more examples of ROI’s on an  Intel 32nm MPU using the 1.4 NA LIO objective. As with the  SIL, the 1340nm CW laser generated TPA-LADA hit-zones  are considerably reduced compared with the 1064nm CW  laser.


Figure 11: Comparison of the LADA hit-zones using the  1064nm CW laser (left) and 1340nm CW laser (right) for a 32  nm MPU with LIO equipped LADA tool.


Figure 12 below shows the LADA hit-zones of Fig. 11 as a  function of 1340nm laser power. Again, the SNR of the LADA  hit-zones is seen to dramatically increase with increasing laser  power. At 30mW, the weak hit-zone that is barely visible at  12mW becomes clearly isolated (left spot in the right-most  image).


Figure 12: By increasing the 1340nm laser power, the SNR  increases dramatically.


Conclusions and discussions


We have demonstrated, for the first time, that TPA phenomena  in Si is possible using high NA LIO and SIL objective lenses  with a 1340nm CW laser. TOBIC measurements show the  characteristic quadratic dependence of the TPA generated  photocurrent on laser power. The application of TPA to  LADA was demonstrated by showing examples from the  debug of Intel 45nm and 32nm MPUs. The dramatic  improvements in localization and SNR that resulted, compared  with single-photon LADA using 1064nm wavelength, shows  the benefit of TPA-LADA.


We find that the device damage threshold is lower for 1340nm  wavelength than for 1064nm. We speculate that single-photon  absorption of the 1340nm beam locally heats the DUT and


generates the damage. Temperature dependent studies show  that lowering the DUT temperature raises the DUT damage  threshold. This finding gives us directions for future  improvements of the TPA-LADA technique: Using  wavelengths that have minimum single photon absorption  1150nm to 1250 nm (but with photon energy still below the Si  indirect band gap) should increase the DUT damage threshold. Using a pulse-on-demand laser source that is synchronized  with the tester pattern would reduce the average power  incident on the DUT considerably, and therefore also reduce  DUT damage. These improvements are expected to enable this  technology to be broadly applicable to future generations of  CMOS and MPU fault isolation and critical timing debug  applications.


The size of the LADA hit-zone is a complex function of the  optical spot size, photocurrent generation volume, carrier  thermal diffusion length, and test conditions [2, 11]. It was  beyond the scope of this paper to attempt a detailed theoretical  analysis for comparison against our experimental results. Such  an analysis is planned for a subsequent paper.


The authors would like to acknowledge workers in Intel's  debug and fault isolation communities for in-depth technical  discussion and support with the experimental setup, especially  the LTD QnR group: Mitch Sacks, Tony Peterson, and Joe  Basile; PTD LYA group:  Dr. Martin von Haartman; Israel  Design Center:  Evgeny Nisenboim, Gila Yampolski and Eli  Abuayob; Folsom Debug Lab:  Jerry Fortier; and Chandler  Debug Lab: Tom Begala.


[1] H. Rong, et al., “Raman gain and nonlinear optical  absorption measurements in a low-loss silicon  waveguide,” Appl. Phys. Lett., 85(12) 2004, pp2196-8.


[2] J. Rowlette and T. Eiles, “Critical Timing Analysis in  Microprocessors Using Near-IR Laser Assisted Device  Alteration (LADA)”, Proc. International Test Conference  2003, pp 264-73.


[3] M. Bruce, et al., “Soft Defect Localization (SDL) on ICs.” Proc. 28th International Symposium for Testing and  Failure Analysis, 2002, pp 21-27


[4] E. I. Cole, Jr., “Beam-Based Defect Localization  Methods,” Microelectronics Failure Analysis Desk  Reference, 5th Ed., pp406-16.


[5] K. A. Serrels, et al., “70nm Resolution in Subsurface  optical imaging of silicon integrated-circuits using pupilfunction engineering,” Appl. Phys. Lett., 94(073113) 2009, and references cited therein.


[6] C. Xu and W. Denk, “Two-photon optical beam induced  current imaging through the backside of integrated  circuits,” Appl. Phys. Lett. 71(18) 1997, pp 2578-2580.


[7] C. Xu and W. Denk, “Comparison of one- and two-photon  optical beam-induced current imaging,” J. Appl. Phys., 86(4), 1999, pp 2226-2231, and references cited therein.


[8] E. Ramsay, et al., “Three-dimensional nanoscale  subsurface optical imaging of silicon circuits,” Appl. Phys. Lett., 90(131101) 2007.


[9] M. A. Green, “Self-consistent optical parameters of  intrinsic Silicon at 300K including temperature


coefficients,” Solar Energy Materials & Solar Cells 92, 2008 pp1305-1310.


[10] P. E. Schmid, “Optical absorption in heavily doped  Silicon,” Phys. Rev. B. 23(10) 1981, pp5531-6, Fig.  2


[11]  A. Mels and F. Zachariasse, “Reduction of Acquisition  Time for RIL, SDL, and LADA,” Proc. International  Symposium for Testing and Failure Analysis, 2007, pp6-13


FAPCT allow FAE to do more looping compare to manual  and also able to know if there is any failure occur instate of


after the failure has occur, and the UUT is continue to loop  and the failure disappear again. For the latest FAPCT software  also include a video function so that when there is a failure  occur, the HOST PC is able to capture a photo of the UUT  POST CODE through a webcam before continue doing the  loop. The photo is saved in the format of time and date of the  failure occurs so that FAE can base on the date to analyze how  frequent the failure will occur. By having the webcam  connected to the HOST PC, FAE is able to remote access to  the HOST PC and see the status of the board through the  webcam that had already setup.


According to micro probe results (see Table 1), the  voltage potential of these M5 signal lines at G/Ds are  positioned at high voltage level (1.5V). But at B/Ds with  abnormal OBIRCH spots, improper voltage levels at M5  signal lines is measured. At high voltage level (1.5V)the  measured voltages at different location all highlight significant  voltage drop, 1.2V, 0.6V to 0.5V, even 0V. These improper  voltage levels will result in insufficient gate voltage control, causing N-/P-MOS turn on or VDD leakage to VSS directly, and then resulting in high Isb current. Therefore, multiple  OBIRCH spots are detected.


Figure 3: The pictures compare the backside I-R OBRICH  spot and layout position. (a) 1X I-R OBIRCH image  (b) 1X  layout image (c) 20X I-R OBIRCH image  (d) 20X layout  image  (e) 100X I-R OBIRCH image  (f) 100X layout image


(a)                           (b)                               (c)


Figure 4: The picture shows the circuit repair position (a) low  mag. layout (b) high mag. layout (c) circuit repair position


Table 1: The table shows the potential of M5 signal lines.


RESULTS AND DISCUSSION


To further verify the above electrical findings, FIB  passive voltage contrast (PVC) method is applied here. PVC  images reveal some gray or dark Via-4 patterns (see Figure 5) under M5 signal lines. It means either Via-4 high resistance, open, or poor connection to below metal/poly layers. These  Via-4 patterns are layout connected to the OBIRCH spot sites  for CMOS gate control. CMOS poly gate floating will induce  tri-state and cause a leakage path from VDD to VSS.


Using cross sectional FIB and TEM inspection, it was  found that insufficient Via-4 etching caused the Via-4  formation to be stopped on the nitride cap layer above the M4  layer. This remaining thin nitride layer is not easy to be  observed by cross sectional FIB but TEM and EELS mapping  analysis show clear evidence of the remaining thin nitride  layer (see Figure 6).


(a)                                                (b)


Figure 5: The pictures show Via-4 FIB PVC and layout  position. (a) Layout position (b) FIB PVC position


(a)                                                 (b)


(c)                                                (d)


Figure6: The pictures show via-4 X-S profile and EELS  mapping.  (a) Via-4 X-S FIB profile of G/D. (b) Via-4 X-S FIB  profile of B/D (c) Via-4 X-S TEM image of B/D (d) N EELS  mapping image


In this paper, a failure analysis case study of deep submicron product with high Isb failure was presented. While IROBIRCH is a useful tool for fault localization, the spot  locations do not always indicate the real physical failure site. Sometimes, the real failure sites are far away from spot  locations. With the help of layout tracing, the relation between  multiple IR-OBIRCH spot locations and real failure sites can  be correlated. Eventually, the failure analysis cycle time can  be greatly reduced and success rate can be greatly increased.


Reference


[1] Cha-Ming Shen. , et a1. “ Combine Micro-probing  and OBIRCH to Catch Non-recognizable Fault in RF and  Mixed-Mode Integrated Circuits” IEEE IPFA, p.214, 2007


[2] J.Y. Liao. , et al. “ OBIRCH analysis of electrically  stressed advanced graphic Ics”  ESREF, p.1575, 2007


[3] R. Ross. , et al. “ OBIRCH driver Failure Analysis for  Process Development of 120nm to 65nm technology nodes”  ISTFA, p.447, 2004.


[4] Chi-Lin Huang. , et al. “ A Novel OBIRCH Fault  Isolation Method to Locate the Leakage Failure Point”  ISTFA, p.269,2008.


# Using Nano-Probing Technique to Clarify Nickel Silicide beyond Process Window Causing Device Failure


Using Nano-Probing Technique to Clarify Nickel Silicide beyond Process  Window Causing Device Failure


Jian-Chang Lin, Wen-Sheng Wu


(Jian_chang_lin@umc.com)


A scanning electron microscopy (SEM) based  nano-probing system is used in this study to clarify nickel  silicide phase beyond process window. According to the  nano-probing measurement result and the cross-sectional  transmission electron microscopy (TEM) images, phenomena  of junction leakage along with high resistance and a larger  nickel silicide area are observed at failure site at the same  time.


The type of failure mechanism and in-line process issue  caused multiple failure phenomena at failure site will be the  major focuses in this paper. Nickel silicide phase  transformation from NiSi to NiSi2 is highly suspected by the  comparison of sheet resistance and silicon consumption. Consequently, nickel silicide beyond process window could be  verified immediately.


By the demand of chip size shrinkage and device high  performance, semiconductor technology has made further  progress to achieve the objective. For the device necessity in  advanced process, silicide formation has been migrated from  titanium silicide, cobalt silicide to nickel silicide. In current  advanced process, NiSi is preferred due to its low sheet  resistance, low silicon consumption, and low junction leakage  current. The sequence of silicide formation between a nickel  film and silicon substrate is well known: Ni2Si forms at ~200°C, followed by NiSi at ~400°C, and finally NiSi2 at ~700°C. [1] A two-step rapid thermal processing (RTP) program for nickel silicide formation is shown in Fig. 1. For  advanced technology, a millisecond anneal (MSA) machine is


introduced to RTP-2 process to meet process window on NiSi  formation without nickel silicide agglomeration and additional  nickel piping. [2]


Here, we will focus on how to clarify nickel silicide  phase beyond process window by electrical data and try to cite  reported literature about nickel silicide phase experiments to  explain physical failure analysis (PFA) findings in this study. Therefore, a SEM based nano-probing system is used in  failure device measurement that provides a clear and detailed  electrical data as electrical evidence.


Fig.1 A two-step program for nickel silicide formation [1]


Some failure samples with nickel silicide formation  process and MSA power control process are adopted in this  study.


First, A SEM based nano-probing system is used to  measure failure bit. A failed NMOS transistor I-V  characteristic curve is shown in Fig. 2 and junction


measurement result is shown in Fig. 3. According to the I-V  curve, drain sweep current reaches saturation but gets a low  turn-on current performance at operation voltage. Source  sweep behaves linearly at operation conditions but leaks to  silicon bulk observed by junction measurement. Referring to  the mathematical model, lower turn-on current could be  caused by high resistance existing at n-channel source site. [3] But what is the possible failure mechanism of high junction  leakage current? By cross-sectional TEM image, it reveals a  larger nickel silicide area as shown in Fig. 4. Besides, another  failure sample after chemical stain etching also shows an  abnormal nickel silicide area by cross-sectional SEM  inspection. (Fig. 5) Thus, higher leakage current may be  explained by ideal diode equation, and a larger junction area  matches a larger reverse current.


The ideal diode equation is given by:


Is = Js*A*(e qV/ kT-1)


Where


Is : reverse saturation current


Js : reverse saturation current density


A : interface area of P-N junction


(a)                       (b)


Fig.2 (a) Drain sweep I-V characteristic curve, (b) Source  sweep I-V characteristic curve at failed NMOS transistor by  SEM based nano-probing system measurement. According to  mathematical modeling, high resistance phenomenon exists at  n-channel source site.


Fig.3 (a) Drain site junction measurement (n+ to P-Well), (b) Source site junction measurement at failed NMOS transistor  by nano-probing system, higher junction leakage current is  found at source site.


Fig.4 Under contact failure site-1 shows larger nickel silicide  area than nearby normal site-2 by cross-sectional TEM. The  red circle emphasizes nickel silicide encroaching on the  n-LDD region.


Fig.5 Another failed sample after chemical stain etching  followed by cross-sectional SEM inspection. By comparing  failure site (a) and normal site (b), a larger nickel silicide area  at failure site is confirmed. (Indicated by red arrow)


Root Case Investigation


To investigate high resistance phenomenon from nickel  silicide formation, some reported studies of nickel silicide  phase diagram will be proposed to explain PFA findings in this  paper. According to FA experience, a blocked n-LDD  implantation could be modeled as a larger resistor [3] and here  an obvious nickel silicide encroaching n-LDD region is found  by TEM image. It is reasonable to consider nickel silicide  phase has been transformed from NiSi and then induced  higher resistance than original n-LDD implantation.


Besides, a larger nickel silicide area represents more  consumption of Silicon substrate. According to sheet  resistance and volume consumption of nickel silicide phases  comparison table [4], all phenomena indicate nickel silicide  out of process window, and NiSi2 is the most possible  candidate due to its higher sheet resistance and larger silicon  consumption than NiSi. Even though, it can just be said that  nickel silicide out of process window unless each nickel  silicide grain has been analyzed by further studies such as  microdiffraction by TEM or other phase analysis methods. [5]


Phase Resistivity (μΩcm) Silicon consumed/ Ni  NiSi


10.5-18


1.83


NiSi2


34-50


3.66


Table 1: A comparison of physical properties of nickel silicide  phases extracted from JCPDS [4]


In advanced semiconductor process, the well-used MSA  technique owns its advantage during nickel silicide formation  but it would lead to higher junction leakage current due to  improper power control. In this study, an electrical I-V  asymmetry behavior of transistors would cause device failure. An unexpected nickel silicide phase transformation  would cause higher sheet resistance and larger silicon  consumption, and then induce asymmetry device behavior and  higher junction leakage current. A SEM based nano-probing  system and cross-sectional TEM are good tools for above  failure observations.


[1] S. H. Chen, L. R. Zheng, C. B. Carter, and J. W. Mayer “Transmission electron microscopy studies on the  lateral growth of nickel silicides”, J. Appl. Phys., Volume 57 (2), 15 January 1985, pp. 258-263.


[2] Y. W. Chen, et. Al,  “Advances on 32nm NiPt  Salicide Process” 17th IEEE International Conference on  Advanced Thermal Processing of Semiconductors - RTP 2009, pp. 1-4.


[3] Cha Ming Shen, Tsan Chen Chuang, Shi Chen Lin, Lian Fon Wen, and Chen May Huang, “Combining the  Nano-Probing Technique with Mathematics to Model and  Identify Non-Visual Failures”, ISTFA 2007, pp. 214 –218.


[4] L. J. Chen, “Silicide Technology for Integrated  Circuits”, Processing Series 5, pp. 101 –102.


[5] B. A. Julies, D. Knoesen, R. Pretorius, and D. Adams, “A study of the NiSi to NiSi2 transition in the Ni-Si binary  system”, Thin Solid Films 347, 1999, pp. 201 –207.


# Fault Isolation on High Resistance Failure of 45nm ET Via Chains Using Combined Technique of SEM PVC and Nanoprobing


Fault Isolation on High Resistance Failure of 45nm ET Via Chains Using  Combined Technique of SEM PVC and Nanoprobing


P.K. Tan, Z.H. Mai, Y.W. Goh, L. Zhu, S.L. Toh, Q. Deng, R. He, H. Tan,  H.L. Li, Q.F. Wang, Y.Z. Ma, W.Y. Lee, G.R. Low, Jeffrey Lam.


Electrical Test (ET) structures are used to monitor the health  and yield of a process line. With the scaling down of  semiconductor devices to nanometer ranges, the number of  metal lines and vias increase. In order to simulate the  electrical performance of devices and to increase the  sensitivity for line health check, ET structures are designed to  be more complicated with a larger area. Hence, fault isolation  and failure analysis become more challenging. In this paper, the combined technique of Scanning Electron Microscope (SEM) Passive Voltage Contrast (PVC), Nanoprobing  technique, and Divide and Conquer Method (DCM) are  proposed to locate open failure and high resistance failure in  an ET via chain.


One of the common ET structures is the via chain. The  objective of via chains is to monitor the resistance of given  structures for each process layer, especially Back End Of Line (BEOL). Laser scanning microscopy (LSM), focused ion  beam (FIB), circuit edit (CE) and SEM are the commonly  used techniques to isolate the failed location with high  resistance failure. Among all the techniques, SEM PVC is  widely used to identify open issue and high resistance issue [1-2]. The advantage of SEM PVC is easiness of adoptability, non destructive and high resolution compared to the other  techniques. PVC is based on the number of collected  secondary electrons (SEs) generated when electron beam (ebeam) from source interacts with the sample’s atom. If an ebeam energy is low (<2kV), the number of SE excited from  the sample surface is more than that of incident primary beam  electrons. In this situation, net positive charge accumulates on  the surface, which may cause attraction to the emitted  electrons. On a floating structure, the positive charge has no  path to the ground, hence generated SEs are prevented from  leaving the specimen surface by the positive electric field, as  shown in Fig. 1(a). In this way, less SEs are collected by the  detector and it appears darker in the SEM image. For a  grounded structure, the excess positive charge is carried away  to ground resulting in less positive charge on the surface. It  allows SE to escape easily from specimen as shown in Fig. 1(b). Hence the structure appears brighter in SEM images. With the differences in brightness of floating and grounded  structure, an open location can to be isolated.


The increases in the size, and the number of metal lines and  vias of ET structures result in a simultaneous increase of the  resistances of a via chain (Fig. 2(a)). The conventional PVC  method becomes difficult to locate an open structure, especially a marginal high resistance failure. Nanoprobing  PVC was commonly used on DRAM, but was not reported on


the isolation of the open failure or high resistance failure of  ET via chains.


In this paper, the PVC method for a conventional open issue  and SEM-based nanoprobing to identify high resistance issue  on leading edge technology nodes ET via chains will be  discussed.


Figure 1 (a) When e-beam enters a floating structure, the  charge accumulate on the surface resulting generated SEs are  prevented from leaving the specimen surface. (b) As e-beam  enters a grounded structure, positive charges discharge to  ground so that the SEs leave easily specimen surface.


Figure 2 (a) Simple illustration of ET via chain and its  equivalent circuit. When resistance from point B to ground is  too large, less positive charges discharge to the ground, resulting in decrease in the voltage contrast (VC) at the  interface, especially in a marginal high resistance issue. (b) Simple illustration of the proposed solution for indistinctive  PVC problem on an open failure or high resistance failure.


Experimental results and discussion


Conventional PVC method to identify the open location in a


0.11um technology ET via chain.


Figure 3(a) shows a typical floating ET via chain structure. To  create PVC in the failed ET via chain, one of the pads must be  grounded. Normally grounding technique with laser zapping  is used; Laser zapping will melt the metal of each layer and  ground the pad to substrate. Figure 3(c) shows dark and bright  PVC observed on the floating and grounded pads which were  zapped with laser respectively.


Figure 3 (a) A typical ET via chain structure. (b) Equivalent  circuit of ET via chain as shown in Fig. 3 (c).


Figure 3 (c) SEM images of dark and bright PVC that  observed on the floating and grounded pads which were  zapped with laser respectively; And cross-sectional TEM  images at the dark/bright PVC interface.


Figure 3(b) is the equivalent circuit of the via chains. If open  occurred at point A (Fig. 3(b)), the via chain from point A to  Pad 1 was a floating structure which caused dark PVC as  shown in Fig. 1(a). The via chain from Point A to Pad 2 is a  grounded structure and results in brighter contrast as shown in  Fig. 1(b). The discontinuity at the interface between the bright  and dark metal will be the open location in the ET via chain (Fig. 3(c)). The cross-sectional Transmission Electron  Microscopy (TEM) image at the dark/bright PVC interface  was shown in Fig. 3(c). The result shows that unlanded via  was the root cause of the open failure.


Nanoprobing PVC method to isolate high resistance failing  location in 45nm ET via chain.


With the increase of the number of vias and metal lines in an  ET via chain, the resistances of the via chains will increase as  illustrated in Fig. 2(a). When the resistance increased, less  positive charges discharge to the ground, resulting in a  decrease in the voltage contrast (VC) at the interface, especially in a partially open failure. Figure 4 (a) and (b) show  PVC at an open location of a 65nm and a 45nm via chain  respectively. Figure 4 (a) and (b), clearly show that VC  decreased with the increase of the via chain length and the  decrease of the size of the vias and metal lines.


Figure 4 (a) SEM and TEM results on 65nm ET via chain  open issue. Unlanded via found at the dark/bright PVC  interface. (b) SEM and TEM results on 45nm ET via chain  open issue. Corrosion occurred in via was found at the  dark/bright PVC interface.


To solve this problem, SEM-based nanoprobing PVC  technique was used. The nanoprobing system used is a FEI  NOVA SEM equipped with a Zyvex KZ100 nanoprober.


Figure 5 (a) SEM PVC image on high resistance failure of ET  via chain. No dark/bright PVC interface found. (b) SEM  results using combination of SEM PVC and nanoprobing. Dark/bright PVC interface appeared in SEM image once  grounded nanoprobe tip landed near the high resistance  location.


Figure 5(c) TEM and EDX results at the interface area shows  unfilled via is the root cause of the high resistance issue.


Figure 2(b) shows the simple illustration of the proposed  solution for indistinctive PVC problem on high resistance  issue. When grounded nanoprobe tip landed near the open  location, positive charges are easier to be discharged to


ground through the nanoprobe tip which has lower resistance. This method enhances the VC at the junction between the  floating and the grounded structure. Figure 5(a) shows the  PVC images of a 45nm ET via chain which failed high  resistance. For this case, there is no PVC found using SEM  and FIB. After landing a grounded nanoprobe tip near the  high resistance location, the dark and bright PVC interface  appeared clearly as shown in Fig. 5(b). Figure 5(c) shows the  TEM and Energy Dispersive X-Ray spectroscopy (EDX) results at the interface location, no Copper (Cu) is detected at  the via area of point 3 in Fig, 5(c). Unfilled via is the root  cause of the high resistance issue. To find the high resistance  location, Divide and Conquer Method (DCM) is used [3]. DCM will be explained in next case study.


Nanoprobing DCM to isolate the high resistance failing  location in a 45nm ET via chain with no PVC detected.


The last case study is a very marginal high resistance failure  of an ET via chain. The specification of the passing die is  105ohm, while the resistance of the failing die is 107ohm. No  PVC can be found with SEM, FIB and Nanoprobing PVC  method. To locate the failing site, Divide and Conquer  Method (DCM) was used. A DCM works by recursively  breaking down a problem into two or more sub-problems of  the same (or related) type, until these become simple enough  to be solved directly. Figure 6 is the simple description of the  DCM. The high resistance location was isolated by measuring  the resistance with nanoprobing DCM as shown in Fig, 7(a). TEM result in Fig. 7(b) and (c) shows that the partial filled via  is the root cause of the high resistance failure. Figure 7(d) shows the EDX result on the partial fill via. The Cu element  count at point 2 and 3 is less compared with point 1. From the  reference via image in Fig. 7(c), the etching level of defective  via is lower compared to reference via. The root cause of this  sample is same as previous example as Fig. 5(c), both suffered  via blocketch by particle and cause partial filled via. The  resistance of this sample is lower compared with previous  sample in Fig. 5(c), this is because of the partial filled via is  less severe. The process issue has been improved after  feedback, no high resistance failure is reported on this via  chain ET.


Divide and Conquer Method:


Each black dot represents a nanoprobe point.


• First divide A1-B1 into two by A2.


• If resistance of A1-A2 > B1-A2, then continue divide A1-A2 into


two by A3.


• If resistance of A1-A3 > A2-A3, then continue divide A1-A3 into


two by A4.


• Continue dividing the area into two, finally high resistance


location is able to be isolated.


Figure 6 Divide and Conquer Method (DCM). A method used  to isolate high resistance location of an ET via chain that  failed high resistance.


Figure 7 (a) SEM image of nanoprobing with DCM. (b) TEM  results on the isolated high resistance location with DCM. (c) Bright and Dark field TEM images of via etching level on  reference and defective via.


Figure 7 (d) EDX result on the defective via.


A combination of SEM PVC and nanoprobing, together with  the DCM to locate high resistance failure in ET via chain  structure were demonstrated. Nanoprobing PVC technique is a  good alternative way to isolate the location of an open or high  resistance failure, especially without the assistance of Electron  Beam Induced Current (EBIC) or Electron Beam Absorbed  Current (EBAC). For a marginal high resistance failure, we  believed that nanoprobing with DCM is the best way among  all techniques.


Defect via


Reference via


The authors would like to thank Globalfoundries Ltd., Singapore TEM FA team for their great support.


[1] V. Liang, H. Sur, S. Bothra, “Passive Voltage Contrast  Technique for Rapid In-line Characterization and Failure  Isolation During Development of Deep-Submiscron ASIC  CMOS Technology”, ISTFA 1998, Proceedings, pp. 221-225.


[2] R. Rosenkranz, W. Werner, “Comparison of Active and  Passive Voltage Contrast for Failure Localization”, ISTFA 2007, Proceeding, pp. 331-336.


[3] Thomas H. Cormen, Charles E. Leiserson, and Ronald L. Rivest, Introduction to Algorithms (MIT Press, 2000)


# DETECTING INTERNAL ÏESD-LIKEÓ DAMAGE ON CMOS GATES


DETECTING INTERNAL “ESD-LIKE” DAMAGE ON CMOS GATES


M. Gores1, H. Dicken2


1Hi-Rel Laboratories, Inc, Spokane, WA 2DM Data, Inc, Scottsdale, AZ


INTRODUCTION


Normally ESD type of damage will be located near  the bonding pads for the input pins.  However, there  have been several recent cases where ESD type


damage has been detected on CMOS gates at


internal locations on the die, two or more transistors  away from any input or output pin.


This paper will describe two examples of this type  of failure and the unique approaches to the analysis  and the special procedures needed to locate the


damage sites.


EXAMPLE OF THE TYPE OF PROBLEM


Figures 1 and 3 show the location on the die where  a leaky N-channel gate was detected.  Note that the  location is in a series of logic cells and is not near  any input bonding pad or pin.  Figure 2 is a closer  view of the gate.


The key problem is to develop the most efficient


and effective sequence of failure analysis steps to


determine and prove this location.


Figure 1


Figure 2


SEQUENCE OF STEPS


Normally the following “safe sequence” of analytic  steps is used to determine the failure mode, the


failure mechanism and the probable cause.  The


goal is to obtain the maximum amount of


information without changing failure mechanism or  destroying the device.  The approach is a sequence  of steps ranging from benign to destructive as


shown below.


BENIGN


Device data, description of the problem


and history from the customer


External visual inspection


X-ray (if not a CMOS op amp)


Fine leak if hermetic package


NON-BENIGN


Electrical test (curve tracing) to confirm the


reported failure mode


PIND


External SEM


Temperature cycling


Hermeticity if electrical values indicate moisture


Bake if electrical values indicate moisture


POSSIBLY DESTRUCTIVE


RGA


Delid or remove plastic


Internal visual inspection    SEM inspection


Liquid crystal or EMMI


Probe/isolation


Glass strip


DESTRUCTIVE (only after the damage site has  been located)


Oxide strip


Metal strip


Decorate


Cross section (last step)


PROBLEMS WITH THE NORMAL


SEQUENCE


The first problem will be to confirm the electrical


failure mode. The typical method of matching the  input pin characteristics between the failed unit and  a known good unit will not work because the


electrical damage site is internal from the bond


pads.  Usually a functional logic level test would be  required to confirm a failure.


The second problem with this normal sequence is


after the package is opened or the die exposed.  The  damage site can not be located.  For this type of


failure there will not be any visual abnormalities,


and in most cases an internal SEM inspection is not  effective.  In addition, this level of ESD-like


damage will not be detected by normal hot spot


methods such as a liquid crystal test.  The typical


liquid crystal detection requires a level of heating of  20 mW.  As shown in figure 3, a good range for


liquid crystal use is when the damage site has a


resistance between 10 and 50,000 ohms.  For these  cases of internal ESD the damage will be typically  in the range of 50K to 100K ohms.


NEW ANALYTIC STEPS REQUIRED


In addition to the normal requirements for a failure  analysis the following data or items will be


necessary for this type of failure.


Figure 3


1. One or more good devices for comparison


purposes.


2. A data sheet of the device.


3. A complete schematic of the die.  In many cases


this is not available and will have to be


developed by the failure analysis personnel.


4. Equipment for functional testing


5. SEM chamber equipped for circuit operation


(switching) and voltage contrast


6. SEM chamber equipped with thermal hot chuck. After the normal sequence and the inspection die


surface the key new step is the addition of voltage  contrast testing in the SEM.  The failed die, a


CD4040 ripple counter is shown below.  There are  no visible defects. It is assumed that liquid crystal  or other hot spot detection will not work.  The


following steps are based on the analysis of this die, which was failing at high temperature.


Figure 4


VOLTAGE CONTRAST


The CD4020 die was electrically tested by


connecting a 12 DC power supply to the device and  using a function generator to simulate the clock


input.  The output was monitored using an


oscilloscope.  Testing at room temperature


confirmed that the device was functional and that  the output would change state at approximately 3.5  minutes with a clock pulse of 40 Hz.  The device


was then heated while monitoring the output and it  was noted that the output ceased to change state


when the temperature of the hybrid reach ~68


degrees.  The heat source was removed and the


device began to function normally as the


temperature dropped to ~63 degrees.  This was


repeated successfully several times.


The test setup was then transferred to the SEM and  the die was observed using voltage contrast.  While  monitoring the device it was possible to watch the  stages of the ripple counter advance as it was


running.  The temperature was increased to the


point where the failure occurred.  It was noted that  pin 1 stopped functioning at elevated temperature.


Figure 5


It was determined that the only electrical


connections necessary to operate the device were


the power supply lines, a clock signal and leads for  a heating stage.  The heating fixture was


constructed using a standard aluminum SEM stub, a


4.5 ohm ceramic encapsulated power resistor and


some high temperature epoxy.  A thermocouple was  also mounted between the resistor and the device.  The device was observed in voltage contrast mode  and it was possible to watch the 14 bits of the


counter as it cycled through.  The temperature was  then increased until the device failed.  Allowing the  failure to be isolated to the stage for pin 1 of the die.


Figure 6 GOOD DEVICE


Figure 7 FAILED DEVICE


DEVELOP SCHEMATIC


Along with the voltage contrast information the


next step is to develop the detailed schematic of the  components in the area of the fault.  Based on the  appearance of the logic signals shown by the


voltage contrast, the fault appears to be located in  the area outlined below.


Figure 8


As shown below a color coding technique was used  to match the layout of the N-channel and P-channel  devices to the logic schematic.   This helped to


simplify the later analysis and discussion.


Figures 9 and 10  Close up view of the failed stage with the  lines color coded for reference.


With this additional information the next set of


voltage contrast images could narrow down the  problem area.  The next basic set is shown below.


Figure 11  Voltage contrast of the device when  working properly.


Figure 12  Voltage contrast when device was failing


Note the lines corresponding to the orange and light blue  are negative when the dark blue input is negative.  On the  failed unit the orange and light blue lines are negative


when the red input is negative.


Figure 13


These images and others allowed the failure to be  traced to the “orange” metallization to the CMOS  pair.  The voltage contrast image as shown below is  of the device after removing the glass.  Note that in  the failed stage (right) the gate is at the same


potential as the ground contact.  The good stage on  the left the gate and ground contact are at opposite  polarities.  This is the orange gate from the colored  image.


The device was then tested using a probe station


and a Tektronix 576 curve tracer.  The gate of the  failed stage and two good stages were tested in


reference to ground.  It was noted that the gate on  the failed device was electrically degraded and that  the leakage current was very sensitive to


temperature (increased as the temperature


increased).


Figure 14  FAILED GATE


Figure 15 GOOD GATE


Figures 16 and 17


Note that the failure site was located by voltage


contrast methods and was confirmed by curve


tracing.   At this point of the analysis with the site  located, the remaining steps can follow the more


typical sequence of confirming the damage. This


would include metal removal and SEM inspection.  The metallization was removed using hot


hydrochloric acid.  SEM inspection of the device


revealed a small damage site in the gate oxide of the  N-channel transistor


SUMMARY


After stripping the gate metal a very small defect


site was found in the gate oxide of the N-channel


device. The damage area is approximately 600 nm


in one dimension.  This small damage area is


consistent with the high resistance leakage, assumed   for the failure.


The failure of the CD4020 CMOS ripple counter  was due to an ESD like damage site in the Nchannel gate of a CMOS pair.  It is estimated that  the resistance of this damage site is in the range of  100K ohms.


The failure is a damage site in the gate oxide with  an estimated resistance in the range of 100K ohms.  Under room temperature operating conditions the  circuit would functional normally. However as tests  on the failed cell indicated, the leakage would


increase significantly with temperature.


The probable cause was an ESD–like transient on  the N-channel drain (ground potential of the circuit) which was transferred through the oxide to the gate  metal run.  Note that for power line transients, the  damaged gate does not have to be near an input pin. At room temperature this leakage would be


sufficient enough to slightly lower the input “1”


logic level to the gate, but not enough to prevent a  switching action. However at a higher temperature  the leakage would increase and be sufficient to


lower the logic level below the switching threshold  voltage.  This action would create a “thermostat”


type of action where the failure would occur at a


fixed temperature range.  This voltage threshold


action was confirmed when it was shown that the


device would operate at higher temperature if the


operating voltage and logic level was also


increased.


SUMMARY OF THIS MODIFIED FAILURE  ANALYSIS SEQUENCE


This material has been presented to show some


possible approaches to apply to device failures,


which do not follow the typical pattern.   The


special conditions are usually:


1. The device has functionally failed.


2. Curve tracing of the external pins show no


abnormalities


3. Optical and/or SEM inspection of the die will


not show any damage sites.


4. Liquid crystal or other thermal techniques will


not usually be effective.


The mechanism will usually be an ESD-like


damage site internal on the die with an equivalent


resistance in the range of 50K to 100K ohms.  Thus  most normal analytic steps will not detect the


problem.


Assuming no visible defects after the inspection of  the die the next effective step is to perform an


operating (logic levels and clock signals) voltage


contrast on the die. There must be a way to compare  the failed images to a good set of images.  This may  be on a good device or on a good section of a gate  or cell.


At this stage the voltage contrast image must be


matched to a photo of the die area and a detailed


schematic must be obtained to correlate a possible  damage site to the failed circuit function.


If a damage site can be located then the analytic


steps can go back to a normal flow of probing and  curve trace evaluation, and then stripping and SEM  inspection of the damage site


Note that this type of analysis will detect failures


which many engineers do no consider possible.


These damage sites will typically be on one of the  gates of a CMOS pair at any location on the die. The gates can be damaged because of an ESD – like transient on either the Vdd or ground power  lines.  This is because most CMOS inverter pairs  are connected directly to both the Vdd and ground  lines at any location on the die. The exact location  of the gate damage will be random and will depend  on variations in the gate oxide and the logic levels  of the previous drive circuits.


# Design Rule of Microchip Al Bond Pad and Optimization of Bonding Process in Wafer Fabrication


Design Rule of Microchip Al Bond Pad and Optimization of Bonding   Process in Wafer Fabrication


Hua Younan, Nistala Ramesh Rao, Ang Ghim Boon and Chen Shuting


Material Failure Analysis, QRA Dept


GLOBALFOUNDRIES Singapore Pte Ltd


60 Woodlands Industrial Park D, Street 2, Singapore 738406   Tel: +(65) 6360-3458, E-mail: huayounan@globalfoundries.com


Wire bonding continues to remain as the dominant chip  interconnect technology in the far backend process, regardless  of the shrinkage of microchip Al bond pad size and the  increase in the number of I/O connections in the modern ICs. The reliability of IC devices is directly affected by the quality  of adhesion between wire bond and microchip Al pad. Many  factors, such as the wafer fab process residue and corrosion, creep-induced wire breakage and electrostatic damage, may  result in poor adhesion. In this paper, we show a p-channel  Field-Effect Transistor (pFET) failure caused by a mismatch  in the bond pad size and the wire bond diameter as well as  electrostatic damage during wire bonding. The failure analysis  results, failure mechanism and the design rule of microchip Al  bond pad in wafer fabrication are discussed.


FA investigations were performed on the high gate leakage (nA to mA level) issue in the packaged pFET. It was found  that two major factors contributed to the failure, namely  mechanical and electrostatic damage. The mechanical damage  was mainly due to incompatible Al pad size and bond wire  diameter. More specifically, in the failed device, the bond  wire diameter was larger than half size of the bond pad  opening, contrary to the general design rules of wire bonding. The failure to adhere to the design rule resulted in the device  failure. In addition, the electrostatic damage during wire  bonding resulted in defects of poly Si/gate oxide and thus the  high gate leakage. In this paper, the FA results, failure  mechanism of the high gate leakage and the bond pad design  rule will be discussed. Also, it will be demonstrated that to  achieve good bonding quality and eliminate mechanical and  ESD damage the diameter of the bond wire should be equal to  or smaller than half of the bond pad opening.


With the developments in microelectronic manufacturing  technologies, the size of device and features keep shrinking  while the operability and manufacturability is either  maintained or improved. Shrinking chip size and increasing  I/O counts has resulted in finer bond pad pitch and smaller  bond pad size for circuitry layout, presenting great challenges  for the wire bonding process. The reliability of the IC devices  is largely influenced by the quality of wire bonding and many


factors, such as process residue, contamination, corrosion [1,2,3,4], creep-induced wire breakage [5] and electrostatic  damage [6], may cause their failure.


The bond pad architecture and design have developed rapidly  with the shrinking of IC devices. The bond pad pitch has  decreased from 45 μm to 35 μm or even 30 μm [7]. While the  bond pad opening in mature technologies used to be 100 μm, in advanced nodes it has shrunk to 50 μm or even 40 μm. The  layout of bond pads changed from in-line to dual- or triple  staggered rows to facilitate the increase in number of bond  pads in IC devices. The compatibility of bond pad design and  wire bonding process plays an important role in the reliability  of the IC devices [7].


In this study, the failure mechanism of high gate leakage  pFET devices is analyzed based on the study of the symptoms  from the device defects. The devices were assembled by the  Au wedge wire bonding and showed high gate leakage (nA~mA) during electrical testing. Physical and electrical  failure analysis results revealed defects in bond pad, metal  lines and poly Si/gate oxide location. It was concluded that  inappropriate bond pad/bond wire size as well as electrostatic  damage during wire bonding are the root causes of the device  failure. Based on the failure analysis results, the compatibility  of bond pad design and wire bonding process is discussed.


Failure Analysis Results and Discussion


Electrical testing was conducted on the failed pFET devices  and abnormally high gate leakage current was observed. Figure 1 shows the I-V curve of a failed sample, which  exhibited leakage current of 40 nA at voltage of 1 V. The  leakage current of some other failed devices was as high as  several mA at the similar testing condition.


Mechanical damage


Failure analysis was first conducted on the failed sample by  performing chemical deprocessing using aqua regia solutions  to remove the bonding wire and Al metal on the bond pads. Inspection on the deprocessed sample by optical microscope  showed peeling at the edge of bond pad and the imprint of  bond wire extended beyond the bond pad (Fig. 2(a)), which is  most likely due to inappropriate wire bonding process.


Figure 1. I-V curve of a failed pFET device


To further investigate the mechanical damage, focused ion  beam (FIB) milling was used to prepare a cross section of the  layer stacks beneath the imprint of the bond wire (location  indicated by the dotted line in Fig. 2(a)). Scanning electron  microscope (SEM) inspection on the cross-section showed  that there was also damage on the metal lines and interlayer  dielectrics in the failed sample (Fig. 2(b)). It is highly possible  that the mechanical damage is responsible to the high leakage  current of the failed sample (see “failure mechanism” section  for details).


Figure 2. Images of the bondpad area of the failed samples:;


(a) optical image of a bond pad after the wire/Al removal by  aqua regia solution. The arrow shows the peeling of bond pad  edge. The dotted line shows the location of FIB cut; (b) SEM  image of the layered structure under a pad after FIB cut.


Electrostatic Damage


Besides the bond pad analysis of the failed samples, we  conducted layer-by-layer failure analysis to further study the  root cause of the leakage current. It is revealed that, in  addition to the mechanical damage, electrostatic damage (ESD) during wire bonding is also one of the possible causes  for the high leakage.


ESD induced burnt metallization and dielectric rupture are  common failures in microelectronic circuits [6]. Among the  various factors, the wire bonding process was reported as one  of the crucial manufacturing step associated to ESD induced  failure [8]. The high current resulting from ESD events may  induce damage on metal lines and dielectrics. More  specifically, the high electric field caused by ESD may be  greater than the dielectric strength of the dielectric materials (e.g. gate oxide) resulting in their  rupture. When the gate


oxide rupture occurs, a conducting path is established that  resulted in leakage current.


Analysis of the device design of the failed sample showed that  there was no ESD protection circuit, which made the sample  highly vulnerable to any electrical overstress caused by the  electrostatic charge accumulation. The failed sample was  deprocessed to the poly Si layer followed by performing  current imaging using atomic force probe microscopy (AFP), on the area beneath the failed bond pad. The AFP is capable  of localizing defects with pico-amp current range and  characterizing failure with nano-meter scale lateral resolution. During the scanning, the current flow between a biased AFP  tip and ground return via the sample was monitored and  consequently a surface map based on current contrast can be  obtained. As shown in Fig. 3, in the failed sample, abnormally  bright contrast poly contacts were observed on several areas  suggested of leaky poly Si on the failed sample due to  presence of leakage path between the poly to the substrate.


Figure 3. Current contrast AFP image of the failed sample


after deprocessed to poly Si. The arrows show the location of  good and leaky poly Si.


To study the cause of the leaky poly Si, a cross-section of the  leaky poly Si site of the failed sample was observed under  TEM. As indicated in Fig. 4(a), it is evident that the gate  oxide at the shallow trench isolation (STI) corner was  damaged. On another failed sample, SEM observation showed  physical damage on the poly Si/gate oxide location. The  observed damage is the typical symptom of defects caused by  ESD induced electrical overstress.


Figure 4. Physical damage of the failed samples caused by


ESD: (a) gate oxide damage at STI corner; (b) damage on the  poly Si


Based on the failure analysis results discussed above, we  found that two possible causes contributing to the high gate  leakage current: (i) mechanical damage due to the wire  bonding process and (ii) damage due to ESD, as schematically  shown in Fig. 5.


Firstly, the wire bonding process caused damage to the  passivation layer and metal lines near the bond pads. As a  result, the bonded wires connected the bond pad with adjacent  bond pads or metal lines which otherwise should be isolated, causing high leakage current. Our electrical testing results  showed that the leakage current of highly leaky samples  dropped significantly from mA to nA level after the bond  wires were removed from the bond pads, strongly supporting  that the mechanical damage by the wire bonding contributed  significantly to the high leakage current.


Secondly, the leakage current of the failed sample might be  also caused by the contribution of the ESD damage, which is  lower in magnitude than that caused by the wire bonding. We  used focused ion beam milling to edit the circuit on the failed  sample and isolated the transistors with the leaky poly Si/gate. It was found that the leakage current of edited device dropped  substantially from nA to pA level (refer to Fig. 6), which  confirms the contribution of the leaky poly Si/gate to the  leakage current of the failed sample.


Figure 5. Leakage mechanism of the failed sample


Figure 6. I-V curve of a failed device after the transistors with  ESD were disconnected by FIB circuit editing.


Discussion of Design Rule for Al Bond Pad


After investigation of the bonding conditions of the failed  samples, we found that inappropriate ratio of the size of bond  pad opening/bond wires might be the cause of the damage.


With the shrinking of the size and pitch of bond pads, the  quality of wire bonding process becomes more and more  critical for the reliability of the microelectronic devices. Many  factors of the bonding process, such as wire parameters, pressure, heat and ultrasonic energy, have significant effect on  the resulting bonding quality. In Tables 1 and 2 data from two  assembly houses are listed that show the relationship of bond  pad opening and bond wire diameter. It is evident that the wire  diameter is proportional to the size of the bond pad opening. According to the above industrial benchmark, one can see that  the relationship of the size of bond pad opening and bond wire  diameter is:


Bond wire diameter ≤ ½ of bondpad opening    (1)


Therefore, we should consider the above relationship as a  design rule in the design of new device. Otherwise, incompatibility of the designing in microelectronic devices  and processing may cause device failure.


Table 1: The relationship of the size of bond pad opening and  bond wire diameter (from the assembly house A)


Bond pad parameter


Size (width or diameter)


Bond pad opening (μm)


58 55 50 45 40


Bond wire diameter (μm)


25 25 25 23 20


Table 2: The relationship of the size of bond pad opening and  bond wire diameter (from the assembly house B)


59 54 49 44 39


Optimization of Bonding Parameters


In this study, the size of bond pad opening is 40 × 40 µm. To  achieve good bonding quality, the bond wire diameter should  be equal to or less than 20 µm according to the general  industrial design rule discussed above. However, in the failed  sample, the diameter of the bond wire used was 1 mil (25 µm), which is larger than 20 µm and violated the design rule of  bondpad. Consequently, the sample surface was very likely to  be damaged by the wedge bonding process due to the  inappropriate bond pad/bond wire size.


Figure 7. Optical image of the sample in our in-house testing  after removal of wire and Al by aqua regia: (a) wire diameter: 1 mil, bond pad opening: 40×40 µm (the same as the failed


sample), (b) wire diameter: 0.7 mil, bond pad opening: 40×40 µm .


To confirm that the mechanical damage observed above in the  failed samples was caused by inappropriate size of bond wires  and bond pads, we have performed an in-house testing to  compare the effect of wire diameter and bond pad size on the  bonding induced damage of samples. First, we chose the bond  wire and pads which were of the same size as the failed  sample and bonded the samples. As presented in Fig. 7(a), mechanical damage on the passivation layer beneath the bond  pads was observed after the wire removal, which is similar to  the result of the failed sample (Fig. 2(a)). The bonded sample  failed during the electrical test.


At the second testing, we reduced the diameter of the bond  wires to 0.7 mil (17.5 μm) and kept the same size of bond  pads. After the wire and Al removal by aqua regia solution, no  damage was observed on the passivation layer beneath the  bond pads (Fig. 7(b)). The bonded sample passed the electric  testing with very low leakage current (pA level), which is  similar with Fig. 6. The in-house testing results are  summarized in Table 3.


Table 3: Comparison of in-house testing with different


bonding parameters


Bond Pad  Opening


Bond Wire  Diameter


Mechanical


Damage on Bond  Pads


Electrical  Test Result


40×40 μm


1.0 mil  (25 μm)


Fail


0.7 mil  (17.5 μm)


The above in-house testing results support our conjecture that  inappropriate size of bond wires and pads caused the  mechanical damage observed in the failed sample, which  could be avoided by adjusting the size of wire and pad to a  reasonable ratio. The failure analysis results of this study  showed the importance of the compatibility of the wire  bonding process and bond pad design on the reliability of the  microelectronic devices.


Detailed FA was performed on high gate leakage current (nA  to mA level) issue in packaged pFET to investigate the root  cause. It was found that there were two dominating factors  contributed to the failure: mechanical damage and electrostatic  damage. Mechanical damage was observed on passivation  layer and metal lines. Electrostatic induced damage was found  in the STI and poly Si/gate oxide locations. The failure  mechanism of the high leakage current is discussed based on  the observed damage.


The damage in the failed sample was mainly due to the  incompatibility in the designing of bond pad opening and  bond wire diameter. Based on the failure analysis results and  the industrial benchmark on the relationship of the size of  bond pad opening and bond wire diameter, a bondpad design  rule is introduced, which is that the diameter of the bond wire  should be equals to or smaller than half of the bond pad  opening.


The authors would like to thank GLOBALFOUNDRIES  Failure Analysis Labs personnel for their contributions to this  paper.


[1] Hua, Younan, et al., “A study on Non-Stick Aluminum


Bondpads due to Fluorine Contamination using SEM,


EDX, TEM, IC, Auger, XPS & TOF-SIMS,” Proc 28th


Int’l Symp for Testing and Failure Analysis, Phoenix,


Arizona, November 2002, pp. 494-504.


[2] Hua, Younan, et al., “A Study on Fluorine-Induced


Corrosion on Microchip Aluminum Bondpads,” Proc 29th


Int’l Symp for Testing and Failure Analysis, Santa Clara,


CA, November 2003, pp. 249-255.


[3] Hua, Younan, et al., “Studies on Fluorine-Induced


Corrosion and Defects on Microchip Al Bondpads and


Elimination Solutions,” Proc 34th Int’l Symp for Testing


and Failure Analysis, Portland, Oregon, November 2008,


pp. 285-290.


[4] Hua, Younan, et al., “Studies on a Qualification Method


(OSAT) of Microchip Al Bondpads in Wafer Fabrication,”


Proc 35th Int’l Symp for Testing and Failure Analysis, San


Jose, California, November 2009, pp. 289-292.


[5] Honeycutt, J. O., et al, “Solution of Wire Creep Rupture


Problem in a Thick-film Power Hybrid, ” IEEE


transactions on components, hybrids, and manufacturing


technology, vol. CHMT-9, No. 2, (1986) pp. 172-180.


[6] Duvvury, C., et al., “ESD: a pervasive reliability concern


for IC technologies,” Proc of the IEEE, vol. 81, No. 5,


(1993) pp. 690-702.


[7] Tok, C. W., et al, “Ultra-Fine-Wire Applications and


Challenges in 30 μm process”, Proc 11th IEEE Electronics


Packaging Technology Conference, Singapore, December


2009, pp. 479-485.


[8] Tan, S. H., “Wire bond causes electrical overstress [BGA


package example],” Proc of the 5th Electronics Packaging


Technology Conference (EPTC 2003), Singapore


December 2003, pp. 366-368.


# Backside Infrared Imaging using Improved Refraction-Assisted Illumination Methods


Backside Infrared Imaging using Improved Refraction-Assisted Illumination  Methods


Terence Yeoh, Stephen LaLumondiere, Neil Ives, Martin Leung


The Aerospace Corporation, El Segundo, California, USA


Infrared backside imaging using refraction assisted  illumination (RAIL) allows for imaging microelectronic  devices at high contrast and resolution through 700 microns of  silicon without the need for specialized optics or coatings. However, due to the angle of illumination, not all of the metal  features are equally illuminated. In this paper we present  improvements on this method through image composition of a  series of RAIL images taken at various illumination directions. The resultant composited image provides more uniform  illumination and better approximates the features seen in  scanning laser confocal microscopy.


Typical silicon backside imaging techniques either employ  bright field infrared (IR) illumination, in which the incident  illumination is normal to the surface or a normal-incidence  laser confocal IR microscope raster-scanned over the region of  interest. These two techniques are limited by surface scattering  at the air-silicon interface which reduces overall contrast and  resolution of the resulting image. There are several approaches  to increase image resolution and contrast such as the use of  anti-reflective coatings [1], solid immersion lenses [2], and  numerical aperture increasing lenses [3,4]. These approaches  require either minimizing the surface scattering of the incident  light into the objective lens, or attempting to diffuse the  scattered light by means of a small depth of focus.


Recently, a new method of backside imaging was discovered  in which the infrared illumination source is placed  approximately 45 degrees with respect to the surface normal at  a point directly beneath a collection objective of a microscope  system [5,6]. Briefly, for a material with a large index of  refraction, as is the case with silicon (n=3.5 @ 1.1 µm), the  transmitted light is refracted inside the silicon at an angle of  approximately 12 degrees with respect to the surface normal as  shown in Fig 1.


This refracted light can eventually be scattered back towards  the top surface if it strikes a highly effective scattering site  such as a metal line. Any light that is returned slightly off  normal will be either refracted away at an angle which does  not fall within the acceptance cone of the objective, or  experience total internal reflection within the structure.


Figure 1: Incident light is reflected in a range of angles  modeled as a cone as a result of surface roughness. The  reflected light is not collected by the objective lens. Some  component will also be transmitted and refracted over a range  of angles, and will strike the underlying metallization.


Although oblique illumination itself is not new, the presence of  a relatively flat, high index of refraction substrate through  which the oblique illumination occurs makes this technique  particularly effective for backside imaging of semiconductor  devices, resulting in a high-contrast, high-resolution image  through 700 microns of substrate. The high index of refraction  substrate assists oblique illumination by refracting the incident  light to an angle closer to a bright field condition. The  presence of the high index of refraction substrate enhances the  contrast of the image by combining the advantages of oblique  illumination; that is, minimized surface scattering of the  illuminating light into the objective lens, with the advantages  of bright field illumination; a nearly perpendicular illumination  condition ensuring that a high degree of scattered light from  the subsurface feature can be collected by the imaging lens. In  this paper, we present results improving on RAIL by  illuminating the sample from multiple directions. The resultant  image provides more uniform illumination and better  approximates the features seen in scanning laser confocal  microscopy. Due to the “Manhattan style layout” of modern  semiconductor integrated circuits, a uniform lighting condition  can be realized with as little as two light sources.


The RAIL microscope is a custom system with a Goodrich  SU320 InGaAs sensor (25 µm pixel pitch), a 1X relay optic  and a Mitutoyo NIR 50X long working distance objective as  shown in Fig 2(a). The NIR objective has a numerical aperture  of 0.42, which translates to a resultant collection half-angle of


24.8 degrees. The field of view (FOV) of the camera in this  configuration is approximately 300 µm X 200 µm. The  spectral output of the lamp is broad and extends beyond the  spectral response of the InGaAs array. Consequently, all light  between 900 and 1700 nm is detected by the array as no  attempt was made to spectrally filter the incident illumination. We calculate the current lateral spatial resolution of this  experimental setup to be on the order of 1.7 microns, currently  limited by the large pixel size of the detector, followed by the  numerical aperture of the objective lens. The ultimate  resolution of this particular setup, as with any other IR  microscope, will be determined by the diffraction limit of  the infrared light transmitted through the substrate.


The devices imaged here are commercially available 65 nm  field programmable gate arrays. These devices were prepared  for imaging in the following manner: The protective metal cap  was removed and a swab of acetone was applied to the surface  to remove the thermal paste. No polishing or AR coatings were  applied to the surfaces before imaging. This device is a flipchip, and so removal of the thermal paste exposes the backside  silicon. The silicon substrates of these devices, as packaged, were approximately 700 microns thick. It was through this full  thickness that the RAIL technique imaged the underlying metal  interconnects defining the IC device connectivity. In this  experiment, the direction of illumination was varied from -90  to 0 degrees as shown in fig 2(b) and the resulting images  acquired.


Figure 2: Diagram of optics setup for RAIL imaging. (a) The  simple RAIL setup consists of an IR camera, transfer and  objective lenses and side-mounted angle-adjustable fiber-optic  delivered white-light source. (b) Variation in side azimuthal  angle allows a combination of lighting directions to provide  contrast enhancement for structural edge features of different  orientation on the sample.


Results and Discussion:


Figure 3 is a comparison between RAIL (a) and laser scanning  confocal microscopy imaged through 700 microns of silicon. The contrast and resolution are quite good as compared to  brightfield imaging [5,6]. Note that a comparison between the  images shows quite different contrasts at any one feature. Some areas are inverted, while others show points in place of  rectangles. These differences are attributed to the orientation  of the 12 degree incident angle illumination from a single  direction, which tends to emphasize one particular scattering  line edge over another. We found that the lines perpendicular  to the incident direction of light were emphasized, and were  able to illuminate different metal features by changing the  angle of the illumination. The greatest overall contrast occurs  when the direction of the light is perpendicular to the metal  lines in question. Structures in manufactured semiconductors  are arranged in a grid-like style akin to the layout of  skyscrapers in central Manhattan in New York.


Figure 3: Comparison of (a) RAIL imaging with single  illumination orientation angle and (b) laser scanning confocal  microscopy of the same region of a 65 nm FPGA structure. These images were taken from the backside of an as-received  chip and are imaged through approximately 700 microns of  silicon.


Figure 4 shows an image of another region of the FPGA  highlighting this effect.  When illuminated from one azimuthal  direction (a), a certain set of features is imaged.  When  illuminated from another single direction (b), a different set of  features is imaged.  When illuminated from both directions, the entire structure is imaged. The images show an  enhancement of specific lines at one direction over another. By  illuminating from both directions simultaneously, a more  uniform imaging condition is achieved. This condition more  closely approximates the images acquired using the laser  scanning microscope.


Figure 4: RAIL image of a FPGA structure made at the 65 nm  process node from (a) -90 deg  and (b) 0 deg. (c) The image  with simultaneous (-90 and 0 deg) illumination.


In this paper we have presented an improved imaging method  of RAIL - a simple backside illumination method that provides  resolution rivaling more expensive and sophisticated  techniques. Given the grid-like nature of today's integrated  circuits, as little as two sources can be used to fully illuminate  the structures. The illumination source is much less expensive  than scanning systems used to achieve similar resolution and  contrast, and the technique described here can easily be  implemented with a standard microscope with IR optics. The  simplicity of the microscope will allow it to be compactly  integrated into other instruments and tools that require  backside IR imaging in confined spaces. Systems such as  focused ion beam systems and laser assisted chemical etch will  benefit from this improved contrast. This technique can also be  used to image through other high-index materials such as  GaAs and InP, and represents an improvement of imaging  capability as compared to standard RAIL microscopy.


The authors thank Brendan Foran, Steven Moss, and Brennan  Davis for their many helpful suggestions. This work was  supported under The Aerospace Corporation's Independent  Research and Development Program.


[1] Seidel, S. et al., “Failure analysis from the back side of a  die,” Proc. ISTFA, 471, (1999).


[2] Mansfield, S. M., et al., “Solid immersion microscope,” Appl. Phys. Lett, 57, 2615, (1990).


[3] Ippolito, S.B, et al., “High spatial resolution subsurface  microscopy,”Appl. Phys. Lett, 78, 4071, (2001).


[4] Ippolito, S.B, et al., M. S., “Theoretical analysis of  numerical aperture increasing lens microscopy,”J. Appl. Phys, 97, 053105, (2005).


[5] Yeoh, T.S., and LaLumondiere, S. “Infrared Backside  Imaging for Flip-Chip DPA,” Microelectronics Qualification  Reliability Workshop, Manhattan Beach, CA, (2009)


[6] La Lumondiere, and Yeoh, T.S., EDFAS magazine, in  press.


# The Novel Dopant Profile Inspection Methodology by FIB


The Novel Dopant Profile Inspection Methodology by FIB


Po Fu Chou, Li Ming Lu


United Microelectronics Corporation, Ltd.,


No. 3, Li-Hsin Rd. II, Hsinchu Science Park, Taiwan 300, R.O.C.


Email: Po_Fu_Chou@umc.com, Phone: 886-3-5782258 ext 36785, Fax: 886-3-563-6722


The controlled introduction of dopants into silicon is a  fundamental part of semiconductor device fabrication [1]. The  electrical performance of various types of devices is ultimately  determined by three-dimensional distribution of the dopants  within the silicon. However, unlike the polysilicon or metal that  are deposited on top of the silicon substrate which can easily be  inspected, the dopant regions are not easily imaged using  standard optical or electron microscopy techniques, e.g., Scanning Electron Microscopy (SEM), Transmission Electron  Microscopy (TEM). The dopants are incorporated within the  silicon lattice at very low concentrations, which makes it  difficult to detect any difference in the structure of the silicon  related to dopant concentration [2].


There are several techniques to inspect doping profiles in  semiconductors, e.g., Secondary Ion Mass Spectrometry (SIMS), Scanning Capacitance Microscopy (SCM), wet staining with  SEM Dopant Contrast (SEM DC). However, the spatial  resolution of SIMS isn’t adequate to be applied in device  structures with dense layout and good sample preparation and a  small analysis area is required for SCM inspection. Furthermore, the wet stain technique is a conventional but destructive way  and the staining process is challenging and complex for dopant  profile inspection. This method is suitable for heavy dopant  areas but stain recipes, etch time, and temperature can seriously  affect the profile result. A better approach to depict the dopant  profile is SEM DC, which is a convenient and powerful method  to inspect dopant regions.  There are many studies that describe  this technique however low concentration dopant profiles are  very difficult to inspect using SEM DC methodology [3].


A Focused Ion Beam (FIB) system is a relatively new tool that  has a high degree of analogy with a focused electron beam  system. It plays an important role in the semiconductor failure  analysis field. The basic FIB application can be divided into  electrical and physical analysis. Furthermore, dopant profile  inspection is one of the FIB physical analysis applications.  Using a focused ion beam, secondary electron imaging of nwells under oxide from the backside of a thinned sample was  accomplished. From the backside the n-wells were initially  observed at a remaining silicon thickness around 4.5 m, which correlates to the actual implant depth where n and p carrier  concentrations are equal. When the n-wells were FIB imaged, contrast appeared dark relative to the p substrate. During  deposition of the oxide film, the n-well brightness changed  from dark (relative to the p-substrate) to bright. It appears that  the interaction volume of the beam reached the silicon/oxide  interface to create tunneling electrons during this deposition


step.  This phenomenon dominated the capacitive effect.  Then  as the film thickness increased the capacitive effect prevailed. The imaging structure is analogous to a Metal-OxideSemiconductor (MOS) capacitor.  The n- and p-MOS capacitive  properties yielded a permanent imaging contrast at an optimized  oxide thickness (130 nm) [4].


In this paper, a novel technique for characterizing P-V dopant  regions in silicon by using a focused ion beam methodology is  presented.  This technique builds on previous work for backside  FIB navigation, in which n-well contrast is observed [5].  The  present work demonstrates that the technique can distinguish  both n and p type dopant regions.  Finally, the capability for  imaging real sample dopant regions on current fabricated  devices is also demonstrated. This method provides a  complementary solution to the chemical or other material  analysis methods (e.g., SEM DC/SIMS/SCM) currently  available.


METHOD


1. Remove all layers above the substrate:


The silicon device was chemically stripped of metal and  dielectric layers above the silicon substrate.


2. Dopant contrast enhancement:


In order to enhance the dopant contrast phenomenon, a silicon  stain process is employed to enhance the contrast. In this  process the sample is stained by a chemical solution (HF/HNO3/CH3COOH) to enhance the dopant contrast.


The dopant contrast enhancement step is critical for increasing  the image contrast and analysis success rate.  As shown in Fig. 1a, if the sample is not suitably stained by a chemical solution  the image is fuzzy and it is difficult to recognize the well  boundary.  However, as the sample is stained, the image  contrast is clear and clearly shows the dopant profile (Fig. 1b). In Fig. 1b, the bright region is n-well.


Figure 1: Dopant contrast images with/without stain procedure


(a) The sample is not stained. (b) The sample is stained.


3. FIB Inspection:


After the dopant contrast enhancement procedure, the dopant  profile can be inspected by a FIB system.   Dual beam FIB, single beam FIB, and circuit edit FIB equipment are all suitable  for DC inspection.  In this procedure an ion beam will be used  to inspect the dopant profile at 30 KV and the detailed results  will be disclosed.


CASE STUDY


Dopant contrast analysis is commonly performed using SEM  DC methodology, however the deep N/P well or well of High  Voltage product are very difficult to observe with SEM DC. In  order to get better dopant profiles, FIB DC methodology will be  employed in these real cases.


Take the Al process product for example; the N-Well boundary  accuracy and dimension should be checked in a failure analysis.  This product layout is shown in Fig. 2.  The green area is the Nwell region.  The SEM DC image (Fig. 3a) is a little fuzzy and  it is difficult to identify the N-well dimension.  In order to get


better image quality, the FIB dopant profile inspection  methodology is employed.  As Fig. 3a shows, the N-well region  is relatively dark compared with other regions using SEM  inspection.  Conversely, the N-well region shows up bright  using FIB inspection. The N-well boundary and dimension  analysis is easier when identified by FIB methodology rather  than SEM and compared with the product layout, the N-well  profile is correct by FIB inspection.


Figure 2: Product layout; the green region is N-well.


Figure 3:  N-well region inspected by SEM and FIB.


(a) Dopant profile inspected by SEM (b) Dopant profile  inspected by FIB.


Deep N-well identification is usually unavailable using SEM  analysis and needs be identified by SCM.  FIB DC  methodology is however, effective for deep N-well  identification.  For example, the deep N-well profile of HV  product is shown in Fig. 4.  The N-well in deep N-well is very  clear with a dark appearance and the deep N-well is also  apparent as a bright region using FIB DC methodology.  In this  case study, it is evident that FIB DC methodology is  complementary to SEM DC methodology.


Figure 4: N-well and deep N-well regions inspected by FIB.


DISCUSSION AND CONCLUSION


In this study, plan view dopant profile analysis by FIB DC  methodology is demonstrated.  However, the dopant profile  contrast is opposite between FIB DC and SEM DC, and the  theory of both is not clear in explaining this contrary  phenomenon.  Therefore, we present a reasonable contention to  support this analysis result.


In published literature, the Induced Conductive Surface Layer (ICSL) has been described as a conductive layer induced by an  ion beam on an oxide surface.  This ICSL is created by  electron-hole pair production in the interaction volume [5].  In  the other paper [4], the author deposited a thick oxide to form a  MOS structure that changed the N-well contrast from dark to  bright in a back-side circuit edit study.  In the MOS structure  depicted in Figure 5, the top layer in the oxide is the ICSL; charges are created by ion interaction with the oxide [7].  The  oxide is the deposited oxide with no generated charges.  The  semiconductor part of the MOS capacitor is comprised of the nwells and the p-substrate.  Contrast is generated by the  differential capacitive properties between a p- and n- MOS  capacitor at a fixed gate voltage.  The incoming dose is constant  over the entire oxide surface and acts as a positive gate voltage (because the ion beam energy is positive). The band bending is  quite low or can be negligible for n-MOS compared to p-MOS


[7, 8] (Fig. 6).  The charges accumulated at the oxide – semiconductor interface are directly related to the amount of  band bending:


Q(s)=1/ Cox   (s- Vg)


Q(s): Silicon surface charge density


Cox : Oxide capacitance (constant)


s: Band bending (potential)


The n-MOS capacitor accumulates fewer charges than the  p-MOS capacitor at the oxide – semiconductor interface and on  the oxide surface. The amount of positive charge at the oxide  surface above the p-substrate is higher.  Consequently, the nwells appear brighter than the p-substrate.  Conversely, if the  incoming energy is negative, e.g, a SEM electron beam, the  result will be different in that the band bending is quite low for  p-MOS compared to n-MOS, and the amount of negative  charge at the oxide surface above the n-substrate is higher.  Consequently, the n-wells appear darker than the p-substrate.  These phenomena provide an explanation for the n-well  contrast changing mechanism.


Figure 5: (a) Cross-section of the voltage contrast structure


(b) MOS capacitor.


Figure 6: Band bending as a function of gate bias.


In the reference paper, the deposited oxide is the key that  makes the n-well become bright or dark. However, in our  investigation, the thick oxide is not formed by FIB but by the  staining procedure.  The staining procedure forms the silicon  oxide (SiO2) that makes the n-well contrast become bright as  thick oxide does.


Si+4HNO3SiO2+2H2O+4NO2.


SiO2+6HFH2SiF6+2H2O


As shown in Fig. 7, the oxide thickness before the staining  procedure is around 36 Angstroms; if the sample is stained the  oxide thickness will become thicker at 279 Angstroms. According to the reference paper, this result fits in with the  contrast mechanism described therein.


Figure 7: (a) The oxide thickness=36 Angstroms before the  staining procedure (b) The oxide thickness=279 Angstroms  after the staining procedure.


In summary, the P-V dopant profile inspected by FIB is  demonstrated.  SEM DC and FIB DC are complementary  methodologies for the inspection of dopants.  The advantage of  the SEM DC method is high resolution; the advantage of FIB  DC methodology is high contrast, especially evident in a deep  N-well region.


[1] VLSI Technology, 2nd edition, S.M.Sze, editor, McGrawHill, Inc., NY, p. 272, 1988.


[2] Robert Pajak, Frank Baiocchi and Erwan Le Roy, ISTFA  proceedings, pp. 8-13 (2005).


[3] Po Fu Chou, Chun Yen Chen. ISTFA proceedings, pp. 189-192 (2009).


[4] Erwan Le Roy and Mark Thompson. Mat. Res. Soc. Symp.


Proc. Vol. 792  (2004)


[5] E. Le Roy and M. Thompson Mat. Res. Soc. Symp. Proc. Vol. 792 (2004)


[6] E.I.Cole Jr in Micro. Failure Analysis Desk Reference, edited by EDFAS p. 133.


[7]  A. Goetzberger, Bell Syst. Tech. J. 45, 1097 (1966).


[8] Nicollian, Brews in MOS Physics and Technology, p. 80 (2003).


# Design Diagnosis with E-beam Probing to Improve Reliability Issue due to Competitive Signal Error


Design Diagnosis with E-beam Probing to Improve Reliability  Issue due to Competitive Signal Error


T.C. Chuang, C.M. Shen, L.F. Wen, S.C. Lin, C.M. Huang, Jon C.Lee


Taiwan Semiconductor Manufacture Company, Ltd., Taiwan


1,Nan-Ke N, Rd., Tainan Science Park, Tainan, Taiwan 741-44, R.O.C.


Phone: 886-6-5056688Ext.7062149   Fax: 886-6-5052007   Email: Chuangtc@tsmc.com


ABSTRACT


Tiny circuit design reliability issue related to competitive  signal was investigated in a sense amplifier (SA) circuitry of  SRAM by E-Beam probing technique in this paper. The  irregular output signals then traced back to former stage  circuit and identified associated waveforms. With such design  concept and technique tracing, the invisible and cunning  circuit mismatch reliability issue could be revealed  successfully.


In the development of new ULSI era, high circuit densities  and small linewidths make it increasingly more difficult to  probe these devices with conventional mechanical probing. Mechanical probes are potentially destructive. Electron-beam  probing is fast becoming the preferred technique for looking  at chips that are too dense or complex for mechanical probers.  E-beam probers are no longer limited to R&D labs but are  penetrating IC manufacturing centers. With the popularity of  e-beam probing comes the need for design and manufacturing  engineers to know more about it. In failure analysis point of  view, engineers usually utilize E-Beam probing to extract  critical signals on a circuit’s internal nodes. And these  waveforms could be help to verify simulations and reveal  errors in design and fabrication. Signal extracting is still very  potent in obtaining detailed information of internal circuit  performance such as AC timing, waveform shape and  reference level to judge failure root cause that other FA  technique still could find no way out [1].


Related to FA field, an unstable competitive signal may  cause intermittent marginal failures in the circuitry, which  may not be detected during chip probing and final testing.  Multiple manual probing techniques were tried unsuccessfully  to analyze the failure mode since the failure mode often  changed due to the loading pressure from the mechanical  probing. Therefore, a repeatable and noncontact technique is  needed in order to measure this type of failure mode and to  trace down the origin of the failure stage. The fact that the  unstable competitive signal was located somewhere inside a  mixed signal circuit complicated the failure analysis  significantly since the failed portion of the circuitry was  surrounded by large analog circuit area and was not accessible  directly. An e-beam prober is a powerful tool for repeatable


and nondestructive testing of internal nets in a circuitry  especially when the prober system is installed with a device  layout database and when it is connected to an ATE tester in  case a complex loop test program is needed. An e-beam  prober can automatically locate the pre-identified nets in a  device using its installed device layout database and measure  voltage waveforms (contrast) directly from the internal nets in  a device run by ATE. An ebeam prober is very useful in  obtaining detailed information of internal circuit performance  such as shape (waveform) and timing of voltage signals.


EXPERIMENT AND CASE STUDY


In this experiment, the related circuitry diagram was shown as  Fig.1, thermal related scan reliability issue (shown in Fig.2) was revealed at final test stage. Then using common FA  manner to localize and search out the accurate failure  mechanism. And the results of FA feedback had no effectively  convergence.


Figure 1. The related SRAM circuitry level frame. Whole  system include core, SA, buffer and I/O sub-circuit.


Figure 2. (a) Scan “0” showed light overshot in ref chip and


(b) stuck-at high failure was revealed in failure chip


(a) Reference chip


(b) Failure chip


CLK


Scan1


Scan0


Schlumberger IDSl0K plus e-beam prober was used in this  failure analysis to trace down the failure mechanism for an  intermittent marginal failure in the SRAM circuitry. The ebeam prober was connected to an ITS9000FX tester so that an  automatic loop test program could be used to run the failed  devices at certain failure modes repeatedly. Known good  devices were also tested to ensure proper hardware and  software setup and to obtain good waveforms as reference.


After the devices were decapped, the top passivation layer  was often removed in order to obtain stronger e-beam signals. An electron beam can be aligned and focused to a localized  area in the circuit to be measured. With diagnosis related  circuit design, E-Beam probing was suitable and could be  used in the case to trace the delinquency movement for a high  temperature worse intermittent marginal scan stuck failure in  the memory circuitry of failed chips at certain scan mode  repeatedly. First of all, both passed and failed chips were  tested to ensure faultless hardware/software setup and  reconfirmed that had the same reliability phenomenon  between testing and FA sites.


Signal extracted was performed at the failed bi-directional  I/O and their related inner sub-circuitry to ingeniously narrow  down the failure site. The I/O is functional well at fail chip  when operating in specific IO proofread mode. In order to  further narrowing down the whereabouts of scan failure occur, the output buffer critical nets were gauged, and results were  showed as Fig.3.


Figure 3. “W1R1W0R0R0” vector was applied. Buffer and  sense amplifier output of failure sample both showed stuck  fault compared with reference.


Abnormal signals in SA and buffer output stage still subsist. For protecting SA output waveform against the influence of  signal flow backward, output buffers of both pass and fail chip  were cut off using FIB and re-extracted SA output signal  under different applied Vcc bias, as shown in Fig 4.


Figure 4. Output buffers of both pass and fail chip were cut  off using FIB and re-extracted SA output signal under  different applied Vcc bias


Fail chip showed punier voltage difference (~0.7V) than  reference (~1V) when SA output signal transit state from “high” to “low”. There are many reasonable causes could lead  this abnormal issue, like tight word line pulse width, SA  circuitry design mismatch, irregular control signal or cell  device driving capacity etc [2].


To clearly differentiate this issue, some critical signals  should be checked. Circuit was overhauled and then picked  probing pad up to top surface using focused ion beam (FIB). This step is critical in order to obtain isolate, stable and noise  free signals. There are some know-how do need our concern  before pick probing pad.


The first concerned is observability ensures that the primary  beam can reach the conductor, or if it encounters an insulating  layer, that the buried conductor has a clear path to the surface. It is not suitable to place bond pads where bond wires or  probe card pins will obscure the areas of the pad we want to  probe. Another situation, if buried signals are to be probed via  capacitive coupling to the surface, then we must have a clear  line of sight from the buried conductor to the surface of the  insulating layers. Thus, overlying metal-2 lines cannot  obscure the metal-1 lines, poly lines, or diffusion areas that  we want to probe. The same applies to all overlying conductor  layers.


For improving signal-to-noise (S/N) ratio, exposed probing  pad surface conductors have to be large enough for the  primary beam to land on. A ratio of conductor width to the  size of the beam spot of at least 3: 1 ensures that 98% of the  beam lands on the conductor (assuming a Gaussian  distribution for the intensity profile of the brightness across  the spot). For buried conductors, one should maximize the  conductor width to increase the capacitive coupling effect to


W1 R1 W0 R0 R0


Ctrl


BUF_ref


SA_ref  BUF_fail  SA_fail


Failure Chip


Reference Chip


SA_1.5  SA_1.0


SA_1.2  SA_0.6


SA_0.8  SA_1.5  SA_1.2  SA_0.6


SA_0.8  SA_1.0


the surface. Related to probing pad topography, a 2-um metal  pad may look pretty flat to a 1-um beam, but not to a 0.1-um  beam, which will be affected by surface microstructures. Some e-beam probes scan lines to turn the probe spot into a  probe line. This allows the beam to average the  microstructures and not produce anomalous readings because  the landing surface is at strange angles.


Another probing issue is that waveform crosstalk occurs  when you make measurements on closely spaced pads. Possible causes such as


1. Local field effect: voltages on circuit lines near the signal


pad create electric fields. These fields modulate the number


of secondary electrons emitted from the signal pads.


2. Poor focus: electron beam samples the voltage on the


adjacent circuit lines.


3. Misplacement of e-beam prober: due to hysteresis of


magnetic lenses.


4. Probe needle signal: power supply noise, (occurs even it is


400um away).


5. Global field effect: GFE deflecting the primary e-beam, if


it is at low clock rate, it can be seen in SEM.


6. Capacitance between adjacent pads.


Some solution include reduce the secondary electron


detector by adjusting parameters of detector, make the signal  pads clearly (one will not be able to make reliable waveform  measurement if cannot see the signal pads clearly), place the  ebeam probe accurately on a clear pads, avoid placing probe  on a topographic feature of circuit line, e.g.: via, vertical step  in conductor, turn off power supply, operate with few nodes


switching in parallel or operating the circuit at a variety of


cycle times.


With carefully FIB operation base on main points mentioned  above, isolate, stable and noise free signals could be got. The  SEM image of probing pad result was shown as Fig. 5.


Figure5. In order to obtain isolate, stable and noise free  waveforms signals, circuit repaired is done using focused ion  beam (FIB) at some critical nets.


After checking the state of related control signals, they all  showed no difference with normal chip. And that is to say, the  suspected failure site could be localized at either sense  amplifier or memory cell circuitry device.


After diagnosing the chip design frame, there are 16 SAs  wire-mux per data pin. Simultaneously, there is only one SA  be enabled and output the sense signal. Other remained 15  SAs outputs keep floating, as shown in Fig 6.


Figure 6. In the meanwhile, there is only one SA be enabled  and output the sensed signal. Other remained 15 SAs outputs  keep floating.


The SA output signals of three failure samples with full, half  and only one SA was kept through circuit modified were  extracted and compared with each other, as shown in Fig. 7.


Figure 7. The SA output signals of three failure samples with  full, half and only one SA was kept through circuit repair. Only one SA remain wired sample had maximum voltage level  difference transfer from “High” to “Low”


Obviously, only one SA remained wired sample had  maximum voltage level difference transfer state from “High” to “Low” compared with other samples. The phenomenon is  very impressive because it will bring about some


SAout- 16 SAs kept  SAout- 8 SAs kept


SAout - only one SAs kept


consequences like SA output stuck at high and tighten process  window. For conscientious and careful confirming this  circumstance, both relaxed word line pulse width and rising  Vcc were applied showed relieved waveform. The root cause  should be floated PMOS of disabled SA sink large current and  then pull up the output voltage level to high. The real situation  is only one SA pull down device competed with 15 SAs pull  up devices, as shown in Fig. 8.


Figure 8. Real situation is that only one SA pull down device  competed with 15 SAs pull up devices.


New SA circuit design was implemented by designer to  overcome these kinds reliability issues related to level  competition campaign. The stuck high failure mode has been  improved since then. No similar faulty has been observed  thereafter.


According to our research, hitting the mark from design point  of view still playing an important role to revealed reliability  issue just like analog design error case. Through designing  diagnosis and E-Beam technique, one could accurately reveal  the invisible reliability root cause in electrical characterization  and tracing back to the site faulty occur according to circuit  design concepts and make forthwith designing modify to  rapidly keep ready for market.


[1] W.T.Lee, “Engineering a Device for Electron-Beam Probing,”


IEEE Design & Test of Computers, Vol. 6, No. 3, June 1989,


pp.36-49


[2] E.Plies and M.Chweizer, “Testing for Different Methods of Deconvolution for Electron Beam Measured Waveform,” Micoelectronic Engineering, Vol. 7, No. 2-4, 1987, pp. 183-193


Copyright ©  2010 ASM International® Proceedings from the 36th International Symposium for Testing and Failure Analysis                                                                              All rights reserved  November 14–18, 2010, Addison, Texas, USA


# Application to Non Destructive physical Analysis Method using X- ray CT Imaging


Application to Non Destructive physical Analysis Method   using X-ray CT Imaging


Akira Mizoguchi, Minoru Sugawara, Masahide Nakamura, Koichiro Takeuchi  MITSUBISHI ELECTRIC CORPORATION


Kamakura City Kanagawa pref. Japan


We have been paying attention to the development of  the nondestructive physical analysis (NDPA) technology. We think that NDPA is a technology  which doesn't depend on the worker's capability or  experience. There are many NDPA techniques, and  analysis using X-ray imaging is one of the principal  techniques. Due to the progress of the image analysis  using computers in recent years, X-ray imaging have  been evolving from two dimensional images to three  dimensional imaging. We have been applying X-ray  CT imaging to actual failure analysis and reliability  evaluation since 2008.


At ISTFA 2009, we reported on the effectiveness of  X-ray Computed Tomography (CT) images in the  failure analysis. [1] We confirmed that the X-ray CT  image had various applications, for example,  screening for counterfeit parts, the detection of the  defect of the multi-layers printed wiring boards (multi-layers PWB), the structure confirmation of  caulking contacts, and the detection of cracks or voids  of the solder joint.


This paper discusses the effectiveness of X-ray CT  imaging in failure analysis and discusses the  effectiveness of applying X-ray CT imaging to the  propagation of cracks occurring at solder joints  during temperature cycling test.


As downsizing in electronics progresses, parts and  materials are becoming more structurally complex. For example, the number of layers of printed circuit


boards (PWB) and the number of the pins in  connectors increase every year. We think that NDPA  technology – X-ray CT imaging, in particular – is  suitable for multi-layers PWB and the multi-pin  connectors in quality assurance or acceptance  inspection, screening, or failure analysis.


Conventional destructive physical analysis (DPA), as  described in MIL-STD-1580, is valuable in order to  evaluate or confirm the quality and the reliability of  parts and materials. However, conventional DPA has  some problems: it demands skilled, experienced  technicians, requires significant time, and is not  always reproducible. Furthermore, conventional DPA  cannot be used for in-line inspections. Therefore, we  predict that NDPA is used much more than DPA for  in-line inspections. Cross section analysis is the  representative DPA technique. On the other hand, there is X-ray image analysis as the representative of  NDPA technique. The comparison between cross  section analysis and X-ray image analysis are shown  in table 1.


We think NDPA technique to be applicable to a  quality evaluation, screening, failure analysis and a  reliability evaluation. Therefore, we make an effort in  acquiring the applicational techniques of the X-ray  CT images which are the most important device of  NDPA.


Table 1 The comparison of characteristics between   Cross-section images and X-ray CT images


Cross-section  images


X-ray CT


images


Accuracy


Very good


Reproducibility


Not so good


Processing time


Excellent


Noise of mages


Dependency of  worker’s skill


Much


Less


X-ray CT imaging can convert the structure  information of the sample into the information of  each layer. The X-ray CT device which we installed  in our factory was equipped with the diagonal CT  method that X-ray analysis could apply for a sample  having various shapes (see Fig. 2.1, XVA-160: UNI-HITE SYSTEM Co Japan [2]). The element  which is important in X-ray analysis is materials of  the samples. In addition, the wavelength of X-ray, the  acceleration voltage and the resolution of the  detectors (the number of the pixels of the CCD  camera) are also important elements of the X-ray  device.


Because we are not X-ray CT devices makers, we do  not have the detailed technical information about the  X-ray CT equipment side. We carry out examination  and an evaluation only about practical uses of the  X-ray CT device as a user of the X-ray CT device.


The parameter that is the most important in X-ray  images is contrast of the images. The contrast of  X-ray images depends on the imaging condition. The  contrast of X-ray images has the dependence on  structure and the materials of the samples. The  detectable power of X-ray analysis is proportional to  the density of the sample. Therefore, an observation  object with the condition that the contrast of the  images is big is suitable for X-ray analysis. For  example, X-ray image analysis is effective for  detecting metal in resin materials. X-ray image  analysis is also effective for detecting the defect such  as a crack in metal and the cavity. In particular X-ray  CT image analysis is very useful when we judge the  defect about solder joints.


Generally, the solder joint is widely used as the  joining technique of terminals of electronic parts. In  addition, in quality and reliability of the electronic  equipment, the solder joint is the most important part.


However, the analytical technique for the solder joint  was a thing mainly on external visual inspection and  the cross section analysis, and X-ray analysis was  placed as secondary technique.


Fig. 2.1 The configuration of the diagonal method of the  X-ray CT system [2]


Here we pick up the case to analyze a cavity or the  crack which occurred in a solder joint. The  conventional two-dimensional X-ray image becomes  incomplete for the positional information of the  defect (the information of the Z-axis direction  disappears). Because the information of the Z-axis  direction disappears in two-dimensional X-ray  analysis (see Fig. 2.2), the precision of the position of  the abnormal part on X-ray analysis photograph  deteriorates.


Therefore, we finally carry out cross section analysis  and must confirm the defect part directly.


X-ray


(Complex :PCA)


Rotation


Camera


Mounted part


Fig. 2.2 The conventional two-dimentional X-ray images


We can find the existence of the defect


On the other hand, in the X-ray CT images, the  information of the Z-axis direction does not vanish. The collation precision between a actual defect part  of the sample and the point by the X-ray CT image  improves. As the result, we strongly expect that we  can omit destruction analysis.


We needed many procedures and number of the time  and the samples in cross section analysis until  installing the X-ray CT device in our factory. In  contrast, we expect that X-ray CT images can  decrease the number of the procedures for analysis, the working hour for analysis and the number of  samples. Furthermore, we expect that the solder joint  of the same sample can trace the outbreak of an  occurring crack and a process of the growth by using  X-ray CT images.


In this paper we show some good examples using  X-ray CT images for failure analysis and we also  show the effectiveness of using X-ray CT images to  detect defects in solder joints.


At first we show the good examples of the defect  analyzed in the multi-layers PWB with X-ray CT  images. The examples of X-ray CT images are shown  in the Fig 3.1-10. In this case, without destroying  multi-layers PWB, we discovered the defect (a short  circuit part) of the inner layer of PWB. Because the  distance of the wiring layer of the PWB has more  than 100um, X-ray CT images can completely  separate in each wiring layer. This example is  completely detected as the short circuit of the bridged  metal (see Fig. 3.3 the 3rd layer). The bridged metal  occurred between via-holes. From our data, we  estimate that our X-ray CT device can detect the  defect size of bigger than 5um.


We show an analysis example about the  disconnection of the multi-pins connector (see Fig.


3.11). The conventional X-ray image (2D X-ray  image) cannot detect this disconnection part. On the  other hand, any situation of cross-section in the  sample can be confirmed by X-ray CT images  without destruction of the sample. Therefore, we can  detect a disconnection part of the multi-pins  connector using X-ray CT images.


The next good example is the poor connection of the  SMA type connector (see Fig. 3.12). In general, the  analysis of the insertion part in connectors is the most  difficult in the failure analysis. This case is an  analysis of the sample that shows abnormality of the  RF characteristic after the temperature cycling test. The Fig. 3.12 shows that the connection of the pin of  the connector that shows an abnormal electrical  property is an insufficient bonding state compared  with the connection of the pin of the connector that  shows a normal electrical property. The slight  difference of the situation between good connection  and poor connection can be detected by this X-ray CT  image.


The Z-axis


The projected images


The defect


Fig. 3.1  The 1st layer


Fig. 3.2  The 2nd layer


Fig. 3.3 The 3rd layer


Fig. 3.4 The 4th layer


Fig. 3.5 The 5th layer


Fig. 3.6 The 6th layer


Fig. 3.7 The 7th layer


Fig. 3.8 The 8th layer


Fig. 3.9 The 9th layer


Fig. 3.10 The 10th layer


Fig. 3.1 3.10 The X-ray CT images for the multi-layers PWB


<The conventional 2D X-ray image>


<The X-ray image>


Fig. 3.11 The disconnection of the multi-pins connector


<Good connection>      <Poor connection >


Fig. 3.12 The situation of connections in SMA type connectors


We show the amount of solder of the through holes (TH) on the PWB using X-ray CT images (see Fig.


3.13). This is also the one of good analysis to solder  joints without destructing samples. The amount of  solder in the through holes (TH) on the PWB has  been evaluated using the cross-section analysis. The  result of the cross section analysis to the same sample  applying X-ray CT analysis is shown (see Fig 3.13). X-ray CT image and the section observation result are  corresponding well.


Needless to say the DPA technique can't be  applicable to any products. The external visual  inspection can't cover the amount of the solder in this  part (TH). Using X-ray CT images can precisely  confirm the amount of the solder in the through holes (TH) on the PWB without destructing them.


Defect


<The X-ray CT image>  <The cross-section analysis>


Fig. 3.13 The comparison of the methods between the X-ray CT  image and the Cross-sectional analysis for the same the through  holes


About the crack in the solder joint of the QFN type  package, we show the evaluation example using  X-ray CT images (see Fig. 3.14-3.17. The red arrows  show cracks in the solder joints). These X-ray CT  photographs show a defect to grow up in the solder  joint. Only by nondestructive analysis, we can track a  process of the growth of this crack precisely.


We think that it is necessary to observe the same part  in nondestructive analysis to evaluate a process of the  growing crack. Furthermore, the crack occurring in a  solder joint has the expanse of 3-dimensional. X-ray  CT images are suitable to evaluate this expanse  precisely.


Fig. 3.14 Initial


Fig. 3.15 After the 250th  cycles


Fig. 3.16 After the 500th  cycles


Fig. 3.17 After the 750th  cycles


Fig 3.14 17 The X-ray CT images of the same solder joints


We can find defects of the assembly levels such as  connectors, PWB and solder joints using X-ray CT  images. We think that detecting defects of solder  joints without destructing the samples is a very  important thing. The conventional method for  confirmation of solder joints was the cross-section  analysis of DPA.


We expect that the inspection of the solder joints  using X-ray CT images can bring the improvement of  the quality confirmation level of the solder joints. Especially, X-ray CT analysis can achieve the  soldering inspection for parts which have solder joints  in bottoms of parts like BGA packages or QFN  packages. Therefore, we predict that the inspection or  the failure analysis of solder joints will demand the  application of X-ray CT technique in future.


We think that we can evaluate a process of the growth  of the cracks in the solder joints by X-ray CT images  precisely. We require observing the same part to  evaluate the growth of the cracks of the solder joints  without destructing the samples. X-ray CT analysis is  suitable for the evaluation of the growth of the crack  in the solder joints. And the cracks occurring in  solder joints have some expansions which are three  dimensional. X-ray CT analysis is also suitable for  precisely evaluating of these expanses.


The conventional test method of solder joints for  reliability confirmation exposes the samples to the  temperature cycling test. We carry out the cross  section analysis of the solder joints at the number for  scheduled cycles. We carry out the cross section  analysis of the solder joints at the number for  scheduled cycles. The length of the cracks which are  observed by cross section analysis in the solder joints  is measured. We evaluate reliability level of the  solder joints as the length of the cracks. We have  been carrying out this conventional method for a long  time. This conventional evaluation technique is the  one of DPA and it needs many samples.


We have been considering replacing this conventional  technique with technique using X-ray CT images. There are some problems when X-ray CT images are  applied to this analysis. The most important problems  are resolution of X-ray CT images. We estimate that  minimum resolution of X-ray CT images is 5um from  the data which we have accumulated. Similarly, the  dispersion about the Z-axis direction becomes a  problem too. About the dispersion of this Z-axis  direction, we also estimate the size of the 5um at the  maximum from our data of the images. These limit  values cannot deny that they become the factor of the  oversight of the cracks.


But, in our experience, these cracks less than 5um  haven't become the problem of the reliability at the  early stage of the temperature cycling test yet. Furthermore, from the conventional cross section  analysis, we have confirmed that the lengths of the  solder cracks which grow up by temperature cycling  are longer than 5um. Therefore, we predict that what  cracks less than 5um cannot detect does not directly  influence an evaluation in the reliability greatly. We  plan some evaluation examinations now to verify this  prediction.


We conclude it is confirmed that X-ray CT images  are effective for the detection of the defect at the  assembly levels such as the connector, PWB, and  solder joints. And X-ray CT images confirmed that  they had the effectiveness in the reliability evaluation.


However, we started that we used X-ray CT images  in reliability examinations. We think that it is  necessary to build more effective data in X-ray CT  analysis.


7. Reference


[1] A. Mizoguchi and K. Takeuchi, Effectiveness of  Non Destructive Physical Analysis Method Using  X-ray CT Imaging, P247, ISTFA 2009


[2] The home page of UNI-HITE SYSTEM Co.


URL: www.unihite-system.co.jp


# Fundamental Study of Al Pad Grain Size Measurement and Its Effectiveness


Fundamental Study of Al Pad Grain Size Measurement and Its Effectiveness


Yaobin Zhao, Haibo Dai, Baolin Gao, Linfeng Wu, Sanan Liang, Chorng Niou, Qiang Guo


Semiconductor Manufacturing International (Beijing) Corp, 18 Wenchang Avenue, Economic-Technological Development  Area, Beijing, P.R.China 10017


Tel: +86-10-67855000-27609/29040, Fax: +86-10-67855256, Gary_Zhao@smics.com


Grain size monitor of Al pad is necessary to assure pad quality  and electrical performance in IC manufacturing. Currently, the  sample is prepared either without pretreatment or with 4.9% HF stain or ion milling before grain size measurement. In this  paper, we demonstrate the pretreatment has a pronounced  effect on the grain size measurement and the method with ion  milling pretreatment shows more reliable results. The  mechanism is further discussed.


Al bonding pad is a very important constituent of an IC  microchip. In wafer fabrication, Al alloy is currently used as  the metallization material of microchip Al bonding pads [1]. Al bonding pad resistance and Al pad surface state strongly  influence the microchip performance for it is used for  communication between IC microchip and outer circuit. Mayadas and Shatkes first described the impact of grain size  on electrical resistance in detail in 1970 [2]. Effectively, each  grain boundary functions is as an internal surface for electron  scattering with some probability of transmission or reflection  from the interface. Usually the grain size of metal is much  bigger than the mean free path (l0, for Al75000Å) due to  other scatters, however, in the case of thin film, the grain size  is generally smaller than l0, and here the grain boundary  contribution to metal resistivity can no longer be regarded as  negligible. The model by Kuan et al. approximates the effect  of grain boundary scattering on resistivity as:


/01+1.5[R/(1-R)]/g            (1)


Where g is the average size of the grains, and the scattering  coefficient, R, varies from 0 for no scattering (i.e., complete  electron transmission) to 1.0 for complete scattering by the  boundary (i.e., R is 0.17 for Al) [3]. So it’s very important to  monitor Al bonding pad grain size in wafer fabrication. There  are three sample preparation methods for Al bonding pads  grain size monitoring: no pretreatment, with 4.9%HF stain and  ion milling. This paper will study the influence of different  sample pretreatments to grain size data collection.


In this paper, FEI DB235 was the major tool performed for  ion milling and SEM images taken; FEI TECNAI F20 was for  TEM analysis. The samples were prepared with either  chemical stain or not, and by ion milling. Regarding the


conventional grain size estimation, the length (L) of a  catercorner line at fixed magnification on SEM image of the  Al pad surface is measured. The grains are counted along the  catercorner line. The average size of grain can be calculated by


Grain size=L/N                     (2)


where N is the number of grain.


Experiments Results


For grain size monitoring, no pretreatment or chemical stain  are preferred for sample preparation because they are easier  and more convenient to handle. Fig.1 (a)~(c) were the same Al  pad with different sample preparation methods, Fig 1(a) and


(b) are plan-view SEM image reveal grain in bonding pad with  no pretreatment and 4.9% HF stain, and grain status after ion  milling shows in Fig 1 (c).


Fig 1 (a), (b) and (c) show obvious difference on grain  boundaries. From Fig 1 (a), “Grain boundaries” of Al bonding  pad which is without pretreatment are disarraying and unclear; After 4.9% HF stain, some new “grain boundaries” become  visible as indicated by arrow 1 in Fig. 1 (b). Fig. 1 (c) shows  clearer and sharper boundaries for the sample pretreated by ion  milling. Some “grain boundaries” (marked by arrows 2 and 3  in Fig. 1 (a) and Fig. 1 (b)) are not visible.


The obtained grain sizes with different sample preparation  methods are presented in Table 1. The average pad grain size  without pretreatment is 2.43m; with 4.9% HF stain it is


3.2m; with ion milling it is 5.71m. The pad grain size with  ion milling is nearly two times larger than the grain size with


4.9% HF stain and even more than two times compared to the  grain size without pretreatment). From Eq .(1), different grain  sizes result in different Al bonding pad resistance values, which strongly influence the IC performance. Therefore it  must be clarified which pretreatment method reveals the true  grain size of Al pad.


Table 1: Grain sizes of different sample preparation method.


Method


Grain size (m)


Average Grain  size (m)


Without


pretreatment2.31 2.56 2.41


2.43


4.9%HF  stain


3.30 3.06 3.24


3.2


Ion milling 5.52 6.21 5.42


5.71


Figure 1: SEM image on pad surface combined with different  sample preparation methods (a): pad surface without  pretreatment: arrow 2 indicates a grain boundary that  disappears after ion milling (b): After 4.9%HF stain: the  grain boundary marked by arrow 1 appears after 4.9% HF  stain and arrow 3 indicates the boundary which disappears  after ion milling (c): After ion milling.


Further study will be applied to clarify the real grain size and  those grain boundaries seems discontinuous from surface  images, as shown in Fig.1 (a) and (b) (as arrows2, 3 directed). Our experimental methodology is outlined as follows.


1. The grain boundaries of pads, which were pretreated with


4.9% HF stain and ion milling, were marked with Pt material, as shown in Fig. 2(a) and Fig. 2(c).


2. Regarding to the sample preparation technique of crosssection TEM observation, Al pad under Pt mark were thinned  down to be no more than 0.1 um and also kept Pt mark visible.


3. The diffraction contrast of TEM was performed to boundary  identification.


Fig.2 (b), cross-section TEM observation is performed under  the condition with an incident beam at [110] crystal orientation  to one grain so that a good contrast can be obtained between  two grains. It shows clear boundary but does not match the  previous Pt mark. There is a concave surface under Pt mark.


Fig.2 (d) is the TEM cross-section image of the Al bonding  pad under Pt mark which pad was prepared by ion milling, incident beam was also at one Al grain [110] crystal  orientation, it shows clear grain boundary which was just  under Pt mark.


Fig.2 (a)~(d) show “discontinuous grain boundary” on the pad  surface which is treated with 4.9% HF stain. There are no real  grain boundaries from cross-section TEM results; after ion  milling, the grain boundaries on pad surface are the real grain  boundaries.


Fig. 2 (a). SEM image of pad surface with 4.9% HF stain, Pt  mark was located on a grain boundary.


Fig. 2 (b). TEM cross-section image of the area same as Pt  mark of Fig.2 (a). Marked, the circle area shows the “Boundary” from top-view is a concave surface, not real  grain boundary.


Pt mark


Pt mark  Grain


boundary


Fig.. 2 (c).  SEM image on pad surface with ion milling, Pt  mark was located on a grain boundary.


Fig. 2 (d). TEM cross-section image shows the area same as  Pt mark of Fig.2 (c). The grain boundary from top-view is  real.


For clarifying there were no FIB ion beam damage induced  grain boundaries changed during ion milling, a series of  pictures were taken at different ion milling time (Fig 3 (a)~(d)), Fig 3 (a) was the pad surface without pretreatment.


Fig.3 (a). Al pad surface topography image without  pretreatment.


Fig. 3 (b)~(d). Al pad surface topography images by different  ion milling time  (b) 2min; (c) 4min; (d) 10min.


In Fig. 3 (b), the contrast enhancement between different  grains by the electron crystallographic effect [4] are observed; the grain boundaries are proved to be the true grain boundaries  in Fig. 2 (a)~(d) and they are sharpened by ion milling. From  Fig. 3 (b)~(d), true grain boundaries do not change the  position and they become sharper with milling time increasing, so ion milling wouldn’t cause Al pad grain boundaries change.


A series of FA results show the real grain size obtained by ion  milling. The pad surface phenomena will be discussed further.  After Al deposition and pad formation during processes, Ti/TiN and polymer on the pad are removed by backend dry  etch and acid clean which probably caused some concave/ roughness on pad surface. After that an Al2O3 layer is formed  automatically on pad surface while the wafer is exposed in air.


Grain


Fig. 4 (a) shows the sketch of an Al pad cross-section profile  without pretreatment. The Al2O3 layer uniformly covers the Al  pad, which has a same topography with pure Al pad surface. No strong crystal orientation contrast [5] of Al grain can be  obtained in SEM inspection because the incident electron  beam is scattered by amorphous Al2O3 layer and causes a  reduced beam intensity in the pure Al grain. Only the concave  surface of the pad can be observed. After the HF stain is  applied to the pad as shown in Fig. 4(b), some concaves  caused by HF enhanced etch at grain boundaries appear, however, the Al2O3 layer still remains on the surface and  previous concaves can not be removed by HF stain. An  incorrect grain size measurement is the result because grains  cannot be distinguished from surface concaves.


Ion milling on pad is performed as shown in Fig. 4 (c). The  milling rate of Al at a grain boundary is faster than within a  grain, so that the milling process is enhanced at a grain  boundary. Deep concaves can be observer at the grain  boundaries after ion milling. The Al2O3 layer is totally  removed and the real boundary can be observed with different  contrast of grains induced by crystallographic effect and deep  concave at grain boundary.


Fig. 4 (a). Cross-section profile and SEM imaging mechanism  of Al pad without pretreatment, similar contrast is obtained on  the pad surface due to a reduced incident beam intensity  penetrated into Al grain.


Fig. 4 (b). Cross-section profile and SEM imaging mechanism  of Al pad with HF stain, same as (a) condition.


Fig. 4 (c). Cross-section profile and SEM imaging mechanism  of Al pad with ion milling, no amorphous Al2O3 layer  remained, different penetration depth could be found on the  difference of crystal orientation and significant contrast could  be obtained finally.


Based on above discussion, Al pad surface without  pretreatment or with HF stain both can lead to a wrong Al pad  size measurement results; ion milling allows to observe the  contrast enhancement of the crystallographic effect and also  enhances the grain boundaries. So it is a more credible  pretreatment method for Al pad grain size measurement than  others.


The grain size of the pad is significantly dependent on the  sample preparation method. The grain size in the sample with  ion milling method is much larger than that without  pretreatment or with 4.9%HF stain. TEM cross-section results  showed that such smaller grain size is caused by the artificial  grain boundaries, which is proven to be concave surfaces on  the Al pad. The authenticity of grain boundaries on Al pad  after ion milling was also proven by TEM cross-section. A  series of Al pad surface topography images by different ion  milling time revealed that ion milling does not change Al pad  grain boundaries. The crystallographic effect proved that ion  milling reveals the true Al pad grain from another point of  view. Crystallographic effect and pronounced well grain  boundaries indicate that ion milling is a more credible  pretreatment method for Al pad grain size measurements than  other methods.


The authors would like to thank FA team from Semiconductor  Manufacturing International (Beijing) Corp for their technical  contributions and suggestions to this paper.


[1] Hua younan, Zhao Siping, Mo Zhiqiang, Cho Jie Ying, “Studies of silicon Dust Corrosion on Microchip Al  Bondpads and Elimination of Silicon Dust During Wafer  Sawing Process,” The proceedings of the 32nd  International Symposium for Testing and Failure  Analysis, November 2006, pp.300-304.


[2] A.F. Mayadas and M. Shatzkes, “Electrical-Resistivity  Model for Polycrystalline Films: the case of Arbitrary  Reflection at External Surfaces,” Physical Review. B Vol. 1, 1970, pp. 1382-1389.


[3] S. M. Rossnagel, T. S. Kuan, “Alteration of Cu  conductivity in the size effect regime,” American Vacuum  Society, B 22(1), Jan/Feb 2004, pp. 240~247.


[4] Shipu Chen, Yongrui Wang, Electron Microscopic  Analysis of Metal, Mechanical Industry Press (Beijing, 1982), pp. 169-171.


[5] H.Seiler, “Secondary electron in the scanning electron  microscope,” Journal of Apply. Physics. 1983, pp.  R1~R18.


Al2O3 layer


Poly-grains of Al SE signal


Grain boundary


Poly-grains of Al


SE signal


Fresh Al surface


# Characterization of Green and Ultraviolet LEDs by Laser-based FA Techniques


Characterization of Green and Ultraviolet LEDs by   Laser-based FA Techniques


M. A.  Miller*, E. I. Cole Jr., and P. Tangyunyong


Sandia National Laboratories, Albuquerque, NM USA  *mamill@sandia.gov


As light emitting diodes (LEDs) continue to push into the  commercial mainstream in traffic lights, displays, and lighting, reliability and efficiency become more relevant issues.  The  success of LED mainstream applications is largely attributed to  nitride-based LEDs containing GaN, InN, AlN and their  alloys.  They are now commercially available from the deep  ultraviolet (UV) to the deep green.  Critical to the efficiency  and performance of nitride-based LEDs as well as the  continued expansion of available device wavelengths, is the  identification and fundamental insight into their failure modes.  A major roadblock in supplying efficient, long lifetime LEDs  is the lack of a native or lattice-matched substrate.  Sapphire  and SiC are commonly utilized, but large differences in lattice  spacing contribute significant stress to the nitride epilayers  grown on these substrates.  The result is a considerable  network of threading dislocations and poor quality material.  Other formidable materials issues include increased nitrogen  vacancies in p-type material, increased non-radiative  recombination sites, joule heating due to poor p-type contact  resistance, current crowding, and decreased carrier injection [1-7].  Enabling efficient, reliable devices that increase the  spectrum of available wavelengths requires analysis of the  mechanisms that lead to failure in operating devices.


Recent efforts to pinpoint a specific cause for short lifetimes  and poor reliability in deep green (~530nm) and deep UV  LEDs (~280nm) utilize such methods as time-resolved  photoluminescence, electroluminescence (EL), and  cathodoluminescence [1-7].  This work modifies existing nondestructive, laser-based techniques, such as thermally-induced  voltage alteration (TIVA) and light-induced voltage alteration (LIVA), to determine precursors to failure in green and UV  LEDs.  Both TIVA and LIVA have been shown to be effective  tools in localizing defects in Si-based integrated circuits and  GaAs vertical cavity surface-emitting lasers (VCSELs) [8-9].  In previous work, TIVA was also used to demonstrate failed  InGaN LEDs in the III-V material system [10].  In this paper, we expand the use of these techniques to localize potential  precursors that lead to premature failures in deep green and  deep UV LEDs.  These devices occupy the ends of the  available commercial spectrum and stand to benefit the most  from defect analysis.


The green and UV LEDs were purchased with relative peak  wavelengths of 525nm and 270nm, respectively.  They were  characterized by I-V curves, electroluminescence (EL) spectra, light emission and TIVA/LIVA.  In the microelectronics  failure analysis community, light emission is also synonymous  with photon emission (PE) and electroluminescence (EL).  These techniques are all non-destructive and the chips can  therefore be monitored throughout aging and annealing  without damage to the devices.  The TIVA/LIVA techniques  could provide unique insight into the electrically active defects  in the III-nitride LEDs.  This insight is important to the future  characterization of degradation mechanisms which lead to low  efficiencies and poor reliabilities.


Characterization of Green LEDs


Twenty-four green LEDs were characterized prior to aging.  Each chip was analyzed by TIVA/LIVA over a range of bias  conditions from normal operating currents (350mA) down to  small reverse bias currents.  The LEDs in this work were  analyzed with TIVA and LIVA.  Images are obtained by  mapping the induced voltage changes of the constant current  power supply as the laser scans across the device.  Measuring  changes in voltage rather than current increases sensitivity and  is easier to instrument [11].  Even in the instance of faint  signals, the ac coupled amplifier can detect small variations in  the voltage otherwise altered or masked by background dc  voltages [11].  In this work, the generated images are referred  to as -IVA maps since in some cases it is difficult to pinpoint  whether signals are TIVA or LIVA in character.


Figure 1 shows the top-side reflected light and -IVA map of a  green LED with the 532nm laser beam.  The active region of  the device is defined by the square shape of the chip, outlined  in the figure with a dashed line.  The bond wires that connect  to the bond pads and the thin metal lines that run on top of the  device comprise the n-type contact of the device.  The p-type  contact is made to the backside of the device (not shown).  The  metal lines and bond pads appear black in the -IVA image.  The small black spots are particles on the surface of the LED  and are not electrically active defects (black arrows in figure).  The interesting features in the -IVA image in Fig. 1 are the  small bright spots (white arrows).  The intensity of the bright  spots varied with the applied current under the 532nm laser  stimulus.  Some of the bright spots appeared even without any  applied bias while others “turned on” near 1µA.  Those bright


spots that were present under zero applied bias also remained  as bright spots at negative currents (an increase in voltage).  At  1-5mA, the intensity of the bright spots is so weak that it is not  distinguishable from the background signal.  This suggests that  there is another overriding device effect at higher currents.


Figure 1: Reflected light image (top) of a green LED and  corresponding -IVA map (middle) taken at 10µA with the  532nm laser.  The defect spots appear bright (white arrows).  Particles on the surface which were not electrically active are  denoted with black arrows.  The corresponding light emission  image taken at 10µA is also shown (bottom).  A subtle  darkening is seen at the –IVA site.


Figure 1 also shows the corresponding light emission image of  the green LED.  Only one of the -IVA bright defect spots  could be matched to a discernable spot in the light emission  image.   In the bottom image, the white arrow indicates a dark  spot, where no emitted light is detected.  The subtle dark spot  is not distinguishable from other similar dark spots in the  image, but coincident with the –IVA contrast site.  Light  emission images were taken over the same current range as the  TIVA/LIVA images.  This particular dark spot was only  apparent near 10-100µA and disappeared into the background  noise at higher currents.  This figure shows how the  TIVA/LIVA FA technique provides information beyond that  obtained by light emission alone.


At higher magnifications, the bright spots were not matched to  any obvious physical defects, as shown in Fig. 2.  It is common  practice to roughen the surfaces in LEDs to promote light  extraction.   The surface roughness could obscure physical  defects on the surface or within the underlying layers.  It is  also likely that the defect may be too small to be observed in  the reflected light images.


Figure 2: Reflected light image (left) of a green LED and  corresponding -IVA map (right) taken at 10µA with the 532nm  laser.  No obvious physical defect was observed in the  reflected light image.


It is believed that the bright defects are electron-hole (e-h) pair  recombination sites.  As the 532nm laser is scanned across the  device, the constant-current source momentarily drives the  voltage up to compensate for a drop in power demand at the  defect site.  When examined with longer laser wavelengths, 1064 and 1340nm, no bright defect signal was evident even at  significantly higher laser powers.  This observation suggests a  LIVA (versus TIVA) character to the bright spots.  In terms of  physical defects, the bright spots in the InGaN-based LED  could represent a number of different possibilities including  threading dislocations, point defects, In segregation, or Vdefects.  Further analysis by focused ion beam cross-sectioning  and transmission electron microscopy of the defect is  warranted.


Five of the green LEDs did not show any observable bright  defects under 532nm laser stimulus.  In contrast, strong dark  signals were observed at all laser wavelengths.  The dark  signals were found near physical defects such as a scratch or a  crack.  Figure 3 demonstrates the latter case where dark signals


stimulated with the 532nm laser match the position of the  crack in the reflected light image.  Dark signals in TIVA  suggest a drop in resistance and a corresponding drop in  voltage under constant-current biasing.  This is consistent with  the large reverse leakage currents measured for this device.


Figure 3: Reflected light image (top) of a green LED and  corresponding -IVA map (bottom) taken at 50mA with the  532nm laser.  Leakage paths along the crack appear dark.


Several green LEDs were selected to undergo short-term aging  at 150mA.  This initial aging took place over five hours.  At  two and five hours of aging, the devices were characterized by  TIVA/LIVA and most devices showed no obvious change in  defect number or intensity.  One of the devices, which  contained a strong leakage component, did change.  The -IVA  maps shown in Fig. 4 illustrate an increase in size of the  defective area with aging time.  Other factors that changed  with aging time included an increase in reverse bias current, a  reduction in light emission signal at this defect site, and a  change in the relative intensity of the peak wavelength  measured with EL.  The decrease in peak intensity measured  by EL was also measured in most of the devices.  The EL  spectra for an average device are shown in Fig. 5 for time zero, 2 hours, and 5 hours of aging at 150mA.  As expected, the  overall intensity dropped with increasing aging time.  After 5  hours of aging, none of the devices have showed any  catastrophic failures, defined in this work by shorted devices  or loss of 50% of peak wavelength intensity.  We plan to


further age these devices until catastrophic failures occur.  TIVA and LIVA will be used to monitor the devices up until  and including failure, providing clues to the degradation  mechanisms in these devices.


Figure 4: -IVA map taken at 10µA with the 532nm laser  before aging (top) and after two hours of aging (bottom).


Figure 5: EL spectra of a green LED subjected to aging at  150mA current at time zero (red curve), after 2 hours (blue  curve) and after 5 hours (black curve).  The EL measurements  were performed with an applied current of 350mA.


Characterization of UV LEDs


As with the green LEDs, the UV LEDs were characterized at  time zero and after initial aging to determine if the  TIVA/LIVA FA technique would be able to identify  electrically active defects within the wide bandgap material.  Figure 6 shows a reflected light image and -IVA map of a UV  LED.  These devices are flip-chipped and bonded to TO-39  cans, where the lens and can were removed for ease of  analysis.  The picture is actually acquired through the back of  the sample and the definitive features are the active region (dumbbell-shaped mesa) and the contrast between n-type (outer) and p-type (inner) contacts.  Ideally, the epilayers  would all be transparent to the 532, 1064 and 1340nm lasers.  However, the 532nm laser has detected two electrically active  defects within the device (Fig. 6), shown as dark spots.  If the  defects were thermally stimulated (TIVA), then the spot could  represent a leakage path with a much lower resistance than  surrounding regions.  In addition, the dark spots in the -IVA  map indicated that the defect had a negative temperature  coefficient of resistance (TCR).  A negative TCR means that  resistance of the defect decreases with increasing temperature.   If the dark signals were entirely due to thermal heating from a  laser (TIVA signals), the longer-wavelength lasers should also  create dark signals, as observed in five of the green LEDs.  Some of the UV LEDs, however, showed dark signals only  with a 532nm laser.  These devices showed no defect signals  using a 1064nm laser or a 1340nm laser.  In other devices, the  dark signals were much stronger using a 532nm laser, compared with those signals generated from longerwavelength lasers.  This suggests that there might be an e-h  pair generation component to the signals.  A possible scenario  might entail a two-step e-h pair generation process involving a  deep level defect that is very near the middle of the bandgap.  Unlike the green LEDs, it appears that the LIVA/TIVA  character of the UV LEDs is defect-dependent.


The bottom light emission image in Fig. 6 was taken at 10µA.  There is a bright signature associated with one of the defects, while the other –IVA defect is not observed.  Unlike the light  emission of the green LEDs, this bright spot is very easy to  detect.  This particular defect was only present at lower current  conditions (10-100 µA), like the TIVA/LIVA defect spots.  Again this indicates that there may be different types of defects  in the UV LEDs.


Each of the UV LED devices had 0 to 4 bias-dependent defect  signals located within the active region or along the mesa edge (one of each type is shown in Fig. 6).  Unlike the green LEDs  they were not present under zero applied bias and were not  present under reverse bias.  The signals had a “turn on” current  of 0.6-1µA, the point when they began to appear.  Their  intensity peaked near 1-4µA and diminished until they became  indistinguishable from the background noise near 1-5mA.


Figure 6: Reflected light image (top) and -IVA map (middle) of an UV LED biased at 10µA and imaged with a 532nm  laser.  Corresponding light emission image (bottom) only  shows one of the electrically active defects.


On closer examination of the reflected light image there were  physical defects which matched the position of the dark defect  signal (Fig. 7).  Not only was TIVA/LIVA able to localize an  electrically active defect, it was able to identify that defect  among a large number of optically similar defects in the  surrounding area.


Figure 7: Reflected light image (left) and corresponding -IVA  map (right) of an UV LED biased at 10µA and imaged with a  532nm laser at higher magnification.


The UV LEDs were aged at a current density ~ 100A/cm2 or  30mA.  Although the position and intensity of the dark defects  were not observed to change after 19 hours of aging, one of  the defects developed a new characteristic.  Under reverse  bias, the defect appeared bright when acquired with a reverse  bias of -0.6µA and higher.  The bright spot was not present at  lower reverse bias currents.  The -IVA maps show the defect at  both polarities in Fig. 8.  Note that another dark defect signal  imaged in the forward-biased state in Fig. 8 does not appear to  give a bright defect signal at reverse bias suggesting that there  may be more than one type of defect within the UV LEDs.


Figure 8: Reflected light image (top left) and -IVA maps at  10µA (top right) and -0.6µA (bottom) bias showing dark and  bright defects at forward and reverse bias, respectively.


We have shown how the TIVA/LIVA techniques were  successfully used to characterize defects in wide bandgap  AlGaN- and InGaN-based LEDs.  The defects in the green  LEDs appear to be e-h pair recombination sites and the  observed voltage signals are due primarily to a LIVA effect.


While in the UV LEDs, the observed voltage signals are most  likely the result of both TIVA (thermal heating) and LIVA (photo-current effect due to electron-hole pair generation).  In  both green and UV LEDs, the intensity of TIVA/LIVA signals  is strongly bias-dependent, with no defect signals observed at  currents greater than ~5mA.  Initial aging of the devices brings  about small changes in the LEDs which have been  characterized by TIVA/LIVA.  Further aging to failure may  allow these FA techniques to determine if these observed  defects are precursors to premature failure in InGaN- and  AlGaN-based LEDs.


The authors would like to thank Leonard Riewe, Darlene  Udoni, Shawn Levesque, and Alex Pimentel for their  analytical and technical support.  Sandia National Laboratories  is a multi-program laboratory managed and operated by Sandia  Corporation, a wholly owned subsidiary of Lockheed Martin  Corporation, for the U.S. Department of Energy's National  Nuclear Security Administration under contract DE-AC04-94AL85000.


[1] Moe, C. G., Reed, M. L., Garrett, G. A., Metcalfe, G. D., Alexander, T., Shen, H.,  and Wraback, M., “Degradation  Mechanisms Beyond Device Self-Heating in Deep  Ultraviolet Light Emitting Diodes,” IEEE Int. Reliab. Phys. Symp. Proc., Vol. 94, (2009), pp. 94-97.


[2] Shatalov, M., Gong, Z., Gaevski, M., Wu, S., Sun, W., Adivarahan, V., and Asif Khan, M., “Reliability of  AlGaN-based Deep UV LEDs on Sapphire,” Proc. SPIE, Vol. 6134, (2006), pp. 61340:1-11.


[3] Li, Z. L., Lai, P. T., and Choi, H. W., “A Reliability Study  on Green InGaN-GaN Light-Emitting Diodes,” IEEE  Photonics Technol. Lett., Vol. 21, (2009), pp. 1429-1431.


[4] Cao, X. A., Sandvik, P. M., LeBoeuf, S. F., Aurthur, S. D., “Defect Generation in InGaN/GaN Light-Emitting  Diodes under Forward and Reverse Electrical Stresses,” Microelectron. Reliab., Vol. 43, (2003), pp. 1987-1991.


[5] Meneghini, M., Tazzoli, A., Mura, G., Meneghesso, G., and Zanoni, E., “A Review on the Physical Mechanisms  That Limit the Reliability of GaN-Based LEDs,” IEEE  Trans. Electron. Devices, Vol. 57, (2010), pp. 108-118.


[6] Meneghini, M., Trivellin, N., Trevisanello, L., Lunev, A., Yang, J., Bilenko, Y.,  Sun, W., Shatalov, M., Gaska, R.,  Zanoni, E.,  and Meneghesso, G., “Combined Optical and  Electrical Analysis of AlGaN-Based Deep-UV LEDs  Reliability,” IEEE Int. Reliab. Phys. Symp. Proc., Vol. 46, (2008), pp. 441-445.


[7] Gong, Z., Chhajed, S., Gaevski, M. E., Sun, W. H.,  Adivarahan, V., Shatalov, M., and Asif Khan, M., “Reliability and Degradation Modes of 280 nm Deep UV  LEDs on Sapphire,” Mater. Res. Soc. Symp. Proc., Vol. 892, (2006), pp. 0892-FF09-01.1--01.6.


[8] McElfresh, D. K. and Vacar, D., “Reverse-bias  Electroluminescence Imaging to Diagnose Failures of  Vertical-Cavity Surface-Emitting Lasers,” Appl. Phys. Lett., Vol. 86, (2005), pp. 22108-22108-3.


[9] Herrick, R. W., Microelectronics Failure Analysis, 5th  Edition, ASM International (2004), pp. 229-252.


[10] Barton, D. L., Osinski, M., Helms, C. J., Berg, N. H. and  Phillips, B. S., “Life Tests and Failure Analysis of


AlGaN/InGaN/GaN Blue Light Emitting Diodes,” Proc. SPIE, Vol. 2693, (1995), pp. 64-72.


[11] Cole Jr., E. I., “Techniques for Localization of IC  Interconnection Defects,” Mat. Res. Soc. Symp. Proc., Vol. 716 (2002), pp. B13.1.1-B13.1.11.

