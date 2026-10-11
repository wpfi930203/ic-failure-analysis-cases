---
title: "ISTFA-2019_compressed.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_9a0042b5bf6e933212c9e79029e4c6677295230462135641
file_size: 45041907
---

ISTFATM\


November 10-14,2019


Oregon Convention Center| Portland, Oregon, USA Conference Proceedings from the 45th International Symposium for Testing and Failure Analysis


OColor SpectrumO -An optical micrograph of a


cleavage fracture on a germanium substrate for an


electro-optical application. The fracture resulted in


the dispersion and diffraction of light resulting in


this rainbow-like image.


Fern Leaves - Un-etched aluminum on a bond pad after pad cratering test


Photo submitted by


Luigi Aranda, Raytheon Failure Analysis Lab


Color 2nd Place Winner


Krizalyn Oligario


EDFAS 2018 Photo Contest


Analog Devices Philippines Inc.


000oresulted in inadequate outgassing.


Carlos R. Cuellar


Raytheon Space and Airborne Systems


Black and White 2nd Place Winner


EDFAS


Electronic Device Failure Analysis Society


ASM INTERNATIONAL


ISTFA/2回19INTERNATIONALASM encapsulation for cross-section


nanoporous silicon and follow up


Casper over silicon-etching of


Color 3rd Place Winner


2019


ISTFA  2019


Conference Proceedings from the 45th International Symposium for


Testing and Failure Analysis


November 10–14, 2019 Oregon Convention Center


Portland, Oregon USA


，


一


TM


0


Organized by


Published by


ASM International


Materials Park, Ohio 44073-0002


®


www.asminternational.org/istfa www.asminternational.org


口 brrrd


EOFASISTFA 192 Electronic Device Failure Analysis Society


INTERNATIONAL ASM


Copyright  © 2019


by


ASM International® All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any  means, electronic, mechanical, photocopying, recording, or otherwise, without the written permission of  the copyright owner.


First printing, December 2019


Great care is taken in the compilation and production of this book, but it should be made clear that  NO WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN CONNECTION WITH THIS PUBLICATION. Although this information is  believed to be accurate by ASM, ASM cannot guarantee that favorable results will be obtained from the  use of this publication alone. This publication is intended for use by persons having technical skill, at  their sole discretion and risk. Since the conditions of product or material use are outside of ASM's  control, ASM assumes no liability or obligation in connection with any use of this information. No  claim of any kind, whether as to products or information in this publication, and whether or not based on  negligence, shall be greater in amount than the purchase price of this product or publication in respect  of which damages are claimed. THE REMEDY HEREBY PROVIDED SHALL BE THE EXCLUSIVE  AND SOLE REMEDY OF BUYER, AND IN NO EVENT SHALL EITHER PARTY BE LIABLE  FOR SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES WHETHER OR NOT CAUSED  BY OR RESULTING FROM THE NEGLIGENCE OF SUCH PARTY. As with any material, evaluation of the material under end-use conditions prior to specification is essential. Therefore, specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or reproduction, in connection with any method, process, apparatus, product, composition, or system, whether or not covered by letters patent, copyright, or trademark, and nothing contained in this  book shall be construed as a defense against any alleged infringement of letters patent, copyright, or  trademark, or as a defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN-13:


978-1-62708-273-0 (print)


ISBN:


978-1-62708-274-7 (pdf)


SAN: 204-7586


ASM International®


Materials Park, OH 44073-0002


www.asminternational.org


Printed in the United States of America


i


ISTFA/2019NOVEL COMPUTING ARCHITECTURES


EDFAS 2019-2020 BOARD OF DIRECTORS


EDFAS President


|Dr. Lee Knauss, FASM |Dr. Lee Knauss, FASM |Dr. James J. Demarest |
|---|---|---|

|Booz Allen Hamilton |Booz Allen Hamilton |International Business Machine |

|EDFAS Board Members |Position |Affiliation |

|Dr. Lee Knauss, FASM |President |Booz Allen Hamilton |

|Dr. James J. Demarets |Vice President |International Business Machine |

|Mr. Ryan Ross |Secretary |NASA Jet propulsion Laboratory |

|Dr. Martin Keim |Financial Officer |Mentor Graphics, a Siemens Busines |

|Dr. Zhiyong Wang |Immediate Past President |Maxim Integrated Products |

|Dr. Felix Beaudoin |Member at Large |GLOBALFOUNDRIES |

|Ms. Rebecca L. Holdford |Member at Large |Texas Instruments |

|Mr. Ted Lundquist |Member at Large |Zeiss Smt Pcs |

|Ms. Renee Parente |Member at Large |Advanced Micro Devices (amd) |

|Dr. Tom Schamp |Member at Large |MAS |

|Ms. Mary Anne Jerson |Administrator, Affiliate Societies |ASM Internatioanl |

|Board Committees |Position |Affiliation |

|Dr. Felix Beaudoin |EDFA Chair |GLOBALFOUNDRIES |

|Mr. Bhanu Sood |Education Chair |NASA |

|Dr. Thomas Moore |Membership Chair |Waviks, Inc. |

|Dr. Zhiyong Wang |Awards and Nominations Chair |Maxim Integrated |

|Dr. Felix Beaudoin |Event Chair |GLOBALFOUNDRIES |

s


EDFAS Vice-President


ii


2019 ORGANIZING COMMITTEE


|Dr. Felix Beaudoin |Dr. David Grosjean |Ms. Susan Li |Mr. Randal Mulder |
|---|---|---|---|

|General |Vice General |Technical Program |Tutorial & Short Course |

|Chair |Chair |Chair |Chair |

|GLOBALFOUNDRIES |Butterfly Networks, Inc. |Cypress Semiconductor Corp. |Silicon Labs |

Ms. Efrat Moyal


Immediate Past General Chair LatticGear


|ACTIVITIES CHAIRS |ACTIVITIES CHAIRS |ACTIVITIES CHAIRS |
|---|---|---|

|Yan Li |Zhigang Song |Christian Schmidt |

|Tutorial & Short Course Vice Chair |Panel Co-Chair |Panel Co-Chair |

|Ted Kolasa |Renee Parente |Anita Madan |

|Audio Visual Chair |Audio Visual Vice Chair |User Groups Chair |

|Tejinder Gandhi |Patrick Pardy |Rose Ring |

|User Groups Vice Chair |Local Arrangements Chair |Expo Chair/Movie Chair |

|Becki Watt |Szuhuat Goh |Frank Altmann |

|Expo Vice Chair |International Chair |International Vice Chair |

|Eckhard Langer |Navid Asadi |Vinod Narang |

|Movie Vice Chair |University Chair |University Vice Chair |

|Keith Serrels |||

|FA Technology Roadmap Chair |||

iii


ISTFA 2019 TECHNICAL PROGRAM COMMITTEE


ISTFA 2019 Technical Program Chair


Ms. Susan Li


Cypress Semiconductor Corp.


|Session Chairs |Session Chairs |Session Chairs |
|---|---|---|

|3D Device Failure Analysis |FIB Circuit Analysis and Edit |Nanoprobing and Electrical |

|Christian Schmidt, NVIDIA |Daminda Dahanayaka, GLOBALFOUNDRIES |Characterization |

|Kristofor Dickson, NXP |Antonio Tollis, Analog Devices |Sweta Pendyala, GLOBALFOUNDRIES |

|||John Sanders, Thermo Fisher Scientific |

|Board and System Level FA |FIB Sample Preparation |Packaging & Assembly Level FA |

|Jason Wheeler, Raytheon |Bryan Tracy, Evans Analytical Group |Kannu Wadhwa, ZEISS |

|Becky Holdford, Consultant |Jake Jensen, Thermo Fisher |Peng Li, Intel Corporation |

|Detecting and Preventing Counterfeit |Hardware Attacks, Security, and Reverse |Product Yield, Test & Diagnostics |

|Microelectronics |Engineering |Jayant D’Souza, Mentor, A Siemens |

|Michael H. Azarian, CALCE, University of |Haoting Shen, University of Florida |Business |

|Maryland |Shahin Tajik, University of Florida |Shahin Tajik, University of Florida |

|Martine Simard-Normandin, |||

|MuAnalysis |||

|Emerging FA Techniques and Concepts |Low Power Devices and Test Structures Case |Low Power Devices and Test Structures Case |

|Frank Altmann, Fraunhofer Institute for |Studies |Studies |

|Mechanics of Materials |Michael Bruce, Consultant |Michael Bruce, Consultant |

|Keith Serrels, NXP |Rose Ring, Howard Hughes Research Labs, LLC |Rose Ring, Howard Hughes Research Labs, LLC |

|FA Processes Case Studies |Microscopy |Microscopy |

|Chuan Zhang, NVIDIA |Lianfeng Fu, Lam Research Corporation |Lianfeng Fu, Lam Research Corporation |

|Erwin Hendarto, Silicon Labs |Ryan Fredrickson, ON Semiconductor |Ryan Fredrickson, ON Semiconductor |

|Fault Isolation |Mixed Mode & High Power Devices Case |Mixed Mode & High Power Devices Case |

|Dan Bodoh, NXP |Studies |Studies |

|Jesse Alton, Teraview |Stephen T. Fasolino, Raytheon Jeff Gambino, ON Semiconductor |Stephen T. Fasolino, Raytheon Jeff Gambino, ON Semiconductor |

|Silicon Photonics FA (New) |Silicon Photonics FA (New) |Silicon Photonics FA (New) |

|Felix Beaudoin, GLOBALFOUNDRIES |Felix Beaudoin, GLOBALFOUNDRIES |Felix Beaudoin, GLOBALFOUNDRIES |

|Artemisia Tsiara, IMEC |Artemisia Tsiara, IMEC |Artemisia Tsiara, IMEC |

iv


Contents


3D Device Failure Analysis


Advanced 3D Localization in Lock-in Themorgraphy Based on the Analysis of the TRTR


(Time-Resolved Thermal Response) Received Upon Arbitrary Waveform Stimulation .............. 1


Sebastian Brand1, Michael Kögel1, Christian Grosse1, Frank Altmann1, Brian Lai2, Qingqing Wang2, James Vickers2, David Tien2, Bernice Zee3, Qiu Wen3


(1) Fraunhofer IMWS, Halle, Germany


(2) Thermo Fisher Scientific, Fremont, California, USA


(3) Advanced Micro Devices Device Analysis Lab, Singapore


Non-Destructive Short Fault Localization in Advanced IC Packages Using Electro Optical


Terahertz Pulse Reflectometry ............................................................................................ 9


B. Zee1, W. Qui1, J. Alton2, T. White2, M. Igarashi2, D. Sullivan2


(1) Device Analysis Laboratory, Advanced Micro Devices, Austin Texas, USA


(2) TeraView Limited, Cambridge, UK


Modern 2D & 3D X-ray Technologies for Testing and Failure Analysis  .................................... 14


Herminso Villaraga-Gómez and Joshua D. Bell, Nikon Metrology Inc., Brighton, Michigan, USA


Localization of Dielectric Breakdown Sites in 3D Through-Silicon Via (TSV) Interconnects by


Laser Stimulation and Chip Deprocessing  .......................................................................... 20


K.J.P. Jacobs1, Y. Li1, I. De Wolf1,2, S. Van Huylenbroeck1, E. Beyne1


(1 )Imec, Kapeldreef 75, B-3001 Leuven, Belgium


(2) KU Leuven, Dept. Materials Engineering, B-3001 Leuven, Belgium


GHz-SAM for Warped Samples using HiSA ........................................................................... 25


C. Hollerith, D. Le 1, P. Hoffrogge2, M. Böckler3


(1) Infineon AG, Neubiberg, Germany


(2) PVA TePLA, Westhausen, Germany


(3) HS Aalen, Aalen, Germany


GHz-Scanning Acoustic Microscopy Combined with ToF-SIMS/AFM for Wafer-Level Failure


Analysis of Bonding Interfaces ...........................................................................................29


Ingrid De Wolf1,2, Ahmad Khaled1,2, Alexis Franquet1, Valentina Spampinato1, Thierry Conard1, Sebastian  Brand2, Michael Kögel2, Ingo Weisler3


(1) IMEC, Leuven, Belgium


(2) Department of Materials Engingeering (MTM), Leuven, Belgium


(3) FhG IMWS-CAM, Halle, Germany


(4) PVA TePla Analytical Systems GmbH, Westhausen, Germany


Machine Learning Assisted Signal Analysis in Acoustic Microscopy for Non-Destructive Defect


Identification  .................................................................................................................. 35


Michael Kögel, Sebastian Brand, Frank Altmann


Fraunhofer Institute for Microstructure of Materials and Systems, IMWS, Halle, Germany


v


Board and System Level FA


Solder Bump Joint Failure Investigation: From Sample Preparation to Advanced Structural


Characterizations and Strain Measurements  ...................................................................... 43


Pawel Nowakowski, Mary Ray, and Paul Fischione ,E.A. Fischione Instruments, Inc., Export, Pennsylvania, USA


The Development of an EVB Socket Solution for Automotive Mixed-Signal ICs  ....................... 48


Eric Cattey1, Alex Van Vianen1, Mitch Curiel1, Gustav Huo1, Kristofor Dickson2, Yvette Meiche2


(1) NXP Semiconductors, Chandler, Arizona


(2) NXP Semiconductors, Austin, Texas


Detecting and Preventing Counterfeit Microelectronics


ToF-SIMS, Time-of-Flight Secondary Ion Mass Spectroscopy for Counterfeit Detection of


Electrical, Electronic, and Electromechanical (EEE) Parts .................................................... 53


M. Simard-Normandin1, C. Banks1, N. Havercroft2, P. Clark3, E. Tallarek4


(1) MuAnalysis, Ottawa, Ontario, Canada


(2) ION-TOF USA, Chestnut Ridge, New York, USA


(3) Tascon USA, Chestnut Ridge, New York, USA


(4)Tascon GmbH, Muenster, Germany


Emerging FA Techniques


Time-Resolved Imaging of VLSI Circuits using a Single-Point Single-Photon Detector


and a Scanning Head ........................................................................................................ 60


Franco Stellari1, Peilin Song1, Yoshitaka Iwaki2, Stanley Kim2, and Manuel Villalobos2


(1) IMB, Yorktwon Heights, New York, USA


(2) Hamamatsu Photonics, Japan & USA


A Study of Clustering for the Enhancement of Image Resolution in Dynamic Photon


Emission ..........................................................................................................................68


S. Chef1, C.T. Chua1, C.L. Gan1,2


(1) Temasek Laboratories@NTU, Nanyang Technological University, Singapore


(2) School of Material Sciences Engineering, Nanyang Technological University, Singapore


Automated Multi-level Circuit Net Trace for Hotspot Analysis .............................................. 79


S.H. Goh1, E. Susanto1, Song Li1, B.L .Yeoh1, M.H. Thor1, D. Zhou2


(1) GLOBALFOUNDRIES, Product Diagnostic Engineering, Singapore


(2) Mentor, A Siemens Business


V-Pulse Technique For Optical Isolation Of Latchup Triggers In Sub-14 nm Standard-Cell Logic


and Memory .................................................................................................................... 86


William Lo, Puneet Gupta, Yen-Tzu Lin, Rakshith Venkatesh, Rudolf Schlangen, Jane Li, Chuan Zhang, Howard Marks, and Bruce Cory, NVIDIA, Santa Clara, California, USA


Integrated Diffractive Lenses for Ultrathin Silicon............................................................... 90


Marc van Veenhuizen1, Peter van der Cruijsen1, Keith A. Serrels2, Frank Zachariasse3


(1) Product Diagnostic Center, Nijmegen, The Netherlands


(2) Product Diagnostic Center, Austin, Texas, USA


(3) Business Line Secure Transactions & Identification, NXP Semiconductors, Nijmegen, The Netherlands


vi


FA Processes Case Studies


Infrared Lock-In Thermography: From Localization of Low Power and Masked Defects to


Absolute Temperature Mapping for Product Debug ............................................................104


J. Jalink1, A. Firiti1, J. van den Biggelaar1, A. Reverdy2, B. Lai3


(1) NXP Semiconductors, Nijmegen, The Netherlands


(2) Sector Technologies, Eybens France


(3) ThermoFisher Scientific, Fremont, California, USA


Contact Leakage Failure Analysis by EBIC, C-AFM and Nano-probing ...................................111


Kuang-Tse Ho, Chien-Wei Wu, Te-Fu Chang, Chia-Hsiang Yen and Ching-Hsiang Chan  Materials Analysis Technology, Hsinchu City, Taiwan


Contamination Troubleshooting Approach from Problem to Solution.................................  116


Victor K.F. Chia, Hugh E. Gotts, Fuhe Li and Mark Camenzind Balazs, NanoAnalysis, Fremont, California, USA


Case Study of Electro-Optical Probing Signal with High Signal-Noise Ratio .......................... 123


Ryan Xiao, William Wang, Ang Li, Shengqiu Xu, Binghai Liu  NXP Semiconductors, Tianjin, China


Artefacts of SEM/TEM Observations Cases on Seal Ring Structure and Correctives Samples


Preparations to Avoid Them .............................................................................................130


Christophe Charles and  Alain Margain, ST Microelectronics, Crolles Cedex, France


Re-Packaging Solution of Bare Dice From Customer Packages To Open-Cavity


Ceramic Packages ...........................................................................................................135


Raymond G. Mendaros1, Bernardino D. Mazon1, Eugene Capito1, Romeo S. Soriano Jr.2


(1) Global Failure Analysis, Cavite, Philippines


(2) Worldwide Manufacturing, Cavite, Philippines


A Novel Approach on Fractography through Infrared ......................................................... 140


Allan Norico and Rommel Estores , ON Semiconductor Belgium BVBA


Case Studies on Application of Electro Optical Probing (EOP) — A Noninvasive Backside


Localization Technique in Failure Analysis.........................................................................148


Srinath Rajaram, Rajesh Kabadi, and Eric Barbian,


Product Analysis Lab, ON Semiconductor, Phoenix, Arizona, USA


Understanding Water Ingress in Scanning Acoustic Microscopy and a Method to Observe Defects


that are Open to the Surface ............................................................................................154


Adam Benak, and Roger Devaney, Hi-Rel Laboratories, Spokane, Washington


Fault Isolation


Dynamic Photon Emission on FinFET Devices Through Novel Scan Test Approaches .............160


Ranganathan Gopinath1, Ravikumar Venkat Krishnan1,2, Lua Winson1, Phoa Angeline1, Jin Jie1


(1) Advanced Micro Devices, Singapore


(2) Singapore University of Technology and Design, Singapore


vii


Thermal Failure Analysis of Functional Failures by IR Lock-in Thermal Emission ................... 164


Paul Hubert P. Llamera and Camille Joyce G. Garcia-Awitan,


Maxim Integrated – Failure Analysis Department, Cavite, Philippines


Interpreting Laser-Based Fault Localization Results: Case Studies ...................................... 168


Sukho Lee, John van den Biggelaar, Marc van Veenhuizen,


Product Diagnostic Center, NXP Semiconductors, Nijmegen, Netherlands


Fast and Accurate Fault Localization Through Effective Use of Design Schematics ................ 173


Ankush Oberai1, Rupa Kamoji2, Arpan Bhattacherjee3


(1) Synopsys Inc. Mountain View, California, USA


(2) Synopsys India Pvt. Ltd. Mumbai, Maharashtra, India


(3) Synopsys Inc. Mountain View, California, USA


MBIST Driven SRAM Failure Analysis Using Laser Voltage Imaging and Laser Voltage


Probing .......................................................................................................................... 179


Jessica Yang, Omprakash Rengaraj, Puneet Gupta, Rudolf Schlangen NVIDIA, Santa Clara, California, USA


A New Approach to IDDQ Failure Fault Localization Using Single Shot Logic (SSL) Patterns ...182


Rommel Estores and Stefaan Verleye , ON Semiconductor Belgium BVBA


Comparison of He+ and Ga+ Voltage Contrast in N-wells ....................................................192


Gregory M. Johnson, David Ferranti, John Notte, Brett Lewis, Chris H. Park, Ted Lundquist, Baohua Niu, Carl Zeiss PCS, Pleasanton CA, Peabody, Massachusetts, USA


Failure Analysis of FinFET Circuitry at GHz Speeds using Voltage-Contrast and Stroboscopic


Techniques on a Scanning Electron Microscope .................................................................197


James Vickers1, Seema Somani1, Blake Freeman1, Pete Carleson2, Lubomír Tůma3, Marek Unčovský3, Petr Hlavenka3


(1)Thermo Fisher Scientific, Fremont, California, USA


(2)Thermo Fisher Scientific, Hillsboro, Oregon, USA


(3)Thermo Fisher Scientific, Brno, Czech Republic


FIB Circuit Analysis and Edit


Forming Discrete Components on an Integrated Circuit Utilizing Focused Ion Beam Direct Write


Capabilities ....................................................................................................................204


Kyle M. Winter, Steven B. Herschbein, Carmelo F. Scrudato, Brian L. Yates, GLOBALFOUNDRIES, EFK CCA , Hopewell Junction, New York, USA


Visualization and Measurements of 3D Structures in Memory and Logic Devices ..................209


A. Avishai1, A. Buxbaum1, D. Klochkov2, J.T. Neumann2, T. Korb2, and E. Foca2


(1) Carl Zeiss SMT Inc., Pleasanton, California, USA


(2) Carl Zeiss SMT GmbH, Oberkochen, Germany


viii


FIB Sample Preparation


Applying a Significant Protection Layer on Double Ex Situ Lift-out TEM Specimens to Protect


Against Ion Beam Impact ................................................................................................  215


Chun-Hung Lin, Hsin-Cheng Hsu, Tsung-Yi Lin, Ru-Hui Lin, I-An Chen, Pei-Lin Hsu, Chao-Kun Chen, Iris Hsieh, Chin-Chih Yeh, Nan-Tzu Lian, Ta-Hone Yang, Kuang-Chao Chen,


Macronix International Co. Ltd, Li-Hsin Road, Hsinchu Science Park, Hsinchu, Taiwan


Variable Angle TEM Grid Holder for Advanced TEM Lamellae Preparation ............................219


Tomáš Hrnčíř1, Marek Šikula1, Pavel Doležel1, Claudio A. G. Savoia2


(1) TESCAN Brno s.r.o., Brno, Czech Republic


(2) STMicroelectronics, Agrate Brianza, Italy


Optimisation of Large Chunk Lift-Out Method and Lamella Preparation for CBED Measurements


using Xenon Plasma FIB ................................................................................................... 223


Miloš Hrabovský1, Tomáš Morávek1, Chandran Narendraraj1, Jürgen Gluch2, Martin Gall2, Ehrenfried Zschech2, Uwe Mühle3


(1) TESCAN Brno, s.r.o., Brno, Czech Republic


(2) Fraunhofer Institute for Ceramic Technologies and Systems IKTS, Dresden, Germany


(3) Institute of Materials Science, Dresden, Germany


Automated Gas-Enhanced PFIB Surface Preparation Enabled Metrology and Statistical Analysis


of 3D NAND Devices .........................................................................................................227


Chris Hakala, James Clarke, Mark Biedrzycki, Kesley Price, Jamie Johnson, Gavin Mitchson, Thermo Fisher Scientific, Hillsboro, Oregon, USA


FIB Enhancement of Mechanically Polished Cross-sections ................................................. 232


Becky Holdford, Retired Failure Analyst, Garland, Texas, USA


3D-Printed Samples For EXLO/INLO Practice and Training ..................................................236


Zachary A. Giannuzzi1, Lucille A. Giannuzzi1, Kathleen A. Gehoski2, William J. Mahoney2


(1) EXpressLO LLC, Lehigh Acres, Florida, USA


(2) The Pennsylvania State University, University Park, Pennsylavania, USA


Low Energy Xe+ PFIB Specimen Preparation for Cs-Corrected HRSTEM Imaging ...................241


Lucille A. Giannuzzi1, Paul A. Anzalone1, Jiancun Rao2, Tom Hoffman3, Mike McKie3, Joseph Girgis3, Takayuki  Kuwahara3, Jamie Ford4, Douglas M. Yates4, Eric A. Stach4


(1) TESCAN USA, Warrendale, Pennsylvania USA


(2) University of Maryland, College Park, Maryland, USA


(3) JEOL USA, Peabody, Maryland, USA


(4) The University of Pennsylvania, Philadelphia, Pennsylvania, USA


Localizing IC Defect Using Nanoprobing: A 3D Approach ..................................................... 244


Jane Y. Li, Chuan Zhang, John Aguada, Christopher Nemirow and Howard Marks,NVIDIA Corporation, Santa Clara, California, USA


Hardware Attacks, Security, and Reverse Engineering


A Novel Approach to Unsupervised Automated Extraction of Standard Cell Library for Reverse


Engineering and Hardware Assurance ............................................................................... 249


Ronald Wilson, Rabin Y. Acharya, Domenic Forte, Navid Asadizanjani and Damon Woodard, Florida Institute for Cyber Security, University of Florida, Gainesville, USA


ix


A Review on Automatic Bill of Material Generation and Visual Inspection on PCBs  ............... 256


Mukhil Azhagan M. S1, Dhwani Mehta1, Hangwei Lu1, Sudarshan Agrawal1, Mark Tehranipoor1, Damon L. Woodard1, and Navid Asadizanjani1, Praveen Chawla2


(1) Florida Institute for Cybersecurity (FICS), ECE Department, University of Florida, Gainesville, USA


(2) Edaptive Computing Inc., Dayton, Ohio, USA


Low Power Devices Case Studies


Stress Analysis of Damage in Active Circuitry beneath Redistribution Layer (RDL) Bonding Pad


and Improvements for Reliability ....................................................................................  266


Chih-Ching Shih, Wei-Hao Hsiao, Leo Chan, Hsiao-Tien Chang, Li-Kuang Kuo, Ding-Jhang Lin, Yen-Hai Chao, Chih-Yuan Lu , Macronix International Co. Ltd., Hsinchu, Taiwan


Nanoprobe Characterization of Soft SRAM Bit Fails in Advanced Technologies ...................... 273


Satish Kodali, Chen Zhe, Chong Khiam Oh, GLOBALFOUNDRIES Inc, Malta, New York, USA


Microscopy


Development of a Characterization Workflow for Reliable Porous Copper Films using SEM-FIB


Tomography and Advanced Image Analysis ......................................................................  277


Andi Wijaya1, Jördis Rosc1, Bernhard Sartory1, Roland Brunner1, Barbara Eichinger2, Martin Mischitz2


(1) Materials Center Leoben Forschung GmbH, Styria Austria


(2) Infineon Technologies Austria AG, Carinthia Austria


Speeding up Chip Layer Imaging with a Multi-Beam SEM ....................................................281


A. L. Eberle, T. Garbowski, S. Nickell, D. Zeidler,


Carl Zeiss Microscopy GmbH, Oberkochen, Germany


Analysis of Voltage Contrast in Secondary Electron Images Using a High-energy Electron


Spectrometer ................................................................................................................. 286


Natsuko Asano1, Shunsuke Asahina1, Natasha Erdman2


(1) JEOL Ltd., Tokyo, Japan


(2) JEOL USA, INC., Peabody, Maryland, USA


Submicron Simultaneous IR and Raman Spectroscopy (IR+Raman): Breakthrough Developments in Optical Photothermal IR (O-PTIR) Combined for Enhanced Failure Analysis .......... 292


Jay Anderson1, Mustafa Kansiz1, Michael Lo1, Curtis Marcott2


(1) Photothermal Spectroscopy Corp., Santa Barbara, California, USA


(2) Light Light Solutions, Athens, Georgia, USA


High Throughput and Multiple Length Scale Sample Preparation for Characterization and


Failure Analysis of Advanced Semiconductor Devices .........................................................295


C.S. Bonifacio1, P. Nowakowski1, M.L. Ray1, P.E. Fischione1, C. Downing2


(1) E.A. Fischione Instruments, Inc., Export, Pennsylvania, USA


(2) The Advanced Microscopy Laboratory, CRANN, Trinity College Dublin (TCD), Dublin, Ireland


x


New Paradigm for EBIC Amplifier on FIB X-Section ............................................................. 302


Valerio Sanna Valle1, Guy Perez2, Guillaume Bascoul2, Helene Chauvin3, †Benoît Viallet4, Giovanna Muraa1, Gian Paolo Apeddu1


(1) University of Cagliari, Cagliari, Italy


(2) Centre National d’Etudes Spatial, Toulouse, France


(3) Thales, Toulouse, France


(4) Institut National des Sciences Appliquées Toulouse, France


Super XHR Cross-Sectional SEM Imaging & EDS Analysis: A Systematic Method for High-Fidelity


Microstructure Characterization of Dense SRAM FinFET ....................................................  308


Zdenek Kral1, Jake Jensen1, Lisa McGill1, Trevan Landin1, Roger Alvis1, Stephen M. Seddio2, Chris Stephens2


(1) Thermo Fisher Scientific, Hillsboro, Oregon, USA


(2) Thermo Fisher Scientific, Madison, Wisconsin, USA


Mixed Mode & High Power Devices Case Studies


Failure Analysis Approaches for Stacking Fault Defects in FinFET Devices ............................313


Beomjun Kim, Seonghee Park, Juhyun Kim, Moonhyun Lee, Seongjun Cho, Seokjun Won, Jinsung Kim,Samsung Electronics Co., Gyeonggi-do, South of Korea


Residual EG Oxide in FinFET Analyses and Its Impact to Yield, Product Performance, and


Transistor Reliability ....................................................................................................... 317


Pat McGinnis, Dave Albert, Zhigang Song, Johns Oarethu, Phong Tran, John Sylvestri, Greg Hornicek, Mike  Tenney, IBM Systems: Product Engineering Failure Analysis, Hopewell Junction, New York, USA


Enhancing Point Defect Isolation by Using Ionizing Radiation ............................................. 323


Douglas J. Martin1, Matthew J. Gadlage1, Wai-Yat Leung1, Jeffrey L. Titus2


(1) Naval Surface Warfare Center, Crane, Indiana, USA


(2) AECOM, Odon, Indiana, USA


Nanoprobing and Electrical Characterization


NanoProbing on 7 nm FinFET Devices in an SRAM Array: Challenges and Solutions ...............329


Anqi Qiu, William Lowe, Mridul Arora, Thermofisher Scientific, Richardson, Texas, USA


Application of Nanoprobing on Subtle Defects in the Embedded Non-Volatile


Memory Device ...............................................................................................................336


C.Q. Chen, P.T. Ng, S.P. Neo, P.K. Tan, A.C.T. Quah, J. Zhu, GLOBALFOUNDRIES Pte.Ltd, Singapore


Failure Analysis on Inter Polysilicon Oxide Reliability Issues of 40nm Automotive


NVM Device ....................................................................................................................340


P.K. Tan, R. Fransiscus, Y.L. Pan, H.H.W. Thoungh, S.L. Ting, Y.Z. Zhao, T.L. Wee, H. Tan, S.P. Neo, C.Q. Chen, Globalfoundries Singapore Pte. Ltd, Singapore


Transistor Level Reliability Assessment of Gate Oxide Defects by BTI Stress Nanoprobing .....346


Dave Albert, Zhigang Song, Mike Tenney, Pat McGinnis, Johns Oarethu ,


IBM Systems: Product Engineering Failure Analysis, Hopewell Junction, New York, USA


xi


Capacitance Characterization of Gate to LDD Overlap Region to Understand Subtle Fail Modes


in Advanced Node Technologies .......................................................................................359


Satish Kodali, Edmund Banghart, Kevin Davidson, Yu Zhang, Jagar Singh, Chong Khiam Oh, GLOBALFOUNDRIES Inc, Malta, New York, USA


Root Cause Analysis of High Input Offset Voltage in Mixed-Signal Design Through Nanoprobing


and Cadence Simulation ..................................................................................................366


Zhenni Wan, Weikai Yin, Yining Zang, Madhukar Karigerasi, Saurabh Kulkarni, Wui Chung Yap, Dian Yu, Naiyi  Wang, Qindi Wu, Maxim Integrated, San Jose, California, USA


Application of Two-pin EBIC Technique to Isolate the Defective Fin(s) in Advanced Bulk


FinFET Devices ................................................................................................................372


Kah Chin Cheong, Liangshan Chen, Yuting Wei, Yu Zhang, Brian Popielarski, Xiaodong Zhang, Chongkhiam  Oh, GLOBALFOUNDRIES, Malta, New York, USA


Efficient Fault Isolation and Failure Analysis Methods to Root Cause Defects in


Microprocessors ..............................................................................................................377


Hasan Faraby, Tristan Deborde, Martin von Haartman, Intel, Hillsboro, Oregon, USA


Nanoprobing of Advanced Silicon-on-Insulator Transistors .................................................381


Stefano Larentis, Kent Erington, Jose Z. Garcia, Khiem Ly, Kris Dickson, Tony Chrastecky, Steve Heineke, Nelson Gomez and Sam Subramanian, NXP Semiconductors Inc., Austin, Texas, USA


Packaging & Assembly


Conductive-Dissipative-Isolating - Do the Actual Limits in Process Equipment Meet the


Requirements of ESD-Sensitive Devices? ...........................................................................388


Peter Jacob, Albert Kunz , Empa Material Science & Technology, Duebendorf, Switzerland


Isolating an Open in 2.5D µBump & Chip Bump Chains using SDR, EBAC and Capacitive


Measurements ................................................................................................................ 393


Kevin Distelhurst, Doug Hunt, Dan Bader, GLOBALFOUNDRIES, Essex Junction, Vermont, USA


Novel X-ray Microscopic Chemical Imaging for Rapid Non-Destructive Identification of


Structural and Compositional Defects— From Microbumps to FinFET ...................................397


S.H.Lau, Benjamin Stripe, Sylvia Lewis, Xiaolin Yang, Wenbing Yun , Sigray, Inc. Concord, California, USA


Study of Thermal Cycle Induced CPI Failure Mode in a Lidded FC-BGA Package ..................... 402


Muhammad Monzur Morshed, Esther Chen and Anita Madan, GLOBALFOUNDRIES, Malta, New York, USA


Nickel Flakes: Past, Present and Future ............................................................................ 405


Ken Turner and Kevin Polito, Hi-Rel Laboratories, Spokane, Washington, USA


xii


Product Yield, Test, & Diagnostics


LADA Synchronization for Symmetric and Asymmetric ATE Test Program Cycles  .................. 410


Arun Kumar Karunanithi, Joseph Caroselli, Jason Christensen, Michell Espitia, Advanced Micro Devices, Inc., Austin, Texas, USA


Utilizing Delta IDDQ to Screen Cell Specific Defects for High Quality and


Reliability Applications ...................................................................................................415


Eric Barbian, Niel Sanico, Julien Thiefain, Andy Koestner, ON Semiconductor, Phoenix, Arizona, USA


A Manual Diagnosis Approach Using Targeted Fault Injection and Fault Simulation to Extend


ATPG Diagnostic Resolution in Localizing Faults ................................................................419


Rommel Estores and Karo Vander Gucht , ON Semiconductor Belgium BVBA


The Investigation of Oven Contamination and Corresponding Methodology ........................426


W.F. Hsieh, Henry Lin, Vincent Chen, Jun Liu, Irene Ou, Y.S. Lou, Ardentec Cooperation,, Hukou Township, Taiwan


Statistical Failure Analysis for Non-parametric Characteristic in DRAM ................................430


Myunghoon Oak, Jongbum Lee, Jungwon Bae, Kyungrak-Cho, Minju-Shin, Choongsun Park,


Sunghoon Park, Hongsun Hwang, Taeyoung Oh, Jonghoon Kim, and Jungbae Lee, Samsung Electronics  Co.,Ltd, Republic of Korea


Loop Transformation Algorithm for Test Vector Accessing at High Speed ............................. 434


Bjorn Dahlberg1 and Martin Versen2


(1) HILEVEL Technology Inc., Irvine, California, USA


(2) Technical University of Applied Sciences Rosenheim, Rosenheim, Germany


Sample Preparation and Device Processing


Artifact-Free Decapsulation of Silver Wire Bonded Semiconductor Devices Using Microwave


Induced Plasma .............................................................................................................. 440


J. Tang1, J. Wang1, W. van den Hoek1, D. Lohier2, B. Forgerit2, G. Gabaston2, C.I.M. Beenakker3


(1) JIACO Instruments, Delft, The Netherlands


(2) HIREX Engineering, Toulouse, France


(3) Delft University of Technology, Delft, The Netherlands


Second Order Effect Monitoring During Backside Milling for Functional End Point


Detection .......................................................................................................................445


Anthony George, Isaac Goldthwaite, Katie Liszewski, Jeremiah Schley, Thomas Kent,Battelle Memorial Institute, Columbus, Ohio, USA


Submicron Thinning of finFET Devices with High Power Density Observed in 10/7nm Process


Nodes using High Aspect Ratio Trenches ..........................................................................  454


Nathan Bakken1, Vladimir Vlasyuk1, Michael Beal1, Ilya Artishuk1, Robert Chivas2, Mike DiBattista2, Scott Silverman2


(1) Intel Corporation, Folsom, California, USA


(2) Varioscale, San Marcos, California, USA


xiii


Site-specific Low Angle Plasma FIB Milling for Cross-sectional Electrical Characterization ....460


Chuan Zhang, Jane Y. Li, John Aguada and Howard Marks, NVIDIA Corporation, Santa Clara, California, USA


Ultra-Thinning of Silicon for Backside Fault Isolation .........................................................465


M. J. Campin, P. Nowakowski, and P. E. Fischione , E.A. Fischione Instruments, Inc., Export, Pennsylvania, USA


Transmission Electron Microscopy Sample Preparation By Design Based Recipe


Writing in a DBFIB Part 2 .................................................................................................. 470


J. Demarest1, B. Austin1, J. Arjavac2, M. Breton1, M. Bergendahl1, M. Biedrzycki2, C. Boye1, B. Cilingiroglu2, J.Gaudiello1, J. Hager2, S. Matham1, K. Nguyen2, M. Persala2, M. Rizzolo1, S. Shaar2, S. Teehan1


(1) IBM, Albany, New York, USA


(2) ThermoFisher, Hillsboro, Oregon, USA


Targeted Silicon Ultra-thinning by Contour Milling for Advanced Fault Isolation ...................472


MW.S. Teo1,2, M.S. Wei1, V. Narang1, C.L. Gan2, C. Richardson3 and G. Liechty3


(1) Device Analysis Laboratory, Advanced Micro Devices (Singapore) Pte Ltd, Singapore


(2) Nanyang Technological University, Singapore


(3) Allied High Tech Products Inc., California, USA


Scanning Probe Analysis


A Novel Method of Fabrication of Metal Probes for Scanning Probe Microscopy ................... 479


Michał Milczarek and Dariusz M. Jarząbek


Institute of Fundamental Technological Research, Polish Academy of Sciences, Warsaw, Poland


Scanning Capacitance Microscopy and Spectroscopy for Root Cause Analysis on Location


Specific Individual FinFET Devices ....................................................................................484


Phil Kaszuba, Leon Moszkowicz, Randy Wells, Globalfoundries, Essex Junction, Vermont, USA


Carrier Profiling of the 10-nm-order Structure in a 3D Flash Memory Cell using Scanning


Nonlinear Dielectric Microscopy .......................................................................................490


Jun Hirota1, Ken Hoshino1, Tsukasa Nakai1, Kohei Yamasue2, Yasuo Cho2


(1) Institute of Memory Technology Research & Development, Toshiba Memory Corporation, Yokkaichi, Mie, Japan


(2) Research Institute of Electrical Communication, Tohoku University, Sendai, Japan


2D Carrier Density Mapping using SNDM-dC/dV and dC/dz of SiC Power MOSFET ..................494


Jing-jiang Yu1, T. Yamaoka2, T. Aiso2, K. Watanabe3, Y. Shikakura3, S. Kudo3, K. Tamura4, K. Mizuguchi4


(1) Hitachi High Technologies America, Inc., Clarksburg, Maryland, USA


(2) Hitachi High Technologies, Kanagawa-ken, Japan


(3) Hitachi High-Tech Science Corporation, Shizuoka-ken, Japan


(4) Hitachi High Technologies, NishiShimbashi, Japan


Unintentional Doping Effects on Atomically-Thin Nb-Doped MoS2 Observed by Scanning


Nonlinear Dielectric Microscopy ....................................................................................... 498


Kohei Yamasue and Yasuo Cho, Research Institute of Electrical Communication, Tohoku University, Sendai, Miyagi, Japan


xiv


The Potential of Inline Automated Defect Review of Mechanical Property and


Electrical Characterization by AFM ...................................................................................504


Sang-Joon Cho, Seong-Oh Kim, Moses Lee and Yoonkyoung Lee, R&D Advanced Application Center, Park Systems Corp, Suwon, Republic of Korea


Si Photonic FA


Introduction of a Novel Sample Preparation Technique for the Failure Analysis of Silicon


Integrated Photonics Modules ..........................................................................................508


Pradip Sairam Pichumani, Fauzia Khatkhatay, GLOBALFOUNDRIES Inc. Malta, New York, USA


Space Application FA and Energy


Robust Test Method of TSOP PEMs for Space Application ....................................................513


Yasunobu Iwai1, Koichi Shinozaki1, Daiki Tanaka2


(1) Japan Aerospace Exploration Agency JAXA, Tsukuba City, Ibaraki, Japan


(2) OKI Engineering CO.,LTD. Nerima-ku,Tokyo,Japan


X-Ray Computed Tomography: A Potentially Destructive “Non-Destructive Evaluation”


Technique ......................................................................................................................519


Ryan Ross, Gil Garteiz, Stephanie Zajac, Jet Propulsion Laboratory, California Institute of Technology, Pasadena, California, United States


Autor Index ....................................................................................................................522


Advanced 3D localization in Lock-In Thermography based on the analysis of


the TRTR (Time-Resolved Thermal Response) received upon arbitrary


waveform stimulation


Sebastian Brand, Michael Kögel, Christian Grosse, Frank Altmann, Fraunhofer IMWS, Halle, Germany


Brian Lai, Qingqing Wang, James Vickers, David Tien, Thermo Fisher Scientific, Fremont, CA, USA


Bernice Zee, Qiu Wen, Advanced Micro Devices Device Analysis Lab, Singapore


Abstract Lock-in thermography (LIT) has been


successfully applied in different excitation and


analysis modes including classical LIT, analysis


of the time-resolved temperature response


(TRTR) upon square wave excitation and TRTR


analysis in combination with arbitrary waveform


stimulation. The results obtained by both


classical square wave- and arbitrary waveform


stimulation showed excellent agreement. Phase


and amplitudes values extracted by classical LIT


analysis and by Fourier analysis of the timeresolved temperature response also coincided, as


expected from the underlying system theory. In


addition to a conceptual test vehicle represented


by a point-shaped thermal source, two


semiconductor packages with actual defects were


studied and the obtained results are presented


herein. The benefit of multi-parametric imaging


for identification of a defect’s lateral position in


the presence of multiple hot spots was also


demonstrated. For axial localization, the phase


shift values have been extracted as a function of


frequency [4]. For comparative validation, LIT


analyses were conducted in both square waveand arbitrary waveform excitation using customdesigned and sample-specific stimulation


signals. In both cases result verification was


performed employing X-ray, scanning electron


microscopy (SEM) and energy dispersive x-ray


(EDX) as complementary techniques.


1. Introduction


In the last decade, trends in microelectronics  pursued the approach of reducing the lateral


space requirements of electronic systems by  using the third spatial dimension for system  integration [1]. As a consequence, adapted  technologies were required for ensuring reliable  electrical interconnections for power supply, data transfer, and communication. These  integration concepts on the other side exhibit  novel defects and failure modes originating in  the interplay of the properties and structures of  the heterogeneous materials integrated into  single systems. In failure analysis, the ultimate  goal is the analysis of the root cause of an  observed defect, requiring the application of  multiple non-destructive and physical inspection  techniques. Non-destructively (ND) operating  techniques have the extraordinary ability of  sensing through optically opaque materials (e.g., of the packaging, metallization layers or  intermediate dies) without the need for sample  preparation. Thus, the introduction of  preparation-related artifacts is mostly avoided. The fact that the sample remains physically  unaltered allows for performing multiple tests at  different conditions and the application of  several non-destructive inspection techniques. As the individual testing methods operate upon  different contrast mechanisms, the detection of  additional defect-accompanying symptoms can  be ensured. As the ND-techniques have a high  value for defect localization to guide subsequent  physical preparation and high-resolution  inspection, the extension of system integration in  the third spatial dimension requires the  adaptation of these techniques accordingly.


Lock-In thermography (LIT) is highly sensitive  towards the detection of resistive defects and  interconnects by spotting emitted thermal signals  of extremely low magnitudes [2]. In previous


# Advanced 3D localization in Lock-In Thermography based on the analysis of the TRTR (Time-Resolved Thermal Response) received upo


ISTFA™ 2019: Conference Proceedings from the 45th


International Symposium for Testing and Failure Analysis  November 10–November 14, 2019, Portland, Oregon, USA


Copyright © 2019 ASM International® All rights reserved. www.asminternational.org


1


studies, it has been observed that the localization  capabilities can be extended from 2D to 3D by  precisely analyzing the propagation-related delay  of the thermal signal [3],[4]. While previous  work was based on classical LIT measurements  at individual single frequencies, the current  paper describes the extension of the  thermographic analysis from single frequencies  to a broad spectral range according to [5] and


[6]. The transient thermal signals at each pixel of  the thermogram are acquired and subjected to a  spectral decomposition for extracting amplitude  and phase images at multiple frequencies from a  single LIT measurement. To further extend the  precision of the method and to reduce the  temporal effort of the inspection task, specifically designed arbitrary waveforms have  been applied for electrical stimulation containing  spectral energy at multiple discrete frequencies


[7]. This approach allowed for increasing the  signal-to-noise ratio (SNR) at the frequencies of  interest while suppressing the intermediate  spectral bands. In the current paper the  applicability and the validity of the inspection  approach and its extension have been evaluated  using a point-shaped thermal source applying  classical LIT and comparing the results to the  ones obtained from analyzing the time-resolved  thermal responses (TRTR) when exciting the  source by square wave and arbitrarily shaped  stimulation signals. Furthermore, two case  studies have been performed applying the  different excitation techniques and spectrally  analyzing the TRTR in an extended spectral  range. Samples investigated were “I”: a  multichip module (MCM) package and “II”: a


2.5D IC high-bandwidth memory device. The  results obtained using the extended method show  excellent agreement with the widely established  classical lock-in thermography.


2. Materials and Methods


Validation of the broadband excitation and  TRTR analysis:


For validation of the applicability of both the  excitation using an extended spectral distribution  in the stimulation signal and the analysis of the  TRTR, fundamental experiments have been  performed. The sample used contained a pointFigure 1: Schematic of the point-shaped thermal source  employed for evaluation and validation of the broadband  excitation and TRTR analysis.


shaped thermal source of 1.5 µm x 1.5 µm  located on monocrystalline silicon. The spot  consisted of a sputter deposited tungsten layer  and exhibited a purely resistive (ohmic) behavior. From both sides the point-shaped  source was electrically connected by a sputter  deposited meander-shaped Au pattern as  illustrated in Figure 1. Classical LIT was  conducted at a series of lock-in frequencies  ranging from 0.25 Hz up to 61.2 Hz. The voltage  and current applied were: 143 mV and 3.9 mA. The measurements were performed for 30 min at  each of the frequencies. For investigating the  applicability of the TRTR analysis, the thermal  source was stimulated equal to the classical LIT  measurements using the built-in source and  measurements unit (SMU) and an arbitrarywaveform generator (AWG) (Keithley 2602B, Tektronix, Beaverton, OR, USA), respectively.


Figure 2: Multi-Sine signal for adapted electrical excitation  in LIT. Top: Signal in time domain. Bottom: Signal in  frequency domain.


2


The standard excitation signals of the SMU had  a square wave shape (“switch On – switch Off”). Using the AWG, two different waveforms have  been designed and experimentally evaluated. These signals were A: a mimicked square wave  equal to the signals generated by the SMU. This  approach allowed comparison of the results  obtained by SMU and AWG. In addition, a  custom-designed signal B: consisting of multiple  superimposed sinusoidal traces was generated by  the AWG and employed for electrically  stimulating the point source. The shape of the  signal in time and frequency domain is shown in  Figure 2. The voltage and current values were set  equal to the classical setup. It can be seen from  the spectrogram at the bottom of Figure 2 that  the custom-designed multi-sine signal contains  energy at discrete frequencies only. Spectral  analysis and extraction of the phase transfer  function (phase shift versus frequency  characteristics) was conducted at these  frequencies.


Case Study I:


In the first case, a MCM package with a  reportedly failed power supply containing a short  that was observed by testing at the automated  test equipment (ATE) has been investigated. The  short was verified when biasing the pin of the  failing power supply with respect to ground by  curve tracing. LIT data acquisition on this  sample was performed in TRTR mode using  square wave and multi-sine excitation. For


150


deriving the z-location of the defect, the phase


-class. LIT singlef-TRTR@7.2 Hz-rect exc.ON/OFF


transfer function of a reference diode was


L美TRTR@ 72HZastarr 5881Hz


recorded in addition. For both types of  excitation, the measurement parameters were


100


kept constant. The square wave excitation was


[。]


performed at a lock-in frequency of 1 Hz.


u!中 Amplitude and phase values of the recorded V TRTR were extracted up to a frequency of


50


25.08 Hz for the defect site and 39.13 Hz for the


reference. Multi-sine excitation was conducted at


a lock-in frequency of 1 Hz with the signal


containing energy at the frequencies 3 Hz, 0


11 Hz, 21 Hz, 31 Hz, and 39 Hz. The applied 020406080100 electrical parameters were -533 mV and -3 mA


for the reference diode as well as 54 mV and


31.7 mA for the defect.


Case Study II:


In the second case study, a 2.5D IC device with  high bandwidth memory suffered a short  between a signal pin and ground, also detected  by ATE. The short was verified when biasing the  defect through the connecting signal pin with  respect to ground for curve tracing. Aiming at  defect localization in all three spatial  dimensions, LIT was applied. In order to  compare the performance and validate the  different operation modes in a manner similar to  case study I, square-wave and multi-sine  excitation were employed in combination with  broad-band TRTR analysis. The phase transfer  function of a reference diode located at the chiplevel of the device was assessed in addition to  data acquisition from the defect site in order to  allow for a more precise axial defect localization. The electrical parameters for stimulating the  reference were 500 mV and 6.9 mA, while for  the defect 76 mV and 34.8 mA were applied. For  square wave excitation the signal was generated  employing the AWG and the lock-in frequency  was set to 1 Hz. Multi-sine excitation was  conducted at 7.2 Hz lock-in frequency with the  signal containing energy at 7.2 Hz, 21.6 Hz, 36 Hz, and 50.4 Hz.


3. Results and Discussion


Figure 3 shows the phase values as a function of  frequency obtained from the point-shaped


f in [Hz]


Figure 3: Phase transfer function of the point-shaped  thermal source obtained by classical LIT and TRTR  analysis. For excitation, a square wave signal in SMU mode  and in arbitrary mode, as well as a multi-sine signal, were  employed.


3


thermal source illustrated in Figure 1. The results  shown were derived from classical LIT  measurements (purple curve), TRTR analysis  using a square wave excitation by SMU (blue  curve), TRTR analysis using a square wave  generated by the AWG (red curve) and a multisine signal containing energy at the frequencies  of 7 Hz, 24 Hz, 40 Hz, 58 Hz, and 81 Hz (green  curve). The repetition rates for the square wave  signals were 7.2 Hz and 1 Hz for the multi-sine  signals. It can be seen from Figure 3 that the  phase transfer functions obtained through  different measurement, analysis and excitation  approaches coincide. This is in agreement with  the theoretically expected behavior, since the  signals obtained from a linear time-invariant  system are the result of convoluting the input  signal with the systems transfer function. In the  classical LIT measurement, the obtained thermal  signature at each lock-in cycle is correlated to a  sine and a cosine function that are in phase with  the electrical excitation signal. The Fourier  transformation performed in the spectral analysis  of the time sequence averaged during the  experiments also performs these correlation  steps; however, since the time-domain data are  available, the analysis is conducted for all


reference position


frequencies that are lower than half of the


(diode)


acquisition frequency of the camera to fulfill the  Nyquist criterion.


Figure 4 shows the results of case study I, addressing the MCM package sample. Plotted  70


60


40


.5


。


30


20


(short)


10


failposition


Figure 4: TRTR analysis of the thermal signals obtained  from a reference diode and an unknown defect (Figure 5).


The phase versus frequency values (phase transfer function) were obtained through excitation by a square wave and a  multi-sine signal in comparison.


are the phase transfer functions of the reference  spot and the defect. The LIT data acquisition was  performed in TRTR mode with square wave and  multi-sine excitation. Square wave experiments  were performed at a lock-in frequency of 1 Hz, and values were extracted for up to the 25th  harmonic for the defect and the 39th harmonic for  the reference. It can be seen that the standard  deviations for both curves increase with  frequency. However, for the defect that is, according to the phase values, deeper below the  surface than the reference, the noise increases  stronger than for the reference, which can be  explained by attenuation effects on the  propagation path of the thermal signal. For  multi-sine excitation, the values of the standard  deviation are substantially lower than for the  square wave excitation. This behavior is likely  explained by the longer relative measurement  time and the discrete spectral distribution of the  signal energy. While in square wave excitation, the sample remains unpowered for half of the


0010203040


Figure 5: Thermograms superimposed with the thresholded  amplitude images, indicating the location of the thermal  source. Top: Thermal signal of a reference diode. Bottom: Thermal signal of an unknown defect (resistive short).


4


A


B


Filament short


Figure 6: 3D X-ray Image of defect at failed position  showing C4 bump filament short.


cycle, excitation is performed throughout the  entire cycle for the multi-sine excitation. As a  consequence, the relative measurement times  required to obtain the same values of the  standard deviation of the phase estimates can be  reduced when stimulating the sample in multisine mode. Figure 5 shows the thermograms of  the MCM package with the thresholded LITamplitude images superimposed. The top-graph  contains the thermogram with the amplitude  image of the reference diode, while in the bottom  image the thermogram with the hot spot of the  defect can be seen. The phase transfer functions  plotted in


Figure 4 were derived at these locations. For all  frequencies the phase values corresponding to  the defect are higher compared to the phase  values extracted from the reference location. Since the phase shift value corresponds to the  propagation time of the thermal signal with


300喜-Fail -square wave@1Hz(B)-REF-multi-sine @7.2Hz


respect to the excitation and normalized to the


-→-Fail -multi-sine@7.2Hz(B)


frequency, it can be concluded from


250.-Fail-multi-sine @7.2 Hz(A)-Fail-square wave@1Hz(A)


Figure 4 that the resistive defect is located deeper


a


200


inside the sample as the thermal signal contains a


S


longer delay to propagate to the sample surface


than the signal originated in the reference diode. 150<In the present case 3D X-ray imaging was


100 conducted and allowed confirmation of the


results concluded from the lock-in thermography


50 inspection. The cause of the shorted electrical


interconnects was found to be a solder filament


0 as shown in the X-ray micrograph in Figure 6.


0102030405060


Figure 7 contains results of the LIT analysis of  the 2.5D IC device investigated in case study II. Two thermograms with the amplitude images of


Figure 7: 2.5D IC device with HBM. Top: Two hot spots  appear when stimulating the resistive defect. Bottom: Hot  spot observed when powering the reference diode at chip  level.


the TRTR analysis at 7.2 Hz superimposed, can  be seen. The parameter map in the upper image  was thresholded and filtered employing a disk  filter to allow for laterally localizing the hot  spots. The location indicated in the red rectangle  corresponds to the defect site of the sample. When inspecting the LIT amplitude image at the  defect site, it is noted that two hot spots labelled “A” and “B” in Figure 7, are present. The hot


The first and still widely used X-ray based technique  is radiography, which aims to produce an image projection of  the internal structures of an object onto a detection screen.  In  radiography, the object is placed in a straight line of sight  between the X-ray source and a detector.  When X-rays are  transmitted through an object, they produce a 2D shadow  image onto the detector, e.g., see Figure 1. With modern 16-bit  detectors, a variety of materials and densities can be  distinguished. Figures 2 and 3 show radiographs of some  electronic components contained in printed circuit boards (PCBs). Different degrees of packages from light-emitting  diodes, hybrids, power devices, multi-layer wire-bonded  packages to ultra-fine pitch devices can be inspected for  package requirements or defective behaviors [8]. Typical  inspections take place on fully populated PCBs to examine the  condition of the package’s voids, concentration area, solder  bridges, pad alignments, etc., and to look for traces of failure  such as wire sweeps, shorts, excess/lack of solder in the joints, cracking, undersize or oversize elements, and missing  components. With high magnification, form and voids in ball  grid arrays (BGAs) can be clearly visualized and quantified  with modern analysis software, e.g., Nikon Inspect-X  software. This software can then measure the percentage of  voiding in a ball or full BGA. By using a pass/fail threshold  condition an analysis of tolerance can be provided. This image  processing technique can be performed directly on a  radiography image without the need for 3D reconstruction  because advanced software algorithms are now capable of  dealing with difficult scenarios, e.g., where solder joints are  partially or fully obstructed by other components on the same  device.


Figure 2. Radiographic images of electronic components  showing bond wires, capacitors, and underlying traces  between them (obtained with a Nikon XTV 160 system at 160  kV, 82 µA, 500 ms exposure, and ~10 µm resolution). Left: a  pad array showing voiding/porosity. Right: a package’s section  showing different components and bond wire traces.


14


Figure 3. Modern software for the analysis of electronic  radiographic images (e.g., Nikon Inspect-X software) can  measure the percentage of voids in a section of a package such  as a quad flat no-leads or a BGA. Pass/fail setting conditions  based on a user-defined threshold can be applied on these  images. Typical resolution of void detection: 0.5 to 10 µm.


Figure 4. X-ray images obtained for the inspection of plated  through holes with partial solder filling (left side) and a plated  through-hole vias feature (on the right). Resolution: 1 to 3 µm.


Classical laminography


With recent developments of image recognition, e.g., by deep machine-learning, some overlapping materials of  obstructed components can certainly be examined by  automatic inspection from 2D radiographs. However, since a  single radiograph cannot discern depth, a more comprehensive  analysis of a device, or overlapping materials, can be  performed with the X-ray technique called ‘laminography’. In  the early 20th century, multiple researchers discovered that by  synchronously moving the radiographic detection system and  the X-ray tube in opposite directions away from the sourceobject-detector line of sight, forming an obtuse angle with the  object on its vertex, they could begin to distinguish the  component of an object in a 3D-like manner with a region in  sharp focus while other specimen planes were blurred out [9, 10, 11]. Figure 4 shows examples of such images obtained for  the inspection of plated through holes and a through hole vias  features using modern inspection software (Nikon Inspect-X). Typical inspections look for fill percentage, void  concentration, cracks, wicking, wetting, etc. In the particular  case of vias, in addition to being filled/unfilled, they may be  buried between layers or staggered/scattered unevenly on one


layer’s side of the PCB. The inspection becomes challenging  as it may only take place at a particular oblique angle, and it  usually takes place at the wafer level, which means very high  throughout put requirements. In such case, changing X-ray  conditions to optimize contrast and brightness in the image are  key factors for increasing the confidence in defect recognition  and failure analysis.


Figure 5.  By taking 2D radiographs at multiple angles, the  depth of features and layers of the board are discernable. The  images in the figure, obtained with a Nikon XTV 160 X-ray  system (max. resolution < 3 µm), show angular radiography or  laminographic visualization of PCB assembly components.


Computed tomography


During the second half of the 20th century, X-ray  computed tomography (CT) came into development.  CT is a  technique wherein a 3D image/model of an object is created  from taking a series of radiographic projections of the object  under rotation [6, 12]. This 3D reconstructed model contains  all internal and external geometry in a voxel-based map, which contains the density distribution or, more precisely, the  distribution of the linear attenuation coefficients inside the  object, and allows the visualization and analysis of internal  structures using clipping views or cross-sectional images with  high spatial resolution [4, 13, 14]. Being able to see inside a  product allows for easy validation of parts, identification of  design issues, investigation of discrepancies, location of flaws  and internal defects, dimensional inspection, and other forms  of quality control that can help with identifying uncertainties  quickly and accurately. As an example, in Figure 6, on the top, a 3D visualization of the CT rendering of an earbud is shown  with different components segmented and highlighted by  different colors; and on the bottom image, a transparent view  of a CT reconstruction of an electronics BGA is shown with  the presence of void pockets highlighted in red. The images in  Figure 7 are full three-dimensional reconstruction of silicon  die, substrate and bond wire connections within a computer  chip.


15


Figure 6. Top: 3D CT segmentation of an earbud (in which  different materials can be segmented and colorized to  highlight different aspects of the sample). Bottom: CT scan of  an electronics chip (in which the different BGA layers and  bond wires are segmented by color; cracks and voids in the  balls are shown). The 3D images here were generated with  VGStudio MAX (Volume Graphics GmbH). The CT data sets  were obtained with a Nikon XTH 225 ST system operated at  180 kV, 30 µA, 0.5 mm Cu filter, ~ 6 µm voxel size, 354 ms  exposure time, and 2880 image projections.


Parts made of plastics, polymers, ceramics, casting  and light metals (e.g., aluminum), and/or composite materials  among others can be measured with the X-ray CT method. This information is useful for the improvement of a part’s  design during product development. Strength, elasticity, resistance, connectivity, and other material properties can  become deteriorated by the presence of multiple defects like  porosity or cracks, which can contribute to degraded  performance and structural failure of manufactured parts. When porosity or other defects are ignored, there is the  potential for product recalls and financial loss. This can be  avoided by accurate defect measurement and precise failure  analysis. X-ray CT can contribute to this area of testing and  failure analysis because it can easily assess the internal  geometries and structural composition of objects in a  nondestructive fashion. Failed parts can be inspected without  breaking them up, thus avoiding the potential alterations  produced by the disassembly process itself.


Figure 7. 3D CT reconstruction of an electronics chip. Left: The traces and connections of bond wires are shown in 3D.  Right: Cross section through a BGA reveals interior voiding. The CT data sets were obtained with a Nikon XTH 225 ST  system (max. resolution < 3 µm) and the 3D images were  generated with VGStudio MAX (Volume Graphics GmbH).


The main advantage of CT is the ability to produce  reconstructions of 3D images and 2D cross-section views that  reveal details of the internal structures of a sample. The virtual  cross-sections can be moved interactively through the  reconstructed 3D volume of the sample, evaluating the internal  characteristics and locating defects in specific areas  determined spatially by a system of 3D coordinates (x, y, z) that can be specified in function of a volume alignment  defined by the user.


In the field of dimensional metrology, CT can obtain  dimensions of internal features normally inaccessible with  coordinate measuring machines (CMMs), and thus parts can  be inspected not only for go/no-go, but also for accuracy of  manufacturing with quantifiable dimensional measurements [6, 15], e.g., see Figure 8, which shows an overview of the  typical CT process from acquisition to extracting dimensional  measurements. In particular, tolerances can be contrasted with  different processes using nondestructive measurement of the  manufactured product. There is considerable benefit in  measuring the products in the assembled state, not only for  comparison of results but also for tracking dimensional  changes after assembly or when modifications are deliberately  applied to a single process or to a particular component. Dimensional measurements with CT allow for size and form  determination, wall thickness analysis, and part-to-model or  part-to-part comparison against a standard. This permits the  detection of dimensional deviations and identification of  differences or accuracy issues.


In addition, CT enables reverse engineering by  converting the 3D reconstructed model of a part to an  stereolithography (STL) model, which can be used for rapid  prototyping, 3D printing (i.e., additive manufacturing), and  computer-aided manufacturing. However, the accuracy of the  reconstructed surfaces is limited by the resolving power on the  grey scale range of voxels in the CT volume data, i.e., by the  spatial resolution, which is dependent upon physical  parameters of the CT system such as the finite diameter of the  X-ray source, X-rays’ collimation, beam projection geometry, precision of the translational and rotational movement  controllers, detector spacing, etc. [4, 13, 16, 17].


16


Figure 8. Workflow chart depicting the process of X-ray CT  with the inclusion of dimensional metrology evaluation. The  test sample shown in the diagram corresponds to the prototype  of a NIST ‘Frustum artifact’ containing internal structures  inaccessible to tactile or vision-based inspection [12, 13].


Computed laminography


The major limitation of classical laminography is the  fact that each measurement needs to locate a focal plane or  region of interest to be imaged sharply; other planes or regions  must be inspected consecutively by displacing the object—or  equivalently, by a correlated motion of the X-ray source and  the detector—to different locations. The interest in this  technique—also referred to as “motion tomography” or “tomosynthesis” [18, 19]—was renewed in the late 1990s with  the advent of new developments in electronics (and modern  computers) and further improvements on X-ray flat-panel  detectors [20]. Computed laminography is equivalent to CT  with a limited aperture, e.g., see Figure 9; the measurement  setup is equivalent to that of a CT scan but with a sample  rotation axis tilted by less than 90 degrees with respect to the  incident X-ray beam. This angle can be anywhere between 30  and 60 degrees. Computed laminography is a current  inspection tool used for objects with geometries that make the  use of CT impractical, e.g., for relatively planar objects with  large lateral dimensions or large aspect ratios such as PCBs, or  ZARotationDetector


extended objects with high absorption of X-rays along


axis


longitudinal directions [132, 133, 134]. Computed


Scanning


laminography yields images of an examined object layer by


&


layer with a higher sensitivity to crack-like flaws as compared


X-ray image


X-ray


to radiography. This is caused by the reconstruction of the


acquisition


source


image from different projections measured from different  angles. Moreover, this reduces the noise of the image because  of the averaging effect.


Reconstruction from 2D images to 3D volume


75°


Local adaptive thresholding<一→29396


51388 BackgroundMatesial


Surface


40352


determination


Iso-urface


****


Geometry fitting


&Dimensional


180°


measurements


-0R


Figure 9. Setup for computed laminography measurement in a  Nikon XTV 160 X-ray system. By angling the detector away  from the sample and rotating the sample (or the source and  detector relative to the observation point) while taking  multiple radiographs, it is possible to build a 3D model. Unlike CT, which requires the sample axis of rotation to be  perpendicular to X-rays, laminography allows for such angle  to be variable as shown on the image above.


Practical Considerations


Parts of varying size and complexity can be  measured. By changing the position of the specimen with  respect to the source-detector distance, different  magnifications can be achieved and the resolution of the scans


17


can be modified. A high resolution close-up view of a specific  region of interest can be obtained. Accurate measurements can  be performed using high resolution scans, and faster  acquisitions can be achieved with lower magnifications. If  time is a constraint, a loss of image quality can be tolerated as  a trade-off for a reduction in scan time. A reduction in  measurement time of several minutes may lead to a reduction  in measurement accuracy of only a few micrometers. Reduction of scanning time down to a few seconds is possible  depending on the application. Automatization is also possible  to allow for the use of 2D and 3D X-ray systems on  production floors. Ultimately, the quality of the data depends  on the sharpness of the X-ray images and the signal-to-noise  ratio, which is dependent upon the quality of the X-ray source, the detector, and the precision and stability of the  manipulating system.


Figure 10. Cross-sectional view and 3D image of a PCB  assembly which was obtained by computed laminography. The  CT data sets were obtained with a Nikon XTV 160 system  operated at 150 kV, 63 µA, ~ 9 µm voxel size, 354 ms  exposure time, 177 ms exposure, 1440 projections.


As a note of caution, induced by radiation effects, an  alteration of the electrical properties may occur in some solidstate devices and integrated circuits that, depending on the  absorbed dose, could produce some amount of damage [21, 22, 23, 24, 25, 26]. X-ray induced electronic damage is  initiated primarily by photo-absorption. However, most X-ray  inspections for high-quality imaging require radiation dose  amounts that are considered inconsequential for device failure  or non-functionality. Since radiation-induced effects on the  electrical characteristics of some materials have been reported [27, 28, 29], it is important to understand and consider the  latent damage or potential radiation degradation that may  occur in some materials and components to avoid operative  damage of electronic devices during X-ray inspection. The  degree of radiation-induced effects has been found to depend  strongly on the process technology. Semiconductor devices are  particularly susceptible to ionizing radiation effects due to  intrinsic features of their design [30, 31, 32]. X-ray radiation  induced damage on long-term reliability of momentary  electronic switches has been reported in some investigations [33, 34]. In some cases, radiation damage plays a major role in  device degradation, and it becomes more important as the  device size reduces.


Conclusions


With new developments in software, 2D and 3D Xray techniques for testing and failure analysis allow for the  extraction of internal features in a nondestructive fashion with  resolutions in the range of 1 µm or less. Current 3D X-ray  technologies have the ability to generate geometric data for a  complete characterization of material structures (including  external features) and detect manufacturing defects and  dimensional deviations from intended design. To study  complex structures produced by a manufacturing process, with  the current NDT technologies, CT might be the only available  technology that can accurately—i.e., with small uncertainty (< 10µm)—determine dimensions of inner or hidden structures in  an assembled product. With a destructive method, the  dimensions extracted from the disassembled state of a product  may differ from the actual geometrical dimensions in the  original assembled state. This is particularly relevant for parts  built with a variety of manufacturing processes including  additive manufacturing. In addition, X-ray technologies can be  used as a quality control tool from optimization to production  or to identify or prevent failures quickly (inspection time can  vary from a few seconds to tens of minutes), which saves both  money and time.


References


[1]  H. Villarraga-Gómez, "The evolution of electric light  bulbs," Optics & Photonics News, p. 27, December 2015.


[2]  W. C. Röntgen, "On a new kind of rays," Nature, vol. 53, no. 1369, pp. 274-276, 1896.


[3]  O. Glasser, Wilhelm Conrad Röntgen and the Early  History of the Roentgen Rays, San Francisco (USA): Norman Publishing, 1993.


[4]  H. Villarraga-Gómez, E. L. Herazo and S. T. Smith, "Xray computed tomography: from medical imaging to  dimensional metrology," Precision Engineering, vol. 60, p. To be published, 2019.


[5]  L. De Chiffre, S. Carmignato, J. P. Kruth, R. Schmitt and  A. Weckenmann, "Industrial applications of computed  tomography," CIRP Annals - Manufacturing Technology, vol. 63, no. 2, pp. 655-677, 2014.


[6]  H. Villarraga-Gómez, "Seeing is believing: X-ray  computed tomography for quality control," Quality  Magazine, vol. 55, no. 6, pp. 20-23, 2016.


[7]  Global Industry Analysts, Inc, "Industrial X-Ray  Inspection Systems - Market Analysis, Trends, and  Forecasts," USA, 2019.


[8]  Z. Fu, D. Goyal, J. Thomas, A. Crawley and A. Ramsey, "3D X-ray computed tomography (CT) for electronic  packages," in Proc. of the 29th International Symposium  for Testing and Failure Analysis, Santa Clara, CA (USA),


2003.


[9]  R. Van Tiggelen, "In search for the third dimension: from  radiostereoscopy to three-dimensional imaging," JBRBTR, vol. 85, pp. 266-270, 2002.


18


[10]  T. D. Moore, D. Vanderstraeten and P. Forssell, "Determination of BGA structural defects and solder joint  defects by 3D X-ray laminography," in 8th International  Symposium on the Physical and Failure Analysis of  Integrated Circuits, IEEE, Singapore (Singapore), pp. 146-150, 2001.


[11]  A. Thompson and R. Leach, "Introduction to Industrial  X-ray Computed Tomography," in Industrial X-ray  Computed Tomography, edited by Carmignato S, Dewulf  W, and Leach R; Cham (Switzerland)), Springer, 2018, pp. 1-23.


[12]  H. Villarraga-Gómez, C. Lee and S. T. Smith, "Dimensional metrology with X-ray CT: a comparison  with CMM measurements on internal features and  compliant structures," Precision Engineering, vol. 51, pp. 291-307, 2018.


[13]  H. Villarraga-Gómez, PhD Dissertation: Studies of  Dimensional Metrology with X-ray CAT Scan, Department of Physics and Optical Science: The  University of North Carolina at Charlotte, 2018.


[14]  J. D. Thousand and S. T. Smith, "A direct silicon bonded  reference object for performance assessment of computed  tomography systems," Precision Engineering, vol. 58, pp. 16-24, 2019.


[15]  H. Villarraga-Gómez, "X-ray computed tomography for  dimensional measurements," in Proc. of Digital Imaging  2016 - An ASNT Topical Conference, Mashantucket, CT (USA), pp. 44-57, 2016.


[16]  J. Hiller and P. Hornberger, "Measurement accuracy in Xray computed tomography metrology: Toward a  systematic analysis of interference effects in tomographic  imaging," Precision Engineering, vol. 45, pp. 18-32,


2016.


[17]  J. Hiller, M. Maisl and L. M. Reindl, "Physical  characterization and performance evaluation of an x-ray  micro-computed tomography system for dimensional  metrology applications," Measurement Science and  Technology, vol. 23, no. 8, p. 085404 (18pp), 2012.


[18]  H. H. Barrett and W. Swindell, "Analog reconstruction  methods for transaxial tomography," Proceedings of the  IEEE, vol. 65, no. 1, pp. 89-107, 1977.


[19]  D. G. Grant, "Tomosynthesis: a three-dimensional  radiographic imaging technique," IEEE Transactions on  Biomedical Engineering, Vols. BME-19, no. 1, pp. 20-28,


1972.


[20]  J. T. Dobbins III, "Tomosynthesis imaging: at a  translational crossroads," Medical physics, vol. 36, no. 6, pp. 1956-1967, 2009.


[21]  A. Ditali, M. Ma and M. Johnston, "X-Ray InspectionInduced Latent Damage in DRAM," in 2006 IEEE  International Reliability Physics Symposium  Proceedings, San Jose, CA (USA), 2006.


[22]  M. J. Gadlage, M. J. Kay, J. D. Ingalls, A. R. Duncan and  S. A. Ashley, "Impact of X-Ray Exposure on a TripleLevel-Cell NAND Flash," IEEE Transactions on Nuclear  Science, vol. 60, no. 6, pp. 4533-4539, 2013.


19


[23]  S. Gerardin, M. Bagatin, A. Paccagnella, A. Visconti, S. Beltrami, M. Bertuccio and L. T. Czeppel, "A study on  the short- and long-term effects of X-ray exposure on  NAND Flash memories," in 2011 International  Reliability Physics Symposium, Monterey, CA (USA),


2011.


[24]  J. R. Srour, D. M. Long, D. G. Millward, R. L. Fitzwilson  and W. L. Chadsey, Radiation effects on and dose  enhancement of electronic materials, Park Ridge, NJ (USA): Noyes Publications, 1984.


[25]  D. Ehrt and W. Vogel, "Radiation effects in glasses," Nuclear Instruments and Methods in Physics Research  Section B: Beam Interactions with Materials and Atoms, vol. 65, no. 1–4, pp. IN1, 1-8, 1992.


[26]  E. W. J. Mitchell, "The effect of radiation damage on the  electronic properties of solids," British Journal of Applied  Physics, vol. 8, no. 5, p. 179, 1957.


[27]  J. S. Bi, Z. S. Han, E. X. Zhang, M. W. McCurdy, R. A. Reed, R. D. Schrimpf, D. M. Fleetwood, M. L. Alles, R. A. Weller, D. Linten, M. Jurczak and A. Fantini, "The  Impact of X-Ray and Proton Irradiation on HfO2/HfBased Bipolar Resistive Memories," IEEE Transactions  on Nuclear Science , vol. 60, no. 6, pp. 4540-4546, 2013.


[28]  M. J. Marinella, S. M. Dalton, P. R. Mickel, P. E. Dodd  Dodd, M. R. Shaneyfelt, E. Bielejec, G. Vizkelethy and P. G. Kotula, "Initial Assessment of the Effects of Radiation  on the Electrical Characteristics of TaOx Memristive  Memories," IEEE Transactions on Nuclear Science, vol. 59, no. 6, pp. 2987-2994, 2012.


[29]  P. Cheng, B. Jun, A. Sutton, A. Appaswamy, C. Zhu, J. D. Cressler, R. D. Schrimpf and D. M. Fleetwood, "Understanding Radiation- and Hot Carrier-Induced  Damage Processes in SiGe HBTs Using Mixed-Mode  Electrical Stress," IEEE Transactions on Nuclear  Science, vol. 54, no. 6, pp. 1938-1945, 2007.


[30]  J. P. Duraud and F. Jollet, "Radiation effects in SiO2  under electronic excitation," Nuclear Instruments and  Methods in Physics Research Section B: Beam  Interactions with Materials and Atoms, vol. 32, no. 1–4, pp. 248-257, 1988.


[31]  D. Braäunig and F. Wulf, "Atomic displacement and total  ionizing dose damage in semiconductors," Radiation  Physics and Chemistry, vol. 43, no. 1–2, pp. 105-127,


1994.


[32]  A. M. Chugg, "Ionising radiation effects: a vital issue for  semiconductor electronics," Engineering Science and  Education Journal, vol. 3, no. 3, pp. 123-130, 1994.


[33]  S. Kim, H. Lee, C. Han, K. Lee, S. Choi, Y. Jeon, E. D. Fabrizio and M. Gentili, "The effects of X-ray irradiationinduced damage on reliability in MOS structures," SolidState Electronics, vol. 38, no. 1, pp. 95-99, 1995.


[34]  A. Balasinski and T. P. Ma, "Ionizing radiation damage  near CMOS transistor channel edges," IEEE Transactions  on Nuclear Science, vol. 39, no. 6, pp. 1998-2003, 1992.


Localization of dielectric breakdown sites in 3D through-silicon via (TSV) interconnects by laser stimulation and chip deprocessing


1 Imec, Kapeldreef 75, B-3001 Leuven, Belgium


2 KU Leuven, Dept. Materials Engineering, B-3001 Leuven, Belgium  E-mail: Kristof.J.P.Jacobs@imec.be


Abstract


We report and demonstrate a new methodology for the  localization of dielectric breakdown sites in through-silicon via (TSV) structures. We apply a combination of optical beam  induced


resistance


change


(OBIRCH)


and  mechanical/chemical chip deprocessing techniques to localize  nm-sized pinhole breakdown sites in a high aspect ratio 3x50 µm TSV array. Thanks to the wavelength-selective absorption  process in silicon, we can extract valuable defect depth  localization info from our laser stimulation measurement. After  chip deprocessing we inspect and localize the defect site in the  dielectric liner using a scanning electron microscope (SEM). We confirm our results and analysis by cross-sectioning a TSV  with a focused-ion beam (FIB).


Introduction


The evolvement of electronic systems in terms of performance, energy efficiency, and cost has been enabled by the continuous  advancement of semiconductor integration technology. Due to  the recent breakthrough of 3D chip technology, it is anticipated  that the chips of the future will prolifically implement this  technology, thereby offering new possibilities and


+V


opportunities for system technology co-optimization [1].


Cu


MIIMD


T


Nevertheless, challenges are still to be overcome in terms of


PMD


stacking, scaling, and performance, as well as testing and


STI OX


analysis techniques for defect localization [2].


The vertical interconnections in advanced 3D


Dielectric


integration technology are nowadays being made by throughbreakdown


silicon vias (TSVs). A TSV is a metallic pillar (e.g. copper) fabricated through the Si substrate and insulated by a thin  dielectric layer (e.g. SiO2) for electrical isolation. The dielectric  strength properties and uniformity of this layer are of critical  importance to ensure reliable interconnect performance [3].


Weakness in


Electrical shorts and/or leakage currents may occur through


dielectric liner


dielectric breakdown when the deposition conditions of the


p-Si


dielectric layer are not well controlled, and/or when the device  is subjected to an electrical overstress (EOS) or electrostatic  discharge (ESD) condition. From a failure analysis (FA) and


吉GND


process optimization perspective, it is important to have the  capability to localize these defects with a high accuracy and  success rate.


In this paper, we report a new FA methodology to  localize dielectric breakdown sites in a TSV by a combination  of laser stimulation based on optical beam induced resistance  change (OBIRCH) and chip deprocessing techniques. The  methodology has been developed on a 3X50 um via-middle  TSV array structure used primarily to study the time-dependent  dielectric breakdown (TDDB) physics in this interconnect


technology [4]. However, the methodology may also find  application on more complex IC structures. Figure 1  schematically shows a cross-sectioned schematic of a TSV  array structure. A zoomed in view of the TSV indicates a region  with a liner thickness anomaly. Given that the dielectric  breakdown strength scales proportionally with dielectric  thickness, the failure is expected to occur at the location with  the strongest electric field (i.e. thinnest dielectric). The  localization of these breakdown sites is challenging due to the  multitude of different materials and their properties that are  involved and the 3D nature of the structure.  To localize these  defects, we report a methodology based on a non-destructive  laser stimulation measurement followed by mechanical and  chemical deprocessing and SEM inspection. This work is  considered complementary to the recently developed  methodology by Altmann et al. whereby backside LIT and  photoemission microscopy (PEM) techniques were applied for  breakdown localization in a similar structure [5]. Whereas  techniques reported by Altmann et al. rely on the principle of  detecting near-infrared (PEM) and mid-infrared (LIT) emission  induced by the defect, our approach may offer solution in those  cases when defects do not generate detectable light (such as an  ohmic defect) or enough heat.


Fig.1. Cross-section schematic of a Cu-filled TSV array. The  zoomed in-view illustrates the principle of dielectric  breakdown (i.e. short-circuit condition between TSV and  substrate) at the weakest location (i.e. thinnest part) of the  TSV liner (in black) upon application of a high electric field  between the TSV and substrate.


# Localization of dielectric breakdown sites in 3D through-silicon via (TSV) interconnects by laser stimulation and chip deprocess


TSV leakage failure by electrical breakdown


The structure under investigation (shown in figure 3) consists of an array of seven 3x50 µm Cu-filled TSVs (3 µm  diameter, 50 µm height) that are connected electrically in  parallel. The TSVs are fabricated on a full thickness Si wafer  with a high conformal atomic layer deposition (ALD) oxide  liner deposition process targeting a nominal liner thickness of  100 nm. TSV metallization consists of a thermally grown ALD  WN barrier, an electroless NiB seed layer, and an electroplated  copper plug. The TSVs are interconnected electrically to a  common probing pad with Al metallization segments on the  chip front-side. The substrate connection is made similarly by  connecting a probing pad to a highly p-doped Si ring  surrounding the TSVs. Further details about the fabrication  process technology is reported elsewhere [6].


Dielectric breakdown was introduced in the TSV array  by applying an electrical overstress condition in a controlled  manner using a Keysight 2450 source measure unit (SMU). Figure 2 shows the measured current-voltage (I-V) characteristic for the array whereby the voltage was ramped up  from zero to breakdown. The TSVs were stressed with the  positive terminal applied to the copper plug and the ground  terminal connected to the substrate (i.e. copper driven mode


[7]). A 1 GΩ current limiting series resistor was connected in  series with the TSV structure to avoid catastrophic failure at  breakdown (Imax = 100 nA @ 100 V). Catastrophic failure  must be avoided as the current compliance circuitry of the SMU  has a finite response time and the breakdown current may  briefly exceed the target compliance of 10 nA.


Fig.2. I-V characteristics of the TSV array structure  measured before and (inset) after electrical breakdown.


A measured leakage current of less than 10 pA (R ~ 100 GΩ) at low bias (typical operating condition) is indicative  of a high-quality oxide liner. However, when the voltage is  increased beyond +58V, a strong rise in current is observed  leading to current shoot-through at +67V. We note that the  intrinsic breakdown voltage of the TSV is slightly less (<1V  expected) as the 1 GΩ series resistor is forming a voltage  divider during the measurement. The inset of Fig. 2 shows the


I-V measured after electrical breakdown (without the current  limiting resistor in circuit but with the current compliance of the  SMU set to 10 nA) for a measured bias range from -1V to +1V. The measured resistance of 83 MΩ at a bias of 0.25V clearly  indicates that TSV structure has failed as the static leakage  current has drastically increased by several orders of magnitude (from pA to nA). The defect shows a quasi-ohmic characteristic  behavior.


Breakdown localization by laser stimulation


Optical-beam induced resistance change (OBIRCH) has  become an important FA technique in the semiconductor  industry. The technique relies on the use of a focused laser beam  to locally heat the device under test and induce a change in the  electrical resistivity (and measure with a meter), which is  usually constant unless when a failure is present [8]. In this  work we have investigated the applicability of this technique  for localizing breakdown sites in TSV structures.


Figure 3 illustrates the adopted measurement principle  and configuration. A focused laser beam is scanned in raster  format over the surface of the structure while the interaction  effect of the beam on the TSV is detected electrically using a  resistance meter. The electrical resistance (i.e. leakage current) is measured between the TSV array and the substrate. The  resistance measurement was performed in constant current  mode whereby a current of 100 pA (i.e. low current to minimize  parasitic joule heating) is applied to the structure while the  induced voltage across the structure is measured. The  measurement was performed using the same Keithley 2450  SMU. Probes were used for electrically contacting the structure.


101.0x10-8


10-90.05.0x10-9


laser beam


Current (A)10110-10.1.0x10.-1.5-1.0-0.5 0.0 0.51.0 10-12


R (Ω)


-5.0x10-9-


10-13


-100


B0090850 μm


10 2030 40 50 60 70 Voltage (V)


Fig.3. Optical microscope image of the TSV structure under  test and measurement configuration. The scanned area (purple square) covers the seven TSVs that are configured  in an inverted U-shape.


Figure 4(a) shows the measured OBIRCH map for a scanned  region of ~60 µm by ~70 µm in size. The measured data (in  color) is superimposed on the laser reflection data shown in  grey scale mode on the same map. The laser reflection data was  collected by measuring the reflected light from the structure  with a photodiode.  The measurement was carried out with laser


21


operating in continuous wave mode at 405 nm with an optical  power output of ~0.5 mW.


Figure 8: Phase transfer functions of the reference diode  and the defect estimated by TRTR using square wave  excitation at 1 Hz and multi-sine excitation @ 7.2 Hz.


5


hot spot corresponding to an I/O-diode at the  chip level. Figure 8 contains the phase transfer  functions of the different hot spots shown in  Figure 7. For both excitation modes, square  wave and multi-sine, the phase shift values of the  hot spot labelled “A” in Figure 7 are larger than  the values of hot spot “B” at all frequencies. Since spot “A” is not located above an active IC  structure it is concluded that the defect is located  underneath hot spot “B”. Furthermore, hot spot “A” is assumed to be an artefact resulting from a  large depth of the defect which allows for a  partial transmission of the thermal signal through  the molding compound, bypassing the direct  path. Caused by the higher emissivity of the  molding compound, the artefact-related hot spot  shows a higher amplitude of the power. The  larger phase shift values of spot “A” compared  to “B” support the hypothesis that the defect is  located underneath “B”. Employing a method of  combined multi-parametric imaging using the  phase values recorded at one frequency and  combining them with the amplitude values  obtained at a different frequency allowed clear  differentiation of the two hot spots. Figure 9  contains a scatterplot of the power amplitudes  extracted from the TRTR at 21.6 Hz and the  phase shift values obtained at 50.4 Hz. Combining the two parameters in a scatterplot


Figure 9: Multi-parametric imaging. Left: Scatterplot of the  power at 21.6 Hz (abscissa) and the phase shift @ 50.4 Hz (ordinate). The values from the colored rectangles in A are  superimposed onto the thermogram and plotted in B-D.


Figure 10: Schematic illustration of the cross section of the


2.5D IC sample. The reference diode is located underneath  the Si die. The larger phase shift values of hot spot "B" in  Figure 7 identify its axial location to be at C4-level. LIT  inspection was performed downward facing through the  ASIC die.


allows for extraction of specific parameter  combinations. In the graph “A” of Figure 9, a  bifurcation can be seen, allowing a phase  selective identification of amplitude values. The  parameter combination of the three regions in the  scatterplot are superimposed onto the thermal  amplitude image in B to D of Figure 9.


For axial localization of the defect, the phase  shift values must be analyzed with respect to  frequency. From Figure 8, it is noted that the  phase values obtained from the reference  location are substantially smaller than the ones at  hot spot “B”, which, according to the above  elaboration belongs to the defect. It can therefore  be concluded that the defect is located deeper  inside the sample, and located as shown in  Figure 10. For verification, complementary 3DFigure 11: 3D X-ray image recorded at the defect location  according to hot spot “B”. A suspicious solder extrusion  between the C4 bumps “ground” and “signal pin” can be  seen.


6


Figure 12: FIB cross section and EDX at the thermal  emission site corresponding to hot spot “B” in Figure 7.


spot labelled “A” however is located outside the  chip without any active structure underneath. The bottom graph in Figure 7 contains the  amplitude map obtained through LIT-TRTR  analysis of the reference location showing the  Xray microscopy was performed at the location  of hot spot “B”, which revealed the presence of  solder-like material that appeared to be shorting  the failing signal pin to ground as seen in Figure


11. After non-destructively detecting and  localizing the defect, precise sample preparation  and high-resolution imaging and elemental  analysis was performed. Employing focused ion  beam (FIB) technique, a cross section through  the defect site was prepared. Figure 12 contains  an electron micrograph of this cross section in  the upper image. At the interface between the  underfill and passivation, indication of the solder  extrusion can be seen. To further investigate the  root cause, EDX was conducted which verified  the presence of solder bridging the two bumps. The short is expected to result from solder  material entering a delamination between the  passivation and the underfill.


4. Conclusions


Lock-in thermography using classical and  broadband excitation has been performed for  evaluation and validation of the TRTR-based  inspection and analysis approach. The phase


transfer functions of a point-shaped thermal  source were derived and compared between the  different stimulation modes. The results show  excellent agreement as expected from the  theoretical considerations. However, during the  development phase of the measurement  equipment it was observed that a careful and  precise synchronization between excitation and  acquisition is of major importance. The case  studies presented in this paper investigated two  different samples. Case study I addressed an  MCM package. For 3D localization the phase  transfer function of a reference diode and an  observed defect-related hotspot were extracted  and analyzed. A depth assignment based on the  TRTR analysis using a multi-sine broad-band  excitation signal was possible. The second case  study investigated a 2.5D IC device with highbandwidth memory. In this sample, two hot spots  were observed near the edge of the die. Employing a multi-parametric imaging approach  allowed for identification and localization of the  defect site by assigning it to one of the observed  hot spots. For axial localization a reference diode  at the die-level was analyzed by LIT. Due to the  substantially lower phase values of the reference, the axial location of the defect was identified to  be at the C4 level of the sample. Result  verification was obtained through physical  failure analysis and high-resolution imaging by  SEM in combination with EDX. The major  finding of the paper is the verification of the  validity of the TRTR-based LIT analysis in  combination with arbitrarily shaped electrical  stimulation that allows for optimizing either the  measurement time or the precision of LITmeasurements with respect to phase shift  assessment for 3D localization.


© 2019 Advanced Micro Devices, Inc. All rights  reserved. AMD, the AMD Arrow logo, and  combinations thereof are trademarks of  Advanced Micro Devices, Inc. Other product  names used in this publication are for  identification purposes only and may be  trademarks of their respective companies.


[1] K. Croes et al., "Reliability Challenges  Related to TSV Integration and 3-D


7


Stacking," in IEEE Design & Test, vol. 33, no. 3, pp. 37-45, 2016.


[2] O. Breitenstein: “Lock-in Thermography – Basic Use for Evaluating Electronic  Devices and Materials, 255 pages, Springer, 2010


[3] R. Schlangen et al: “Use of Lock-In  Thermography for Non-Destructive 3D  Defect Localization on System in Package  and


Stacked-Die


Technology”,


proceedings of ISTFA 2011, pp. 68-73


[4] C. Schmidt, F. Altmann: “Quantitative  Phase Shift Analysis for 3D Defect


Localization


Using


Lock-in


Thermography”, proceedings of ISTFA


2011, p 74-80


[5] F. Naumann et. al., Efficient nondestructive 3D Defect Localization by  Lock-in-Thermography utilizing Multi  Harmonics analysis, Proc. of the 40th  International Symposium for Testing and  Failure Analysis (ISTFA), 2014, pp 130-135


[6] S. Brand et al.: “Time-resolved lock-in  thermography for defect localization in  3D” Proc. 3rd CAM Workshop, Halle, Germany, 2018


[7] S. Brand et al.: “Arbitrary Waveform  Stimulation and TRTR Analysis for  Advanced 3D LIT Inspection” Proc. 4th  CAM Workshop, Halle, Germany, 2019


8


Non-Destructive Short Fault Localization in Advanced IC Packages Using Electro  Optical Terahertz Pulse Reflectometry


B. Zee, W. Qiu


Device Analysis Laboratory, Advanced Micro Devices


J. Alton, T. White, M. Igarashi, D. Sullivan


TeraView Limited, 1 Enterprise, Cambridge Research Park, Cambridge, CB25 9PD, United Kingdom


We demonstrate how electro optical terahertz pulse  reflectometry (EOTPR) can be used in conjunction with a new  one-dimensional lump circuit simulation software to quickly  and non-destructively isolate faults in advanced IC packages. In  the case studies presented, short failures are accurately located  in a series of advanced IC package.


High accuracy, rapid localization of short failures in advanced  IC packages is an increasingly challenging issue due to the  decreasing feature dimensions present in state-of-the-art  packages and their corresponding increased complexity. In  recent years, EOTPR has become an essential tool in fault  analysis labs in the semiconductor industry [1-11], due to its  ability to non-destructively detect and localize faults in a wide  range of device architectures [11], its rapid measurement time (<5 minutes), and its fault localization accuracy of better than  10 µm. However, the localization of short faults in measured  EOTPR waveforms can be challenging, due to the signal being  a sum of the short current path and the good current path. Here, we demonstrate how a newly released analysis application, EOTPR QuickSim, can overcome these challenges and enable  short fault localization with high accuracy.


Figure 1: Schematic diagram of an EOTPR system


During EOTPR operation, electrical pulses are launched into  the device under test (DUT) via a high frequency circuit probe (figure 1), which is contacted to the DUT using a manual or  semi-manual probing station. Reflections from device  structures and faults are recorded as a voltage-time waveform  by a fast-photoconductive switch.


QuickSim utilizes a one-dimensional lump circuit model to  rapidly and efficiently simulate a measured EOTPR waveform. The waveforms are simulated as reflected impulses from a onedimensional lumped-element equivalent circuit. The  application allows equivalent circuits to be defined as  sequences of elements that may include RLC impedances (both  serial and parallel) and transmission lines with radiative  transmission losses. A faulty circuit is modelled by the addition  of extra impedance elements, that may be located part-way  along a transmission line that would be intact in the equivalent “good” circuit. QuickSim provides a global optimization  function, based on the Monte Carlo method [12], that finds the  circuit parameters that best match an experimental EOTPR  waveform. It is then straightforward to interpret the optimized  circuit model to predict the location of a fault.


An example QuickSim model is described below. The model is  of the flip chip bare substrate trace detailed in case study 2 of  this paper. The trace of interest is represented in the model by 4  circuit elements:


1. Resonant probe: This element represents the circuit


Transceiver module


probe / LGA contact interaction and is defined by a


optical fibers


resistance, frequency, and quality factor.


区


2. Transmission line 1: This element represents the bottom trace in the bare substrate and is defined by an


区区


impedance, length, dielectric constant, and loss.


photoconductivealements


3. Transmission line 2: This element represents the


BSoptical delay卤


plated through hole (PTH) and is defined by an


*-semi-rigid co-ax


4. Transmission line 3: This element represents the top


780nm


110GHz probe


modelocked


trace in the bare substrate and terminates in a dead


laser


open at the c4 bump pad and is defined by an


..0000 000000 EOTPR Core system000000


impedance, length, dielectric constant, and loss


DUT


The inputs to the model are the actual lengths of the bottom and  top traces, height of the PTH, and measured EOTPR waveform. All other model parameters are optimized by the software (within predefined limits) to obtain the best fit to the measured  EOTPR waveform. The whole process of designing and  optimizing the circuit model to the waveform typically takes


# Non-Destructive Short Fault Localization in Advanced IC Packages Using Electro Optical Terahertz Pulse Reflectometry


9


less than 30 minutes. The model can then be saved for later use.


Measured - Substrate


Once an acceptable solution for the model is obtained, faults


--· Model - Substrate


can be rapidly positioned anywhere within the model to show


- Measured - Die removed


the expected EOTPR waveform for a failure at that location.


750


-- Measured - Good--· Model -Dle removed


Alternatively, a measured failed unit waveform can be


--·Model - Good


imported, and the software used to find the fault location by


-- Measured - Fail--· Model - Fail


varying only the faults location and resistance in the model and


500


finding the best fit to the measured waveform. When importing  a failed waveform into an already-optimized model, the entire  fault localization process typically takes less than 5 minutes.


Siqnal unkeEOTPR fork


Results and Discussion


Case Study 1:


Figure 2 depicts the advanced IC package used in case study 1.


-250


It comprised a die attached on a reconstituted substrate of  copper redistribution lines in polyimide. A signal pin was found


210 optecl Deary


505600


to exhibit a short failure after electrical test.


Figure 2: Schematic of the advanced IC package used in this  study.


Figure 3 shows the waveforms acquired for the bare substrate (black solid waveform, offset for clarity), a known good device (green solid waveform), a known good device with the die  removed (blue solid waveform) and the failed device. Comparing the good and failed devices, the short feature can be  observed as the broad negative feature at around 250 ps.


To identify the location of the fault, a QuickSim model was


Top View


constructed for each reference device; the corresponding  simulated waveforms are shown by the dashed lines in Figure


3. Each model consists of a series of transmission line circuit  elements used to represent the key DUT features. For example,


Ground pin


the bare substrate model consists of three transmission line


Anoma'observed


elements, representing the bottom trace, through via, and top  trace. The actual trace and via lengths are input into the model  to define the lengths of the transmission line elements and the  impedance, loss, and dielectric constant are used as fitting


Signal pin


parameters in the QuickSim software to obtain the best fit to the  measured EOTPR waveforms. The simulation results fit closely  with the measured waveforms in each case (Figure 3).


The location of the short fault was determined by adding a short  fault to one of the transmission line circuit elements, and then  repeating the simulation whilst sweeping only the faults  location and resistance. In this manner, the best fit was found  with the short failure position at the very end of the trace in the  advanced IC package (Figure 3, solid and dashed lines).


Figure 3: EOTPR results from the advanced IC package. The  solid lines show the measured EOTPR waveforms and the


MC


Die


dashed lines show the simulation results. The EOTPR waveform


0000000000


from the failed unit (solid red line) clearly shows a short failure


Reconstituted substrate


indicated by the negative feature at around 250 ps in the  waveform.


This is in good agreement with non-destructive X-ray imaging  performed at the identified failure location, which showed an  anomaly at the signal and ground pins, as seen in Figure 4. Subsequently physical failure analysis performed using focused  ion beam (FIB) X-section confirmed that the cause of the short  was solder extrusion into a delamination at the mold  compound/polyimide interface, as shown in Figure 5. The  failure location determined with QuickSim is within 5 µm of  the actual failure location.


Figure 4: 3D X-ray microscope image at the identified failure  location showing anomaly between failed signal pin and  ground.


器313


Figure 5: FIB X-section at the identified failure location  showing solder extrusion into the delaminated mold  compound/polyimide interface.


Case Study 2:


In case study 2, a short failure in a flip chip package when  biasing a signal pin with respect to a power supply pin was  identified by curve trace. Figure 6 shows the waveforms


Short at bottom of C4


top of C4 Short at


acquired for the bare substrate (black solid waveform), and the  failed device (red solid waveform). Typically, a known good  reference device is an essential requirement for an EOTPR  investigation, which would make fault localization in this case  impossible. However, QuickSim allows the defect location to  be estimated with just the structure of the device under test.


X0


Solder extrusion


Figure 6: EOTPR results from the failed flip chip package. The  solid lines show the measured EOTPR waveforms and the  dashed lines show the simulation results. The EOTPR waveform  from the failed unit (solid red line) clearly shows a short failure  indicated by the negative feature at around 250 ps in the


Signal pinPower


waveform.


Supply Pin


As in case 1, a circuit model of the reference device was first  constructed and optimised using its measured waveform. The  location of the short fault was then determined by fixing all  parameters in the good unit model and sweeping the location of  a short failure to find the best fit to the measured fail unit  waveform. Figure 7 show the QuickSim simulation results for  shorts located at the top (orange dashed line), middle (red  dashed) and bottom (pink dashed line) of the C4 bump. In this  case the best fit to the fault location is at 45 % of the way along  the C4 bump element. This is equivalent to 36µm into the C4  bump, which indicates that the short fault was located in the  middle of the C4 bump.


3axa aue|wedo is u


Signal Pin


Measured - Bare


.-.Model- Bare


Measured - Fail


--·Model - Fall


---Model - Fall bottom C4


Pcyimidle


--·Model - Fail top C4


Short in


middie of C4


Figure 7: QuickSim data with simulated short defect at different


locations along the C4 bump.


Non-destructive X-ray imaging performed at the identified


200-


-Measured - Bare.-·Model- Bare


failure location supports the EOTPR results, which showed


-Measured-Fail


solder extruding between the signal pin and power supply pin


--'Model - Fail


at the midpoint (40 µm from the bottom) of the signal pin, as


shown in Figure 8. Subsequent physical failure analysis done  using FIB X-section confirmed that the short was caused by  solder flowing into an underfill crack, shorting the signal pin to  the power supply pin, as shown in Figure 9. Here, the failure  location determined with QuickSim is 4 µm from the actual


sCTPR SAra(


failure location.


X-section view


Figure 8: 3D X-ray microscope image at the identified failure  location showing filament short between failed signal pin and  power supply pin.


11


ANH KN


Bare Substrate


Underfill


Known Good Unit


Power


Signal


supply


Pin


Pln


flowed in


Solder mask


Sn


UF crack with solder


705


unesCOn qralarb-1on


Figure 9: FIB X-section at the identified failure location


showing solder flowing into underfill crack, shorting signal pin  to power supply pin.


-201


Case Study 3:


2500250500710cp25150017202,000


sgal/arbcorpn-300


Figure 10: Schematic of MCM package used in this study.


--· Model - Bare Substrate


- Measured - Bare Substrate


In case study 3, a short failure in a multichip module (MCM)


when biasing a signal pin with respect to the ground pin was


+200-


--·Model-Fail


observed by curve trace. It was noted that in the substrate


cLOD20030050060o20810


design, the initial trace from BGA contact splits into two traces  that link to two different die, as shown in Figure 10.


The waveforms obtained for a known good device (green) and  a reference substrate (black) are shown in Figure 11. The  features in both waveforms at 200ps correspond to the  branching point, whilst those at 400 and 1500ps correspond to  the substrate terminations that connect to Die 1 and Die 2, respectively.


Figure 12 shows the measured and simulated waveforms for the  bare substrate and the failed device, offset for clarity. The failed  device waveform shows a stronger negative feature at 200ps, arising from the short identified by curve tracer. In this case the  best fit to the fault location was found to be 30 µm from the top  of the PTH. The EOTPR fault localization was supported by  subsequent non-destructive X-ray imaging performed at the  identified failure location. Figure 13 shows the obtained  images, where a substrate defect can be observed at the top of  the PTH, causing a short between the signal line and the power  supply line. Here, the actual failure location is within 20 µm of  that determined with QuickSim.


BGA contact below


MCM package


Figure 11: EOTPR results from the MCM package for the bare  substrate (black line) and known good unit (green line).


Die 1Die 2


3630


Figure 12. EOTPR results from the MCM package. The solid  lines show the measured EOTPR waveforms and the dashed  lines show the simulation results. The EOTPR waveform from  the failed unit (solid red line) clearly shows a short failure  indicated by the negative feature at around 200 ps in the  waveform.


12


Figure 13: 3D X-ray microscope image at the identified failure  location showing substrate defect at the top of the PTH as the  cause of short between failed signal pin and power supply pin.


In summary, we have shown how EOTPR can be used in  conjunction with lump circuit modelling to non-destructively  isolate short failures in advanced IC packages.


Acknowledgments


The authors would like to acknowledge Advanced Micro  Devices, Inc. (Singapore) for collaborating in this project.


© 2019 Advanced Micro Devices, Inc. All rights reserved. AMD, the AMD Arrow logo, and combinations thereof are  trademarks of Advanced Micro Devices, Inc. Other product  names used in this publication are for identification purposes  only and may be trademarks of their respective companies.


[1] Y. Cai, Z. Wang, R. Dias, and D. Goyal, "Electro Optical  Terahertz Pulse Reflectometry - an Innovative Fault  Isolation Tool", Proceedings of the 60th Electronic  Components and Technology Conference (ECTC), Las  Vegas, Nevada, USA, June 1-4, pp. 1309-1315, 2010.


[2] M. Y. Tay, L. Cao, M. Venkata, L. Tran, W. Donna, W. Qiu, J. Alton, P. F. Taday, and M. Lin, "Advanced Fault  Isolation Technique Using Electro-optical Terahertz Pulse  Reflectometry", Proceedings of the 19th International


d


Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), Singapore, July 2-6, 2012.


[3] L. Cao, M. Venkata, M. Y. Tay, W. Qiu, J. Alton, P. F.


7 S


Taday, and M. Igarashi, "Advanced Fault Isolation  Technique Using Electro-optical Terahertz Pulse


L6


Reflectometry (EOTPR) for 2D and 2.5D Flip-chip  Package", Proceedings of the 38th International  Symposium for Testing and Failure Analysis (ISTFA),


VSS


PROCHOT_L


Phoenix, Arizona, USA, November 11-15, pp. 21-25,


2012.


[4] S. Barbeau, J. Alton, and M. Igarashi, "Electro Optical  Terahertz Pulse Reflectometry - a fast and highly accurate  non-destructive fault isolation technique for 3D Flip Chip  Packages", Proceedings of the 39th International  Symposium for Testing and Failure Analysis (ISTFA), San  Jose, California, USA, November 3-7, 2013.


L5 L6


[5] K.C. Lee, J. Alton, M. Igarashi, and S. Barbeau, "Feature  Based Non-Destructive Fault Isolation in Advanced IC


P R


Packages", Proceedings of the 40th International


C


Symposium for Testing and Failure Analysis (ISTFA),


HO


Houston, Texas, USA, November 9-13, pp. 214-218, 2014.


T L


[6] E. Kowalczuk, A. Bhattacharya, K. C. Lee, J. Alton, M. Igarashi, and S. Barbeau, “Fault Localisation of defects  using Electro Optical Terahertz Pulse Reflectometry and  3D EM modelling with Virtual Known Good Device”, Proceedings of the IEEE 3D System Integration  Conference 2014, Kinsale, Cork, Ireland, December 1-3


2014.


[7] K.C. Lee, J. Alton, M. Igarashi, and S. Barbeau, " Fast  Feature Based Non-Destructive Fault Isolation in 3D IC  Packages Utilizing Virtual Known Good Device ", Proceedings of the 41st International Symposium for  Testing and Failure Analysis (ISTFA), Portland, Oregon, USA, November 1-5, 2015.


[8] C. Schmidt, P. S. Pichumani, J. Alton, M. Igarashi, L. Chan, and E. Principe, " Advanced Package FA flow for  next-gen packaging technology using EOTPR, 3DXRAY & Plasma FIB", Proceedings of the 42nd International  Symposium for Testing and Failure Analysis (ISTFA), Fort  Worth Convention Center; Fort Worth , Texas, USA, November 6-10, 2016.


[9] B. Zee, W. Qiu, J. Alton, T. White, and M. Igarashi, “NonDestructive Fault Localization in 2.5D Packages Using  Electro Optical Terahertz Pulse Reflectometry”, International Symposium for Testing and Failure Analysis (ISTFA), 2017, EDFAS, November 5-9.


[10] Yi-Sheng Lin, Yu-Hsiang Hsiao, and Shu-Hua Lee, “Application of Electro Optical Terahertz Pulse  Reflectometry for Fault Localization and Defect Analysis”, International Symposium for Testing and Failure Analysis (ISTFA), 2017, EDFAS, November 5-9.


[11] J. Alton, T. White, and M. Igarashi, “Advanced Packaging  fault isolation case studies and advancement of EOTPR”, Electronic Device Failure Analysis, 2018, Volume 20, No.


4.


[12] Numerical Recipes in C, William H. Press et al., Cambridge University Press (1992)


13


Copyright © 2019 ASM International®


International Symposium for Testing and Failure Analysis


All rights reserved.


November 10–November 14, 2019, Portland, Oregon, USA


# Modern 2D & 3D X-ray technologies for testing and failure analysis


Modern 2D & 3D X-ray technologies for testing and failure analysis


Herminso Villaraga-Gómez and Joshua D. Bell


Nikon Metrology Inc., Brighton, MI, USA


Figure 1. X-ray image depicting the evolution of electric light


bulbs (from left to right: Edison style incandescent light bulb;


fluorescent light bulb; LED light bulb). Image obtained with a


Nikon XTH 225 ST X-ray system [1].


Modern 2D and 3D X-ray technologies are among


the most useful non-destructive testing (NDT) methods that


enable the inspection of an object’s internal features without


cutting or disassembling the sample. The discovery of X-rays


(Röntgen, 1895 [2, 3]) marked a revolution that led to major


advances in the fields of physics and medicine. Several X-ray


based technologies began in medicine, then found use in


industrial applications, and are today widely used in failure


analysis of manufactured medical devices, electronics,


packaging and assembly of printed circuit boards, etc. [4].


Some of the techniques that can be used for NDT include


radiography, laminography, computed tomography, limited


angle tomography, and computed laminography; they can be


of assistance in the determination of voids/porosity, flaws,


cracks, and inclusions within manufactured parts from the


electronics industry [5, 6]. According to a recent report


produced by the market research company and consulting firm


Research and Market™, the global market for industrial X-ray


inspection technologies (CT, radiography, and film-based


systems) is estimated to exceed the US$722.4 million by 2024


[7].  As the global manufacturing industry continues to grow


and require top tier safety and quality standards, X-ray


technologies and techniques provide the visualization and


metrology analysis necessary to meet those demands.  In this


paper, the authors discuss modern 2D & 3D X-ray based


approaches for testing and failure analysis, and describe how


these different methods have practical application for failure


analysis and dimensional metrology.


Radiography


The routing layout of the structure can clearly be identified in  Fig.4(a) due to metallization showing up in bright contrast as  more light is reflected towards the source (and hence  photodiode). The locations of the seven TSVs of the array are  also observable in the image, this also due to a modulation  effect of the reflected laser light. Most interestingly is that a  strong signal is detected when the laser is focused at the XY  coordinates x=14, y=24 (i.e. bottom-left TSV). This signal  identifies a location in the structure where the absorbed optical  energy is strongly interacting with the current flow through that  structure. As dielectric breakdown typically occurs at the  weakest part of the structure, this signal is a clear indication of  such a location where leakage current is flowing from the core  of the TSV, through the defective liner, into the substrate. The  measured increase in resistance indicates that the absorbed  optical energy causes impediment of leakage current flow  through the structure.


Fig. 4: (a) OBIRCH image measured after electrical  breakdown for an array of 7 TSVs. The scale bar (in color) represents the measured resistance between the TSV array  and substrate. The signal is superimposed on the laser  reflection image (in grey scale) (b) horizontal line profile  extracted from the OBIRCH image at the signal spot.


Figure 4(b) shows a line profile extracted from  Fig.4(a) through the signal spot as indicated by the dashed white


line. The measured resistance has been found to increase by ~120% from ~80 MΩ to ~175 MΩ at the signal spot.


The measured increase in resistance at the defect site is  attributed to a thermal heating effect of the defect (due to  conversion of optical laser energy into heat). Our observation  follows an expected positive shift in resistance given the  positive temperature coefficient of resistance (TCR) of the TSV  metals (Cu, Ni, W).


Whereas conventional OBIRCH is typically carried  out with a laser operating at a wavelength below the band gap  of silicon (~1120 nm) to avoid the generation of electron-hole  pairs (photocurrent generation) that may obscure the thermal  signal and skew data interpretation, we have selected a visible  laser operating at 405 nm for our measurements as there are no  electrical junctions in our structure (except the defect itself) where this may be problematic. By utilizing a visible laser, we  take advantage of [9]: 1) more incident laser energy being  absorbed by the structure for a given excitation power as metal  reflectance is lower at visible wavelengths than at near IR  wavelengths and silicon being highly absorptive at 405 nm, 2) larger power density due to smaller excitation spot resulting in


70


1.76x10B


more heat generated at the defect site and therefore stronger


1.70x10B


signal, 3)  increased spatial resolution it being directly related  to excitation wavelength, and 4) our measurement is highly


1.65x10B


sensitive to  near subsurface defects (below the STI oxide) due


to the very shallow absorption depth of the 405 nm excitation


40-


1.59x10B


light in silicon (<1 µm). Regarding the last point, thanks to the


1.53x10Beu


limited penetration depth of visible light in Si we can extract


defect depth information from the measured data set,


1.47x108ea


information that may otherwise be difficult to extract from


]Y[μm20- Position


measurements performed with a near-IR excitation laser. The


1.42x10B


narrow signal spot in Fig. 4(a) indicates that the defect is most  likely located right below the surface of the structure, as deeper


10-


1.36x108


defects would have resulted in a much weaker signal spot (if at


1.30x10B


all observable) and must be broader due to heat spreading.


However, localizing those defects may still benefit from the use


X Position [um]


of a longer wavelength excitation (including near IR) laser due  to the limited absorption depth of the 405 nm excitation light in  Si. At last, we note that the signal spot is observed when the


1.75x108


laser is illuminating the Si and not the Al metallization segment.


乙


]


1.50x1088


We attribute this observation to the fact that the optical


absorption coefficient of Si (it being a semiconductor) is much


1.25x108eu


higher than Al (metal so a good light reflector), thus this


1.00x1089s


inevitably results in a higher temperature rise and signal when


y


the laser is illuminating the Si instead of the metallization


7.50x107


segment. As the signal spot is located at the left side of the


010 20 30405060


metallization line, we also expect the defect to be located


X-position [um]


towards that side of the TSV. We further note that  circumferential localization info may be difficult to obtain from  an OBIRCH measurement with a near-IR laser as the signal  spot would be generated on the metallization segment itself  above the 3 µm wide TSV. However, no information is  currently available to confirm this.


22


Chip Deprocessing


A combination of mechanical milling, chemical  etching, SEM inspection and FIB cross sectioning was carried  out to further investigate the failure location and cause. The Si  substrate was selectively removed to enable SEM inspection of  the TSV and its dielectric liner to localize the defect. This  differs from the more conventional approach whereby a 3D cut  is typically created by performing stepwise FIB milling and  SEM imaging. A concern for that method is that depending on  the selected milling step size, small defects may not be localized  and are destructively removed in the process. By selectively  removing the substrate, we can ensure that the TSV and its liner  remains intact and thereby also provide opportunity for further  analysis. Substrate removal was performed from the chip  backside by abrasively milling a crater in the substrate with a  diamond milling tool, this followed by a selective wet etch  towards the STI oxide on the chip frontside. To prevent  cracking in the chip during deprocessing, we have bonded the  sample frontside down on a glass cover slip using an etchant  resistant epoxy for mechanical support. Fig.5 schematically  shows cross-sectional views and sample images of the twostage milling (left image) and etching (right image) process. Abrasive milling was performed down to a depth of ~688 µm (measured from the wafer backside) to leave a remaining Si  thickness of ~50 µm towards the bottom of the TSV. The  remaining Si was thereafter removed using a  tetramethylammonium hydroxide (TMAH) based etchant  which has an excellent etch selectively over SiO2. A high etch  selectively over SiO2 is highly desirable to ensure that the  dielectric liner remains intact and defects are not removed  during etching. For an etch selectivity ratio between Si and  SiO2 of ~5000 [10], we expect that the liner thickness has  reduced by a maximum of 10 nm at the bottom of the TSV.


Etching was performed at a temperature of 85 ˚C to achieve an


etch rate of ~1 µm/min. We note that increasing the temperature


of the etchant above 85 ˚C may considerably reduce the etching


time in future [10].


Fig. 5: two-stage chip deprocessing for substrate removal by  mechanical milling (left) and chemical etching (right). Optical images are shown after both steps. The crosssectional views illustrate the process steps and provide  depth information of the removed material.


Figure 6 shows SEM images of the TSV array after  substrate removal. The TSVs can clearly be identified in the  figure as upstanding pillars.  We note the etching process has  not introduced severe roughness in the TSVs as the sidewalls  appear smooth. SEM inspection has revealed a small pinhole  defect in the liner of a TSV as indicated by the red arrow on the  zoomed-in view. The location of this pinhole on the SEM image  has been found to be in excellent agreement with the location  of the signal spot on the OBIRCH map (Fig. 3, note: SEM  image looks from chip backside). No pinholes were observed  for the remainder of the array. Also, as expected from our laser  stimulation results, the dielectric breakdown has occurred near  the surface of the chip (i.e. top side of TSV).


Fig. 6: SEM image after the removal of the silicon substrate  by mechanical polishing and chemical etching. The TSVs  are free-standing and can be easily inspected. The yellow  arrow indicates the viewing angle for the zoomed in image  of the short failed TSV.


As can be observed on the SEM images, the scalloped sidewall  roughness (an artifact of the Bosch dry-etching process) is  stronger near the top of the TSV (i.e. bottom of the SEM  images) giving indication of a region where the thickness of the  dielectric liner may not be not uniform and therefore a  reliability concern.


A FIB cross-section (Fig. 7, different TSV but same  wafer) was thereafter made to investigate the dielectric liner  thickness uniformity of the TSV process in greater detail. As  indicated by the red arrow in figure 7, a local reduction in  dielectric liner thickness is observed right above the bottleneck  of the TSV, this being in excellent agreement with our SEM  observations. The local reduction in dielectric thickness  signifies a weakness in the dielectric liner where local electric  field enhancement may inevitably lead to a failure.


23


Fig. 7: FIB cross section image of a TSV (different TSV, same wafer) indicating a local reduction in liner thickness  near the TSV bottleneck


The application of laser stimulation and chip deprocessing has  been demonstrated for the localization of a dielectric pinhole  defect on a short failed (R ~ 0.1GΩ) 3x50 µm TSV array. We  have been able to pinpoint the breakdown site in XY and Z by  an optical beam induced resistance change measurement. Observation of a signal with short wavelength excitation light (λ =405 nm) with a corresponding short penetration depth in Si (  <1 µm) provided evidence of a near-surface defect. Deprocessing the chip by abrasive milling and chemical etching  enabled us to validate our result through SEM inspection. The  failure cause has been attributed to a local reduction in liner  thickness near the bottleneck of the TSV through the Bosch dryetching process.


[1] E. Beyne, IEEE Design & Test, vol. 33, no. 3, pp. 8-20, (2016)


[2] I. De Wolf, EDFAAO 18, 24 (2016)


[3] S. Van Huylenbroeck et al.,2016 IEEE International 3D  Systems Integration Conference (3DIC), San Francisco, CA, 2016, pp. 1-4.


[4] Y. Lee et al., Microelectronic Engineering, vol. 156, pp. 37-40 (2016)


[5] F. Altmann et al., Proc. 43rd ISTFA, Pasadena, USA, 2017, pp.19-24


[6] A. Redolfi et al., Proc. 2011 IEEE 61st ECTC, Florida, 2011, pp. 1384-1388.


[7] Y. Li et al., Proc. 2015 IITC/MAM,  Grenoble, 2015, pp. 327-330.


[8] Κ. Nikawa, S. Tozaki, Proc. Proc. ISTFA, pp. 303-310,


1993.


[9] P. Tangyunyong, A. Rodarte, EDFAAO (2019) 2:4-7


[10] O. Tabata et al., Sensors and Actuator A, 34, 1992, pp.51-57


24


GHz-SAM for Warped Samples using HiSA


C. Hollerith, D. Le


Infineon AG, Neubiberg, Germany  christian.hollerith@infineon.com


P. Hoffrogge


PVA TePLA, Westhausen, Germany


M. Böckler


HS Aalen, Aalen, Germany


GHz-SAM using toneburst transducers is a method currently  lacking the possibility to measure warped samples easily  because large parts of such samples are out of focus due to the  limited depth of focus of these types of transducers. This paper  shows an approach to use the already established HiSA (High  Speed Axis) method to overcome this disadvantage. Therefore  warpage of the sample is measured by a white-light  interferometer. The detected bow is parametrized and submitted  in the control electronics of the HiSA. With this data the HiSA  is enabled to keep the distance between sample and transducer  precisely constant. This allows eliminating the influence of the  warpage on the performance of this method and therefore  highly increases the image quality.


Due to the ongoing integration of dies inside the package, known under the slogan “More Than Moore” [1], innovative  methods to detect also very small failures within packages are  essential. One of these lately developed methods is highresolution SAM using toneburst transducers with frequencies


up to 1 GHz [2]. Unfortunately the focal length and also the  depth of focus of these transducers are very short and therefore


0、


image resolution is strongly influenced even by small warpages  of the samples of some 10 µm. On the other hand especially


-20


2.5D- and 3D-packages show comparatively high warpage due  to complex material setup and high CT-mismatch. Thus, for


40、


warped packages a method is necessary to keep the distance  between transducer and warped sample constant.


-60 HiSA is a SAM scanning system with a very fast z-axis infeed 0 which is mechanically able to keep the distance between


2000


transducer and sample constant during scan. Typically in SAM


4000


the distance between sample and transducer can be determined


6000


400060008000


sufficiently precise by measuring the time of flight of the


800002000


surface signal. This method is used to control the HiSA of  contemporary PVA TePLA-SAM systems [2]. Unfortunately  toneburst transducers show no surface signal which could be  detected easily. Additionally the signal is quite long in the time


domain as the exciting frequency is within a narrow band and  can therefore not be used for sufficiently precise TOF  measurements. Thus, conventional HiSA is not usable for  toneburst-transducers.


Warpage measurement


A solution to overcome this issue is to control the HiSA with  external data. In this case a Cybertechnologies CT100 whitelight interferometer was used to measure the surface profile of  a sample. The height resolution of the included sensor is about  14nm allowing measuring the z-profile precisely. The used  sample was a flip-chip with known cracked solder bumps in one  sample corner. First, the flip-chip was grinded from the  backside with only a small amount of silicon remaining. Afterwards, the silicon was removed completely by dry  chemical etching. So the backside of the metallization stack of  the die was accessible to SAM. Remaining thickness below the  pads was about 2 µm. The measurement of this sample by  white-light interferometer can be seen in fig. 1.


Figure 1: Warpage measurement of die surface (all axes are  in µm)


# GHz-SAM for Warped Samples using HiSA


25


This measurement can be done quite fast, a scan like seen in fig. 1 is done within 2 minutes. This measurement shows a warpage  of the sample of about 50µm, see fig. 2.


Figure 2: Line scan from corner to corner


Subsequently, the complete surface measurement data was  fitted with a paraboloid function using Matlab, see eq. 1.


   =   1 +   2 ∗    +   3 ∗   2 +   4 ∗    +   5 ∗   2


Equation 1: Fit function for measured profile, see fig. 1


The found coefficients c1-c5 were used to control HiSA as  described in the next chapter. Using the coefficients offers two  advantages. On the one hand it easily removes noise from the  measured data and on the other hand it proved for HA Aalen to  be the easiest way to import warpage data into the HiSA axis. The disadvantage of this method is that samples have to be  nearly parabolic to follow this approach.


Figure 3: Deviation of fit to measured height


Fig. 3 shows the deviation of the parabolic fit to the measured  data. It shows that the fit works very well, deviation of the  measured surface to a paraboloid is only a few micrometers, so  this is still within the focal depth of the transducer.


HiSA with external warpage data


PVA TePLA together with HS Aalen developed an additional  control algorithm for HiSA. It allows following a parabolic  shape with external defined coefficients. Thus, with help of the  data port in the HiSA control electronics all coefficients c1-c5 of  the fitted paraboloid in eq. 1 are imported and can be  reproduced in the HiSA. A first test of this new method was  performed with a 230 MHz transducer with 2.4mm focal length, see fig. 4. The left image shows the TOF measurement without  activated HiSA. The right image shows a TOF measurement  with the same scaling after activation of the HiSA based on the  fitted data from CT100.


Figure 4: TOF measurement of sample surface with 230MHz  conventional transducer without HiSA (left) and with activated  HiSA (right) using same color bar for warpage


The plot with activated HiSA only shows differences in TOF in  the order of µm. Therefore the method proves to work  sufficiently also for 400 MHz toneburst transducers. After the  first functional test of the external measured warpage data, the  flip-chip sample was measured with 400Mhz toneburst  transducer, see fig. 5.


26


Figure 5: Flip-chip sample measured with 400Mhz TBtransducer without HiSA


Due to high warpage, the sample can only be focused in the  center of the sample. The sample edges and the corners are  completely out of focus and no image at all is obtained from  these areas. Figure 6 shows the same sample with activated  HiSA using imported data. Here a homogeneous image quality  is obtained over the whole sample even showing the corners of  the sample in focus.


Figure 6: FC-Sample measured with 400 Mhz TB-transducer  with activated HiSA, damaged bumps marked


The magnification of the upper right corner shows that


defective bumps can be clearly separated from undamaged  bumps, see figure 7.


Figure 7: Upper right area of figure 6, damaged bumps (red) vs. undamaged bumps (green) clearly visible


In the example used in this paper, a crack was found in the  BEOL below the bump, see figure 8. Thus, this method allows  fast and efficient inspection for defective bumps also on quite  large, warped samples with homogeneous image quality till  edges and corners. A homogeneous image quality is very  important for the detectability of defective bumps as they are  identified in contrast to undamaged bumps. This is a  challenging task as in many packages the number of bumps is  very large and they therefore appear small in the image, as can  also be seen in the overview image of this example, see figure


6.


Figure 8: FIB- cross section of damaged bump, damage in  low-k dielectricum is marked. The UBM of the bump causing  the damage can be seen on the lower part of the image. The  scan size of the image is approximately 20 µm


Thus, varying image quality impedes the inspection and  therefore increases failure rate of inspection.


Conclusions and Outlook


The presented method significantly reduces the effects of  warpage in measurements with toneburst transducers and  therefore helps to extend the usability of the method to state of  the art packages. In these often warped packages small failures


27


can be detected also on large areas now and therefore allows  complete scan of such a package in one step and with high  quality to do inspections such as searching for defective bumps.   In future this method shall be established by default in the  WINSAM-software of PVA TePLA. It also should be possible  to import measured and filtered data directly into the HiSA to  be able to correct also irregular warpage shapes. Also  determination of fit-parameters with TOF measurements of  conventional transducers shall be included although in any case  white-light interferometry offers better resolution and better  precision for determination of the needed fit parameters and  would be the preferred method if available.


This work has been performed in the project SAM3, where the  German partners are funded by the BMBF under contract


16ES0339k and the French partners by the French Ministry for  Industry and Economy. SAM3 is a joint project running in the  European EUREKA EURIPIDES and CATRENE programs.


[1] W. Arden, M. Brillouet, P. Cogez, M. Gräf, G. Huizing and


R. Mahnkopf, “More than Moore” White Paper,


http://www.itrs2.net/uploads/4/9/7/7/49775221/irc-itrsmtm-v2_3.pdf


[2] P. Czurratis, T. Tjuric P. Hoffrogge, New Scanning  Acoustic Microscopy Technologies Applied to 3D  Integration Applications, 2013 Workshop on 3D  Integration


Application: https://www.nist.gov/sites/default/files/czurratis.pdf


28


GHz-Scanning Acoustic Microscopy combined with ToF-SIMS/AFM for   wafer-level failure analysis of bonding interfaces.


Ingrid De Wolf*, Ahmad Khaled*, Alexis Franquet, Valentina Spampinato, Thierry Conard


imec, Leuven, Belgium


*also at Dept. Materials Engineering (MTM), Fac. Engineering Science, KULeuven, Leuven, Belgium Ingrid.dewolf@imec.be


Sebastian Brand, Michael Kögel


FhG IMWS-CAM, Halle, Germany


Ingo Wiesler


PVA TePla Analytical Systems GmbH, Westhausen, Germany


This paper discusses the implementation of GHz-Scanning  Acoustic Microscopy (GHz-SAM) into a wafer level scanning  tool and its application for the detection of delamination at the  interface of hybrid bonded wafers. It is demonstrated that the  in-plane resolution of the GHz-SAM technique can be  enhanced by thinning the sample. In the current study this  thinning step has been performed by the ion beam of a ToFSIMS tool containing an in-situ AFM, which allows not only


chemical analysis of the interface but also a well-controlled


"9


local thinning (size, depth and roughness).


In recent years, GHz-SAM [1] got increasing attention for its  potential application for failure analysis in microelectronics  systems [2,3]. Especially for 3D technology applications, its  higher spatial resolution compared to conventional SAM, its  ability of exciting and visualizing Rayleigh waves, and its  superior sensitivity to sub-surface defects, make this technique  of high interest [4-7].


We have previously demonstrated [8] that the GHz-SAM  system, which consisted of an acoustic lens implemented onto  an optical microscope (SAM1000, PVA TePla), allows  analyzing the interface of a hybrid bonded wafer pair through  a 5 μm thick top Si chip, and, in particular, enables the  detection of delamination near single micron-sized Cu-Cu  bonded pads of a daisy chain array connecting both wafers.


Although local defects near Cu-Cu pads could be clearly seen (Fig. 1 left), further issues and open questions remained. A  first issue concerns interference effects which caused large  interference fringes in the GHz-SAM images, complicating  the data analysis and interpretation. This interference artefact  is visible in all images of Fig. 1. A second open issue  addresses the achievable resolution. For daisy chains with 900  nm top and 2700 nm bottom Cu pad width, individual pads


could be distinguished (Fig. 1, left). However, the acoustic  image obtained on 900 nm top and bottom Cu pads, as shown  in Fig. 1 center, did not reveal individual pads. In this paper, both issues are addressed, and solutions and/or optimizations  are demonstrated.


Figure 1: GHz-SAM images of a daisy chain array consisting  of Cu-Cu bonded pads. Left: Top/bottom wafer Cu pad size is  900 nm/2700 nm (DC30) (scan field ~200μmx200μm). Center: Top/bottom wafer Cu pad size is 900 nm/900 nm (DC40) (scan  field ~200μmx200μm). Right: GHz-SAM image of a bare Si  wafer, scan field 1mmx1mm.


Samples


The investigated sample is a chip obtained from a wafer stack  with a 5 μm thick top Si wafer which was hybrid bonded to a  full thickness bottom wafer (Fig. 2a). The chip contains  various interwoven daisy chain (DC) arrays, shown as  rectangles at the top left of the chip design in Fig. 2b. A zoomin on the design of one such a rectangle is shown in Fig. 2c, and a further zoom-in to the top of a rectangular array in Fig. 2d. The latter shows the top (grey) and bottom (white) metal  connections and Cu pads (white dots). The chips contain  arrays with different widths of the top and bottom Cu pads and  also different pad densities. Table 1 lists the width of bottom (Wb) and top (Wt) Cu pads and their pitch for two investigated  daisy chains.


# GHz-Scanning Acoustic Microscopy combined with ToF-SIMS/AFM for wafer-level failure analysis of bonding interfaces.


29


b


c


△z=2f(1-cosθR)'vwater


(1)


Figure 2. a. Schematic cross-section through the hybrid-bond  interface of the samples. b. Chip design, with at the top left the  location of interwoven daisy chain arrays (rectangles) containing different widths of the top and bottom Cu pads. c. Zoom-in on one of the arrays. d. Zoom-in to the top of a  typical array. Dark lines are top metal (M1 Top in Fig. 2a), white lines refer to bottom metal (M1 bottom in Fig. 2a). White dots show the location of the Cu pads.


Table 1: Size information of the Cu pads for the two analyzed  daisy chains: DC30 and DC40. Wb is the width of the Cu pad  at the bottom, Wt of the one at the top (see Fig. 2 a).


||Daisy chain name: |Wb-Wt / Pitch (nm |
|---|---|---|

|DC30: |2700-900 / 5400 ||

|DC40: |900-900 / 2250 ||

)


Results


Top Si wafer


5 μm thickM1 Top


Fringes


To study the origin of the fringes visible in the scans of Fig. 1,


Cu pad Top


tests were done with various settings and parameters of the


Bonding Interface


acoustic GHz-microscope (acoustic lenses, frequencies, gate  width and position, pulse width, defocus, scanning area,


Cu pad Bottom


sample tilt, scanning frequency). From the obtained results, it


M1 Bottom


was concluded that the occurrence of the fringes most likely


Bottom Si


originates in the behavior of the scanner unit, to which the


wafer


acoustic lens is mounted. When during a scan in x and y (in


Full thickness


the sample plane), the distance z (out-of-plane distance) between lens and sample is not constant, interference between  individual signals will occur. Indeed, for wide-angle acoustic  lenses, as the ones used in GHz-SAM, surface acoustic waves  are excited on the sample surface (Rayleigh waves) in addition  to the geometrical waves (Fig. 3, top). The echoes of both  acoustic wave modes reach the lens after interaction with the  sample and interfere, affecting the total measured signal  intensity. These signals, which vary in time of flight (TOF) according to the axial spacing between the sample and the lens  also have the potential of interfering with static internal lens  signals that occur upon the excitation of transverse and  compressional modes that are converted into one another at  the boundaries of the lens. If the distance between the lens and  the sample is fixed, phase alteration between the individual  static and dynamic signals is kept constant and consequently  the total signal intensity remains constant. If e.g. the lens  approaches the sample by a distance Δz, the propagation path  of the Rayleigh wave increases, while that of the geometrical  wave decreases (see Fig. 3, top) leading to a change in relative  phase of the two signals and resulting in alternating  constructive and destructive interference affecting the  intensity when changing the focus of the lens, as shown in Fig. 3, bottom (from [9]). The distance, Δz, between periodic  minima or maxima is given by [9]


where, vwater is the acoustic velocity in water, f is the acoustic  wave frequency and ϴR is the critical angle for exciting  Rayleigh waves on the sample. So, the higher the frequency, the smaller ∆z. For the GHz lens used in our system, the zdistance between a minimum and maximum ∆z/2 is about 7 µm. But already for smaller changes in z, variations in  intensity will be observed as can be deduced from Fig. 3, bottom. A small z-motion of the lens upon scanning in x and y  will cause phase alterations resulting in the occurrence of  interference fringes visible in the images of Fig. 1. From these  experiments it can be concluded that a perfect control of z is  required for optimal measurements using a GHz-SAM system.   To confirm this, the GHz-lens was mounted on a conventional  SAM system (SAM300, PVA TePla) which contains a larger  scanner system and a water bath. The electronics were adapted  to allow for operating the GHz-imaging equipment. An  additional advantage of this system over the microscope  version is that it allows much larger scan fields (instead of 1


mm x 1 mm, 10 mm x 10 mm and larger, depending on  sample flatness). Fringe-free results obtained with this system  on single and multiple arrays and their contact pads, and for  small and large scan fields, are shown in Fig. 4. The resolution  evaluation discussed in the following part was mainly  performed using this adapted system.


700


TOFSIMS crater


tudes [a.u.]relative ampli200


0.0


200204060


-1.0-0.5


300 400 500 600


△z


defocus position [μm]


-1.5


Figure 3: Top: Schematics showing how the distance lenssurface affects the path length of geometrical and Rayleigh


-2.0


waves. Bottom: Impact of focus position (z) on GHz-SAM


Topographym) (μ-2.5


signal intensity (V(z)-curve). Taken from [9].


0100200300400-3.0+


aa


Cc


Figure 4: GHz-SAM images taken on a wafer scanning  system. Scan field a. 420µmx290µm, b. zoom-in on the image  from a, c. 3mmx2mm, d. 8mmx7mm


Learning Toolbox (MATLAB, The Mathworks, Nattick, MA,


The core blocks of the CNN consist of a set of filter kernels with


USA).


a small receptive field that moves across the input signal  performing the convolutional operation. The same


Verification by physical cross-sectioning


transformation is applied to every segment of the signal. A


For physical verification, selected rows of bump interconnects


pattern learnt at one position can also be recognized at a


were cross-sectioned and polished using a Mecapol P230 (Presi


different position, making the 1D-CNN translation invariant.


GmbH, Germany). Imaging was performed by optical


The subsequent downsampling by pooling layers reduce the


microscopy.


dimension of the input data and preserve the extracted features  that are characterized by displacement, scaling and invariance


Case Study I


[5]. Finally, after the applying multiple of the above described


The first sample addressed in the current study is a SAM dataset


layers, the high-level processing in the neural network is


recorded from a CPU-device manufactured in flip-chip


performed by fully connected layers with connections to all


technology containing solder bumps with a diameter of 80 µm


neurons in the previous layer. The output contains the


for interconnecting the silicon die to the organic laminate


probability distribution over a set of classes with respect to the


substrate. The surface area of the silicon die was


input.


In Figure 2 the final architecture of the model is shown. The  network consists of three convolutional blocks followed by a  fully-connected layer with a softmax activation function [6] as  output. Each of the convolutional block starts with a  convolutional layer followed by a series of normalization  layers. Figure 2 also contains the number of feature maps, the  kernel size of the filters and the size of the pooling layers. After  each block, a dropout layer with a probability of 0.2 is applied  to avoid overfitting of the model. The training procedure has  been applied with a stochastic gradient descent optimizer [6] for  50 epochs by a batch size of 64.


The labeled dataset was split into an 80% training, 10% validation and 10% test dataset. For the datasets an equal  distribution of the occurrence of the individual classes was  aimed for. While the training dataset was used to fit the  parameters of the model, the validation dataset served for  tuning the hyperparameters of the model architecture. The  performance of the proposed method is evaluated on a separate  dataset of an unknown sample. To measure the performance of  the model the following metrics are used to measure the  performance of the model: Accuracy and Cross-entropy loss.


400Um


Conv [4x1]Conv [8x8]Conv [8x16]


Norm/DropNorm/DropNorm/Drop


Pooling [2]Pooling [2]Pooling [2]Layers


Fully-Connected


silicon


defective bump


intact bumps


Figure 3: Images from processed SAM data recorded from a  flip-chip CPU-device. Top: BAI micrograph from C-Scan


119x1 117x8 59x8 57x16 29x16 27x32324


Figure 2: Architecture of the final model with three


through the silicon die with the bump interface in focus.


convolutional blocks followed by a fully-connected layer. The


Bottom: Cross-section image along red marker in Top-graph


top line contains the size of the filter kernels and pooling


(B-Scan) through the CPU-device. The orange lines (dashed)


windows. At the bottom the size of the input and the feature


indicate the boundaries of the 725 µm Si die and the flip-chip


matrices are described. The bottom of the fully connected layers


interface underneath marked in red (defective bump) and green


contains the number of nodes per layer.


(non-defective bump) arrows.


37


20 mm x 20 mm with a thickness of approximately 725 µm.


on top of the bond interfaces, differentiation between variations


The selected ultrasonic transducer was operating at 230 MHz


in the silicon/bump interface and the defects are difficult to


with a focal length of the aperture of 8 mm in water.


assess from these amplitude image.


Figure 3 illustrates a classic signal analysis approach for failure


ICA on sample #1 was performed extracting 12 independent


analysis by SAM through the top of the sample for the given


components from the rf-echo signals after dimensional


region of interest (ROI). Parameter values of the BAI were


reduction and pre-whitening of the input data by PCA. The


computed within the time range between the exit echo of the


weighting matrices of the individual independent components


silicon and the solder/substrate interface. The result shows that


containing patterns corresponding to the sample structure or to


an evaluation purely by amplitude and phase deviation is not


potential defects were summed to maps for each class. By


sufficient for a defect identification and localization in such


thresholding the resulting matrices, binarized masks are


complex geometries.


generated for the following four categories: defective bump,


The ICA was performed on the 3D data matrix (x, y and t) after


intact bump, background and idle (including signals that are


pre-whitening and dimensionality reduction by principal


related to diffraction artefacts from edges). In order to verify


component analysis (PCA) [7]. The extracted eight independent


the marked positions to be truly corresponding to defective


components with the highest variance within the data were used


bumps physical cross-sectioning was performed. Afterwards


for evaluation. The binarized masks derived from the estimated


the labeled dataset was formed by labeling each of the timeweighting matrices were compared to results from crossdomain signal vectors from the SAM dataset according to their


sectioning and SEM imaging of previous investigations on the


position in the binary masks. For training, validation and test,


same dataset as described in [2].


the elements in each class were selected randomly from the data  set, while keeping the number of elements equal. The 1D-CNN


Case Study II


model was trained after the adaptation of the hyperparameters


The second case study addressed a set of samples consisting of


for best results on the validation dataset. Performance


a daisy chain interconnected through SnAgCu-bumps with a


parameters of the final model were estimated using the test


diameter of ~280 µm to the external circuitry manufactured in


dataset. Finally, the model derived and trained by the data of


flip-chip technology. The thickness of the top silicon layer was


sample #1 was applied to the data recorded from sample #2. A


approximately 375 µm. The ultrasonic transducer for acquiring


rf-signal was assigned to a certain class when its predicted


the unprocessed rf-data operated at 175 MHz with a focal length


probability was above 70%. Physical verification on sample #2


of the aperture of 4 mm in water.


was performed in order to evaluate the benefit and applicability


Based on the results of conventional SAM as provided in Figure


of this machine-learning based approach.


4, the presence of several defect types can be assumed from the  differences in amplitude and phase that appear in those graphs.


Resolution


To test whether the thickness of the top Si (5 μm here) through  which imaging of the sample interface was performed, has  impact on the spatial resolution of the GHz-SAM, the sample  had to be thinned, preferably locally, to a well-controlled  thickness. For this purpose, an in-house available ToF-SIMS  tool which is equipped with an AFM (ToF-SIMS V, ION-TOF  GmbH, Münster, Germany) was used. An optical image of the


sample with ToF-SIMS crater on top of an array and an in-situ


Acoustic Lens


AFM scan through the center of the crater are shown in Fig. 5.


Water


Δz


The crater is about 300 μm x 300 μm wide and at the center


wave


defocus Scanner


about 3 μm deep (2.85 μm + 0.03 μm), indicating that the  remaining Si thickness at the bottom of the crater is about 2


10年Geometrical


wayww


RayleighSithe sample


Rayleigh


Moving towardt


μm. The bottom surface is flat but shows an increased


roughness (RMS = 30 nm) compared to the Si surface outside


waves


the crater.


Position (μm)


Figure 5: ToF-SIMS crater located on top of daisy chain  DC30 (see Fig.2e). Top: optical image (IR laser scanning  microscope) of the crater. Bottom: AFM topography scan  across the center of the image.


Fig. 6-top shows a GHz-SAM image obtained inside the crater  shown in Fig. 5. The bonding interface can clearly be imaged. This result demonstrates that it is possible to perform GHzSAM imaging inside such a crater. Imaging of this interface  with an IR laser scanning microscope is not possible, due to a  too high roughness (Fig. 6, bottom left). Outside the crater, IR  imaging is possible, but only the top metal pads and, in  between, part of the bottom metal pads can be seen (Fig. 6, bottom right, compare with design in Fig. 2d). This results in a  cross-like image. These results show that GHz-SAM seems  not to be affected by surface roughness, in contrast with IRimaging.


31


40 µm


Thinned (I um Si)


80 μm


15 μm


Figure 6: Top: GHz-SAM image obtained from the interface  through the bottom of a 3 μm deep crater made by ToF-SIMS (2 μm Si remaining) on top of daisy chain DC30 (see Fig.2e). Bottom left: IR laser scanning microscope image of the crater. Bottom right: IR laser scanning microscope image taken  below the crater of the central figure, at a position where the  Si was not thinned (thickness =5 μm).


To answer the question regarding the impact of thinning on  the achievable lateral resolution of the GHz-Sam imaging, a 4


μm deep crater was prepared (leading to about 1 μm remaining


Si) on top of a DC40 structure containing 900 nm square Cu  pads. Fig. 7 shows a GHz-SAM image recorded partly in the  crater and partly outside. Inside the crater, the individual Cu  pads can be seen, although with some noise. Outside the crater  the Cu pads cannot be distinguished. This indicates that the


1.4 resolution improves when thinning the sample to reduce the PC1.2 propagation path of the acoustic waves. One could argue that


8/P1 O


the system focus was optimal for the region inside the crater


00.8


and not for the one outside the crater in Fig. 7. Changing the


0a


focus in the region outside the crater however did not improve


E


the resolution considerably. In addition, the central image of


p8心


Fig. 1 shows the results obtained on a similar sample (DC40),


u


without thinning and with optimal focusing conditions. The


uC2FSi305iO02SIozCICNHCC3180OHSIOSiNsiz


resolution is clearly worse than after thinning. This impact of  thinning on resolution might possibly be due to the  contribution of surface Rayleigh waves interacting with the Cu  pads. The Rayleigh waves are composed of both longitudinal  and shear waves and provide nm resolution on the surface of  the sample. By thinning the top silicon layer to 1 µm, Rayleigh waves can penetrate the silicon and reflect from the  Cu pads and still be received at the lens transducer with


adequate intensity providing a significant increase in GHzSAM resolution.


The ToF-SIMS craters were made with a 2 keV O2+ sputter  beam. Reducing the sputtering energy to 500 eV reduced the  roughness from ~30 nm to 8 nm. This reduced roughness now  allowed IR laser scanning microscopy imaging of the metal  layers through the thinned Si. But it did not conclusively  impact the GHz-SAM results. This confirms that the impact of  roughness (at least up to an RMS of 30nm as studied here) on  GHz-SAM can be neglected.


Not thinned (5 μm Si)


Daisy chain:Wo-WiRemaining SiCrater depth


DC40:900-900I μm


4 μm


Figure 7: GHz-SAM image obtained from the interface  through the bottom of a 4 μm deep crater prepared by ToFSIMS (1 μm Si remaining inside the crater, 5 μm outside). The  crater is located on top of daisy chain DC40 (see Fig.2e).


The purpose of a ToF-SIMS system is of course not sample  preparation. It was used here only to demonstrate the effect of  thinning on the lateral resolution in GHz-SAM. However, during the thinning, also a chemical analysis of the sample  along the depth was performed, comparing an electrically  yielding sample (good) with a defective (bad) one. The  intensity ratio of various detected elements is compared in Fig.


8. Si and Cl are compared with Cu in Fig. 9. This analysis  allows to detect which element is present at which interface. For example, in this test Cl was detected at the bonding  interface. The difference in Cl between bad and good sample  is however too small to allow any conclusions on its potential  reason for the failure cause of the defective sample.


lon cluster


Figure 8: ToF-SIMS analysis results obtained at a similar  position (see Fig. 9) of two samples: a good and bad (showing  air gaps) one. The data show the intensity ration of various  ions and ion clusters measured in these samples.


32


Figure 8: ToF-SIMS analysis along the depth measured on a  good and bad (showing air gaps in the GHz SAM) hybrid  sample and comparison with cross-section FIB/SEM images of  Cu-Cu bonded pads of the bad sample (the latter were not  taken at the same position as the ToF-SIMS analysis, but used  for positioning of the ToF-SIMS signals along the sample  depth).


In this paper we show that in a GHz-SAM system, interference  fringes can become visible if the distance acoustic lens to  sample varies by even a few microns during scanning. The  GHz-SAM is demonstrated to work very well and fringe-free  on a wafer scanning system with a robust X-Y scanning unit, allowing GHz-imaging of much larger scan fields and a study  of the impact of top Si thickness on resolution.


It is demonstrated that the resolution of the GHz-SAM for  defects and features located at the interface of two bonded  wafers, can be improved by thinning of the top Si. Cu pads as  small as 900 nm can be distinguished. The GHz-SAM results  are not measurably affected by the surface roughness, while  this has a clear impact on optical imaging. For example, while  GHz-SAM imaging is possible through a surface with RMS 30  nm, this is not possible using IR laser scanning microscopy.  For the purpose of thinning, a ToF-SIMS system combined  with an in-situ AFM was used. This allowed control of the  crater depth and width, and also of the roughness at the  bottom. In addition, this approach allowed for chemical  analysis of the samples and sample interface. Although an ‘expensive’ tool to be used for sample preparation, this might  open new opportunities for the combination with other FAtechniques.


Acknowledgements


The authors thank the 3D technology team from imec for  providing samples and acknowledge the EU Horizon 2020  Metro4_3D project under the grant No 688225.


[1] A. Briggs and O. Kolosov, Acoustic Microscopy, in  Monographs on the Physics and Chemistry of Materials. 2nd ed. 2010, Oxford, Oxford University Press


[2] S. Brand et al., Detection and analysis of stress-induced  voiding in Al-power lines by acoustic GHz-microscopy. Microelectronics Reliability 64, pp. 314-345, 2016


[3] G. Vogg et al., Scanning acoustic GHz-microscopy versus  conventional SAM for advanced assessment of ball bond  and metal interfaces in microelectronic devices. Microelectronics Reliability 55, pp. 1554-1558, 2016


[4] F. Altmann et al., Innovative failure analysis techniques for  3-D packaging developments, IEEE Design & Test, vol. 33, no.3, pp. 46-55, 2016


[5] S. Brand et al., Scanning acoustic gigahertz microscopy for  metrology applications in three-dimensional integration  technologies, J. Micro/Nanolith. MEMS MOEMS 13, pp. 1-10, 2014


[6] A. Phommahaxay et al., Defect detection in through silicon  vias by GHz scanning acoustic microscopy: key ultrasonic  characteristics. Proc. IEEE Electronic Comp. & Techn. Conference (ECTC), pp. 850-855, 2014


33


[7] A. Khaled et al. Study of GHz-SAM sensitivity to  delamination in BEOL layers. Microelectronics  Reliability, 76-77, pp. 238-242, 2017


[8] I. De Wolf et al., Detection of local Cu-to-Cu bonding  defects in wafer-to-wafer hybrid bonding using GHzSAM. Proc. 44th Int, Symp. For Testing and Failure  Analysis (ISTFA), pp. 8-11, 2018


[9] W. Yun et al., Advances in 3D interconnect  characterization techniques for fault isolation and defect  imaging, in Metrology and diagnostic techniques for  nanoelectronics. Ed. Z. Ma and D.G. Seiler, Pan Stanford  Publishing, 2017, pp. 1147-1274


34


Machine learning assisted signal analysis in Acoustic Microscopy for nondestructive defect identification


Signal processing and data interpretation in scanning acoustic  microscopy is often challenging and based on the subjective  decisions of the operator, making the defect classification  results prone to human error. The aim of this work was to  combine unsupervised and supervised machine learning  techniques for feature extraction and image segmentation that  allows automated classification and predictive failure analysis  on scanning acoustic microscopy (SAM) data. In the first part, conspicuous signal components of the time-domain echo  signals and their weighting matrices are extracted using  independent component analysis. The applicability was shown  by the assisted separation of signal patterns to intact and  defective bumps from a dataset of a CPU-device manufactured  in flip-chip technology. The high success-rate was verified by  physical cross-sectioning and high-resolution imaging. In the  second part, the before mentioned signal separation was  employed to generate a labeled dataset for training and finetuning of a classification model based on a one-dimensional  convolutional neural network. The learning model was  sensitive to critical features of the given task without human  intervention for classification between intact bumps, defective  bumps and background. This approach was evaluated on two  individual test samples that contained multiple defects in the  solder bumps and has been verified by physical inspection. The  verification of the classification model reached an accuracy of  more than 97% and was successfully applied to an unknown  sample which demonstrates the high potential of machinelearning concepts for further developments in assisted failure  analysis.


The trend for miniaturization in microelectronics remains  ongoing. While technological advancements aim at combining  increasing functionality and performance with reduced spatial  dimensions, the complexity of modern microelectronic  components highly challenge established methods of failure  analysis. For investigating defect signatures to uncover the  specifics of the root cause, non-destructively operating  techniques are of superior value for defect localization upon  which physical preparation and high-resolution analytics are  guided. The increased complexity, the shrunk feature  dimensions and the extent into the third spatial dimension  require appropriate adaptation of entrenched inspection  approaches and their parameters. Acoustic microscopy  inspection is widely accepted in quality assessment and failure  analysis, as it provides valuable information about sample


internals while operating fully non-destructive. Interpretation  of acoustic signals and images however, can be challenging, requiring comprehensive experience. The complexity of  interpreting acoustic data can be explained by the high  sensitivity of acoustic waves towards gradients in mechanical  and structural properties, resulting in rather complicated signals  that contain the full information about the interaction of the  acoustic wave with the sample under test. While the presence  of a large content of information can be disadvantageous for an  untrained operator, an algorithm that would be capable of  processing them in total would be highly beneficial for  supporting the necessary interpretation.


Recently, considerable progress has been made in the field of  machine learning, especially deep learning, which enables  algorithms to achieve high performances in combination of  multiple data sources in order to draw conclusions and make  decisions for classification upon trained knowledge. Inspection  techniques that easily produce a large amount of data containing  a high degree of information like the time-domain data in  acoustic microscopy are predestined for the application of deep  learning architectures to extract the required relevant  information and relate them to the device for defect localization  and characterization. An introduction of various computer  vision techniques and deep learning techniques in ultrasonic  imaging can be found in [1].


The current paper describes the application of machine learning  based algorithms onto time resolved echo signals obtained by  acoustic microscopy for the identification of defects in flip-chip  interconnects in two case studies.


In the first stage, unsupervised learning techniques using  independent component analysis (ICA) were performed to  extract the independent signal components and their weighting  matrices. The applicability of this signal analysis method was  evaluated for the identification of bump interconnects and the  characterization of these interconnects and the detection of  internal defects. Based on these results a segmentation of the  acoustic micrographs into intact and defective bumps was  performed and resulting maps are color-coded and  superimposed onto the acoustic image for a simplified visual  assessment. Validation of the results was obtained through  physical cross sectioning and scanning electron microscopy (SEM) imaging. The application of the ICA-based processing  approach is demonstrated in case study I analyzing the acoustic  data recorded from a CPU-device manufactured in flip-chip  technology. The herein obtained results are compared to the  ones of a previous investigation also addressing automated  inspection and classification as described in [2].


In the second stage, acoustic microscopy data and the  information from the before mentioned signal separation by  ICA was used to generate a labeled dataset for supervised


# Machine learning assisted signal analysis in Acoustic Microscopy for nondestructive defect identification


35


learning techniques. The data are employed for training of a  model that was based on a one-dimensional convolutional  neural network (1D-CNN) for the classification into bump, defective bump or background signals recorded from flip-chip  samples. After validation and verification by physical crosssectioning, the resulting model was used for the defect  classification of unknown datasets.


This 1D-CNN based method was evaluated and is described in  case study II analyzing two flip-chip samples containing  multiple defects in the solder bumps. The results obtained  illustrate that automated defect identification with high  accuracy can be reached through a suitable training data set  derived from even a single sample.


Materials and Methods


In the current paper two approaches of machine-learning based  classification were pursued. Firstly, to generate a suitable  training dataset for automated feature extraction, ICA [3] is  performed on the SAM data to extract signal patterns that are  potentially related to a defective behavior of the inspected  sample. By using the weighting factors of the independent  signal components, the dataset can be segmented and clustered  into defect and non-defect areas reducing the required manual  effort. This labeled dataset containing signals from the original  SAM data is further used to train and fine-tune a 1D-CNN to  acquire feature matrices without human interaction. As a result, the final classification-model will be able to perform an  automated classification of an unknown dataset for a given type  of sample. Choosing a different technique of feature extraction  for the training process than the prediction may lead to a  reduced sensitivity of the model towards noise and increases the  stability at a higher variance within the data.


Figure 1: Signal processing workflow. In the first step the SAM  signals are low-pass filtered and aligned to the entrance echo  of the sample surface. Feature extraction by ICA on the training  data allows segmentation and performing physical crosssectioning for verification and assignment to the corresponding  condition. The Labeled training data are used to train the 1DCNN. Finally, the test data of the unknown sample are used  directly as input data of the 1D-CNN model to complete the  feature extraction and classification.


Scanning Acoustic Microscopy


In the current study scanning acoustic microscopy (SAM) was  performed using two focused ultrasonic transducers operating  at 175 MHz and 230 MHz. The acoustic microscope consisted  of a 3-axis scanner and was equipped with a pulser-receiver unit (DPR 500, Imaginant Inc., Pittsford, NY, USA). For coupling  the acoustic signals into the sample, deionized and


degassed water was employed. During the scan process in C(t)-Mode, the acoustic echo signals at each position were sampled  and digitized at a sampling rate of 1 GS/s with a resolution of 8  bit. The resulting 3-dimensional data matrix was analyzed off  line using custom developed MATLAB code (The Mathworks, Nattick, MA, USA). For visual representation, micrographs  were computed from the backscatter amplitude integral (BAI) within a specified time range.


Feature extraction by ICA


Independent Component Analysis (ICA) is a method of  multivariate statistics for blind source separation as described  in [3]. It attempts to decompose independent components from  a mixture of statistically independent random variables. The  linear mixing model of an observed acoustic signal  ⃗ (  ) =  (  1(  ),   2(  ), … ,     (  ))   from    = 1                is  defined as:


 ⃗  =     


where A is the unknown mixing matrix and   (  ) =(  1(  ),   2(  ), … ,     (  ))  is the vector of n possible  independent components. The intent of this method is to obtain  a linear static transformation to convert the acoustic signal into  a vector of maximally independent components    measured by  a function F of independence. The model can then be rewritten  as:


   =    ⃗ 


(2)


where    =    −1 is the unmixing matrix that will be estimated  by the algorithm using numerical pseudo inverse techniques [3]. The independent sources can be the results of a nonlinear  process. Only the mixing process assumes linearity.


For the presented work, the Fast-ICA algorithm as described in


[4] was applied, it employs a gradient method to separate the  independent components by measuring the non-Gaussianity


ICASegmentation


after each iteration. The extracted components of the echo  signals that can be related to the sample structure are ignored


Input signal


(training data)Matrixfeaturedata


verification)Labeled trainingResults (physical


while signal anomalies attributable to potential defects are  selected for segmentation. Based on the concept of separating


Preprocessing


-Train / validate


the signals into components of different classes the  corresponding mixing matrices were binarized by thresholding


Input signal↓10CNN→(test data)MatrixFeature→ Classification


them to above the noise level of the algorithm in order to mark  the individual regions in the acoustic micrograph.


Additional image processing with morphological operations  was applied to reduce pixel noise in the mask. Finally, the mask  is superimposed onto the acoustic micrograph for visual  assessment of the potentially defective areas.


Classification by Convolutional Neural Networks


The attempt of this research was the creation and fine-tuning of  an artificial neural network based on the concept of a 1D-CNN  in order to perform automated feature extraction and  subsequent classification of the echo signals obtained by SAM.  A CNN is a particular type of multilayer perceptron (MLP) consisting of neurons with weights and biases that have to be  trained through the backpropagation method employing a  training dataset [5]. They are most commonly applied for  analyzing visual imagery. The intended application in the  current study is the analysis of time-domain signals that are


36


obtained in a one-dimensional form in which the samples are


The computation was implemented using the MATLAB Deep


arranged in sequential time steps.


Figure 5: Three independent components of the acoustic  signals recorded from a flip-chip device. Top: Component  characteristic of a defective flip-chip interconnect. Center: Component characteristic for defect-free bumps. Bottom: Component prominent in signals of the background.


decision mask is color coded and superimposed onto the   acoustic micrograph of an entire section of the chip for a


simplified visual assessment of the defective bumps. From this  graph it can be seen that artefacts occur which lead to the  presence of the independent signal component that is mainly  observed at locations of a defective bump, but also can be seen


around the rim of the device where no bumps are located. Bumps in Figure 6 marked with a yellow circle have been  confirmed to be defective by physical cross-sectioning and  SEM imaging.


For recording electron micrographs, the CPU device was  sequentially polished to the middle of each bump row. Figure 7  contains SEM micrographs of four defective flip-chip  interconnects that have been revealed when analyzing the  ultrasonic signals acquired by SAM. It can be seen that all of  the flip-chip contacts are fully or partially disconnected from  the substrate. The numbering in Figure 6 bottom corresponds to  the numbering in Figure 7. It should be noted that one falsenegative detection (bump# 2) occurred. However, the overall  success rate of this approach is still high.


Case study II


Based on the results of the ICA on sample #1, four independent  signal components have been identified that are related to  potential defects within the bumps. Furthermore, three  components were extracted that can be assigned to intact bumps  and two components that allow identifying background signals. In Figure 8 in the top left image, the raw map from the summed  weighting matrices of the four “defective” components is  shown, containing the proportion of the conspicuous signal  patterns with respect to the pixel intensity. By manual   thresholding, a binary mask was obtained that is superimposed


Figure 6: Results of the defect identification by ICA – analysis  from case study I. Top-Left: Weighting matrix of the component  that is characteristic for a defective bump. Top-Right: Classification mask derived from the weighting factors of the  defect-signature. Bottom: Classification mask (red) superimposed on the acoustic micrograph for simplified visual  assessment. Yellow circles indicate where defective FCcontacts were verified by cross-sectioning and SEM-imaging. SEM investigations were only performed on columns three and  four (counting from the right-side of the device) marked by  yellow arrows at the top.


onto the BAI micrograph in the top-right image of Figure 8. The  classification masks for identifying intact bumps and the  background as shown in the bottom images were derived  accordingly. Pixels in the map which cannot be related to one  of the three labels are marked as idle, since they are likely  related to artefacts. It is important to mention that the selection  of the components in the current section is still related to the  operator's experience. In case study I, defect classification is  only assisted by the extraction of the signal patterns employing  machine learning algorithms.


Cross-sectioning and optical microscopy was performed on the  three columns on the left of the sample and are presented in  Figure 9. The optical micrographs confirm the assumption that


39


Figure 7: Scanning electron micrographs of defective flip-chip  interconnects after physical cross-sectioning of the CPU-device  investigated in case study I. The numbering in the electron  micrographs correspond to the numbers in Figure 6 identifying  the bumps in the acoustic image.


multiple types of defects occurred in the sample. The two  micrographs at the top reveal dark shaped regions (in the orange  circle) indicating cracks in the interface Si-die/bump. In the  bottom micrographs, large voids can be noted that are likely  related to degassing mechanisms occurring during the process.


o


,


e


.


n


vp


Figure 8: Results of the signal classification by ICA in case


0.2


study II applied to sample #1. Top-Left: Weighting matrix of the  4 components that are characteristic for defects in bumps. TopRight: Binary classification mask (red) of bump defects


00500100015002000250030003500 40004500


superimposed onto the acoustic micrograph. Bottom-Left: Binary classification mask indicating intact bumps obtained by  ICA. Bottom-Right: Binary classification mask related to  background signals (underfill, etc.).


Figure 9: Optical micrographs after physical cross-sectioning  with defective regions in flip-chip interconnects of sample #1, marked in orange. The arrows point to the locations of the  defective spots in the acoustic micrograph onto which the  classification mask is superimposed (center). The red arrow  indicates a false positive detection obtained through ICA.


Table 1: Number of elements for all categories in the training, validation and test data set from sample #1


Defective  bumps


Intact  bumps


Background


Idle


Dataset


906


25418


69351


27233


Training 724


1600


Validation 91


~


Test


91


From the defects observed upon the physical analysis, the  corresponding marks in the map are verified to be defective  regions in the sample. In contrast, also one false-positive  marking occurred as seen in row three, column two in Figure 9. The optical micrograph reveals small defective regions at the  top of the bump that have not been marked because of the low  signal weight. The results of the physical analysis verified the  predominantly correct classification of the acoustic data based  on the machine learning approach.


In the following step the resulting labeled signal vectors were  split according to Table 1 and the model is trained using the  training and validation data set.


Iterations


Figure 10: Accuracy and cross-validation loss for the training  and validation calculated after each iteration of the training  phase of the final model for the first 4096 iterations.


Target Class


Figure 11: Confusion Matrix obtained from the test dataset with  each column representing the instances in the actual classes  and each row representing the output class from the model. The  diagonal elements represent the number of points for which the  predicted label is equal to the true label, while off-diagonal  elements are those that are mislabeled by the classifier.


The evolution of the training process for the first 4096 iterations  is shown in Figure 10. During the training, the model was   evaluated against the validation set every 30 iterations. There  was no indication for the model to overfit or underfit according  to the performance metrics of the dataset as can be seen from  Figure 10. In the case of overfitting the model would have a low  sensitivity to the validation data set while improving the  training accuracy. An underfitting model would result in an  overall low classification accuracy.


The trained model was evaluated against the test set reaching  an accuracy of 97% at a cross-entropy loss of 0.09. The output  of the test set is presented as confusion matrix in Figure 11. The  majority of the target classes is predicted correctly as can be  seen by the low values of the off-diagonal fields. The highest  deviations occur for intact bumps that are classified as defective  bump (false-negative). There are also misclassifications  between “idle” and “background”, which can be ignored for the


Figure 12: Results of the signal classification on sample #2. Left: Mask indicating the defective-bump class for each  position by likelihood. Right: Classification mask  superimposed with BAI acoustic micrograph (red: defective  bump, green: intact bump, blue: background, black: idle).


Confusion Matrix


|192|1||0.0%|1|99.0%|
|---|---|---|---|---|---|

|27.8%|0.1%||0.0%|0.1%|1.0%|

|4|90 13.0%|90 13.0%|0.0%|0.0%|95.7%|

|0.6%|90 13.0%|90 13.0%|0.0%|0.0%|4.3%|

|0|0||196|3|98.5%|

|0.0%|0.0%||28.4%|0.4%|1.5%|

|4 0.6%|0.0%|0.0%|4|196|96.1%|

|4 0.6%|0.0%|0.0%|0.6%|28.4%|3.9%|

|96.0%|98.9%|98.9%|98.0%|98.0%|97.5%|

|4.0%|1.1%|1.1%|2.0%|2.0%|2.5%|

intact bump


100um


100μm


background


Output Class


100 μm


idle


Figure 13: Optical micrographs after physical cross-sectioning  with marked defective regions (orange) in flip-chip  interconnects of sample #2. The arrows point to the location of  the defective spot on the acoustic micrograph superimposed


oundae


with classification mask in the center.


given task.


Automated signal classification by 1D-CNN has been  performed on the acoustic signals obtained through SAM from  test sample #2. The obtained results are shown in Figure 12. The graph on the left contains a map in which the probability of   a signal vector indicating a defective bump is color-coded in  yellow. Thresholding the resulting maps by a value above 0.7  for each class results in the mask on the right superimposed onto  the acoustic micrograph (the dark pixels represent the mask for  the class “idle”, which was hidden in favor of the visualization  of the acoustic micrograph).


For verification the three columns of bumps on the left of the  sample were cross-sectioned and inspected by optical  microscopy. The results of four selected bumps are shown in  Figure 13. The defects detected and marked in sample #2 show  the same characteristic in the ultrasonic signal as observed from  the physically confirmed defects in sample #1. Caused by  diffraction effects, the acoustic signals at the edges of the  bumps contain disturbances leading to false-negative  classification.


Almost all elements of the remaining classes that are not related  to defects are primarily classified correctly and allow  segmentation of the sample structure.


Summary and Conclusion


Scanning acoustic microscopy has been performed on flip-chip  devices for the acquisition of the unprocessed acoustic echo


0.9


signal data. Although acoustic waves are very effective when


0.8


used to analyze mechanical properties of materials, there are


0.7


cases where the echo signals contain a large amount of


0.6


information and the presence of a bump-crack may remain


0.5


unrecognized by conventional acoustic imaging algorithms. For


0.4


feature extraction, the acquired echo signals have been


0.3


subjected to an independent component analysis and several


signal components have been extracted. Subsequent parametric


0.1


imaging was performed employing the matrices of the  weighting factors of specific components which allowed  recognition of flip-chip interconnects from the entire acoustic  data set. Furthermore, the application of the weighting factors  of different components lead to the identification of defective  bumps. The method was evaluated by performing two case


41


studies on samples manufactured in flip-chip technology. Case  study I applied the developed method to the SAM dataset of a  CPU-device resulting in a high success rate for identifying  defective bumps. These bumps, as subsequent verification by  mechanical cross-sectioning and SEM or optical inspection  revealed, showed partial and complete disconnection from the  corresponding solder pad.


Besides the extraction of signal features for the purpose of pure  parametric imaging in SAM, the application of machine  learning algorithms appears highly promising for classification  with the aim at automated defect identification. Using the  acoustic signals acquired and the verification by physical  failure analysis a convolutional neural network was trained, fine-tuned and applied to an unknown data set. The complete  procedure was successfully tested on two test samples  consisting of daisy chains interconnected through SnAgCubumps. Therefore, one of the available samples was preanalyzed to generate a labeled dataset using the before  mentioned method of signal separation. On the second sample, automated classification based on the 1D-CNN was performed  and identified defects were also verified by physical crosssectioning. The results show excellent agreement with the  results of the automated classification. And thus appear highly  promising for further developments and applications to meet  the challenges of automated defect identification in more  complex packaging technologies.


[1]


Ye J, Ito S, Toyama N., Computerized Ultrasonic  Imaging Inspection: From Shallow to Deep Learning, Sensors (Basel) 2018, pp. 18(11):3820, 2018


[2]


S. Brand, P.Czurratis, P. Hofrogge, M. Petzold,  Automated inspection and classification of flip-chip  contacts using Scanning Acoustic Microscopy, Microelectronics Reliability, pp. 50(9):1469-1473, 2010


[3]


P. Comon, Independent component analysis, A new  concept?, Signal Processing Volume 36 Issue 3, pp. 287 – 314, 1994


[4]


A. Hyvärinen, Fast and Robust Fixed-Point  Algorithms for Independent Component Analysis, IEEE Transactions on Neural Networks, pp. 10(3):626-634, 1999


[5]


LeCun, Y., Bengio, Y. and Hinton, G., Deep  learning. Nature, 521(7553), pp.436-444, 2015


[6]


K. P. Murphy, Machine Learning: A Probabilistic  Perspective, MIT Press (Cambridge / Massachusetts, 2012), pp. 106 & 285 & 999-1010


[7]


I.T. Jolliffe, Principal Component Analysis, Springer  Verlag New York (New York, 2001), pp. 1-6 & 209-210 & 229-338


42


# Solder bump joint failure investigation: From sample preparation to advanced structural characterizations and strain measurement


Solder bump joint failure investigation: From sample preparation to advanced  structural characterizations and strain measurements


Pawel Nowakowski, Mary Ray, and Paul Fischione


E.A. Fischione Instruments, Inc., Export, PA, USA


This paper describes the detailed sample preparation  of a solder joint at the level between a  semiconductor package and board. Different sample  preparation techniques are described and compared. Preparing and targeting a large sample area  containing multiple solder bumps is discussed. The  sample preparation methods will then be confirmed  by advanced structural characterization and strain  measurement. The presence of strain is associated  with the development of cracks and delamination at  the solder joint interface.


The packaging technologies of microelectronic flip  chips involve solder joints that connect the chip and  board. To guarantee reliability of microelectronic  devices, the prediction of solder joint failures and  their early state detection is critical. Both leaded and  lead-free solder bumps are used as joints. Because  of constantly decreasing solder bump dimensions  and pitch, defect detection and investigation is  becoming more challenging. An accurate, reliable, and easy-to-use investigation technique is critical  for solder joint defect inspection in high density  microelectronic packaging [1-5].


One of the most critical failures of this joint is the  loss of connectivity between copper pads and solder  bumps, which appears in the form of cracks or  delamination. These defects result from joint  microstructural evolution induced by constant or  cyclic loading conditions during device service. The  strain accumulated at the interface between solder  bump and copper pad can lead to joint failure. Therefore, an understanding of the joint structure  evolution and knowledge about the strain state at  the joint interface can provide insight into the  failure mechanism and prevent it in the future.


43


A solder joint is typically made of a Sn-based alloy (solder material), an intermetallic compound at the  joint interface, and copper pad. Tin is a very soft  and ductile material that can be very easily  deformed, i.e., any exterior intervention to the joint  can lead to structural change. For that reason, preparation of solder bump samples is typically a  delicate and potentially complex process. Any  mechanical action, such as cutting, grinding, and  polishing, can provoke structural changes and  introduce strain at the joint interface that leads to  cracks and delamination. A sample preparation  technique that preserves the native state of the joint  structure without introducing any artifacts is  necessary to fully understand the failure mechanism. In this paper, we first look for an appropriate sample  preparation technique that allows the preservation  of the solder joint’s native state. Second, we  concentrate on structural characterization and strain  measurement at the joint interface.


|To |illustrate our |unique solder |bump |
|---|---|---|---|

|characterization |approach, |we |consider two |

|samples:|samples: |||

• Device #1: A chip package with solder bumps ready to be installed on the board(Figure 1).


• Device #2: A chip package already installed on the board, which was extracted from a commercially available “smart” phone(Figure 2).


Two sample preparation techniques are considered  for comparison purposes: Mechanical polishing (MP) and argon broad ion beam milling (BIB).


Figure 1. Cross-section image of a chip package with solder  bumps ready to be put on a board. The cross-section sample  was created by argon BIB milling. Back-scattered electron (BSE) contrast image of seven bumps on the package (a) and  EDS overlay maps of Cu, Sn, O, and Si (b).


Figure 2. Cross-section image of a chip package connected to  a board. The cross-section sample was created by argon BIB  milling. BSE contrast image of four bumps located between  the package and board (a) and EDS overlay maps of Cu, Sn, O, and Si (b).


Sample preparation


Two sample preparation techniques were used: MP  and argon BIB milling. The MP technique consists  of polishing using abrasives. The sample was  polished using #800- and #1200-grade SiC papers (for 3 minutes or less per paper grade). The sample  was then polished using 3, 1, and 0.5 µm diamond  particles in oil suspension; the polishing times  increased from 5 to 15 minutes as the particle size  decreased. The last step of the MP process was  colloidal silica (0.05 µm particles) polishing for  2 hours. The total MP time, including cleaning  could take up to 4 hours. In contrast, the BIB  technique required only 20 minutes to 1 hour of  processing depending on sample surface finished  prior to the process.


The BIB technique consists of material removal (polishing) by action of argon ions accelerated to a  user-specified energy between 0.1 eV to 10 keV.


The ions form a beam with a user-specified beam  current value. The process is commonly known as  ion milling. In this manuscript, all samples, after  MP process, and prior to ion milling, were  repolished using 1 µm and 0.5 µm diamond pastes. The following ion milling conditions were used:


• Beam energy: 6 keV for 20 minutes, followed by 4 keV for 40 minutes.


• Beam angle: 3° (grazing angle).


• Stage cooling: Because of tin solder bump  thermal sensitivity, liquid nitrogen was used  to cool the ion mill’s sample stage to -150 °C during milling.


MP (Figure 3a) and BIB milling (Figure 3b) scanning electron microscopy (SEM) observations  show that results of each technique appear to be


500μm


similar. However, sample surface cleaning after MP (colloidal silica suspension) was very difficult. The  SiO2 particles stuck to the sample surface and were  very difficult to remove. Attempts to remove the  particles led to the introduction of scratches on the  soft tin and copper that damaged the joint interface. In addition, the use of water for cleaning provoked  corrosion of different package components and  made the polishing and cleaning process very  complex.


package  board


Package


44


Figure 3. BSE contrast image of solder joints after mechanical  polishing (a) and after argon BIB milling (b).


Sample preparation technique evaluation


Electron backscatter diffraction (EBSD) was used to  perform structural characterization; high resolution  EBSD (HR-EBSD) was used to perform strain  measurements. Figure 4 shows EBSD analyses of  the solder bumps prepared by MP and argon BIB  milling. In the MP sample, the area close to the joint  interface (Figure 4a, yellow square) cannot be  analyzed by the EBSD technique. The copper pad  caused a shadowing effect due to the difference in  material removal during mechanical polishing. In  addition, corrosion product from package  components contaminated (Figure 4a, green  squares) the area of interest; these areas also cannot  be analyzed by the EBSD technique. In contrast, the  sample prepared by argon BIB milling (Figure 4b) produced excellent quality EBSD patterns – the  entire tin bump and the copper pad (including the  joint interface) were visualized. From such highquality sample preparation, accurate microstructural  analyses and strain localization and measurements  were possible. Figure 4 shows the grain structure, size, and crystallographic orientation of the tin  bump and the copper pads.


Figure 4. EBSD inverse pole figure (IPF) orientation maps  overlaid on band contrast maps collected from solder joints  after: (a) mechanical polishing ( yellow square indicates that  the solder bump is shadowed by the copper pad; green  squares indicate areas where corrosion product from  packaging components redeposited onto the area of interest); and (b) after argon BIB milling.


Strain measurements results and discussion


The strains were first localized using local  misorientation measurement from the EBSD data (Figure 5). Next, the strains were measured by  HR-EBSD technique [6-9] (Figures 6 and 7). Only  the argon BIB milled samples were of high enough  quality to undergo strain evaluation investigation.  Figure 5 clearly shows a difference in the strain  present in the sample of the device package not  connected to a board (Figure 5a) and a device  package connected to a board (Figure 5b). Strain  evaluated from local misorientation measurements  clearly show an absence of deformation in device 1 (Figure 5a). In contrast, device #2 shows strain  accumulated at the interface of the solder bump and  copper pad (Figure 5b, red square) and at the area  between the solder bump void and copper pad (Figure 5b, black square). In these two areas, there  is a high probability for failures (cracks or  delamination) to occur.


100 µm


50 µm  50 µm


45


Figure 5. Strain contouring EBSD map of a solder joint after  argon BIB milling: a) device #1 not connected to a board; b) device #2 connected to a board. Strain accumulated at the  interface of the solder bump and copper pad (b, red square) and at the area between the solder bump void and copper pad (b, black square).


HR-EBSD measurements were carried out at this  early state of deformation, which preceded the  appearance of cracks or delamination. Figure 6  shows the average total effective strain measured by  HR-EBSD analyses. Total average effective strain  for device #1 was of 10-3 order of magnitude (Figure 6a), while for device #2, the effective strain  was much higher: 10-2 order of magnitude (Figure  6b). The accumulation of strain is clearly observed  in the solder bump area close to the copper pad (Figure 6b).


Figure 6. Average total effective strain from HR-EBSD  measurements for device #1 (a) and device #2 (b).


To better understand how strain accumulated and  the deformation process, we investigated strain


fields obtained for principal strain components εxx, εyy, and εzz (Figures 7 and 8). The results show  average elastic strain is lower by up to two orders of  magnitude between device #1 and device #2. For  device #1 (Figure 7), strain was uniformly  distributed around the zero value of the scale (x10-5  magnitude order). In contrast, device #2 (Figure 8) strain was primarily localized at the solder  bump/copper pad interface. High positive strain  present in a normal (εzz) direction, a compressed (negative) strain in the horizontal (εxx) direction, and mixed strain in the transverse (εyy) direction  were observed (Figure 8). This indicates that  complex loading conditions acted on the solder  bump between the package substrate on the one side  and the board on the other side.


rw


56371791242


Figure 7. Device #1 HR-EBSD strain field obtained for  principal strain components: εxx, εyy, and εzz.


b.a6


Figure 8. Device #2 HR-EBSD strain field obtained for  principal strain components: εxx, εyy, and εzz.


Conclusion


A comparison of sample preparation methods for  solder bump failure investigation was presented. The argon BIB milling was found superior to MP  because argon BIB milling because it did not


50 µm


Average total strain: 6 x10-3


Average total strain: 5 x10-2


εxx average 2.2 x10-5


εyy average -9.8 x10-5


εzz average -2.6 x10-4


εxx average -9.5 x10-3


εyy average -1.3 x10-3


εzz average 7.3 x10-3


46


introduce additional mechanical stress or defects to  the sample.


In addition, argon BIB milling allowed accurate  structure and microstructure investigation of the  solder junction, which included advanced strain  quantification.


The presence of strain is associated with the  development of cracks and delamination at the  solder joint interface; understanding the strain  characteristics is the first step toward understanding  the failure mechanism and, ultimately, how to  prevent these types of failures in the future.


[1] Liu, A. et al. (2011). Characterization of fine-pitch  solder bump joint and package warpage for low K  high-pin-count flip-chip BGA through shadow moiré  and micro moiré techniques. In 2011 IEEE 61st  Electronic Components and Technology Conference (ECTC) (pp. 431-440). Lake Buena Vista, FL: IEEE.


[2] Fan, M. et al. (2016). Defect inspection of solder  bumps using the scanning acoustic microscopy and  fuzzy SVM algorithm. Microelectronics Reliability, 65, 192-197. doi:10.1016/j.microrel.2016.08.01


[3] Kang, S. K., Gruber, P., and Shih, D. (2008). An  overview of Pb-free, flip-chip wafer-bumping  technologies. JOM, 60(6), 66-70.


[4] Mercado, L. et al. (2003). Analysis of flip-chip  packaging challenges on copper/low-k interconnects. IEEE Transactions on Device and Materials  Reliability, 3(4), 111-118.


[5] Mallik, D. et al. (2005). Advanced package  technologies for high-performance systems. Intel  Technology Journal, 09(04), 259-271.


[6] K.Z. Troost, et al., (1993). Microscale elastic strain  determination by backscatter Kikuchi diffraction in  the scanning electron microscope. Applied Physics  Letters 62 (10), 1110-1112.


Due to the contrast variations caused by the surface roughness


#1


Figure 5 contains the results of the independent component  analysis. The parametric images in all three rows in the left  column show the maps of the weighting factors with which the  individual component, displayed in the diagram to the right, was contained in the acoustic time-domain signal. The upper  row shows the component that has been found to be  characteristic for defective flip-chip interconnects showing  higher reflection characteristics in time ranges after the pulse is


400 µm


transmitted into the bump structure.


In the vertical center the component corresponding to possibly


#2


intact bumps is shown, while in the bottom row the component  representing the background in the acoustic micrograph is  plotted.


The correlation between the signal components for defective  and intact flip-chip connects was obtained through validation  by physical preparation and SEM imaging of two rows of  bumps indicated by the yellow arrows in Figure 6. While Figure  5 contains the weighting matrix of selected bumps, Figure 6


shows the distribution of the weighting factors for an entire  section of the flip-chip device. The graph on the top left (in


Figure 4: Left: Acoustic micrograph (C-Scan) computed from


Figure 6) shows the raw values of the weighting factors. In the


the BAI in a specified time gate. The red line indicates the


top right graph, the decision map is shown which was derived


location of the B-Scan evaluation for sample #1 (Top) and


from the weighting factors by low-pass filtering and


sample #2 (Bottom). Right: Acoustic cross-section image (Bthresholding. All yellow colored pixels correspond to the


Scan) of sample #1 (Top) and sample #2 (Bottom) with the timeclassification as a “defective bump”. In the bottom image the


domain in vertical direction and the lateral expansion in  horizontal orientation.


38


component identifying defect


apridue[yu]


-009


100150200


ocudoueuji peuju6u ou-pejapg niud


['vu] epngdue-0'09


SO


100190 gwo] us[


V0.02。


√NNW、mN


、


at-0.02


"


-0.04


050100150200


h


心


ooudouauyp aujj/uBo epx6uxnup


0一wV 009


time [ns]


mnive bump


[7] A. Wilkinson, et al., (1996). Measurement of elastic  strains and small lattice rotations using electron back  scatter diffraction. Ultramicroscopy 62, 237-247.


[8] A. Wilkinson, et al., (2006). High-resolution elastic  strain measurement from electron backscatter  diffraction patterns: new levels of sensitivity. Ultramicroscopy 106 307-313.


[9] T.B. Britton, et al., (2011). Measurement of residual  elastic strain and lattice rotations with high resolution  electron backscatter diffraction. Ultramicroscopy  111(8) 1395-1404.


47


The Development of an EVB Socket Solution for  Automotive Mixed-Signal ICs


Eric Cattey, Alex Van Vianen, Mitch Curiel, Gustav Huo


NXP Semiconductors, Chandler, Arizona


Kristofor Dickson, Yvette Meiche


NXP Semiconductors, Austin, Texas


Failure analysis on mixed-signal ICs for automotive  applications often requires the use of EVBs (evaluation boards) to replicate the failure mode. Typically, automotive ICs are  used in conjunction with other components to create automotive  modules, such as; PCM (power-train control modules), ECU (engine control units), TCU (transmission control units), etc. EVBs are used to replicate module level functionality, as well  as reproduce ATE (automatic test equipment) tests required for  analysis. An integral part of EVB design, functionality and  performance is related to the IC socket, which is the direct  interface between the IC and the EVB. See Figure 1. EVB  socket solutions will vary based on the required analysis (backside / topside analysis), package type and IC functionality.


Figure 1: Automotive Mixed-Signal EVB. A backside socket  solution is highlighted in white.


The premise of this paper is the development of an EVB socket  solution for QFN (quad flat no-leads) PMICs (power  management ICs) that use an EP (exposed pad) as the primary  ground connection. The original socket solution had  insufficient ground connections to the EP, which consequently  created noise and instability in the ground plane preventing  comprehensive failure analysis. A new EVB socket solution  was developed to mitigate this problem. The new solution  provides more robust ground connections, thereby improving  device functionality and stability during analysis.


This paper will discuss specific FA challenges for QFN PMIC  devices, the deficiencies in the original EVB socket setup, new  socket solution development, sample preparation and electrical  data supporting proof of concept. This solution can potentially  be fanned out to other products with similar ground instability  issues.


FA Challenges for QFN PMIC Devices


PMICs typically have multiple high current switcher power  FET arrays which use down-bonds to connect the grounds to  the EP. Figure 2 shows an x-ray image of a QFN PMIC with  down-bond connections.


Figure 2: X-ray image of a QFN PMIC showing ground  down-bonds to the EP (red arrows). The ground connections  are critical for IC functionality and performance.


Multiple switcher FETs can consume significant current  making a robust ground connection important. One of the  primary challenges when analyzing QFN PMICs is the  retention of the ground down-bonds during sample preparation  for backside fault isolation.


EP


↑↑↑↑


NO VRISSIO FA DOAAD IEY


# The Development of an EVB Socket Solution for Automotive Mixed-Signal ICs


48


The typical process for backside analysis requires the removal  of the EP to access the back of the die, which consequently loses  the ground connections making the IC non-functional. To  mitigate this issue, a specialized backside sample preparation  technique was implemented. This is discussed further in the  sample preparation section of this paper. Other FA challenges  related to QFN PMICs include optimal working distance for  backside fault isolation, especially when utilizing a SIL (solid  immersion lens), copper wire bonding and atypical bonding  configurations.


Deficiencies in Original EVB Socket Setup


The need to develop a more robust socket solution stemmed


from both physical and electrical deficiencies in the previous )socket solution. A physical limitation of the socket was the


thickness of the plastic lid and interposer design, which


contributed to an overall working distance of ~3mm between


the top of the socket lid and the backside of the die. This


configuration was not conducive for use with a SIL.  The


260HV


electrical deficiencies, which were the primary motivation for


2015


redesigning the socket, were excessive ground noise and  inadequate current consumption capabilities which affected IC  functionality during failure analysis. The ground noise and  current consumption limitation were a direct consequence of  inadequate ground connections and inherent parasitic  inductance and resistance within the socket. An additional  deficiency in the original socket was the loss of ground  connections when the EP was milled away for backside  analysis. Figure 3 shows an image of the original socket  solution.


I5OOV82.60V创D500ms


190V


Figure 3: QFN socket with interposer design and limited


2perk-Fork


ground connections to the EP.


The previous solution used an interposer and pogo pins to route  the signals from the IC to the EVB. The interposer and  relatively long pogo pins created parasitic inductances which  significantly affected IC functionality and current consumption.


Figure 4 shows an oscilloscope plot measuring 1.32V of peakto-peak IC ground plane noise on the EVB during device  power-up using the original socket solution. The excessive  ground noise resulted in intermittent loss of IC communication, consequently causing logic resets to occur preventing  comprehensive failure analysis.


Figure 4: Oscilloscope plot showing the IC ground plane  noise of an EVB using the original socket solution. A peak-topeak noise voltage measurement of 1.32V was measured  during device power-up.


Figure 5 shows an oscilloscope plot for an EVB with the  original socket solution during an IC power-up sequence. When  the VDDOTP signal toggles low, the VPRE, BUCK1 and  BOOST regulators should turn on. As shown in the plot, the  regulators are unable to turn on (toggle high). This was  diagnosed as inadequate ground connections from the IC to the  EVB which consequently limited the current consumption  ability of the IC.


Stor


Figure 5: Oscilloscope plot showing the power-up sequence of  a PMIC with an EVB using the original socket solution. The  VPRE, BUCK1 and BOOST regulators are unable to turn on


due to inadequate ground connections within the socket.


DVPRH


DBUCKI


DVDDOTP


0DOST


。5.0205-2S7.mV


03.0195


A280.0nsA80.47mv-177.DaV


ground noise 1.32V pp


VPRE, BUCK1 and BOOST regulators should turn on when VDDOTP toggles low


49


Because of these deficiencies in the previous EVB socket  solution, a new solution was developed to mitigate the issues  and enable comprehensive failure analysis on QFN PMICs.


New Socket Solution Development


A new socket solution was developed to address the ground  noise and current consumption limitations. One of the primary  goals was to enhance the robustness and stability of the ground  plane by adding additional ground connections between the IC  and the EVB. The challenge however was to incorporate the  physical ground connections while at the same time optimizing


the socket’s working distance for backside fault isolation,


particularly for use with a SIL. The physical challenge for QFN  packages is that access to the backside of the die needed for  fault isolation is on the same side where the socket contacts are  located. This means that the package must sit upside down with  the signals from the contacts inverted and routed downwards to  the EVB. See Figure 6.


Figure 6: Cartoon of original socket solution showing


interposer inversion needed for backside analysis.


The novel socket presented here addresses the need to remove  the EP and preserve the ground connections. As with the  interposer socket, the QFN package goes in an inverted


Lid


position; however, connections are not made to the package


leadframe


Leadframe


leads but to the lead frame fingers (LFF) of the package.  Mold


QFN Package


compound around the edge of the package is lased out to expose


Socket


the LFF. Pogo connections are made to the LFF. Refer to Figure


7. Although the EP needs to be partially milled out, the ground


PCB


connections are preserved because the remaining EP in the lead  frame has corner fingers that extend all the way to the edge of  the package. The socket is designed to include connections to  these corner fingers. Furthermore, this socket is SIL compatible  for large QFN packages. See Figure 8.


Figure 7: Top view of QFN device after lase showing the lead  frame fingers.


Figure 8: New socket solution.


Sample Preparation


This section of the paper describes the sample preparation  needed to prepare a QFN PMIC device for analysis with the  new socket solution. To preserve the ground down-bonds, an  Allied High Tech X-Prep milling process was developed to mill  the EP for backside analysis, without disturbing the down-bond  wires.  Sample images before and after milling are shown in  Figure 9.   An x-ray image of the milled device is also shown in  Figure 10 showing the preserved down-bond wires.


Interposer


Inteposer


Die QFN Package


Figure 9: QFN device before and after EP mill to expose the  backside of the die while retaining down-bond connections to  the EP.


Figure 10: X-ray of QFN device after EP mill showing the  preserved down-bond connections to the EP (red arrows).


Next, a laser process was developed to expose the lead frame  leads for the new socket solution. Mold compound was  removed over the periphery of the package as shown in Figures  7 & 11.


Figure 11: Side view of QFN device after lase showing the  exposed lead frame leads.


Frontside analysis such as microprobing can also be performed  after backside fill and topside decapsulation. See frontside  image, Figure 12.


Figure 12: Top view of QFN device after chemical  decapsulation showing the exposed die.


Electrical Data Supporting Proof of Concept


After overcoming the sample preparation challenges and  implementing the redesigned socket solution on the EVB, bench testing was performed to validate functionality. Figure  13 shows an oscilloscope plot measuring 0.65V peak-to-peak  of IC ground plane noise on the EVB during device power-up  using the new socket solution. The ground noise improved from


↑↑↑


1.32V peak-to-peak to 0.65V peak-to-peak and the IC no longer  loses communication due to logic resets from the ground noise.


0000


Backside of die


51


Figure 13: Oscilloscope plot showing the ground plane noise  of an EVB using the new socket solution. The peak to peak  voltage noise improved from 1.32V peak-to-peak to 0.65V  peak-to-peak using the new socket solution.


Figure 14 shows an oscilloscope plot of the IC power-up  sequence using the new socket solution. With the previous  socket solution shown in Figure 5, the VPRE, BUCK1 and  BOOST regulators were unable to turn-on due to inadequate  grounding. With the new socket solution, all three regulators  are able to turn-on correctly without issue.


CS.00V②


valus2.60V


Pek-peakd273m1519UXO 100


3.0V


Figure 14: Oscilloscope plot showing the power-up sequence  of a PMIC with an EVB using the new socket solution. The  VPRE, BUCK1 and BOOST regulators are now able to turn  on and function correctly.


In summary, this paper discussed specific FA challenges for  QFN PMIC devices, the deficiencies in an original EVB socket  setup, new socket solution development, sample preparation  and electrical data supporting proof of concept. This solution  can potentially be fanned out to other products with similar  ground instability issues.


Acknowledgement


The authors would like to thank Delia Leung and Rose Stone  from the Product Diagnostic Center Lab for their efforts and


200mW


Min


peak-peak


3989.000元0pn


4o


contributions which helped enable this work.


ground noise 0.65Vpp


08.020ms


③8.019ms-37.50mVA780.3nsD39.84mV-27.34mV


VPRE, BUCK1 and BOOST regulators now turn-on correctly when VDDOTP toggles low


VEBI


UCX


DOST


52


ToF-SIMS, Time-of-Flight Secondary Ion Mass Spectroscopy for counterfeit


detection of Electrical, Electronic, and Electromechanical (EEE) parts.


1.MuAnalysis, Ottawa, ON


2.ION-TOF USA, Chestnut Ridge, NY


3.Tascon USA, Chestnut Ridge, NY


4.Tascon GmbH, Muenster, Germany


martine@muanalysis.com


ABSTRACT


This presentation demonstrates how Time-of-Flight  Secondary Ion Mass Spectroscopy provides unique  information to identify suspect counterfeit semiconductor  devices. An example is shown where the epitaxial layers of  a light emitting device (LED) do not match those of the  exemplar.


Keywords: Secondary Ion Mass Spectroscopy, SIMS, counterfeit detection, LED, Light emitting diode.


INTRODUCTION


This work is done in part for the SAE G19A committee. A  series of test method documents are being prepared to  complement the AS6171 standard [1]. One such document  is SAE AS6171/13. Technique for Suspect/Counterfeit  EEE Parts Detection by Secondary Ion Mass Spectroscopy (SIMS) Test Methods. [2].  The aim of the document is to  provide guidance for those using this technique for  counterfeit detection.


TIME-OF-FLIGHT SECONDARY ION MASS  SPECTROMETRY


Time-of-Flight Secondary Ion Mass Spectrometry (ToFSIMS) is an analytical technique that uses ion beams to  obtain the chemical composition of the outer surface region  of a sample. The technique can be used in two ways: Firstly  in a psuedo non-destructive mode called Static SIMS  where the composition is determined from the first 1-2  monolayers of a sample, and secondly in Dynamic SIMS  mode, in which the sample is eroded during the analysis  and the composition is determined over a larger depth, up  to several tens of microns.


A focused primary ion beam is rastered across the surface  of interest which causes material to be ejected from this  area. The portion of the ejected material that is ionized, known as secondary ions, is then extracted in to the  spectrometer where they are sorted by mass and counted. Atypical mass spectra will range from mass one to several


53


hundred amu but the mass range can be extended up to  approximately 10,000 amu as needed. This allows for the  analysis of elements, fragments and full molecules in  certain cases. Generally, for every analysis a single polarity (positive or negative) must be chosen, so in order to obtain  as much information as possible at least two analyses are  required. It is however possible to obtain both positive and  negative information in a single analysis by utilizing the  MCs+ mode of depth profiling. [3,4] This is particularly  useful for samples where only a limited area is available for  analysis.


In ToF-SIMS a full mass spectrum is taken at every pixel  meaning that the analyst does not necessarily need to know  what masses are of interest before starting the experiment. It also means that the data can be re-evaluated for all  elements at a later time without having to analyze the  sample again. However, for practical reasons a prior  knowledge of the sample will aid in experimental design  and analysis. This static SIMS spectrometry is useful for  identifying packaging differences in suspected counterfeit  parts.


By utilizing this mass spectrum at every pixel feature, it is  possible to acquire SIMS images (chemical maps) for any  of the masses present in the spectra. These images are ideal  for determining sample homogeneity and images with  lateral resolutions of sub-100nm are possible.


SIMS depth profiles show the change in chemistry as the  sample is probed from the surface in to the bulk. In ToFSIMS this is usually performed in the dual beam mode  where an appropriate ion beam is used for the sputtering  and an independent higher energy ion beam is used for the  analysis cycle.


By combining imaging SIMS with depth profiling SIMS, it  is possible to obtain 3-dimensional SIMS images that allow  one to see the distribution of elements/compounds with the  sample volume.


Figure 1.  A typical ToF-SIMS instrument


THE SAMPLES


This paper presents a case study involving after-market  replacement H4 light bulbs with LED devices.  The product  packaging makes several claims, several of which are not  met, including the type of LEDs used [5].


Figure 2. Parts used in this study.


This product was chosen because the type of LEDs is  clearly identified as Lumileds ZES emitters. Yet the photo  of the LED is a flipped image of the Lumileds Luxeon Z  photo available on the Lumileds website, which is an  earlier version of the product. This the first indication that  the LEDs used might not be ZES.


Figure 3. Product image and Luxeon Z image


At first glance, the LED emitters in the product do look like  Lumileds devices but there are significant differences. The  size of the protection diode is different and the pattern of  vias, visible through the phosphor layer is also different.


Figure 4. Left: product LED still soldered to the circuitry,


X3HEADLIGHTLED180093


right: a genuine ZES to be used as exemplar, purchased


LUMILEDS


from an authorized distributor and positioned beside the  suspect LED.


360°出


IP67 BAJERPROON


Free DiY withkinds colorful tim


Golden ligteCool WhiteLight Blue


50W 6000LM ZES 20G LIGHT SOURCE


Figure 5. Side views after the suspect part was desoldered. Top: suspect LED, bottom: exemplar ZES LED.


The difference in the pattern of the vias is more evident  once the phosphor layer is removed. Although all three


54


LEDs are in flip chip configuration, X-Ray imaging reveals  differences in packaging. The ZES shows a pattern of  bumps, absent from the suspect part. In SEM imaging, it is  clear that the suspect part still has the growth sapphire layer  attached, while it is absent from the Luxeon.


WD21


27-APRFigure 6. Parts after phosphor removal: Top: suspect part, middle: Luxeon ZES, bottom: Luxeon Z.


Figure 7. XRAY images. Left: suspect LED, right: exemplar ZES LED.  Since the suspect part was  desoldered, there is solder residue casting a dark shadow  on the part. No bump array is seen in the suspect part.


20.0kvx50060


Figure 8. Corner of the die of suspect part. Most of the die  is the sapphire substrate. The GaN layer is the thin lighter  color layer.


27-APR.


@kV(x500


Figure 9. Corner of the die of the ZES. The sapphire is not  present. The thin patterned GaN layer is surrounded by the  underfill that is present between the bumps.


Although there are significant differences in construction  between the LEDs used in the product and genuine LEDs  purchased separately from an authorized distributor, it is  still possible that the product LED die is authentic yet  mounted in a different package. The morphological  information obtained to date may not be enough if the  dispute went to court. SIMS depth profiling is the  technique of choice to characterize the epitaxial layers and  dopant profiles of semiconductor devices.


Sapphire


GaN


55


SAMPLE PREPARATION FOR SIMS


To prepare the samples for SIMS analysis, it is important  to understand their geometry and material systems.  Both  devices are in flip-chip orientation which means that the  active region is facing the substrate.


Figure 10. Interface between the GaN layer and the  package in the suspect part. The die is soldered to the  package traces and the anode and cathode regions are  connected to the traces by a series of redistribution layers  containing several metals and dielectric. The active region  of the LED is in contact with the top redistribution layer. The package, solder and redistribution layers must be  removed for SIMS, exposing the active region.


Figure 11. Interface between the GaN layer and the  package in the Luxeon Z. The ZES is very similar.  For this  cross-section, the phosphor layer was left on the part and  most of the package was ground away. There is no sapphire  on the GaN and it is thin (7µm) but because the surface of  the GaN in contact with the phosphor layer is rough and  patterned, SIMS cannot be done from this direction. The  package and redistribution layers must be removed.


Figure 12. After sample preparation, the metals will be


9-MAY-18


gone, leaving only the GaN layers and vias to n-GaN.


Figure 13.  Suspect device after sample preparation. SIMS  analysis is to be done within the clear areas.


Figure 14. Exemplar ZES device after sample preparation  and one attempt at SIMS.


EXPERIMENTAL


All SIMS experiments in this study were performed using  a TOF.SIMS 5 (IONTOF GmbH, Münster, Germany) instrument equipped with a bismuth liquid metal ion gun (30 keV), a dual-beam column sputter gun with Cs and Xe  ion sources (200 eV – 2 keV), an Ar gas cluster ion beam (20 keV) and an Extended Dynamic Range (EDR) analyzer. All ion beams have a 45˚ angle of incidence. Depth profiles were acquired in the dual beam MCs+ mode


WD20


6.79 μm


6.68 μm


Ni plating


Cu trace 20.0kv x3.0ak''ie:o''m Redistribution


layers   Solder


8.855μm7.290μm


WD19


2-AUG-13 Phosphor layer


0.763μm


10 839μml


Redistribution  layers


n-GaN


p-GaN


MQW


56


utilizing 15 keV Bi+ ions as the analysis beam and a Cs+


sputter beam (2 keV, 1 keV and 500 eV). Crater depth


measurements were performed with a Sensofar ply neox


optical profiler.


RESULTS


The 2 keV CsM+ ToF-SIMS depth profiles acquired from


the suspect part are shown in figures 15 and 16. The profile


confirms the presence of Al+, Ga +, and In+ matrix elements,


two Al+ layers and a series of complex In-rich multilayer


quantum well structures.


Figure 15. 2 keV MCs+ SIMS depth profile of the


suspected counterfeit part for the total range (approx. edsa 7µm).


Figure 16. 2 keV MCs+ SIMS depth profile of the


suspected counterfeit part showing the first approximately


400nm.


The MCs+ ToF-SIMS depth profile acquired from the 2013


Luxeon Z LED is shown in figures 17 and 18. These depth


profiles confirms the presence of Al+, Ga+, and In+ matrix


elements. However, this sample also has a SiO+ and Ti+


overlayer.


Figure 17. 2 keV MCs+ SIMS total depth profile of the


2013 Luxeon Z LED.


Figure 18. 2 keV MCs+ SIMS depth profile of the 2013  Luxeon Z LED. This profile shows the first third of the data  points.


The 2 keV MCs+ ToF-SIMS depth profile acquired from  the 2018 Luxeon ZES LED is shown in figures 19 and 20. These depth profiles confirm the presence of Al+, Ga+, and  In+ matrix elements and two Al+ layers. However, unlike


W


the suspected counterfeit LED, the complex In-rich  multilayer structures are missing.


Figure 19. 2 keV MCs+ SIMS depth profile of the 2018  Luxeon ZES LED. Total crater depth was measured as 7.7 µm by optical profilometry.


57


-1 10


Depth [nm]


5000


3000


1000


m


Al+


CsIn+CsSi2N+


-


CsGa+Mg+


CsSi+CsGaN+


File: A20272


Sample: Couterfeit LED


360


320


280


240


160


120


80


CsIn+CsSi2N+CsGa+Mg+


Data Point [#]


2800


2400


1200


800


400


Mg+


Cs2GaN+CsIn+


SiOCs+CsSi2N+CsGa+CsSi+


File: A20269


Sample: 2018 Luxeon ZES


Figure 20. 2 keV MCs+ SIMS depth profile of the 2018  Luxeon ZES LED (first 250 data points).


It was hypothesized that the multilayer quantum well layers  are thinner on the 2018 Luxeon ZES LED sample than on  the suspected counterfeit LED, so further depth profiles  were acquired using 500 eV Cs. The resulting profile is  shown in figure 21.


Figure 21. 500 eV MCs+ SIMS depth profile of the 2018  Luxeon ZES LED.


As can be seen in figure 21 the quantum well structure is  still not well defined. Using TOF-SIMS’s unique  retrospective analysis capabilities it is possible to view the  three-dimensional data set (figure 22) and this confirmed  the roughness of the sample. This can also be seen in the  XZ/YZ slices shown in figure 23.


58


Figure 22. 3D reconstruction of the CsIn+ signal from the  500 eV MCs+ SIMS depth profile of the 2018 Luxeon


ZES LED.


Figure 23. XY, XZ and YZ slices showing the CsIn+ signal  from the 500 eV MCs+ SIMS depth profile of the 2018  Luxeon ZES LED.


As sample roughness can affect both the mass and depth  resolution in SIMS experiments the data was reconstructed  from a smaller (less rough) area of the original data set. Again, due to the retrospective analysis capabilities of the  technique no additional data had to be acquired for this  depth profile.


Once the data was reconstructed from the smaller area (figure 24) the quantum well structure could be seen and  optical profilometry was performed to confirm the depth of  the sputter crater.


220


180


140


1400


600


3 10


2 10


1 10


0 10


Al+CsIn+


File: A20369_1400s Sample: 2018 Luxeon


μm


X-Z Slice of:CsIn+


MC:    20; TC: 4.493e+004


20 18 15 13 10 8 5 3 0


X-Y Total of:CsIn+


MC:    62; TC: 5.351e+005


Y-Z Slice of:CsIn+


MC:    21; TC: 4.412e+004


Figure 24. SIMS depth profile showing the CsIn+ and Cs  Al+ signals from a limited area of the 500 eV MCs+ SIMS  depth profile of the 2018 Luxeon ZES LED.


CONCLUSION


SIMS depth profiling revealed significant differences in  composition and doping profiles between the authentic  LED and the suspect counterfeit LED, confirming the  counterfeit status of the suspect device. Specifically the  suspected counterfeit LED had its In quantum well  structure between approximately 70 and 330nm from the  surface whereas the genuine ZES LED has its In quantum  well structure between 50 and 130nm. The three times  thicker structure in the counterfeit LED suggests that this  part is perhaps based on older technology.


REFERENCES


1. SAE AS6171 Test Methods Standard; GeneralRequirements, Suspect/Counterfeit, Electrical,Electronic, and Electromechanical Parts. Issued 2016-10-30.


https://www.sae.org/standards/content/as6171/


2. SAE AS6171/13. Technique for


Suspect/Counterfeit EEE Parts Detection by


Secondary Ion Mass Spectroscopy (SIMS) Test Methods.In draft


3. Y. Gao, J. Appl. Phys. 1988, 64, 3760.


4. E. Niehuis, T. Grehl, F. Kollmer, R. Moellers, D.


Rading, R. Kersting, B. Hagenhoff. Surf.


Interface Anal. 2011, 43, 204–206


5. M. Simard-Normandin, C. Banks, S. Trifoli.


Aftermarket LED-based electronic devices,


buyer beware. SMTA ICEET Conference, 2018


59


↑


File: A20369


pourmy s


Sample: 2018 Luxeon


Time-Resolved Imaging of VLSI Circuits using


a Single-Point Single-Photon Detector and a Scanning Head


1 IBM T.J. Watson Research Center, 1101 Kitchawan Rd, Yorktown Heights, NY 10598 – stellari@us.ibm.com  2 Hamamatsu Photonics, Japan & USA


In this paper, we present the first prototype of a Scanning TimeResolved Emission (STRE) system consisting of a highsensitivity, low-noise, and low-jitter single-point  Superconducting Single-Photon Detector (SSPD) combined  with a specialized scanning head of a Laser Scanning  Microscope (LSM). This idea was first proposed in late 2006


[1] but required the right combination of detector,customization, and collaboration with a tool vendor to get to fruition. It should be understood that this is still a prototype system under development and significant improvements in acquisition time, resolutions, and performance are expected in the near future. In this paper, we will also present the first preliminary results acquired using a test chip fabricated in 32 nm SOI.


The use of hot-carrier photon emission from VLSI circuits for  localizing and identifying failures has been widely used for  several decades in both time-integrated and time-resolved  applications. More advanced extensions have also been added  to this technique during the years, based for example on the  detection of the Light Emission due to Off-State Leakage  Current (LEOSLC) [2-4]: circuit logic states mapping [5], power grid drop evaluation [3,6,7], circuit internal temperature  and gate self-heating measurements [8,9], etc. In 1995, Picosecond Imaging Circuit Analysis (PICA) was first  introduced by Kash and Tsang at IBM [10]. This technique  allows the observation in time and space of the faint NearInfraRed (NIR) light pulses emitted by hot-carriers during the  switching transitions of CMOS transistors. From the optical  waveforms it is possible to extract propagation delays, signal  skews and other time-dependent problems in a non-invasive  and very effective way that allowed its widespread adoption by  the testing and diagnostic community.


The evolution and improvements of PICA capabilities have  been strongly influenced by different detectors that have been  adopted over the years to measure the arrival time of the  photons compared to a reference signal (trigger). The  Mepsicron S-25 detector [11] was originally adopted because  of its capability of measuring the spatial coordinates of the  photons in 2D, besides their arrival time. This allows the  creation of images in time (movies) of the evolution of the chip, thus simplifying the interpretation of the data. However, the  continuous trend of the semiconductor industry towards smaller  devices and lower supply voltages [12] has caused significant


reduction in emission intensity as well as a spectrum shift  towards longer wavelengths [13-15]. This has pushed the  adoption of single-point detectors with higher sensitivity at  longer wavelengths, including InGaAs Single Photon  Avalanche Detectors (SPADs) [16] and Superconducting  Nanowire Single Photon Detector (SnSPD) [17-19]. These  detectors demonstrated to be very useful for probing internal  nodes but lacked key advantages offered by imaging detectors.


About 10 years ago, Hamamatsu Photonics introduced a novel  2D imaging PICA camera [20] cryogenically cooled down to  120 K to reduce noise. The camera consists of a thin  GaAs/InGaAs cathode of approximately 5 mm x 5 mm in size  that absorbs the impinging emission while a resistive anode is  used to measure both the arrival time and the spatial XY  position of each electron pulse, corresponding to a detected  photon, with a time jitter of ~110 ps-FWHM (Full-Width at  Half the Maximum) and about 200 x 200 “pixels”. However, the limited sensitivity of the camera in scaled low voltage  technologies and the availability of Laser Voltage Probing (LVP) and Laser Voltage Imaging (LVI) techniques [21] prevented a wider adoption of PICA for several years.


In more recent years, laser probing techniques have also been  showing some limitations due to their invasiveness and limited  spatial resolution caused by destructive interference from  neighboring gates [22]. On the other hand, SSPD detectors have  been steadily improving in performance [23], compactness, and  availability, thanks to their commercial applications in quantum  communication technologies. Additionally, TRE does not  suffer of some of the spatial resolution requirements of laserbased technique because there is no destructive interference and  the high time resolution can be leveraged to separate signals as  discussed in [24].


Around 2006, some of us envisioned a time resolved system  that would take advantage of the novel high sensitivity, low  jitter, low dead-time SSPDs and would combine it with a  custom scanner head, similar to the one already used for LSMs, to create pseudo 2D imaging, at the cost of additional  acquisition time [1]. In this paper, we will describe the proposed  idea and present preliminary results acquired using a prototype  system developed by Hamamatsu Photonics.


Scanning Time-Resolved Emission System


A large number of failure analysis systems combines  photoemission (i.e., time-integrated emission measurement  with an InGaAs or MCT camera) and laser-based techniques


(probing or stimulation techniques). This is usually achieved  with separated optical paths that are distinguished soon after the  objective (see Fig. 1). This is due to the different wavelengths  involved (i.e., a single wavelength for laser and a broad band  requirement for emission) as well as imaging vs. single point  requirements. Following a similar principle, when higher  sensitivity single-point detectors were first introduced [25], an  additional separated path was added to maximize the collection  efficiency onto detectors with specific fiber coupling  requirements (see Fig. 1). Ultimately, this required the  development of various techniques to steer the collection spot  of the detector onto the targeted device and provide/maintain a  calibrated alignment for the user.


At the same time, one can understand that a Laser Scanning  Microscope (LSM) is designed to aim a point light source onto  different positions of a sample with high precision and  reproducibility, as well as to collect returning light reflected by  the sample and aim it onto a single point detector as shown in  Fig. 2. Typically, these detectors are not required to be very  sensitive (i.e., single-photon capable), work in linear mode, and  do not have very fast response time.


continuous


trigger signal


optics


pin hole


reflected/excited light emission


opticspin holeopticsPIN APD,PMTphotodetector:static


opticsolen hpiicsoptSPAD,SSPD,PMT


dichroic mirrorof


intensity


dichroic mirrorf


timing↓signal


x,y scan


古electronics


zz*TCSPC


sample


static or slow


↓electronics


→


14 channels photon photodetector:timing


pulsed


However, for some applications, certain types of modifications


power suppytester


have been already proposed and implemented. For example, in  fluorescence lifetime measurement systems, more advanced


test board


detectors have already been incorporated into a custom LSM to


temporary chip


improve sensitivity and time resolution [26]. Referring to


attachment


circuit under test


lens


Fig. 3, a short laser pulse is sent to the sample through a  dichroic mirror that is transparent only to the wavelength of the


3-position mirror


optical coupling


laser. The pulse stimulates fluorescence at the target location at  a difference wavelength and with a characteristic delay and time


SSPD


constant. The combination of the dichroic mirror and a delayed  activation (gating) of the single-photon detector allows one to


PEMLSM


isolate the small useful signal from the larger laser background. Similarly, in LVP and LVI applications, higher bandwidth  communication detectors in the 10 GHz range are typically  used to improve the time resolution and sensitivity of acquired  waveforms. One can also notice, that in both proposed  examples and applications, the measured light from the sample  is directly affected by the presence and intensity of the  stimulating laser probe.


In our STRE system, we propose to use the LSM to collect  spontaneous photoemission generated by the sample, with no  light source being aimed to the sample. Additionally, a singlephoton counting detector is used as a sensor for the LSM. An  SSPD is a particularly good choice because it is typically fiber  coupled, it has a detection efficiency that can easily achieve  80% or more with a broadband response that can be tuned with  resonant cavities, and it has a very low jitter of less than 20 psFWHM (Full With and Half the Maximum). Additional very  desirable features include its low intrinsic noise and short  recovery (or dead) time. All these features make it very suitable  for single point waveform probing as well as for scanning  applications. Higher efficiency, low false noise detections, and  a quick recovery time, to be ready for the next iteration, allow  to reduce the dwell time and the total acquisition time.


Fig. 4 shows a simplified diagram of the STRE system. Besides  the replacement of the detector to enable time-resolved  emission measurements, additional modifications of the


light tight enclosure


optical fiber


Figure 1: Diagram of a typical failure analysis tool  incorporating different paths for photoemission (PEM), laser  techniques using an LSM, and a fiber-coupled detector [25].


changing image


Figure 2: Diagram of an LSM highlighting the impinging (green) and reflected (blue) light paths.


movie


Figure 3: Diagram of system for fluorescence lifetime  measurement used in biomolecular applications.


61


electronics and LSM are needed. Key considerations relate to  differences in wavelength, polarization, and fibers. Firstly, photoemission is intrinsically broadband, peaking between  1800-2000 nm but extending much further at both shorter and  longer wavelengths. For this reason, optical components in the  LSM path need to be adjusted to properly reflect and transmit  such wavelengths with limited distortions that would cause  undesirable loss in lateral spatial resolution. Furthermore, laser  sources used for laser-based applications are typically  polarized, and LSMs take advantage of this to reduce spurious  back reflections by using polarized beam splitters and quarter  wave rotation plates. Obviously, such elements would be  detrimental causing losses larger than 50%, if used for  spontaneous photoemission, which has typically no significant  polarization. Additionally, most SSPDs use ~9 µm core SingleMode Fiber (SMF) pigtails, which introduce a much smaller  coupling target that typical LSM photodetectors. A final  consideration relates to the use of multiple optical elements and  their contribution to noise background. Due to the complexity  of scanning heads and the requirement of coupling to such a  small fiber, multiple optical elements are typically needed. Unfortunately, they can also easily add up to a reduction in  signal, as well as an increase in background thermal noise.


timing photodetector:


Pseudo 2D image construction


SPAD,SSPD,PMT,etc


The pseudo 2D images of the STRE system are constructed


spontaneous/intrinsic light emission


timing photon


using the methodology illustrated in this section. First, a pattern


image is acquired to navigate to the desired probing location


signal


and to determine a Region Of Interest (ROI). The latter may


system


consist of a single probe point, or more probe points,


*4 channelscontrol


corresponding to multiple gates, or an area to be imaged.


Z↑TCSPC


trigger signalelectronics


During all subsequent emission measurements, no light of any


↓


kind is used to illuminate the sample, contrary to all laser-based  techniques and fluorescence life time measurements.


event


database9 PC


If a single probe point is being acquired, the scanner head is  actuated to collect the emission from that location and send it  to the SSPD through its fiber. In this case, a TRE waveform is  created and displayed to the user for subsequent analysis.


More interestingly, a 2D image of an area of the sample may be  desirable to help in the localization of the unknown emission or  to allow the application of advanced techniques to improve the  lateral spatial resolvability of signals from closely spaced gates, as described in [24]. Referring to the diagram in in Fig. 5, the  ROI is first expressed as a list of (x,y) locations for the scanner  head. The scanner head is then positioned to target each  location, one at the time. For each one, TRE is acquired using  the SSPD. In some cases, the acquired data may be first  processed to create an histogram of the photon arrival time (i.e., TRE waveform). Then, the raw data or the TRE waveform is  analyzed with various algorithms to calculate a Figure Of Merit (FOM) that represents a feature of interest for the device, user, and test application. Finally, the FOM is used to set an  appropriate color/intensity of a pseudo 2D image at a pixel  location derived from the (x,y) coordinate of the scanner head.


Smart scanning


The previous simple implementation can be significantly  improved by devising smatter scanning plans to reduce the  overall acquisition time. These may include creating a sparse  coverage of the area followed by a targeted selection of  additional pixels as shown in Fig. 6. In this case, instead of  simply implementing a raster scan of the ROI from a corner or


Scanning head


Photodetector


the center of the ROI, one could easily implement a sparse  coverage of the ROI as shown by the blue pixels in the scanner  mask. Locations with low FOM (e.g., location “1” in Fig. 6)


↓ Arrival time


may not receive additional time, while locations with elevated


(x,y) position


Create TRE


FOM (e.g., location “2” in Fig. 6) may be further analyzed by


waveforms


adding additional probe points as indicated by the red pixels in


Calculate FOM


Figure 4: Diagram of the proposed scanning Time-Resolved


Emission measurement system.


Create


image


Figure 5: Diagram explaining how the pseudo 2D images of the  TRE are created using a system as the one described in Fig. 4.


Figure 6: Example of smart scanning strategy.


62


Fig. 6. Adaptive algorithms that automatically decide probe  locations based on layout information and already acquired  emission are very effective in reducing the acquisition time.


Off-state leakage


Switching activity


Falling edge


Rising edge


Stable logic state


In many practical applications, one may also want to implement


a methodology where the ROI is continuously traced by the


scanner head with a determined speed. Photons would be


continuously acquired and tagged with time and the (x,y)


position of the scanner head. This would allow to generate 0123456789 10 11 12 images with progressively better SNR through the allocated


acquisition time, similarly to real 2D cameras. This approach


can give a more rapid feedback to the user. Additionally, by


creating multiple frames of the pseudo 2D image, one could


implement correction algorithms to counteract mechanical


drifts. Unfortunately, this feature is not yet implemented in our


prototype system and will be demonstrated at a later time.


FOM calculation


Most interestingly, the choice of a specific FOM to be used to  create the pseudo 2D image is a key differentiator from other  existing time-integrated and time-resolved emission  techniques. For example, an InGaAs camera or MCT array  would only be able to display the total emission intensity. The  same behavior can be implemented in the proposed system by  choosing a FOM corresponding to the total photon counts  acquired during the dwell time at each location of the scanner  head. However, since full time tagging of the single photos is  implemented, many other types of FOMs, targeting specific  features, may be much more interesting and useful. In fact, both  frequency- and time-domain approaches could be used.


For example, a Fast Fourier Transform (FFT) of the time tagged  photons may be used to determine which portion of the ROI (and therefore of the circuit) is switching at a specific frequency  of interest (e.g., the clock or data frequency). At the same time, the phase delay would provide the order of the gates as well as  an indication of the amount of delay. It should also be noted that  frequency-domain images could be easily generated at the same  time of other types of images because all the information is  readily available and can be processed and analyze on the fly, either live or as a post processing step.


Dynamic logic state mapping is also very easy to implement  using time-domain analysis techniques because full spatial and  time information is available. For example, time windowing of  the emission at different clock cycles. Similarly, Fig. 7 illustrate  that pseudo 2D images highlighting the rising/falling edge of a  transition as well as the leakage of the gate can be easily  implemented. A bright emission spot in an image could be  analyzed by breaking it down in its components to determine if  an anomalous leakage path exists in specific logic states or  during switching events. From the same acquisition one could  also extract a measure of the gate switching activity, corresponding to falling/rising edges, as well as a map of the  gate leakages to target variability and self-heating applications.


Measurements


To demonstrate the capability of the first prototype system, we  have acquired STRE images of a test chip fabricated in 32 nm  SOI technology node [27]. The DUT consists of multiple delay  lines in parallel. Fig. 8 shows a diagram of the specific  acquisition process that has been implemented. A pattern image  is first acquired using laser illumination and the scanner head, similarly to any other LSM implementation used for failure  analysis. A ROI (green box) is selected and re-scanned by the  scanner head following the naïve raster scanning procedure or  the more advanced scanning procedures described in the  previous section. For a given location marked by the red cross,


(285,291)ROI


(285,291)


(285,291)Time [ns]


Figure 7: Time-domain analysis, such as time windowing, allows to break down the acquired emission into key dynamic  and static components.


Time [ns]


90


Acquire TRE waveform


Emission intensity (a.u.)台古台吕70


00.511.522.533.544.55


Calculate FigureOf Merit (FOM)


Figure 8: Pseudo 2D image acquisition process implemented using a 32 nm SOI test chip.


63


TRE is acquired by the SSPD for a time corresponding to the  predetermined dwell time of the scanner head. Depending on  the type of FOM selected, a TRE waveform may be generated  using the time-tagged photos acquired at the (x,y) location. A  corresponding FOM is then computed and used to determine  the value (e.g., intensity/color) of a pseudo 2D image that is  finally presented to the user. Although this entire process could  be easily implemented live by the tool, due to current  limitations of the prototype system, most of the analysis was  implemented as post-processing. It should also be noted that, in  most cases, multiple pseudo 2D images are automatically  generated, corresponding to different FOM algorithms.


For the examples shown in this paper, the sample was imaged  using a 2.5 NA centric SIL with a magnification of ~250X. The  ROI is chosen to be slightly larger than the target 7 inverter  stages delay line and is approximately 30 pixels wide and 85  pixels high. It should also be noted that the pseudo 2D images  presented have several missing pixels (dark blue pixels in the  colored images) that are due to miss-positioning of the scanner  head due to a bug in the control software that is being fixed. For  full disclosure, it should also be understood that the current  prototype system has several known and resolvable bottle necks  that introduce significant delays in the measurement acquisition  and do not permit a fair comparison yet with other tools and  techniques, which is outside the scope set forth by this work.


Fig. 9 shows a comparison of the time-integrated emission  image acquired with an InGaAs camera (a) to the pseudo 2D  image of the total emission intensity acquired from the sample  using the prototype STRE system (b). In this case a full map of  the 30 x 85 ROI was acquired for completeness. Note also that  a small percentage of the pseudo 2D image are wrong due to a  previously mentioned scanning head software issue.


As expected, the two images show very similar and equivalent  features. While the InGaAs camera may be affected by  saturation effects and artifacts due to the presence of bright  emission spots at the left-hand side of the ROI, the STRE image  has a virtually unlimited dynamic range in presence of bright


emission spots, as well as “unlimited” acquisition time to gather


emission from very faint emission spots.


By comparing the two images, we can confirm that the InGaAs  camera image currently offers a higher pixel count, lower noise, and significantly shorter acquisition time. Even by resolving the  know bottle necks of the current system, we do not envision that  the STRE system could offer faster acquisition times than an  imaging detector (e.g., InGaAs or MCT camera) for  applications aiming to simply measure the total emission  intensity. Using STRE makes sense only when the sample, and  therefore its emission, is intrinsically dynamic in nature. Additionally, using time- and/or frequency-domain analysis  allows one to extract additional useful information.


Frequency-domain analysis


As discussed in the previous session, a dataset acquired with the  prototype STRE system can be readily analyzed in the  frequency domain to bring out specific features of interest, such  as switching activity or a signal path of interest that was  targeted by a specific test pattern.


In our example, only one of the inverter-based delay lines is  being activated with a signal at 20 MHz, while all other lines  are quiescent. For this reason, a frequency domain filter can be  used to isolate the gates that are part of the active delay line  from surrounding gates that just contribute to background  emission and noise. This is a situation similar to scan debug.


(a)


(b)


Figure 9: (a) An InGaAs camera image is compared to (b) a  pseudo 2D image of the prototype STRE system.


Figure 10: (a) Amplitude and (b) phase of the FFT of the STRE  dataset at 20 MHz, corresponding to the input signal.


64


Fig. 10 shows the (a) amplitude and (b) phase of the of the FFT  of the STRE dataset calculated at 20 MHz. One can notice that  the pseudo 2D image of the amplitude clearly shows the 14  emission spots corresponding to the 7 n-FETs and 7 p-FETs. This technique is very effective to filter out the  stationary/quiescent background even when it is much brighter  than the switching gates of interest (see bright emission at the  left had side of Fig. 9). Additionally, one can appreciate that the  frequency-domain analysis allows a more accurate localization  of the emitting transistors. This can be used to improve layout  registration or any other subsequent analysis, such as the  creation of TRE waveform with stronger SNR, by precisely  combining photons from neighboring channels.


Advanced scanning algorithms


Depending on the pixel dwell time and data acquisition  overhead, scanning a large ROI may be time consuming. Several strategies could be used to help the user collect  preliminary data and have a sense of the emission distribution.


Fig. 11(a) shows a pseudo 2D image of the amplitude of the  FFT at 20 MHz acquired by scanning alternated pixels of the  ROI, as represented by the light-colored pixels in the scan mask  in Fig. 11(b). This allows one to reduce the acquisition time by  roughly 50% while providing a good indication of the locations  of the switching gates.


Thanks to the high sensitivity of the frequency-domain analysis  and its capability of isolating very well the gates and transistors  of interest, the approach can be pushed even further by  dramatically reducing the number of probed locations.


Referring to Fig. 12, a very low density scanning mask (a), corresponding to one pixel being measured in each block of


4 x 4 pixels, is initially used to create a rough pseudo 2D image  of the emission (b) inside the ROI by plotting the amplitude of  the FFT at 20 MHz, corresponding to the gate input signal  frequency. This allows for roughly 16X saving in total  acquisition time. In this case, the resulting image appears too  severely down sampled to be immediately useful for the user. However, adaptive algorithms can be subsequently used to  select locations with good FFT signal and expand on them with  subsequently targeted scans. In particular, one could implement  an adaptive algorithm that acquires TRE data from pixels in (a)


Figure 11: (a) A pseudo 2D image of the amplitude of the FFT  at 20 MHz is acquired using a scanning mask (b) that skip one  every two pixels to save ~50% of the acquisition time.


(c)


(d)


Figure 12: A scanning mask (a) with one probe location per 4 x 4 pixels block is sued to quickly generate an initial pseudo 2D image


(b) that is subsequently refined with an adaptive mask (c) that acquires STRE data from pixels near other bright pixel dues obtaining  the final pseudo 2D image (d) while saving ~40% of the acquisition time.


65


close proximity to already acquired pixels with a signal above  a set threshold. Fig. 12(c) shows the resulting scanning mask  after applying this adaptive algorithm several times. The  resulting image in Fig. 12(d) yields results very similar to the  full scan image Fig. 10(a), while saving ~40% of time.


Time-domain analysis


Time-domain analysis technique can also be very effectively  used to create pseudo 2D maps of both switching events and  logic states. Referring to Fig. 13, time windowing the data  around specific times corresponding to switching transistors of  interest allows one to map the locations of the circuit affected  by such events. For example, Fig. 13(a) shows three brighter  n-FETs at even positions along the delay line, emitting light  during a falling edge transition. In the same image, 4 p-FETs in


5000600


nFETX1


4500


4000 350


nFET #8


N


"a000


nFETA?


2566


3500


2328295Tie frst


Emissionintensity [ccunts]


1500-


1000 therp amstdn raaghCAR


50000.511.522.533.54导


w外动


2958305 02E


oFET #6 nFET 4-nFET *3


见见


-nFET 42


odd positions of the delay line are also visible on the left-hand


side of the n-FETs, shifted by one gate. By time windowing the  STRE dataset at the time of the opposite input edge, the 4  n-FETs at even positions of the delay line become now visible  in Fig. 13(b). It should be noted that, although this technique  slightly reduces the background contributions of quiescent  gates, thanks to the very short duration of the window used to  highlight a transition edge, it is often far less effective than the  frequency-domain analysis. However, since both pseudo 2D  images can be easily generated concurrently from the same  acquisition, the frequency-domain image can be used as a filter  mask during time-domain analysis.


Similar to the switching event example, off-state leakage  emission can be also integrated during quiescent periods


Figure 13: Time domain analysis of the STRE dataset showing: (a) the switching emission during one transition of the input signal, (b) the switching emission during the opposite transition, and the leakage emission during the two logic states (c) and (d).


Figure 14: TRE waveforms extracted from the 7 n-FETs of the delay line.


66


between transitions. Fig. 13(c) and (d) show the result for the  two possible logic states of the delay line. In the first case the 3  odd n-FETs are leaking, while in the second case the 4 even  n-FETs are leaking. Contrary to logic state mapping obtained with a time-integrated camera, this technique does not require stopping the clock of the DUT, or multiple acquisitions.


the parameters discarded photons emitted from sources where


emission was more spread in time or space.


010203040


The 2D histogram post-clustering is available in Fig. 9. Compared to Fig. 8, the relative intensity of the area squared in  red has diminished while the area squared in white drew the  image contrast. The TRE waveform of the red area, prior to the  processing (Fig. 10), shows that emission duration is quite  spread in time while the emission from the white area in Fig. 9  is more localized. The time parameter, EpsT, has been chosen  to be in the range of tens of picoseconds, which is very small as  compared to the duration of emission events in Fig. 10. During  clustering, since the photons from the red area are further from  each other along time axis (Fig. 10), they cannot be detected by  the algorithm with such parameters and as a result, the intensity  of this area was decreased as compared to the white area (Fig. 11) after processing. Potentially, this issue could be solved with  a clustering algorithm capable of handling variable densities.


X coordinates (μm)


Figure 8: 2D histogram generated from the 3D data with an  image resolution of 32 x 32. Data acquired with the 50X  objective lens equipped (NA 0.4). The color bar indicates the


00246810


number of photons.


Figure 9: Post-Clustering 2D histogram image computed from  remaining photons. The color bar indicates the number of  photons per pixel.


From each cluster, an associated 2D Gaussian distribution with  a spatial resolution improvement of factor 2 was computed. All  the associated Gaussians were then summed, generating the  image in Fig. 12. The image resolution is now 64 x 64.


In this specific case of application, the low quantity of points  per cluster remains one of the weak points for the interpolation. The more points there are, the more reliably the Gaussian  function can be computed.


73


Time (ns)


Figure 10: Photon counting histogram of the area square in red  in Fig. 9 prior to filtering.


Time(ns)


Figure 11: Photon counting histogram of the area squared in  white in Fig. 9 prior to filtering.


Figure 12: Interpolated image from the results of clustering by  STDBSCAN on the TRE data acquired at a resolution of  32 x 32. Clustering parameters: EpsT = 15 ps, EpsXY = 1 pixel, Minpts = 3. Image resolution was interpolated by a factor 2 (new image resolution is 64 x 64).


Discussion


Study in under sampling conditions


台


In the introduction section to the experiment setup, the duration


of acquisition has been identified as the main bottleneck in this  study. Since some analysis may require a fast turnover, it is


critical to explore how shorter duration can be reached.


Photon Count


Using a scanning microscope, image resolution can be changed.


For instance, assuming the full field of view of the objective  lens is scanned, it is possible to obtain an image with a


resolution of 256 x 256 or 1024 x 1024. The main difference is


the step between pixels. The larger the resolution, the smaller


02004006008001000


the step size between pixels. Similarly, considering a fixed  objective lens, one can zoom in, meaning that a smaller area  within the field of view is scanned. As the area is smaller but  the number of pixels is the same as without zoom, then the step


between pixels is smaller and spatial sampling frequency  increases. Scanning a large area with a low spatial resolution


thus provides the fastest throughput but may fail to highlight the  information of interest.


In order to explore how the interpolation process performs in


合


various scanning conditions, data are acquired at different


spatial resolution. As a reference, an emission image was first


CountPhoton


acquired on an 8-bit microcontroller (Microchip


PIC16F84A [21]) with a low magnification objective lens (5X, NA 0.15). The microcontroller executed a simple loop where it


read a byte from the SRAM, stored it in the accumulator and  sent an acknowledgement signal on one output before clearing


the accumulator. The InGaAs camera image in Fig. 13 shows  activity from what is assumed to be the core logic of the device. In this section, the focus will be set on the area squared in  yellow since it appears that there are strong emission signals. A  zoom of this area is available in Fig. 14.


0 5


u15 S20


a e 0 p


0 0 0>35


45 30 25


Figure 13: InGaAs emission image of the area under  investigation. Measurement performed with the 5X objective  lens equipped (NA 0.15). The yellow square indicates the area  probed.


74


Figure 14: Zoom of the area squared in yellow in Fig. 13.


450


Figure 15: 2D histogram generated from the 3D data. The  image resolution is 32 x 32. Data acquired with the 5X objective  lens (NA 0.15).


For the photon counting measurements, the acknowledgement  signal from the microcontroller was used as a time reference. A  small area was scanned with a resolution of 32 x 32 pixels and  a dwell time of 4 seconds per pixels (Fig. 15). The clustering  and interpolation process was applied with the following  parameters: EpsT = 1 ns, EpsXY = 1 pixel and MinPts = 5. The  post interpolation results with resolution improvement by a  factor of 10 is shown in Fig. 16. Compared to Fig. 14, equivalent emission spots can be seen in the central row, even  though they appeared to be single pixel in Fig. 15. These results  suggest that even if the spatial resolution is low, the process  developed in this study can help to recover higher frequency  information. Some spots of lower intensity also appear in the  image. Since they do not appear in the reference image, it is  difficult to conclude if they actually resulted from photon  emission or from remaining photons due to the clustering  parameters. In addition, some spots were visible in Fig. 14 but  do not appear in Fig. 16. Once again, they could have been  removed by the clustering, merged with other clusters or the


system could have failed to detect them for unknown reasons. At this juncture, there is not enough evidence to identify the  cause and further research and development have to be carried  out. The same observation is made for the two close spots  circled in yellow Fig. 14. They seem to have merged in Fig. 16, where they are indicated by the yellow arrow.


3.5


w150


2.5


9200 6


e 0250 p


0 0 0人350


300


1.5


X coordinates (m)


95


1000100200300400


Figure 16: Post interpolation image of data from Fig. 15.


Interpolation factor of 10 (new image resolution: 320 x 320) and clustering parameters: EpsT = 1 ns, EpsXY = 1 pixel and


85


MinPts = 5.


兰


Finally, in IC design, elements constituting the circuit are


75


usually placed following a grid and should be either collinear


or perpendicular to one another. Having distribution orientation


coordinates (μY)m


such as the one pointed out by the red arrow in Fig. 16 is thus


unexpected and indicates a potential failure of the estimation


process. For a bivariate normal distribution, the orientation is


qualified by the covariance term in the variance-covariance


0100200300400


matrix. Hence, such estimation errors occur due to a lack of  constrains for this term. This is another parameter to explore for  future improvement of the process.


Comparison of results from various scanning resolution


Trying to overcome the issue of the two spots that had merged  as one in Fig. 16, we explored if a change of scanning resolution  helps in resolving them. The same objective lens was used while  a zoom factor of 3 was applied for scanning. This means that the  field of view of the area under investigation was divided by 4. Two sets of measurement were acquired. For the first, the  scanning resolution was 32 x 32 pixels while in the second, it  was set to 64 x 64 pixels. This means that between the two  experiments, the sampling frequency was increased by a factor


2. Hereafter, these two sets will be referred as LR and HR sets. In order to acquire similar quantities of photons, the dwell time  for the first experiment was 8 seconds and 2 seconds for the  second set. Upon completion of experiments, 149198 (LR) and  150119 (HR) photons were collected. The two images of the 2D  photons counting histograms are available in Fig. 17 and Fig. 18. Between the two images, spots of stronger intensity than the  background can be seen at the same locations. However, since  resolution had been increased, energy was spread between more


pixels and the maximum photon count per pixel is lower in the  HR image.


The clustering and interpolation process was applied to both


sets with the following parameters:


- Set LR: EpsXY = 1 pixels; EpsT = 500 ps; MinPts = 20


古


pts.


- Set HR: EpsXY = 1 pixels; EpsT = 500 ps; MinPts =


召


10 pts.


2D photon counting histograms of the photons remaining after


clustering are shown in Fig. 19 and Fig. 20. Similar to what was


Y coordinates (μm)


observed on raw images in Fig. 17 and Fig. 18, photons arise


from the same locations, although energy is more spread for the  HR set. After generation and summation of the PDF (Fig. 21  and Fig. 22), the spots that had previously merged can now be


020406080100120


distinguished. The HR set shows a better localization. For the


LR set, the chosen EpsXY matches with a distance of 3.7 µm


while for the HR set, a single pixel matches with a distance of


1.85 µm. In both cases, the resolution is superior to the value of


the InGaAs camera (with the 5X objective lens, 1 pixel <=> 3.9


µm). Hence, the higher spatial resolution allows a more 0


localized estimation of the PDF.


190


U u


:180


170


e u8 0


0 0


0品>


g


130


Y)(μm coordinates


1100204060801001200 10 100


60 70


Figure 17: 2D histogram generated from the LR set. Image


resolution of 32 x 32. Data acquired with the 5X objective lens 0


(NA 0.15) and a zoom factor of 3.


In Fig. 22, the two spots on the right side of the image seem to  have a larger intensity compared to the other spots. This is not


山40


the case in Fig. 21. This high energy is well localized, meaning


1)S


that it results from distribution with very small variance


compared to the other distributions. Indeed, since the integral


e u


p


of a PDF over its interval of definition is equal to 1, the


maximum amplitude of PDF with a small variance is higher


0人


品


than the one of a distribution with large variance. Experiments  with other sets of parameters show that this phenomenon can be


attenuated (Fig. 23). Once again, some spots have disappeared  in the process, suggesting that variable densities of photons


exist in this set and there is a need to further study the choice of 020406080100120 parameters for the clustering process.


Figure 18: 2D histogram generated from the HR set. Image  resolution of 64 x 64. Data acquired with the 5X objective lens (NA 0.15) and a zoom factor of 3.


Figure 19: 2D photon count histogram after clustering for the


LR set. Parameters: MinPts = 20, Eps XY = 1 pixel, EpsT = 500 ps.


Figure 20: 2D photon count histogram after clustering for the  HR set. Parameters: MinPts = 10, Eps XY = 1 pixel, EpsT = 500 ps.


76


X coordinates (mm)


Figure 21: Interpolated image of the LR set with an improved  resolution by a factor of 10. New image resolution of 320 x320.


Figure 22: Interpolated image of the HR set with an improved  resolution by a factor of 10. New image resolution of 640 x 640.


Figure 23: Interpolation results for HR set with clustering  parameters EpsXY = 1 pix; EpsT =300 ps; MinPts = 10 pts. Resolution improved by a factor of 10. New image resolution of  640 x 640.


x10~3


Framework of application of clustering and interpolation


processing scheme


The process introduced in this paper relies on identifying


photons originating from the same event, i.e. a specific time and


node (for instance transistor, gate). The localized groups of


photons have boundaries in the 3 dimensions and two spots that


seem close in the (x,y) plane can be differentiated once the time


吕


dimension is taken into consideration. As long as emission is  qualified by time, the clustering and interpolation process can


be considered to generate images at higher resolution (i.e.


increase the number of pixels) and improving the precision. In


case emission is happening independently from time, then  clustering can only be performed using space dimensions and


this approach may not be the most efficient one.


In the field of FA, distinction is made between static PEM and  Time Resolved Imaging. The terms static and dynamic may be  sometimes misleading as they may refer to either the electrical  biasing conditions (i.e. DC or AC signals are provided to the


circuit) or to the time-resolved capability of the detection


scheme (i.e. time integrated sensor versus time-resolved sensor,


0.45


as mentioned in the introduction). From the electrical biasing


perspective, since DC signals are not qualified by time, this 3D  processing scheme may not be the most suitable, as discussed


0.35


in the previous paragraph. On the other hand, it has been


designed to handle emission originating from AC signals. From


0.25


the instrumentation perspective, it can be applied as long as the


detection scheme provides the (x,y,t) data. Applications  reported at the beginning of the Discussion section have shown


Y coordinates(μm)


0.15


that compared to emission images generated by a matrix array


sensor (Fig. 13 and Fig. 14), images can be generated with a


0.05


superior spatial resolution (Fig. 19 to Fig. 23). Thus, the 3D


process can be considered to be used in various applications as


long as some of the emission is time-dependent. It may provide  additional information to a time-integrated measurement such  as PEM or improve image resolution in time resolved imaging.


In dynamic photon emission microscopy, image quality and the


quantity of information it can bring can be challenged by  parameters such as optical resolution, spatial resolution and low


SNR. In this paper, we reported on a post-acquisition  processing scheme based on clustering and Gaussian


interpolation to generate images with a larger image resolution,


Y coordinates (μm)吕吕古


compare to what could be directly achieved from the detection


scheme.


This process is built on the identification of groups of photons


generated by a specific event, i.e. switching of a node by


。20406080100120


clustering. Density-based clustering algorithms have shown to  be efficient to identify groups, even though photon emission  data are sparse and SNR is low. Form these results, a probability  density function is estimated with larger spatial sampling  frequency than the initial observation and associated to each  cluster. The Gaussians are then summed to generate the high  resolution image.


77


Using a customized setup normally dedicated to single point  time-resolved emission measurement, images with low spatial  resolution were generated on different devices and proofs of  concept of the image enhancement by the clustering-based  process have been reported. Experiments have shown that even  with low spatial sampling frequency, some information can  actually be recovered using this process. This result is of  interest for the study of ultimate VLSI where spatial resolution  may not be enough. However, results remains qualified by the  clustering parameters and the higher the spatial sampling  frequency, the better results can be achieved.


This process could be applied in many context such as failure  analysis and security analysis where photon emission is time  and space dependent. Finally, it has potential to also help in  overcoming the optical resolution limit in dynamic photon  emission. This 3D unsupervised learning process remains at  initial development stage and more R&D work needs to be  achieved before qualifying it as a robust solution to the overall  optical and spatial resolution challenge.


[1] J. Kölzer, C. Boit, A. Dallman, G. Deboy, J. Otto, D.


Weimann, “Quantitative Emission Microscopy”, Journal  of Applied Physics, vol. 71, no. 11 (1992), R23-R41.


[2] J.C. Tsang, J.A. Kash, D. Vallett, “Picosecond Imaging  Circuit Analysis”, IBM Journal of Research and  Development,  vol. 44, no. 4  (2000), pp. 583-603.


[3] A. Schlösser, D. Nesdospasov, J. Krämer, S. Orlic, J.P. Seifert, “Simple Photonic Analysis of AES”, Journal of  Cryptographic Engineering, vol. 3, no. 1 (2013), pp. 3-15.


[4] F. Stellari, P. Song, M. Villabos, J. Silvestri, “Revealing  SRAM Memory Content using Spontaneous Photons  Emission”, 2016 IEEE VLSI Test Symposium (VTS), Las  Vegas,  NV,  April 2016, pp. 1-6.


[5] J. Krämer, D. Nesdospasov, A. Schlösser, J. P. Seifert, “Differential Photonic Analysis”, COSADE 2013: Constructive Side-Channel Analysis and Secure Design, 2013, pp. 1-16


[6] C. Boit, “Fundamentals of Photon Emission (PEM) in  Silicon- Electroluminescence for Analysis of Electronic  Circuit and Device Functionality”, Microelectronics  Failure Analysis Desk Reference, 6th Edition (2011), pp. 279-291.


[7] W. Becker, Advanced Time Correlated Single Photon  Counting Techniques, Springer Verilag, 2005.


[8] K.A. Serrels, E. Ramsay, P.A. Dalgamo, B. Gerardot, J. A. O’Connor, R. H. Hadfield, R. J. Warburton, D.T. Reid, “Solid Immersion lens for nanophotonics devices”, Journal of nanophotonics, vol. 2, no. 1, 2008, pp. 021854.


[9] F. Lan, F. Stellari, A.B. Shehata, P.Song, “Extending the  resolution of emission images beyond diffraction limits  using deconvolution”, ISTFA 2016: Conference  Proceedings from the 42nd International Symposium for  Testing and Failure Analysis, Fort Worth, TX, November  2016, pp.  1-7.


[10] I. Vogt, A. Glowacki, U. Kerst, P. Perdu, T. Nakamura, C. Boit, “New method for enhancing Photon Emission  Measurements similar to 2D-tomography”, 2018 IEEE  International Symposium on the Physical and Failure  Analysis of Integrated Circuits (IPFA), Singapore, July  2018, pp.1-6.


[11] F. Stellari, P. Song, A.J. Weger, D. Maliuk, H.A. Ainspan, S. Kim, Y. Kwark, C.W. Baks, “Tester-based methods to  enhance spatial resolvability and interpretation of timeintegrated and time-resolved emission measurements”,  ISTFA 2013: Conference Proceedings  from the 39th  International  Symposium for  Testing and Failure  Analysis, San Jose, CA, November 2013, pp. 341-349


[12] R. Desplats, G. Faggion, F. Beaudoin, P. Perdu, T. Lundquist, K. Shah, A. Chion, M. Vallet, P.Sardin, “A  new approach for faster IC analysis with PICA: STPC3D”, in Proceedings of the 10th International Symposium  on the Physical and Failure Analysis of Integrated  Circuits (IPFA), Singapore, July 2003, pp. 45-53.


[13] S. Chef, S. Jacquir, K. Sanchez, P. Perdu, S. Binczak,  “New statistical post processing approach for precise fault  and defect localization in TRI database acquired on  complex VLSI”, IPFA 2013: Proceedings of the 20th  IEEE International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA), Suzhou, China, July 2013, pp. 136-141.


[14] S. Chef, S. Jacquir, K. Sanchez, P. Perdu, S. Binczak “Cluster matching in Time Resolved Imaging for VLSI  Analysis”, Proceedings of the 21th International  Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), Sungapore, July 2014, pp. 379-382.


[15] H.P. Kriegel, P. Kröger, J. Sander, A. Zimek, “DensityBased Clustering”, Wiley Interdisciplinary Reviews: Data  Mining and Knowledge Discovery, vol. 1, no. 3, 2011, pp. 231-240.


[16] M. Ester, H.P. Kriegel, J. Sander, X. Xu, “A density-based  algorithm for discovering clusters in large spatial  databases with noise”, Proceedings of Second  International Conference on Knowledge Discovery and  Data Mining, 1996, pp. 226-231.


[17] D. Briant, A. Kut, “ST-DBSCAN: An algorithm for  clustering spatial–temporal data”, Data & Knowledge  Engineering, vol.60, no.1, 2007, pp. 208-221


[18] https://www.idquantique.com/single-photonsystems/products/id230/, IDQuantique ID230 Brochure.


[19] DS180 : 7 Series FPGA Data sheet: Overview, Xilinx Inc,  https://www.xilinx.com/support/documentation/data_she ets/ds180_7Series_Overview.pdf


[20] Skoll Kintex 7 User’s manual, Numato Lab, https://numato.com/docs/skoll-kintex-7-fpga-module/


[21] Microchip Technology, “PIC16F84A Datasheet”, Ver. DS35007C, 2001-2013


78


Automated Multi-level Circuit Net Trace for Hotspot Analysis


SH Goh, E Susanto, Song Li, BL Yeoh, MH THor


GLOBALFOUNDRIES, Product Diagnostic Engineering, Singapore


D Zhou


Mentor - A Siemens Business


Post-fault isolation layout net trace and circuit analysis based  on abnormal hotspots is a critical step because it directly  impacts the outcome of failure analysis. In this work, we  review current commercial net tracing solutions in terms of  their strengths and drawbacks. As an enhancement, a new net  methodology that enables automation and the capability to  execute tracing beyond first-level transistors is introduced. This approach could potentially eliminate manual net tracing  and significantly improves the overall failure analysis  turnaround time.


Since the sub-45 nm technology, there has been increasing  occurrences of complex fails such as structural, functional or  soft fails, to name a few. Unlike parametric or power railrelated fails whose defects are fundamentally static in nature [1, 2]; a direct physical inspection following global fault  isolation (FI) is not recommended for such complex fails. The  localized signals no longer pinpoint the exact defect site or  electrical weak point [3, 4, 5]. In order to fulfil the mission of  global FI which is to narrow the search area for physical  inspection to as small and accurate as possible, a layout net  trace is inevitable. Figure 1(a) and (b) shows a single photon  emission signal micrograph and the first-level layout trace  path from the gate of the isolated device (encircled) respectively. In most cases, net tracing is required because a  photon emission signal is usually the consequence of a defect  that occurs along a driver net. In a worse case, some defects  could give rise to more than one emission signals such as  shown in figure 2(a). A more tedious net trace is required to  identify the suspected fail paths that relate all the hotspots as  shown in figure 2(b). It is worthy to mention that multiple  iterations are usually required to identify such specific nets. It  is not a trivial task.  In this example, an open defect that  occurs in the driver circuitry was found on physical  inspection.


A comprehensive understanding of the relationship/s between  the localized signal spots using layout net trace is necessary to  either hypothesize locations for physical inspection or guide


subsequent local fault localization process using techniques  such as nanoprobing [6] or laser voltage probing [7] to further  pinpoint the failing sites. Therefore, the quality of layout net  trace can influence the overall failure analysis (FA) success  significantly.


As we operate under escalating time pressures to deliver  faster product time-to-market, it is important to constantly  review the turnaround time of custom methods so that layout  trace analysis does not become a bottleneck to FA. This is the  main motivation behind this work.


The remaining paper will be organized as follows. The  second section reviews current state-of-the-art solutions. Section 3 introduces the proposed automated trace  methodology and section 4 presents two case examples to  demonstrate the effectiveness of the new trace concept. The  last section concludes.


Figure 1: (a) PEM signal image and (b) suspected trace path  where he defect lies.


79


Figure 2: (a) PEM signal overlay with optical image. (b) Suspected trace paths connecting all emissions to a single  driver net.


Current Situation


In general, there are two ways to perform net tracing on  GDSII layout.


Manual Trace


First, the location of interest which typically refers to a point  on a net polygon or contact (or via) node is identified  following FI. Generating a trace involves a simple click at  that point. Figure 3 shows two standard cells bounded in  boxes. The M1 (first metallization layer) net connected to the  gate of the bottom cell is selected and a trace connecting to  the active nodes on the top cell is highlighted. This process  iterates until sufficient traces are attained for analysis. Common tools for the tracing of nets are Synopsys Laker, Synopsys Avalon (formerly known as Camelot) and Mentor  Calibre DESIGNrev.


Figure 3: Manual net trace result of a net connecting two  cells.


Semi-Automated Trace


The second method is an automated approach which is  currently only available on the Synopsys Avalon platform. The enabling feature is called hotspot analyzer as shown in  figure 4(a).  First, bounding boxes are drawn over the hotpots. The analysis is then executed without further need to study  the anatomy of the standard cells. Within the layout field of  view, any net traces that relate the bounding boxes will be  highlighted. The results are shown in figure 4(b). The top  three outcomes refer to traces that relate the two hotspots. These include the common power and ground rails (top two  rows) to the two cells which are usually omitted for further  analysis. Although the third trace outcome was validated to  be similar to that of manual trace, this is certainly more time  efficient in comparison.


Figure 4: Synopsys Avalon’s (a) hotspot analyzer feature and


(b) trace results.


Limitations


However, a limitation exists in the second approach. This  technique only applies to cases where the hotspots are related  by a first-level net trace. In many cases, a second or higher  level of tracing is required. The definition of secondary level  trace is illustrated in figure 5. Using the same example as the  previous section, a third cell A is included as shown in figure


5(a). As shown in figure 5(b), cell A does not relate directly  to the top cell but has an intermediate connection to B. In the  event that a hotspot falls on A instead of B, the hotspot  analyzer will fail to identify the relationship between A and  the top cell. As a result, there will be no trace outcomes. This  can be explained because the analyzer will terminate its trace  at the encounter of a device or transistor; in other words, it  does not trace beyond the first-level. Therefore, manual trace  unfortunately, is still superior for a complete analysis even


area of M1>0


though it is well-known to be tedious and time consuming.


L.


S/D


V1口


M2


D91


M19


M1


Figure 5: (a) Two net traces relating three cells and (b) illustration of the connection between standard cell A and B.


Automated Layout Trace Concept


N+N+N+N+


Design Rule Check


P-sub


Time-resolved waveforms


Since each photon is precisely time-tagged by the timing  electronics. Full TRE waveforms can also be generated from  any pixel, or group of pixels, of the acquire dataset, as shown  in Fig. 14. An overall average jitter of ~60 ps-FWHM (Full  Width at Half Maximum) is observed in the waveform. This  allows to measure a stage-to-stage gate delay of ~5 ps.


In this paper, we have presented the first prototype of a  Scanning Time-Resolved Emission (STRE) system using an  SSPD and a modified LSM scanning head. The system can be  used to construct very useful pseudo 2D images of several  different features of the TRE coming from the sample. After  discussing the principle of operation and key features of the  system, we have presented preliminary data acquired from a test  chip fabricated in 32 nm SOI technology node. Although the  system suffers from several known inefficiencies and bottle  necks, it was able to show promising results in both frequencyand time-domain analysis. The low jitter of the SSPD allows for  very precise delay measurements of few Picoseconds.


The authors would like to thank A.J. Weger, S. Kim, D. Maliuk, H.A. Ainspan, Y. Kwark, C.W. Baks from IBM for their work  in designing the test chip and test board used in these  experiments. The authors would like to thank H Iida, T. Nakamura, M. Takeda from Hamamatsu Photonics for  designing the new scanner head and providing the  Superconducting Single-Photon Detector (SSPD).


[1] F. Stellari et al., “Method and apparatus for creating time-resolved emission images of integrated circuits using a single-point single-photon  detector and a scanning system”, US 8,115,170.


[2] S. Polonsky, A. Weger, and M.K. McManus, “Picosecond Imaging  Circuit Analysis of Leakage Currents in CMOS Circuits”, Int. Symp. for  Testing and Failure Analysis (ISTFA), 2002.


[3] F. Stellari et al., “Circuit voltage probe based on time-integrated  measurements of optical emission from leakage current”, Int. Symp. for  Testing and Failure Analysis (ISTFA), 2002, pp. 667-672.


[4] F. Stellari et al., “Testing and Diagnostics of CMOS Circuits Using Light Emission from Off-State Leakage Current”, IEEE Trans. on Electron  Dev., vol. 51, no. 9, 2004, pp. 1455-1462.


[5] S. Polonsky et al., “Photon emission microscopy of inter/intra chip device  performance variations”, European Symp. Reliab. of Electron Devices, Failure Physics and Analysis (ESREF), 2005, pp. 1471-1475.


[6] F. Stellari, P. Song, and W.D. Becker, “Local Probing of Switching Noise  in VLSI Chips using Time Resolved Emission (TRE)”, North Atlantic  Test Workshop (NATW), 2005, pp. 130-137.


[7] F. Stellari et al., “Optical diagnosis of excess IDDQ in low power CMOS  circuits”, European Symp. Reliab. of Electron Devices, Failure Physics  and Analysis (ESREF), 2002, pp. 1689-1694.


[8] S. Polonsky and K.A. Jenkins, “Time-resolved measurements of selfheating in SOI and strained-silicon MOSFETs using photon emission  microscopy”, IEEE Electron Dev. Lett., vol. 25, no. 4, 2004, pp. 208-210.


[9] A.J. Weger et al., “Device channel temperature measurement using NIR emission”, Int. Symp. for Testing and Failure Analysis (ISTFA), Pasadena, CA, 2017.


[10] J.A. Kash and J.C. Tsang, “Dynamic Internal Testing of CMOS Circuits  Using Hot Luminescence”, IEEE Electron Dev. Let., vol. 18, no. 7, 1997, pp. 330-332.


[11] W.G. McMullan et al., “Simultaneous subnanosecond timing information  and 2D spatial information from imaging photomultiplier tubes”, Rev. Scientific Instr., vol. 58, no. 9, 1987, pp. 1626-1628.


[12] S. Thompson et al., “A 90 nm Logic Technology Featuring 50nm Strained  Silicon Channel Transistors, 7 Layers of Cu Interconnects, Low k ILD,and 1um² SRAM Cell”, Tech. Dig. Int. Electron Dev. Meeting (IEDM),


2002.


[13] S. Rusu et al., “Backside infrared probing for static voltage drop and  dynamic timing measurements”, ISSCC, 2001, pp. 276-277.


[14] Rowlette et al., “Hot carrier emission from 50 nm n- and p-channel  MOSFET devices”, LEOS, 2003, pp. 740-741.


[15] U. Kindereit et al., “Comparison of Near-Infrared Photon Emission  Spectroscopy of a 45 nm and 32 nm SOI Ring Oscillators”, ISTFA, 2012, pp. 128-134.


[16] F. Stellari et al., “Evaluating PICA capability for future low voltage SOI  chips”, Int. Symp. for Testing and Failure Analysis (ISTFA), 2008, pp. 407-416.


[17] W.K. Lo et al., “Next-generation optical probing tools for design debug  of high speed integrated circuits”, Int. Symp. for Testing and Failure  Analysis (ISTFA), 2002, pp. 753-762.


[18] F. Stellari et al., “Time-resolved optical measurements from 0.13 m  CMOS technology microprocessor using a Superconducting SinglePhoton Detector”, Int. Symp. for Testing and Failure Analysis (ISTFA), 2003, pp. 40-44.


[19] F. Stellari et al., “Superconducting Nanowire Single-Photon Detector (SnSPD) system for ultra low voltage Time-Resolved Emission (TRE) measurements of VLSI circuits”, Int. Symp. for Testing and Failure  Analysis (ISTFA), 2013.


[20] F. Stellari et al., “A position sensitive single photon detector with  enhanced NIR response”, Int. Symp. for Testing and Failure Analysis (ISTFA), 2011.


[21] Y.S. Ng et al., “Laser Voltage Imaging: a new perspective of Laser Voltage Probing”, Int. Symp. for Testing and Failure Analysis (ISTFA), 2010, pp. 5-13.


[22] T. Elies and P. Pardy, “Visible Laser Probing (VLP) with GaP solid  immersion lens demonstrating 110nm resolution in common laser probing  applications”, Int. Symp. for Testing and Failure Analysis (ISTFA), 2016.


[23] A. Bahgat Shehata et al., “Superconducting single photon detector brings  back light to time-resolved emission testing of ICs”, Elec. Dev. Failure  Analysis (EDFA) Mag., vol. 18 no. 4, 2016, pp.16-22.


[24] F. Stellari et al., “Tester-based methods to enhance spatial resolvability  and interpretation of time-integrated and time-resolved emission  measurements”, Int. Symp. for Testing and Failure Analysis (ISTFA), San  Jose, CA, 2013.


[25] F. Stellari et al., “Testing of ultra low voltage VLSI Chips using the  Superconducting Single-Photon Detector (SSPD)”, European Symp. on  Reliab. of Electron Dev., Failure Physics and Analysis (ESREF), 2004, pp. 1663-1668.


[26] X. Michalet et al., “New photon-counting detectors for single-molecule fluorescence spectroscopy and imaging”, SPIE Int Soc Opt Eng., 2011. --


[27] A.J. Weger et al., “32nm CMOS SOI Test Site for Emission Tool Evaluation”, Int. Symp. for Testing and Failure Analysis (ISTFA), San  Jose, CA, 2013.


67


A study of clustering for the enhancement of image resolution in dynamic  photon emission


S. CHEFa, C.T. CHUAa and C.L. GANa,b


aTemasek Laboratories@NTU, Nanyang Technological University, 50 Nanyang Avenue, 637553, Singapore


csamuel@ntu.edu.sg, clgan@ntu.edu.sg


bSchool of Material Sciences Engineering, Nanyang Technological University, 50 Nanyang Avenue, 639798, Singapore


Limited spatial resolution and low signal to noise ratio are some  of the main challenges in optical signal observation, especially  for photon emission microscopy. As dynamic emission signals  are generated in a 3D space, the use of the time dimension in  addition to space enables a better localization of switching  events. It can actually be used to infer information with a  precision above the resolution limits of the acquired signals. Taking advantage of this property, we report on a postacquisition processing scheme to generate emission images  with a better image resolution than the initial acquisition.


Photon emission [1, 2] is one of the key techniques for defect  localization, whether it is to track static or dynamic faults. Besides using it for failure analysis (FA) of microelectronic  devices, its capabilities for the security analysis of IC has been  established with various applications such as memory  descrambling, estimation of logic state of bit cells [3, 4] and  differential power analysis through time resolved photon  emission (TRE) signal [5].


Several detection schemes can be found in literature [6, 7]. Notwithstanding those dedicated to spectral analysis, they can  be classified into two main categories: time integrated schemes  using an image array sensor (e.g. InGaAs or Si-CCD camera  sensor) and time resolved scheme (e.g. gated measurement  Microchannel Plates, Single Photon Diode, Superconducting  Nanowire). The former category provides an image where  emission sources can be localized in the (x,y) plane while the  latter can display data of different dimensions (1D local optical  waveforms with emission as a function of time; 2D images  similar to time integrated schemes or even movies). If the time  resolved measurement brings additional information compared  to standard camera sensor, the detection scheme is more  complex and requires access to some synchronization signals.


Like any optical technique, a precise localization of the source  of signal is a major concern when studying the most advanced  technology nodes. It is challenged by several factors:


- System optical resolution: It defines the capability of the optical system to differentiate two closely positioned neighboring point sources.


- Spatial resolution: It refers to the spatial sampling frequency of the image. For instance, with a camera array sensor, the sampling frequency will be defined by the image area in the image plane divided by the number of pixels. If there is no decimation step in the chain of acquisition, the image resolution of the output image is equivalent to spatial resolution.


- Signal to Noise ratio (SNR): Depending on the properties of the source, the photon emission and detection process may have a low yield, resulting in low SNR from very sparse signal.


In terms of signal theory, the first factor mentioned above is  equivalent to the analog bandwidth of the optical system. It can  be interpreted as a low pass filter. The second factor is the  digital bandwidth of the system. As such, the Nyquist-Shannon  theorem applies and signal of maximum frequency larger than  half of the value of the sampling frequency cannot be resolved. These constitute two of the fundamental limitations of the  digital microscope imaging system.


For IC analysis, strong research effort was put to improve the  optical resolution by adapting immersion microscopy to  semiconductors, leading to the development of current state-ofthe-art Solid Immersion Lens [8]. Besides improvements at the  system level, some recent work developed a post-acquisition  processing approach through deconvolution, which enabled a  better localization of the emission spots [9]. These approaches  remain focused mostly on improving the optical resolution as  in the first case, numerical aperture is improved while the  second case focuses on the estimation of the low-pass filter that  constitutes the optical system.


Linked to the spatial/image resolution limits, one method based  on the observation of multiple low resolution images through  different angles like in tomography [10] was suggested. This  method used a combination of system level improvement (different scheme from standard microscope) and postacquisition processing. Another approach has demonstrated  that better spatial localization can be achieved by comparing  emission signals resulting from different electrical biasing  conditions [11] and performing image subtraction operations. Dynamic photon emission signals result from a discrete random  process generated by the local electrical activity. As such, they  are defined by 3 dimensions: 2 spatial coordinates (x,y) and 1  time coordinates (t). The approaches mentioned in this


# A study of clustering for the enhancement of image resolution in dynamic photon emission


68


paragraph focused mostly on the space dimensions to recover  information with a precision beyond the spatial resolution limit  of the acquisition scheme via an image processing framework.


Integrated circuits are complex system and they can integrate  analog and digital parts, combinational or sequential logic  circuits. Even with the capability to perform 3D measurements, photon emission observed from these circuits can be complex  and rarely results from a single source. For instance, if a  combinational logic circuit is considered, a change on one input  triggers a switch from all the gates constituting the circuit and  thus within the field of view, many sources may exist.


Previous work on processing data in (x,y,t) space has  demonstrated that it is actually possible to pinpoint time and  place when an odd emission event happens by analyzing  statistical properties of clusters of photons [12]. A cluster  designates all the photons that are generated from the same  event and node. By formulating some hypothesis on the various  probability laws they may follow, a higher resolution model can  be generated from the observation. From this idea, we report a  study on a processing scheme based on clustering and Gaussian  interpolation to improve photon emission image resolution.


Resolution enhancement process


Overview of dynamic emission signal


Photon emission is a discrete random process that requires both  current and voltage to occur. As these quantities change through  time, photon emission probabilities vary too. In digital CMOS  circuits, a larger quantity of photons is generated during the  switching of transistors from one state to another. This is mostly  due to the fact that for this short period of time, transistors are  operating in saturation mode, which is the most favorable state  for photon emission (high current and voltage). In DC biasing  conditions, depending on the technology, off-state leakage  current may be significant enough to generate a detectable  signal. However, when transistors switch, faint emission from  leakage current is less intense than switching emission. In  addition, not all of the transistors may emit at the same time. It  depends on various external and internal parameters such as  input/test signal, design, and propagation delay. As a  consequence, if we consider a (x,y,t) space, photons emitted  during the switching of a single node are well localized around  specific locations that match the place where and the time when  the switching occurs.


The schematic in Fig. 1 illustrates this principle. For this  example, a hypothetical inverter chain consisting of four  inverters is considered with a pulse signal on its input. The  schematic in Fig. 1(a) only considers the time dimension for the  whole area. As there is only one pulse at the input, two spikes  of emission are expected, matching with the two changes of  state. Fig. 1(b) shows the results expected after integration of  the photons in the (x,y) plane. This is similar to standard  emission image generated by time-integrated camera sensor  such as InGaAs camera. In this mode of acquisition, four spots, each matching one inverter, should appear. If resolution  parameters allow it, there should even be possibilities to


distinguish emission from the NMOS and PMOS transistors  which make up the inverters.


Figure 1: Schematic of the different ways of representation of  data and signal in dynamic photon emission. (a) In time  domain. (b) In space domain. (c) In (x,y,t) space.


Finally, if both time and space dimensions are considered, then  there should exist dense groups of photons which match with  the time and place where the switching occurs (Fig. 1(c)). In  such mode of representation, photons resulting from nonelectrical activity (i.e. noise) are randomly located in the 3D  space while photons resulting from gate activities are densely  located around the time and place where this activity occurs. An  example of real data acquired from an 8-bit microcontroller is  reported in Fig. 2. A densely localized population of photons is  circled in red and illustrates the concept discussed in this  paragraph. Noise can be seen as more spread out within the  representation space.


69


Figure 2: Example of densely localized emission from switching  activity. Photons were acquired on an 8-bit microcontroller. The red circle indicates the dense area.


Since photon emission is a discrete random process, photons  generated during a specific event belong to the same  distribution. It must then follow a specific probability  distribution and a probability density function (PDF) can be  associated with each of them. Being a theoretical model, the  PDF can then be generated at a higher spatial resolution than  what the observation is.


At this juncture, two questions remain to be solved to take  advantage of this phenomenon:


(a) How to detect groups of photons generated by the  same event in dynamic photon emission and  differentiate signal photons from noise?


(b) What model of PDF should be chosen to generate a  higher resolution image?


Localization and labeling of photons belonging to the same  emission event


In the previous section, it has been concluded that photons  generated from electrical activity are more densely localized in  time and space. This property has been explored [12] for  filtering but it did not focus on automated identification of  groups of photons emitted during the same event.


In view of the data, machine learning can be considered for this  task. The choice of a family of algorithms (e.g. supervised or  unsupervised learning) depends on the inputs that the end-user  can provide. Previous studies [13, 14] on dynamic photon  emission showed that density-based clustering algorithms [15] such as DBSCAN [16] can provide good results to identify  clusters of photons resulting from the same switching activities  while handling noise. As a conclusion, density-based clustering  seems well suited to identify the groups of photons in this study.


Estimation of the PDF from clusters


In microscopy, any point source of light with dimensions which  are below the optical resolution of the system generates a shape  known as Airy disk. Considering all the signal estimation errors  generated by the acquisition system, this function can be


approximated by a Gaussian function. In view of this, it can be  assumed that the photons emitted by a single point source (e.g. transistors or groups of transistors) with dimensions below the  optical resolution of the system follow a Gaussian profile.


In IC analysis, photon emission is a random process that  depends on many factors (e.g. local electrical field, current  intensity, transistor dimensions) and so is the detection in single  photon counting. As a result, upon detection, emission signals  are very sparse. In spite of this, if the emission follows a  Gaussian profile, a stronger intensity can be expected at the  center of the emission spot and spreading parameters may  follow what the optical system bandwidth allows to.


As modern microscope imaging systems generate a digital  image, this Gaussian profile is further digitized and the  observation quality is decimated by the noise of the detection  scheme. As a consequence, in the (x,y) plane, a single emission  source may not follow a Gaussian profile in an obvious manner.


Photon counting process is a random sampling process. It can  be assumed that detected photons constitute random  observations of the same Gaussian distribution. As with any  statistical process, if a large enough sample of a phenomenon is  available and if it follows a known probability law, then  parameters of the distribution can be estimated with good  precision. As a consequence, even if photon emission of a  switching event is a very sparse signal, statistics can be  computed and it can be interpolated in the (x,y) space using a  2D Gaussian function with parameters (µ, Σ). These designate  the mean and the variance-covariance matrix of the distribution, which are computed from the clusters of photons. From these  parameters, an image of higher resolution that what the  detection scheme allows, can be estimated.


Clustering and interpolation process


The interpolation follows the process below:


1. Observation of the properties of emission signals to  identify parameters for clustering.


2. Application of the clustering algorithm.


3. Estimation of statistics (µ, Σ) for each cluster.


4. Generation of a 2D Gaussian function using the (µ, Σ) previously computed.


5. Summation of the Gaussian functions in the (x,y) plane.


As mentioned previously, for IC analysis, clustering algorithm  such as density-based spatial clustering in applications with  noise (DBSCAN) has shown its efficiency. In this study, the  spatio-temporal variant (STDBSCAN) is used [17]. As a quick  reminder, the DBSCAN algorithm first seeks for the points with  the larger number of neighbors within a radius defined by the  end-user. If a point has a weight larger than a user defined  threshold (referred hereafter as MinPts), it is labeled as a core  point and a cluster is initiated. All the points that can be reached  from this core point are assigned to the same cluster. For more  details about these algorithms, readers can refer to [16, 17].The


STDBSCAN version requires two different radius for the  estimation of weight: one in space (hereafter EpsXY) and one  in time (hereafter EpsT). First, time and space are two different  dimensions, hence computing a distance metric cannot be  achieved without further transformation (e.g. standardization). In addition, even after transformation, one of the dimensions  may weigh more than the other and thus biasing the distance  estimation process and resulting in wrong results. In order to  keep coherence with physical quantities and minimize errors, using two different parameters for space and time appear to be  more appropriate.


The parameters can be determined from observations of the  data, experiment setup and knowledge of the DUT. For  instance, studying a circuit manufactured using older  technology, longer rising and falling edges can be expected as  compared to a state-of-the-art IC. Along time axis, photons are  more spread out for the older technology, hence a larger EpsT  parameter has to be chosen. In (x,y) space, due to the optical  setup and sensor resolution, if a pixel matches with several tens  of micrometers, a EpsXY parameter of 1 pixel is appropriate,


XY Scanning Mirror


Beam SplitterOscilloscope


as a single pixel matches with many transistors.


From the different clusters, the parameters for the estimation of  the PDF can be estimated by various methods such as least  squares or maximum likelihood estimation (MLE). In this  work, the MLE is used. For a normal distribution, it is  equivalent to the empirical estimation of mean and variancecovariance.


Input


For 2D Gaussian distributions, the PDF is defined as:


SOM


  (  ) =           (−    (   −    )′  −  (   −  ) ),


ID230


where µ designates the vector of the coordinates of the center  of the distribution and Σ is the variance-covariance matrix. The  amplitude parameter A is defined as:


   =


    √      (  )


where the operator det() designates the determinant of the  matrix.


Application and results


TRE Instrumentation and database generation


All acquisitions were performed using a customized setup of  the Semicaps SOM1100. Photons are detected by a free running  single photon sensor (ID230 from ID Quantique [18]) connected to one of the fiber ports normally used for laser  scanning. This configuration is usually dedicated to single point  TRE measurement and not to perform an extensive scanning of  areas. However, in order to demonstrate proof of the concepts  discussed in the previous section, the XY scanner laser scanner  was used to generate the (x,y,t) photons measurement. This  measurement approach allows multiple choices of image  resolution or zoom factor by changing the appropriate set of  parameters as it is possible for laser scanning-based  applications (e.g. OBIC, LIVA, etc.). The image resolution


indicates the number of measurements performed in the area  while the zoom parameter defines the size of the area that is  scanned. For instance, if a scan is performed with a zoom factor  of 1, then the full field of view allowed by the objective lens is  scanned. With a zoom factor of 2, the area scanned is half the  size of the previous one. If the same image resolution is  requested for two different zoom factors (for instance 512 x 512  pixels), then the scanning step (which defines the spatial  resolution) between two subsequent measures is divided by 2, hence the spatial sampling frequency increases by 2. The  impact of these parameters on the suggested processing scheme  is further explored in the Discussion section.


A schematic of the measurement setup is available in Fig. 3. The optical path includes a polarizing beam splitter near the  fiber input/output normally used in laser applications. This  reduces the number of photons that can actually reach the sensor  and is one of the major drawbacks if we want to keep the  possibility of switching fibers, depending of the application.


Figure 3: Schematic of the measurement setup.


The usual scheme found in time-correlated single photon  counting applications includes a counting module which  records the time of arrival of photons with regard to a reference  signal (e.g. test loop trigger in IC analysis). In our case, such  module was not available and thus we used an oscilloscope (LeCroy WaveMaster Zi-808B) to register the time of arrival of  each photon. A synchronization signal was connected to both  the scanner of the SOM and the oscilloscope, in order to record  the location where the photons were acquired. The oscilloscope  was set to trigger on the detection pulse generated by the sensor. This approach minimizes the number of missed detection pulses  compared to a trigger on the test loop signal. The oscilloscope  then measured the duration between the rising edge of the test  loop signal and the rising edge of the photon detection pulse and  stored this value. Upon completion of a scan, it only requires to  transfer the recording of this value for further processing. This  approach saves storage space. Example of the measurement by  the oscilloscope is available in Fig. 4. The ph parameter  indicates the measurement of the time of detection of the photon  with reference to the test loop.


71


F2


Figure 4: Example of photon counting and referencing by the  oscilloscope. C1: Test loop signal. C2: Photon detection pulse  from the sensor. F1: Recording trace of the measurement of the ph parameter. F2: Preview of the photon counting histogram  generated from F1. TimeBase for C1 and C2: 500 ns/div. Vertical Scale: 2 V/div.


The scanning speed (or dwell time - time spend per pixel) has  to be defined as a trade-off between total scanning duration and  signal to noise ratio of the TRE waveforms. In order to do so, properties of the detector have to be considered. After detecting  a photon, the sensor has a dead time of approximately 20 µs. For this setup, the oscilloscope performs all the recording and  thus it also plays a part in the acquisition speed. In standard  trigger mode, the oscilloscope needs to be rearmed before  triggering again. In our experiments, we observed duration  between two consecutive triggers ranging between 5 ms to  several hundreds of ms, meaning that potentially, many photons  detected by the sensor may have been neglected by the  oscilloscope. In view of this, the oscilloscope is the main  bottleneck in this study. Once again, the use of dedicated  photon counting module would mitigate this issue and allow a  faster scanning speed. Once the scanning of the whole area is  completed, a database of the coordinates (x,y,t) of each detected  photon is generated.


Test conditions and device under test


To test the validity of the approach, some signals were acquired  on a Xilinx Kintex 7 FPGA [19], manufactured in 28 nm  technology. The device was mounted on a Skoll Kintex 7 board   from Numato Lab [20]. As it is packaged in flip-chip with no  molding compound, very little sample preparation had to be  done on the circuit. Some thinning (few tens of microns) of the  substrate was performed to remove the marking on top of it. Prior to the removal, substrate thickness was estimated to be  700 µm.


The circuit was programmed to execute a simple inversion  function. The input received a square signal (1.2 V, 5 MHz, 50% duty cycle). A periodic pulse signal of 100 ns with a  frequency of 1 MHz constituted the time reference to measure  the time of arrival of photons by the oscilloscope.


|||||Tph||||
|---|---|---|---|---|---|---|---|

C2


F1


Figure 5: Emission image overlay onto the device micrograph. Both images were acquired using the InGaAs camera and the  50X objective lens (NA 0.4). The red square indicates the area  chosen for TRE investigation.


Figure 6: Zoom of the area, previously marked out by red  square in Fig. 5 that was further investigated.


As this is a commercial product and no design information (other than the floorplan in the FPGA development software) was available, the area of interest was first identified using the  SOM InGaAs camera (Fig. 5). Based on the floorplan, this area  is related to the IO. A zoom of the area (set to scale with regards  to the laser scanner area) is shown in Fig. 6.


The area was scanned with a resolution of 32 x 32 and a dwell  time of 2 seconds per pixel. A total of 72729 photons were  collected. From the photons database, the photon counting  histogram of the whole area was computed (Fig. 7).  It shows 5  periodic groups of spikes, matching with the input signal of 5  MHz with regards to the time reference (1 MHz). A photon  counting image (i.e. 2D photon histogram) was generated by  counting the number of photons detected at a specific  location/pixel (Fig. 8). The resolution of this image is the same  as the scanning resolution and will be considered in the


72


remaining of this paper as the low resolution image. On the 0 figure, the coordinates are computed according to the field of


250


view of the acquisition area to provide a reference after  clustering and interpolation.


山


、8


250-


8 u


0 0 0


人


40 45


100-


05101520 25 30 352940 45


30 25


x105


Figure 7: Photon counting histogram (i.e. TRE signal) of the 0 complete area.


The clustering algorithm was then applied to the data with the


following parameters: EpsT = 20 ps, EpsXY = 1 pixel, Minpts = 3.


0O15


The parameters were chosen by observing the distance to the


s20


nearest neighbors. After clustering, only 847 photons in the


e u25


database are classified into 216 clusters. The others have been p labeled as noise. The clustering parameters to identify core


30 points are quite stringent and as a result, many clusters were >35 constituted of the minimum point requirements. It is possible


that due to the multiple photon densities existing in this area,


Laser stimulation techniques also have a long history for  latchup investigations. [10-15]. As mentioned above, using a  CW laser typically requires that the device latchup margin be  reduced by some means, else laser-induced damage may occur  before latchup can be triggered. Biasing the supply voltage  close to Vtrig is one way to do this [14]. For our debugs, this  also helps ensure that we actually target the Vtrig limiters of  interest, versus unrelated secondary issues. However, the high  power-dissipation of an IC that is DC biased near Vtrig can  result in self-heating, thermal runaway and subsequent latchup  behavior independent of any externally applied triggers such  as the laser beam. Another complication is the potential for  device damage if a latchup event is left to progress unchecked  at such high biases. Means to rapidly quench the latchup event  and/or limit the supply current is required.


Weichold, et al., worked around both issues by biasing the  DUT using an AC waveform with Vmin = 0 V and Vmax near  Vtrig [14]. A Lock-In Amplifier (LIA) synchronized to the  modulation frequency was used to monitor the DUT current. A visible-light CW laser was then scanned over the frontside  of the DUT to trigger latchup at any sensitive sites. Image  contrast was provided by the in-phase signal of the LIA which  was responsive to the high current draw induced by latchup. Because the AC waveform dropped to 0 V during each cycle, any latchup event induced during the cycle was automatically  terminated. We implemented a similar biasing scheme, except  the high power-dissipation of our DUT required much lower  duty-cycle operation to achieve long-term stability. We were


87


also able to use a bench oscilloscope monitoring Vdd instead  of a LIA monitoring current to generate the latchup flag.


More recently, Llido, et al., reported the combined use of  PEM and 1064 nm CW laser stimulation to identify designrelated latchup triggers and latchup sites in a 90 nm  technology microcontroller [10]. They DC biased the DUT  and first scanned it with the laser while monitoring the supply  current to identify latchup trigger sites. Then, PEM images of  the DUT were acquired after latchup was triggered by the  laser at the individual sites to identify the structures  undergoing latchup. DUT damage was prevented by biasing  the DUT nominally and current limiting the power supply. The whole procedure was computer controlled, including  resetting of the DUT after latchup and generating the latchup  flag for the laser stimulation system. Since our debugs  required biasing the DUT to near Vtrig, it wasn’t possible to  use the DC biasing scheme required with this technique, again, because of the high power dissipated in the DUT.


V-Pulse Technique


Previous attempts by us to use DC biasing near Vtrig resulted  in thermal runaway and erroneous isolations, even with chilled  forced-air cooling. With the latest processes, DUT power  dissipation at such high biases can be well over 100 W/cm^2. The use of a temperature-controlled plunger on full-thickness  parts prevents device damage during ATE testing. However, our isolations required that the DUT be thinned to 50 µm and  the backside exposed for optical access. As a result, we had to  develop a new methodology based on low duty-cycle pulsing  of the DUT’s voltage rail. In this section, we describe this ‘V-Pulse’ technique in detail.


Figure 1 shows a block diagram of the V-Pulse setup for laser  stimulation studies. Its description will be split into three  parts: Vdd voltage-pulse generation, latchup flag and pixelclock generation, and latchup quenching and persistence  effects. This will be followed by a brief description of the  simplified setup suitable for PEM-only studies.


Vdd Voltage Pulse Generation


Referring to Fig. 1, a Function Generator is used to drive Vdd  of the DUT via a Current Amplifier to increase drive strength. According to the manufacturer, the amplifier can both source  and sink > 5 Amps of current, has 1 MHz maximum frequency  response and 16 V/µs maximum slew rate [20]. Up to three  units can be ganged (i.e., connected in parallel).


The Function Generator is set to output a low duty-cycle pulse  train which results in a train of current pulses to the DUT. The  width of the current pulses out of the amplifier tracks the  Function Generator’s output, as shown in Fig. 2. Pulse widths  can be set with <0.1 µs resolution. The amplitude of the pulses  out of the Function Generator is somewhat arbitrarily set at  7 V, much higher than the Vtrig values of our DUT. The  Current Amplifier also attempts to track this value but is  internally current limited for the pulse durations used due to


the high loading of the DUT and DUT Card. The Current  Amplifier therefore operates as a quasi-constant-current  source.


To ensure good manufacturability of silicon chips according  to intended layout specifications, a procedure known as  design rule check parses the layout and screens different  attributes such as polygon width, spacing or overlap as shown  in figure 6, just to name a few. A run deck which consists of a  set of appropriate design rules is developed to accomplish this  task. The Mentor Calibre DESIGNrev is one of the  mainstream tools for this purpose.


Figure 6: Some examples of design rule check.


Implementation of Automated 1st Level Trace


The concept of design rule check can be extended to realize  automated net tracing. For example, the Net Area Ratio rule  can be used to perform a first-level trace. This rule checks for  a pre-determined percentage in area overlap between 2  specified layers which are electrically related. Consider a  starting trace point on M1 and a criterion defined as follows:


area of V1


V1 (vias above the first metal layer) that are electrically  connected to the M1 net polygon of interest as shown in  figure 7(a) will be highlighted. The same procedure applies  on M1/ M2 to highlight the M2 polygons that are electrically  related to the M1 source net as shown in figure 7(b). Figure


C0H!H


7(c) shows a cross-sectional view of the trace connection.


tEHIFETH


国Gate


This example illustrates a simple way to automate net tracing


Gafe 03TwoBox:02


using design rules. The coordinates and corresponding layer


科*


of a starting trace point (eg. Coord X, Coord Y, Layer M1)


aHFT


has to be provided as a prerequisite.


NAU技


种胜


Figure 7: Simplified diagrammatic representation on the  application of Net Area Ratio rule to (a) M1/V1 and (b) M1/M2. (c) Cross-sectional perspective of a net trace from  M1 to M2.


Implementation of Automated Multi-Level Trace


For a net trace to proceed beyond a transistor node, the main  challenge lies in transferring the trace across a gate to the


The three basic DRC checks


source/drain nodes (or vice versa) which are not electrically


Width


coupled due to the presence of the oxide layer. In this case,


Enclosure


the simple Net Area Ratio rule does not work. To achieve  this, another rule is applied. The RX (active layer) Interact  Poly (polysilicon layer) rule seeks the RX layer that overlaps  with the highlighted poly of the interested transistor as shown


Spacing


in figure 8(a). Figure 8(b) shows the RX layer that is  identified in this procedure. Thereafter, the Net Area Ratio  rule can be applied again to determine the contact node of  interest for the next stage of tracing. This explains how net  tracing beyond active devices can be realized. More .svrf


81


scripting rules [8] are involved to implement the multi-trace  methodology but will not be elaborated further. The rules are  written into macros and referred to as layer operations in the  automated tracing workflow as shown in figure 9. These  macros are called iteratively to implement the automated net  trace capability until all the pre-determined probe points and  number of trace levels is fulfilled. In this work, the Mentor  Calibre DESIGNrev tool is used.


Figure 8: Simplified representation of (a) a highlighted poly  and (b) the identified RX layer after applying the Interact  rule to the polysilicon and active layers.


Figure 9: Flowchart for multi-level net trace.


Proposed Net Trace Concept


With reference to figure 10, consider a test case involving  three hotspots (labeled as HS1 - 3). HS1 is identified as the  starting trace point. By conventional manual tracing, an FA  analyst is required to iteratively toggle between high  magnification to identify the location for incremental trace  and low magnification to inspect the overall trace paths on


the bird’s eye view perspective. In an ideal scenario where the


hotspots are related by buffers, tracing simply involves  multiple steps of polygon selection. However, when a traced  net fans out, the situation becomes more complicated. Additional decision-making on the nets selection and retracing in the event of wrong choices are inevitable.


In the proposed approach, layout coordinates based on  hotspots, process layer that correspond to the starting trace  coordinates as well as the number of trace levels, are required  as probe details. Upon a script execution, the Calibre tool  automatically traces up to four levels in this case and then  terminates. Layout analysis is conducted at the bird’s eye  view perspective that encompasses all the hotspots without  the need to change the magnification. The FA analyst then  activates the net trace level incrementally and observe how  they fan-out and relate to the vicinity of the hotspots. It is  clear from figure 10 that HS1 and HS2 are related by the first  level trace while 4 levels are needed to connect to HS3. There  is a threefold advantage in the proposed trace concept. Besides automation and the convenience of analyzing at a  fixed field of view, this approach eliminates the need for  decision making on the fan-out net to trace. The result is a  drastic improvement in the turnaround time from days to  hours so that more emphasis can be placed on analysis rather  than manual tracing.


Figure 10: Panoramic view of incremental traced nets.


A case of a 40 nm technology device failing memory built-inself-test (MBIST) will be presented. It involves 6 multiple  hotspots in the peripheral logic as shown in figure 11. Figure  12 shows their respective cell locations on layout (indicated  from A-F with bounding boxes). The manual trace approach  and proposed methodology are compared.


82


tooum


Figure 11: Dynamic photon emission micrograph under (a) 50X and (b) SIL objective lens.


0 Figure 12: Overview of 6 emission hotspots locations on  layout (labelled as A-F).


Conventional Approach


Consider the starting point for trace at cell E. Using the  manual trace approach, relevant gates and active diffusion  nodes are identified. To proceed, there are two trace  possibilities, namely from the source/ drain to the next cell (defined as forward) or from the gate to the preceding cell (defined as backward), as shown in figure 13(a) and (b) respectively. It was found that the forward trace yields no  meaningful result in the first-level trace and not advanced  further. The backward trace connects to cell D as shown in  figure 13(c). A second-level trace backwards connects cells D  to C. It is also observed from figure 13(c) that the secondlevel trace fans out. Tracing from this point onwards will  involve iterations of trial and error.


Backward


50X


si


宁


Memory cells


2nd用


。D'st


Figure 13: Custom method of net tracing (a) forward from  source/ drain and (b) backward from the gate of standard  cell at E. Cell E connects to cell D in the first-level trace. (c) Second trace level connecting cells D and C.


Proposed Approach


Automated multi-level tracing is employed. The starting trace  locations for all the 6 hotspots are identified and executed in


F


parallel. The number of trace levels is set to 5. The entire


姣姣姣姣蚊蚊蚊蚊蜕蚊姣姣姣


trace process lasts slightly more than an hour. During


analysis, since the objective is to observe the relationship of


Cb9D


the traces with respect to the hotspots, the process layers can  be disabled, leaving only the bounding boxes and traced nets


A88


as shown in figure 14. This action has the effect of enhancing


90909999998999999999999999


the visual contrast without distractions of underlying process  layers. The field of view is also appropriated to encompass all  the hotspots. Figure 14(a) shows the first-level trace forward  from cell E and F with the other traces disabled as shown by  the strikethrough in the legend. Figure 14(b) shows the  second-level trace that suggests a possible relationship which  was later found to be just nets passing in close proximity, hence omitted for further analysis. The rest of the images in  figure 14 depict the incremental trace steps backwards. Eventually, all, except cells A and B are found to be related as  shown in figure 14(d). However, this is not sufficient to  explain all the signals. The first-level traces from cells A and  B are then enabled and both are found to be related as shown  in figure 14(e). Overall, although there are no common nets  that can be identified, at this high level panoramic view, it is  not difficult to observe a group of traces that appear to pass  through in close proximity (encircled in figure 14(e)). Figure  15(a) shows the zoom-in view of the suspected fail site in the  layout and figure 15(b) shows the open metallization defects  due to a particle in that locality on physical inspection. This  test case demonstrates the advantages of performing analysis  at low magnification as well as the importance of


E用目:*a


COCIN


管理


重量**


emphasizing the analyst’s effort into examining the traces


instead of the actual tracing activity.


3g88


on


e推引


che


Forward


*。


a二二作a=


**


83


|6|||
|---|---|---|

|*.............|||

?


99


(e)


Figure 14: First 5 trace levels using automated tracing (a)-(e) respectively. The 6 emission hotspots are indicated.


9即9


??


Figure 15: (a) Zoom-in on the nets encircled in figure 14(e) and (b) SEM image showing open metallization defects.


The second case involves a large chip (spanning ~8 mm) which fails for embedded memories functionality. Dynamic


photon emission microscopy is employed and the results are  shown in figure 16. Obvious differences are observed in the  emission micrographs between failing and passing dies as  shown in figure 16(a) and (b) respectively. Two anomalies are  encircled in figure 16(a). Based on further test and design  inputs, one of the abnormal signals together with a pad signal  as shown in figure 17(a), are found to be suspicious. The next  step requires establishing a possible relationship between  these signals.


00


1mm


Figure 16: Emission micrographs of (a) failing and (b) passing dies.


84


(f)


Figure 17: (a) Signals of interest. (b) – (f) First five trace  paths starting from the pad. The traces are overlay onto the  emission micrograph of a typical failing die.


The two signals are found to be more than 6 mm apart. At  this distance, tracing using custom approach can easily take  at least 1-2 days. By employing the proposed automated  multi-level trace method, the time taken is drastically reduced  to about an hour. The net traces are enabled incrementally  and observed at a low magnification. It is evident that the  signals of interest are related at the 5th trace level. Again, this  test case clearly demonstrates the value proposition.


We develop an enhanced approach to perform net tracing. It  is automated and more importantly, enables tracing beyond  the first-level across transistors. This multi-level tracing  concept is achieved using modular standard design  verification rules written as a workflow in the form of an  executable script. In principle, there is no limit to the number  of trace levels but because of the fan-out nature of higher  level nets, it is useful to analyze the traces incrementally. It is  worthy to highlight that the developed approach disregard  traces to Vdd and Gnd which are considered nuisances in net  trace analysis. The above advantages address limitations that  exist in current state-of-the-art net trace solutions.


|pad|□ ROI|
|---|---|

|(a) |(a) |

|(b) |(b) |

|(c) (d) |(c) (d) |

|(e) |(e) |

[1] EI Cole, P Tangyunyong, DA Benson, DL Barton, “TIVA and SEI developments for enhanced front and  backside


interconnection


failure


analysis”, Microelectronics Reliability, Vol 39, Issues 6–7, 1999, pg. 991-996.


[2] WY Cheng, TY Chiu, Jon C Lee, JY Chiou, “Laser  Based Defect Localization for the Failure Analysis of  Advanced Product”, Proc Int Symp for Testing and  Failure Analysis, 2006, pg. 230-233.


[3] SH Goh, et al., “Effectiveness of frequency mapping on  28 nm device broken scan chain failures”, The Review of  scientific instruments, 83(2):023702, 2012.


[4] SH Goh et al., “Comparison of Photon and Thermal  Emission microscopy for Dynamic Fault Isolation”, Proc  Int Symp on the Physical and Failure Analysis of  Integrated Circuits, 2015.


[5] CK Ang Chung Keow, H Ismail, WC Lee, “Logic circuit  failure analysis & micro-probing on floating signal net”, Proc Int Symp on the Physical and Failure Analysis of  Integrated Circuits, 2018.


[6] SJ Cho, et al., “Logic failure analysis 65/45nm device  using RCI & nano scale probe”, Proc Int Symp on the  Physical and Failure Analysis of Integrated Circuits,


2009.


[7] VK Ravikumar, et al., “Laser voltage probing in failure  analysis of advanced integrated circuits on SOI”, Proc Int  Symp on the Physical and Failure Analysis of Integrated  Circuits, 2012.


[8] Mentor, “Calibre Verification User's Manual – Read”, http://read.pudn.com/downloads218/ebook/1028073/calb r_ver_user.pdf, 2006.


V-Pulse Technique For Optical Isolation Of Latchup Triggers In Sub-14 nm Standard-Cell Logic And Memory


William Lo, Puneet Gupta, Yen-Tzu Lin, Rakshith Venkatesh, Rudolf Schlangen, Jane Li, Chuan Zhang, Howard Marks, and Bruce Cory


NVIDIA, Santa Clara, CA, USA   wilo@nvidia.com


High core-Vdd overvoltage latchup margins in CMOS ICs are  required to enable many reliability screens (e.g., DVS and  HTOL testing). We introduce an efficient way to isolate  defects that degrade these margins using PEM and  1064/1340 nm CW laser-stimulation. Current pulses from a  current amplifier are used to rapidly charge and discharge the  DUT power rail to repetitively ramp Vdd to (or near) the  latchup threshold. The characteristic drop in Vdd when  latchup is induced is used to generate a latchup flag for laserstimulation mapping. Latchup events are automatically  terminated and latchup durations are minimized, leading to  high stability/repeatability of the technique. Isolations down to  the cell level were successfully performed in sub-14 nm  FinFET test vehicles. This level of isolation is unmatched and  this is the first reported use of thermal laser stimulation for  latchup investigations. In one provided example, the latchup  trigger was isolated to FET based decoupling capacitors (decaps) widely used as fill.


Latchup occurs when the parasitic Bipolar Junction  Transistors (BJTs) that are inherent in a CMOS (Complementary Metal-Oxide-Semiconductor) process are  inadvertently activated, creating a low impedance path  between power and ground. The BJTs form a Silicon  Controlled Rectifier (SCR) which, once triggered, is  maintained in a conducting state. The resultant current flow  causes latchup to rapidly spread until either catastrophic  device damage occurs, or the power supply’s current limit is  reached. Recovery usually requires power cycling of the  device. Excess heat or charge are common triggers [1].


Despite being a well understood phenomenon, CMOS  latchup  remains a reliability concern because of shrinking margins, the  myriad ways it can be triggered, and the potential for device  damage when it occurs [1, 2]. Maintaining high latchup  margins for power-supply overvoltage conditions in the core  of an IC is also required to enable various forms of accelerated  lifetime testing, e.g., High-Temperature Operating-Life (HTOL) testing, and for Dynamic Voltage Stress (DVS) screening [3, 4]. The semiconductor industry is heavily


dependent on techniques such as these to ensure the reliability  of their products.


As geometries shrink, susceptibility to latchup increases and  new defect- or process- based triggers can appear [5, 6]. As  part of process qualification, the latchup limits of our logic  and memory test vehicles are tested on ATE (Automated Test  Equipment) to verify that they meet specifications. The “Vtrig” test that is used involves increasing the core supply  voltage incrementally until either the latch-up voltage  specification is reached (passing condition), or the current  compliance limit of the supply is abruptly hit and maintained, even as voltage is reduced (failing condition).


For units that fail the Vtrig test, root-causing the latchup  triggers is a part of process improvement activities. Isolation  of these triggers down to the cell level in standard-cell logic  and memory is typically required. Unfortunately, the defects  that produce these triggers often escape standard MBIST (Memory Built-In Self-Test) and ATPG (Automatic Test  Pattern Generation) testing and are therefore difficult or  impossible to isolate to the required level using normal EFA  methodologies.


Optical techniques have been widely used by others to isolate  latchup trigger sites. The charge carriers created by latchup  can recombine before they are collected, thus emitting nearinfrared (NIR) photons with energy near the bandgap of Si (~1100 nm wavelength). Since these photons are emitted in  and near the latchup region, PEM (Photon-Emission  Microscopy) can be used to identify these regions [6-8]. Techniques utilizing pseudo or direct time resolved imaging to  track the latchup progression and better localize the trigger site  have been reported [7-9].


Since latchup can be triggered by charge, it’s also possible to  use laser stimulation techniques to isolate trigger sites [10-15]. Pulsed laser sources can induce enough current to initiate  latchup at sensitive sites in a normally biased DUT (DeviceUnder-Test). As a result, they are often used for single-event  latchup (SEL) sensitivity studies [16-19]. Continuous-Wave (CW) lasers can also be used, but they may not be able to  induce enough instantaneous current to initiate latchup unless  the latchup margin is reduced by other means [13, 14]. For  flip-chip DUT, 1064 nm wavelength (1.17 eV photon energy) is typically used. Since latchup can also be triggered by heat, it


# V-Pulse Technique For Optical Isolation Of Latchup Triggers In Sub-14 nm Standard-Cell Logic And Memory


86


should be possible to alternatively use 1340 nm wavelength (0.93 eV). To the best of our knowledge, however, no one has  yet reported doing so.


Unfortunately, none of the previously reported techniques  could fully meet the unique set of challenges presented by our  Vtrig debug cases. We required a technique that could  address:


1. The low CW laser damage threshold of our <14 nm  FinFET DUT, especially when using Solid  Immersion Lenses (SILs).


2. The high electrical power dissipation due to the dense  logic and memory in the test vehicles examined and  the high supply voltages and currents required to test  their latch-up limits.


3. The high power-supply decoupling capacitance of the  DUT and DUT card setup used, which prevented  rapid external modulation of the DUT’s supply rail.


4. The level of isolation required- down to the cell level  in standard-cell logic and memory.


The technique that we ultimately developed features:


1. Ability to image Vtrig latchup regions using static  PEM.


2. Ability to use 1064 nm as well as1340 nm  wavelength CW lasers (versus picosecond pulsed  laser sources) to isolate latchup triggers down to the  cell level.


3. Automatic quenching of latchup events.


4. Simple latchup flag generation using only a bench  oscilloscope.


5. Ability to use a standard DUT card setup with FA  socket.


6. Stable long-term operation with only passive air  cooling.


7. No custom software or hardware required: Only  bench test equipment and standard FA tools.


In the rest of this paper, we first give a brief overview of some  of the existing FA techniques for investigating latchup. Then  we describe our V-Pulse technique in detail, show  characterization result, and present several isolation examples. We end with a discussion and summary/conclusion of our  work.


Overview of Existing Techniques


NIR PEM was one of the first techniques used to study latchup  in CMOS ICs [7]. However, the rapid spread of latchup and  current starvation effects can obscure the region where latchup  is first initiated [7, 8]. In addition, the slow time response of  typically available cameras only allows a gross tracking of the  progression of latchup events. (Although not demonstrated, a  PICA camera-based imaging system with its intrinsic  50-100 ps response may be an exception [9].)


To work around this limitation, Khurana implemented a  voltage pulsing technique to track latchup spreading using a


static emission camera [7]. By varying the voltage-pulse width  applied to the supply pins of a DUT, the progression of  latchup sites could be determined by noting the times at which  they became visible after triggering. Latchup emission could  be captured w/in 50-100 ns of initiation, which was adequate  for identifying the initial latchup site for his application.


Quincke, et al., was able to achieve slightly better time  resolution of 20-250 ns using a modified laser scanning  microscope (LSM) and a liquid nitrogen cooled Ge detector to  capture the latchup emission [8]. A custom electro-optic  modulator placed into the LSM’s return beam path was time  gated to sample the emission at each image pixel location at  various delays after latchup was triggered. Stroboscopic  sampling was used to generate waveforms of the latchup event  at selected pixel locations. Despite the low-bandwidth  stroboscopic measurements and use of a cryogenically cooled  detector, low Signal-to-Noise Ratio (SNR) severely limited  the usefulness of the technique: According to the authors, images took hours to acquire, even with time resolution  reduced to 250 ns.


The response time of the power grid to external modulation is  one of the limiting factors for achievable time resolution using  the above techniques. For our DUT and setup, minimum  voltage rise/fall times were ~10-100 µs. Even when using the  minimum pulse-widths possible, we were only able to localize  the initial latchup site to an area of ~105 - 106 µm2 using PEM.


where xj is the relative distance between rj and rj+1. To correct  for the shadowing, the top of the grooves needs to be cut  which yields the corrected shape shown in Fig. 4.


Figure 4: Perfect Fresnel lens with a focal length of 5μm. This  lens is corrected for groove depth variation and shadowing.


The lens in Fig. 4 has been corrected for groove depth  dependence on groove radius and shadowing caused by  neighboring grooves. Notice though that this lens has not been  corrected yet for the shadowing caused by the outermost edge, but this can easily be done by extending the last groove  laterally. From Fig. 4 it can also be seen that the groove width  becomes less for larger radius. In fact, for thin silicon the  width quickly becomes less than the wavelength, thus limiting  the effectiveness of the groove. Groove widths can be  increased by designing for wavefronts that are multiple  wavelengths apart. In an algorithm this can be implemented by  doubling the delta in wavelengths whenever the groove width  becomes less than the wavelength. This has been  experimentally done as shown in Figs. 5 and 6 that give the  lens as designed and when focused on the IC through the lens, respectively.


Figure 5: Experimental Fresnel lens with groove depth, shadow and width correction. The silicon thickness is only 50 μm.


Figure 6: Imaging performance of the Fresnel lens of Fig. 5. The pitch of the white structures is 1.22 μm.


However, for very thin silicon groove width correction quickly  becomes ineffective since with larger width also the groove  depth is increased. A natural lens size limitation is then when  the depth becomes larger than the silicon. This is shown in Fig.


7.


Figure 7: Groove width corrected thin lens; a natural size  limit is when the groove depth becomes more than the silicon  thickness.


Thus, for thin silicon the best Fresnel lens that can be obtained  is illustrated in Fig. 4. Let’s now see what its imaging  performance is.


FDTD Simulation Results


For the simulations, lenses are defined on rather thick silicon  of several tens of μm but then defined to have a certain focal  length. Let’s consider a very short focal length of 5 μm. For  this thickness all of the above described implications for lens  design are important. If then a diffraction lens corrected for  depth and shadowing effect is simulated, the point-spreadfunction (PSF) shown in Fig. 8 is obtained.


Figure 8: Simulated point spread function for a SIL lens (black), a depth and shadow corrected Fresnel lens (blue) and  a binary approximation of a Fresnel lens (red). All lenses are  targeting a focal length of 5 μm.


The full-width-half-maximum (FWHM) is a good measure for  the width of the PSF and is for both the SIL and Fresnel lenses  approximately 280 nm. Since the expected width is 0.61λ/NA, the numerical aperture of the lenses is NA = 2.9. Surprisingly, the binary approximation [11] of the Fresnel lens is seen to  perform quite well from Fig. 8 with the only apparent drawback being a reduced intensity. In fact, the binary lens has an  advantage in that it can be used on very thin silicon where the  curvature of the perfect Fresnel lens, evident in Fig. 4, becomes a limiting factor.


101


Field of View


The FOV of the SIL lens has been experimentally investigated  in [12] using resolution targets and it was demonstrated that  the FOV varies with the focal depth of the lens. Here, we  investigate the FOV of the Fresnel lens using simulations. Namely, it can be simulated by laterally offsetting the  incoming spherical laser source by a certain distance from the  central axis and calculating the resulting PSF. The results have  been shown for the perfect Fresnel lens in Fig. 9.


Figure 9: Simulated PSF for the perfect Fresnel lens with 5 μm focal length for various offsets of the laser with respect to  the central lens axis. The transmission is negative since the  light propagates in the -z direction.


There are several noteworthy observations to be made from  Fig. 9. First, a 3 μm lateral offset of the source yields an  effective focus shift of only ~0.83 μm. This directly reveals the  lens magnification which is concluded to be 3.6X. In [12] the  magnification change as a function of the focal depth has been  derived for the SIL and this will hold true for the Fresnel lens  as well. It is also interesting to see how the magnification  varies with the lateral offset of the laser. This has been plotted  for the perfect and binary lens with various focal lengths in  Fig. 10.


Figure 10: Lens magnification as a function of lateral offset  for the perfect and binary Fresnel lens with various focal  lengths.


A magnification deviating from ~3.5x means that the image  gets distorted. Thus, if the FOV is defined as the image field  that is free from distortions, then from Fig. 10 it can be  concluded that the effective FOV for the perfect Fresnel lens is  about equal to the focal length and for the binary Fresnel lens  it is even smaller.


Another observation made from Fig. 9 is that the intensity of  the focused light quickly drops for larger x-offsets of the laser. In fact, for an offset of 10 μm there is hardly any intensity left. Thus, at the edges of the FOV the image fades into darkness, as is observed experimentally in Fig. 6. It is also instructive to  look at the peak intensity as a function of the focus point, as  shown in Fig. 11.


Figure 11: The same simulated PSF as in Fig. 9, but now  plotted as a function of focus position along the silicon depth. Thus, the various curves plotted are for increasing lateral  offset which then leads to an axial shift in focal point.


What is seen from Fig. 11 is that the focal length increases for  increasing lateral offset of the laser. Experimentally this is also  observed in that by focusing deeper, the part of the image in  focus spreads out like a ring extending from the central axis. Thus, the focal plane is curved and from the simulations it is  seen that the curvature increases for thinner silicon which can  be observed by considering the PSF for a 10 μm focal length  lens, as plotted in Fig. 12.


102


Figure 12: Simulated PSF for the perfect Fresnel lens with  10μm focal length plotted as a function of focus position along  the silicon depth.


The focal plane curvature poses a limitation on the  effectiveness of an ultrathin lens since only a small part of the  image can simultaneously be brought into focus. Coincidentally, this correlates with the distortion-free image  field as described above. Thus, the FOV is quite small for an  ultrathin Fresnel lens, especially considering the fact that  effectively it is reduced once more by the lens magnification. This is also observed from the image in Fig. 6 which has an  experimental FOV of ~14 μm. Indeed, the focal length divided  by the magnification yields 14 μm as well.


Integrated diffractive lenses on ultrathin silicon require careful  design in order to function properly but can be reasonably  approximated by a binary equivalent. The main limitation  though hindering the use of integrated lenses for ultrathin  silicon is the limited FOV that can be obtained. For integrated  refractive lenses, the FOV is limited by the silicon thickness. For integrated diffractive lenses, the focal plane of the lens is  curved, and the curvature increases for decreasing focal length. Thus, only a limited area can be simultaneously brought into  focus resulting in a limited FOV. Furthermore, outside a circle  of diameter equal to the focal length, the image is distorted. Hence also for integrated diffractive lenses the FOV is limited  by the silicon thickness.


We would like to thank Anthony Blakely for the excellent  compute server facilities.


[1] Keith A. Serrels, Euan Ramsay, Paul A. Dalgarno, Brian


D. Gerardot, John A. O’Connor, Robert H. Hadfield,


Richard J. Warburton, and Derryck T. Reida, "Solid


immersion lens applications for nanophotonic devices", Journal of Nanophotonics, Vol. 2, 021854 (2008)


[2] SH Goh, ACT Quah, CJR Sheppard, CM Chua, LS Koh, JCH Phang, "Effect of Refractive Solid Immersion Lens  Parameters on the Enhancement of Laser Induced Fault  Localization Techniques", pp. 1-6, IPFA 2008.


[3] Ikuo Arata, Shigeru Sakamoto, Yoshiyuki Yokoyama and  Hirotoshi, "Photoemission and OBIRCH Analysis with  Solid Immersion Lens (SIL)", pp. 325-329, ISTFA 2003.


[4] P. Scholz, U. Kerst, C. Boit, C.-C. Tsao, T. Lundquist, "Creation of Solid Immersion Lenses in Bulk Silicon  Using Focused Ion Beam Backside Editing Techniques", pp. 157-162, ISTFA 2008.


[5] P. Scholz, M. Sadowski, C. Boit, S. Kupijai, M. Henniges, C. Theiss, S. Meister, D. Stolarek, H.H. Richter, and M. Boostandoost, "Turning Sample Into (Re)Solution - Focused Ion Beam Shaped Solid Immersion Lenses", pp. 66-70, ISTFA 2015


[6] Frank Zachariasse, Martijn Goossens, "Diffractive Lenses  for High Resolution Laser Based Failure Analysis", pp. 1-7, ISTFA 2005.


[7] Marc van Veenhuizen, Harry Kerver, Lei Peters-Wu, Sukho Lee, Frank Zachariasse, "The use of a Fresnel lens  on an actual failure", pp. 284-293, ISTFA 2015.


[8] Brian Morgan, Christopher M. Waits, John Krizmanic, and Reza Ghodssi, "Development of a Deep Silicon Phase  Fresnel Lens Using Gray-Scale Lithography and Deep  Reactive Ion Etching", J. Microelectromechanical  Systems, Vol. 13, pp. 113-120 (2004)


[9] A.F. Oskooi, D. Roundy, M. Ibanescu, P. Bermel, J.D. Joannopoulos, and S.G. Johnson, "MEEP: A flexible freesoftware package for electromagnetic simulations by the  FDTD method", Computer Physics Communications, Vol. 181, pp. 687-702 (2010)


[10] Robert Brunner, Matthias Burkhardt, Alexander Pesch, Oliver Sandfuchs, Margit Ferstl, Sungchul Hohng, Jeffrey  O White, "Diffraction-based solid immersion lens", J. Opt. Soc. Am. A, Vol 21, No. 7 (2004)


[11] Tom D. Milster, "Ch. 7: Miniature and Micro-Optics", Handbook of optics 2, McGraw-Hill, Inc.: New York, (1995)


[12] Goh Szu Huat, "Development and characterization of  refractive solid immersion lens technology for far-field  integrated circuit failure analysis using laser induced  techniques", Ph.D. thesis, (2009)


103


Infrared Lock-In Thermography: from localization of low power and masked defects to absolute temperature mapping for product debug


J. Jalink, A. Firiti, J. van den Biggelaar


NXP Semiconductors, Gerstweg 2, Nijmegen, The Netherlands


A. Reverdy


Sector Technologies, 24 rue LAMARTINE, Eybens France


B. Lai


ThermoFisher Scientiﬁc, Warren avenue, Fremont, USA


Abstract—The application of IR-Lock-In Thermography (IRLIT) has been extended from 2D and 3D package fault isolation to on-die level analysis. In addition, the technique has become more sensitive allowing for detection of much lower dissipated power. In this paper, several fault localization cases covering PCB assemblies down to die level analysis are discussed using IR-LIT and absolute temperature mapping. Where possible,the analysis is complemented with physical defect veriﬁcation.


The fault isolation cases include an ultra-low power dissipation(<150 nW) and several case studies with high ohmic connections.


For the latter a new method based on phase mapping is discussed allowing for 2D localization of thermally invisible defects. The method will be demonstrated on a test vehicle where phase data extracted from a visible feature of the device under test is studied.


Figure 27 shows, for example, that the predominant emitter in  the SRAM macros under normal DC biasing is the circuitry  surrounding the bit-arrays. In Figure 32, they are some of the  bit-arrays themselves. There are also obvious differences in  the emission hotspots in the logic cores (bottom portion of the  images).


These differences indicate that the dependence of photon  emission rate on voltage bias can vary in an IC, at least for the  high values that are made accessible with V-pulse biasing. We  don’t yet understand the reason for these variations, nor if they


have applications for fault isolation, but we intend to  investigate further.


Figure 32. PEM image acquired using V-pulse biasing of  same DUT shown in Fig. 27. Different structures seen to  dominate emission pattern compared to DC bias condition (Fig. 27). 131 µs/2 ms pulse-width/period, 20 s integration  time.


Summary/Conclusion


We introduced a new technique for optically isolating latchup  triggers in core logic and memory of sub-14 nm CMOS  FinFET flip-chip DUT. A current-pulse from a current  amplifier is used to charge the DUT capacitance to rapidly  ramp Vdd. The amplifier’s ability to sink current allows the  DUT capacitance to also be quickly discharged to ramp-down  Vdd. Quasi-static PEM imaging of the latchup region can be  performed by adjusting the pulse-width to ramp Vdd to Vtrig, the latchup value for the DUT. Using a CW laser to trigger  latchup is made possible by ramping Vdd to just below Vtrig  to reduce the DUT’s latchup margin. Biasing the DUT close to  Vtrig in this fashion also helps ensure that the true Vtrig  limiter is targeted for isolation. Latchup quenching is  automatic since Vdd drops to 0 V after each pulse. A latchup (i.e., pass/fail) flag is generated by using the advanced trigger  modes of a standard bench oscilloscope.


The technique was successfully used to isolate latchup triggers  down to the cell level and has led to successful root-cause  analyses. Several isolation examples were provided. One  revealed decaps to be an unanticipated reliability concern, and  another demonstrated the unique capability of laser  stimulation using the V-Pulse methodology to isolate latchup  triggers. We believe that ours is the first reported application  of using a CW ‘thermal’ laser (1340 nm wavelength) for  investigating Vtrig related latchup in CMOS logic and  memory.


We thank Roy Ng and Steven Kasapi for useful discussions  and Elia Halteh, John Aguada, and Steven Scott for preparing  the samples. We also thank our foundry partners for  performing many of the root-cause PFA and Thermo-Fisher  Scientific for providing time on their ELITE LIT system.


97


[1] Troutman, R.R., Latch-up in CMOS Technology, Kluwer  Academic (New York, 1986).


[2] JEDEC Standard JESD78E, IC Latch-Up Test, April


2016. www.jedec.org.


[3] Tsao, C.-Y., Shiue, R. Y., Ting, C. C., Huang, Y. S., Lin, Y. C., and Yue, J. T., “Applying Dynamic Voltage  Stressing to Reduce Early Failure Rate,” Proceedings, 39th IEEE International Reliability Physics Symposium (IRPS), Orlando, Fl, April 2001, pp. 37-41.


[4] London, A., Ng, K., and Wick, P., “Use of Voltage  Stressing at Wafer Probe for Reliability Predictions,” IEEE Trans. Semiconductor Manufacturing, Vol. 12, No. 4, (1999) pp. 516-22.


[5] Domanski, K., “Latch-up in FinFET technologies,” Proceedings, IEEE International Reliability Physics  Symposium (IRPS), Burlingame, CA, March 2018, pp. 2C.4-1 thru 5.


[6] Dai, C.-T., Chen, S.-H., Linten, D., Scholz, M., Hellings, G., Boschke, R., Karp, J., Hart, M., Groeseneken, G., Ker, M.-D., Mocuta, A., and Horiguchi, N., “ Latchup in Bulk  FinFET Technology,” Proc. IEEE Internation Reliability  Physics Symposium (IRPS), Monterey, CA, April 2017, pp.  EL-1.1-3.


[7] Khurana, N., “Pulsed Infra-Red Microscopy for  Debugging Latch-Up on CMOS Products,” Proc. 22nd  IEEE International Reliability Physics Symposium (IRPS), Las Vegas, NV, April 1984, pp. 122-7.


[8] Quincke, J., Boit, C., Führer, D., “Electroluminescence  Measurements with Temporal and Spatial Resolution for  CMOS Latch-Up Investigations,” Microlectronic  Engineering 12 (1990) pp. 157-62.


[9] Weger, A., Voldman, S., Stellari, F., Song, P., Sanda, P., McManus, M., “Transmission Line Pulse Picosecond  Imaging Circuit Analysis Methodology for Evaluation of  ESD and Latchup,” Proc. 41st International Reliability  Physics Symposium (IRPS), Dallas, TX March 2003, pp. 99-104.


[10] Llido, R., Gomez, J., Goubier, V., Froidevaux, N., Dufayard, L., Haller, G., Pouget, V., and Lewis, D., “Photoelectric Laser Stimulation Applied to Latch-Up  Phenomenon and Localization of Parasitic Transistors in  an Industrial Failure Analysis Laboratory,” Microelectronics Reliability, 51 (2010) pp. 1658-61.


[11] Burns, D. J. and Kendall, J. M., “Imaging Latch-Up Sites  in LSI CMOS with a Laser Photoscanner,” Proc. 21st  IEEE International Reliability Physics Symposium (IRPS), Phoenix, AZ, April 1983, pp. 118-21.


[12] Shiragasawa, T., Shimura, H., Kagawi, K. Yonezawa, T., and Noyori, M., “Latch-Up Analysis on a 64 K Bit Full  CMOS Static RAM Using a Laser Scanner,” Proc. 22nd  IEEE International Reliability Physics Symposium (IRPS), Las Vegas, NV, April 1984, pp. 63-8.


[13] Henley, F. J., Chi, M. H., and Oldham, W. G., “CMOS  Latch-Up Characterization Using a Laser Scanner,” Proc. 21st IEEE International Reliability Physics Symposium (IRPS), Phoenix, AZ, April 1983, pp. 122-9.


[14] Weichold, M. H., Parker, D. L., and Fenech, J.- F., “Imaging Latch-Up Sites in CMOS Integrated Circuits  Using Laser Scanning,” IEEE Trans. On Components, Hybrids, and Manufacturing Technol., V. CHMT-8, No. 4


(1985) pp. 556-8.


[15] Wills, K. S., Pilch, C. J. Jr., and Hyslop, A., “A Study of  CMOS Latch-Up by Laser Scanning and Voltage Contrast  Techniques,” Proc. 24th IEEE International Reliability  Physics Symposium (IRPS), Anaheim, CA, April 1986, pp. 115-9.


[16] McMorrow, D., Buchner, S., Baze, M., Bartholet, B., Katz, R., O’Bryan, M., Poivey, C., Label, K. A., Ladbury, R., Maher, M., and Sexton, F., “Laser-Induced Latchup  Screening and Mitigation in CMOS Devices,” IEEE  Trans. Nuclear Science, Vol. 53. No. 4 (2006) pp. 1819-24.


[17] Roche, N. J.-H., Khachatrian, A., Buchner, S., Foster, C. C., Ferlet-Cavrois, V., Muschitiello, M., Miller, F., Morand, S., Warner, J., Decker, T., and McMorrow, D., “Application of a Pulsed Laser to Identify a Single-Event  Latchup Precursor,” IEEE Trans. Nuclear Science, Vol. 62, No. 6 (2015) pp. 2679-86.


[18] Wang, P., Sternberg, A. L., Kozub, J. A., Zhang, E. X., Dodds, N. A., Jordan, S. L., Fleetwood, D. M., Reed, R. A., and Schrimpf, R. D., “Analysis of TPA Pulsed-LaserInduced Single-Event Latchup Sensitive-Area,” IEEE  Trans. Nuclear Science, Vol. 65. No. 1 (2018) pp. 502-9.


[19] Moss, S. C., LaLumondiere, S. D., Scarpulla, J. R., MacWilliams, K. P., Crain, W. R., and Koga, R., “Correlation of Picosecond Laser-Induced Latchup and  Energetic Particle-Induced Latchup in CMOS Test  Structures,” IEEE Trans. Nuclear Science, Vol. 42. No. 6


(1995) pp. 1948-56.


[20] Accel Instruments TS250 Waveform Amplifier, Accel  Instruments, Irvine, CA 92618.


[21] BK Precision 9130B Programmable Triple Output DC  Power Supplies Data Sheet, BK Precision, Yorba Linda, CA 92887.


[22] For capacitance C and constant current I, ignoring  resistive losses, Q=I*t, where Q = charge on C and t = current pulse duration. Capacitance equation, C=Q/V, then gives V=(I/C)*t.


[23] Tektronix MDO3024, Tektronix, Inc., Beaverton, OR


97077.


[24] Tektronix MDO3000 oscilloscope user’s manual, pp. 87-100.


[25] Tektronix HFS9003.


[26] Beitenstein, O., Warta, W., and Schubert, M.C.,  Lock-in  Thermography: Basics and Use for Evaluating Electronic  Devices and Materials, 3rd Ed, Springer Nature (Switzerland, 2018).


[27] Charania, T., Opal, A., and Sachdev, M., “Analysis and  Design of On-Chip Decoupling Capacitors,” IEEE Trans. VLSI Systems, 21(4) 2013, pp. 648-58.


98


Integrated Diffractive Lenses for Ultrathin Silicon


Marc van Veenhuizen, Peter van der Cruijsen


Product Diagnostic Center Nijmegen, Gerstweg 2, Nijmegen, The Netherlands


Keith A. Serrels


Product Diagnostic Center Austin, 6501 West William Cannon Drive, Austin, TX 78735, USA


Frank Zachariasse


Business Line Secure Transactions & Identification, NXP Semiconductors, Nijmegen, The Netherlands


High numerical aperture (NA) laser scanning for fault  localization requires the use of special lenses aimed at creating  a tightly focused laser spot within an integrated circuit. Typically, extrinsic solid immersion lenses are employed that  optimize the refraction at the air-silicon surface. In this  feasibility study we investigate with both simulations and  experiments the use of integrated diffraction lenses for highNA imaging. We take the limit to ultrathin silicon and discuss  the implications for the lens design and performance.


With the ever-decreasing feature sizes in integrated circuits (IC) comes the need for ever increasing resolution of laserbased fault isolation techniques. As in lithography, this is  accomplished by regularly increasing the numerical aperture (NA) of the imaging system and occasionally decreasing the  wavelength of the laser used. Typically, the NA of the  projection optics is increased by integrating a solid immersion  lens (SIL) into the objective lens system that then makes  physical contact to the exposed silicon substrate of the IC [1 - 3]. Thus, this is an external solution requiring a dedicated  objective lens with SIL cap. Another approach is to shape the  exposed silicon itself into a lens, either refractive (SIL) [4], [5] or diffractive (Fresnel) [6], [7], with the latter being easier to  fabricate since it is basically a flattened version of the former. There are certain advantages to the silicon shaping approach, namely, reduced setup complexity, better cost efficiency, and  higher lens design flexibility. Clear downsides however are  increased fabrication complexity, reduced time efficiency, and  diminished image quality. It is interesting to see how this  comparison holds in the limit of ultrathin silicon. This is  relevant since in order to increase the NA of the Fresnel lens  the silicon needs to be thinned. Another reason to investigate  this is the industry drive towards enabling visible light fault  localization solutions to address the need for improved  resolution and sensitivity; ultrathin silicon is required since  visible light is attenuated in silicon. The present article will


investigate how lenses integrated on ultrathin silicon perform, primarily through lens simulations.


Numerical simulations can greatly facilitate the design of these  micro-lenses, which is especially valuable since the fabrication  is in general complicated [8]. There is a powerful free software  package called MEEP [9] that we used to simulate the light  propagation of the lens system. MEEP employs the FiniteDifference-Time-Domain (FDTD) approach to solve  Maxwell's equations on a discrete grid. In the following, we  use this package to check the performance of ultrathin Fresnel  lenses, as compared to a conventional refractive SIL lens. A  typical simulation snap-shot is given in Fig. 1. It shows how  the electro-magnetic wavefronts propagate through the lens  system.


Figure 1: Shown is a snap-shot of the simulated electric field  in the lens system. The grey surface is the silicon with the  Fresnel lens defined at the air-silicon interface.


In all the simulation results shown in the following, the source  is a spherically converging Gaussian wave with wavelength λ = 1320nm that is propagating in the negative z-direction. It  should be noted that the results also hold true for smaller  wavelengths. The lens is integrated at the device backside at


# Integrated Diffractive Lenses for Ultrathin Silicon


the boundary between air and silicon, the latter of which has a  refractive index n = 3.5. To avoid reflections, the silicon  extends to the left and right (±x) and down (-z) to the  simulation cell boundary which has perfectly matched layers.  The simulations are quasi-2D in that the lens is effectively  modeled as a cylinder extending infinitely in the out-of-plane  directions; the findings in this paper however carry over to a  3D lens.


Scaling Integrated Lenses


To increase the NA significantly, the silicon needs to be  thinned. In this work, a thin silicon substrate is defined as less  than 100 μm and all the way down to 5 μm. This holds for  integrated refractive lenses but even more so for integrated  diffractive lenses. For integrated refractive lenses, if the silicon  is thinned then the maximum attainable lens radius is reduced  since the largest radius is given by the silicon thickness. A  smaller lens radius results in a smaller field-of-view (FOV). Thus, thinning the silicon imposes restrictions on the FOV for  integrated refractive lenses. Consider now a perfect diffractive  lens integrated onto thin silicon. There are 3 physical  limitations that start to have an impact and ultimately put a  limit to the scaling attainable. These are groove depth, shadowing, and groove width. A perfect diffraction lens that is  defined on relatively thick silicon (focal length is 20 μm) is  shown in Fig. 2.


Figure 2: Perfect Fresnel lens with a focal length of 20 μm.


Here, and in the following, when describing a “perfect Fresnel  lens” it equates to a multi-step approximation of the blazed  groove profile by 8 steps in total. For thin silicon, the lens of  Fig. 2 would look like Fig. 3.


Figure 3: Fresnel lens defined on thin silicon with a very short  focal length of only 5 μm, illustrating the groove depth  variation and shadowing effect.


Various wavefronts that are integral numbers of wavelengths  apart fall on different grooves of the lens. From Fig. 3 it is  seen that this implies that the groove depth increases with the  radius, as described by the formula given below.


Here, the variable convention of [10] is followed where ƒ  means silicon thickness, and rj the radius of the jth groove.


For thin silicon, neighboring grooves cause a shadowing effect  that effectively cause the light rays to scatter twice. This can  be seen from Fig. 3 where all rays between the two labeled "1" and "2" will be scattered by two grooves. The intersection of  where the lower ray hits the curved edge of the groove can be  derived as


Figure 1. Block diagram showing V-Pulse setup for laser  stimulation studies. See text for details.


Figure 2. Output current of Current Amplifier in Fig. 1 when  driving DUT setup, monitored through Current Monitor  output of amplifier. Shown for Function Generator pulse  widths of 25, 50, 75, and 100 µs. Positive values indicate  amplifier sourcing current; negative values indicate amplifier  sinking current.


Each current-pulse from the Current Amplifier charges the  DUT and DUT card capacitance to ramp Vdd, as shown in  Fig. 3. The maximum value of Vdd is determined by the  duration of the current pulse. Figure 3 shows that the fastest  rate at which Vdd can be ramped with our setup for the  particular DUT used is ~1 V/100 µs when using a single  Current Amplifier. This is limited by the capacitance of the  DUT and DUT card used. This slew rate is much faster than  possible with typical bench DC power supplies, which are  usually internally limited by the filtering used to reduce their  output noise [e.g., 21]. Also important is the rate at which Vdd


88


can be decreased, which is dependent on the amplifier’s ability


Current Vs Pulse Width


to sink current (Fig. 2). Typical bench supplies are not  designed to sink large currents: Their ramp-down rates are


-0.120ms--0.121ms


dependent on DUT leakage [21].


0.122ms-0.123ms


Voltage Vs Pulse Width


-0.025 ms-0.050ms


宝


Vdd (Volts)0.3


Time(ms)


0.110


0.115


0.120


0.125


0.130


0.135


0.140


0.145


0.150


二


08


Amps10)/Current (-0.6


0.075 ms-0.100ms


Figure 3. DUT Vdd for current pulses shown in Fig. 2. DUT  and DUT card capacitance performs a time-to-voltage


1.2


conversion [22].


1.15


0.120ms--0.121 ms


Using the Current Amplifier as a constant current source and


1.1


0.122 ms--0.123ms


setting peak Vdd indirectly via the current pulse width,


王


91.05


together with the amplifier’s ability to sink current, minimizes


01


the time over which the DUT is biased near Vtrig. This


0.95


directly contributes to the long-term stability and


p0.9


reproducibility of the V-Pulse technique.


0.85


Pass/Fail (Latchup) Flag and Pixel Clock Generation


0.75


As the current-pulse width is increased (Fig. 4) Vdd will


continue to ramp (Fig. 5) eventually reaching the Vtrig value  for the DUT and initiating latchup. A latchup event is


characterized by an abrupt drop in Vdd caused by the sudden


drop in DUT resistance and the current limit of the  amplifier [14]. The 123 µs (blue) trace in Fig. 5 shows this  latchup-induced voltage drop. If the Function Generator pulse  width is reduced slightly (122 µs, for example) then the DUT  will be briefly biased near the threshold of latchup. With the  latchup margin thus reduced, it then becomes possible to scan  a CW laser beam over the DUT to trigger latchup using laser  powers well below the DUT’s laser-damage threshold.


When the DUT is biased close to Vtrig, the latchup event  induced by the laser beam results in a Vdd drop that is similar  to the one caused by pure voltage biasing. A moderately  capable bench oscilloscope can be set up to distinguish  between the latchup and non-latchup voltage pulse waveforms [e.g., 23, 24]. We find it most convenient to set the  oscilloscope to trigger on ‘less-than’ pulse-width and adjust  the trigger level and pulse-width thresholds as illustrated in  Fig. 6. The scope will then be triggered only by the latchup  events.


Figure 4. Current Amplifier output for Function Generator  pulse widths of 120, 121, 122, and 123 µs. Positive values


-0.0500.000


0.050


0.1000.150


0.200


0.250


0.300


0.3500.400


indicate amplifier sourcing current; negative values indicate


Time (ms)


amplifier sinking current.


Figure 5. Vdd of DUT corresponding to current pulses shown  in Fig. 4. Latchup occurs with 123 µs pulse width, as  indicated by sudden drop in Vdd caused by sudden drop in  DUT resistance.


To generate the actual pass/fail flag for the laser stimulation  systems used (Thermo-Fisher M4 and M5 systems) we use the  auxiliary output (AUX OUT) of the oscilloscope which can be  set up to output a pulse whenever a trigger is captured [24]. For our scope and the typical timebase settings used, the  AUX OUT signal is normally High and outputs a ~120 µs  Low pulse whenever triggered (Fig. 7). This signal can be fed  directly into the frame-grabber input of the laser stimulation  system with no further processing required. Each latchup  event is then recorded as a ‘fail’ by the system.


89


Figure 6. Illustration showing scope trigger setup used to  distinguish between Vdd pulse traces acquired under laserinduced latchup (brown) and non-latchup (blue) conditions. Trigger level and pulse-width parameters set as shown for ‘Less-than’ pulse-width trigger mode of scope. Note: Vdd rolloff caused by DUT leakage due to higher Vtrig threshold for  DUT used.


Tek


Vdd Sense


Scope Aux Out (P/F)


Fn Gen TTL Out


Delay Gen Output (Pixel Cik)


40.0ps2.50MS/


+72.00000u11000points74.5


Figure 7. Scope screen shot showing (in order from top to  bottom): Voltage pulse in latchup condition, P/F flag from  Oscilloscope auxiliary output, Function Generator TTL output (synchronized to the start of each current pulse to the DUT) and Pixel Clock signal from Delay Generator. See text for full  details.


To operate in synchronous mode, a pixel clock must also be  generated for the laser stimulation system. The rising-edge of  the clock must be properly timed for the system to latch the  pass/fail flag from the oscilloscope. For convenience, we  derive the pixel clock from the TTL output signal of the  Function Generator (Fig. 1) instead of tapping off the pulse  output. The signal can’t be used directly, however: It must be  delayed before it is input to the laser stimulation system (Fig. 7) to account for the DUT’s delayed response to the  output current-pulse and the various other delays in the setup. To generate the properly timed pixel clock to the system, we  use a programmable pattern generator that is triggered by the  Function Generator [e.g., 25]. It is set up to output a ~100 µs  delayed pulse whenever it is triggered by a pulse from the  Function Generator.


Latchup Quenching and Persistence Effects


Latchup


Trigger


Similar to the scheme used by Weichold, latchup events are


1.5Level


No Latchup


automatically quenched with our V-Pulse technique because  Vdd is brought back down to 0 V for each voltage pulse, as


indicated in Figs. 3 and 6 [14]. This is the case regardless of  whether latchup was induced during the pulse event, or not. However, latchup can be retriggered for follow-on pulses,


Vdd (Volts)


Threshold Width


Runt Pulse


even when the laser is moved off the sensitive node. This


happens when the voltage is pulsed again too quickly  following a latchup event. Others have noted this


-0.5


possibility [18]. We assume this latchup persistence is due to a


-0.0500.050.10.150.2


temporary latchup threshold reduction caused by local heating


of the DUT from the latchup current. This persistence effect  leads to streaking in the pass/fail maps, as shown in Fig. 8.


Figure 8. Laser stimulation map overlaid on greyscale LSM  image, taken with 20x lens and 1064 nm laser. Red indicates  locations where latchup is induced by laser. Horizontal  streaking occurs in map when using 2 ms pulse period due to  latchup persistence effects (Fast scan direction: left to right).


To eliminate or reduce latchup persistence, the cool-down  time following a latchup event must be increased to allow the  DUT to fully recover (Fig. 9). Since our simple setup doesn’t  allow the pulse period to be varied during an acquisition, the  pulse period selected is necessarily a trade-off between shorter  acquisition times (shorter pulse period / less cool-down time) versus reduced persistence effects in the maps (longer pulse  period / more cool-down time). Another issue to keep in mind  is the scope’s maximum trigger rate. Using periods that are too  short can result in missed latchup events due to the scope’s  trigger dead time. We typically use 2-10 ms pulse periods. We  are investigating a more flexible holdoff scheme that increases  the pulse period only following a latchup event to provide  both shorter acquisition times and reduced persistence effects.


Other factors that can affect latchup persistence are how far  the DUT is biased below the Vtrig value, the laser power used,


and the laser wavelength: 1340 nm tends to induce more


V-Sense


latchup persistence than 1064 nm. One possible reason for this


DUTDUT


difference is that 1340 nm produces a weaker effect and


O-Scope


Card


usually requires operating closer to the Vtrig threshold to stay


V-Force


below the laser-damage threshold of the DUT.


I-Pulse Current」」Amplifier Output


Emission


RF


Function Generator


V-Pulse


System Camera


Figure 9. Laser stimulation map taken using 10 ms pulse  period showing elimination of streaking caused by latchup  persistence effects (compare to Fig. 8).


Dedicated Photon Emission Microscopy Setup


A simplified setup suitable for PEM-only studies is shown in  Fig. 10. The Function Generator and Current Amplifier are  operated as described above, except the current pulse width is  increased until Vdd just reaches Vtrig to electrically induce  latchup (monitored using the oscilloscope). Pulse periods are  similar to those used for laser stimulation. Under these  conditions, latchup emission is usually visible in the live  image mode used for navigation using the LN2 cooled InGaAs  camera in our system (Thermo-Fisher Scientifics’ Meridian 4  system). Capturing images in the normal emission mode of the  system for improved SNR usually requires <30 s integration  time (e.g., Fig. 11).


Due to the short voltage pulses used, latchup spreading is  reduced to an absolute minimum, given the limitations of our  setup. Despite this, latchup emission is observed to span an  area of ~105 – 106 µm2 (Fig. 11) far too large for successful  PFA. Still, we find PEM to be a very useful complimentary  technique to laser stimulation studies. It offers:


1. Gross isolations, e.g., logic vs SRAM.


2. Guidance for the laser isolations to help ensure the  true Vtrig limiter is targeted and to minimize the  areas searched.


3. Isolation of any anomalous emission hotspots related  to the Vtrig limiter.


Figure 10. Block diagram showing simplified setup for PEMonly studies. See text for details.


Figure 11. Latchup emission image acquired using V-Pulse  technique (color) overlaid on illuminated light image (greyscale) taken using 5x lens and LN2 cooled InGaAs  camera. 39.6 ms pulse-width, 10 ms pulse-period. Integration  time: 5 s. Image cropped.


V-Pulse Characterization


In this section, we present characterization results showing the  stability of the V-Pulse technique and the correlation of Vtrig  values to ATE measurements.


Stability


Figure 12 shows two voltage pulse waveforms, taken ~40 min  apart under latchup conditions. They are identical, within the  noise of the measurements. During actual debug activity, stability over at least several hours is achieved, as determined  by the lack of observed drift of the Vtrig threshold, provided  the DUT and test equipment are allowed to warm up for


~15 min. The day-to-day repeatability of the setup for any  particular DUT is limited mostly by slight resistance  variations in the power supply lead connections due to  handling: Pulse widths required to trigger latchup can vary by  a few microseconds when reseating the connectors.


Figure 12. Vdd latchup pulses taken ~40 minutes apart  demonstrating stability of V-pulse technique. During debug  activities, setup is observed to be stable for many hours.


Correlation with ATE Vtrig Measurements


Figure 13. Vtrig scatter plot showing correlation between VPulse and ATE measurements for 7 DUT. Dashed line is a  linear fit to the data. V-Pulse measurements are uniformly  higher, likely due to reduced heating from low duty cycle  voltage pulses used versus quasi-DC biasing used for ATE  testing.


To have confidence that the optical isolations performed target  the same Vtrig limiters detected during ATE testing, we  confirmed the correlation between Vtrig values measured  using the V-Pulse technique versus ATE testing. Figure 13  shows a scatter plot of Vtrig values for several DUT. The  correlation is clear despite the different test conditions used.


The Vtrig values found under V-Pulse conditions are  uniformly elevated, likely due to the greatly reduced average  power dissipation for V-Pulse biasing compared to the quasiDC biasing used for ATE testing. Even with the superior  temperature control solutions used, fully controlling selfheating effects during ATE testing can be difficult.


Vtrig Isolation Examples


In this section, we present three Vtrig isolation examples. The  first example is a straightforward case from a DUT that failed  both MBIST and Vtrig testing. PEM images showed an  emission hotspot at the failing bitcell locations, which lay  within the latchup emission region. Vtrig isolation confirmed  that the failing bitcells were also the latchup triggers.


The second example is from another DUT that exhibited an  extremely low Vtrig value but otherwise passed both MBIST  and Logic testing. PEM identified an emission hotspot at a  cluster of FinFET based decoupling capacitors within the  latchup-emission region. Laser-stimulation confirmed that  these were the latchup triggers and not the result of collateral  damage caused by the initial latchup event.


The final example is from a DUT that failed both Vtrig and  Logic testing. The expectation was that the failures were  linked, but Vtrig isolation indicated otherwise. Additionally, unlike the previous two examples, no traditional PEM  anomalies were found at the latchup trigger sites. This  example demonstrates the unique capability of the V-Pulse  methodology to isolate the failure.


Example #1


The DUT in this example failed MBIST Vmin testing and  exhibited a very low Vtrig value. Bitmapping identified a  cluster of failing bitcells in a single SRAM macro. Vtrig  isolation was performed to confirm that the Vtrig and MBIST  failures were linked.


Following our typical Vtrig debug workflow, lowmagnification PEM was first used to image the full-thickness  DUT under V-Pulse stimulation to grossly isolate the latchup  emission region. The current-pulse width was increased until  the latchup threshold was found. Figure 14A) shows the Vdd  and current-pulse waveforms with the pulse width set slightly  below the latchup threshold. Figure 14B) shows the  corresponding waveforms at latchup. The sudden drop in Vdd  that is characteristic of latchup is indicated (arrows). PEM  images were acquired under both conditions: The results are  shown in Fig. 15. The latchup-emission region was found to  surround the failing SRAM macro (dashed rectangles).


92


Figure 14. A) Oscilloscope screenshots showing Vdd and A current-pulse waveforms (top/purple and bottom/green traces,


respectively) used to bring DUT in example #1 to slightly


below latchup threshold. Current-pulse width/period:


104 µs/2 ms. B) Corresponding waveforms under latchup


conditions. Sudden Vdd drop characterizing latchup indicated


by arrows. Pulse-width/period: 105 µs/2 ms. Associated low-B magnification PEM images shown in Fig. 15.


Figure 15. Cropped 5x magnification Live-View PEM images


corresponding to V-Pulse stimulus shown in Fig. 14. A) Sublatchup condition. B) In latchup. Failing macro indicated by


dashed rectangle. Extra emission caused by latchup, visible


in B, originates from logic surrounding SRAM macros.


Before proceeding further, the DUT was thinned to 50 µm  Remaining Silicon Thickness (RST) in anticipation of SIL  imaging. In addition, a second current-amplifier was added to  the V-Pulse setup of Fig. 1 to increase current drive-strength  for faster voltage pulsing. 20x PEM images are shown in  Fig. 16. An isolated emission site was identified in the failing


SRAM macro (blue rectangle) under sub-latchup  condition (A). In latchup (B) the latchup emission is seen to  encompass the peripheral logic in the failing macro and  several others nearby.


Figure 16. Cropped 20x PEM images acquired using modified  V-Pulse setup (2nd Current-Amplifier added). Emission map (color) overlaid on background image (grayscale). Failing  SRAM macro indicated by blue rectangle. A) Acquired near  threshold of latchup: 56 µs/10 ms pulse-width/period, 60 s  PEM integration time. B) Acquired under latchup condition: 58 µs/10 ms pulse-width/period, 2 s integration time. Arrows  indicate isolated emission site w/in failing SRAM macro. Latchup emission in peripheral logic of some macros also  visible in B).


Figure 17. 5 s integration time SIL image of isolated emission  spot (color) overlaid on background image (grayscale). Failing bitcell locations indicated (inset, blue rectangles). VPulse setup: 56 µs/10 ms pulse-width/period.


PEM images acquired using a SIL confirmed that the isolated  emission site matched the failing bitcell locations (Fig. 17, inset). 1064 nm laser stimulation results acquired using the  SIL confirmed that these failing bitcells were also the latchup  triggers (Fig. 18). No other region near the SRAM macro  exhibited sensitivity at this laser power level. Using slightly  higher laser power (1.33 mW vs 1.0 mW) caused the latchup


93


sensitive region to marginally expand, but no other laser-


》


sensitive site appeared.


Figure 18. 1064 nm, 1.0 mW laser stimulation map (red) overlaid on background LSM image (grayscale). Map shows  locations where laser triggered latchup. Inset shows failing  bitcell locations (blue rectangles). V-Pulse setup: 57 µs/10 ms  pulse-width/period.


Example #2


The DUT in this example also exhibited a very low Vtrig  value but otherwise passed all MBIST and Logic testing. Using the V-Pulse setup shown in Fig. 1, the current-pulse  width was set to induce latchup in the unthinned DUT (Fig. 19) and a 5x, 2 s long integration time PEM image was  acquired (Fig. 20A). The latchup emission was isolated to one  of the logic cores in the DUT. An abnormal emission hotspot  was also observed within the latchup region (Fig. 20B) which  was exposed by voltage pulsing slightly below the latchup  threshold and integrating for a longer period (60 s).


123us ----124us


Vdd (Volts)0.9


0.070.080.090.10.110.120.130.140.15


Figure 19. Zoom-in of peak of Vdd pulses for DUT in  example #2. 124 µs pulse width induced latchup in DUT, as  exhibited by rapid drop in Vdd (arrow) compared to 123 µs  non-latchup waveform.


一人


Figure 20. Cropped 5x PEM images of: A) Latchup emission  acquired under V-Pulse stimulation overlaid on background  image. (124 µs/10 ms current pulse-width/period, 2 s  integration time.) B) Emission image acquired with DUT  biased below latchup condition. Abnormal emission hotspot  within latchup region indicated (arrow). (122 µs/10 ms pulsewidth/period, 60 s integration.)


Figure 21. 1340 nm laser stimulation map (red) showing a  single cluster of hits where the laser induces latchup. Image  field-of-view matches that shown in Fig. 20. Map acquired  using 5x lens, 20 mW laser power, 122.8 µs/10 ms current  pulse width/period (below the latchup threshold).


Figure 22. 2.9NA SIL, 1340 nm laser stimulation map of  latchup trigger sites for example #2. Acquisition conditions: 2 mW power, 121.6 µs/10 ms current-pulse width/period.


94


Next, 1340 nm CW laser stimulation using a 5x lens was  performed. A small cluster of hits within the latchup emission  region were found (Fig. 21). The location of hits appeared to  coincide with the emission site shown in Fig. 20B.


Figure 23. 2.9NA SIL, 1064 nm laser stimulation map of  latchup trigger sites for example #2. Acquisition conditions:


0.9 mW power, 121.7 µs current-pulse width, 10 ms period.


Figure 24. 2.9NA SIL PEM image obtained under sub-latchup, V-Pulse stimulation: 123.1 µs/10 ms current-pulse  width/period, 60 s integration time.


To further isolate the latchup trigger(s), the DUT was thinned  to 50 µm RST and the region rescanned using 1340 nm  wavelength and a 2.9 N.A. SIL (Fig. 22). The cluster was  revealed to consist of several decap cells, one of which is  identified (blue rectangle). Laser stimulation using 1064 nm (Fig. 23) and PEM imaging (Fig. 24) were also performed.


The PEM image shows that the identified decaps were indeed  the source of anomalous emission. The 1064 nm map  demonstrates the stronger, but less discriminating effect that


charge injection can produce. This DUT was submitted for  PFA with instructions to probe the highlighted decap. Excessive gate leakage was found. (See CAFM map in Fig. 30, obtained from a different DUT.)


Example #3


This final example is from a DUT that failed both Logic and  Vtrig testing. The initial expectation was that the failures were  linked. The first step was to again perform a lowmagnification PEM acquisition under V-Pulse latchup  stimulation to grossly localize the latchup region (Fig. 25). The latchup emission was indeed found to cover the failing  logic core, with part of it extending into a nearby SRAM  macro (arrow). However, laser stimulation results showed the  strongest sensitivity in the SRAM macro (Fig. 26). CAFM  identified widespread gate leakage defectivity at this location.


Figure 25. Cropped 5x PEM image taken under latchup VPulse stimulation: 72 µs/10 ms current-pulse width/period, 2 s  integration time. Latchup observed in failing logic core with  tail extending into nearby SRAM macro (arrow).


Figure 26. 1340 nm laser stimulation map of latchup trigger  sites (red) in SRAM macro (dashed rectangle). 5.3 mW power, 20x lens. Inset: Higher resolution SIL map (1.0 mW, 1340 nm) identifying large cluster of cells w/in SRAM macro as latchup  trigger sites.


Figure 27 shows a PEM image of the same DUT acquired


Vdd


under DC bias conditions. Unlike the previous two examples, no anomalous emission site was found in the region flagged  by laser stimulation, although several were found in the failing  logic core. Lock-in Thermography (LIT) was also performed


Gnd


(results not shown) but no thermal hot-spots were found at the  latchup trigger site either [26]. This case demonstrates a  situation in which only laser-stimulation under V-Pulse bias  was able to isolate the latchup trigger site.


Gnd o-


-o Vdd


(P+N+N+


N+)


Figure 27. Cropped 5x PEM image acquired under 1.0 V DC  bias conditions. Although some anomalous emission sites were  observed, notably in failing logic core, none were found in  SRAM region flagged by laser stimulation. SRAM macro  indicated by blue dashed rectangle.


- nFET S/D


1 Gate


Several of the latchup trigger isolations performed, e.g.,


pFET S/D


example #1, demonstrate that defects that cause logic or  memory failures can also degrade Vtrig values. This is  unsurprising since many of these defects are known to exhibit  photon and/or thermal emission. In other words, they are  defects which cause excessive current flow and/or elevated  temperatures, both of which are potential latchup triggers. From the point of view of clearing latchup issues, this is  convenient because these defects can be isolated using normal  means, such as Scan Diagnosis, MBIST/Bitmapping, LVx, PEM, SDL, etc., and addressing the logic/memory failures  also addresses the associated latchup issues.


Other isolations, including example #2, revealed decaps to be  an unexpected source of latchup triggers. In hindsight, this  result should not have been unexpected since these are  FinFET-based decaps with the same CMOS structure as  normal switching transistors. Figure 28 shows the  configuration of a typical CMOS decap, while Fig. 29 shows a  cross-sectional diagram of the decap. Unlike a switching  transistor, source and drain of each FET in the CMOS pair are  tied to the same rail (Vdd for pFET, Gnd for nFET). However, the pnpn SCR structure, and, hence, latchup susceptibility, is  retained. As mentioned in example #2, excessive gate leakage  is one mechanism by which latchup margins can be reduced in  these decaps (Fig. 30).


Figure 28. CMOS based decap configuration utilizing gate  capacitance in the MOS transistors [27].


P


Figure 29. CMOS decap cross-section showing parasitic  bipolar transistors forming pnpn SCR structure (adapted  from [1]).


Figure 30. Top: Conductive Atomic Force Microscope (CAFM) current map of decap isolated as latchup trigger (dashed rectangle). Rows of S/D and Gate contacts indicated.  Excessive gate leakage (red arrow) found. Teal and Blue  arrows indicate S/D contacts. Bottom: Current plot taken  along dashed red line in CAFM map.


This finding presents a problem since decaps can’t be tested  through normal means (i.e., Logic/MBIST testing) yet, they  can make up a large fraction of the total transistor count in  modern ICs [27]. Since pre-isolation through normal test  techniques can’t be applied, isolation of failing decaps are  dependent on global isolation techniques such as LIT and/or  PEM. V-pulse biasing combined with laser stimulation helps  ensure that the true Vtrig limiter is targeted, especially in the  not uncommon situation where more than one anomalous  hotspot is found.


96


A third class of latchup triggers, e.g., example 3, exhibit no  LIT or PEM signature, and don’t cause memory or logic  failures. In these situations, the V-pulse methodology is  essential for their isolation.


Beyond the isolation of Vtrig related defects, the V-pulse  technique can be used to investigate marginalities caused by  cell design and/or circuit layout effects. Figure 31 shows a  1064 nm laser stimulation map of a DUT with almost-passing  Vtrig value. For high Vtrig DUT such as this, the expectation  is that the failure is caused by a parametric effect (e.g., process  skew) instead of an isolated defect. Indeed, the map obtained  shows a large distribution of hits with very similar latchup  thresholds: No single site clearly stands out as laser power is  reduced. Furthermore, there’s a clear pattern (arrows) to the  clusters of hits. They align to the same region in each of the (identical) logic cores. (See also Fig. 11, which shows latchup  emission aligned to the same features in adjacent cores.) Analysis of the cells and layout in these regions to understand  why they are more susceptible to latchup is ongoing. This  might ultimately lead to design changes or revised layout rules  if increased latchup resistance is desired.


Figure 31. Cropped 5x laser stimulation map (red) showing  regular pattern (arrows) of latchup sensitive sites that align  with same region in each logic core of DUT. 4mW laser  power, 1064 nm wavelength, 38.5 µs/10 ms pulsewidth/period.


More speculatively, V-pulse biasing may find applications  beyond V-trig isolations. Figure 32 is a PEM image of the  same DUT shown in Fig. 27, except acquired with V-pulse  biasing to near the Vtrig threshold. DC biasing to the same  value is not possible due to the risk of thermal runaway. Comparison of the two images shows that different structures  dominate the PEM image under the different biasing  conditions.


After this, a case study at die level is presented in an attempt to distinguish the phase information from two stacked M2-M3 metallization layers of the Back-End Of the Line (BEOL). Finally,temperature mapping results of a 5 micron wide aluminum feature in silicon-oxide is presented that is pushing the optical resolution of the tool.


Into the last decade, IR Lock-In Thermography (IR-LIT)and in general thermography analysis has been widely adopted by the Failure Analysis (FA) community [1], [2]. One of the main reasons of this large adoption is the ability of IR-LIT to be used as one of the very ﬁrst steps in the FA ﬂow without any speciﬁc sample preparation step required. Thermography and Lock-In Thermography (LIT) can be easily run at board(PCB) level, package level [3] and die level [4]. This high level of ﬂexibility in terms of analyzed target makes IR-LIT the perfect ﬁrst step of the FA ﬂow to extract a ﬁrst level of information on the failure location, allowing FA engineers to select the appropriate and most efﬁcient ﬂow to ﬁnd the root cause of the failure.


In this paper we present several case studies using the thermography approach and demonstrate the ﬂexibility of this approach regarding the type of samples that can be analyzed as well as a range of techniques that can be applied to solve a speciﬁc problem. Here, we limit ourselves to voltage or current excitation, but other stimuli can be considered as well (light


[5], ultrasound [6], magnetic [7]). Hoe et al. [8] show that for backside IR-LIT analysis through the silicon, a dissipated power in the order of 20 µW can be used for successful


localization of a failure. The exact details of the system under evaluation plays a key role in the minimum power that can be localized. As ﬁrst case study, we show that a defect dissipating in the nW range can be detected (with acceptable integration time) on the surface of package. As discussed by Li et al.


[1], LIT also allows localization of high ohmic connections.


This will be the topic for the second case study, showing the localization of high ohmic contacts for a product in a Flip-Chip Ball Grid Array (FC-BGA) package after reliability testing.


Apart from 2D localization using the phase and amplitude mapping for the x,y coordinates of the defect, post-processing of phase data as function of lock-in frequency is of utmost importance for extracting the z-location of the defect [9]. We present an additional method for post-processing of phase data to localize hidden or masked defects. This method extends the application of fault isolation for devices with complex geometry where the heat generated by the failure can not be emitted at the surface above the fail location. The third case study presents in depth analysis of phase information of a current path at die level in an attempt to separate metallization layers in the BEOL. Finally, absolute temperature mapping is discussed. While thermoreﬂectance can provide absolute temperature measurements with micrometer resolution [10],IR Thermography is used here to investigate a test structure with features in the micrometer range, using the calibrated 1X lens of the system. The results are in good agreement with the calculated temperature for this device, showing that an IR-LIT tool with temperature mapping option can be used for devices with small features.


THERMOGRAPHY TECHNIQUES


Lock-In Thermography


Lock-In Thermography is a well established technique that allows to localize a resistive short, low ohmic short and leakage currents on microelectronic devices. The lock-in approach here is based on a forced electrical alternating excitation of the Device Under Test (DUT) at a given frequency. This technique is taking beneﬁt of the known forced excitation frequency to perform a very narrow ampliﬁcation of the thermal signal emitted by the DUT at the excitation frequency. This allows to increase the sensitivity of the thermal system by more


104


Fig. 1. Lock-In Thermography implementation.


than one order of magnitude, making it possible to detect dissipated power down to the µW range and even lower for some speciﬁc cases as presented in this paper. On top of this critical sensitivity improvement, the Lock-In approach allows to get access to both amplitude and phase information of the thermal response of the hot spot under investigation. Phase information can be very useful in case of investigation on


2.5D or 3D packages or sub-system (PCB board) in order to extract the z-localization of the defect [9]. Figure 1 and 2 are describing the thermal Lock-In implementation and the main principle of the Lock-In approach [11].


Absolute Temperature Mapping


Complementary information that can be provided by an IRLIT tool is the real temperature of a DUT stimulated with different test conditions, and its behavior versus time. An obvious domain in which this application can add its value is the package thermal management validation. The main difﬁculty when trying to extract the absolute temperature from a device consists in generating an accurate emissivity map of the DUT. To do so, the ELITE system from ThermoFisher Scientiﬁc that has been used in this study, is calculating the emissivity map using the following method:


• The ﬁrst step is done only one time for a given systemand is usually done by the tool manufacturer. The thermal camera and lenses are calibrated on a black body source with a well know emissivity. While monitoring the lens temperature, the goal is to acquire a complete set of images on the black body source set at different temperature (typically with a 10◦C step), using various acquisition times on the detector. The acquisition time set on the camera will deﬁne the maximum temperature that can be acquired by the detector before saturation. So, for all chosen acquisition times, we will deﬁne a range of workable temperatures (typically: [10◦C- 50◦C], [20◦C100◦C], [20◦C-150◦C]; [50◦C-250◦C]), that will be use by the end user depending on his application. This set of


Fig. 2. Lock-In Thermography principle.


images will be used by the system to convert the camera count received by each individual pixel into an absolute temperature for a known emissivity material.


• The second step of this absolute temperature measure-ment ﬂow is run by the end user on the DUT. It consists in acquiring two images of the DUT, while heating up the DUT to known temperatures using a thermal chuck. These two reference images will be used by the calculation software to determine the emissivity of each individual pixels of the Field Of View (FOV). During this process, the calculation software will also take into account one of the main sources of error that can be induced by this type of measurement, which is the correction of the environment temperature reﬂecting on the DUT that can signiﬁcantly affect the absolute temperature calculation. This is speciﬁcally important when looking at high reﬂective material such as metals, which is a very typical material for microelectronic devices.


After this calibration procedure has been followed, the system will be able to provide thermal images or sequences with an absolute temperature scale.


105


EXPERIMENTS AND RESULTS


Ultra-Low Power Dissipation Failure at Package Level


In this ﬁrst case study, a high resistive behavior was reported for a die in an HVQFN package resulting in a low leakage current of 360 nA. Photon-Emission-Microscopy (PEM) and Optical Beam Induce Resistance Change (OBIRCH) analysis from the backside opened product did not provide any information to the nature of this deviation. As the deviating current consumption could readily be measured with a pin-topin setup, a backside LIT analysis was attempted using two probe needles placed directly on the leads of the package. With an ultra-low power dissipation of just 144 nW, a hot spot was found at the edge of the package, between the leads (Fig. 3)using the 1X thermal lens, lock-in frequency of 0.5 Hz and 20 min integration time.


Fig. 3. LIT analysis showing overlaid amplitude (a) and phase (b) images from the backside of the fail sample.


Instead of a 3D localization using a phase versus frequency acquisition [9], a more pragmatic approach was used. The package was rotated by 90◦ allowing a direct analysis from the side. The analysis, again using probe needles directly on the leads, conﬁrmed the presence of a resistive path between the indicated leads. Based on the LIT result, showing a thermal response at the outside of the package precisely between the biased leads, an artifact in the Epoxy Mold Compound (EMC)or between the leads might be expected. Figure 4 shows the LIT results from the failing lateral side of the package:


Fig. 4. LIT acquisition showing overlaid amplitude image (a) and phase image (b) from the side view of the package.


Additional conﬁrmation of the short at the outside of the package was obtained using Scanning Electron Microscopy(SEM) voltage contrast on the uncoated sample. As the contaminant was judged to be on the surface of the package, TimeOf-Flight Secondary Ion Mass-Spectrometry (TOF-SIMS) was performed to obtain the chemical ﬁngerprint as depicted in Fig. 5. A carbon-based contamination was found as a surface artifact that is not related to the package manufacturing.


Fig. 5. (a) SEM voltage contrast on an uncoated sample shows the short on the side of the package. (b) TOF-SIMS analysis on the package side revealed a carbon-based contamination.


Fig. 6. (a) LIT analysis of complete system (FC-BGA with metal cap)showing hotspot at the side of the metallic cap. (b) LIT analysis after metal cap removal showing a hotspot on the product laminate. (c) overlay analysis of the hotspot with design shows that the hotspot originates from a part of a laminate trace. (d) SEM inspection of plan-view sectioned laminate shows a crack in the Cu-trace.


Localization of High Ohmic Connections after Reliability Testing


LIT can be used to separate fail location between die and test board as some reliability tests are recommended to be carried out on a printed circuit board [12], [13]. Here, a high ohmic connection was reported after board level temperature cycling testing using a test chip in a FC-BGA package with metal cap and experimental bill of materials. First, LIT is performed on the complete system showing heat dissipation underneath the metal cap. Second, the metal cap is removed and LIT is again performed to improve localization. An overlay of the LIT results and the routing information of the package substrate, see Fig. 6, allows pinpointing a speciﬁc copper trace. Physical failure analysis at the hotspot locations shows that a copper trace on the laminate has been cracked due to thermo-mechanical stress. The remaining fractional contact of the copper trace allows LIT to be a very powerful method to localize such failure.


106


Fig. 7. (a) Pattern image of the PCB Cu-line with two probe needles. (b)Phase mapping of obtained at 5Hz; red box indicates the data selected for further analysis (c) Phase versus distance for several excitation frequencies


Localization of Masked Defects using Phase Data


In the latter case the metal cap from the package was removed. This might not always be an option. In such situation the previous failure isolation would have been more difﬁcult because of limited heat coming out of the package side. With this potential limitation in mind, a new method is discussed to estimate the defect location for devices where the fail location is optically/thermally blocked by a product feature.


A simpliﬁed case is studied where a short is made via two probe needles on a PCB Cu-pad. This allows direct optical access to the fail location and heat propagation, see Fig. 7. Several LIT acquisitions are made by varying the excitation frequency. The phase (correct with the system delay)versus distance is extracted from the mapping and shows an expected linear dependence as the heat dissipates with a constant velocity. The heat generated at the short location at minimum phase is readily visible, see Fig. 7c. The heat then propagates and shows a phase shift at approximately 100 pixels due to the solder mask on top of the Cu. This can explain the change in slope in the data that is visible for Lock-In frequencies from 1 to 20 Hz. For higher frequencies this slope is still present, but less apparent.


The following can be concluded based on this simpliﬁed


Fig. 8. (a) Phase versus distance data for various lock-in frequencies extracted from image (b), with linear extrapolation to predict the fail location. (c)Veriﬁcation of the fail location after removal of the metal cap.


exercise: Post-processing of phase data can be used to localize masked defects. However, details of the device under test need to be considered, e.g. in this case the solder mask on top of the Cu-line. Additionally, for more complex systems this approach can be used when the lateral thermal path is large compared to the vertical thermal path.


This approach is now used for a high ohmic contact that was reported for a FC-BGA with a metallic cap assembled on a PCB and as such only the periphery of the device can be seen. It must be noted that the investigated thermal path,in contrast to the test case, does not have a solder mask on the Cu-line. Estimation of the fail location was done by extrapolating the phase versus distance over the Cu-line that is in the failing path, see Fig. 8. Extrapolation of multiple phase versus distance lines as function of frequency resulted in a prediction of the fail location (Fig. 8a) that is in line with the location provided after removal of the metal cap(Fig. 8c). Averaging the extrapolated locations at 0◦ phase for multiple frequency acquisitions results in a predicted location of 460 ± 22 pixels from the left-hand side of the image. Whichis in good agreement with the hotspot location recorded after removing the metal cap at 438 pixels from the left-hand side of the image.


This approach is not limited to linear extrapolation of the phase data. One can consider extracting line or area proﬁles of the amplitude or phase mapping and use system details and material properties to approximate the fail location.


107


Identiﬁcation of the Back End Of the Line by using Phase Mapping


IR-Lock-In Thermography technique has been applied on a device that can be considered as a complex packagein-package system. A current path between two terminals,caused by a resistance of 65 Ω, was investigated. Successive frontside and backside (silicon-side) IR-LIT investigations were performed at package level. The heat source was conﬁrmed to be on the silicon die, thus excluding any package related defect. After package decapsulation, a new LIT session was performed from the backside of the die and conﬁrmed the previous localization result. Using bias conditions of 200 mV / 3.1 mA and a Lock-In frequency of 25 Hz, an interesting LIT mapping with 10X magniﬁcation highlighted a clear thermal path (Fig. 9a), like an OBIRCH mapping (Fig. 9b) showing the current path. Figure 10 depicts


Fig. 9. (a) Backside LIT amplitude image with 10X magniﬁcation, 25Hz Lock-In frequency and 200mV / 3.1mA. (b) Backside OBIRCH image with 20X magniﬁcation. Both techniques show similar mapping


respectively the amplitude image (a), the phase image (b) and the overlaid image (c) obtained with 10X magniﬁcation.


Fig. 10. Amplitude image (a), Phase image (b) and overlaid Phase image


(c) are highlighting the thermal path within the stacked BEOL layers of the die.


This case study will focus on the the analysis of the thermal path in the silicon die. In particular, to evaluate the phase mapping that will be used as an attempt to identify different metal layers within the BEOL. Design data from the device will be used to understand the experimental data.


The phase map in Figure 11a, obtained at 10X magniﬁcation, shows two main colors (green and red) respectively associated with the long lines and two small spots. The red color corresponds to the lowest phase value (close to surface)whereas the green color corresponds to a higher phase value(deeper in the device). The design analysis conﬁrmed that the thermal path was associated to layout routines of metal stack of the BEOL (Fig. 11b), and more precisely to aluminum M2


Fig. 11. (a) Phase image and its associated layout drawing with the involved BEOL metal layers in the thermal signature. The numbers represent speciﬁc sections that are discussed in the text. (b) From the design extracted physical routing of the involved BEOL.


and M3 lines and their tungsten interconnects. Consequently,the phase map can be interpreted as: Green phase color is obtained over long M3 metal lines, whereas red phase red color is found at interconnection and short M2 metal lines. The layout analysis (Fig. 11b) correlates the thermal intensity and the phase mapping detected on the involved M2 and M3 metal lines at die level. For a better interpretation of the LIT results,the phase map has been decomposed in six speciﬁc sections as described in Fig. 11. The minimum phase values have been detected at position 1 and 2 which include short M2 metal lines interconnected to long M3 metal lines with VIA2. A higher and uniform phase value has been detected at locations 3, 4, 5, and 6, which is the main thermal path. A detailed investigation on location 3 shows that the layout conﬁguration is like location 1, with VIA2-M2 line, but the corresponding phase map is different (minimum phase map expected). This phase variation can be explained by the presence of multiple M1 metal lines at location 3 (Fig. 11b) that affects the thermal response over M2 metal line and VIA2. Additionally, a slight phase variation can be observed too in the left side of the location 1, where a similar M1 metal line conﬁguration is present and affects the LIT map (Fig. 12b). At this stage,the green color map is clearly from M3 metal line, but it is more difﬁcult to conﬁrm if the minimum phase value of the red color is due to the VIA2 only (tungsten material), or to short M2 line (aluminum) or to the combination of both layers VIA2+M2. Additional experiments and measurements are needed to determine precisely which layer, M2 (Al) or


Fig. 12. a) Backside layout cross section view of M1 M2 M3 layers. (b)Zoom from 2D phase map of location 1 (fLIT =25Hz). (c) 3D representation of the phase proﬁle at location 1 (fLIT =25Hz).


108


Fig. 13. Phase versus frequency plots on locations 1 and 5 from Fig. 11.


VIA2 (W), is the main contributor of the minimum phase value map.


In this paper, we will consider both layers VIA2-M2 as one stack contributing to the minimum phase in location 1(Fig. 11). Then, additional phase data was processed by adapting the phase slider speciﬁcally to the location 1 as described in Fig. 11a. Consequently, the minimum phase value on VIA2/M2 line was measured about 44◦, whereas the minimum phase value on M3 line was measured about 54◦.


The difference between the minimum phase values of red and green phase colors is below 10◦. With our considerations, the delta of 10 degrees corresponds to a total material thickness of 1.9 µm, between top of M2 and top of M3. This very local 3D analysis on the BEOL stack (M2-VIA2-M2) has been completed with phase versus Lock-In frequency measurements on location 1 (red) and location 5 (green) to predict their respective depth. Figure 13 shows the distinct lines which are not superimposed, meaning different z-position (depth) and thus distinguishable layers. The experimental measurements indicated a delta of minimum phase between both locations of 3◦ at 0.5 Hz and 7◦ at 25 Hz.


Based on our considerations, this approach conﬁrmed that an acceptable phase resolution can be extracted from LIT acquisitions and demonstrated that M2/VIA2 and M3 layers of BEOL can be distinguished in this case study. The possibility that only VIA2 layer or only M2 metal line is the main contributor of the minimum phase map in location is not excluded and needs additional experiments for validation. In this speciﬁc case, the combination of the LIT phase mapping and the design study was used to extend the LIT possibilities and to identify the BEOL layers in the IC under certain conditions and with an acceptable phase resolution. This case study demonstrated that IR-LIT technique can be helpful to support product debug and design optimization.


Temperature Mapping of a Test Structure


Temperature mapping is a very welcomed feature as it can support product level analysis for (high power) devices and can provide feedback on calculations used for temperature driven life time testing on process evaluation modules. But it also appears as a challenging technique when dealing with


Fig. 14. Overview of the test structure


Fig. 15. Full ﬁeld of view temperature mapping image of the test structure(aluminum line in silicon-oxide) with a forced current of 150mA. The heat emission at the probe pads is due to the needle contacts.


microelectronics devices which contain small structures with large emissivity variations. Use of a thermal chuck with wafer material, single die or single unit without board level setup is one of the most common and traditional ways to calibrate for emissivity prior to any temperature measurement.


Here we show temperature mapping results of an aluminum line in silicon-oxide with tungsten interconnects, where the IRLIT tool is pushed towards the limit for the optical resolution.


The aluminum line is 5 µm wide and connects with tungsten VIAs to the top metal which has a width of 15 µm. A high level overview of the test structure geometry is shown in Figure 14. The current through the metal line is 150 mA and the environmental temperature is 30◦C. The temperature mapping option is calibrated for the 1X lens with a ﬁeld-ofview of about 9600 µm x 7680 µm and a pixel resolution of about 15 µm. The temperature mapping results can be seen in Figure 15. Despite the fact that the feature size is comparable to the optical resolution, good agreement is found between the calculated self-heating of 26.9◦C and the measured selfheating of 24.0◦C, see Fig. 16. Still, it is recommended to enable temperature mapping at higher optical magniﬁcation to improve the spatial resolution and accuracy of such measurements.


109


Fig. 16. Average temperature proﬁle extracted from the two extremities of the test structure showing an increase in temperature of 24.0◦C.


CONCLUSIONS


In this paper we have presented challenging Infrared LockIn Thermography use cases showing both the localization of low power and high ohmic defects ranging from package to die level. This demonstrates great ﬂexibility in terms of ﬁeld of applications. Ultra-low power dissipation (<150 nW) caused by carbon contamination was localized at package level. This surface artifact is not related to package manufacturing. In addition, deviating ohmic paths are studied at package and die level. The former shows that IR-LIT can be used to detect cracks at the package level, while the latter is showing an OBIRCH like current path where the phase data allows to discriminate between different metallization layers in the BEOL. However, additional experiments are needed to validate these results.


On top of that, we also introduced a novel method to use phase information on defects that are thermally masked by DUT features, by analyzing the thermal propagation of the induced heat along the connected copper trace. This method allows to estimate the location of a defect that is masked by product features that are blocking the thermal emission at the DUT surface. Finally, the optical resolution of the tool is pushed to the limited for an absolute thermal mapping application where good results are obtained on a 5 µm wide aluminum feature in silicon-oxide. Yet, it is highly recommended to further enable higher magniﬁcation lenses for temperature mapping.


ACKNOWLEDGMENT


The authors acknowledge ThermoFisher Scientiﬁc (TFS)for providing support and information about their ELITE thermal Lock-In solution; NXP Business partners for sharing the use cases and paper review; Engineers and technicians from NXP Product Diagnostic Center (PDC) Nijmegen for their contributions.


[1] Y. Li, P.K.M. Srinath and A, Goyal, A Review of Failure Analysis Methods for Advanced 3D Microelectronic Packages, D. Journal of Elec Materi (2016) 45: 116


[2] M. Krause, F. Altmann, C. Schmidt, M. Petzold, D. Malta and D. Temple, Characterization and failure analysis of TSV interconnects: From non-destructive defect localization to material analysis with nanometer resolution, 2011 IEEE 61st Electronic Components and Technology Conference (ECTC), Lake Buena Vista, FL, 2011, pp. 1452-1458.


[3] M.Y. Tay, M.C. Tan, W. Qiu and X.L. Zhao, Lock-in Thermography Application in Flip-chip Packaging for Short Defect Localization, 2011 IEEE 13th Electronics Packaging Technology Conference, Singapore,2011, pp. 642-646.


[4] S. Huth and O. Breitenstein, Localization of gate oxide integrity defects in silicon metal-oxide-semiconductor structures with lock-in IR thermography, Journal of Applied Physics 88, 4000 (2000)


[5] Th. Zweschpe, D. Wu and G. Busse, Detection of loose rivets in aeroplane components using lockin thermography,http://dx.doi.org/10.21611/qirt.1998.025


[6] Th. Zweschper, A. Dillenz and G. Busse, Inspection of aerospace structures with ultrasound lock-in-Thermography CD of 15th WCNDT,Roma, 2000 - ndt.net


[7] J. Bohm and K. Wolter, Inductive excited lock–in thermography for electronic packages and modules, 33rd International Spring Seminar on Electronics Technology, ISSE 2010, Warsaw, 2010, pp. 190-195.


[8] T. M. Hoe and K. K. Ng, The factors study of backside hotspot localization with application Infrared Lock-in Thermography, 2015 IEEE 22nd International Symposium on the Physical and Failure Analysis of Integrated Circuits, Hsinchu, 2015, pp. 213-218.


[9] C. Schmidt, F. Altmann and C. Grosse, Lock-in-Thermography for 3-dimensional localization of electrical defects inside complex packaged devices, ISTFA 2008: Proceedings from the 34th International Symposium for Testing and Failure Analysis


[10] W. Claeys, S. Dilhaire, V. Quintard and J.P. Dom, Absolute dynamic measurements of temperature changes in electronic components from a thermoreﬂectance optical test probe, Proceedings ETC 93 Third European Test Conference, Rotterdam, Netherlands, 1993, pp. 378-384.


[11] O. Breitenstein, C. Schmidt, F. Altmann and D. Karg. Thermal Failure Analysis by IR Lock-in Thermography, Microelectronics Failure Analysis, 2011


[12] R. Rongen, R. Roucou, P.J. vd Wel, F. Voogt, F. Swartjes and K. WeideZaage, Reliability of Wafer Level Chip Scale Packages, Microelectronics Reliability, Volume 54, Issues 9–10, 2014, Pages 1988-1994.


[13] K.Y. Lin and S. Chen, Case study of leakage/short on PCB after biasedHAST, 2016 IEEE 23rd International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA)


110


Contact Leakage Failure Analysis by EBIC, C-AFM and Nano-probing


Kuang-Tse Ho, Chien-Wei Wu, Te-Fu Chang, Chia-Hsiang Yen and Ching-Hsiang Chan


Materials Analysis Technology, 1A3, No.1 Li-Hsing Rd. 1, Science-Based Industrial Park, Hsinchu City, 300 Taiwan  ktho@ma-tek.com


This research sets up failure analysis flow to verify failure  mechanisms and root causes of different kinds of contact  leakage. This flow mainly uses EBIC, C-AFM and nanoprobing to do fault isolation and confirm electrical failure  mechanisms. Appropriate sample preparation is also  mandatory for FIB, SEM and TEM inspection.


In the failure analysis of low yield wafer, ESD test and field  return parts, the standard flow is fault localization by  electrical failure analysis (EFA) followed by physical  inspection by deprocessing or cross-sectioning by Focused Ion  Beam (FIB) or Transmission Electron Microscope (TEM). Contact leakage is one of the most common failure  phenomena. It is usually revealed by passive voltage contrast (PVC) technique [1], but PVC capability is limited. Firstly, it  shows only contacts that are fully open or have large leakage. If a contact suffers from high resistance or has small leakage, it cannot be detected. Secondly, PVC technique indicates only  contact leakage and is unable to tell leakage path. For  example, bright gate contact PVC implies that a possible  failure mechanism is gate oxide breakdown or gate short to  drain/source (D/S). Thirdly, some leakage paths cannot be  observed, like leakage between drain and source or P+ and Nwell. To overcome the above issues, electron beam induced  current (EBIC) [2], conductive atomic force microscope (CAFM) and nano-probing must be used to identify failure  locations or leakage paths to decide which physical  methodology should be adopted. Corresponding cases of  contact leakage failure analysis are collected in this paper. Fault isolation was performed by EBIC, C-AFM or nanoprobing and the root cause was clarified by Scanning Electron  Microscope (SEM), FIB and TEM [3]. A comprehensive  failure analysis flow of contact leakage was set up according  to above achievements. Defects can thus be identified easily.


Experiments


In order to pinpoint precise failure location, probing  technology, EBIC, C-AFM and nano-probing, were utilized. Two nanomanipulators were installed in TESCAN fera3  plasma FIB system for EBIC function. EBIC can be used to  locate gate oxide breakdown and junction defects. C-AFM  was performed with Bruker INNOVA. High resistance or  leaky contacts may be isolated by current mapping and I-V


curve measurements.  Nano-probing was conducted in AFMbased Hyperion AFP to extract transistor characteristics. Leakage path can be confirmed by nano-probing.


Four basic contact leakage paths were studied, including gate  to well, gate to D/S, D/S to well and drain to source. When  gate leakage happens, PVC technique can often reveal leaky  gate contact, and then EBIC can be performed to find out  leakage point. If gate contact PVC is normal or leaky D/S  contact is found by PVC technique, C-AFM and nanoprobing are suggested to confirm leakage path, and then the  appropriate physical failure analysis (PFA) methodology can  be implemented.


A comprehensive failure analysis flow involving all kinds of  contact leakage is presented in Fig.1. The FA flow consists of  five phases. Phase 1 is PVC investigation to localize defective  contact rapidly, and then analyst can decide to use EBIC, CAFM or nano-probing. Phase 2 is probing measurement for  fault isolation or device electrical characteristics extraction by  I-V curve tracing. Phase 3 is to confirm leakage path according to the data obtained by phase 2. Basically, a field effect transistor (FET) has four nodes, drain, source, gate, and well. Analyst needs to judge which two nodes have dominant leakage and proposes the most possible failure model. Then analyst can decide how to do sample preparation and to find out the defect in phase 4. Phase 5 is PFA to observe the defect by microscopy.


Figure 1: contact leakage failure analysis flow.


The detailed FA flow will be discussed according to the four  failure mechanisms in phase 3, i.e. gate to well, gate to D/S, D/S to well and drain to source. Each leakage path has its  associated possible root causes. Once the possible root causes


111


are proposed, corresponding sample preparation and  inspection microscopy will be applied.


A. Leakage between gate and well


When gate contact PVC is brighter than that of normal ones, one of the failure mechanism is leakage between gate and  well, or gate oxide breakdown. Sometimes leaky contacts  cannot be identified by PVC due to smaller leakage, and then  C-AFM can be implemented to reveal these contacts as shown  in Fig.2. Fig.2(a) is suspicious area localized by photon  emission microscopy (PEM), but no anomaly was found by  PVC technology. Fig.2(b) and (c) are current mapping done  by C-AFM in reference and failed units, respectively. The  difference apparently showed abnormal contact. Traditionally, the sample was deprocessed to polysilicon by  parallel lapping and then polysilicon can be etched away by  diluted potassium hydroxide (KOH) to reveal gate oxide  pinhole. However, such FA method suffers from lower sample  preparation success rate, defects are destroyed and process  issue cannot be shown by top view. Since preserving original  defects is the most important in failure analysis for  countermeasure proposal, this method is not suitable to dig  out the possible root cause.


Figure 2: (a) normal PVC in failed unit (b) reference unit by  C-AFM (c) abnormal contact found by C-AFM in failed unit.


Most gate oxide breakdown points can be revealed by EBIC  successfully with only one probe. EBIC current can flow  between probe and substrate. After defect localization, crosssectional TEM is suggested to perform. Fig.3(a) shows that  non-uniform gate oxide thickness induced gate oxide  breakdown, and Fig.3(b) was dielectric breakdown induced  epitaxy (DBIE) [4].


Figure 3: one-probe EBIC (a) thinner gate oxide caused gate  oxide breakdown (b) DBIE due to electrical over stress.


If device structure is deep n-well (DNW) or silicon on  insulator (SOI), EBIC current is not able to flow from probe  to substrate, and then EBIC with two probes, one connected  to gate contact and the other connected to well contact, must  be used to enhance breakdown spots. As shown in Fig.4, the  product had DNW structure and two probes are necessary to  reveal the EBIC spots. Cross-sectional FIB proved it was gate  oxide breakdown.


Figure 4: two-probe EBIC revealed gate oxide breakdown  site and cross-sectional FIB was performed to show gate  oxide breakdown.


If the breakdown is too serious and induces ohmic short  between polysilicon gate and substrate, which is verified by  IV curve tracing function in EBIC system, EBIC spots won’t  be observed due to absence of micro p-n junction [5]. It is  suspected that silicon substrate suffered from serious burnout, and substrate damage can be found easily after all layers are  removed. Fig.5(a) shows IV curve representing direct short  between substrate and abnormal gate with brighter PVC. Fig.5(b) illustrates obvious substrate burnout identified by red  circles by top view SEM inspection.


Figure 5: (a) direct short between gate and substrate (b) serious substrate burnout in channel region.


B. Leakage between gate and D/S


Not all gate contact PVC anomalies are due to gate oxide  breakdown. It may result from gate short to D/S, too. Some  defects can be found by EBIC. Fig.6 shows Ti residue  inducing gate short to silicide in D/S region. It was suspected  that Ti-silicide-substrate formed Schottky barrier and built-in  field to separate generated electron-hole pairs.


If EBIC spots cannot be observed and IV curve tracing


demonstrates gate short to D/S, it indicates that there’s no


built-in field between gate and substrate. The defect must be  above silicon substrate. To find out the defect, interlayer  dielectric (ILD) can be thinned by parallel lapping and defect  can be searched under high kilo-voltage SEM inspection.


112


Fig.7(a) shows that abnormal gate PVC was found under 1kV  SEM inspection. Direct short between gate and drain was  measured using nano-probing in Fig.7(b). After ILD  thinning, a residue was found between drain contact and  polysilicon gate by SEM as shown in Fig.7(c). Since the  defect was very small and detailed defect profile was  necessary to be checked, cross-sectional TEM was performed  as shown in Fig.7(d). Obviously, a metal-like residue lay  upon spacer and caused short between gate silicide and  contact. In order to investigate the root cause, energy  dispersive X-ray spectroscopy (EDX) mapping was utilized to  check element distribution. The residue was confirmed to be  titanium which dropped after SiN spacer and before oxide  liner deposition as shown in Fig.8.


Figure 6: (a) PVC showed abnormal gate contacts (b) EBIC  spot was located at polysilicon edge (c) Ti residue on spacer  caused gate short to D/S observed by cross-sectional FIB.


Figure 7: (a) abnormal gate contact PVC (b) IV curve of gate  to drain by nano-probing showed direct short (c) residue was  found after ILD thinning (d) Ti residue was found by crosssectional TEM.


Figure 8: EDX mapping revealed Ti (blue) residue on SiN  spacer.


C. Leakage between D/S and well


Leakage between D/S and well is junction leakage which can  be isolated in rough region by PEM first, and then failed  contact can be narrowed down by PVC, C-AFM or nanoprobing. Junction defects can be observed by plan-view or  cross-sectional SEM/TEM. Fig.9 showed that leaky contacts  were highlighted by current mapping of C-AFM under  biasing of -2V. From the circuit structure analysis, the only  leakage path is junction leakage. Plan-view SEM inspection  was performed after removing all layers, and burnout was  found at failed contact location.


Figure 9: (a) leakage locations revealed by C-AFM (b)(c) Location 10-2 and 4-9 showed burnout by plan-view SEM.


Another junction leakage case is presented in Fig.10. Fig.10(a) was atomic force microscopy (AFM) topography in  the region of interest. Fig.10(b) and Fig.10(c) were the  current mapping of C-AFM by biasing the substrate -2V and +2V, respectively, and no obvious abnormality was found. However, IV curve in Fig.10(d) reveals pico-ampere order  difference between failed and normal contacts at +2V. The  color bar of current mapping is in nano-ampere range. That’s  why such junction leakage was only found by IV curve  tracing instead of current mapping. Fig.11 shows burnout at  contact bottom observed by cross-sectional FIB.


113


Figure 10: (a) AFM topography in ROI (b) current mapping  at substrate bias -2V (c) current mapping at substrate bias +2V (d) IV curve comparison between failed and normal  contacts.


Figure 11: burnout at contact bottom, resulting in junction  leakage.


D. Leakage between drain and source


Drain to source leakage cannot be detected by PVC and CAFM since PVC is only used to find out leaky via or contact  with different potential, and C-AFM can only measure the  current path in vertical direction, like drain to substrate or  gate to substrate. EBIC can detect signal, but precise defect  location cannot be pointed out. As shown in Fig.12, whole  channel was bright when probing drain and source in EBIC  operation. Hence, EBIC also fails to locate such line defects  in drain to source leakage. It must be characterized by nanoprobing first. Basically, turn-off current (Ioff), which is Ids  measurement at Vgs=0V and Vds=Vdd, can be used to judge  drain to source leakage. If Id is opposite to Is and Ig has no


leakage, it means the gate is unable to control the channel, and there is direct leakage path between drain and source. It  also indicates that this defect must exist under silicon  substrate due to absence of gate oxide leakage. Now that it is  substrate anomaly, plan-view SEM or TEM is suggested to  reveal substrate or crystal defects.


Figure 12: EBIC signal highlighted only conducting channel, and failed to locate precise defect location.


There are two cases which suffered from drain short to source  presented in this paper. The first case is shown in Fig.13. Fig.13(a) was IV curve showing drain current (ID), source  current (IS), gate current (IG) and bulk current (IB) by  sweeping drain voltage from 0V to 5V and biasing all other  nodes with 0V using nano-probing. IV curve verified that  drain was short to source directly without gate leakage. The  standard delayering procedure was followed by plan-view  SEM after removing all layers. Punch-through phenomenon  was found easily as shown in Fig.13(b). Note that even  though this burnout was serious, gate oxide was not damaged.


Figure 13: (a) drain to source short was confirmed by I-V  curve measurement (b) punchthrough inspection by SEM.


The IV curve in the second case also indicated drain to source  leakage by sweeping the drain voltage from 0V to 3V and  forcing other nodes with 0V by nano-probing. Obviously, drain had leakage and its current was opposite to source  current as shown in Fig.14(a). That meant there was a  leakage path between drain and source. Since minor defect in  Si substrate was expected per IV curve, plan-view TEM was  conducted. As illustrated in the left part of Fig.14(b), two  dislocation lines were across whole device at the edge of  active area. In order to understand dislocation depth, the  same sample was prepared for cross-sectional TEM for 3D  TEM imaging as shown in the right part of Fig.14(b). It was  found that the dislocations were located at the shallow trench  isolation (STI) bottom corner and was possibly induced by  STI stress [6].


114


Figure 14: (a) drain to source leakage was confirmed by I-V  curve measurement (b) plan-view TEM revealed that  dislocations were at the edge of active area and across whole  device. Cross-sectional TEM showed that dislocations were  at STI bottom corner.


In this paper, several possible contact leakage mechanisms  are presented and associated FA procedures are proposed. Following the flow, all device-related defects inducing  leakage can be identified by EBIC, C-AFM, and nanoprobing and verified by SEM, FIB, and TEM examination.


The author would like to thank nano-probing team for fault  isolation, project team for delayering and FIB/TEM team for  physical analysis support.


[1] R. Rosenkranz, “Failure localization with active and  passive voltage contrast in FIB and SEM,”


Microelectronics Failure Analysis: Desk Reference 2011


Supplement, pp. 269-278


[2] M. Strizich, “Electron beam induced current isolation  techniques,” Electronic Device Failure Analysis News,


vol. 2, No. 1 (2000), pp. 1-9


[3] N. Wang, S. Daniel, “Microanalysis of Semiconductor  Devices with FIB and TEM for Identifying Small


Defects,” Microelectronics Failure Analysis: Desk


Reference 2002 Supplement, pp. 21-28


[4] C.Y. Lu, C.H. Tung, K.L. Pey, “Microstructure evolution  and breakdown mechanism studies in mosfet with ultra


thin gate dielectrics in nanometer technology era,”


Electrochemical Society Proceedings Volume 2004-04, pp. 404-417


[5] M. Tamatsuka, S. Oka, H.R. Kirk, G.A. Rozgonyi,


“Novel GOI failure analysis using SEM/MOS/EBIC with  sub-nano ampere current breakdown,” Electrochemical  Society Proceedings Volume 97-12, pp. 80-91


[6] K. Parekh, C. Mouli, M. Hermes, F. Gonzalez, “Processinduced defects and diode leakage in ULSI FEOL  integration,” Electrochemical Society Proceedings  Volume 2001-2, pp. 359-372


115


Contamination Troubleshooting Approach from Problem to Solution


Victor K.F. Chia, Hugh E. Gotts, Fuhe Li and Mark Camenzind


Balazs NanoAnalysis, Air Liquide   46409 Landing Parkway, Fremont, CA 94538, USA  Phone: +1 510-825-3701   Email: victor.chia@airliquide.com


Semiconductor devices are sensitive to contamination that can  cause product defects and product rejects. There are many  possible types and sources of contamination. Root cause  resolution of the contamination source can improve yield. The  purpose of contamination troubleshooting is to identify and  eliminate major yield limiters. This requires the use of a  variety of analytical techniques[1]. Most important, it requires  an understanding of the principle of contamination  troubleshooting and general knowledge of analytical tests. This  paper describes a contamination troubleshooting approach  with case studies as examples of its application.


Integrated circuits (IC) are the heart and brains of most circuits  that are in modern electronic products. Studies estimate that  contamination may be responsible for 50% or more of the  yield loss in IC fabrication. All types of contamination can  cause fatal device failures, from fibers to particles to  molecules. Contamination can generally be divided into three  categories. Namely, ionic contamination[2], airborne  molecular contamination (AMC)[3] and particles defect  density[4].


Particles larger than about ¼ of the minimum line-width may  cause fatal device failure. An important process step is  therefore wafer cleaning. The number of cleaning steps have  increased with each generation of the semiconductor  manufacturing process, also known as "technology node." For  example, Dynamic Random-Access Memory (DRAM) cleaning counts have increased from about 40 to 75 cleans  with decreasing nodes from 0.30-μm to 0.12-μm. Similarly, the  number of cleaning steps for Complementary Metal–Oxide–Semiconductor CMOS logic has increased from 40 to about  140 with decreasing nodes from 0.28-μm to 0.07-μm.


Despite the introduction of cleaning steps, contamination still  occurs causing (i) environmental induced defects from  cleanrooms, cleanroom suits and HEPA filters, (ii) particle  defects from process chemicals, ultrapure water, packaging  and consumables, (iii) handling errors from automation and  static electricity control, and (iv) equipment-induced defects  from process tool ceramic and quartz components.


The defect type must be identified when a contamination  escalation or yield problem occurs after which an effort should  be made to find the source of the defects and to fix the  problem. We will discuss an approach to identify the  contamination and to determine the root source and possible  cause.


Analytical Criteria


The first step is to understand the history of the sample  because this will provide an insight to the defect and  contamination type and their probable spatial and lateral  locations on the wafer. For example, if we know the  contaminant was detected after thermal anneal or ion  implantation then there is a high probability the contamination  was driven into the wafer by thermal energy and knock-on, respectively. Additional knowledge of the contaminant’s  concentration or defect size will enable the appropriate  analytical techniques to be selected based on the instrument’s  capabilities.


Table 1: Analytical Criteria to Select the Appropriate Test  Method.


Indirect and Direct Analytical Techniques


A test criterion often overlooked when selecting an analytical  technique is whether a test method provides direct or indirect  results. Figure 1 is a dining table setting to illustrate this. The  table is the wafer and the plates and glasses, for example, represent the different types of contamination.


To characterize and quantify the contaminants, we can perform  the analysis by washing off all the contaminants from the table  and collecting them in a bucket for analysis. This is an indirect


116


approach and depicts a leach or extraction test. The sampling  or extraction preparation step is used to collect the  contamination on a wafer and an aliquot of the extract solution  is analyzed by Inductively Coupled Plasma Mass Spectrometry (ICP-MS) for metals, Ion Chromatography (IC) for anions (and cations) and Gas Chromatography–Mass Spectrometry (GC-MS) for organics. A caveat for this extraction procedure  is it assumes all the contaminants are removed from the  surface for analysis.


Figure 1: A schematic representation of a wafer with  contaminants as depicted by a dining table setting. The plates  and glasses represent contaminants.


A direct test method can micro sample and analyze individual  defects on the wafer. An incident beam is focused onto the  contaminant of interest and depending on the type of incident  beam source the contaminants are excited and emit some forms  of characteristic signals with specific energy, wavelength, electron or molecule that can be detected. A direct test method  can characterize and quantify specific defects, even a silicon  particle on a silicon wafer. Or in the case of the dining set  analogy, a direct test method can differentiate a dinner plate  from a salad plate or a water goblet from a wine glass.


The following illustrates the difference in application between  an indirect and direct test method. An example of an indirect  application is to qualify a new wafer carrier or Front Opening  Unified Pod or Front Opening Universal Pod (FOUP) vendor  for organic outgassing. The qualification test requires witness  wafers to be placed in the carrier and to place the carrier in an  oven at 50 C for 1 hr. Outgassed compounds from the carrier  are physisorbed onto the wafer. The wafers are then removed  and analyzed by full wafer outgassing using Thermal  Desorption (TD) GC-MS per SEMI MF1982-0317[5] with a  reporting detection limit of 0.1 ng/cm2.


A direct test method is required to determine which carrier  component is responsible for the outgassed organics onto the  wafer. Pieces of the carrier or FOUP are cut and analyzed by  TD GC-MS using IEST-RP-CC31[6] analysis protocol. Figure  2 shows the results of the outgassed compounds from the box  and lid of a wafer carrier and reveals they have different


organic signatures. The source is confirmed by matching the  organic signatures of the wafer and the carrier components.


Figure 2: TD GC-MS outgassing results from a wafer carrier  box and lid, outgassed at 50 C for 30 min.


Selecting an Analytical Technique


Identifying the cause of a defect is usually the most time  consuming and costly component of yield improvement  efforts. Some defect types are not too difficult to diagnose. Easy to diagnose defects include those caused by particles  because they are often still present during in-line inspection. Consequently, the particle composition can be determined by a  technique, such as Scanning Electron Microscopy with Energy  Dispersive Spectroscopy (SEM-EDS), a valuable screening  technique. SEM provides the visual “answer” while EDS  provides the elemental “answer.”


On the other hand, some defect types are difficult to diagnose  because they occur sometime during a process cycle and takes  on some distorted shape or appearance that can further  complicate diagnosis. Contamination troubleshooting typically  involves process tool partitioning and running pre-designed  experiments. Such experiments commonly involve processing  sets of wafers with different fabrication recipes. Often, the  number of wafers used in such experiments is limited in order  to save material costs and reduced tool time. But if too few  wafers are used, experimental results may turn out to be  inconclusive thereby further frustrating the defect diagnosis.


Contamination troubleshooting is a multidisciplinary process  and includes visual inspections, metallographic, environmental  and chemical analysis and simulation tests. An analytical test  plan typically utilizes a number of analytical techniques  ranging from traditional wet chemical analysis to advanced  surface characterization. Analytical techniques have specific  applications and each technique has advantages and  limitations.


Figure 3 shows an analytical decision tree to guide the  selection of a technique to characterize a defect or  contamination. SEM-EDS is always a good “first look”


117


technique to use. It provides elemental information that can  determine if the defect is inorganic or organic. The decision  tree then directs the selection of an inorganic and organic  technique for surface and in-depth analyses and suggests  techniques for analyzing low and high concentration defects. Notice some techniques in Fig. 3 are positioned in two  categories. For example, Time-of-Flight Secondary Ion Mass  Spectrometry (TOF-SIMS) and X-ray Photoelectron  Spectroscopy (XPS) can perform surface and in-depth  analyses.


Some techniques are ideal for surface or in-depth/bulk  analysis. And some are suited to detect gross (high) contamination. While others are best suited to low


concentration analyses. For example, a human or glove print is


a “killer” defect that can result in scrapping wafer lots due to


IC device failures. This killer defect may be only 0.1  monolayer or ~2 Å of organics on a surface that is ~ 1014  atoms/cm2. Time-of-Flight SIMS and TD GC-MS is best  suited to meet these detection limits.


The specific requirements of individual situations will often  dictate the choice of technique that is most appropriate. In  general, no single analytical technique can provide the answer  to every contamination problem, especially if the goal is to  identify and implement a root cause fix of the defect source.


Figure 3: An analytical decision tree for contamination troubleshooting and failure analysis.


Figure 4: Mathematical model for contamination troubleshooting and a schematic escalation and  contamination reduction cycle to implement a root cause fix.


118


Process Cycle for a Root Cause Fix


Figure 4 shows an approach to determine the root source of a  contamination and steps to implement a root cause fix. Low  yield results when high concentration of contaminants, such as  A, B, C, D, etc., build up during a period of time and exceed  the contamination threshold of the process step, thereby  causing the failure. Capital “A” denotes a high concentration  of “A.” Contaminant “A” may be Na, for example. The next  step is to determine where and when the contaminant was  introduced. The Escalation Cycle is important to do next  because following a hunch can be time consuming and can  lead to no positive result. Partitioning experiments will  determine if the source is Fab, Tool or Process related. The fix  is specific to the source. For example, a Fab related solution  may be as simple as introducing more wipe downs and glove  changes during the shift. A Tool related solution may be to  replace an O-ring that is degrading from the harsh process  environment. And, a Process related fix may be to replace the  high purity alumina liner of the diffusion furnace.


The end game is the Contamination Reduction Cycle to  replace the defective material or part. The worst-case scenario  is for the need to qualify a new material or vendor that is time  consuming. Note, the root cause may be from poor adherence  of a protocol and the fix may simply be to add more stringent  checks and balances. Perhaps, the addition of inspection steps  or more wipe down is sufficient. High yield can now be  achieved because the contaminant concentration is reduced. The High Yield equation in Fig. 4 reflects this with a lower  case “a” indicating a low concentration of “a.” The time  interval before the next failure is extended because it now  takes longer to accumulate and exceed the contamination  threshold.


Case Studies


TDDB (Time Dependent Dielectric Breakdown)


Intermittent time dependent dielectric breakdown (TDDB)[7] is observed after wafer processing. Mobile ions are frequently  the cause of this type of electrical failure. Following the  analytical decision tree, Vapor Phase Decomposition (VPD) ICP-MS or Total Reflection X-ray Fluorescence (TXRF) are  appropriate techniques to consider. VPD ICP-MS is better in  this case because it can detect Na while TXRF cannot. VPD  ICP-MS also has lower detection limit than TXRF and  provides total surface measurement while TXRF measures  predetermined locations. Na was detected on the wafer that  was not surprising because Na is a common contaminant of  TDDB. Process tool partitioning experiments were performed  and determined Na was introduced after a new chamber kit  was installed in the plasma process tool.


Inspection of the chamber kit components revealed discolored  ceramic isolators. The coloration was characterized by  ultraviolet (UV) fluorescence and by FTIR that showed the  presence of an organic residue of straight chain aliphatic


hydrocarbons. Ultrapure water (UPW) leach of the discolored  ceramics followed by ion chromatography determined the  discolored ceramic contained Na, as shown in Fig. 5. The  ceramic isolators were cleaned and re-installed.


Figure 5: Ultrapure water leach/extraction and ion  chromatography analysis of discolored ceramic isolators.


The TDDB problem re-occurred. An in-depth analysis using  Laser Ablation Inductively Coupled Plasma Mass  Spectrometry (LA ICP-MS)[8] was performed on the ceramic  isolators to verify a hypothesis that there was a virtual Na  source deep within the ceramic isolators. The LA ICP-MS  depth profile shown in Fig. 6 confirmed this hypothesis. So, even though the isolators were cleaned, the in-depth Na  migrated to the ceramic surface during plasma processing and  contaminated the wafer.


Figure 6: Laser ablation ICP-MS depth profile of discolored  ceramic isolators.


The focus of the investigation now turned to how Na was  introduced into the ceramic isolators. A Process  Contamination audit of the ceramic supplier revealed poor  handling of the ceramic isolators prior to sintering. The oven  was tested for cleanliness using critical wipes and witness  wafers. Na was detected by both test methods. Na level builtup in the oven over time because it was not frequently cleaned. Na in the oven cross-contaminated the ceramics and during the  sintering process and Na was driven into the ceramic isolators. The intrinsic Na migrated to the ceramic surface during plasma  processing and deposited onto the wafer causing the TDDB. The vendor has several ovens and only ceramic batches from  this contaminated oven were troublesome. The time taken to  resolve this escalation took longer than expected because not  all the ceramic isolators from the vendor had issue. But once


119


the ovens were identified as a potential culprit the  investigation concluded swiftly.


Aperture Degradation


An aperture beam strip was installed in a process tool during  routine preventive maintenance (PM). The aperture strip has 5  apertures, each are 12 μm in diameter. When an aperture is “blown” larger by the primary source over time, the engineer  can move the strip over to expose the next new aperture to the  beam. This allows the tool to continue processing longer  between tool maintenance.


During tool start up, the beam current was observed to be well  below the SPC’s LCL (lower control limit). SEM images  showed the aperture diameters were smaller than the 12 μm  specification, as shown in Fig. 7.


Figure 7: SEM images of current beam apertures showing  different internal diameters and a common “halo” diameter.


The left and right images show the aperture diameters to be ~5.89 μm and ~8.63 μm in diameter, respectively. The SEM  images also revealed a “halo” around all the aperture openings  and corresponds to ~12 μm diameter. Figure 8A shows EDS  spectra from the “halo” region and in a control area outside of  the “halo” region. The spectrum of the control area is shown  by itself in Fig 8B for clarity.


Figure 8: SEM images of current beam apertures showing


different internal diameters and a common “halo” diameter.


The composition of the “halo” region is composed primarily of  Si, O and C. Adventitious C is always present on a sample as  shown in spectrum B. However, the Carbon intensity in  spectrum A is well above the control level. The EDS result  suggests the “halo” is composed of an organic compound  composed of Si, O and C.


Materials in proximity with the aperture during shipment were  analyzed by TD GC-MS. The preliminary analyses led to  further investigation of the packaging. Current and past  adhesive gels used to secure the apertures in the package were  analyzed. The results are summarized in Fig. 9.


Figure 9: TD GC-MS outgassing results of packaging  adhesive systems. The new adhesive outgassed 15 time more  than the previous adhesive packaging system.


The TD GC-MS results shown in Fig. 9 revealed the new  adhesive gel, though less sticky for ease of product removal, outgassed more, ~15 times higher, than the previous adhesive  gel product. TD GC-MS data confirmed the organo-Si  compound of the aperture “halo” and the gel composition were  the same thus confirming the adhesive gel was the source of  the “halo.” The solution is for the packaging supplier to revise  their adhesive gel’s chemistry for low outgassing and to use no  plasticizers. A corrective action was to ensure any changes  made by the supplier were documented and provided to their  customers with a certificate of analysis (CoA).


Bond Pad Defect


Figure 10 shows a defect on a 50 μm x 50 μm bond pad. The  defect appeared to be a piece of plastic material. Raman  spectroscopy was selected because the material was suspected  to have polyethylene/ethylene vinyl acetate (PE/EVA) polymer  blends. The vinyl group has a symmetric stretching mode  known to give a moderate to strong Raman signal. This mode  is better observed by Raman scattering than infrared  absorption since it usually appears weak in the infrared. Figure  11 shows the Raman spectrum of the defect and revealed it  was composed of polyethylene and other types of resins.


Figure 10: SEM images of the defect on a 50 μm x 50 μm bond  pad.


Figure 11: Raman spectrum of the defect on a 50 μm x 50 μm  bond pad.


Figure 12: Raman spectra of blue (top) and white (bottom) nitrile gloves.


Many plastic materials were analyzed to determine what this  defect could be. Figure 12 shows the Raman spectra of a blue  and white nitrile glove. Eventually, a blue bubble wrap was  concluded to be the defect material as shown by the matching  spectra in Fig 13. Initial discussion with the supplier suggests  the cause was operation related. A Process Contamination  audit confirmed the cause and a new a robust operation system  was established that eliminated reliance on human error.


Figure 13: Raman spectra of the defect and bubble wrap. The  two spectra show a good correlation.


Vibration Isolation Pad Failure


After a preventive maintenance (PM) the process tool base  pressure increased, and Cl was detected on the wafer at 5x1013  at/cm2 by TXRF. All metals measured by TXRF were present  at or below 5x1010 at/cm2 that was the tool wafer cleanliness  specification. The fix is different for an inorganic Cl versus an  organic Cl. An analytical test plan can be made based on the  portion of the analytical decision tree shown in Fig. 14.


Figure 14: A portion of the analytical decision tree to  determine if Chlorine on the wafer is inorganic or organic.


Chlorine was determined to be from an organo-chloride  compound using full wafer TD GC-MS. Chlorine was not from  insufficient rinsing after acid cleaning or from poor handling  since no ionic Cl was detected on the wafer from UPW  extraction and ion chromatography.


Interestingly, a wafer left on the electrostatic chuck (ESC) for  1 h in the tool showed no Cl while a wafer after cycling  through the tool showed Cl at 5x1013 at/cm2. The latter Cl  concentration could be generated anytime by cycling a wafer  through the tool. This experimental observation will become  significance after we identify the contamination source.


The organo-chloride compound was identified as a common  flame retardant. Flame retardant chemicals address smoldering  ignition and was commonly used on furniture fabrics and foam  until about 2015. After reviewing the build of material (BOM), the root source of the organo-chloride compound was traced to  a vibration isolation pad that was blue in color. The BOM  specified a black vibration pad that does not outgas, confirmed  by TD GC-MS analysis. The outgassed compounds from the  blue isolation pad matched the wafer organic signature, thereby confirming it to be the source.


The static and dynamic tool wafer results now become clear. No water leaks from a saturated sponge if you hold it carefully. However, if you shake your hand some water will leak out of  the sponge. When the wafer handler is static the pads are not  active and do not outgas. However, when the wafer handler is  moving the pads are adsorbing vibrations and in the process


121


they will compress and outgas. So, even though the mechanical  and physical specifications for the blue isolation pad was met, its outgassing property was not because it was not specified. An action item is to establish an outgassing specification and  include it clearly on the part’s document and drawing.


The objective of this paper is to provide a guideline to  troubleshoot contamination from problem to solution. The goal  of any contamination issue is to eradicate the contamination  source once and for all so it will not return. We discussed the  criteria for selecting the best analytical technique, the thought  process to identify the contaminant and a process to determine  the root source and cause. Successful case studies are  presented to illustrate this approach to implement a root cause  fix.


Product defects in IC fabrication or in any manufacturing  process is detrimental to product quality and yield. Customers  are always demanding higher quality in their product. Competitive manufacturing requires trying to reduce the  operating cost to stay profitable. Any contamination issues  during manufacturing can cause delays as defective parts have  to be weeded out of the system. In addition, the process of  identifying the root cause and then implementing an  improvement action plan is time consuming. It is important to  be thorough in the first pass to ensure the contamination  escalation is fully understood so that it can be resolved as  quickly as possible.


Challenges along the way to reduce defect rates include  showing the influence of cleanroom air, semiconductor  processes and tools, gases, chemicals, deionized water, etc. to  the manufacturing process. With increasing material and  processing complexities, defects and yield loss mechanisms  must be considered an integral part of the process  development. This can only be done if a coordinated effort is  focused to achieve contamination-free manufacturing.


The author wishes to thank Balazs NanoAnalysis’ analysts and  scientists of the Fremont laboratory. The Water Lab provided  the UPW leach results, the Organic Lab provided the TD GCMS and Raman results, and the Advanced Materials Lab  provided the LA ICP-MS, SEM and EDS results.


[1] V.K.F. Chia, “A Review of Analytical Techniques for  Identifying Contaminants in the Semiconductor Industry,”


47th Annual Meeting of the Institute of Environmental


Sciences and Technology, Phoenix, AZ, April 22-25,


2001.


[2] I-Kai Lin, Hsunling Bai, and Bi-Jun Wu, “Surface  Deposition of Ionic Contaminants on Silicon Wafers in a  Cleanroom Environment,” IEEE Transactions on  Semiconductor Manufacturing, Vol 22, No.2, May, 2009  pp 321.


[3] Walter Den, Hsunling Bai and Yuhao Kang, “Organic  Airborne Molecular Contamination in Semiconductor  Fabrication Clean Rooms,” Journal of the  Electrochemical Society, 153, October 12, 2006, pp. 149-159.


[4] Robyn Coleman, “Particulate and Defect Reduction  Strategies for Semiconductor Devices: Tools and  Methodologies,” Particles on Surfaces, Ch 3, pp 203-215.


[5] SEMI Standards, “SEMI MF1982 - Test Method for  Analyzing Organic Contaminants on Silicon Wafer  Surfaces by Thermal Desorption Gas Chromatography.”


[6] Institute of Environmental Sciences and Technology (IEST), Recommended Practice (RP), IEST-RP-CC031.3, “Method for Characterizing Outgassed Organic  Compound from Cleanroom Materials and Components.”


[7] Mustafa Tarık Saniç and Mustafa Berke Yelten, “Timedependent dielectric breakdown (TDDB) reliability  analysis of CMOS analog and radio frequency (RF) circuits,” Analog Integrated Circuits and Signal  Processing, October 2018, Volume 97, Issue 1, pp 39–47.


[8] Fuhe Li and Scott Anderson, “A new approach to  chemical analysis of packaging/assembly materials: SARIS™ laser ablation ICP mass spectrometry,” Proceedings of the IEEE/CPMT 29th International  Electronics Manufacturing Technology (IEMT) Symposium, February 2004.


122


# Case Study of Electro-Optical Probing Signal with High Signal-Noise Ratio


Case Study of Electro-Optical Probing Signal with High Signal-Noise Ratio


Ryan Xiao, William Wang, Ang Li, Shengqiu Xu, Binghai Liu


NXP Semiconductors, Tianjin, China


E-mail: nan.xiao_1@nxp.com, Phone: 86-22-85684202


With the development of semiconductor technology and the  increment quantity of metal layers in past few years, backside  EFA (Electrical Failure Analysis) technology has become the  dominant method. In this paper, abnormally high Signal Noise  Ratio (SNR) signal captured by Electro-Optical Probing (EOP)/ Laser Voltage Probing (LVP) from backside is shown  and the cause of these phenomena are studied. Based on the  real case collection, two kinds of failure mode are  summarized, and simulated experiments are performed. The  results indicate that when a current path from power to ground  is formed, the high SNR signal can be captured at the  transistor which was on this current path. It is helpful of this  consequence for FA to identify the failure mode by high SNR  signal.


EOP technique is frequently-used one during EFA to obtain  the operational information of internal circuit from backside. Based on the waveforms captured by EOP, logical error can be  identified, and the failure can be isolated [1].


In some of the cases we have done, abnormal EOP signal with  very high SNR can be captured and caught our attention. In  order to explore and study the hidden clues of this kind of  signal brought to us, statistic and classification analysis has  been completed and it turns out that these cases can be divided  into two groups. In the following paragraphs, cases from each  group was selected respectively for brief introduction.


Case 1


The first was a scan chain failure case. The output of suspected  scan cell was missing. During capturing the EOP waveform  along the data path, high SNR signal with correct data was  found at Pmos of the inverter from I99 to Q, and the correct  signal with slow rising and falling edge was captured at Nmos. Based on the EFA finding, Physical Failure Analysis (PFA) was performed and low resistance (~40kOhm) IV curve was  found between I99 and ground, and V2-M2 short was  observed by Transmission Electron Microscopy (TEM). In this  case, the high SNR signal was found at the Pmos of the  inverter whose output short to ground. Fig.1 showed the EOP  waveform, the schematic of scan cell and its corresponding  TEM image.


Figure 1: Images of first sharing case


(a)EOP waveforms image on reference and rejected sample;(b)Schematic circuit diagram of suspected scan cell; (c)IV curve between net Q and Vss; (d)Defect image by TEM.


Case 2


The second was also a scan chain failure case. A bunch of  emission sites were captured by Photon Emission Microscopy (PEM) with InGaAs camera, and all of them were located at  the downstream inverters of pink net in Fig.2 (a) & (b). Based  on the schematic study, the failure was located at the Scan  Enable (SE) path. In the process of capturing the waveform  along the path, high SNR signal with clock signal was found at  the inverters where PEM spots were located. Based on the  EFA finding, PFA was performed and net open was found by  EBAC, abnormal metal and via were observed by  Transmission Electron Microscopy (TEM). In this case, the  high SNR signal was found at the inverters whose input was  floating. Fig.2 shows the PEM image, the schematic of related


123


circuit, the EOP waveform, the Electron Beam Absorbed  Current (EBAC) image and its corresponding TEM image.


Figure 2: Images of second sharing case


(a)PEM image overlaid with layout; (b)Related schematic  circuit diagram; (c)EOP waveforms image of rejected sample; (d)EBAC image and corresponding net outline;


Figure 2 Continued:


(e)Defect image by Transmission Electron Microscopy (TEM).


According to the two cases above, it can be concluded that the  high SNR signal may be captured at the device when two kinds  of failure mechanism was occurred:


1. The input of the inverter is floating.


2. The output of the device is short to power or ground.


In order to verify whether the suspecion is correct, a series of  simulation experiments are conducted for further judgement of  the generation of high SNR signals.


Simulation Experiment


In this paragraph, four kinds of experiment were designed and  carried out to verify the generation of high SNR signal. For the  convenience of circuit edit and EOP waveform capturing, all  the experiments are carried out with 90nm wafer technology  and LQFP package sample.


Experiment 1: Output net short to power


In the first experiment, one internal net n_5750 was connected  to Vdd to simulate the failure mechanism: output net short to  power. The net we selected was the output of one inverter, and  scan chain pattern was used to inject the data to this net. The  Optical Microscopy (OM) image of circuit edit, the PEM  image, the schematic of related circuit and the EOP waveform  were shown respectively in Fig.3(a) to Fig.3(d). The result  shows that high SNR signal with correct data and little clock  signal was observed at Nmos of the inverter whose drain was  short to power, and abnormal signal with slow rising and  falling edge was found at Pmos of the inverter. PEM spot also  locateed at the Nmos where high SNR signal captured.


124


Figure 3: images of Experiment one


(a)Optical Microscopy image of circuit edit to connect the net  n_5750 to Vdd; (b)PEM image; (c)Related schematic circuit  diagram; (d)EOP waveforms image of reference and


experimental sample;


Figure 4: images of Experiment two


(a)Optical Microscopy image of circuit edit to connect the net  n_5750 to Vss; (b)PEM image; (c)Related schematic circuit  diagram; (d)EOP waveforms image of reference and


125


Experiment 2: Output net short to ground


The internal net n_5750 which shown above was connected to  Vss manually in the second experiment. Fig.4 showed the OM  image of circuit edit, the PEM image, the schematic of related  circuit and the EOP waveform. The result showed that high  SNR signal with correct data and little clock signal was  observed at Pmos of the inverter whose drain was short to  ground, and abnormal signal with slow rising and falling edge  was found at Nmos of the inverter. PEM spot also located at  the Pmos where high SNR signal captured.


Experiment 3: Input net of AND open


In the third experiment, net n_5750 which was one of the  inputs of the AND cell was cut off manually. Fig.5 (a) to (d) showed the OM image of circuit edit, the PEM image, the  schematic of related circuit and the EOP waveform  respectively. The result showed that no high SNR signal was  observed at the transistors which directly connected to the  floating net (N/Pmos A/B). Instead, wrong data was found at  downstream transistors, and slight PEM spot was observed at  Pmos B. The conclusion was that the experiment result didn’t  match our suspicion, high SNR signal wasn’t found at  downstream transistors which were directly controlled by  floating net.


In the third experiment, we tried to simulate the open failure  and find the relationship between the defect and the generation  of high SNR waveform. However, high SNR signal didn’t  appear on the suspected transistor. Based on this fact, we  attempted to find some other commonalities except open  failure mechanism. After deep study, two commonalities were  concluded from the real cases which existed high SNR signal:


1. For the open defect, all the downstream cells where found  high SNR signal were the inverter.


2. The open net was the global signal, such as clock path or  scan enable path.


Based on the two information above, the corresponding  experiment will be carried on, and introduced on Experiment 4 & 5.


Experiment 4: Input net of inverter open


In the fourth experiment, n_5740 which is the input of one  inverter was selected and cut off manually. Fig.6 (a) to (d) showed the OM image of circuit edit, the PEM image, the  schematic of related circuit and the EOP waveform  respectively. The result showed that no high SNR signal was  observed at the transistors which directly connected to the  floating net (N/Pmos A/B), only wrong data at downstream  transistors, and PEM spot at Nmos B. The conclusion of this


experiment was that the result didn’t match our suspicion, high  SNR signal wasn’t found at downstream transistors which


were directly controlled by floating net.


Figure 5: images of Experiment three


(a)Optical Microscopy image of circuit edit to cut off net


n_5750; (b)PEM image; (c)Related schematic circuit diagram; (d)EOP waveforms image of reference and experimental


sample;


126


Figure 6: images of Experiment four


n_5740; (b)PEM image; (c)Related schematic circuit diagram; (d)EOP waveforms image of reference and experimental


Figure 7: images of Experiment five


SE_N0; (b)PEM image; (c)Related schematic circuit diagram; (d)EOP waveforms image at upstream and downstream


transistors on experimental sample;


127


Experiment 5: Input net of inverter open (Scan Enable  Path)


In the last experiment, one branch of scan enabled signal  SE_N0 was selected and cut off manually. The OM image of  circuit editing, the PEM image, the schematic of related circuit  and the EOP waveform were showed in Fig 7 (a) to (d) respectively. The result showed that the signal was correct at  upstream inverter A and downstream inverter B whose control  gate was good. But no signal can be captured at inverter C  whose control gate was floating by circuit-edit, included high  SNR signal, only PEM spot at Nmos C, which was same as  Experiment 4. In this experiment, it can be concluded that  there was still no high SNR signal at downstream transistors  which were directly controlled by floating net, although it was  a global signal and controlled a lot of inverters.


Among the simulation experiments above, the first two short  experiments are successful, and the conclusion meets our  suspicion, we can capture the high SNR signal at specific  transistor. However, the last three open experiments are failed. We don’t find high SNR signal at the transistor around the  defect. Based on this fact, the discussion below will be  separated to two parts: the first part will summarize the details  of successful experiments to conclude the characteristic for the  short failure, and the second part will introduce some other  suspicions from our point of view that can caused high SNR  signal on open failure mode.


1st part: High SNR signal on short failure


From the two experiments performed in the previous section, we can summarize the relationship between the location where  can capture high SNR signal and the failure mechanism into  two conditions respectively as below:


a) High SNR signal is found at Pmos whose drain is  connected to Vss, and source is Vdd.


b) High SNR signal is found at Nmos whose drain is  connected to Vdd, and source is Vss.


Figure 8: Two kinds of short failure model which induces high  SNR signal


Fig.8 shows the failure model of two conditions. A common  point can be concluded from this figure: the high SNR signal is  observed at the transistor whose drain and source are directly  connected to power and ground. Therefore, high Ids current  from power to ground exists all the time when the transistor is  on.


Besides, there are also three additional points of interest will  be addressed below:


Point 1: PEM spot


From the experiments above we can also summarize that there  should be the strong PEM signal at the transistor where high  SNR signal can be captured. This phenomenon can also be  explained by the mechanism above: since drain and source are  connected to power and ground respectively, the absolute  value of electrical potential difference from drain to source (Vds) is always equal to the voltage of power Vdd. In that  case, when the transistor is on, which means the electrical  potential difference from gate to source Vgs is greater than the  threshold voltage Vt. At this moment, the transistor is operated  at saturation region (Vgs>Vt, Vgs-Vds<Vt), which can emit a  lot of photons, then PEM spot was shone [3].


Point 2: overlaid weak clock signal


Another point of interest is the weak clock signal  superimposed on the high SNR signal. Ang [4] has performed  a lot of study about the origin of the clock signal which should  be from the substrate. However, the clock noise from substrate  should exist all the time, the reason why we cannot find it from  reference sample is the same as the one of high SNR signal: there exist a large Vds all the time, it will amplify the clock  noise and react on the EOP waveform when the transistor is  off, and the influence of clock noise will be ignored when  transistor is on.


Point 3: slow rising/falling edge of the signal


At last, we can also observe the EOP waveform with obvious  slow rising and falling edge at the other transistor whose drain  is also wrong (Pmos A in the first experiment, and Nmos A in  the second experiment).


Figure 9: The equivalent model of the transistor which induce  slow edge signal in experiment 1 and 2


128


Fig.7 shows the schematic of two kinds of failure model. It can  be easily realized that the drain and source are connected by  the defect, and the transistor is equivalent to a capacitor  between gate and drain/source. Therefore, a resistor-capacitor  low pass filter takes shape and the signal from gate will be  low-pass filtered.


Based on the three points above, the location of defect can be  isolated more precisely, more confidence will be given in  subsequent physical analysis, and cycle time will be declined.


2nd part: High SNR signal on open failure


In the last three experiments, we introduce three kinds of open  experiment, the defect was located at three positions which  included:


1. On the data path which controlled cell is an AND.


2. On the data path which controlled cell is an inverter.


3. On one branch of the scan enable path which controlled  several inverters.


These three experiments aim to confirm the relationship  between the occurrence condition of the high SNR signal and  the circuit location of open defect. However, no high SNR  signal can be found during all the three experiments. Based on  this fact, the occurrence condition of the high SNR signal has  nothing to do with the circuit location of the open failure.


To dig deeper into the causing of high SNR signal, we try to  conclude the differences between the real cases and simulated  experiment, some conclusions were summarized below:


Infrared Imaging [1, 2, 3] and fractography [4, 5] covers a  wide range of topics that is beyond the scope of this paper. The primary objective of this paper is to share cases that  combine two different techniques to successfully identify the  real failure mechanism and to provide valuable information for  root-cause investigation.


CASE 1


The first case is related to the successful identification on the  horizontal internal propagation of the crack which leads to  electrical shorting and it also helps to determine the possible  root-cause.  The failing unit is designed for automotive  applications.


The reported failure states an electrical short between two  pins.  However, the customer also mentioned that the previous  returned units are showing die cracks with and without  electrical overstress (EOS) damage [6].  C-mode Scanning


Acoustic Microscopy (CSAM) showed a delamination  between top die to molding compound interface.  Curve trace  analysis showed an electrical hard short between pins 48 and


49.


Figure 1: CSAM photo showing a delamination located at the  top side area of the die.  The name of the product, customer  and lot ID# were covered by grey color.


The failing unit was subjected to decapsulation.  Internal  optical die inspection did not show any signs of hardened  molding compound residue caused by excessive heating. Further Scanning Electron Microscope (SEM) showed crack  propagation from the sidewalls which extends from the bottom  to top die.


Figure 2: SEM photos showing cracks at the sidewalls.


Optical Beam Induced Resistance Change (OBIRCH) [6] using Seebeck Effect Imaging (SEI) showed a hot spot that  confirmed the location of the electrical short between pins 48  and 49.  Top die optical inspection at the location of the hot  spot showed no obvious anomalies.  Neither cracks nor  hardened molding compound caused by excessive heating was  observed.


Figure 3: A hot spot using SEI was observed on OUT2 driver.


Backside IR inspection after full decapsulation showed that the  crack propagated from the right top corner to left as evidenced  by Wallner lines.  The location of the hot spot lies at the area  of hackle marks where it finally occurs during final break-up  going to the top surface where it leads to an electrical short  between pins 48 and 49.  The rib marks also indicate the  direction of the crack propagation.


Figure 4: IR photos showing the fracture features.  Red  arrows showed the direction of the crack propagation.  Yellow  box showed the hot spot location, which lies at the area where  hackle marks can be found.


Figure 5: IR and SEM photos showing the location of the  internal secondary crack where the point of origin on the rib  marks was observed.


Based on the gathered results of fractography using Infrared  Microscopy and SEM inspections, it can be concluded that the  electrical short is just a consequence of the die crack. Simulation also showed that the cracked die is due to board  warpage. Knowing the fracture features helps to provide  information for the correct identification of possible rootcause.


CASE 2


The second case is related to a crack that has not yet been  completely propagated where the die is still intact.  The rootcause has been determined through successful identification of  the point of origin caused by a small chipout(s) from the  bottom. The product is designed for automotive applications.


This case consists of two failing units and these are:


 SN1: Partially cracked die where further analysis was  performed.


 SN2: The external subcontractor sent a die with  continuous crack where it was detected at their  assembly line.


Analysis on SN1


Extensive electrical characterization found the unit to be  passing at 25°C and 105°C but failing at -40°C during  initialization and alternate memory tests.  C-mode Scanning  Acoustic Microscopy (CSAM) did not show signs of  delamination.


141


Figure 6: A CSAM photo showing no signs of obvious  delamination.


Internal optical die inspection showed a crack near the TEST  pin, cutting through metal tracks including some parts of the  OTP (memory) block circuitry.   This crack could explain why  it fails during initialization and alternate memory tests at -40°C.


Figure 7: Optical photo showing a cracked die near TEST pin.


Further inspection showed that the crack is not fully  propagated and is confined at the circuitry near TEST pin.  SEM inspection showed no obvious tool mark from the side  walls and top die that could start the propagation of the crack.


Figure 8: Photo of the layout showing the discontinued crack.


Figure 9: SEM photo from the top die showing the location of  the discontinued crack.


142


Figure 10: Higher magnification of the crack.


The unit was successfully subjected to full decapsulation.  SEM inspection of the sidewalls and bottom die was  performed.  No signs of mouse bites nor chip-outs was  observed at the sidewalls.


Figure 11: SEM photo of the die backside showing the length  of the crack propagation to be 379.8 um.


Figure 12: SEM photos showing small markings or chipouts  along with crack. This information is not enough to conclude  that these are the cause of the crack.


Backside infrared inspection was performed.  The fractures are  difficult to determine due multiple layers that were reflected  back to the sensor. The result did not provide detailed info on  crack origin and propagation.


Figure 13: Backside IR photo showed that the crack  propagates vertically rather than horizontally (see Case 1).


To maximize the reflection of the infrared signal, the unit was  coated by epoxy and to be subjected for polishing where the  direction of the crack should be in parallel with the crack  propagation.


Figure 14: A graphic presentation on the direction of  polishing in parallel with the crack.


143


IR inspection after initial polishing already showed the origin  of the crack. The fractures are radiating outward from the  point of origin.


Figure 15: IR photo showing the origin of the crack and the  projected distance from the edge of the crack.


Further mechanical polishing was performed.  The fracture  lines such as mirror and twisted hackle lines became more  visible, confirming the point of origin and providing more  details of fracture lines and crack propagation.


Figure 16: IR photo after further polishing showing the point  of origin


Figure 17: Higher magnification IR photo showing more  details of the crack origin and fracture lines (mirror and  twisted hackle)


Analysis on SN2


After the die was received, optical inspection showed  continuous crack propagation starting from right to left.


Figure 18: Optical photos showing the continuous  propagation of the crack.  The red rectangle is the location of  the origin of the crack coming from the bottom.


The unit was mechanically separated to observe the internal  fractures.  SEM inspection showed the origin of the crack and  exhibited similar type of fracture as SN1.  However, additional  secondary cracks and chip outs were induced due to additional  stress caused by separation.


144


Figure 19: SEM photo at the origin of the crack.


Figure 20: SEM photo at higher magnification which  confirms the fractures from SN1.


With the basic understanding on how the infrared inspection  works, fractography and by thinking out of the box, the origin  of the crack has been successfully determined.


CASE 3


The third case is related to “which came first: chicken or  egg?”.   An electrically overstress damaged device [8] with  multiple die cracks is a dilemma during FA analysis and  fractography. With backside IR inspection, the internal  fractures will be visible as well as the substrate damages. For  the analysis of this case showed that the die crack is just a  consequence of the electrical damage.  The failing unit is  designed for automotive applications.


External optical die inspection showed missing/melted pins  and a blown package.  X-ray analysis showed fused bond  wires.


Figure 21: Optical photos showing the condition of the  package upon receipt.


Figure 22: X-ray photo showing fused bond wires and melted  pins.


Post-decapsulation optical die inspection showed multiple  fractures, hardened molding compound caused by excessive  current and melted/reflowed aluminum metallization.


145


Figure 23: Optical photo post-decapsulation.


This unit was further subjected to full decapsulation.  The  VBOOST supply line exhibited heavy electrical damage  compared to the other location.  This supply pin can reach up  to 60V and can deliver high amount of current in an  automotive application.


Figure 24: Optical photo post-full decapsulation.


Figure 25: Representative photos during SEM inspection  showed melted silicon as well as fractures.  The crack  propagated from the melted silicon from the bottom left photo.


The multiple cracked parts were subjected to backside-IR  inspection.  The results showed a heavily damaged VBOOST  bond pad which extends to the output driver.


Figure 26: Representative IR photos showing the electrical  damage from the VBOOST supply and melted silicon from the  bottom where cracks are propagated.


Backside IR imaging inspection of the electrical damage from  the VBOOST can be performed in combination with die  cracks reduces several steps such as detailed SEM inspection  for the identification of the external fractures and deprocessing  to check for the substrate damages that goes along with the  cracks.


The analyst should also be aware that the stress from the  package will be relieved during the course of decapsulation.


146


Internal fractures either due to electrical damage or mechanical  stress, would be difficult to analyze using the usual  fractography without inducing additional stress on the sample. With infrared microscopy, it reduce the additional stress as  well the generation of the secondary crack where the point of  origin will be difficult to analyze.


The author would like to acknowledge our global director  Mark Morris and our manager Pascal Vercruysse for the  support and encouragement. We would like to acknowledge  our Material Analysis (MA) team for their support especially  Peter Baert for the cross-sectioning and Ives Oliquiano for  providing a case.


[1] Burgraaf, P., IR Imaging: Microscopy and Thermography, Semiconductor International, pp. 58-65, July, 1986.


[2] Zissis, G. J., Infrared Technology Fundamentals, Optical  Engineering, Vol. 15, no. 6, pp. 484-497, 1976


[3] W.S. Lau, Infrared Characterization for Microelectronics, World Scientific Publishing Co. Pte. Ltd., 1999


[4] George Quinn, Fractography of Ceramics and Glasses, Forgotten Books, 2017.


[5] Derek Hull, Fractography: Observing, Measuring and  Interpreting Fracture Surface Topography, Cambridge


University Press, 1999.


[6] Alan Righter, Ed Wolfe, Jean-Jacques Hajjar, “Non-EOS  Root Causes of EOS-Like Damage” 36th Electrical


Overstress/Electrostatic


Discharge


Symposium


(EOS/ESD), 2014


[7] Kiyoshi Nikawa, Shoji Tozaki, "Optical Beam Induced  Resistivity Change", ISTFA1993 proceedings, pp. 303-


310, 1993.


[8] S. Voldman, Electrical Overstress (EOS): Devices  Circuits and Systems, Chichester, UK:John Wiley and


Sons, Ltd., 2013


147


Case Studies on Application of Electro Optical Probing (EOP) - A Noninvasive  Backside Localization Technique in Failure Analysis


Srinath Rajaram, Rajesh Kabadi, and Eric Barbian


Given the challenges FA Engineers have in fault localization, top-side analysis is facing a major challenge with today’s  advanced packaging and shrinking of die sizes. At wafer and  die level it is relatively easy to probe with little or no sample  preparation. Greater challenges occur after the die is packaged. The difficulty further lies in non-destructively analyzing the  die. Another issue with failure analysis is accurately  deprocessing the device for probe pad deposition. Techniques  like Electro Optical Probing (EOP) or Laser Voltage Probing (LVP) acquire electrical signals on transistors and create an  activity map of the circuitry. In failure analysis, it is applied to  localize defects. This paper discusses integrating EOP  techniques in traditional FA to localize failure in mixed signal  ICs. Three case studies were presented in this paper to  establish the technique to be effective, quick and easy to probe  non-invasively with minimal backside sample preparation.


With increasing metal layers and decreasing metal width, topside fault localization techniques are becoming a challenge in  Failure Analysis (FA) process, resulting in low success rate


[1], [2]. In addition, failure mode involving timing, clock race  conditions which may fail only at extreme test conditions [3], resistive interconnects [4], continuity detection [5] are quite  challenging. Today’s fault localization techniques rely heavily  on traditional Photo Emission Microscopy (PEM) [6] and  microprobing techniques. Non-invasive backside localization  techniques such as electro optical techniques are gaining  attention to optically analyze the electrical activity of devices


[7]–[9]. The general principle behind EOP is based on the  interaction of the laser beam with the device under test. Current systems typically use near infrared (NIR) 1319/1340  nm or 1064 nm lasers, which can be used to focus through  thinned and polished silicon backside of the device. A solid  immersion lens (SIL) which makes contact with the device  with thinned silicon can be used to increase the numerical  aperture (NA) of an optical system thereby giving better  resolution. When the laser beam is incident on the device, portion of the radiation that was transmitted through the bulk is  incident on the active areas of the devices and reflected off the  interfaces in the depth of focus and the intensity can be  detected with a photo detector to generate an image of the  device. The reflected radiation also consists of amplitude and


phase information if the device is active. More detailed  information on the signal generation process can be found in [10].


The most significant benefit of EOP is the accessibility of the  nodes with minimal sample preparation. For example, there is  no need of a probe pad and simple backside thinning is  sufficient. This makes EOP a much faster, non-destructive, contactless analysis technique. EOP is a very versatile  technique that has proven to be useful on many different  devices (analog devices [11], MOSFET’s [12], scan failures


[13]). In this paper, we evaluated better ways to analyze clock  skew delay, abnormal transistor switching and clock shootthrough by applying EOP for acquiring timing and fault  information.


Fig. 1. Abnormal NTSC output on Customer returned unit


148


Case Studies of Actual Customer Returns  Utilizing EOP


In the first case study, the failing image sensor unit was  returned from a customer due to abnormal NTSC output as  shown in Fig. 1. Automatic Test Pattern Generation (ATPG) diagnosis reported 14 internal faulty chains indicating error in  the clock tree. Additional chain diagnostic patterns were  created, but the diagnostic resolution was not improved. Diagnosis involving clock failures is more challenging task  due to the fact that multiple scan chain failures can be  confused by multiple independent defects on these scan chains.


Fig. 2. Backside PEM image with 0.8X Macro lens image


Fig. 3. (a) Layout analysis of PEM sites overlaid (b) Schematic inference


The returned unit was backside polished to expose the silicon. Photo Emission Microscopy (PEM) was performed while  looping the failing SCAN pattern at a clock rate of 10MHz. While compared to a Reference unit, three abnormal photo  emitting sites were detected on the customer returned unit as  shown in Fig. 2. Layout and schematic studies showed the  emissions were located on the clock buffers in a digital block  as shown in Fig. 3. EOP analysis was then performed while  running the scan pattern in an infinite loop at the scanning  clock frequency of 10MHz.


Fig. 4. EOP measurements made at Driver and SINK1  locations


Fig. 5. CAD layout with first suspect net from Fig. 3  highlighted


EOP waveform acquisition was taken on the clock buffers. On  the customer returned unit, measurements taken on one of the  clock buffers had abnormal waveform while other two sites  were normal. EOP waveforms were captured at the driver and  Sink1 in Fig. 4. Based on the EOP waveform analysis, layout  study indicated the Sink1 having the PEM site had abnormal  rising edges with 8.34ns delay creating a race condition. Sink1  was a clock buffer that was connected to the driver with the net  going up metal 3 to metal 4 as shown in Fig. 4. Further  analysis on the layout revealed possibility of any/all three  connections resistively connected as shown in Fig. 5. To  visualize the defect, Transmission Electron Microscopy (TEM) lamella was FIB-prepared on the first via2 location  closer to the Sink1 slave clock buffer. TEM imaging on the  lamella found anomalous interfacial layer at the bottom of the  via2 (see Fig. 6), which is the root cause of the abnormal  NTSC output and SCAN failure.


149


Fig. 6. Physical analysis conclusion showing anomalous  interfacial layer at bottom of via


In the second case study, a failing automotive image sensor  integrated circuit packaged in an iBGA63 package was  returned from a customer. The returned unit was noted to pass  all Stuck-at Scan test patterns and fail only transitional delay  fault scan patterns.


Using a bench top digital tester, a known good unit was noted  to pass all transitional delay patterns down to 0.8x TSF (TSF = Time Scaling Factor, 1 x TSF = 100nSec). The returned unit  was noted to fail at TSF <2.5x. ATPG diagnosis on the  original compressed transitional production patterns and also  on patterns created for iterative diagnosis did not yield  substantially better results and indicated too much  equivalency. The following was summary of observations  made through ATPG diagnosis.


ATPG Compressed Transition Delay: (2 failing patterns) 4  Defects, 159 possible candidates including equivalencies all  100% match ATPG Generated Uncompressed Transitional  Delay: (4 Failing patterns) 161 suspects, 6 at 100% match and  remaining at 90%. ATPG Iterative Diagnosis: (56 failing  patterns) 232 suspects, best match was only at 46%. Shmoo  studies were conducted by varying the Vdd over TSF. Vdd  supply was varied from 1.70V to 1.90V (y axis). TSF was  varied from 2.80x (slower clock speed) to 1.00x (faster clock  speed). As seen in the Shmoo plot (top) in Fig. 7, returned unit  fails at lower Vdd levels and faster clock speeds. The color  gradient indicates number of failed cycles. From the Shmoo  plot (bottom) in Fig. 7, it is evident that the returned unit starts  to pass at lower Vdd and higher clock speeds at elevated  temperatures.


Fig. 7. Shmoo results of Vdd vs Timing at (top) Room  temperature (bottom) 85C


Fig. 8. DALS analysis indicated a site at the location  indicated by white arrow


Fig. 9. DALS site overlaid on the CAD layout at location of  the arrow from Fig. 8


Dynamic Analysis by Laser Stimulation (DALS) was  conducted. A single DALS site was identified at the location  indicated by white arrow in Fig. 8. The highlighted net in Fig. 8 indicates the downstream logic from the driver cell. Study of  the CAD layout indicated that the DALS site was located at  via3 specified by the white arrow in Fig. 9. The location of the  driver cell is labelled. EOP waveforms were captured at the  driver and then at two locations, Sink1 and Sink2 as shown in  Fig. 10. Fig. 10 shows that Sink2 of the failed chip having  abnormal waveform. Sink1 was a logic cell that was prior to  via3 at the DALS site and Sink2 was a logic cell that was after  the DALS site in connectivity.


Transmission Electron Microscope (TEM) lamella was FIBprepared on the via3 that connects Sink1 and Sink2. TEM  imaging found it to be voided, which was the root cause of the  customer problem (see Fig. 11).


Fig. 10. EOP measurements made at Driver and SINK1 and  SINK2 locations


Fig. 11. Physical analysis conclusion showing voided via


Case 3


In the final case study, a failing automotive driver packaged in  Quad-Flat No-leads (QFN-32) was returned from customer  due to incorrect Integrated Circuit (IC) revision (see Fig. 12). A sequence of simple SPI commands to perform basic  functional testing was used and multiple fails were observed. Photo Emission Microscopy (PEM) was performed and no  differences were observed between a good unit and the failing  unit. The defect could not be localized because of timing  shoot-through failure. The device was prepared for backside  analysis by selectively removing the exposed pad of the  package as shown in Fig. 13.


Fig. 12. Incorrect SPI device revision on Customer returned  unit


151


Next, Electro-Optical Probing (EOP) was performed to isolate  the location of the failure. Analysis of the failing unit revealed  the fault is localized to the internal SPI output 16-bit shift  register as shown in Fig. 14. The data SRO 7 moves to the  SRO 8 and SRO 9 on one clock cycle. This indicates that the  flip flop outputting SRO 9 has a timing issue allowing the data  to shoot-through. The output of each flip-flop was probed, and  it was observed that the data from flop DFFPLD4 was  shooting through DFFPLD5.


Fig. 13. Optical image after backside milling of 5x5mm QFN32 package.


Fig. 14. EOP waveforms at the SPI shift register with a  continuous device revision command executed.


A delay of 6.5ns was observed on the clock driving DFFPLD5  as compared to the preceding shift register DFFPLD4. This  edge delay caused a race condition as the output data from  DFFPLD4 reached DFFPLD5 before it was clocked. EOP  analysis of the clock tree revealed an abnormal 6.5ns delay on  the clock to DFFPLD5. This delay was isolated to net PRE  CTS NET N304 as shown in Fig. 15. Based on EOP results, a  small segment of that net was suspected to have abnormally  high resistance. With layout analysis the failure was further  confirmed on net PRE CTS NET N304 as shown in Fig. 16.


Fig. 15. Partial schematic view of the clock tree driving flipflop DFFPLD5.


To visualize the defect, Focused Ion Beam (FIB) was utilized  to pull the small suspect net for Transmission Electron  Microscope (TEM) analysis. TEM analysis revealed an  abnormal via formation as shown in Fig. 17.


Fig. 16. CAD layout view of PRE CTS NET N304 net  corresponding to EOP data along the clock tree.


Fig. 17. Physical analysis conclusion showing voided via


152


The case studies presented in this paper, demonstrates the EOP  technique to be an effective, non-destructive localization  technique combined with traditional PEM and OBIRCH. EOP  could be easily implemented to check the activity of the  transistors in the suspect area with simple backside thinning  and not requiring to create FIB probe pads. With this  technique, the turnout time for fault localization of a  component/failing block could be significantly reduced. Furthermore, EOP analysis can be improved with a redesigned Evaluation Board with wider opening or with a  backside repackaging method for using the SIL.


The authors would like to acknowledge our global Product  Analysis Lab managers for the support and encouragement. The ON Semiconductor global failure analysis teams for the  invaluable contributions towards failure analysis capability  improvements. We would also like to thank our colleagues for  their interesting cases that we used in this paper to give actual  examples. We would like to acknowledge our Material  Analysis (MA) and Technology and Characterization Lab (TACL) teams for their support in the sample preparation and  material analysis of these cases. This paper is only a small  portion of the continued improvements that our teams are  continuously striving to increase our analytical capability.


[1] L. C. Wagner, “Failure analysis challenges,” in  Proceedings of the 2001 8th International Symposium on  the Physical and Failure Analysis of Integrated Circuits. IPFA 2001 (Cat. No.01TH8548), July 2001, pp. 36–41.


[2] C. Boit, “Can failure analysis keep pace with ic technology  development?” in Proceedings of the 1999 7th  International Symposium on the Physical and Failure  Analysis of Integrated Circuits (Cat. No.99TH8394), July  1999, pp. 9–14.


[3] C. Metra, S. Di Francescantonio, and T. M. Mak, “Implications of clock distribution faults and issues with  screening them during manufacturing testing,” IEEE  Transactions on Computers, vol. 53, no. 5, pp. 531–546, May 2004.


[4] E. Zschech, E. Langer, H.-J. Engelmann, and K. Dittmar, “Physical failure analysis in semiconductor industry—challenges of the copper interconnect process,” Materials  Science in Semiconductor Processing, vol. 5, no. 4, pp. 457 – 464, 2002, eMRS, symposium O. [Online]. Available:


http://www.sciencedirect.com/science/article/pii/S136980 0102001245


[5] Y. Yamada and H. Komoda, “A successful failure analysis  using front and backside fault localization techniques on a  deep sub-micron cmos device,” in INTERNATIONAL  SYMPOSIUM FOR TESTING AND FAILURE


ANALYSIS. ASM International; 1998, 2001, pp. 305–


312.


[6] J. C. H. Phang, D. S. H. Chan, S. L. Tan, W. B. Len, K. H. Yim, L. S. Koh, C. M. Chua, and L. J. Balk, “A review of  near infrared photon emission microscopy and  spectroscopy,” in Proceedings of the 12th International  Symposium on the Physical and Failure Analysis of  Integrated Circuits, 2005. IPFA 2005., June 2005, pp. 275–281.


[7] H. K. Heinrich, “Nonivasive optical probe for detecting  electrical signals in silicon integrated circuits,” Stanford  Univ., CA (USA), Tech. Rep., 1987.


[8] M. Bruce, G. Dabney, S. McBride, J. Mulig, V. Bruce, C. Bachand, S. Kasapi, and J. Block, “Waveform acquisition  from the backside of silicon using electro-optic probing,” in ISTFA 1999: 25th International Symposium for Testing  and Failure Analysis, 1999, pp. 19–25.


[9] M. Paniccia, T. Eiles, V. Rao, and W. M. Yee, “Novel  optical probing technique for flip chip packaged  microprocessors,” in Proceedings International Test  Conference 1998 (IEEE Cat. No. 98CH36270). IEEE, 1998, pp. 740– 747.


[10] U. Kindereit, “Fundamentals and future applications of  laser voltage probing,” in 2014 IEEE International  Reliability Physics Symposium. IEEE, 2014, pp. 3F–1.


[11] N. Jandee, D. Korbsrisawat, and F. Paulino, “Integrating  eop/eofm as a complimentary localization technique for  open via/contact,” in 2018 IEEE International Symposium  on the Physical and Failure Analysis of Integrated Circuits (IPFA), July 2018, pp. 1–4.


[12] C. He, H. Zhang, J. Song, P. Tian, and W. Wang, “Study  and application on thermal eop (electro optical probing) / eofm (electro optical frequency mapping) technique,” 2018 IEEE International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA), pp. 1–4,


2018.


[13] S. Jinrong, F. Diwei, G. Xue, and H. Chi, “High resistive  via localization using electro optical techniques,” in 2017  IEEE 24th International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA). IEEE, 2017, pp. 1–4.


153


1. The wafer technology is different: in the real cases, the  product is 40nm tech, and the experimental product in this  paper is 90nm tech. The different wafer technology leads  to different threshold voltage (Vt), which may cause  current flow from Vdd to Vss since the PMOS and NMOS  may open at the same time. The generation of high SNR  signal is similar to the one in short failure.


2. The defect model is different: in the real cases, the defect  was taken shape by copper migration or loss which  induced high resistance on suspected net. However, the  image Fig.2 (e) shown that there may be a short between  the suspected net and the net on the right hand. The short  may generate large current, then lead to high SNR signal. Since the copper migration, net open may occur on V3  which induced EBAC signal missing. While the defect in  the simulated experiment was made by circuit edit, which  is completely broken, and induced open in the electrical  characteristic.


Since the experiments on open failure are all failed, no definite  conclusion could be given, and further study is needed to find  out the root cause of the high SNR signal.


In this paper, two real cases with high SNR signal captured by  EOP are introduced. Based on our finding, two experiments  which simulated the short failure are carried out, and the  results meet the expectation. It can be concluded that the high  SNR signal can be found at the transistor which exist high Ids  current from power to ground. Besides, another three points,


the abnormal PEM spot, overlaid weak clock signal and slow  edge signal, are also discussed and explained separately. However, the other three experiments which try to find out the  occurrence condition of high SNR signal in open failure are  failed. No definite conclusion can be summarized in this paper, only some suspicions are listed, and further study is needed. According to the finding in this paper, it will be helpful for FA  to isolate the failure more precisely and understand the failure  mechanism more clearly.


[1] Yee W M, Paniccia M, Eiles T, et al. “Laser voltage  probe (LVP): A novel optical probing technology for flipchip packaged microprocessors,” Proceedings of the 1999  7th International Symposium on the Physical and Failure  Analysis of Integrated Circuits, Singapore, 1999, pp. 15-20.


[2] Soref R, Bennett B. “Electrooptical effects in silicon,” IEEE journal of quantum electronics, Vol. 23, No. 1 (1987), pp. 123-129.


[3] Li A, Xiao R, Guo M, et al. “Case Study on Abnormal  Electron-Optical Frequency Mapping phenomena in  Failure Analysis,” ISTFA 2018: Proceedings from the  44th International Symposium for Testing and Failure  Analysis, Pheonix, Arizona, November 2018, pp. 156-160.


[4] Boit C. “Fundamentals of photon emission (PEM) in  silicon-electroluminescence for analysis of electronic  circuit and device functionality,” Microelectronics  Failure Analysis, Ohio, 2004, pp. 356-368.


129


Artefacts of SEM/TEM observations cases on seal ring structure and correctives  samples preparations to avoid them


Christophe CHARLES, Alain MARGAIN


ST Microelectronics, 850 rue Jean Monnet, 38926, Crolles Cedex  christophe.charles@st.com


FIB/SEM and TEM are standard characterization techniques  for evaluation of process modification of microelectronics  samples. In this paper, artefacts from characterization  techniques are studied. The sample preparation methods are  optimized to avoid damages.


For microscopic analyses, electron/matter interaction can  locally alter the observed material. The impact of those  interactions may be negligible but they can also lead to false  interpretation of the data. During failure analysis of  microelectronics devices, it is critical to differentiate sample  preparation artefacts from true process defect. The  interpretation of degraded samples is always complex. It  requires to differentiate damages related to the full analysis  flow from degradations occurring during manufacturing or  qualification phases.


Materials: seal ring structures


In this study, seal-ring structures are chosen as an example to  show artefacts and difficulties in SEM and TEM observations.  These structures are made of Cu layers stacks (Figure 1) on  the edge of a die, acting as a protecting wall from external  threats like mechanical constraints during wafer sawing and  from moisture infiltration.


The size of such a structure is much more important compared  to typical devices size, leading in some difficulties in sample  preparation and observation. In addition, as for advanced  technology nodes, dielectric layers are made of porous low-k  materials. In seal-rings case, there are a coexistence of hard  materials with large size such as copper with soft and small  materials like low-k materials. This coexistence complicates  sample preparation.


Two cases of artefacts will be studied here: one with TEM  sample preparation followed by TEM imaging, and the other  one with SEM observations after FIB cross-sectioning.


Figure 1 – Schematic of Seal-ring structure and SEM crosssection picture of it


Case studies


1. TEM sample preparation


In the first case, we investigate electronic chips that failed  during stress tests (cycles of temperature, pressure, high level  of moisture, etc.). The fail was due to corrosion of metal  layers inside die. Thus seal ring did not work as expected. Following this results, several TEM analysis have been  carried out to determine seal-ring morphology (height, space, thickness) and validate process parameters, allowing to fix  this reliability issue.


Degradation of the low-k dielectric layer (delamination) has  been identified several times (Figure 2), but not  systematically. Doubt appeared to know if those damages  were artefacts of observation or were defects happening  during production process of device.


Indeed, electron beam can break Si-CH3 bonds in porous lowk dielectric, replacing it with Si-H and Si-O (CH3 desorb),


# Artefacts of SEM/TEM observations cases on seal ring structure and correctives samples preparations to avoid them


and making layer to shrink. Rapidly, TEM analysts have  noticed that those delaminations appeared when magnifying  the image. The first images, acquired at low magnification, have shown no damage.


Owing to further investigation between sites with or without  delamination, thickness of TEM lamellae appear as a  discriminator factor of this phenomenon.


Figure 2 – TEM observations, with voids (left) and without (right)


Then a hypothesis has been developed to explain how low-k  dielectric was damaged [1] [2]. As lamella thickness increases, interactions between electron beam and low-k dielectric  increase too. When thickness becomes more important than  the mean free path (of low-k dielectric), more interactions  between sample and beam occurs, resulting in the shrinkage of  the sample, and thus inducing voids/delaminations.


After the mechanism of the artefact was understood, several  ways of preventing the effect can be considered: 1. Operating  TEM at a low e-beam current to minimize interaction between  electron and the sample materials [3]. 2. Decreasing TEM  lamellae thickness to reduce the interaction of e-beam with the  sample. In this paper, we will focus on TEM lamella  preparation methods.


Thinner TEM lamellae have been tested, but only a low  success rate has been achieved with standard methods due to  the large size of seal rings and inhomogeneity of material  density. Different approaches of sample preparation have been  evaluated depending on the area of analysis.


Several difficulties exist when preparing thin TEM lamella on  seal ring structures:


1. Bending of lamella for wide and tall area.


2. Inhomogeneous thickness.


3. Pit and sometimes warping in lighter material


To avoid bending of wide and tall TEM lamella during  thinning, a prop (a small not thinned area) was made to  mechanically strengthen the lamella, as shown in Figure 3. By  surrounding the thinner area of interest with the prop, the  problem of bending was reduced. In seal ring cases, structures  are often divided in two parts, so a prop can easily be made  between those two parts.


Figure 3 – Prop on TEM lamella (STEM view on top and  tilted FIB view on bottom)


Against inhomogeneous thickness, using a wide range of tilt  angle during thinning, a pretty thin TEM lamella can be  obtained (Figure 4).


Two drawbacks of thin lamella are the risk to get some pit or  warping. In order to limit the phenomenon, a part of the  lamella is “sacrificed” depending on analysis objective. By  adapting tilt and rotation angle of FIB beam, one part of seal  ring is really thin while other part stays a little thicker, so for  each level there are at least one area that is thin enough to get  rid of artefact from the picture at higher magnification.


Figure 4 – TEM observation of Sealring lamella thinned with  a wide range of tilt angle.


There is not a single method to perfectly realize thin TEM  lamella in seal ring. To avoid defect artefact, a thin lamella is  necessary, but to obtain it some concessions may be required. Sometimes observation is only required at a very specific  location and thus thinning can be focused on bottom part of  TEM lamella only. On every analysis, choice between each  technique has to be done wisely by taking into consideration  analysis objective versus what can be achieved during  preparation.


2. Broken Contacts


131


In the second case, during robustness qualification test, a part  has been dismissed. Then failure analysis techniques have led  to FIB/SEM investigation of a located area on chip. SEM  imaging after FIB cross-section suggested a process issue: a  broken interconnection between active area and 1st level of  metallic line (call “contact” thereafter) has been found (Figure  5).


Figure 5 – SEM observation of a broken contact


The analyzed device presented redundant contact plugs. Consequently, broken contacts could be present at several  locations/wafer but not detected electrically. This posts a  potential reliability risk. Therefore, several samples with  distinct stress tests and manufacturing process variation were  analyzed. FIB cross-section and SEM imaging techniques  have been used. Broken contacts were found on some samples  but not all.


More such broken contacts should have been found on wafers  gone through stress tests than on wafers with no test. But no  such a correlation with test conditions was observed. Therefore we assumed that it was induced by  preparation/observation. In that case, the nature of damages  looks like a plausible real defect and requires more analysis to  conclude.


To get more data, several other sites were studies with FIB  cross-section and TEM. Three mechanisms have been  identified (Figure 6): one with delamination on top of contact, another one on bottom and the third one with broken contact.


Figure 6 – Three mechanisms identified


Delamination between contact and another layer due to SEM  observation has already been displayed previously and  identified as artefacts several times. But it was first time a  broken contact has been identified.


Figure 7 – TEM picture of broken contacts


TEM image of the contact showed that the crack happened  always on the top interface of the nitride layer (Figure 7). TEM lamella of broken contact have been done after a SEM  analysis. But if TEM sample preparation was performed  without previous SEM analysis, no crack was evidenced. From this, we concluded that not only the sample preparation, but also with or without the SEM observation both have  impact on presence of broken contact.


Analysis of the region around broken contact shows that there  is no metallic layer on top of it (Figure 8), only silicon nitride  and low-k layers. On other areas, there are always some  metallic layers.


Figure 8 – SEM picture of area of broken contacts


Consequently, the main hypothesis is that SEM damage (shrinkage) on large low-k regions generates a big strain on  contacts, which can cause a higher probability of broken  contact. But why did contact broke in middle and not at  interface like it usually does? Technology of studied device  has a higher height/width ratio on contact than on other, meaning mechanically weaker contact. And cracks always  happen slightly on top nitride, thus different interfaces  between contact with nitride and oxide layer could explain  localization of crack.


Several trials have been performed to reproduce defect:


- A test structure with similar environment has been  chosen: between 2 pads, a chain consisting of metal  lines connected to active silicon through contact with


132


only dielectric on top of it. It has been characterized  electrically before and after 20 kV electron beam  exposure from above (Figure 9).  A variation of  around + 1700Ω has been observed, proving damage  due to electron beam on this sort of structure.


Figure 9 – SEM impact on electrical characteristics


- On structure of interest, a cross-section area has been  scanned a long time with SEM beam. Thus another  cross-section at 90° from first one has been  performed to observed impact (Figure 10-a). Deformation of structure and delamination between  contact and silicon has been exhibited. On structure  with metal layer on top (Figure 10-b), damages due  to electron beam observation has been localized at  metal layer level instead of contact level.


Figure 10 – SEM impact on cross-section


Now that defect has been proven as an artefact and knowing  its origin, a methodology to observe this structure without  creating artefact has been developed. Several constraints have  to be taken account:


- Analysis must be done on full wafer (wafer can’t be  cleaved)


- Limited equipment time required (lower is better)


- Robustness and repeatability (“industrial” solution) On TEM lamella done without prior SEM observation, no  artefact has been shown, so this technique could be considered  as standard protocol but it required a long time and if too


much SEM observation was done during TEM lamella  preparation artefact may appear.


Deprocessing by polishing of top layer would be a quick and  robust method but it required a cleaved wafer.


Chosen method was to start as a standard SEM analysis, a  rough FIB milling to open SEM field view near area of  interest (FIB perpendicular to sample). Then removing part of  top layer with a cleaning cross-section at FIB 52° to sample (Figure 11). And thus finish cross-section normally. This  method adds only a few minutes of FIB milling, it does not  require to cleave the wafer (done on Helios1200 from  Thermofisher with a 300mm stage) and it is repeatable in  Dual-Beam.


Figure 11 – SEM on perpendicular to cross-section analysis


This method has been tried several times on such samples  with no damage identified on contact (Figure 12).


Figure 12 – No damaged/artefact on contacts


SEM and TEM analysis can lead to artefact during  observations due to electron-matter interactions.


Identification of artefact require careful analysis, by  combining different source of data, elaborating and validating  theory. Depending on the type of materials, new process and  technology may have different artifacts due to the new  materials used, presenting new challenges.


In this paper, two cases have been examined.


In a first case, thickness of TEM lamellae has been evidenced  as a key factor for delamination between layers under beam. Some methods are pointed out to avoid damages during


133


sample preparation. First of all, these methods have been  adjusted to seal-ring structures.


In a second case, we observed that electron beam lead to a  shrink of oxide layers which induced the break of underlying  contacts. Ion beam cross-section at zero tilt allows to remove  irrelevant layer in a few minutes.


[1] R.F. Egerton, P. Li, M. Malac, « Radiation damage in the  TEM and SEM », Micron 35 (2004) 399–409


[2] F. Lorut, et al., “Ultra low-K shrinkage behavior when  under electron beam in a scanning electron microscope”, JOURNAL OF APPLIED PHYSICS 114, 084508 (2013)


[3] Liu Binghai, et al., « TEM/FIB Technical Solutions to  Electron Beam Induced Radiation Damage to Low  K/Ultra Low K Dielectrics in Semiconductor Failure  Analysis » ISTFA 2012, pp542-547


134


Re-Packaging Solution of Bare Dice From Customer Packages To  Open-Cavity Ceramic Packages


Raymond G. Mendaros, Bernardino D. Mazon, Eugene Capito


Global Failure Analysis


Analog Devices General Trias (ADGT)


Gateway Business Park, Brgy. Javalera, Gen. Trias, Cavite, Philippines 4107


raymond.mendaros@anFalog.com, Bernardino.Mazon@analog.com, Eugene.Capito@analog.com


Romeo S. Soriano Jr.


Worldwide Manufacturing


Gateway Business Park, Brgy. Javalera, Gen. Trias, Cavite, Philippines 4107  romeo.soriano@analog.com


The advent of bare die form in the semiconductor industry  driven by the high-performance multichip modules’ (MCM) requirement posed electrical access and testing challenges on  customer returned units (CRUs) for failure analysis (FA). In  this technical literature, the developed die extraction  processes and re-packaging solution on molded MCM and  flex package types were discussed.


1.0 INTRODUCTION


Bare die solutions, commonly termed as known good die (KGD), driven by the high-performance multichip modules’ (MCM) requirement, posed electrical access and testing challenges on customer returned parts for FA. MCMs were envisioned as a technology for incorporating large, highspeed die on an interconnecting substrate1. A bare die product is simply a package-free semiconductor and allows the system designer to use the full potential of the bare die form without incurring the penalties such as degraded electrical performance or temperature limitations that can result from using the product in a standard package format. Bare die products allow more efficient use of limited space. Bare die benefits are improved electrical efficiency, reduced space volume envelope, ruggedization, thermal uprating and higher integration2.


Customers integrate KGD or Bare die with other devices to  come up with a customized product for certain applications. The devices are mounted on MCMs, flex printed circuit  boards (PCBs), molded packages or other packaging  solutions. To support customers’ FA requirements for KGD  or bare die failures, die extraction processes and re-packaging  solution need to be established to facilitate electrical testing  and fault isolation analysis.


The established die extraction processes and re-packaging  solution by Analog Devices General Trias’ (ADGT) FA team  were discussed in this technical document including the  successful implementation on 222-Bumped dice in flex  package and wire bonded bare dice in MCM. The 222-Bumped dice, wherein not all of the pins were utilized, were  re-packaged into 208L Ceramic Quad Flat Pack (CQFP) package while the bare dice were re-packaged into a 28L  Ceramic surface-mounted integrated circuit (SOIC) package  using a gold wire bonder.


2.0 REVIEW OF RELATED WORK


There are various products that are processed as KGDs or  Bare dice in Analog Devices Inc. (ADI). As an after-sales  support, FA capability was established. Re-packaging the  dice was the most viable option to have electrical access after  the dice were extracted from the package. Micro-probing is  another option but was set aside due to the high pin count  requirement for most of the products. One critical step in the  re-packaging solution was the wire re-bonding process. Existing bonder capabilities in the ADGT Hermetic line and  local subcontractors were considered. Machine capabilities  and turn-around time were assessed. Results of the  assessments showed that the purchase of a gold wire bonder  was most viable option.


3.0 METHODOLOGY


3.1 Materials:


35 samples of 222-Bumped dice, 35 samples of CQFP, 15  samples of bare dice in MCMs, 15 samples of 28L ceramic  SOIC, Nitric Acid, Die attach material and gold wires


# Re-Packaging Solution of Bare Dice From Customer Packages To Open-Cavity Ceramic Packages


135


3.2 Equipment:


Hotplate, gold wire bonder, optical microscope, scanning  electron microscope (SEM), wire pull and ball shearing  machines


3.3 Procedure:


3.3.1 Purchase of a New Wire Bonder


A gold wire automated bonder was purchased.


3.3.2 Die extraction evaluations from flex and MCM


3.3.3 Re-packaging of the Extracted Dice into Ceramic


Packages


Two die extraction processes, chemical and mechanical  techniques, were evaluated.


3.3.4 Application


Analysis of actual rejects.


4.0 RESULTS AND DISCUSSION


4.1 Wire Bonder and bonding accessories’ purchase and


installation.


The assessment of the machine capabilities and support was  conducted to determine the most viable option for the repackaging process. The current capabilities at ADGT  Hermetic line and a subcontractor were assessed. Results of  the assessments were as follows:


4.1.1 ADGT Hermetic Line Gold Wire Bonder


4.1.1.1 Existing capability was 1.3 mil gold ball bonding. This capability was not suitable for the 50umx50um  gold (Au) bump and pitch of 80um of the bond pads  for the 222-Bumped die.


4.1.1.2 Wire length capability is 6.35 mm maximum.


4.1.1.3 No chuck for 208L CQFP


Findings: Not capable of processing the 208L CQFP


4.1.2 ADGT Hermetic Line Wedge Bonder


4.1.2.1 Existing capabilities were 1.25 mil and 1.0 mil  Aluminum wedge bonding.


4.1.2.2 Wedge bond was not suitable for the 50umx50um Au  bump and pitch of 80um of the bond pads for the 222-Bumped die.


4.1.2.3 Bond layout which had angled bond position would  result in wire shorting.


4.1.2.4 No existing chuck for 208L CQFP


4.1.2.5 No existing process for gold wedge bonding


4.1.2.6 Machine is not capable for ball bonding


4.1.3 Subcontractor Gold Wire Bonder


4.1.3.1 Bonding temperature capability was 220 degrees  Celsius, however the requirement is 120C.


4.1.3.2 Wire length/span was 185mils max. Requirement has  a maximum wire length of about 275mils (7mm).


4.1.3.3 Long Cycle Time requirement of 14days


4.1.3.4 Intellectual Property (IP) concerns since the assembly  of ADI parts are not confined to this subcontractor


Findings: Not capable of processing the 208L CQFP. It also  exposes ADI to IP-related issues.


4.1.4 Purchase of a New Wire Bonder


The most viable option was to purchase a new wire bonder. The bonder that was purchased has the following major  capabilities:


4.1.4.1 Long wire span = 7.6mm max at 1 mil wire diameter


4.1.4.2 Small pitch = 35um min


4.1.4.3 Small wire diameter: 0.6mil at 3mm maximum wire  length


4.1.4.4 Capable for Ball Stitch on Ball (BSOB).


4.1.4.5 Suitable for high pin count devices


4.2 Die Extraction Process


The die extraction processes were dependent on the  customers’ packaging forms. For dice in MCM (molded  package), the samples were subjected to mechanical parallel  lapping from the top of the package until the ball bonds were  exposed. This was followed by chemical decapsulation to  extract the dice. Prior the re-bonding process, the dice were  subjected to plasma cleaning to remove any contaminants or  residues. See Figures 1 and 2 for representative photos of a  mechanically polished ball bonds and re-bonded ball bond.


Figure 1. Optical photo of  polished ball bonds


Figure 2. Representative  photo of a re-balled ball bond


136


For dice in flex PCBs, they were extracted by submerging to  acid etchants followed by a water cleaning step. Process flow  was illustrated in Fig. 3. This was the process used for the  extraction of the 222-Bumped dice from the flex board.


Figure. 3. Extraction process for dice mounted to flex  boards


4.3 Application: Re-packaging of the Extracted Dice into


Ceramic Packages


The extracted dice discussed in section 4.2 were re-packaged  into standard ceramic packages using the established repackaging capability. The bare dice from MCM were repackaged in 28L Ceramic SOIC while the 222-Bumped dice  from flex board were re-packaged in 208L CQFP. Not all  bond pads of the 222-bumped die were needed; thus, 208L  CQFP was sufficient. Refer to figure 4 for photo of a repackaged bare die while representative photos of a repackaged 222-bumped die including wedge bonds, wire pull, ball shear and crater tests results were shown in Figures 5-9. The re-packaging results were successful and the gathered  mechanical tests (wire pull and ball shear) readings were  within acceptable range. No pad cracking was uncovered  from the crater test analysis.


Figure 4. Optical photo of the re-packaged bare die


Figure 5. Optical photo of the re-packaged 222-bumped die.


Figure 6. Zoomed-in SEM photo on representative wedge  bonds


Figure 7. Wire pull data


Figure 8. Ball shear data


137


Figure 9. Optical and SEM photos of a representative bond  pad after crater tests


4.4 Re-packaging Applications on Actual Reject Samples


More than 20 reject samples from different devices were  successfully re-packaged in various ceramic packages after  the established re-packaging capability and process was  deployed. All the needed electrical testing and failure  analysis techniques were successfully performed on these  parts.


Two of the reject units, marked as SN1 and SN2, were  UltraSonic Oil Level Sensor devices. The devices were  extracted from MCM and re-packaged in 28L ceramic  packages. Automatic test equipment (ATE) testing using the  FA test program for re-packaged parts showed that the units  were valid functionality failures. The failing parameter was  verified on a bench set-up. Light Emission Microscopy (LEM) analysis using the failing functionality parameter as  stimulus showed an absence of and faint emissions in SN1  and SN2, respectively. Scanning Electron Microscope (SEM) inspection post chemical deprocessing revealed silicon  damage sites on transistors due to an electro-static discharge (ESD) event on both parts associated with the anomalous (absence and weak) photon emissions. See Figures 10-14 for  the LEM and silicon damage photos.


Figure 10. Reject with  missing photon emissions


Figure 11. Good unit showing  the normal photon emissions


Figure12. SEM photo showing a substrate damage


Figure 13. SN2 showed faint photon emissions as compared  to a known good unit


Figure 14. SEM photo showed contact spiking/gate damage  on an NMOS transistor in SN2


5.0 CONCLUSION


The established die extraction and re-packaging processes  were confirmed to be successful. The availability of the  capability and process in ADGT ensured the after-sales FA  support for die sales or KGD customer returns requiring FA.


138


6.0 RECOMMENDATIONS


Establish re-packaging capability for devices with pin  counts greater than 208 pins.


7.0 ACKNOWLEDGMENT


The authors would like to acknowledge the contributions and  support of the following personnel:


7.1. Global Failure Analysis: Cindy Cabezas, Ronel  Dipalac, Eugene Capito, Ellen Andal, Mitch  Pagkatipunan and FA Support Team


7.2. Assembly Engineering: Melanie Baligod, Polly  Policarpio, Paulino Tumala, Emmie Vasquez, Edmar  Cocjin and Noel Roxas


7.3. Material Management: Emma Estioco


7.4. Customer Service: Irene Ontog


7.5. IS Manufacturing Systems: Sheila Catacutan and  Evelyn Tolentino


7.6. Finance/Accounting: Agnes Felix


8.0 REFERENCES


[1] ScienceDirect, ‘Multichip Modules”,


https://www.sciencedirect.com/topics/engineering/multi chip-modules


[2] Empower custom designs and enhance applications,


Micross components, http://www.micross.com/siliconics-ad.aspx


139


A Novel Approach on Fractography through Infrared Microscopy


Allan Norico and Rommel Estores


ON Semiconductor Belgium BVBA


Some of the most challenging task in analyzing fractures is a  die that has not been fully cracked apart and a cracked die with  electrical overstress damage. Traditional tools such as simple  magnifying lens, optical microscope and up to the advance  Scanning Electron Microscope are not enough to study the  internal fractures or markings that could lead back to the origin  of the crack.  In order to study these internal fractures, the  analyst tends to break the sample into pieces. However, this  method creates additional mechanical stress and leads to a  secondary crack where the point of origin will be difficult to  analyze.


This paper aims to introduce infrared microscopy in  fractography (mainly on silicon) using cases and techniques to  minimize the occurrence of secondary crack in analyzing  internal fractures.


Which came first: crack or electrical overstress damage? How  can I effectively perform a fractography on a partially or noncompletely cracked die while trying to preserve the existing  fractures? These are some of the most challenging questions  that will be encountered by the analyst.


# Understanding Water Ingress in Scanning Acoustic Microscopy and a Method to Observe Defects that are Open to the Surface


Understanding Water Ingress in Scanning Acoustic Microscopy  and a Method to Observe Defects that are Open to the Surface


Adam Benak, Acoustic Microscopy Analyst and Roger Devaney, Lab Director


Hi-Rel Laboratories, Spokane, Washington


Scanning Acoustic Microscopy (SAM) is a very important  tool in the evaluation of molded plastic electronic components.  SAM is used to non-destructively determine the configuration  and quality of components using ultrasonic sound waves and  consequently is an important test step in the screening, Destructive Physical Analysis (DPA) or Failure Analysis (FA) of plastic components.  SAM is performed in a water bath so if  internal defects are open to the surface of the device they can  fill with water and become invisible to SAM.


In SAM an ultrasonic transducer is placed over the sample in a  water bath which acts as the medium for the sound waves to  travel.  The transducer sends a signal into the sample and the  return (or reflected) signal is then displayed on a monitor as  A-Scan data and a C-Scan image, see figure 1. The A-Scan displays the returning sound signal amplitude versus time,which equates to depth within the sample. The C-Scan is the confocal image created by the scanning acoustic microscope.


Each material transition, such as the molded plastic to die surface interface within the sample, is visible as a change in the scan amplitude due to the differing acoustic impedance of each.  The presence of an air gap (delamination) of any thickness may change the phase of the received wave and it may stop the acoustic signal from penetrating any deeper.


Figure 1.  C_SCAN image on left with A-scans for the three  primary areas on interest on the right.


The SAM allows us to select or “gate” a portion of the A-scan  that pertains to features of interest at a certain depth, and then  scan the transducer over the part creating an image with the  gated acoustic signal (fig.1).  This allows us to image features


154


such as the molded plastic to die interface, the die attach, and  the plastic to lead frame or die paddle interfaces.


Most of the defects that SAM is used to detect in Plastic  Encapsulated Microcircuit (PEM) devices are basically  pockets of air at an interface that is internal to the device.  The  phenomenon we are concerned with in this paper occurs when  there is a defect that breaks the device surface which allows  water to fill it.  Because SAM is performed in a water bath, if  there are fine separations, cracks, delaminations or voids  within the sample that are open to the surface, water can seep  into them and displace the air at those locations. The  displacement of air by water in these locations is called water  ingress.  Due to the surface tension of the deionized water, the  complete exchange of water and air is usually not immediate. If a sample is scanned immediately upon being placed in the  water these delaminations are often visible with SAM since it  takes time for the water to seep into them (fig. 2).  As the  water continues to seep into these delaminations they begin to  become invisible to SAM because the water conducts the  sound waves through them (fig.3).


Figure 2.  SAM image immediately after placing sample in  water showing delaminations (red/yellow areas) over the lead  frame.


Figure 3.  SAM image of sample from figure 2 after several  minutes in the water showing how indications have diminished  and changed over time.


It is common practice that SAM examinations are performed  on trays containing many samples that are all placed in the  water bath at the same time and may spend minutes to hours  there before the examination. If there are any surface breaking  cracks or delaminations present, water ingress may prevent  them from being detected making a bad sample appear to be  good.


We have documented water ingress on many hundreds of  samples and have confirmed the presence of these  delaminations that are open to the surface by cross sectioning  using an UltraViolet (UV) dye filled epoxy mounting medium.  This paper will present several case studies that clearly  illustrate the phenomenon of water ingress and the proper  procedures to prevent it from masking defective samples.


Case Study #1:  16 pin SOIC


Six pieces of this device were submitted for DPA, of which  SAM is a required step in the non-destructive portion of the  testing per Mil-Std 1580B w/Change 3, Requirement 16.5.1.3.


[1]  SAM used in combination with radiographic examination  gives an excellent understanding of the device configuration  and quality which are especially important before proceeding  with further destructive testing (fig. 4-6).


Figure 4.  External view of device


Figure 5.  Radiographic top view of device


Figure 6.  Radiographic side view of device


155


Figure 7.  SAM view of die/lead frame/paddle, circuit side, immediately after being placed in the water bath; note  indications over the lead frame.


Figure 8.  Same view as above after 15 minutes in the water  showing decrease in anomalous indications over the lead  frame due to water ingress.


The SAM images in Figures 7-8 show a marked decrease in  the anomalous indications (delaminations of the molded  plastic from the metal lead frame) after extended time in the  water bath.  This is caused by water seeping into these  delaminations, which indicates that they are open to the  surface of the device.  This is proven by cross sectioning of  the sample after infusing it with UV dyed resin in accordance  with Mil-Std 883K, Method 1034.2. [2]


All of the SAM images shown in this paper are generated  using an asymmetrical color map for maximum contrast  because gray scale images are more difficult to discern the  often subtle changes due to water ingress.


Figure 9.  Cross section view of device from figure 8 under  UV illumination showing dyed epoxy ingress along open  delaminations around the lead frame, bonding pad and die  attach.


Figure 10.  Cross section view of the device showing dyed  resin around the lead and the wire bond at the die surface.  This proves the delaminations observed at SAM and  subsequently masked by water ingress were open to the  exterior of the device.


The photos in Figures 9-10 illustrate how the UV dyed epoxy  penetrated in to the delaminations that were observed in the  original SAM image, and in this case traveled along the bond  wire all the way to the die surface.  This proves conclusively  that these delaminations are both real and open to the surface  of the device.  This has become the standard protocol in DPA  of plastic devices when delaminations, and especially water  ingress, are observed at SAM examination.


156


Case Study #2:  8 pin QFN


Figure 11.  Front and backside view of QFN device; note  cracks.


Figure 12.  SAM view of die/lead frame/paddle immediately  after being placed in the water bath with large indications.


Figure 13.  Same view as above after 15+ minutes in the  water showing decrease in anomalous indications over the die  paddle due to water ingress.


157


Five pieces of this device with an exposed die paddle were  received for DPA.  This package style can have problems with  adhesion of the molded plastic case to the exposed die paddle  and leads since it is relying strictly on the chemical adhesion  of the plastic to the metal components.  Visible cracks in the  molded plastic case can sometimes be observed as with this  device (Fig. 11).  The initial SAM view (fig.12) observed  significant delamination at the die paddle which was greatly  masked by water ingress (fig.13).  Subsequent dye penetrant  cross sectioning confirmed the anomalous conditions, please  refer to figures 14-16.


Figure 14.  Cross section view of the device from figure 13  under UV illumination showing the dyed resin penetrating in  to the device along the die paddle.


Figure 15.  Higher power view from figure 14 showing dye in  delamination which is open to the device surface.


Figure 16.  Bright field view of sample from figure 15 showing  damage to the die attach and die as a result of the  delamination.


Case Study #3:  64 pin QFP


Five pieces of this common device type were received for  DPA (fig.17).  This package style is normally pretty robust, but depending on the die size and internal configuration, can  be prone to delamination.


Figure 17.  External view of 64 pin QFP device.


Radiography was performed to verify the internal  configuration of the device (fig 18).   The initial SAM image  indicated delamination of the tie bar and leads (fig. 19) which  had been masked by water ingress upon subsequent  examination (fig. 20).


Dye penetrant cross sectioning was performed on the SAM  sample and confirmed that the lead and tie bar delaminations  were open to the device surface, refer to figures 21-22.


Figure 18.  Top view radiograph of device.


Figure 19.  SAM view of die/lead frame/paddle, circuit side  immediately after being placed in the water bath with large  indications (red arrows).


Figure 20. Same view as above after 15+ minutes in the water  showing decrease in anomalous indications over the leads and  tie bar due to water ingress.


158


Figure 21.  Cross section views of device showing dyed epoxy  penetrating into the device along the lead.


Figure 22.  Higher power view of device showing dyed epoxy  penetrating along the tie bar/paddle to the die.


How to avoid water ingress masking defects


The best nondestructive technique to avoid masking defects  due to water ingress is to have a setup sample available that is  identical to your test samples.  This sample is then used to set  up the SAM machine with the proper gating for your desired  image, whether a circuit side view of the die/lead  frame/paddle, or a backside view of the paddle/lead frame.  The test sample is then placed in the water bath and  immediately scanned with the saved settings from the setup  sample.  Only one sample at a time is placed in the bath so that  each can be scanned immediately.  Follow up scans can then  per performed later after the samples have been in the water  for 15+ minutes to determine if water ingress has occurred.


If no setup samples are available then the actual test sample  must be used to set up the machine.  If water ingress is  suspected, then the sample may be removed and subjected to  vacuum baking at 110 degrees Celsius for 4+ hours to ensure


159


that any moisture that has ingressed into the device is  removed.  The sample is then rescanned in the SAM  immediately upon placing it in the water bath, using the  previously determined settings.


If water ingress is suspected and time is a factor then the  sample can be removed from the water bath after the initial  scan and briefly immersed in Isopropyl Alcohol (IPA).  IPA  will ingress into any open delaminations much faster than  water.  The sample is then placed back into the water bath and   rescanned.


This paper has discussed the phenomenon of water ingress  into delaminations within molded plastic devices that are open  to the surface in the performance of Scanning Acoustic  Microscopy (SAM).  Several case studies have been presented  to clearly illustrate what water ingress looks like and how it  can be proven by the use of UV-dyed epoxy and  metallographic cross sectioning.


Several techniques on how to avoid the masking of defects  due to water ingress without damaging or changing the sample  have been presented, including the use of setup samples or  vacuum baking.  A technique for accelerating water ingress by  using isopropyl alcohol was also discussed.


If water ingress is suspected on parts being examined, it would  be recommended to only place one sample in the water bath at  a time.


[1]  Military Standard 1580B w/Change 3, Requirement


16.5.1.3


Military Standard 883K, Method 1034.2


Dynamic photon emission on FinFET devices through novel scan test  approaches


1. Advanced Micro Devices, Singapore; 2. Singapore University of Technology and Design, Singapore


Dynamic Photon Emission Microscopy (D-PEM) is an  established technique for isolating short and open failures, where photons emitted by transistors are collected by sensitive  infra-red detectors while the device under test is electrically  exercised with automated test equipment (ATE). Common  tests, such as scan, use patterns that are generated through  Automatic Test Pattern Generator (ATPG) in compressed  mode. When these patterns are looped for D-PEM, it results in  indeterministic states within cells during the load or unload  sequences, making interpretation of emission challenging. Moreover, photons are emitted with lower probability and  lesser energies for smaller technology nodes such as the  FinFET. In this paper, we will discuss executing scan tests in  manners that can be used to bring out emission which did not  show up in conventional test loops.


Photon Emission Microscopy (PEM) is a commonly used  semiconductor fault isolation technique. Photons in infra-red  wavelength emitted by transistors and other semiconductor  devices, such as p-n junction diodes, are collected with the  help of highly sensitive detectors while the device under test is  electrically exercised through a static or dynamic setup [1].


Generally, in the static mode of biasing, the photons emitted


are mostly from diode junctions or sub-threshold leakages [2]. When the device is exercised under a dynamic setup on tester, transistor switching contributes significantly to the overall


emission [3]. The tester biasing is done by executing the


structural tests like scan and BIST. A group of input patterns  are injected into the device and the transistor states are toggled  during the pattern execution. There are many sources of


emissions during D-PEM and results can be difficult to


interpret especially as devices scale [4]. Also, with devices


scaling, photons are emitted with lower probability and lesser  energies, requiring fault isolation tools to be equipped with


higher sensitivity and broader wavelength cameras. When


coupled with patterns that exercise the defect better, weaker


emission sites due to subtle defects can be captured.


Scan tests commonly use compressed patterns which makes  targeting of the circuitry of interest difficult. Through test  pattern customization and tester-based lock-in background  subtractions, fault isolation precision can be improved. In this  paper, we will discuss some novel approaches used in scan  tests to capture the emission sites from subtle defects.


2. Experimental Setup


The hardware setup is based on a ThermoFisher system with a  high sensitivity broadband (DBX) emission camera that can  collect photons with a wide spectral range (1-2+um). The  system also supports amplitude lock-in background  subtraction with the DBX camera. A Keithley digital source  meter 2440 is integrated into the system for the lock-In  application.


Standard ATE testers are used to electrically exercise the  device with test patterns. The device under test (DUT) is  electrically connected to the tester through a device interface  board (DIB). A trigger input/output (I/O) pin on the DIB/DUT  assists the triggering required for the amplitude lock-in  background subtraction. The trigger I/O pin is connected to  the source meter on the Thermo Fisher System with the help  of a BNC cable, as shown in Figure 1.


Figure 1: Dynamic amplitude lock-in background subtraction  setup.


For amplitude lock-in D-PEM, two different device states are  used and subtracted from each other. Two different states are  achieved with two separate patterns, background pattern and  signal pattern, where background pattern is a subset of signal  pattern. The source meter controls the test pattern execution  through trigger I/O pin. The ATE is setup to execute signal  pattern when the input from source meter is 1V and  background pattern when the input is 0V as shown in Figure 2. The pulsing continues till the execution is aborted manually. The system software also provides provision to define the  number of pulses to be executed for the lock-in D-PEM.


Figure 2: Pattern execution with respect to voltage biasing  from the source meter.


3. Case Studies


3.1 Scan Chain Failure


The first case study is a reject, failing to scan chain. Scan  diagnostics pointed to multiple instances as suspected defect  locations. Conventional dynamic photon emission is  performed on the area of interest and the results are shown in  Figure 3.


Figure 3: Dynamic photon emission with conventional method  showing emission sites on all the reported failing instances (marked in yellow).


Emission sites are observed across the entire field of view  including all the reported failing instances. The emissions  observed are primarily due to the scan initialization patterns  combined with scan chain pattern execution. The abnormal  emission needed to be differentiated from the expected  emission sites due to normal setup and operation of the DUT. An amplitude lock-in D-PEM is conducted to separate the  emissions from the initialization and the actual test execution. As two separate patterns are required for the lock-in D-PEM, the scan init pattern is set as background pattern and scan  chain pattern together with the scan init pattern is set as signal  pattern (as shown in Figure 4).


Figure 4: The two pattern sets background pattern & signal  pattern customized with Scan Init & Scan Chain patterns


The result of the lock in D-PEM is shown in Figure 5, where a  distinct emission site is observed on one of the reported failing  instances– a scan flop. The stronger emission is due to the  subtraction of emissions from scan init patterns, subtracted  with the help of lock-in D-PEM, and thereby the photon  emission due to the physical defect is isolated.


Figure 5: Dynamic photon emission with lock in method  removed all background emissions sites, leaving a distinct  emission site which matters to the failure (marked in red).


PFA was focused on this suspected scan flop. two-point  probing within the scan flop showed resistive short between an  enable signal and VDD (as shown in Figure 6). TEM  inspection on the shorted location revealed presence of  physical short between the contact (VDD) and the gate (enable).


Figure 6: Two-point probing showing short between the two  signals contact (VDD) and gate (enable).


3.2 Scan Logic Failure


In this case study, the DUT failed gross to scan logic stuck-atfault test pattern. Since the failure is not sensitive to voltage or  frequency, D-PEM was considered. Conventionally D-PEM as  mentioned earlier is performed by electrically exercising the  device with the test patterns that are used in the production  environment. Scan diagnostics pointed to a logic gate as a


161


suspect and emissions are collected on the region of interest  containing the reported logic gate.  No emission site is  observed on the suspected logic gate even when biasing the  device at a voltage 20% higher than the nominal operating  voltage as shown in Figure 7.


Figure 7:  Photoemission with conventional method shows no  emission site on the suspected logic gate (marked in yellow).


The patterns used in the conventional method are generated by  ATPG (Automatic Test Pattern Generator). The values  injected into the scan input pins are not predictable by the user  as they operate in compressed mode. No emission site is  observed on the suspected logic gate by executing the original  logic pattern with the random inputs 1110,0010,0101,1100 on  the pin Scan-In 3 (as shown in Figure 8).


Figure 8: Scan Pattern with random inputs on the scan input  pin Scan-In 3 (marked in red).


As the conventional approach is unsuccessful, a different scan  pattern approach is chosen for photon emission. The random  scan inputs on Scan-In 3 are manually modified to  0000,0000,0000,0000 (as shown in Figure 9). This forced the  input pin to stay low throughout the pattern execution. D-PEM  with this customized pattern execution (in Figure 10) shows  no difference in emission when compared to Figure 3.


Figure 9: Scan Pattern with inputs modified to  0000,0000,0000,0000 on the scan input pin Scan-In 3 (marked  in red).


Figure 10: Dynamic photon emission with customized pattern  execution (0000,0000,0000,0000) shows no emission site on  the suspected logic gate (marked in yellow).


Next the inputs are set as 1111,1111,1111,1111 (as shown in  Figure 11) throughout the pattern


Figure 11: Scan pattern with inputs modified to 1111, 1111, 1111, 1111 on the scan input pin Scan-In 3 (marked in red).


162


A strong emission site is observed on the suspected logic gate, as shown in Figure 12.


Figure 12: By constraining the scan-in to 1111, abnormal  emission site appeared on the suspected logic gate (marked in  yellow).


Physical Failure Analysis was performed on the suspected  logic gate. 2-point probing within the logic gate showed  resistive short between an internal net “n3” and VSS (as  shown in Figure 13. TEM inspection on the shorted location  revealed presence of physical short between the contact (VSS) and the gate (“n3”). The internal net “n3” drives the output X  of the logic gate.  An input of a string of 1s had generated a  logic state of 1 (high) at the output of the logic gate and the  physical short with VSS resulted in a contention phenomenon  at the output net and thereby showed a strong emission site on  the suspected logic gate, matched to reported stuck-at-fault  signature.


Figure 13: 2-point probing showing short between the two  signals VSS (contact) and internal net n3 (gate).


4. Conclusion


Conventional PEM technique is useful for isolating many  failures, but it might not be adequate for certain failures as  discussed in the above two case studies. The two novel  approaches introduced in this paper, scan pattern  customization and amplitude lock-in D-PEM would be a better  alternate for the conventional PEM for specific scan failures.


The results clearly show that these techniques are effective in  bringing out distinct emission sites for both stuck at and chain  failures which was not observed on conventional PEM


technique. A strong emission site on the suspected area  provides higher confidence for physical failure analysis and  there by helps in improving the success rate of failure analysis.


Authors would like to thank AMD management for  sponsoring this work.


© 2019 Advanced Micro Devices, Inc. All rights reserved. AMD, the AMD Arrow logo, and combinations thereof are  trademarks of Advanced Micro Devices, Inc.  Other product  names used in this publication are for identification purposes  only and may be trademarks of their respective companies.


[1] Jiann Min Chin et al., “Fault isolation in  semiconductor product, process, physical and  package failure analysis: Importance and  overview,” Microelectronics Reliability (September  2011), 51 (9-11), pp. 1440-1448.


[2] Christian Boit, “Fundamentals of Photon  Emission (PEM) in Silicon-Electroluminescence for  Analysis of Electronic Circuit and Device  functionality,” Desktop Reference of Failure  Analysis, 2005.


[3] Jacob C.H. Phang et al., “A review of near  infrared photon emission microscopy and  spectroscopy,” IPFA 2005.


[4] Zhongling Qian et al., “Differential and Lockin  Imaging of Dynamic Photon Emission and  Applications in Failure Analysis,” ISTFA 2010.


[5] O. Breitenstein et al., “Thermal Failure Analysis  by IR Lock-in Thermography,” Microelectronics  Failure Analysis, 2011.


163


Copyright © 2019 ASM  International® All rights reserved. www.asminternational.org


# Thermal Failure Analysis of Functional Failures by IR Lock-in Thermal Emission


Thermal Failure Analysis of Functional Failures by IR Lock-in Thermal Emission


Paul Hubert P. Llamera1 and Camille Joyce G. Garcia-Awitan2


Maxim Integrated – Failure Analysis Department, Gateway Business Park, General Trias, Cavite, Philippines  Phone: +632 902 2000 local 2396


Email: 1Paul.Llamera@maximintegrated.com,  2Camille.Garcia@maximintegrated.com


Lock-in Thermography


LIT belongs to the newer generation of IR-based localization  technique with improved sensitivity for fault localization. [5, 7]


Lock-in thermography (LIT), known as a powerful nonWhile PEM uses the principle of electron-hole recombination,


destructive fault localization technique, can also be used for


LIT uses the principle of lock-in and thermography where the


microscopic failure analysis of integrated circuits (ICs). The


device under test (DUT) is powered up using periodically


dynamic characteristic of LIT in terms of measurement,


modulated signal and analyzing its surface temperature


imaging and sensitivity, is a distinct advantage compared to


response using an IR thermo camera as shown in Fig. 1. [5, 6]


other thermal fault localization methods as well as other fault


The sum of thermal images captured while the device is


isolation techniques like emission microscopy. In this study,


unpowered are subtracted from the sum of thermal images


LIT is utilized for failure localization of units exhibiting


captured while the device is powered.


functional failure. Results showed that LIT was able to point  defects with emissions in the mid-wave infra-red (MWIR) range that Photo Emission Microscopy (PEM) with near infrared (NIR) to short- wave infra-red (SWIR) detection  wavelength sensitivity cannot to detect.


The key to successful failure analysis depends highly on the  effective fault isolation technique to pinpoint root cause of  failure and providing the physical manifestation of defect. [1] For functional failures, PEM has been an advantage over laserbased localization techniques in terms of resolution and ease of  detecting many failures through photon emission covering NIR  to SWIR [2].


Fig. 1. LIT Principle


However, the growing complexity of ICs steadily increases


LIT results are presented in terms of Amplitude (total increase


which consequently resulted to smaller dimension and reduced


in temperature during repeated power cycling) and Phase (time


power consumption of basic components like transistors,


delay between powering up and subsequent heating) as shown


creating a more demanding challenge in failure analysis. [3]


in Fig. 2.


Resistive heat generates low energy emissions at longer  wavelengths that are not detected by PEM with NIR and SWIR  sensitivity configuration. [4] Because of this limitation, LIT has  become a complementary fault isolation method for ICs  exhibiting functional failures, since it can detect emission in the  MWIR range. [2, 3]


Over the years, LIT has proven itself to be a powerful tool not  only for non-destructive and packaged-level failure analysis, but also for thermal analysis of devices exhibiting functional  failures. [3, 5, 6] The dynamic characteristic of LIT in terms of  measurement, imaging and sensitivity, has put it in advantage  in comparison to other thermal fault localization methods as  well as other fault isolation techniques like emission  microscopy. [1, 4].


164


Fig. 2. LIT Results


Fig. 3 shows a comparative chart of the wavelength sensitivity  range for different fault isolation detectors. The sensitivity  range of the Enhanced Lock-In Thermal Emission (ELITE) system utilized in the study, uses an Indium Antimonide (InSb) detector that can detect emissions in the MWIR range (3 – 5 µm  wavelength). On the other hand, the sensitivity range of PEM  of the Hamamatsu iPhemos which uses Indium Gallium  Arsenide (InGaAs) detector is on the NIR to SWIR range (0.8 – 1.8 µm wavelength). Hence, resistive heat emissions beyond  the 2000nm range can be detected by the ELITE system making  it a powerful tool for fault isolation of functional failures.


Fig. 3. Fault Isolation Detector Wavelength Sensitivity Range


Case Study 1


A 1-channel high brightness LED driver device was found to  fail on output switching signal. Fault isolation using emission  microscopy while the DUT was exercised using ATE test setup for oscillator frequency showed that multiple internal circuit  blocks of the unit are failing. Because the PEM results are  inconclusive, different fault isolation method was performed  with LIT emission using the same ATE test set-up.


Fig. 4 (a) shows the LIT amplitude image where hotspot was  observed on a poly capacitor inside the regulator circuit block  of the unit. Fig. 4 (b) shows the emission microscopy image on  the same location with no emission observed on the poly  capacitor.


Fig. 4. (a) LIT Image (b) PEM Image


Fig. 5 shows the (a) optical and (b) superimposed LIT image to  optical image and device layout showing defect coincident to  the hotspot observed during LIT fault isolation. The observed  defect suggests a shorted poly capacitor.


Fig. 5. (a) Optical Image (b) Superimposed LIT Image


Case Study 2


A 4-channel high brightness LED driver device was found to  exhibit intermittent output switching signal. Fault isolation  using emission microscopy by powering up the unit using  application specific evaluation kit showed distinct emission on  an NMOS transistor inside the undervoltage lock-out circuit  block of the unit. To verify the result of PEM, unit was  subjected to LIT as a complementary fault isolation method  using the same test set-up.


Fig. 6 (a) shows the LIT amplitude image where hotspot was  observed on a group of metal lines inside the undervoltage lockout circuit block of the unit. Fig. 6 (b) shows the emission  microscopy image on the same location with emission observed  on an NMOS transistor inside the same circuit block.


Fig. 6. (a) LIT Image (b) PEM Image


Fig. 7 shows the (a) optical and (b) superimposed LIT image to  optical image and device layout showing the defect, shorting  net A and net B, coincident to the hotspot observed during LIT  fault isolation.


Fig. 7. (a) Optical Image (b) Superimposed LIT Image


Defect


Metal Lines


NMOS


net A


net B


165


Fig. 8 shows the Focused Ion Beam (FIB) cross-section image  on the hotspot location, where a fabrication defect shorting net  A and net B was observed.


Fig. 8. FIB Image


Review of schematic revealed that the emission observed on the  NMOS transistor inside the undervoltage lock-out circuit block  is due to a failing net C signal which is the inverted signal of  net B, and therefore a secondary effect of the shorting between  net A and net B as shown in Fig. 9.


Fig. 9. Simplified Schematic Diagram


Case Study 3


A 4-channel high brightness LED driver exhibited stuck low  output switching signal. Emission microscopy by powering up  the unit using application specific evaluation kit showed  distinct emission sites on multiple transistors of the unit. Since  the result of PEM is inconclusive, unit was subjected to further  fault isolation using LIT with the same test set-up.


Fig. 10 (a) shows the LIT amplitude image where hotspots were  observed on multiple transistors of the unit. Fig. 10 (b) shows  the emission microscopy results where multiple distinct  emissions were observed on multiple transistors of the unit. Hotspot 2 and emission 6 were found to be on the same PMOS  transistor inside the soft start circuit block of the unit.


(b) Fig. 10. (a) LIT Image (b) PEM Image


Physical failure analysis was focused on the common hotspot  and emission location. Fig. 11 (a) shows the passive voltage  contrast result where bright contact contrast was observed on  the gate of the PMOS transistor. Normal gate contact contrast  is dark. Bright gate contact contrast indicates leakage path to  substrate. Fig 11 (b) shows the FIB cross-section result on the  PMOS transistor where gate oxide damage was observed.


Fig. 11. (a) PVC Image (b) FIB Image


Fig. 12 presents the simplified schematic showing the  relationship between the hotspots and emissions sites. Review  of schematic revealed that hotspots 1 and 3 are directly  connected to the gate of the failing PMOS transistor, while  emissions 4 and 5 are secondary effect of the failure on the gate  signal of the PMOS transistor.


Fig. 12. Simplified Schematic Diagram


Case Study 4


A 4-channel high brightness LED driver device was found to  fail only when dim signal is applied using an application  specific evaluation kit. Fig. 13 shows the fault isolation results  using emission microscopy where (a) distinct emission on the  digital circuit block of the unit was observed when dim signal  was applied and (b) no distinct emission observed on the unit  when no dim signal is fed.


Fig. 13. PEM Results (a) with dim and (b) no dim signal


4  5


Common PMOS


PMOS


PMOS Gate


Gate Oxide  Damage


Bright Gate  Contact


Fabrication Defect


net C NMOS


Shorted Nets


2 and 6


Failing PMOS


166


Further fault isolation thru LIT using same test set-up was  performed on the unit. In Fig. 14 (a), LIT Phase result was able  to identify hotspot location inside the digital circuit block of the  unit even when no DIM signal was fed.


Fig. 14. LIT Results (a) with no dim and (b) with dim signal


In Fig. 15, the results of PEM and LIT were found to be the  comparable to each other when superimposed to the device  layout.


Fig. 15. Superimposed (a) PEM and (b) LIT Results to Layout


Because of the growing complexity of ICs, the reduced  dimension and power consumption of components led to a more  demanding challenge in failure analysis. Defects with emission  wavelengths greater than 2000nm are hard to detect using a  PEM fault isolation method with NIR and SWIR detector  configuration. In this study, ELITE system, which can detect  emission in the MWIR wavelength emission, was successfully  utilized in fault localization of devices with functional failures. LIT was able to point exact defect location that PEM failed to  identify and can detect different failure mechanisms.


Moreover, LIT was proven to be an effective complementary  and alternative fault isolation technique for fault localization of  functional failures. Results from using LIT were found to be  similar and comparable to emissions observed during PEM  fault isolation.


The authors would like to thank Maxim Integrated – Philippines  FA LIT team for their support and guidance on the case studies  and Jerome Escobedo and Zhiyong Wang for supporting and  making this project happen.


[1] Schlangen, R., Deslandes, H., Lundquist, T., Schmidt, C., Altmann, F., Yu, K., Andreasyan, A., & Li, S. (2010). Dynamic lock-in thermography for operation modedependent thermally active fault localization. Microelectronics Reliability, 50, 1454-1458.


[2] M. C. Tan, M. Y. Tay, W. Qiu and S. L. Phoa, "Fault  localization using infra-red lock-in thermography for SOIbased advanced microprocessors," 18th IEEE International  Symposium on the Physical and Failure Analysis of  Integrated Circuits (IPFA), Incheon, 2011, pp. 1-5.


[3] Breitenstein, O., & Altmann, F. (2011). APPLICATION  OF LOCK-IN THERMOGRAPHY TO FAILURE  ANALYSIS IN INTEGRATED CIRCUITS.


[4] J.C.H. Phang et al., “A Review of Near Infrared Photon  Emission Microscopy and Spectroscopy,” Proc. 12th  International Symposium Physical & Failure Analysis of  Integrated Circuits, 2005.


[5] Breitenstein, O & P Rakotoniaina, J & Altmann, Frank & Schulz, J & Linse, G. (2019). Fault Localization and  Functional Testing of ICs by Lock-in Thermography.


[6] X.P.V. Maldague, Theory and Practice of Infrared  Technology for Nondestructive Testing, Wiley, New York (2001)


[7] O. Breitenstein, J.P. Rakotoniaina, F. Altmann, T.Riediger, and M. Gradhand, “New Developments in IR Lock-in  Thermography,” Proc. 30th International Symposium for  Testing & Failure Analysis, 2004


Amplitude


Phase


167


Interpreting laser-based fault localization results: Case studies


Sukho Lee, John van den Biggelaar, Marc van Veenhuizen


Product Diagnostic Center, NXP Semiconductors, Nijmegen, Netherlands  sukho.lee@nxp.com


Laser-based dynamic analysis has become a very important tool  for analyzing advanced process technology and complex circuit  design. Thus, many good reference papers discuss a high  resolution, high sensitivity, and useful applications. However, proper interpretation of the measurement is very important as  well to understand the failure behavior and to find the root  cause. This paper demonstrates this importance by describing  two insightful case studies on laser voltage probing (LVP) and  soft defect localization (SDL) which could only be resolved by  a detailed interpretation of the measurement results.


The first case is a sawtooth LVP signal induced by a metal  short. We will talk about the unusual LVI/LVP results when the  signal modulation is dominated by the channel region of a  transistor. The second case is a mismatched result between an  LVP and SDL analysis. This is a good case of unusual LVP data  induced by a very sensitive response to laser light.


Case 1: Sawtooth LVP waveform induced by a metal short


Figure 1: Simplified schematic of the function block.


Figure 1 shows a simplified schematic of a custom-designed  circuit with two complementary input signals. Failure analysis (FA) was requested to investigate a functional failure that  suffered from a missing output signal. The FA set up was  prepared with an application test environment because the  faulty design block is designed without scan insertion. But the  application test program easily generated complementary  square wave input signals. Therefore, fault localization started  with laser voltage imaging (LVI) which provides the most  reliable and visualized result for signal frequency signal trace.


Initially, the designer had a suspected design block after fail  behavior observation and lots of debugging. Base on the


candidate from the designer, the area of interest was scanned  for a 1 MHz input frequency and mapped onto the LSM image. Although the first LVI results did not indicate a fail location  clearly, it did show a brighter (higher intensity) image on NOR1  and NOR2 for the fail device, as shown in Fig. 2.


Figure 2: LVI results in the suspected area (Infrascan, Checkpoint).


It is likely that the 1 MHz frequency signal still exists on the  NOR gates but is unusual which therefore requires a more  detailed analysis. So, the analysis was continued with LVP on  several important nodes around NOR1/2, given in Fig. 3. LVP  measurement confirmed that the abnormality is observed from  the output node of NOR1 and NOR2.


Figure 3: LVP waveform from NOR gates (Normalized  amplitude).


Some interesting observations are described below.


1. Sawtooth signals were observed on the NMOS of the


NOR1/2 out (NOR1/2_out_n) node, curved falling signals


were observed on the PMOS of the NOR1 out


(NOR1_out_n) node , and distorted signals were observed


on the PMOS of the NOR2 out (NOR2_out_n) node.


# Interpreting laser-based fault localization results: Case studies


168


2. The amplitude of the sawtooth signal is 10 times bigger


than the other signals. And this matches the abnormally


brighter LVI image.


3. The switching time of the output signals of NOR1/2 is not


simultaneous to each other but appear to be mixed.


4. Glitch signals were observed on the NOR3/4 output node


and the timing of the glitch matches the falling edge of the


NOR1/2 input.


From LVP signals observation, we expected that the fail  symptom is due to a certain signal interference such as a short  or a cross-talk of two input signals around NOR1/2.


(a) LVI image with the INB signal disabled.


(b) LVI image with the IN signal disabled.


Figure 4: LVI image with respective input signal disabled.


After more brainstorming and debugging, we found that the  circuit is still functional when one of the input signals is  disabled. Therefore, it is expected that this experiment provides  the frequency component from only one signal path for the  reference device whereas for the fail device an additional signal  path is expected. Indeed, as observed from Fig. 4, the LVI result  for the reference device shows that only one signal path is  mapped with a 1 MHz LVI image. However, brighter images  were observed from the opposite side of the signal path on  NOR1/2 for the fail device. The combination of the two images  of Fig. 4 gives just the same LVI image as depicted in Fig. 2  which stands true for both reference and fail device.


CAD Navigation Database:


Various data sources from the IC design flow are used to build  a cohesive CADNav database. It consolidates all of the  necessary design data for FA and allows custom configurations  to the database in order to match the manufactured silicon  product.


Database Inputs:


A complete CADNav database is generated from three primary  design data sources:


I. Layout File:


A file containing the physical CAD layout for all mask layers in the IC. Common formats include GDSII and OASIS. Along with the layout file, additional information such as layer name,order of layers in which they are manufactured along with information required to reconstruct the design intent layers in case the process technology uses the multi patterning


# Fast and Accurate Fault Localization Through Effective Use of Design Schematics


173


technology (MPT). This information can be obtained from  designers.


II. Netlist/Schematic File:


A netlist file contains circuit connectivity information. Most  commonly used format used in the industry is SPICE. The  schematic files in EDIF and OpenAccess formats contain  graphic representation of circuit along with netlist  connectivity.


III. Layout Versus Schematic (LVS) Files:


A set of files generated during physical verification that checks  and confirms the consistency between IC layout and


schematic. The results of “sign off” LVS run are used to


correlate devices, nets and instances from physical domain (layout) to the logical domain (netlists) and vice versa.


Fig 2. CAD data preparation


Database for Mixed Signal design flows:


Mixed mode designs, or “systems on a chip” (SoC), are  becoming increasingly popular and have gained market  acceptance worldwide. SoC designs are getting more and more  complex in their logic parts in efforts to enhance functional  intelligence. The growing complexity of logic parts has driven  a change in the overall design flow. It becomes impossible to  code complex logic parts with schematic view file types such  as EDIF. Apart from regular netlist data that gives design  hierarchy and connectivity information, mixed signal design  flows have data to visualize schematic for analog blocks. The  graphical presentation of a device’s schematics is a  requirement for successful failure analysis in mixed signal and  analog ICs.


A feature in Synopsys® Avalon™ supports integrating and  aligning multiple design files and flows, such that a user can  obtain maximum visualization value through a seamless UI  display, even in conditions when incomplete details exist.


The solution allows viewing of design quality schematics when  the necessary EDIF file details exist, while other parts of the  circuit which only have a SPICE/CDL netlist representation  are shown in a synthesized schematic view in parallel. Thus, it  will allow a true mixed mode operation and provide design  quality schematics for analog components and a safe fall back  to synthesized schematic for logic blocks. This will also allow  user to cross probe the nets, devices, or instances from  schematic to layout and vice versa through a highly optimized


and efficient Crossmap1 database, which is generated using  netlist data for the complete design.


Figure 3 shows the schematic view dynamically working on  both netlist DB and schematic DB. It reads the schematic DB  to display design quality schematic for analog blocks. It  generates synthesized schematic for logic blocks based on the  connectivity information from netlist DB.


Fig 3. Schematic view for mixed signal design flows


Usage of Design Schematic in FA Flows


Fault Isolation using ATPG Scan Chain Analysis and  Schematic Data:


To assist a designer or a failure analysis engineer, the  diagnosis tool tries to identify the possible locations of the  failure effectively and quickly. While many defects reside in  the logic part of a chip, defects in scan chains have become  more common in recent nodes. As 30%-50% of logic gates on  a typical chip impact the operation of scan chains [Kundu 94], scan chain failures are the cause of a substantial proportion of  failing chips. Accurate diagnosis of scan chain failures is  important for physical failure analysis and yield analysis [2].


Laser Voltage Imaging (LVI) provides a unique capability to  map the periodic signal [3-6] in a DUT, which makes it a great  diagnostic technique for scan chain failures, whether the  failure is due to a clock issue or an issue with the latch itself. In addition, LVP probing [7-9] can further confirm the failure  identified by LVI.


The typical FA workflow for scan chain integrity failures starts  by using an ATPG Diagnostics tool (provided by an EDA  vendor). The diagnosis will provide a list of candidates that  could be causing the failure, identified by scan chain name and  scan cell position along the chain, as well as instance and net  names and various attributes to aid analysis (e.g., fault scores  and suspected fault type).


To analyze the scan chain report from diagnosis report, the  complete chain information is imported onto the CADNav  layout by means of querying the integrated schematic data in  the crossmap database. The diagnosis results are overlaid with


174


LVI image. The data from three domains viz. mask layout, LVI image and diagnosis result help accurately pin point the  broken chain [1]. Figure 4 shows the broken chain location. This approach ultimately tends to detect where in the chain, the data stops propagating due to any of the fault models like  the stuck-at fault model, the bridge fault model, the open fault  model, the gate delay fault model and the path delay fault  model.


Figure 4: Scan cell bounding boxes from diagnosis overlaid  with LVI image to detect scan chain failure


Further debug of logic blocks at the fail location helps FA  engineers accurately assess the root cause of the failure. For  this, the gate or device at the identified failed location is  loaded in the schematic viewer. Figure 5.1 and 5.2 shows the  layout and the schematic of the failed scan cell.


Figure 5.1: Scan cell mapped to layout viewer


Figure 5.2: Scan cell mapped to schematic viewer


For further analysis of scan cell, driving instance is found and  input cone is analyzed as shown in figure 6. This helps in fault  back tracking.


Figure 6: Driving instance and input cone in schematic viewer


Once the driver is found, the net along with receivers can be  cross mapped back to layout view as shown in figures 7 and  figure 8. This helps in finding the accurate location in layout  view for further physical failure analysis.


175


Figure 7.1: Receiver and Driver highlighted in schematic view


Figure 7.2: Receiver and Driver highlighted in layout view


Figure 8: Driving instance highlighted in red color in layout  view


For device level analysis, the transistors of the driving instance  are mapped from schematic to layout. Figure 9.1 and 9.2  shows the transistor highlighted in schematic and layout view. These device locations are then sent to analytical tool for  physical analysis like nanoprobing.


Figure 9.1: Devices highlighted in schematic view


Figure 9.2: Devices highlighted in layout view


Fault Isolation Using Diagnosis and Schematic Data:


ATPG scan failures have been one of the main failures  contributing to low yield issues and problems in  microelectronics. Diagnosis tools are used to analyze the such  failures [10]. This often requires more intensive crossreferencing between CAD layout and schematic.


The diagnosis results are loaded and overlaid to CAD layout  as shown in figure 10. At times, analysis of gates or nets  reported by diagnosis needs circuit level analysis. The reported  net from diagnosis is crossmapped to schematic as shown in  figure 11. This opens whole lot of possibilities to perform  logic analysis on the potential fail net before finalizing the area  for physical failure analysis.


176


Figure 10: Diagnosis results overlaid on CAD layout


Figure 11: Connectivity of net reported by diagnosis in  schematic viewer


Fault Isolation using Cell-Aware Diagnosis Results and  Schematic Data:


Even when a defect is known to be within a cell, finding  defects in a complex cell in physical failure analysis (PFA) can  be daunting. Determining whether such a defect is systematic  or yield limiting typically requires the examination of a large  number of failing die, which can take several months. Cellaware diagnosis short-cuts the lengthy investigation process by  pinpointing a small subsection of the suspected cell. [11]


Cell-aware test targets specific shorts opens and other physical  defects internal to each cell by modeling it at the transistor  level. Analog simulations are performed to characterize the  effects of potential short and open defects. Based on the  analog simulation results, a cell-aware fault model is created  that directs ATPG to generate patterns targeting these internal  cell defects. There have been multiple studies that show that


tests generated using cell-aware fault models find defects that  the normal test methods miss.


The cell aware fault models help to accurately pin point the  transistor causing the defect. Figure 12 shows cell test model (CTM) defects from a cell aware diagnosis results overlaid  with design layout. As shown in figure 13, crossmapping the  nearest transistor to a CTM defect helps to locate the device in  schematic view. Further analysis of connectivity, driver of this  faulty transistor helps to find the root cause and narrow down  the area for a successful PFA.


Figure 12: CTM defects from cell aware diagnosis results  overlaid on CAD layout


Figure 13: Faulty transistor from cell aware diagnosis results  overlaid in schematic viewer


In summary, the presented methods of using schematic data  and viewer for logic analysis helps the FA engineer to perform  more accurate fault isolation before proceeding to expensive  physical failure analysis. Here circuit analysis helps the failure  analysis engineer focus on the most critical nets and devices  for faster fault localization and failure analysis.


177


Acknowledgements to Synopsys® Inc. Silicon Engineering  Group and Avalon team.


[1] Arpan Bhattacherjee, Martin Parley, “CAD Navigation  Principles”, EDFAS Desk Reference, 7th Ed.


[2] Tang, Xun, University of Iowa, "Diagnosis of VLSI  circuit defects: defects in scan chain and circuit logic." PhD (Doctor of Philosophy) thesis, 2010


[3] Zhigang Song and Laura Safran, GlobalFoundries, “LVI  AND LVP APPLICATIONS IN IN-LINE SCAN CHAIN  FAILURE ANALYSIS”, EDFAAO (2016) 4:4-14


[4] Y.S. Ng, T. Lundquist, D. Skvortsov, J. Liao, S. Kasapi, and H. Marks: “Laser Voltage Imaging: A New  Perspective of Laser Voltage Probing,” Int. Symp. Test. Fail. Anal. (ISTFA), 2010.


[5] Y.S. Ng, H. Marks, C. Nemirov, C.C. Tsao, and J. Vickers: “Scan-Shift Debug Using LVI Phase Mapping” Int. Symp. Test. Fail. Anal. (ISTFA), 2013


[6] T. Parrassin, G. Celi, S. Dudit, M. Vallet, A. Reverdy, P. Perdu, and D. Lewis: “Laser Voltage Imaging and Its  Derivatives, Efficient Techniques to Address Defect on 28  nm Technology” Int. Symp. Test. Fail. Anal. (ISTFA),


2013.


[7] H.K. Heinrich, D.M. Bloom, B.R. Hemenway, K. McGroddy, and U. Keller: “Noninvasive Optical Sheet  Charge Density Probe for Silicon Integrated Circuits,” IEEE Trans. Electron Dev., 1987, 33(11), p. 1860.


[8] M. Paniccia, T. Eiles, V.R.M. Rao, and W.M. Yee: “Novel Optical Probing Technique for Flip-Chip  Packaged Microprocessors,” Proc. Int. Test Conf. (ITC), 1998, p. 740.


[9] Y.S. Ng, W. Lo, and K. Wilsher: “Next Generation Laser  Voltage Probing,” Proc. Int. Symp. Test. Fail. Anal. (ISTFA), 2008, p. 249.


[10] A. G. Boon, C. C. Kit, C. K. Keng and O. C. Khiam, "TetraMax Diagnosis and Laker Software on Failure  Analysis For ATPG/Scan Failures," 2006 13th  International Symposium on the Physical and Failure  Analysis of Integrated Circuits, Singapore, 2006, pp. 217-221.


[11] Geir Eide, “Transistor-Level Defect Diagnosis”, December 22nd, 2016, Semiconductor Engineering.


178


MBIST Driven SRAM Failure Analysis Using Laser Voltage Imaging and Laser  Voltage Probing


Jessica Yang, Omprakash Rengaraj, Puneet Gupta, Rudolf Schlangen


NVIDIA, Santa Clara, California, USA   jesyang@nvidia.com


Static Random-Access Memory (SRAM) failure analysis (FA) is important during chip-level reliability evaluation and yield  improvement. Single-bit, paired-bit, and quad-bit failures—whose defect should be at the failing bit-cell locations—can be  directly sent for Physical Failure Analysis (PFA). For one or  multiple row/column failures with too large of a suspected  circuit area, more detailed fault isolation is required before  PFA. Currently, Photon Emission Microscopy (PEM) is the  most commonly used Electrical Failure Analysis (EFA) technique for this kind of fail [1]. Soft-Defect Localization / Dynamic Laser Stimulation (SDL/DLS) can also be applied on  soft (Vmin) row/column fails for further isolation [2]. However, some failures do not have abnormal emission spots  or DLS sensitivity and require different localization  techniques. Laser Voltage Imaging (LVI) and Laser Voltage  Probing (LVP) are widely established for logic EFA, [3] but


require periodic activation via ATE which may not be possible  using MBIST hardware and test-patterns optimized for fast  production testing. This paper discusses the test setup  challenges to enable LVI & LVP on SRAM fails and includes  two case studies on <14 nm advanced process silicon.


The fault isolation and diagnosis of SRAMs is significant as  their density and circuit proportion keep increasing in systemon-chips (SOC). Prior to FA, a multi-level fault diagnosis flow  is used to provide information including failing RAM instance  type, the defect classification, logical and physical location of  faults, etc. In production, it is executed as follows: Automated  Test Equipment (ATE) runs production Memory Built-In SelfTests (MBIST) pattern to identify the first failing RAM  instance for each BIST engine. Then bitmap pattern is  executed on target failing RAM instances and provides the  failing logical addresses (rows and columns) as well as the  physical X, Y coordinates for each failing bit-cell.


MBIST and bitmapping vectors are the most commonly used  fault diagnosis patterns in production field. Hence, PEM on  SRAM can be performed while looping on these two patterns  as stimulus. The two case study examples included in this  paper do not show any abnormal PEM hotspots with MBIST  or bitmap patterns and both have “hard fails” (no passing  condition), so SDL cannot be used. The loop mode MBIST


pattern is proposed to enable LVI & LVP as an alternative  way of failure analysis.


Loop Mode MBIST pattern


The main challenge for enabling LVP is the test setup, since it  requires periodic activity in the RAM with shortest possible  test-loop-length. The generic MBIST architecture consists of  multiple blocks as displayed in figure.1 [4]. The controller  controls the overall test process and the pattern generator  provides address sequence and data vectors required for test, then response analyzer feeds back to controller with test result. From this test procedure, each SRAM macro is logically  addressable by the BIST engine, and a sequence of March test  algorithm M with a finite number of March Elements (MEs) M1; M2; …; Mi; ... to be executed. Each March Element Mi  consists of an addressing order Ai and a finite number of  Read/Write operations [5, 6]:


Mi = Ai (O1D1, …, OmDm)


 Ai ∈{Ascending, descending, arbitrary};


 Oj  ∈{R, W} - operations: R – Read, W – Write;


 Dj - background pattern.


Figure.1 generic MBIST architecture


The address space and MEs are JTAG programmable. For a  production MBIST pattern running in an ATE environment, the MBIST engine is programmed to go through the entire  address space across all MEs and stop on first fail of each  BIST engine. This mode cannot be used for LVP since the  resulting loop length (pattern length) would be much too long (several ms) and the targeted RAM would only be activated  for a fraction of the loop.


The setup can be improved by using a “targeted MBIST  pattern” where only the targeted RAM is tested by specific


179


MEs. But the resulting loop-length will most likely still be too  long since every loop repetition must include the j-tag register  programming and j-tag is usually limited to run at low  frequency (<50MHz).  The best possible test setup for LVP is  enabling an MBIST internal loop mode, where the ATE  programs the MBIST engine via j-tag only once at the start (specifying the RAM, address space & MEs) and the MBIST  engine will continue to execute the programmed sequence  infinitely, until stopped via j-tag command. This mode does  not produce any pass/fail decision but its best suited for  applications like LVI & LVP since it generates continuous and  periodic activity throughout the whole RAM, including write & read periphery and IO data paths.


Some RAM designs include scan-flops in the IO data-path  and/or address registers, which can also be used for periodic  activation by simply looping scan-shift or ATPG pattern, but  that only activates limited areas of the RAM periphery without  toggling the bit-array and associated circuits (eg. sense  amplifier connecting to bit-lines). In addition, the RAM design  of the failing instances in our case study examples does not  implement any scan-flops within RAM macro, so logic scan  patterns would not be useful for FA in these cases.


Case study A shows a partial physical row failing and case  study B shows two full physical columns failing. For both  cases A & B we programmed the MBIST engine to test just  one physical row then let the engine run in an infinite mode  such that it kept looping pre-programmed MEs across the  defined address range. These special loop mode patterns allow  us to observe the toggling condition of the SRAM macro’s  peripheral circuitry with LVI and LVP.


Analysis of SRAM failing cases


For the case study A, the RAM was failing all bits from one  half of physical row#216, which indicates the defect could be  along the Word-Line (WL) path within the periphery driving  this partial row. The loop mode pattern programmed the  targeted SRAM macro to keep writing checkerboard data (alternate ‘1’ and ‘0’) for physical row#216 to induce repeated  toggling on the suspected WL path. As shown in Fig. 2, LVI  on the passing half of the targeted row shows normal  modulation mapping on bit-cells of the half row, WL driver, WL driver-1 (the gate driving WL driver) and WL driver-2 (the gate driving WL driver-1). The failing half does not show  the identical modulation mapping starting from WL driver-1. The LVP result shown in Fig. 3 clearly displays an abnormally  distorted waveform on WL driver-2 of the failing half row  which results in weak signal on WL driver-1 then eventually  stuck-at signal on WL driver. Based on the LVI and LVP  results, the WL driver-2, along with its input and output nets, were called out for PFA inspection. PFA found a short defect  induced by an abnormal Via (V0) connecting M0 and the  drain of transistor (MD) within WL driver-2 n-FET area.


Figure.2: 1st example – LVI


Figure.3: 1st example – LVP. Left part of image displaying  signals from passing half row vs. Right part of image


displaying signals from failing half row.


In case study B, all addresses fail in two neighboring physical  columns, which constitute one logical column sharing one  write/read data path in the periphery. Therefore, the defect is  suspected to be along this data path of the failing logical  column. To repeatedly toggle the data paths, including the  suspected one, one loop mode MBIST pattern was created to  write checkerboard data once to the first address and then  infinitely read out data from all bits. In Figure 4 LVI shows  that the gate Driver-2 is normal with identical modulation  mapping compared with neighboring gates of passing  columns. Driver-1 (driven by Driver-2 and driving the data  input of sense latch) displays abnormal data & clock  modulation mapping. The following sense latch does not show  the expected data modulation and is likely stuck-at. The LVP  result shown in Figure 5 confirms the failing behavior: the  signal is stuck-at starting from the output of Driver-1. In this  case, the Driver-1 gate, along with its input and output net, were called-out for PFA. A gate (MG) to drain (MD) short  defect was successfully identified within Driver-1 n-FET area.


181


Figure.4: 2nd example – LVI


Figure.5: 2nd example – LVP. Left part of image displaying  signals from neighboring passing column vs. Right part of  image displaying signals from failing column.


These two case study examples demonstrate that the special


loop mode MBIST vectors can be very useful to enable LVI & LVP techniques for SRAM failure analysis. By programming  the vectors to activate a specific address range with intended  pattern sets, these loop mode MBIST vectors create infinite


periodic toggling for failing rows or columns as well as the


corresponding peripheral paths. This technique facilitates


direct observation of where the signal starts to become


abnormal and subsequently, identification of the defective


circuit/nets. This is also an alternative way to enable PFA in


the absence of PE spots and / or SDL localization.


[1] JCH Phang, DSH Chan, SL Tan, WB Len, KH Yim, LS  Koh, CM Chua, and LJ Balk, “A Review of Near Infrared  Photon Emission Microscopy and Spectroscopy,” Proc. 12th IEEE International Symposium on the Physical and


Failure Analysis of Integrated Circuits (IPFA), Singapore


2005.


[2] Je, M.S. & Lian, Y.B. & Goh, S. H. & Chithambaram, S & Quah, A. & Lam, J., “Application of soft defect  localization technique for SRAM soft failure debug,” Proceedings of the 40th International Symposium for  Testing and Failure Analysis (ISTFA), Nov.2014, Houston, Texas, pp 307-311.


[3] Kasapi, S., Lo, W., Liao, J., Cory, B., and Marks, H., “Advanced Scan Chain Failure Analysis Using Laser  Modulation Mapping and Continuous Wave Probing,” Proc. 37th International Symposium for Testing and  Failure Analysis (ISTFA), Nov 2011, San Jose, CA, pp. 12-7.


[4] Zaidi Haron, Nor & Mat Junos, Siti Aisah & Razak, Abdul & Idris, Muhammad. (2008). “Modeling and simulation  of finite state machine Memory Built-in Self-Test  architecture for embedded memories”, IEEE Asia-Pacific  Conference on Applied Electromagnetics (APACE).2007


[5] G. Harutyunyan, S. Martirosyan, S. Shoukourian, Y.


Zorian, “Memory Physical Aware Multi-Level Fault


Diagnosis Flow”, IEEE Transactions on Emerging Topics  in Computing, 2018.


[6] K. Darbinyan, G. Harutyunyan, S. Shoukourian, V. Vardanian and Y. Zorian, "A Robust Solution for  Embedded Memory Test and Repair," 2011 Asian Test  Symposium, New Delhi, 2011, pp. 461-462.


A New Approach to IDDQ Failure Fault Localization  Using Single Shot Logic (SSL) Patterns


Rommel Estores and Stefaan Verleye


In this paper the authors will discuss an application of Single  Shot Logic (SSL) patterns used for further localizing IDDQ  failures using ATPG constraints and targeted faults. This new  method provides the analyst a possibility of performing circuit  analysis using IDDQ measurement results as a pass/fail  criterion rather than logic mismatches. Once a defective area  was partially isolated through fault localization, SSL patterns  were created to control individual internal node logic states in a  deterministic way. IDDQ was measured at each SSL iteration  where schematic analysis can further isolate the failure to a  specific location. Two case studies will be discussed to show  how this technique was used on actual failing units, with  detailed explanation of the steps performed that led to a more  precise determination of the fault location in the suspect cell.


Automatic Test Pattern Generation (ATPG) utilizes different  fault models to detect faults in the digital core where Design  For Test (DFT) was implemented. These fault models include  stuck-at, transition delay, bridging, cell aware, loopback, and  IDDQ. With the exception of IDDQ, these fault models detect  mismatches to determine a passing or failing result. ATPG  diagnosis can then be used to isolate the fault in the digital. On  the other hand, IDDQ fault model requires measurement of the  IDDQ current in the determination of a passing or failing result. ATPG diagnosis cannot be used for IDDQ fault model for units  that fail a current measurement on the tester without  corresponding vector failures. To isolate an IDDQ fault, the  analyst makes use of other fault isolation techniques like  Photoemission Microscopy (PEM) [5], Optical Beam Induced  Resistance Change (OBIRCH) [6] analysis, Thermal Imaging (Thermography). Generally, the failing unit is put in a static  condition where the IDDQ current is higher than normal; then  fault localization is performed. If needed, the unit could also be  put on a static condition where the IDDQ current is normal for  comparative results. A good unit may also be used as a  reference from which the failing device results may be  compared to. On the failing units where both the patterns from  logical fault models (stuck-at, bridging, transition delay, …) and IDDQ current measurement were failing, the analyst could  perform both ATPG diagnosis, dynamic and static fault  isolation techniques to try and isolate the fault. However, there  were cases where only the IDDQ current measurement is failing  while all the other patterns were passing. This is the case for the


two failing units that will be discussed on this paper. In  addition, ATPG diagnosis may lead to multiple candidates  whereby SSL patterns could be utilized for further localization.


Digital Design File Requirements and Cost-Effective  Implementation


As described in our previous paper on Single Shot Logic Pattern


[1], various digital design files were needed including the  ATPG-ready archive of the design [3][4] to enable the FA  group to perform ATPG testing, diagnosis, and generation of  new patterns including single shot logic (SSL) patterns.


ATPG testing and characterization was performed using a  compact test HW [2]. An IDDQ module, implemented on the  test board, was used for easy and fast IDDQ current  measurements. Furthermore, the compact test HW uses a userfriendly GUI with great flexibility for testing and analysis, allowing easy manipulation of test parameters like voltages, timings, editing the test settings including adding IDDQ  measurement points. For logic failures, the result shows the  mismatches in relation the test data and directly identifies the  mismatching scan cells. This gives the analyst more flexibility  for a faster and in-depth analysis including use of single shot  logic patterns.


Bringing direct access to the ATPG tools and files enables the  analyst to read in the design, write out new pattern sets like  single shot logic patterns to a desired settings and format. Efficiency in ATPG testing, ATPG diagnosis, and use of single  shot logic patterns in analysis could be realized by combining  direct access to the ATPG tools and files with the compact test  HW.


In addition to the LVI results, the LVP waveforms were  obtained in the same way, see Fig. 5. Abnormal high amplitude  and curved waveforms (sawtooth waveform from the first  measurement) were observed for the disabled signal path on  NOR1/2. Plus, the waveforms from NOR3 and NOR4 are an  exact copy of each other even though one of them should be  disabled for a single input. Thus, the fail behavior seemed to be  that the output signal of NOR1 was transferred to NOR2 and


vice versa. This realization led us to layout inspection to look  for possibilities of a short between the NOR outputs. Indeed, it  was observed that these nodes are laid by two long metal lines  that run parallel with minimum design rule space. To further  investigate this root-cause hypothesis, a device simulation was  performed to reveal if the measured fail behavior could be  reproduced.


(a) NOR1/2 LVP waveform with the INB signal off.


(b) NOR1/2 LVP waveform when the IN signal off.


(c) NOR3/4 LVP waveform with the IN or the INB signal  off.


Figure 5: LVP waveform with respective input signal disabled (Normalized amplitude).


(a) Simulated waveform with a metal short model.


(b) LVP waveform from the fail device.


Figure 6: Simulation versus LVP result in NOR3/4.


Figure 6 shows a simulation result with the suspected metal  short fail inserted into the model and the result corresponds the  same with the measured LVP waveform of Fig. 3, so we were  very convinced of the metal short failure. And we believed that  optical beam induced resistance change (OBIRCH) is the most  proper analysis tool to narrow down the fail location. Two  probe pads were created by focused ion beam (FIB) on the


169


output signal node of NOR1 and NOR2. The probe pads were  biased carefully with small voltage and current compliance to  prevent damage from high current flow during OBIRCH  measurement.


(a) OBIRCH image with 5X mag.


(b) OBIRCH image with 200X mag.


Figure 7: OBIRCH image (Phemos1000, Hamamatus).


The top side image of Fig. 7 shows the location of the probe  pads and the overall current path displayed by OBIRCH  between the two probe pads, and the bottom side image shows  the short fail location in more detail. Although the OBIRCH  signal was partially blocked by horizontal metal lines above the  suspected metal layer, we believed that the OBIRCH spot  indicated the short location. Therefore we decided to continue  FIB cross-section analysis and observed a metal short between  two metal lines as shown in Fig. 8.


Figure 8: FIB X-section image showing a metal short.


It was difficult to interpret the abnormally strong LVI image  and the sawtooth LVP waveforms at the beginning of the  analysis. But after confirmation of the metal short between the  output nodes of the two NOR gates, we were able to explain the  observations. In principal digital circuits have no static IDS  current so LVP waveforms are measured mainly by modulation  of the drain area of the transistors and the modulation from the  channel region is weak. But in this case, the modulation at  channel region becomes more dominant due to the IDS current  caused by the metal short. Although the fundamental  understanding is subject to further study, we were nevertheless  successfully able to interpret the observations of the laser-based  fault localization tools such as LVI, LVP, and OBIRCH.


Case 2: Mismatch between LVP and SDL result


This case explains the impact of the laser light on the transistor  comparing the LVP waveform and SDL spot location from low  voltage scan chain failure analysis.


Figure 9: Scan chain pattern shmoo plot.


As shown in Fig. 9, the fail device showed less voltage margin  from the scan chain test pattern compared with a reference  device. The shmoo boundary looks like having a typical shape  of a hold violation which is only dependent on the operating  voltage.


But after we reviewed the fail log, we understood that the failure  behavior is something different. The fail log from 1V looks like  a hold violation but the failing cycle is the 1st vector after data  switching which means a slow transition. And it became worse  when the voltage was lowered to 0.95V showing data were not  able to switch from “H” to “L” at all.


Scan chain fault localization normally starts with the LVI  binary search method through the failing chain with data  frequency. The fail location was narrowed down between flipflops FF_0 output (Q) and FF_1 scan input (SI) using LVI. The  fail location might be the output driver transistor of FF_0 or the  metal interconnection of the Q signal node between the two  FFs. But the FF_1 internal node was not considered as a  possible fail location because the LVI image didn’t show  activity inside of FF_1. LVP waveforms revealed a very slow  falling slope from the output driver PMOS transistor depending  on the operation voltage but the waveform from the NMOS  transistor looked normal. From the LVP result observation, the  metal interconnection layer of the FF_0 Q could be excluded


and the PMOS transistor became a strong candidate for the fail  location.


Figure 10: Fail log from 1V and 0.95V.


Figure 11: LVI&LVP data from low voltage scan chain failure.


Because this is a typical type of marginal failure, we still had a  chance to perform LADA/SDL analysis and we expected that  would indicate the faulty location very accurately somewhere  in the PMOS transistor.


Figure 12: SDL image and overlaid shmoo plot.


As shown in Fig. 12, the SDL result indicated the faulty location  with a clear spot, but the location is not on the PMOS but rather  on the NMOS transistor of the output driver (FF_0 Q). This


mismatched result between LVP and SDL was a bit confusing  but later this gave very impressive information.


We were able to interpret the observation with a combination  of logic circuit function and SDL theory. The slow falling slope  can be explained by the digital circuit function that the falling  signal is driven by the nmos and the rising signal is driven by  the pmos. Thus, although we observed the slow slope on the  pmos, it stemmed from the slow performance of the nmos.  The  reason why we could not observe a slow slope from LVP  measurement on the nmos can be explained from SDL theory. As can be seen from the shmoo plot in Fig. 12, the voltage  margin shifted very sensitively in response to the laser light. Hence, the nmos transistor’s voltage margin was already shifted  significantly during the LVP measurement, therefore we were  not able to observe a slow slope from the LVP waveform on the  nmos.


The assumption from LVP and SDL measurement was  supported by TEM cross-section inspection providing a soft  defect in the gate oxide layer.


We generally believe that LVP and LADA/SDL indicate the fail  location straightforwardly in most of the cases. However, this  case demonstrates that LVP can indicate a fail location  indirectly due to a certain amount of stimulation by laser light  during signal probing. And it is important to know/judge  whether the probing location is sensitive to even a small amount  of laser light that then may influence the obtained waveforms.


Two unique case studies have been presented with very unique  observations from LVI/LVP, OBIRCH, and SDL analysis. The  observations did not pinpoint straightforwardly to the root  cause but instead required an in-depth interpretation of the FA  results. Because a misunderstanding from insufficient data  possibly drives in the wrong direction of the next procedure, it  is very important to understand and interpret the analysis results  to find the root cause or to decide what is the most meaningful  analysis for the next step. The authors believe that this paper  provides a good reference on how to properly explain FA  results.


[1] U Kindereit, G Woods, J Tian, U Kerst, C Boit,


“Investigation of Laser Voltage Probing Signals in CMOS  Transistors”, Proc 45th IEEE Int’l Reliability Physics  Symp, Phoenix, Arizona, April 2007, pp. 526-532.


[2] Yin S Ng et al, “Laser Voltage Imaging: A new Perspective  of Laser Voltage Probing”, Proc 36th Int’l Symp for Testing  and Failure Analysis, Dallas, Texas, November 2010, pp. 5-13.


[3] Jeremy A. Rowlette, Travis M. Eiles, “Critical Timing  Analysis in Microprocessors Using Near-IR Laser Assisted  Device Alteration (LADA)”, Proc 32nd Int’l Test  Conference, Charlotte, NC, October 2003, pp. 264-273.


171


[4] Kent Erington, Dan Bodoh, Kris Dickson, George Lange, “The Role of Free Carrier Absorption in LADA”, Proc 40th  Int’l Symp for Testing and Failure Analysis, Houston, Texas, November 2014, pp. 73-81.


[5] Kyeongju Jin et al, “Laser Stimulation Effect on FinFET  and Case”, Proc 41st Int’l Symp for Testing and Failure  Analysis, Houston, Portland, Oregon 2015, pp. 243-246.


[6] Keonil Kim et al, “Verification of DLS data by LVP in case  of marginal failure’, Proc 42nd Int’l Symp for Testing and  Failure Analysis, Fort Worth, Texas 2016, pp. 573-575.


172


Fast and Accurate Fault Localization Through Effective Use of Design  Schematics


Dr. Ankush Oberai


Synopsys Inc. Mountain View, California, USA


Ankush.Oberai@synopsys.com, Ph: +1-408-888-3542


Rupa Kamoji


Synopsys India Pvt. Ltd. Mumbai, Maharashtra, India  Rupa.Kamoji@synopsys.com, Ph: +91-22-61649598


Arpan Bhattacherjee


Arpan.Bhattacherjee@synopsys.com, Ph: +1-510-468-9009


In modern-day semiconductor failure analysis (FA), the need  for computer-aided design (CAD) has extended beyond the  sole physical layout to a much larger scope of integrated  circuit (IC) design data, such as the source schematic and  netlist.  Due to the improved accuracy of predicted failures  reported by test and diagnosis tools, it has become virtually  mandatory to correlate the potential failing schematic features (e.g., nets and instances) to their corresponding location on the  physical-CAD layout and actual device under test (DUT). This paper covers the latest advancements of utilizing IC  design schematics for fast and accurate fault localization; along with some of the most-effective methodologies for  efficient root-cause analysis.


As technology nodes continue to shrink, systematic defects due  to design-process interactions are a dominant component of  integrated circuit (IC) yield loss. Shrinking nodes have  continually increased the need for CAD-based FA techniques  to isolate defects in ICs. Electrical Fault Isolation (EFI) becomes more complex with added levels of interconnects, smaller feature sizes, and higher transistor densities in leadingnode ICs. These challenges significantly increase FA cycle  time.


There are many analytical techniques and approaches that are  implemented in semiconductor failure analysis labs. The  approach presented here utilizes design data, silicon, microscope images, and CAD Navigation (CADNav) software  to identify root causes related to the defects that have a high  impact on yield. The work in this paper primarily focuses on  the usage of circuit schematic analysis by leveraging IC design  netlist data and related tools. Depending on the type of failure, corrective action can be taken either in the design or process  phase.


The sooner root causes of IC defects can be confirmed and  corrected, the sooner the final product can reach the market.


Figure 1: Faster fault localization enables faster yield ramp


In the work presented here, Synopsys® Avalon™ CAD  navigation software is used to perform logic circuit analysis. The software uses various formats of design data to aid FA  engineers to perform analysis and debug effectively.


Figure 1: An example of ATPG Testing and Diagnosis  Implementation in FA


182


Single Shot Logic Pattern for IDDQ


The approach used in the analysis of these two failing units  combines static fault isolation techniques with using Single  Shot Logic Patterns (SSL) specifically created to allow the  analyst to analyze these IDDQ failures in more detail. SSL


patterns utilize ‘ATPG constraints’ to put the inputs of


suspected leaky/failing cell to known states and IDDQ current  is measured at each of these conditions. Circuit analysis can be  performed taking into account the calculated logic gates and the  IDDQ current measurement results.  Both the passing and  failing results are used in to further isolate the fault. Through  this, the suspect net(s) that is most probably related to the  increased IDDQ can be identified.


Take for example the 3-input XOR circuit shown below:


Output


Q


Figure 2: Schematic symbol of cell U1, which was a 3-Input  XOR (top) and its corresponding truth table (bottom)


For XOR circuits, the output was logic 1 when there was odd


number of 1’s on its inputs. Furthermore, when the input


combination at the inputs were known, the logic on internal  nodes can also be calculated.


The image below shows the calculated logic states on its


nodes when the input ABC = 001.


Figure 3: Logic state at the nodes of cell U1 when its inputs  ABC=001


If there is a leakage between two nodes, it can be detected by  IDDQ measurement when the logic between them is opposite. When they have the same logic, no current will flow through  the leakage path and IDDQ current measurement will most  probably be normal. Say for example, there was a leakage  between the Gate and Drain of transistor P7. Then, increased  IDDQ current could be measured when the internal nodes D and  E were of opposite logic (DE = 10 or 01) and normal IDDQ  current when they have similar logic (DE = 00 or 11)


Figure 4: Schematic of cell U1 showing that a leakage between  gate and drain of P7 can be detected through increased IDDQ  current when internal nodes D and E were of opposite logic


Table 1: Expected IDDQ current measurement result at  different input combinations of the 3-input XOR circuit when  there was a leakage between gate and drain of transistor P7 as  shown in Figure 4.


Combination/ SSL Pattern


Internal  Node


Internal


Node Output IDDQ  current


A B C


D


Fail


0 0 1


Pass


0 1 0


0 1 1


1 0 0


1 0 1


1 1 0


1 1 1


The results from Table 1 above show that the IDDQ current  fails when there is opposing logic between internal nodes D and  E. Among other possibilities, this could indicate a leakage  between the gate and drain of transistor P7 as shown in Figure


Using ATPG constraints to put the cell of interest to a ‘known’ state


For generating SSL patterns for IDDQ failures discussed above, we typically start with a stuck at fault model, add constraints, add faults, and manually add the IDDQ test points. ATPG  constraints can be used to set the input to a known state. For


U1


P1


P2


N1


N2


P3


P4


P5


P6


P7


P8


P9


P10


N3


N4


N5


N6


N7


N9


N8


N10


D  C


1 0


0  0


183


example, to set inputs A, B, and C of cell U1 respectively to  logic states 0, 0, and 1; constraints could set as follows:





Add a constraint to ‘0’ (c0) at input A of U1


Add a constraint to ‘0’ (c0) at input B of U1


Add a constraint to ‘1’ (c1) at input C of U1


Add stuck at fault (sa0/sa1) at output Q of U1


Figure 5: 3-Input XOR with constraints added to its input and  faults added to its output


Note that depending on the circuit, some input combinations  might not be possible due to conflicts in constraints. In such a  case, running the ATPG will not generate any pattern and will  result to a fault/test coverage of 0%. If there are no conflicts in  constraints, the ATPG pattern will generate a pattern without  any issues.


In adding stuck at fault at the output, the user has two options:


1. Compute for the output logic for each input combination  and add a corresponding stuck-at fault at the output


2. Simply add both stuck-at faults (sa0 and sa1) at the output.


Note however that option 2 will only give a maximum fault  coverage of 50% per SSL pattern. This is because a specific  input combination will result to either a logic 0 or 1 at the  output. Hence, only one out of two stuck-at fault at the output  can be covered per SSL pattern.


One IDDQ measurement per input combination alone could not  confidently distinguish between a fault on U1 or a fault on a  related but different cell. Increasing the number of times a  certain fault was detected (Ndetects) will put the other cells to  different logic values while keeping U1 to a known state (thanks to constraints). If the fault was activated by that specific  input combination of U1, then IDDQ current measurement will  always show increased IDDQ currents (compared with good). If not, it was possible that some IDDQ test points would yield  good results.


Having the required ATPG files, SSL patterns can be generated  to put the cell of interest to a known logic state using the ATPG  tool and following the related user guidelines [9][10].


General procedure for generating SSL Pattern to put the cell of  interest to a known logic state(s):


1.


Read in the ATPG-archive of the design


2.


Set fault model to Stuck-At


3.


Add constraints to put the cell of interest to a known  state


Add sa0/1 fault to output of the cell of interest


5.


Set the number of detections to a high value (say for  example 5)


Run the ATPG


Write out the pattern


8.


Remove/delete all faults, constraints, and (internal) patterns


9.


Repeat steps 3-8 for generating the next single shot  logic pattern.


10.


Manually add IDDQ test points  This was typically  added after the load operation was completed (putting  the scan chains to a known state) but before the capture  clock.


Test unit using these single shot logic patterns to measure the  IDDQ currents and analyze results:


11.


Validate the patterns by testing known good unit(s)


12.


Test the failing unit to measure the IDDQ currents and  analyze results


13.


Tabulate and analyze the results


14.


Circuit and layout analysis, and if needed, identify  next port(s) for generating new single shot logic


The pattern generated using the above conditions will test Z of  U1 using ABC = 001. This will have 10 IDDQ measurement  points. If the device fails all 10 IDDQ points, it can indicate that  the leakage was indeed related to ABC=001. If not, then it can  indicate that the fault was probably related to some other cells.


SSL patterns were generated each time using different input  combinations constraints. In each combination, multiple IDDQ  test points was generated by using a high number of detects.


Table 2: Expected IDDQ current measurement result at  different input combinations of the 3-input XOR circuit when  there was a leakage between gate and drain of transistor P7 as  shown in Figure 4.


SSL Pattern


Output IDDQ test  point  1


IDDQ  test  point


Fail Fail Fail Fail Fail


Pass  Pass  Pass Pass   Pass


Add c0


Add c1  Add c0


184


Scope and Limitation of this Technique


Without any clue or information where the fault could be  located in the digital core, it will take huge effort to try and  isolate the IDDQ fault using single shot logic patterns alone. This technique was a complementary approach to fault isolation  techniques such as Photoemission Microscopy (PEM), Optical  Beam Induced Resistance Change (OBIRCH) Microprobing, and probably also (iterative) ATPG diagnosis [3][4], Soft  Defect Localization (SDL) like Dynamic Analysis by Laser  Stimulation (DALS) [7][8].


The results from initial fault localization could yield multiple  candidates or the resolution was not enough to give high  confidence of the exact fault location. Single shot patterns could


be generated to individually test cells at specific ‘known’


conditions. Tabulate and analyze the results and based on that  the fault could be isolated further. Both the failing and passing  results could be used in performing circuit analysis based on  single shot patterns.


Starting point and Flow


Before analysis of IDDQ failures using SSL patterns could be  performed, a starting point is usually needed to identify which  cells of interest to target. The diagram below shows a possible  flow for analysis of IDDQ failure, starting from initial fault  localization, then generation of SSL patterns, followed by  testing/measurement of IDDQ failures, and finally circuit  analysis considering all results.


Figure 6: Process flow chart showing the use of SSL patterns  for further fault localization of IDDQ failures


The cases discussed hereafter followed this flow until the  information is sufficient to identify a more precise fault  location.


Both failing devices used in this case study were failing for  excessive IDDQ currents while all other ATPG patterns (Stuck  at, bridging, and transition delay) were passing. Testing on ATE  and on a compact test HW confirmed the IDDQ failure.


Table 3: IDDQ current for the different IDDQ stop points


2026 3029 4032 5035 6038 7041 8043 9047


Device


> 10* µA


0.16 µA


* Compliance set to 10 µA


With the failure mode activated (high IDDQ current), fault


localization steps like Photoemission Microscopy (PEM) and  Optical Beam Induced Resistance Change (OBIRCH) analysis  were performed. The results isolated the fault to a cell but it


was not possible to determine what particular nodes were


involved with the high IDDQ current. The authors used an


approach combining Single Shot Logic (SSL) patterns, IDDQ  measurements, and circuit analysis to identify the potential


nodes/nets responsible for the increased IDDQ current.


Device 1


Fault localization of Device 1 through PEM and OBIRCH


analysis, performed on each of the IDDQ stop vectors with  high current, isolated the fault to a small area in the digital


core.  Layout and circuit analysis identified the PEM and


OBIRCH spot to be located on a 3-input XOR cell


(exor3x2_d). However, it was not possible from the results to  determine which transistor or nodes were responsible for the  increased IDDQ current.


Figure 7: OBIRCH analysis shows a leakage path on a logic  cell in the digital core in more detail


SSL pattern


From Table 3, it was already known that the high IDDQ current  was not visible on every stop vector. Now it would be  interesting to know the condition of signal A, B and C to get  this normal IDDQ current, and in which condition the excessive  IDDQ current was observed. This was hard to know by logic  calculation and also probing on the nets running at low metal


Fault


Testing


Circuit  Analysis


Initial Fault  Localization:


- PEM


- OBIRCH


- ATPG


Diagnosis (when


applicable)


Generate SSL  patterns for  IDDQ to put  target cell to  a specific


‘known’


condition


Measure the  IDDQ


currents for  each SSL


pattern and  tabulate the  results


Perform circuit


analysis to deduce the  defect candidates. Use  both the passing and  failing IDDQ currents  in combination with


the calculated logic at  each net pairs.


185


level was difficult. For that reason, a reverse approach was  done. Special patterns were created to force only combination  of interest to those 3 signals and in the meantime the IDDQ  current was monitored. By SSL pattern generation (Single Shot  Logic pattern generation) the logic conditions of Table 4 were  forced, and for every condition, the IDDQ-current was  measured.


Table 4: Logic conditions tested by SSL pattern


SSL


A of  g46


B of  g46


C of 1676


net36


IDDQ current


>10 µA*


0.212 µA


0.073 µA


0.213 µA


Since there was no impact on the normal functionality, the logic  states were still correct and can be calculated. A gate leakage  can only be created when the gate was at a different potential  compared to the source and/or to the drain. Starting from logic  condition 1 of Table 4, there were 6 possible leakage locations  and they were indicated by          in Figure 8.


By doing the same on another logic condition, some of the  previous locations were no longer valid. Those which become  invalid were indicated by     . Doing this on a sequence of  condition 1, 2, and 3, it was clear that the leakage must be  located in the NMOS driven by net 36.


Figure 8: Finding the leakage location by deduction based on  the logic conditions with excessive leakage


Figure 9: Finding the leakage location by deduction based on  the logic condition without leakage


Device 2


Similar to Device 1, Device 2 was subjected to initial fault  localization steps. Photon emission analysis shows an emission  spot, however a higher magnification image on the location was  not possible since the emission was too weak. OBIRCH  analysis on the IDDQ current consumption points to the same  location, and this position can be captured with higher  magnification.


Figure 10: OBIRCH analysis shows leakage path on a logic cell  in the digital core in more detail


Other combination of A and B were not  interesting since they create the same  logic state on D


1: excessive leakage


Can be gate-source  Can be gate-drain


Can be gate-drain


Can be gate-drain  Can be gate-source


2: no leakage


0  1


0 1


Suspect leakage site identified!


3: no leakage


186


Layout and circuit analysis identified the OBIRCH spot to be  located on a 5-input AND-OR cell (aoi311x2_d). However, it  was not possible from the results to determine which transistor  or nodes were responsible for the increased IDDQ current. Refer to Figure 10.


From Table 3, it looks like the device has an excessive IDDQ  current for all the logic conditions, however this was not true. The 8 stop vectors in Table 3 have an excessive current but  there were many conditions in the logic pattern with a normal  IDDQ leakage.


Table 5: Vectors in IDDQ pattern with normal IDDQ current  were existing


279 283


287 291 295 299 303 307 311


Dev ice 2


0.13µA


0.071µA


0.15µA


0.07µA


0.21µA


Now it would be interesting to know the condition to get this  normal IDDQ current, and in which condition the excessive  IDDQ current was observed. This was hard to know by logic  calculation, and also probing on the nets running at low metal  level was difficult. For that reason, a reverse approach was  done. Special patterns were created to force those signals and  in the meantime the IDDQ current was monitored.


By SSL pattern generation (Single Shot Logic pattern  generation), the logic conditions of Table 6 were forced and for  every condition the IDDQ-current was measured.


Table 6: Logic state conditions tested using SSL pattern


SSL A of  1676


B of  1676


C of  1676


D of  1676


E of  1676


IDDQ  current


> 10 µA*


0.209µA


Since there was no impact on the normal functionality, the  logic levels were still correct and can be calculated. A gate  leakage can only be created when the gate is at a different


potential compared to the source and/or to the drain. Starting  from logic condition 2 in Table 6, there were 9 possible


leakage locations and they were indicated by          in Figure


By doing the same on another logic condition, some of the  previous locations were no longer valid. These that become  invalid were indicated by          . Doing this on a sequence of  condition 2, 5, 8 and 7, it was clear that the leakage must be  located in the PMOS driven by signal E.


Figure 11: Finding the leakage location by deduction based on  the logic conditions with excessive leakage


187


Finally, it can be deduced that the leakage must be between


source and drain. Since the logic condition 3 of Table 6 has no  leakage, it was even possible to narrow down to a gate to


source leakage on MP0 or a gate to drain leakage on PMOS_3.


Figure 12: finding the leakage location by deduction based on  the logic condition without leakage


FIB cross sectioning


Focused Ion Beam (FIB) cross sectioning of the suspected  PMOS transistors showed that the gate to drain leakage path  on PMOS_3 which was created by a poly stringer.


Figure 13: FIB cross sectioning result. Arrow point to the to the  poly stringer


The device discussed here in Case Study 2 is failing only for  IDDQ while all other ATPG patterns are passing. Fault  localization through PEM analysis showed no obvious  anomalies but OBIRCH analysis isolated the suspected leakage  site to a small area in the digital core.


Figure 14: OBIRCH analysis results isolating the potential  fault location to filter capacitor or the 4-input OR gate


However, it was not clear from the result whether the leakage  is at the output stage of the 4-input OR gate, at the filter  capacitor, or between them.


The assumptions used to isolate the fault further is as follows:  The filter capacitor is connected to VDD and VSS, If the  leakage is at this capacitor, the leakage current remains the  same regardless of the logic condition of the 4-input OR  gate


PMOS_3


MPO


188


 If the leakage is at the output stage of the 4-input OR gate (inverter), then specific logic input combination will result


to a change in the leakage current


 If the leakage is in between the filter capacitor and OR gate, then the leakage will be affected by the output Q logic of


the OR gate


Figure 15: Circuit schematic showing the possible fault  locations


To isolate the fault further, SSL patterns were generated to put  the 4-input OR gate to ‘known’ logic states and IDDQ currents  are measured at each of these conditions. The circuit around this  OR gate only allowed for the following possible input  combinations due to conflict in constraints.


Table 7: SSL patterns generated and IDDQ measurement  results


S S L


IN


OUT IDDQ test  point  1


Average  IDDQ  Current


A B C D Q


1 0 0 0 0 0


4.21 µA


4.15 µA


4.18 µA


4.09 µA


4.12 µA


2 1 0 0 0 1


4.46 µA


4.49 µA


4.40 µA


4.45 µA


3 0 1 0 0 1


4.55 µA


4.37  uA


4.52 µA


4.43 µA


4.48 µA


4 0 0 1 0 1


4,52 µA


4.39 µA


4.47 µA


5 0 0 0 1 1


The average IDDQ current on a known good unit, using the  same SSL patterns in Table 7, is between 0.4 to 0.6 µA. The  currents measured on the reject unit were significantly higher  than the known good unit. The reject unit was observed to be  failing all IDDQ test points in all SSL patterns used.


SSL pattern # 1 (ABCD = ‘0000’; Q = ‘0’) resulted to an IDDQ  current of 4.2 µA. SSL pattern #’s 2 – 5 (ABCD = ‘1000’, ‘0100’, ‘0010’ and ‘0001’; Q = ‘1’) resulted to a slightly higher  IDDQ current of about 4.5 µA. By circuit analysis based on  these SSL patterns and IDDQ measurement results, the possible


faults causing the increased IDDQ current could be deduced as  follows:


Table 8: Possible Faults and their probability based on the  IDDQ measurement results using SSL patterns


Possible Fault


Probability Rationale


Leakage on filter  capacitor C1


Less


probable


A leakage on capapcitor C1  will not be affected by the  logic states on the 4-input  OR gate.


There is a slight but  consistent difference in the  IDDQ current using SSL  pattern #1 with using SSL  patterns #’s 2-5.


Leakage on the  output


stage (inverter) of the 4-input OR gate (G2649)


Most


The IDDQ measurement  results per SSL pattern  correlate with a possible  leakage between the input  and output of the inverter at  the output stage of G2649. See Table 7 and Figure 16.


Leakage between  the filter C1  capacitor and output  Q of the 4-input OR  gate (G2649)


The gate of capacitor C1 is  connected to VSS. IDDQ  current is observed to be  failing regardless of the  logic at the output Q of  G2649. This measurement  do not fit with when the  leakage is between capacitor  C1 and the output of G2649.


Figure 16: IDDQ current path assuming leakage between the  input (QN) and output (Q) of inverter at output stage of G2649  cell. A slightly lower IDDQ current when ABCD = ‘0000’ could  be explained by the higher resistance due to the four PMOS  connected in series.


The unit was subjected to parallel lapping until MET2 is  removed but there is still remaining oxide on top or MET1. High magnification optical inspection showed a possible


QN


D  C  B  A


B  C


VDD


C1


G2649 (OR4X2)


FILCAP


IDDQ current  path when


ABCD = ‘0000’


ABCD = ‘0001’


B  C  D


189


anomaly between the two identified MET1 tracks, between the  input and output of the inverter cell of the OR gate.


Figure 17: Optical inspection after parallel lapping to MET1  layer. Arrow points to a possible anomaly between or below Q  and QN.


Construction analysis was performed by progressive FIB crosssectioning towards the possible anomaly. The results found a  particle below MET1, at and above the poly level was observed. EDX analysis of the anomaly showed peaks of Iron (Fe), Nickel (Ni), and Chromium (Cr).


Figure 18: Top image: FIB cross-sectioning revealed particle  affecting the polysilicon and MET1 (Q and QN node) at the  output stage of the 4-Input OR gate (G2649).


Bottom image: EDX analysis of the particle showed that it is a  metallic particle, showing peaks of Iron (Fe), Nickel (Ni) and  Chromium (Cr)


This paper have successfully demonstrated a new approach for  further fault localization of IDDQ failures by using Single Shot  Logic (SSL) patterns.


The purpose of using SSL patterns is to put the area/cell of  interest to a ‘specific/known logic state’ and target a specific  fault. One SSL pattern is written out for each possible logic state  combination. Increasing the number of times the target fault is  detected allowed more IDDQ test points per SSL pattern, increasing the resolution. Multiple SSL patterns could be  generated to cover the different possible logic state  combinations. Since the logic states are known, further fault  localization can be performed by circuit analysis based on the ‘known logic states’ and IDDQ measurement results.


As shown in the case studies discussed in this paper, it was  possible with this approach to determine the suspect nets  causing the increased IDDQ current, leading to a more precise  and successful determination of root cause.


Outlook


In this paper, SSL pattern was combined with IDDQ  measurements and circuit analysis that allowed the analyst to  perform logic analysis to further isolate the fault. The authors  believe that single shot patterns can also be combined with  laser-based probing techniques like Electro-Optical Probing (EOP) and Laser Voltage Probing (LVP) [11][12][13] or other  analysis where it is needed or helpful to put a specific cell/net  to a known state.


Single shot logic patterns could be generated to test the net/port  of interest for a certain fault. Additionally, other nets could be  constrained and therefore put certain cell, nets, or ports to a  known state where possible. Having known this, interpreting  the analysis results could be made simpler as compared to not  being able to control the net/port or at least know their logic  states. The logic states at ports of cells at a specific cycle could  be determined using digital design simulation tools which will  not be discussed on this paper. However, controlling a specific  net could only be obtained by either targeting a specific fault or  using constraints, and their combination. This is the idea behind  generating Single Shot Logic patterns.


Furthermore, as the technology size continues to shrink, laser  based probing and other techniques were reaching their  limitation whereas ATPG diagnosis and use of single shot logic  patterns is not necessarily affected by it. It was therefore  essential that this technique could be used to help bridge that  gap in fault isolation.


The authors would like to acknowledge our global Product  Analysis Lab management, Mark Morris and Pascal  Vercruysse, for the continued support and encouragement. We  would like to thank Eric Barbian for the trainings and his  invaluable inputs for this paper. The ON Semiconductor Global  Failure Analysis teams for the invaluable contributions towards  FA capability improvements. We would like to acknowledge  our Material Analysis (MA) and Technology and  Characterization Lab (TACL) teams for their support in the  sample preparation and material analysis of these cases. We  would like to thank our Design Engineering Centers and  Product Engineering for facilitating and providing the ATPG  files needed to allow the global failure analysis teams to  perform ATPG testing, diagnosis, and create targeted patterns  including single shot logic patterns. This paper was only a small  portion of the improvement efforts that our teams were  continuously striving to increase our analytical capability.


[1] R. Estores, E. Barbian, “Single Shot Logic Patterns:


Increasing Diagnostic Resolution of Logic Failures


Utilizing Single Fault Targeting and Constraints” ISTFA


[2] R. Estores, E. Barbian, P. Vercruysse, K. Villareal, R. Sanchez, R. Ackerman, “Failure Analysis Enhancement by  Incorporating a Compact Scan Diagnosis System” ISTFA


[3] E. Barbian, R. Estores, “ATPG Testing and Diagnosis


Implementation in FA for a Fast and Efficient Iterative


ATPG Diagnosis and Fault Isolation” ISTFA 2017.


[4] K Gearhardt, C Schuermyer, R Guo, "Improving fault  isolation using iterative diagnosis", Proc. of International


Symposium for Testing and Failure Analysis, pages 390-395, 2008.


[5] J. Koltzer, et al., “Quantitative Emission Microscopy,” J. Applied Physics, 71 (11), pp. R23-R41, June 1992.


[6] K. Nikawa, "Optical beam induced resistance change (OBIRCH): Overview and recent results," Proc. 16th


Annual Meeting IEEE Lasers and Electro-Optics Society (LEOS), Tucson, AZ, 2003, vol. 2, pp. 742-743.


[7] Bruce, M. et al., “Soft Defect Localization (SDL) on  ICs.” ISTFA 2002, pp. 21-27.


[8] Seah, Y. et al., “Applications of Soft Defect Localization (SDL) on AMD Advanced SOI Microprocessors.” ISTFA


2006, pp. 311-315.


[9] ‘‘Synopsys TetraMAX ATPG User Guide” Version Version  N-2017.09-SP3


[10] ‘‘Mentor Graphics ATPG and Failure Diagnosis Tools  Reference Manual” Version 2015.4


[11] U Kindereit, G Woods, Tian Jing, U Kerst, R Leihkauf, C  Boit, Device and Matl Rel, "Quantitative investigation of


laser beam modulation in electrically active devices as used


in laser voltage probing", IEEE, Vol 7, Issue 1, pg 19-30,


2007.


[12] W. M. Yee, "Laser voltage probe (LVP): A novel optical


probing technology for flip-chip packaged


microprocessors", Proc. IEEE 7th IPFA, pp. 15-20, 1999


[13] C. He, H. Zhang, J. Song, P. Tian, and W. Wang, “Study


and application on thermal eop (electro optical probing) /


eofm (electro optical frequency mapping) technique,”


2018 IEEE International Symposium on the Physical and


Failure Analysis of Integrated Circuits (IPFA), pp. 1–4,


191


# Comparison of He+ and Ga+ voltage contrast in N-wells


Comparison of He+ and Ga+ voltage contrast in N-wells


Gregory M. Johnson, David Ferranti, John Notte, Brett Lewis, Chris H. Park, Ted Lundquist, Baohua Niu


Carl Zeiss PCS,


Pleasanton CA, Peabody, MA


greg.johnson@zeiss.com


The examination of partially deprocessed ICs for well imaging  has been investigated.  First it has been shown [1] that Ga+ FIB  imaging can readily and strongly highlight the N-well / P-well  boundary in an IC as shown again here. Second, a model  which only considers secondary electron creation and  scattering [2] is confirmed to be sufficient for understanding  these imaging effects. Heavy Ga doping provides no marked  change in PVC (passive voltage contrast).  Then comparisons  in the same field of view between optimized He+ and Ga+ imaging, has shown that He+ provides much greater PVC  contrast when looking through deep oxide, and much better  resolution on shallow surfaces. The quantitative model  Stopping and Range of Ions in Matter (SRIM) [3] was  consulted and confirmed these expectations for resolution and  depth superiority of the He+ beam.  According to the SRIM, there may even be less damage from the He+ beam.  Yet these  known effects of Ga+ damage has not prevented its widespread  use in semiconductor FA and process monitoring.   Thus, the  use of GFIS (Gas field ion source) He+ beam for voltage  contrast and junction imaging warrants further exploration.


As semiconductor processing advances to smaller technology  nodes, the inherent scaling challenges to be overcome include  junction engineering [3]. Thus, it is useful to have rapid and  accurate ways to characterize alignment and quality of  junctions in ICs.  Electron-beam and Ga+ FIB inspections are  well known [2]; Helium GFIS FIB inspection is relatively new  to the field of failure analysis and process monitoring [3]. This  paper investigates the usefulness of He+ FIB for certain  applications involving passive voltage contrast and  demonstrates some unique advantages.


PVC MECHANISM


The mechanism for passive voltage contrast of p/n junctions is  well-known. A p/n junction has a built-in, or electrostatic  potential, as shown in Figure 1.  When a particle such as an  electron interacts with an IC, creating electron hole pairs, the  net positive charge on the N-side increases the work function  for secondary electrons to leave the IC: hence N-type material  is dark in a charge particle instrument.


Figure 1.  Diagrams of the charge, field and voltage of a p-n  junction. The N-doped side of a junction has a net positive  charge due to the flow of majority carriers to the P-side.


Figure 2. Model for passive voltage contrast in an IC with a  P-N junction buried under a thin layer of dielectric. The negative p side either provides no barrier to the escape of secondaries, or may actually aid in their escape by providing a replusive force. The positive n side attracts or captures secondaries, thus making the N side darker.


This mechanism, depicted in Figure 2, shows the case of an IC  where there are tens of nm of oxide above the junction.  Here, the cloud of secondary electrons (recoil and cascade) in the  oxide may provide the strongest drive for voltage contrast.


This model is still valid for the use of metal ion FIB species, as  these species create secondary electrons. Alternative theories  for metal-ion FIB PVC may suggest that a field is set up in the  oxide/dielectric. Or that charges on the oxide surface itself


192


interact with the impinging particle. In either of these  alternative models it seems that extreme doses of a metal ion, especially one like Ga known to be a p-type dopant, would  quickly wreck an IC’s ability to provide PVC [4].


PVC as FUNCTION OF Ga+ DOSE


To test these models, a 22 nm bulk technology IC was  delayered by mechanical polishing to an arbitrary depth below  the gates. At such a depth, the only features existing on the top  surface are active fins and STI oxide. This surface was then  scanned with a 30kV, 66 pA, 50 μs/pixel Ga+ beam across a 6 μm field of view with 1024 pixels. The results of the  secondary electron imaging from such a scan are shown in  Figure 3a. The sausage-shaped features are fins that have  broken the surface. The dark bands running upward left to  right in the IC indicate the N-wells (NW) underneath the  oxide.  This result demonstrates that (with an arbitrary depth of  oxide above the silicon), that Ga+ FIB can provide a very  strong PVC effect for N-well / P-well distinction.


Figure 3.  Ga+ FIB imaging of one field of view with three, consecutive, relatively long 50 μs pixel scans.  a) one scan; b) two scans c) three scans. The dark bands running upward left  to right in the IC are the NWs, which are buried underneath  oxide. Note that there is relatively no change in NW/PW PVC  even with such an heavy dose.


Considering the Figures 3b and 3c, we see the effect from two  additional, heavy doses of Ga+. While there is some evidence  of mechanical damage to the IC (sausages getting darker), there was no let-up to the strength of the PVC effect.  Thus, any model for metal-ion PVC that requires “doping” or “surface charge accumulation” appears invalid.  The IC has  been imaged to the point of physical damage, and any doping  or surface charge effect should likely have been swamped out. This provides a very strong indication that the simple, secondary-electron model of Figure 2 is at play in metal ion  PVC. This model is the basis of our later discussion.  These


193


results should eliminate worries about the experimental  technique, such as the ion beam scanning a surface first.


PVC COMPARISON: Ga+ vs. He+


A field of view from the same IC was now imaged by both He+ and Ga+ FIB in a NanoFab. Again, we have chosen an  arbitrary but shallow plane in the IC, where only features  present should be shallow trench oxide and fins. The  conditions for the two beams are: Ga+, 30kV, 6 pA, 5 μ s/pixel  Ga+ beam across a 2.5 um, 1024-pixel field of view; and He+, 30kV, 2 pA, 50 μs/pixel He+ beam across a 2.5 μm, 1024-pixel  field of view. The SEI results are shown in Figure 4. It is very  clear that the dark bands in the IC are cases where the N-well  shape underneath the oxide is revealed with PVC.


Figure 4. SEI images from the same field of view with imaging  by both Ga+ (left) and He+ (right) beams at 30kV.  Contrast is  very high in both cases.


Figure 5 further explains the contrast mechanisms seen in this  effect.  The sample has been polished to just below the gates  and is therefore imaged through the STI oxide.  The NW and  PW regions show up in PVC.


Figure 5. Comparison of SEI (left) with He+ beam with crosssectional interpretation (right). The PVC effect here strongly  delineates PW and NW regions through the STI.


The resolution of the features in general are much greater for  the He+ beam.  If one wants to check the alignment of N-well  to the fins, it’s largely impossible in the Ga+ case.  The  resolution of the He+ beam, however provides a very strong  contrast, as shown in Figure 6. Some overlay error is observed.


Figure 6. Blowup of Ga+ (left) and He+ (right) imaging from  Figure 4. It is very easy to measure the relative overlay error  in the He-imaged IC compared to that in the Ga+ sample.


DEEP OXIDE SAMPLE ICs


Next, an area in the IC was carefully chosen such the local  area of polish was exactly at the bottom of the gates. Here, the  STI is expected to be roughly 100 nm.  Figure 7 shows Ga+ vs. He imaging of the same field of view, using the same imaging  conditions as before. Once again, the He+ image (right) shows  a very strong voltage contrast distinction between the NW and  PW buried features of the IC. The Ga+ image does not show  this, even with extreme tweaking of the contrast in an imageediting program.  The He+ image also provides very high  resolution to clearly show the gates in the IC. The same effect  is shown even more strongly in an SRAM area in Figure 7.


Figure 7. Comparison of He+ and Ga+ imaging of the same  area, one chosen precisely underneath the gates. Strong PVC  is seen in the He+ case but is lost in the Ga+ one. The He+ image has such good resolution that one can see the remnants  of gate present over the tops of the fins but not seen with Ga+.


194


Figure 8. Comparison of He+ and Ga+ imaging of SRAMs, delayered to just underneath the gate. In the Helium image, the NW shape is clearly visible through from the NW contacts  into the array.


SRIM MODELING


The effect of He+ and Ga+ beams were then studied using the


“Stopping and Range of Ions in Matter” computer model, as


depicted in Figure 9. The simulation was run for ten minutes  using standard parameters. The Ga+ beam has two effects  which are detrimental to the purpose of this paper:  wider  cascade and shallower effect. The He+ beam, meanwhile  provides for a much narrower beam, and maintains this effect  relatively deep into the IC.  These two effects exactly predict  our results in Figures 4 (better He+ resolution) and 7 (better  He+ depth).  Quantitative results of the SRIM program are  shown in Table 1.  Here we have some indication of the type  and magnitude of mechanical damage to the IC from these two  beams.  The Ga+ beam has a greater sputter yield and greater  number of vacancies created per incident ion. The vacancies


created are typically a “Frenkel” defect where an atom is


dislodged out of its lattice position, to create an interstitial  somewhere else in the matrix. Thus, for identical imaging  conditions, the He+ will damage the IC less. The one caution is  that the physical effects of the He+ beam occur at a much  deeper depth, and so it may be less immediately noticeable if  one were less careful with the techniques.


Figure 9. Top: Comparison of the impact of similar Ga+ and  He+ beams using the SRIM program across a very large scale, showing recoil & cascade secondaries, as well as atom  disturbance.  The Ga+ beam provides a response that is much  wider and shallower compared to the He+ beam. Bottom: expanded view in the top 20 nm of oxide.


Table 1. Quantitative view of the SRIM results from Figure 8. For equivalent conditions, the He+ beam may be less  damaging, in terms of both sputter yield and vacancies  created per incident ion.


ENERGY LOSS


The projected path of the recoiled ions through the material, however, do not provide a fully satisfying explanation as to  why there may be such a great difference between the Ga+ and  He+ effects.  Next, a calculation of the energy loss, expressed


in eV/Angstrom of travel, were compared.  These figures are  plotted by SRIM in Figure 10.  It is clear that within the  typical depth of STI in a sample, the He+ beam is losing most  of its energy due to ionization events, whereas the Ga+ is  losing energy due to recoils. While it is possible that the recoil  events themselves could create secondaries, the He+ beam has  a significant advantage in terms of the creation of secondaries, which are used for imaging. The secondary electron escape  depth has been cited as high as 20 nm for insulators and  semiconductors [7].


Figure 10. Comparison of energy loss profiles between Ga+ and He+ beams. The He+ beam loses most of its energy in the  creation of ions, here interpreted to be secondary electrons.


Electron beam Comparison


Similar fields of view, with chips mechanically polished to just  under the gate, were next imaged with a SEM beam with  different primary energies.  These images are shown in Figure


11. It is apparent that the effective PVC of the electron beam reaches a maximum of around 5 kV but decreases with increasing potential.  Figure 12 compares the relative particle traces for each of the beams in this study.


Figure 11.  Comparison of contrast by SEI imaging of similar  areas in a delayered chip with increasing acceleration  potential. The N-wells are delineated most strongly at 5 kV, with a decreasing effect at higher kV’s.


195


Figure 12. Comparison of SRIM data for Ga+ and He+ beams against electron beams of 1, 2, and 5 kV.


The examination of partially deprocessed ICs for well imaging  was investigated with both Ga+ and He+. First it was shown  that Ga+ FIB imaging can strongly highlight the N-well / Pwell boundary in an IC with relative ease. Next the model  which only considers secondary electron creation and  scattering was shown to be good enough for imaging and  heavy Ga+ doping and did provide a marked change in the  PVC effect.  Then, comparison of the same field of view with  optimal He+ and Ga+ imaging showed that He+ provides much  greater PVC contrast when looking through deep oxide, and  much better resolution at shallow surfaces.  The SRIM model  agreed with these findings for resolution and depth superiority  of the He+ beam.  According to SRIM, there may even be less  damage from the He+ beam.  The known effects of Ga+ damage has not prevented its widespread use in semiconductor  FA and process monitoring.  The use of GFIS He+ beam for  passive voltage contrast and junction imaging warrants further  exploration.  The electron beam results further validate the  theory that primary beam interaction with the buried layer is a  key component of this mechanism.


The help of Sean Kenny and David Dryden in acquiring, delayering, and some initial imaging of these ICs is greatly  appreciated.


[1] C. Boit, K. Wirth, E. Le Roy, "Voltage Contrast like Imaging of N-Wells", ISTFA 2003


[2] Rosenkranz, Rüdiger. (2011). Failure localization with active and passive voltage contrast in FIB and SEM.


Journal of Materials Science-materials in Electronics - J MATER SCI-MATER ELECTRON. 22. J.F. Ziegler,M.D. Ziegler, J.P. Biersack, “SRIM – The Stopping and Range of Ions in Matter,” Nuclear Instruments and Methods in Physics Research B, vol. 268(11-12), pp.


1818-1823, 2010.


[3] R. Livengood, M. Grumski, Y. Greenzweig, T. Liang, R.


Jamison, Q. Xie, "Helium ion microscope invasiveness study and novel imaging analysis for semiconductor applications," Proceedings of the Seventh International Conference on Charged Particle Optics


[4] G Johnson, J Nxumalo, A Arya, J Johnson, Q Gao,"Innovative use of FA techniques SCM and OBIRCH


196


along with TCAD to resolve junction scaling issues at  advanced technology nodes", ASMC 2018


[5] Marshall Brain, "How Semiconductors Work," https://electronics.howstuffworks.com/diode1.htm,


accessed on 8/9/2019


[6] Ang, G. B.; Hua, Y.N.; Loh, S. K.; Yogaspari; Redkar, S.,"Application of passive voltage contrast and focused ion beam on failure analysis of metal via defect in wafer fabrication," Physical and Failure Analysis of Integrated Circuits, 2001. IPFA 2001. Proceedings of the 2001 8th International Symposium on the , vol., no., pp.107,111,2001


[7] "SRIM - The Stopping and Range of Ions in Solids",application based on  J. P. Biersack and L. Haggmark,Nucl. Instr. and Meth., vol. 174, 257, 1980, and J. F.


Ziegler  "The Stopping and Range of Ions in Matter",volumes 2 - 6, Pergamon Press, 1977-1985


[8] R. E. Simon and B. F. Williams, "Secondary-Electron Emission," in IEEE Transactions on Nuclear Science, vol.


15, no. 3, pp. 167-170, June 1968


[9] A. Chee, "A comparison of donor mapping techniques using the scanning helium ion microscope and scanning electron microscope," 2014 12th IEEE International Conference on Solid-State and Integrated Circuit Technology (ICSICT), Guilin, 2014, pp. 1-3


[10] monte CArlo SImulation of electroN trajectory in sOlids,Casino Version 3.3.0.4, 2016, by D. Drouin, A. Couture,D. Joly, N. Poirier-Demers, and H. Demers.


# Failure analysis of FinFET circuitry at GHz speeds using voltage-contrast and stroboscopic techniques on a scanning electron mic


Failure analysis of FinFET circuitry at GHz speeds using voltage-contrast and  stroboscopic techniques on a scanning electron microscope


James Vickers(1), Seema Somani(1), Blake Freeman(1), Pete Carleson(2) Lubomír Tůma(3), Marek Unčovský(3), Petr Hlavenka(3)


We report on using the voltage-contrast mechanism of a  scanning electron microscope to probe electrical waveforms  on FinFET transistors that are located within active integrated  circuits. The FinFET devices are accessed from the backside  of the integrated circuit, enabling electrical activity on any  transistor within a working device to be probed. We  demonstrate gigahertz-bandwidth probing at 10-nm resolution  using a stroboscopic pulsed electron source.


There is an unmet need for performing failure analysis (FA) with high spatial and temporal resolution on integrated circuits (ICs) having 10-nm or smaller feature sizes. The current  generation of FA tools employs optical techniques to localize  defects in the design or manufacture of ICs, yet minimum IC  feature sizes have become too small to be resolved optically. As a result, a transition from optical imaging to imaging using  a scanning electron microscope (SEM) appears warranted [1,2,3]. This paper addresses whether a SEM-based FA tool  can – in addition to achieving high spatial resolution – also  enable high-bandwidth waveform measurements from active  modern IC devices. A challenge along this path is that the  temporal bandwidth of secondary-electron detectors (SEDs) used with SEMs is typically limited to 10 MHz, which  necessitates a non-standard solution to meet the high-temporal  resolution demanded by the FA community.


We present preliminary results of a stroboscopic technique  where the electron beam is chopped using a standard  electrostatic beam blanker, and we demonstrate subnanosecond electron pulses having high spatial resolution  using this technique. Separate work by Meuret et al. [4] demonstrates that this blanker technology can be extended to  produce 25-ps FWHM electron pulses, which if successful in  our application, could provide a roadmap to 10 GHz e-beam  probing. For this work e-beam pulses from the standard  blanker are synchronized with the test voltage pattern applied  to the device under test (DUT). Results using this method to  measure voltage contrast of a periodic clock signal on  relatively large (micron-scale) metallic test structures achieved  a bandwidth of approximately 1.6 GHz. To measure nonperiodic arbitrary waveforms, however, we implemented a  pulse-on-demand blanking method where only one electronbeam pulse per test cycle was allowed through the SEM. Using this method we measured waveforms directly from 14-nm FinFET transistors from backside silicon, as well as from a  high-bandwidth copper microstrip transmission line. Results  from the FinFET transistors appeared to show a bandwidth of  approximately 300 MHz, though it is likely our results were  impacted by our test setup, which was not designed for highspeed operation. Results from probing the transmission line, which was designed for high-speed operation, show 500 ps  full rise times, suggesting the system is capable of 1 GHz  performance.


Measurement Technique


We use an electrostatic beam blanker placed at a beam  crossover location within the SEM source to chop the electron  beam for our stroboscopic measurements. This blanker  comprises two parallel plates that can be driven differentially  to create an electric field perpendicular to the beam axis. When no field is applied between the plates, the beam passes  undeflected through the blanker, proceeds from the blanker  through an on-axis beam aperture placed further down-column  towards the DUT, and becomes focused by the SEM into a  small spot on the DUT; this represents the normal operating  mode of the SEM. To blank the electron beam, an electric  field is applied between the blanker plates, which deflects the  beam off axis, preventing the beam from passing through the  aperture and reaching the DUT. Depending on the electronics  driving the beam blanker, it is possible to create electron  pulses on demand, or to create periodic stroboscopic electron  pulses. For pulse-on-demand, we drive the beam blanker  plates at equal and opposite polarities, with an amplitude  sufficient to fully blank the beam, and we create on-demand  electron pulses by reversing the polarities of the beam blanker  plates. Using this technique, the beam blanker only passes  electrons through to the DUT while the electric field within  the blanker is sufficiently close to zero during its transition. For the periodic stroboscopic pulses, we drive the blanker  with a purely sinusoidal electric field (i.e. one having no DC  electric field across the plates) with the result that pulses of  electrons uniformly spaced in time pass through to the DUT  during the zero-field crossings of the sinusoidal driving field, which occurs at twice the frequency of the driving sinusoid.


197


This stroboscopic beam-blanking technique is illustrated in  Fig. 1.


To measure signal waveforms from a DUT at frequencies well  below the bandwidth of the SED (typically 5 to 10 MHz), it is  sufficient to direct a continuous electron-beam probe current  to the DUT, and to average repeated measurements of the  SED output signal. However, to measure signal waveforms at  or above the bandwidth of the SED, it is necessary to  implement a stroboscopic technique where the system  bandwidth limitation no longer depends on the SED  bandwidth, but instead depends on the stroboscopic e-beam  pulse-width duration, as well as on the timing jitter involved  in synchronizing the pulses to the DUT waveform.


To measure high-frequency signal waveforms (i.e. at  frequencies above the SED bandwidth) using the voltagecontrast feature of a SEM, we have implemented two forms of  stroboscopic electron illumination: 1) for periodic waveforms  such as clock signals, we use the stroboscopic beam blanking  technique, and we synchronize the electron pulse frequency  and the waveform frequency such that the difference between  the electron pulse frequency and the waveform frequency is  within the bandwidth of the SED; 2) for arbitrary waveforms  such as data streams, we synchronize our pulse-on-demand  electron source to a trigger of the arbitrary waveform, then  slowly walk the electron pulses (one pulse per trigger) across  successive repetitions of the arbitrary waveform. The voltagecontrast mechanism used to detect the DUT waveforms has  low sensitivity, and many repetitive measurements are  typically required to reproduce a DUT waveform with  adequate (for instance, greater than 3:1) signal-to-noise ratio. We will present results characterizing the voltage-contrast  mechanism when probing FinFETs from the substrate-side of  the DUT.


Figure 2 illustrates the process of measuring periodic waveforms using stroboscopic electron illumination as described in  the first method of the preceding paragraph. Shown is a DUT  waveform, that repeats at a 150 MHz rate, with the beam  blanker plates driven differentially – one plate at a 0-degree  phase angle and the other at a 180-degree phase angle – with a  75 MHz sinusoid. Driving the blanker plates with a 75 MHz  frequency produces a uniform train of electron pulses at a  150 MHz rate, and if the DUT waveform and the blanker  waveform are phase locked to a common reference frequency, the electron pulses remain locked in time relative to the DUT  waveform being probed. In this case since the electrons  always probe the same potential on the DUT waveform, a  SED reproduces the voltage contrast at that one time instant of  the DUT waveform. To scan temporally across the DUT  waveform, the driving frequency applied to the blanker plates  is re-programmed to a nearby frequency. For instance, if the  blanker frequency is set to 74.99 MHz, electron pulses will be  produced at 149.98 MHz, and the electron pulses will advance  in time through successive DUT waveforms, sampling  complete periods of the DUT waveform at the difference  frequency of 20 kHz. In this example, it will take 50 µs for the  electron pulses to advance across one period of the periodic  DUT waveform signal, during which time it will have  sampled 7500 successive waveforms to reproduce a single  period of the DUT waveform. Such oversampling can have a  side benefit of obtaining better SNR in the resulting  measurement due to the many (7500 in this example) samplings of a single period of the DUT waveform. Capturing  this SED output will record a complete period of the DUT  waveform, which repeats at 150 MHz, at a slower rate of 20  kHz. Averaging the SED output signal with this 20 kHz  repetition rate will eventually capture a high signal-to-noise  inverted copy of the periodic DUT waveform.


A third technique is useful for locating transistors that are  switching at a fixed frequency (for instance, the chip’s clock  frequency) within a region of interest. We accomplish this  using a technique analogous to Laser Voltage Imaging [Kimball et al., 5] on optical diagnostic tools, which we have  called eLVI to evoke its similarity to the generally-known  Laser Voltage Imaging (LVI) technique. This same technique  is equivalent to Electron-beam Signal Image Mapping  disclosed in Tong et al. [6] In its simplest form, the technique  scans a continuous e-beam over a region of interest of a DUT  while the DUT is clocked at a fixed frequency below the  bandwidth of the SED. The clock frequency and the SED  signal are fed into a lock-in amplifier, and whenever the ebeam strikes a portion of the DUT where the potential is  changing at the clock frequency, the lock-in detects this  frequency in the SED signal. Simultaneously recording, in two


198


Figure 1: Beam blanker operation through sinusoidal beamblanker deflection. Shown in blue is a sinusoidal potential  applied to the left plate of the beam blanker, and in yellow, the same signal with opposite polarity applied to the right  plate of the beam blanker. Near the zero crossings of the sinusoids, which occur at twice the frequency of the sinusoid  itself, electrons are undeflected and can pass through the  beam aperture to strike the DUT. Otherwise the field across  the beam blanker deflects the source electrons laterally, causing them to strike the aperture and preventing the beam from  reaching the DUT.


image arrays, both the SED signal (DUT SEM image) and  lock-in output (clock activity image) allows for the easy  determination of active locations within the chip to probe. This technique also finds use during the final stages of DUT  preparation as an indication that sufficient backside silicon  material has been removed from a DUT to enable e-beam  probing. While the method described requires clocking the  DUT at relatively low frequencies (up to a few MHz) as  constrained by the SED bandwidth limit, it is also possible to  detect clock frequencies much high than the SED bandwidth  limit by scanning a chopped e-beam in place of a continuous  e-beam, and performing the lock-in at the difference  frequency between the DUT clock and e-beam chopping  frequencies, as described in the previous paragraph.


DUT Preparation


For flip-chip packaged devices the active layer resides  underneath a thick silicon substrate, and the silicon substrate  requires thinning to allow for the interaction of incident  electrons with active circuitry, which is required to detect  voltage contrast through secondary electron imaging. We have  developed a proprietary method using mechanical polishing of  the DUT to remove most of the substrate material; the  remaining material is removed using a plasma-derived  focused-ion beam to locally thin the substrate. The thinning  process ceases at a critical level such that circuits on the DUT  remain operational, yet enough backside material has been  removed for the optimal detection of the secondary-electron  voltage-contrast signals from the switching devices on the  DUT. See Schlangen [7] for ion-based preparation techniques.


Experimental Setup


Shown in Fig. 3 is the Thermo Fisher Scientific Helios G4  small dual plasma- and electron-beam system used to make  our initial measurements. Also shown are two signal


generators used for making the periodic-waveform  measurements detailed in Fig. 2 – one a dual-generator to  drive the blanker plates, the other a single-generator to drive  the DUT – and a sampling oscilloscope to record the SED  output signal. Although not visible in the image, the signal  generators are phase-locked to a common clock source using  rear-panel connectors. The SED is a standard through-lens  detector comprising a scintillator to convert secondary  electrons into photons, and a photomultiplier tube (PMT) to  convert those photons into electrical pulses. To achieve high  spatial resolution, we operate our Helios SEM system in its  magnetic immersion mode where, depending on the beam  current we choose, we can achieve imaging spatial resolution  below a few nanometers. The system of Fig. 3 was used for  our proof-of-concept measurement, but due to speed  limitations of the signal generators shown, we were limited to  probing a DUT signal operating at a maximum frequency of  150 MHz with this setup.


A refinement used two radio frequency (RF) signal generators  in place of the signal generators shown in Fig. 3, also phase  locked to each other, with one driving the two plates of the  electrostatic beam blanker through a single-ended to balanced  differential-output RF transformer, and the other driving the  DUT. Using this configuration, and the standard Helios beam  blanker that was not designed for high-speed blanking, we  were able to record signals from a metal trace up to 2 GHz, with a 3-dB bandwidth of approximately 1.6 GHz.


Our third refinement enabled pulse-on-demand e-beam  measurements, which we used to measure arbitrary pulse  waveforms on a DUT. For this we drove each plate of the  beam blanker with outputs from a differential logic chip. With  the logic chip output in its steady state, one beam blanker  plate is at a logic-high potential, while the other is at a logiclow potential, resulting in a blanked beam where no current  reaches the DUT. Only during the switching transition of the  logic chip, when one output transitions from high to low while  the other output transitions from low to high, would a pulse of


199


Figure 2: Illustration of synchronization between DUT voltage and electron pulses. In this figure the electron pulses are locked in  phase with the DUT waveform, and the SED will see a signal consistent with the voltage-contrast at that one instant within the DUT  period. By slightly decreasing the frequency of the electron pulses relative to the DUT signal, the probe point on the periodic DUT  waveform will begin to advance in time, sampling whole periods of the DUT waveform at a rate given by the difference between the  pattern frequency and the pulse frequency.


electrons make it through the SEM to strike the DUT. This  single pulse of electrons – timed to occur once per period of  the waveform being sampled – captures the potential of the  logic waveform during the brief duration of the electron pulse  via the voltage-contrast mechanism of the SEM. Repeated  measurements improve the signal-to-noise ratio of this  measurement in time, while advancing the strobe in time  through the arbitrary pulse waveform provides the temporal  response of the arbitrary pulse waveform being measured.


For our eLVI lock-in measurements, our lock-in amplifier is  limited to 100 kHz operation, and together with other system  limitations, we clock the device at 78.125 kHz, which is well  below the bandwidth limitation (~ 5MHz) of the SED. We use  a pixel dwell time commensurate with our lock-in bandwidth  setting to capture our eLVI images, and typical images require  on the order of tens of seconds to acquire. Once switching  transistors are identified, we change the signal from the


78.125 kHz clock to any waveform – periodic or arbitrary – at  any frequency we chose for probing. If clocking a DUT at  such low frequencies is not possible, eLVI using chopped ebeam pulses can extend this to arbitrarily high clock  frequencies.


Fundamental to all stroboscopic techniques is a measure of the  equivalent width of the stroboscopic e-beam pulses used to  sample our waveforms. We calculate this quantity as the ratio  of transmitted current when the beam blanker is on vs. when it  is off. For example, if we configure the stroboscopic blanker  to produce e-beam pulses at 1 MHz, then the ratio of current  reaching the DUT when the chopper is turned on, vs. the  current with the chopper off, represents the ratio of equivalent  width of the stroboscopic e-beam pulses to the blanker period. Using this method, we calculate equivalent widths of the  stroboscopic e-beam pulses as 200 ps when driving the  blanker plates with sinusoidal waveforms (as in Fig. 2) while  for our pulse-on-demand system we calculate equivalent  widths of approximately 600 ps. The main difference between  the sinusoidal blanking and pulse-on-demand blanking  measurements is that with sinusoidal waveforms we can drive  the blanker plates at high RF frequencies and at high voltages (5 to 10 Volts peak-to-peak) while for our pulse-on-demand  system we employ differential logic chips capable of only 0.8  Volts peak-to-peak outputs, possibly with slower slew rates. We see no reason why, with similar amplification levels  applied to the blanking plates, pulse-on-demand blanking  could not reach the 200-ps equivalent widths achieved with  sinusoidal blanking.


As corroborating evidence that we can achieve 200-ps  equivalent width with sinusoidal blanking using our standard  blanker, we built a test system to go inside our SEM system  consisting of a printed circuit board with a 50-ohm exposedcopper microstrip transmission line, and using the method of  Fig. 2 we were able to measure RF signals up to a 3-dB  bandwidth of 1.6 GHz. We do not present these results  because it is comparatively easy to measure a high-speed  sinusoidal signal from millimeter-scale copper conductors. Instead, this paper focuses on measuring arbitrary logic  waveforms from a single fin of a FinFET transistor, and the  data we will present comes from a commercial GPU having  48-nm fin pitch and 14-nm gate lengths.


Figure 4 shows a region of the GPU after milling down to the  FinFET layer using a PFIB until individual transistor fins  could be resolved. At this point additional milling was  performed on the central region to maximize the strength of  the eLVI image observed on the lower rows of FinFET  transistors. This region contains four rows of 18 transistors  and forms a JTAG clock buffer operating at 0.8-V core logic  levels. Adjacent transistors share drain and source regions, and the nine drain regions clearly show the JTAG clocking  activity.


Once an active region is identified, we switch from the eLVI  imaging to point-mode probing of electrical waveforms by  switching from a continuous e-beam to a chopped e-beam. Shown at left in Fig. 5 is a region of the DUT imaged with an  un-chopped e-beam at 800 pA beam current. With chopping  activated, as shown at right in Fig. 5, the effective beam


Figure 3: Proof-of-concept experimental setup. Shown at left  is the Helios G4 system, which includes a SEM as well as a  plasma focused-ion-beam column. The DUT, located within  the Helios G4 system, is driven by the single-channel signal  generator (middle unit), while the two electrostatic beam  blanker plates are driven at opposite polarity by the dualchannel signal generator (bottom unit). The SED output, which records the voltage contrast of the DUT signal, is  captured by an oscilloscope (top unit). The system shown  measured waveforms up to 150 MHz, the limit of the test  equipment shown, and confirmed that stroboscopic beam  blanking could measure DUT waveforms higher than the SED  bandwidth limit of approximately 5 MHz. Subsequent  refinements to this setup, as described in the body, showed the  beam blanker could be used to measure waveforms up to 1.6  GHz bandwidths.


current drops to approximately 500 fA, representing on  average three electrons through the SEM column every  microsecond. While chopping we still maintains sufficient  resolution to image the individual fins, but resolution due to  chopping the beam is impacted. Using a standard tin-ball SEM  resolution target, and with our SEM configured for 800 pA  beam current, 1kV beam, 2-mm working distance, we  obtained under 4-nm edge resolution, but this increased to  nearly 10-nm edge resolution along the beam-blanking  direction with beam chopping activated. Because the beam  blanking occurs along one axis within the source, the e-beam  spot when chopped appears elliptical, leading to the observed  degradation along the blanking axis. Note that the right image  of Fig. 5 shows a ghost image; this effect appears unrelated to  the elliptical beam stretching, and it is not observed in our tinball images; its origin in this image is unknown, though  perhaps relates to some bleed through of beam current when  the beam is nominally off.


Figure 6 shows electrical waveforms measured directly from a  transistor fin of the JTAG input circuitry. This waveform was  obtained by chopping an 800-pA beam, with one burst of  electrons transmitted every microsecond through the SEM  column (see Fig. 6 caption for further details). One obvious  artifact is the ringing observed on the input signal, both after  the rising edge and the falling edge. Our test setup was not


designed with high-frequency operation in mind. The clock  signal is sourced outside of the dual-beam vacuum chamber; it  has an intrinsic rise time of approximately 500 ns. Within the  chamber a coaxial cable runs from a vacuum feedthrough to a  tee at the DUT, then through another coaxial cable back to a  second vacuum feedthrough, then on to an oscilloscope. The  tee in the coaxial cable, loaded by the DUT JTAG clock input, apparently introduces this ringing, as the exact same ringing  that is observed in the e-beam waveform below is also  observed on the oscilloscope by measuring the clock signal  that has passed through the dual-beam chamber. Otherwise we  measure a rise time of approximately 1.2 ns in this data. Also  worth noting is the signal we are probing has already passed  through some JTAG clock-driver circuitry within the chip at  our probe location, and it is unknown to us what the expected  rise time should be at this node within the DUT.


The bottom plot of Fig. 6 shows results when the JTAG clock  frequency is increased to 320 MHz. Note that the signal  observed appears more sinusoidal than square, likely limited  by a combination of the beam-blanking circuit, our poor highfrequency test setup, and the possibility that this DUT was not  designed to operate a such a high JTAG clock frequency.


In order to remove the unknown DUT performance from the  previous measurements, we replaced the DUT with the copper


Figure 4: Left image shows a region containing a JTAG clock buffer, with fins running horizontally. Fin pitch is approximately 48  nm from the SEM image. Right “eLVI” image shows clock activity on the buffer; the bright regions are the FinFET drain regions  where the potential is changing at the JTAG clock frequency (78.125 kHz). By identifying regions where activity is occurring, we can  locate regions to probe for waveforms. 


Figure 5: Left image shows FinFET transistors imaged with SEM settings of 800 pA beam current, 1kV landing energy, and 100 ns  pixel dwell times. Right image shows approximately the same region, but with beam blanking activated, allowing one pulse of  electrons through the SEM column each microsecond. Although the DC beam current is still 800 pA, due to chopping the effective  current in the right image is approximately 500 fA. The image dwell time is increased to 300 µs per pixel to reduce the graininess of  the image. Note the weak (~10%) ghost image in the chopped image, of unknown origin as discussed in the body.


201


microstrip transmission line discussed earlier. We drove this  with the fastest edge we could generate using our test  equipment, which was a 0 to 1 Volt pulse, 10 ns wide, repeating at 5 MHz, with a 100 ps rise time and a 1 ns fall  time. This fast edge was generated with a rise-time sharpener (Stanford Research model SRD1), which sharpens slow-rising  edges to 100-ps, but which does not sharpen the falling edge, instead inducing ringing artifacts on that edge. These edge  times were confirmed on a high-speed 20 GHz oscilloscope. This signal was passed into the SEM chamber, onto the  microstrip transmission line, back out of the SEM chamber, and back into the oscilloscope, at which time we measured a  300 ps rising edge, which suggests the signal on the microstrip  transmission line had a rising edge between 100 and 300 ps. We then measured this edge using SEM voltage contrast with  the identical setup as for probing the JTAG clock FinFETs, and observed the data of Fig. 7, which shows a 0-to-100% edge of approximately 500 ps, with a 20-80% edge time  slightly in excess of 300 ps. Note that voltage-contrast signals


are high when the DUT potential is low, effectively inverting  the measured signal.


We have demonstrated that the stroboscopic technique using a  standard Helios G4 beam blanker on the SEM column  achieves sub-nanosecond temporal resolution along with  sufficient spatial resolution to resolve FinFET transistors on  the 14-nm node. We have demonstrated an electrical-probing  system bandwidth of 1.6 GHz from micron-sized metallic  structures using sinusoidal beam blanking, and our pulse-ondemand e-beam blanker that was used for the proof-ofconcept data taken on FinFET transistors in a JTAG clock  chain showed rise times of 1.2 ns. However, using the same  pulse-on-demand setup, we observed a rise time of  approximately 500 ps from a copper microstrip transmission  line, suggesting our system is capable of GHz performance, and we therefore suspect the reduced-bandwidth edges


202


Figure 6: Waveforms probed directly from the FinFETs of the JTAG input clock buffer operating at 1.8V-logic while clocking the  device at (top) 80 MHz and (bottom) 320 MHz. The measured rise time is approximately 1.2 ns. The electron source operated at a  nominal DC current of 800 pA, though this beam was chopped to pass one pulse of electrons at one-microsecond pulse spacings. Each data point shown is an average of 2048 measurements of the SED signal, and there are 1000 data points in the above  waveforms, each spaced 50 ps apart, for a total span of 50 ns. This data set thus took 2048 × 1000 × 1 µs (i.e. approximately 2  seconds) to acquire.


observed on the JTAG clock were likely limited by our test  setup and not by any system measurement limitation.


We continue to learn how this tool operates, and we  acknowledge that a more custom SEM configuration could be  designed with high-speed e-beam probing in mind. Nevertheless, this standard Helios tool enables analysis of  circuit activity through voltage contrast measurements with  GHz measurement capability. This is a giant leap in the spatial  resolution from optical failure analysis methods that have  approximately 160-nm resolution. This work paves a path for  transistor-level analysis on FinFET circuits. By further  optimizing the system and blanker design, higher temporal  resolution may be achieved. A dedicated high-speed beam  blanker such as the one described in Meuret et al. should  allow us to probe DUT signals at 8-GHz speeds, though this is  currently untested.


The authors would like to thank William Lo and Howard  Marks of Nvidia Corporation for sharing enough design data  to make these preliminary FinFET measurements possible.


[1] Thong, John TL. (2004) Electron beam probing. Microelectronics Failure Analysis Desk Reference, ASM  International, Fifth Edition, 438-443.


[2] Thong, John T. L. (Editor) (1993) Electron Beam testing  technology, MICRODEVICES, Physics and Fabrication  Technologies.


[3] Shaw, C., et al. U. S. Patent 6,872,581.


[4] Meuret, S., et al. (2019). Complementary cathodoluminescence lifetime imaging configurations in a scanning  electron microscope. Ultramicroscopy, 197, 28-38.


[5] Kimball, Mark, et al. (2012). Advanced laser probe  techniques applied to FA of RF integrated circuits – A  case study, ISTFA 2012: Conference Proceedings from  the 38th International Symposium for Testing and Failure  Analysis, Nov 11-15, 2012, Phoenix, Arizona, USA.


[6] Tong, T., et al. (2018). Electron beam probing of active  advanced FinFET circuit with fin-level resolution, ISTFA  2018: Proceedings from the 44th International Symposium  for Testing and Failure Analysis, Oct. 28 – Nov. 1, 2018, Phoenix, Arizona, USA.


[7] Schlangen, R. (2010). Development and evaluation of  novel chip modification and analysis techniques, based on  backside focused ion beam preparation. Technischen  Universität Berlin, Ph. D. Dissertation.


203


Forming Discrete Components on an Integrated Circuit Utilizing Focused Ion  Beam Direct Write Capabilities


Kyle M. Winter, Steven B. Herschbein, Carmelo F. Scrudato, Brian L. Yates


GLOBALFOUNDRIES, EFK CCA


2070 Route 52, Hopewell Junction, NY, 12533


Focused Ion Beam (FIB) circuit edit allows for rapid  prototyping of potential semiconductor design changes without  the need to run a full manufacturing cycle in a semiconductor  Fab. By FIB editing a completed module, thorough testing on  the bench or in a full system can be achieved.  Logic can be  toggled, validation of speed enhancements performed, and  constructive and destructive failure analysis can be enabled. In  order to fulfill all the needs of clients in a rapidly evolving SOC  driven market, simply modifying existing devices by


“rewiring” circuits is becoming insufficient. Often the team is


tasked with making very repeatable structures to aid the circuit  analysis group.  These include relatively precise resistors for  tuning RF circuits (part of an RC network), adding known loads  or delays, et cetera.  Naturally resistive FIB deposited metal  lines connected to the existing circuitry can be used in this  capacity.


FIB chip edit is considered to be a “Direct Write” process.  The


beam pattern in conjunction with process gases defines the  regions of milling and deposition.   Unfortunately, FIB edit is  rarely an exact science.  In many cases, a number of  characteristics seem to be outside the realm of precise  repeatable control.  This is evident not only in individual tool  operational logs but also in FIB tool matching, where  maintaining identical system performance within the lab is  difficult or nearly impossible. These characteristics are highly  dependent on precursor reservoir composition and flow, surface  adsorption conditions, beam patterning integrity, and the total  interaction space of competing back sputtering during the new  material structure formation. Due to these factors, the shape, composition and electrical performance of metal and insulator  depositions vary over an often unacceptable range.  As a result, we were not meeting the needs of some critical customer  applications.


Direct written precision resistive structures displayed several  issues for which iterative edits were required to compensate for  variability. When attempting to create an exact resistance, this  process was not reliable, nor was it repeatable enough for  accurate circuit performance trimming.  Space-constrained  serpentine resistors or multiple discrete resistors side-by-side  showed the greatest process variability.  Metal deposition  processes tend to be somewhat self-limiting, so thick boxprofile lines are difficult to form.  Conductive material  deposited outside of the pattern definition (overspray) results in  line-to-line leakages. Attempts to remove the overspray thru ion  beam assisted etch-back tends to damage the deposited  conductors and underlying insulators. The low-k region  between lines can become cross-linked, experience gallium  doping, and become tungsten impregnated. This lowered the  resistivity of the insulator, increased the resistivity of the  conductor, and produced variability in the device which was  especially an issue when dealing with varying initial substrates.


GLOBALFOUNDRIES began a project to create a more robust  repeatable resistive structure by removing several variables. Rather than direct writing lines onto a top surface layer, a  confined deposition based on the concepts of dual damascene  processing used with copper layers in modern semiconductor  fabrication will be employed. The damascene process begins  with the definition of a box to be filled with a conductive  material.


The process of ion beam gas assisted anisotropic  etching/milling has a far more predictable outcome than ion  beam induced deposition.  It is possible to create a surface box  mill or even a deep drilled via of desired dimensions with a  more consistent repeatability. Deposition of tungsten into a  confined region using, for example, a W(CO)6 precursor and a  Ga+ ion beam results in an excellent via fill. Using this  behavior, precision resistors can be created with metal  deposition within the trenches which are created by the gas  assisted mill. An enclosed space can be filled nearly void-free, and has repeatable electrical parameters. The self-limiting  factors with tungsten deposition go away as sputtered material  becomes trapped within the well resulting in a near limitless Zheight potential.


The constant dielectric with a uniform and contained tungsten  fill can allow for a well-defined resistivity for the FIB deposited  tungsten material. Having a known resistivity, calculation of  dimensions for resistive and inductive structures during the  design process becomes feasible. With process variability under  control, structures can be formed reliably enough to offer this  as a service to customers.


# Forming Discrete Components on an Integrated Circuit Utilizing Focused Ion Beam Direct Write Capabilities


204


Despite increasing automation of semiconductor layout designs  through the use of rigid ground rules and key word controls, errors, both with wiring and in logical designs continue to occur  with frequency. Fixing these errors requires photo-mask respins. Often this will result in months of delay to get from mask  fabrication to the end of a semiconductor process line and  finally to a testable product module. If the mask revision does  not fix the error as intended, the delay may compound, resulting  in lost revenue, contracts, or even missing a technology node  entirely. To facilitate a faster learning cycle, a faster  prototyping method is necessary.


FIB circuit editing provides the industry with much needed  prototyping capability. With the ability to direct write design  changes for design revision validation, a FIB provides an etch  tool, as well as local dielectric and conductive depositions. These capabilities allow for reconfiguration of a chip's circuitry  making use of in chip power and ground lines, as well as preexisting logic arrays. Devices can be removed and logical high  and low can be applied to specific traces as needed to drive  desired circuit behavior. Simple devices such as capacitors and  resistors can be fabricated using existing metal or dielectric  layers in conjunction with FIB deposited materials.


The FIB circuit edit process generally involves backside, through silicon editing due to the higher ease of working in the  spaces between active transistor circuitry. The process itself  involves first thinning the silicon substrate to fraction of the  initial substrate thickness utilizing physical milling equipment. The thinned substrate is then polished for optical transparency. Samples are loaded into a FIB tool and required trenching is  performed to expose desired circuit location. Care is taken on  approach to not disturb active circuitry. If active circuitry is  disturbed a module can be rendered irreparable.


Once the targeted edit region is exposed, devices are added or  removed as requested by the customer. Connections are made  and the edited region is re-sealed using a dielectric deposition. The edited module is then repackaged and returned to the  customer for validation of the circuit edit and the proposed logic  or wiring design changes. A representative full FIB circuit  editing process is shown in Figure 1 below. [1]


Figure 1.  Pictorial representation of the basic module FIB process for a single location  wiring edit. [1]


Direct Written Devices


FIB circuit edit often involves a simple cut and a trace  connection. While many FIB edit customers need this  seemingly simple type of circuit edit, sometimes a new device  must be introduced into an existing microelectronic circuit to  achieve the desired outcome. Though not as precise, nor  reliable, as devices produced with standard planar processing, a  FIB deposited resistor could be all that is needed to build a  functional prototype.


Direct written devices are not limited to resistors, however this  study is most applicable for devices which involve, potentially  complex, long lines.[6] As such, resistors and inductors are the  direct written devices which are targeted for improvement due  to the FIB chip circuit edit needs of GLOBALFOUNDRIES lab  customers.


The resistive material utilized this study will be tungsten using  the precursor W(CO)6, partly for the excellent via filling  properties of the material, but also due to the relatively high  resistivity, low material cost, and widespread availability on  chip circuit edit FIBs. Other materials have been utilized in  experiments within the GLOBALFOUNDRIES chip circuit  edit laboratory, but will not be the topic of this publication.


Surface Preparation


Initial module preparation is always required, both to perform  the FIB circuit edit, and also to provide a proper substrate region  for resistor device formation. Standard surface preparation  involves thinning (milling) of the substrate down to less than  100µm of remaining thickness. The edit sites will be trenched  from remaining module substrate thickness in desired regions, and FIB cuts and connects will be performed. From the edit  location, a connection to the resistor will need to be created.


There are a few options for creation of discrete components. Devices can be formed entirely with FIB deposited materials  both conductive and insulative. Existing planar process  deposited films can also be incorporated into a FIB augmented  device. The advantage of devices formed entirely from FIB  deposited materials comes from the flexibility in the location of  devices. Theoretically, in the case of a resistor, a wire could run  out of an edit region, up 100µm of remaining substrate  thickness and could even be formed on the outer substrate (though this would not be a reasonable or practical way to add  a device).


A better option for resistor dielectric material involves utilizing  original existing planar deposited or grown insulative material. In general, it is easier to use existing fat wire level dielectrics  for forming FIB deposited dielectric structures, not only from  the standpoint of time to create devices, but also in terms of  overall dielectric quality.


In cases where no space exists in a dielectric layer for a resistive  structure to be built, the requisite dielectric layer can be  deposited. This may be accomplished either utilizing FIB


205


deposition which will be a lower quality material due to gallium  implantation and possible crosslinking. More preferably, the  dielectric material will be deposited by sputtering or growth of  a SiO2 or TEOS in a blanket deposition tool. Utilizing a blanket  deposition tool allows for a few microns to be blanketed across  the entire module. With a functional planar dielectric layer on  the module, devices may be fabricated as needed.


For most of the experiments performed in this study, preexisting aluminum test sites and fat wire level dielectric  materials will be incorporated into the FIB deposited resistors. The area allowed at the surface of the chips used between  aluminum pads was ample for experimental resistor formation. In a chip edit scenario, the dielectric constant of any  conventional dielectric of sufficient depth is less substantial to  device resistivity than the material of the conductive resistive  line. More leakage and variability occurs due to the conductive  material deposition than due to a slightly higher k dielectric  constant, assuming sufficient dielectric thickness.


The Challenge


The GLOBALFOUNDRIES chip circuit edit lab has been  tasked with providing specific high precision resistive  structures to be used in RF applications to tune errant circuits. The tolerances for resistive ranges are far tighter than in  previous FIB edits performed in the GLOBALFOUNDRIES  lab. The increased sensitivity, combined with the need for  multiple successful device edits, push a traditionally surface  deposited resistive structure out of manufacturability. The FIB  chip circuit edits may occasionally require higher ohm resistors. Creating devices on a scale of 1 ohm per square micron area  results in relatively large structures.


Figure 2: Direct write of three adjacent tungsten lines bridged by precursor


decomposition (overspray) outside of the beam pattern.  Attempts to isolate the lines will  invariably damage the remaining conductors.


Attempts to accommodate tight working conditions often  include building non-linear resistive structures which coil, zigzag, or take on a serpentine pattern encounter issues with  overspray shorting. Clean-up of the direct written resistive  structures while marginally effective, contributes to device  variability and lower prototype effective yield.


When tasked to build larger 1K+ ohm resistors, the FIB opened  edit region quickly becomes inadequate (Figure 2) for the task, the resistance tolerances too tight, and previous direct write  methods fail.


Device Construction & Edit Approach


Initial investigative work involved looking into known research  for lowering the variability of our deposited tungsten. Experiments were performed attempting to find best focuses to  modulate both deposition rate and profile. The via-filling


characteristics of tungsten quickly became a focal point of  interest in GLOBALFOUNDRIES FIB circuit edit  experimentation. Whereas a deposition in a FIB forms a  somewhat Gaussian distribution, with overspray creating the “tails” (Figure 3), a FIB etch is very anisotropic in comparison.


(Single and Double Deck Architectures)


In today’s market, there are various 3D-NAND memory  architectures, with an ever increasing number of layers, ranging from 32 to 96 (and beyond), depending on the  manufacturer and their technology node.  Besides increasing  the number of layers in a device, vertical scaling is augmented  by doubling or tripling the number of stacks (groups of layers) in a device, where each stack is comprised of 32 or more  layers.  In this study, both single and double stack 3D-NAND  devices were investigated.


Commercial samples were procured, depackaged and mounted  on standard SEM stubs and loaded into a ZEISS Crossbeam  550 FIB-SEM for data collection.  Site specific locations on  the samples were targeted by SEM and FIB navigation.  For  optimum throughput, imaging and milling were performed  simultaneously, without compromising resolution.  Data was  acquired in the form of a series of cross-sectional 2D SEM  images, collected through a volume of material (typically  ranging from 2x2x2µm to 8x8x8µm).  The spacing between  the images is nominally set by the FIB patterning parameters.  For the examples shown here, the nominal slice thickness was  set to 4nm.  Both secondary (SE) and backscattered (BSE) signals were collected for each image. Each set of images (SE  and BSE) was analyzed for slice positioning within the  acquired volume (i.e., the position of each slice is  determined).  This enabled the set of acquired cross-sectional  images to be rendered into an accurate 3D volume using inhouse algorithms.


This technology, FIB-SEM tomography [11-13], was applied to  characterize the shape and position of the vertical channel  holes throughout an 8x8x8µm volume in 3D-NAND devices.  The position and shape of each hole can be analyzed in terms  of diameter, ellipticity, bowing/bending and tilt.  Variation in  any of these parameters can affect device performance.


This approach is uniquely suited for 3D metrology because it  is possible to attain hundreds of measurements for each  channel hole and thus provide statistics not possible by  conventional cross-sectional SEM or TEM methods.


209


Following acquisition and alignment of the cross-sectional  images, a 3D rendering of the entire volume of a 64-layer (single stack) was created (Fig. 1).


Figure 1: (a) An example of a single cross-sectional image  from the acquired FIB-SEM tomography dataset and (b) a  volume rendering of a 3D-NAND structure.


Measurements of the positions and diameters of the channel  holes were performed on a virtual (reconstructed) plane in a  plan-view orientation (see blue colored plane in Fig. 1b).  Within that plane, contours were extracted from the edges of  the channel holes (Fig. 2a) resulting in measurements of the  position of the hole centers, and the relative variation of hole  center position with depth in the 3D-NAND volume (Fig. 2b).  What is especially surprising is that there is little correlation  among the relative positional shifts.


As an example of channel hole positional characterization, we  analyzed the path of three individual channel holes (chosen at  random) and plotted X-position of the channel hole center as a  function of channel hole depth (Fig. 3). These results, evaluated from thousands of raw measurements, show that  one of the three channel holes studied shows a higher shift in  position starting at 2500 nm from the top of the structures, and possibly due to local etch process variations which can  lead to lower yield and reliability. Further investigations of  channel variances with depth show a similar trend, i.e. the  positional variability increases with channel hole depth.  Fig


4. shows that relative shifts in channel hole positions in x and  in y increase as a function of depth.  We measure the


variability (3σ) increasing 4-fold between 1 and 4µm’s in  depth.  Repeating this analysis at various positions within the  die or across the wafer will provide valuable information to  monitor and improve process control.


Figure 2. (a) Edge contours extracted from a single plane of  the 3D rendered volume.  (b) Variation of measured channel  hole position:  position at the top of the channel holes (near  the surface) are shown as red dots and the corresponding  relative positional shift at the bottom are shown as blue  vectors. The magnitudes of the vectors augmented by 10x to  enhance the effect.


Figure 3: Measurement results for the position (x) of three  individual channel holes, as a function of depth from the  surface.  Each measurement point represents an average  value of 15 measurements from contours extracted for each  layer in the single deck 3D NAND structure.


210


Plan  view


Figure 4: Relative hole position (averaged over 468 holes) and corresponding 3σ variability of position as a function of  depth from the top-most hole.  Measured positional variability  increases with depth.


A double-stack 3D-NAND structure was prepared and imaged  by the same procedure of FIB-SEM 3D Tomography (Fig. 5).  For this device, a 5x2um area was imaged down to a depth of  3um, which includes the full top stack, the gap between the  stacks and a portion of the bottom stack.  The top-down SEM  images of the channels reveal the double ring and core  structure within each pillar (Fig. 6), which are typically  comprised of various silicon-oxides, silicone-nitrides and  poly-silicon films [1].  Contours were fitted to these doubleringed pillars as shown in Figure 6c, where the outer contour (blocking oxide) is represented in blue, middle contour (charge trap) in green, and the edges of the center core (in  red).  These contours were extracted from all the memory  channels in the analyzed volume (Fig. 6d shows 390 discrete  channels) providing over 135,000 measurements, which  highlights the statistical benefits of this approach over  traditional 2D cross sections (by SEM or TEM).


Figure 5: Cross sectional SEM image of a double-stack 3DNAND device.


Two examples of measurements obtained from contour  extractions are channel diameter and eccentricity (Fig 7.).  As  noted above, the channel diameter and channel diameter  uniformity is a key parameter which governs device  performance.  The Average channel radius for upper stack of  channels was 70.47nm.  The analysis of radius Vs. depth (Fig. 7a) showed the radius near the mid-point of the upper stack


211


trended larger than the top or bottom by ~4nm, as shown for 3  individual channel holes (chosen at random, but representing  the population trend).  The eccentricity (or circularity) of the  channels was also accessed, since it is another form of  deviation from design and therefore should conform within  the design tolerances.  The eccentricity shows different results  for different channels, with the largest variations about 1um  below the top surface of the upper stack.  Though the source  of this behavior is beyond the scope of this study, its  measurement provides additional non-idyllic structural  information for correlation with device performance.


Figure 6: (a) Secondary electron SEM image showing the  double-ring and core structure of the 3D-NAND pillars. (b) A  3D reconstruction result from the FIB-SEM tomography  dataset, (c) contours extracted from the dataset showing core  and rings of the 3D-NAND pillars, each colorized to enhance  the contrast, (d) contours extracted from the entire analyzed  volume: a 5x2um area and a depth of 3um.


Figure 7: Variation of channel structural characteristics in a  3D-NAND device.  Measurements of radius (a) and  eccentricity (b) are given as a function of depth from the  upper surface, for 3 randomly selected individual channel  structures.


Analysis of Logic Devices (14nm, 7nm)


Advanced logic process development and ramp-up requires  accurate methods for comparison of the desired layout with  the manufactured result.  Errors (or defects) can be manifested  as logical (e.g. layout) as well as fabrication errors (e.g. dimensional deviations beyond specified tolerances).   Application of 3D FIB-SEM tomography for identifying and  characterizing these errors was demonstrated on commercially  acquired devices: 14nm node (for layout verification) and 7nm  node (for fabrication errors).


Using backscattered electron signals acquired by FIB-SEM3D tomography, and accurate rendered 3-dimentional model  from a 14nm logic device was obtained (Fig. 8).  Results from  the 3D rendering clearly show the device layout starting at the  poly-gates and up through metal-0 (Fig. 9), by virtual  navigation using 3D visualization software.  Results from all  metal and via layers were obtained.  A comparison of the  plan-view (top down) images to CAD layout can be used to  verify physical layout with design.


212


Figure 8:  3D volumes from area of 1.5 x 3µm (and full depth  of the stack) from a 14nm logic device.  Voxel transparency  was assigned based on gray level intensity, such that BSE


signal from metal structures appears opaque.


Overlay of 3D structures governs the physical contact area  between the layers, and is most challenging for advanced  technology nodes having the tightest geometries.  One  example of a critical overlay are the contacts to gate.  Improper overlay (or edge placement) can result in opens, shorts or diminished reliability.   An example of what appears  to be a critical overlay in a 7nm-node sample is shown in a 2-dimentional (standard) cross-sectional SEM image of Fig. 10, revealing what appears to be single contact having less contact  area to the gate than the nearby contacts.  A 3D FIB-SEM  tomography analysis of this contact (Fig. 11) indeed reveals a  significantly reduced contact area than the nearby contact (58% less contact area).  This tomography shows the 3-dimentional nature of the edge placement error, enabling  direct measurement of the process errors at specific critical  manufacturing steps.


Figure 9:  Structures of a 14nm device shown reconstructed in  plan-view orientation.  (a) Fin structures, (b) Contacts to


gate, (c) Via-0, (d) Metal-0.


Figure 10: Cross-section SEM image of 7nm-node logic  device, acquired with backscattered electrons, showing finpairs, source-drain doping, gates, contact to gates and MEOL  metal layers.  Green (solid) arrow points to a contact to gate  with critical edge placement, which appears to be “overhanging” from the gate; blue (striped) arrow points to a  contact which is aligned to the gate.  The diminished contact  area was measured to be 42% of the reference, as seen in  Fig.11.


Figure 11: (a) 3D-contours of a reference contact to gate  structure denoted by the blue (striped) arrow in Fig. 10, (b) the corresponding area of physical contact between the  structures, (c) 3D-contours of an “overhanging” contact to  gate structure denoted by the green (solid) arrow in Fig. 10,


(d) the corresponding area of physical contact between the “overhanging” structures.


Contacted


area: 147nm2  Contacted


area: 62nm2


213


These results demonstrate the value of 3D FIB-SEM  tomography for physical confirmation of the structural layout, which can be applied towards device debug and reverse  engineering.  Furthermore, this methodology is well suited for  defect localization within the metal stack, without the need for  definitive nm-level fault isolation (as is required for defect  localization by TEM).


Demonstrated examples included two types of 3D-NAND (single and double stack), where channel profiles were  measured over hundreds of channels, each with dozens of  layers.  Also demonstrated are example measurements based  on 3D FIB Tomography acquired from 14 and 7nm logic  nodes, where layout verification and edge placement errors  were shown.


3D FIB-SEM tomography clearly holds statistical benefits  over conventional SEM or TEM cross-sectional approaches, providing hundreds of thousands measurements at a time, as  well as a complete 3D view of the layout and included defects.


The authors would like to thank the following persons from  Carl Zeiss SMT Inc.  for their valuable contribution to this  work: Keumsil Lee, Ramani Pichumani, Ted Lundquist, Baohua Niu.


Literature references are numbered in the order of their  appearance in the manuscript and are confined by brackets. They are listed at the end of the manuscript using the “ISTFA  References” format. Here is an example of the correct format.


[1] Y.T. Oh et al., Microelectronics Journal 79 (2018) 1-6


[2] Zhang, S., Byrnes, A., Jankovic, J., & Neilly, J. (2019). Management, Analysis, and Simulation of Micrographs  with Cloud Computing. Microscopy Today, 27(2), 26-33.


[3] Christopher J. Peddie Lucy & M. Collinson, “Exploring  the third dimension: Volume electron microscopy comes  of age”, Micron, Volume 61, June 2014, Pages 9-19.


[4]  Nobuhiko Ohno, Grahame J. Kidd, Don Mahad, Sumiko  Kiryu-Seo, Amir Avishai, Hitoshi Komuro, Bruce D. Trapp, “Myelination and Axonal Electrical Activity  Modulate the Distribution and Motility of Mitochondria  at CNS Nodes of Ranvier”, Journal of Neuroscience  18  May 2011,  31  (20)  7249-7258.


[5] Duarte, S., Avishai, N., Avishai, A., Heuer, A., & Phark, J. (2011). Three-Dimensional Characterization of Dental  Bonded Interface Degradation Using Serial Ion-Ablation  Scanning Electron Microscopy. Microscopy and  Microanalysis, 17(S2), 1016-1017.


[6] Grahame Kidd, Amir Avishai, Xinghua Yin, and Bruce  D. Trapp. “Three-Dimensional Analysis of Optic Nerve  Axons Using a Focused Ion Beam-Based Approach.” Microscopy Today 18, no. 1 (2010): 18–22.


214


[7] Debarshi Mustafi, Amir Avishai, Nanthawan Avishai, Andreas Engel, Arthur Heuer, and Krzysztof Palczewski. “Serial Sectioning for Examination of Photoreceptor Cell  Architecture by Focused Ion Beam Technology.” Journal  of Neuroscience Methods 198, no. 1 (2011): 70–76.


[8] Cantoni, Marco, and Lorenz Holzer. “Advances in 3D  Focused Ion Beam Tomography.” MRS Bulletin 39, no. 4 (2014): 354–360.


[9] Lorenz Holzer, and Marco Cantoni. “Review of FIBTomography.” Nanofabrication Using Focused Ion and  Electron Beams: Principles and Applications 559201222 (2012): 410–435.


[10] Paul G. Kotula, Gregory S. Rohrer, and Michael P. Marsh. "Focused ion beam and scanning electron  microscopy for 3D materials characterization." MRS  Bulletin 39, no. 4 (2014): 361-365.


[11]  E. Principe, Method and apparatus for quantitative threedimensional reconstruction in a SEM, US Patent #7,312,448 B2.


[12] I. Schulmeyer et al., "Advanced metrology and inspection  solutions for a 3D world," 2016 International Symposium  on VLSI Technology, Systems and Application (VLSITSA), Hsinchu, 2016, pp. 1-2.


[13] R. Jammy, 2nd CIES Technology Forum 2016  www.cies.tohoku.ac.jp/english/2nd_forum/


[2][3]


Figure 3: Surface Deposited Resistor Cross Section


This anisotropy can be combined with the excellent via fill  properties of tungsten to create very precise shapes in a module.


[4][5] (Figure 4)


Figure 4: Tungsten Filled FIB Etched Via


Resistive devices fabricated, whether direct written or etched  and filled using tungsten, require an insulative dielectric  substrate. The first experiments utilized a blanket deposition of  dielectric on a bare silicon sample with a TEOS layer of  approximately 4µm. The coating worked adequately well  electrically grounded product modules, but even with the  charge neutralizer active, arcing still occurred on test samples  fabricated on bare silicon with the blanket TEOS coating. To  facilitate data collection, an older product previously edited in  the GLOBALFOUNDRIES FIB circuit edit laboratory was  incorporated into this series of experiments. Pre-existing  aluminum test pads on this product were utilized after pad pairs  were verified to have greater than 1M-Ohm impedance. Devices were then fabricated as seen below. (Figure 5)


206


Figure 5: Straight Resistors on Oxide


The underlying material is a dielectric 6µm thick. Devices


were written in batches of five, with a simple device design, a  straight line, with a dose of 4 nC/µm². Surface and trench


deposited materials were deposited with an identical


deposition recipe. The target deposition polygon shape width  was 2µm and the length was 135µm. Figure 3 shows the


resulting shape and distribution of this deposition on the


surface of the oxide film. Vias were made with 5µm x 5µm


squares running down to the buried metal layer. Larger vias  merely increased deposition times. Smaller via dimensions,


such as 1µm2 which was initially tested, resulted in a


substantial amount of the resistive effect being added by the  vias themselves rather than the resistive line.


The distribution of the direct written 2µm line width resulted  in a 4µm line width due to overspray. This necessitated FIB  etch material removal and therefore restricts compression of  serpentine resistive structures due to residual tungsten


implantation and crosslinking providing leakage paths.


To encapsulate potential overspray, damascene deposited


resistors were filled using the same process as the direct


written resistors. Instead of a surface deposition, tungsten was  deposited within a 3µm wide and 2µm deep trench. The result  appears to increase the overall deposited tungsten due to the  enhanced dep rate of tungsten in confined space.


Figure 6: 100nmx100nm Tungsten Cross Section


Damascene deposited tungsten resistors utilizing a dose of 4  nC/µm² yielded much cleaner lines with almost zero taper.


Furthermore, experimental device construction showed line


integrity and aspect ratio were maintained down to 100nm by  100nm cross sectional dimensions.  (Figure 6)


After demonstrating successful device designs in a linear


resistive structure, more complex designs were fabricated to  create higher resistance. In these devices the effects of the


damascene process become more apparent as overspray from  parallel lines bridges parallel resistors rendering them


ineffective without cleanup and increases variability post


cleanup in the final devices. (Figure 2) Tungsten lines


deposited into trenches, however, show superior isolation with  greatly reduced overspray and required minimal cleanup.


(Figure 3)


Additional research and development into complex resistive


shapes is still ongoing and data collection is in progress.


Experimental Results


Resistivity of damascene deposited resistive structures showed  a lower resistivity than direct surface deposited tungsten  resistive structures. This is due to the seemingly higher  deposition rate which was observed in the damascene process. The higher deposition rate most likely correlates to the  combination of more trapped secondary electrons and phonons  in the trench region resulting in higher precursor adsorption. Though the additional surface area of the sidewalls, open lattice  structures due to etch process damage or other variables could  be responsible for the mean resistance delta between sets of  experiments.


For lines of the same run, the range of resistance for a batch of  experiments using the damascene process was about 15 ohms, and had a standard deviation of 4.7 ohms. In contrast direct  surface written resistors had a process range of 30 ohms and  standard deviation is 8.2. Preliminary results seem to be  showing a 50% reduction in variability with the new damascene  process when compared to direct surface written structures in a  linear device.


Figure 7: Damascene Fabricated Serpentine Resistor


After proving out device designs in a linear resistive structure, more complex designs were fabricated to create higher


207


resistance. (Figure 7) In these devices, the effects of the


damascene process becomes more apparent. Overspray from  parallel lines bridges deposited tungsten, lowering resistivity, and rendering the devices ineffective without cleanup. Figure  8 shows even after cleanup, overspray from the tungsten


deposition still bridges lines slightly. This residual over


sprayed tungsten also increases variability post cleanup in the  final devices. (Figure 2) Tungsten lines deposited into trenches  however show a strong isolation with near zero overspray and  do not require excessive cleanup. (Figure 3)


Figure 8: Cross-section of a Serpentine Direct Deposited Resistor


FIB circuit edit techniques have become an integral part of the  process for accelerating design of new technologies as well as  integrated IP solutions in ASICS products. As with the  evolution of the microelectronics industry as a whole, we are  evolving our FIB techniques to meet new challenges with every  job.


In several recent edits the GLOBALFOUNDRIES chip circuit  edit group has been tasked with fabrication of resistive  structures in a circuit edited module. As with all new techniques  fabrication outcomes have shown variability as initial  experimentation results in better understanding of the process. The challenge was, and is, to take a development project and  make it a “manufacturable” process for customers. The best  way to accomplish this shift is to minimize variables in the best  known process.


Direct written tungsten lines with the inherent overspray  present a number of variables in device construction not only in  potential leakage paths, but also in the subsequent cleanup  activities. A more controlled FIB etch followed by a selfcontaining deposition reduces a few variables that are known  but adds the variable of the FIB etch itself. Nevertheless early  experimental data shows a 50% reduction in variance.


In the future, one goal would be design and fabrication of FIB  created resistors based on a known resistivity per linear micron  and understand how it relates to dep rates. This is a fairly  difficult task given the inherent variability in all FIB  depositions. The difficulty is, in large part, due to the number  of variables introduced from source lifetimes, aperture wear, tungsten loading and substrate properties. Initial data however


suggests, with all readily controllable experimental variables  equal, damascene resistors are much more consistent in their  resistivity.


Several questions do remain: Would a different material  perform better than tungsten for this application? Or would  other materials exhibit the same deposition properties within a  confined trench? Could gases be introduced to the metal  deposition to make a more “resistive” conductor?


These are questions which the GLOBALFOUNDRIES FIB  circuit edit lab in East Fishkill, NY would like to explore and  understand through ongoing research into these damascene  deposited devices. It has been observed that FIB circuit edits  are more reliable with a damascene deposited tungsten, and the  future will yield only more information and progress as research  continues.


[1] S. Herschbein, et al, “Exploring the Physical Limits of  Gallium-Based Focused Ion Beam (FIB) Chip Circuit  Editing,” Proc. 43rd ISTFA, Pasadena, CA, Nov. 2017, pp. 238-245.


[2] R. Young, et al, “Characteristics of gas‐assisted focused  ion beam etching”, Journal of Vacuum Science & Technology B: Microelectronics and Nanometer Structures  Processing, Measurement, and Phenomena, Vol 11, No  234, 1993 https://doi.org/10.1116/1.586708


[3] M. Ishida, et al, “Focused ion beam-induced fabrication of  tungsten structures”, Journal of Vacuum Science & Technology B: Microelectronics and Nanometer Structures  Processing, Measurement, and Phenomena, Vol 21, No 6, 2017 pp. 2728-2731 https://doi.org/10.1116/1.1627806


[4] H. Langfischer, et al, “Evolution of tungsten film  deposition induced by focused ion beam”, Journal of  Vacuum Science & Technology A, Vol 20, No 1408, 2002  https://doi.org/10.1116/1.1486230


[5] Y. Drezner, et al, “Characterization of damage induced by  FIB etch and tungsten deposition in high aspect ratio vias”, Journal of Vacuum Science & Technology B, Vol 29, No  011026, 2011 https://doi.org/10.1116/1.3539204


[6] W. Clark, et al, “Integrated circuit resistor fabrication  using focused ion beam”, U.S. Patent 5047827A 10 Sep.,


1991.


208


# Visualization and Measurements of 3D Structures in Memory and Logic Devices


Visualization and Measurements of 3D Structures in Memory and Logic Devices


A. Avishai, and A. Buxbaum


Carl Zeiss SMT Inc., Pleasanton, CA


amir.avishai@zeiss.com, alex.buxbaum@zeiss.com


D. Klochkov, J.T. Neumann, T. Korb, and E. Foca


Carl Zeiss SMT GmbH, Oberkochen, Germany


Requirements for imaging and metrology of structures in ICs  continues to challenge the semiconductor industry.  New  materials and scaling in 3-dimensions (with very high aspect  ratios, HAR-in many applications) add complexity to the tasks  of defect localization and process control.  The importance of  dimensional tolerances on device functionality is well  understood.  For example, a 3D-NAND memory device has a  structure comprised of channel holes etched deep (>6um) through dozens of thin film layers.  Variations in channel  diameter across the die and through depth is known to affect  the threshold voltage at which the devices operate [1]. Therefore, knowledge of the etch profiles and channel hole  diameters throughout the volume, is essential for  understanding performance characteristics and serves as a  metric for the etch process optimization.


High aspect ratio (HAR) devices are particularly challenging  structures to measure by conventional TEM, where analysis is  limited to ~20nm thin slices containing only a few structures (note that typical NAND structures are ~8µm in height, which  is at the dimensional limits of TEM lamella).  This also limits  the number of structures that can be analyzed by this method, and consequently results in poor statistics.  This demands new  approaches to device analysis.


3D FIB-SEM Tomography methods have been applied in  other fields where 3-dimensional structures are present, such  as neural structural research in the medical field [3-8], fuel cells [2,8,9], and oil and gas [2,8,9]. In some cases, a 3D FIB-SEM has  been used in conjunction with analytical techniques such as  EDS and EBSD [8-10].


In this paper we describe the application of 3D FIB-SEM  tomography as a method for quantifying process variations  across the die and across the wafer (e.g. metal line CD and via  to metal line overlay error), as well as layout investigations.  The value of measurements taken from a 3D rendering is in  the quantification of structural variation, with very large  sampling statistics.  These measurements of statistical  variation in structures from various points on the wafer are  instrumental in process development and process control.  The  analysis of results acquired by 3D FIB-SEM tomography were  applied to a 64L 3D-NAND device where we measure process  induced variation in the HAR vertical memory channels and to  a “double stack” 3D-NAND architecture, which is comprised  of two 32-layer stacks where eccentricity of the pillars was


evaluated for layers in both upper and lower stacks.  In  addition, a partial layout of a 14nm logic device is  investigated by this method, demonstrating the capabilities for  structural verification. Finally, structural overlay of elements  from a 7nm logic device were evaluated.


Analysis of 3D-NAND Structures


Applying a Significant Protection Layer on Double Ex Situ Lift-out TEM  Specimens to Protect Against Ion Beam Impact


Chun-Hung Lin, Hsin-Cheng Hsu, Tsung-Yi Lin, Ru-Hui Lin, I-An Chen, Pei-Lin Hsu, Chao-Kun Chen, Iris Hsieh, Chin-Chih Yeh, Nan-Tzu Lian, Ta-Hone Yang, Kuang-Chao Chen


Macronix International Co. Ltd, Li-Hsin Road, Hsinchu Science Park, Hsinchu, Taiwan. E-mail: chunhunglin@mxic.com.tw, Phone: +886-3-6668999 ext. 52352


Protection layers on double ex situ lift-out TEM specimens  were investigate in this paper and two protection layer  approaches for double INLO or double EXLO were  introduced. The improved protection methods greatly  decreased the damage layer on the top surface from 90 nm to 5  nm (or lower) during FIB milling. According to the property  of different sample and its preliminary treatment in the FIB, we have the satisfactory approaches to be applied. Using this  improved protection method, we demonstrate the structures  within the TEM lamella can be observed without ion beam  damage/implantation during FIB


Focused ion beam (FIB) instruments have been widely used to  prepare high quality transmission electron microscopy (TEM) specimens. FIBs can easily prepare site-specific TEM lamellae  on a variety of materials systems, with observed thicknesses  less than 10 nm [1, 2].


One FIB technique, the lift-out method, has become very  popular owing to the relatively short times to produce highquality TEM specimens from semiconductors.  In fact, both  the ex situ lift-out (EXLO) and in situ lift-out (INLO) methods  which are routinely used to create TEM samples are involved  in this method. The major difference is the former utilizes a  micromanipulator with a fine tip (or glass needle) to pick up a  prepared specimen from a bulk sample to transfer it onto a  TEM grid while the latter is performed entirely inside the  enclosed FIB chamber [3].


The EXLO method involves milling a free-standing sitespecific lamella to electron transparency in the FIB and then  transferring the thin lamella from its trench to a TEM grid  with a micromanipulator. It employs a light optical  microscope (OM) and a glass needle to conduct the lift-out  procedure.  An advantage to the EXLO method is that it is  very fast and often satisfactory for the majority of routine  TEM sample analysis in the semiconductor industry. The  disadvantages of the method are (a) it is very difficult to rethin and rework the EXLO specimen once it is mounted on a  coated-grid, (b) the grid type may hinder some TEM analysis  such as electron energy loss spectroscopy, (c) the operator


must be careful to avoid the redepositing effect on the  specimens, and (d) the OM used in the process has resolution  and the depth of field limitations, often making it difficult to  manipulate the sample during this procedure.  Moreover, the  pick-up process relies on electrostatic forces to attract and  keep the TEM specimen attached to the glass needle while  transferring it from the bulk sample to the TEM grid.  These  adhesion forces are sometimes too weak and unpredictable to  reliably perform a successful lift-out procedure [4].


Accordingly, the INLO method is performed inside the FIB  instrument by using a built-in micromanipulator. The  drawbacks of the EXLO method are eliminated since the  manipulator tip is welded onto the specimen using an ion  beam induced deposition in the FIB instead of adhesion forces  on glass needle. A similar welding process is also performed  to attach the specimen section to a TEM grid. These  procedures enhance the physical strength of the connections  resulting in more reliable weldment and, in turn, a higher  success rate during the lift-out process.


Due to the intense scaling competition in industry, unpredictable tiny defects, which may cause failures in  semiconductor devices, have become a challenge for  conventional FA tools to visualize easily. In order to find out  the root cause for process optimization and yield  improvement, these defects must be identified and  characterized. TEM is a powerful technique for semiconductor  process characterization and failure analysis. In general, the  thickness of lamella should achieve electron-transparency  which is dependent upon the size scale of the defects of  interest. It is common for targeted lamellae thicknesses to be <100 nm.  Considering some tricky process issues which may  be difficult to identify the root cause, it is necessary to prevent  any lost information from a critical area in TEM specimen.


An ideal sample preparation technique, the double lift-out  approach, was introduced and demonstrated benefits for  failure analysis to achieve 3D observations from two  dimensional data [5].  Since a TEM lamella has only severaltens nanometers of thickness, the double lift-out approach can  prepare the cross-section TEM specimen from an observed  TEM lamella in the DB-FIB.  However, FIB milling  inherently results in lamella surface damage and ion  implantation, which must be overcome.


Prior to creating a TEM lamella, a protective layer is deposited  onto the specimen section using ion beam induced carbon (or


# Applying a Significant Protection Layer on Double Ex Situ Lift-out TEM Specimens to Protect Against Ion Beam Impact


215


W, or Pt) deposition. The ion impact on the specimen surface  causes not only material removal (sputtering), but also surface  damage. The thickness of this damage layer into the bulk of  the material is almost proportional to the depth range of Ga+ implantation and is roughly proportional to the primary energy  of the Ga ions [6].


Therefore, for the double lift-out specimen, a strategy of  coating the cross-section of TEM lamella with a significant  protection layer is proposed to prevent the surface damage. Specifically, ink coating and FIB e-beam induced carbon (or  Pt) depositions are applied to create a protective layer before  ion beam deposition and milling in an effort to mitigate  surface damage.


Experiment


TEM lamellae preparation and ion/e-beam depositions were  performed using a dual-beam FIB (Helios 400, Thermo  Fisher).   The light optical microscope (OM) (Eclipse FN1, Nikon) combined with a fine glass needle micromanipulator  was utilized for the ex situ lift-out procedure.  The ink coating  was performed by brushing the target surface at room  temperature.


A copper grid overlaid with a carbon-coated collodion film  was used to support the TEM lamellae.  The TEM analysis  was conducted using an Osiris TEM (FEI/Thermo Fisher) coupled with EDS (SDD, Bruker).


For preparing a TEM specimen, a protective layer on top  surface of sample is required before FIB milling.  Ion beam (iBeam) deposition is the most popular technique to deposit a  suitable layer on the region of interest.  The 30kV Ga+ ions  impinge the sample surface, depositing their momentum  leading to material removal, ion plantation and surface  damage.  As shown in Figure 1, the carbon layer is deposited  on the wafer surface by IB deposition at accelerating voltage  of 30kV and current of 0.28nA. The TEM bright field images (BFIs) show the substrate surface becomes rough and  amorphous. The same phenomenon is observed at conditions  of 30kV and 93pA.  This result means that lower beam current  does not reduce the damage layer.  This effect is well known  in the TEM community.  All FIB prepared samples are  damaged in this way including those prepared by the double  EXLO and the double INLO methods technique.  It is tough  mission for the double cross-section technique.  TEM lamella  which may have only a thickness of several tens cannot  withstand further loss in thickness.  Thus, we present two  methods consisting of ink coating and eBeam deposition.


For TEM specimen preparation, eBeam depositions are often  performed as an alternative to iBeam depositions to prevent  ion impacting onto the sample [7].  But eBeam takes at least  20 times longer than the later so that the electron beam  induced deposition layer is seldom used for the entire  protective layer.


As mention by Giannuzzi, most protective layers consist of 50  to 200 nm thick eBeam followed by an iBeam deposition layer


[2].  We recommend the layer thickness be larger than 100 nm  to have perfect protection. We found eBeam deposited carbon  can be easily removed during iBeam deposition. Once the  protecting layer is thinner than 100nm, a damaged layer will  be observed.


In order to understand the reliability of eBeam carbon for  protecting the surface of a double cross-section sample, Figure  2 shows 100nm of eBeam carbon followed by an iBeam Pt. (50nm carbon /50nmPt). The images show the substrate  surface is smooth and the Silicon lattice is preserved.


Figure 1 (a) TEM BFI with damage layer on Si substrate, and (b) magnified BFI from (a) with clearly uneven surface (yellow arrow).


Applying ink (Sharpie) as a protecting layer for TEM  specimen preparation is the most popular method in the  semiconductor industry.  A major challenge in the preparation  of TEM samples by FIB is the curtaining effect [8].  This  effect consists of striations across the lamella, when the  sample has non-uniform material properties, such as density, crystal orientation, atomic weight, irregular topography, or  chemical composition. The consequence curtaining is  significant ambiguity in the the TEM result because the  sample no longer has constant thickness. Ink has good  mobility, strength and covers well over aspect ratio of  surfaces. It also prevents ion impact when deposited with  sufficient thickness.


Figure 2 (a) TEM BFI for eBeam C / ibeam Pt / iBeam C on  Si, (b) magnified BFI from (a), and (c) eBeam carbon on Si  substrate with clear lattice image.


Figure 3 (a) and (b) shows a 100nm thick ink coated on Si  substrate followed iBeam carbon. With ink, the Si substrate  has no amorphous layer or uneven surface.  However, this  approach is difficult to apply in the double in situ technique  because of equipment limitations. Coating ink (or epoxy) requires optimization.


216


Figure 3 (a) TEM BFI for iBeam C / ink coated on Si (b) magnified BFI from (a) on Si substrate with clear lattices  image.


Figure 4 presents a TEM lamella fabricated by the double  EXLO method.  Figure 4 (a) shows an electron-transparent  TEM cross section specimen put onto an ink-coated blanket  wafer and followed ink coating. After routine preparation of  the cross-section sample, including trenching and thinning in  FIB, the new lamella is a plan view of the original sample (Fig  4 (b)).


In Figure 4 (c), we can clearly distinguish the specimen from  the two ink-layers on substrate and image the desired  morphologies.  Surface damage which comes from the first  cross-section specimen is found in Figure 4 (d). There are  many literature references to the relationship between the  thickness of damage layer and the accelerating voltage [9-13]. In this case, the final milling occurs at 5kV of leading to a  5nm thick amorphous layer.  This result is consistent with the  reported data.


Figure 4(a) SEM image of an ink-coated TEM lamella (b) TEM BFI for double ex-situ specimen from (a) (c)  magnified BFI from (a) with distinguishable layer stacks (d) damage layer from the first cross-section.


Case Study


Electronic failure analysis found a single bit retention issue in  areal device.  The failing bit shows charge loss, after thermal  stress of baking for 48 hours/150C.  The threshold voltage


distribution has shown in Figures 5 (a) and (b), displaying the  retention of single bit.  The ONO thin film and the below layer  are suspected to be the issue.


In the past, TEM cross-section results can easily catch the  point and then provide a path to the solution.  Recently, with  the scale reduction, tiny or tricky defects make root cause  identification much harder.  Delayering is done to approach  the region of interest.  Acid etching is used to enhance the  defect. As shown in Figure 5 (c), there is a pattern which  differs from the nearby two contacts.  As shown by the yellow  rectangle, y-direction of TEM cross-section lamella contains  the failed bit.


Figure 5(a) the threshold voltage distribution with pass  feature (b) the threshold voltage distribution after thermal  stress of baking for 48 hours/150 oC  (c) SEM image for fail  bit after polishing and acid etching.


From the TEM BFI in Figures 6 (a) and (b), the defect region  is found and an ONO thin film issue is determined to be the  root cause.  However, EDS mapping show several species  present including Si, N, O and Co between the contact and the  failed bit. In order to find out the root cause for process  optimization and yield improvement, these tricky defects must  be identified.  We performed the EXLO technique to clarify  the problem. Before doing TEM, the failed region needs a  protection layer to preserved vital information.  Ink coating  was used to protect the surface of the specimen.  By  comparing Figures 6(d) and 6(f), the CoSi extends across the  contact to the fail bit leading to the SiN film between them to  lose its function to stop charge transfer.  The root cause comes  from the defect between the poly-Si etch and low pressure  SiO2 deposition.


Figure 6 (a) BFI for issue region; (b) BFI for pass region;


(c) EDS mapping for issue region; (d) BFI of double EXLO  specimen of (a);  (e) BFI of double EXLO specimen of (b);


(f) EDS mapping for issue region of double ex situ specimen.


217


We have introduced two approaches for protection layers  during either double INLO or double EXLO process.


According to the property of sample and its preliminary  treatment in FIB, a satisfactory approach can be applied.  By  applying the method, we demonstrated that fine failure  analysis detail in TEM lamella can preserved by avoiding ion  impact during FIB preparation.


[1] Mayer J, Giannuzzi L A, Kamino T and Michael J, MRS  Bul. 32 400–7 2007


[2] Giannuzzi L A and Stevie F A, Micron 30 197–204 1999


[3] M Lekstrom, M A McLachlan, S Husain, D W McComb  and B A Shollock, Journal of Physics: Conference Series 126 (2008) 012028


[4] Lucille A. Giannuzzi, Zhiyang Yu, Denise Yin, Martin P. Harmer, Qiang Xu, Noel S. Smith, Lisa Chan, Jon Hiller,


Dustin Hess, and Trevor Clark, Microsc. Microanal. 21, 1034–1048, 2015


[5] C. H. Lin et al., "Dislocation Analysis in STI Structure of  Flash Memory by Advanced 3D TEM Sample Preparation


Approach" 2016 IEEE 23rd International Symposium on the


Physical and Failure Analysis of Integrated Circuits (IPFA)


[6] Joachim Mayer, Lucille A. Giannuzzi, Takeo Kamino, Joseph Michael, MRS BULLETIN VOLUME 32 MAY 2007


[7] Chen Li, Gerlinde Habler, Lisa C. Baldwin, Rainer Abart, Ultramicroscopy 184 (2018) 310–317


[8] E. Montora et al., "Evaluation of Top, Angle, and Side  Cleaned FIB Samples for TEM Analysis "MICROSCOPY  RESEARCH AND TECHNIQUE 70:1060–1071 (2007)


[9] L.A. Giannuzzi, R. Geurts, J. Ringnalda, Microsc. Microanal. 11 suppl. 2, 828 (2005).


[10] K. Thompson et al., Microsc. Microanal. 12 suppl. 2, 1736CD (2006).


[11] J.D. Casey et al., J. Vac. Sci. Technol. B 20, 2682 (2002).


[12] J.R. Michael, Microsc. Microanal. 12 suppl. 2, 1248CD (2006).


[13] R. Spolenak, L. Sauter, C. Eberl, Scripta Mater. 53, 1292 (2005)


218


Variable Angle TEM Grid Holder for Advanced TEM Lamellae Preparation


Tomáš Hrn číř, Marek Šikula, Pavel Doležel


TESCAN Brno s.r.o., Brno, Czech Republic


tomas.hrncir@tescan.com , phone +420 530 353 468


Claudio A. G. Savoia


STMicroelectronics, Agrate Brianza, Italy


Multipurpose sample holder for advanced Transmission  Electron Microscopy (TEM) sample preparation which reduces  cost of the tool and most importantly simplifies the workflow is


introduced. Following the current demand for user-friendly


interface, semi-automated approach is aimed to be build up. Abilities to prepare advanced TEM lamellae in various


geometries without rotary nanomanipulator and using various  end-point detection signals are perceived as biggest advantages  of this design.


The common approach starts by cutting out a small portion of  the analyzed sample with the Focused Ion Beam (FIB). This


portion is then transferred onto the TEM specimen holder by  performing in-situ lift-out process. Subsequently, it is thinned  with FIB to the desired thickness on this holder, making a thin  and electron transparent lamella. This lamella can be then  observed in-situ by using Retractable Transmission Electron  Microscopy (R-STEM) detector or transferred for more detailed  investigation into a dedicated TEM microscope. However, there  are several possibilities how the lamella could be oriented  towards the original sample or how the lamella could be treated  during or after the lift-out process. Sometimes it is necessary to  prepare the lamella perpendicular to the original sample surface (plain lamella), sometimes it should be parallel to the original  surface (planar lamella) [1, 2]. Moreover, plain lamella should  be sometimes rotated to the opposite side, to get FIB access  from its bottom side (inverted or back-side lamella). This is a  must for present state-of-the-art front-side semiconductor  samples, where the final polishing from the back side (silicon  side) gives much better quality of the lamella and allows to  prepare much thinner lamellae containing only specific region (gate-cut, fin-cut) [3]. Sometimes it is even necessary to prepare  another lamella crossing that thin lamella perpendicularly (cross-lamella), to focus e.g. on a certain single transistor gate  only. For all of these lamella preparation types, the lamella must  be rotated in a special way so that it is accessible for FIB ion  beam from its different sides. To make things even more  complex, certain position of the lamella is necessary to perform  the final thinning by FIB and to precisely control the end-point, where FIB beam and lamella are almost parallel. Another  position is needed to observe the progress of the work e.g. with


219


R-STEM detector, where the ideal direction of Scanning Electron


Microscope (SEM) beam for observation is being perpendicular


to the plane of the lamella. Another limitation for backside


sample preparation is the necessity of having the nanomanipulator with the rotary tip, while the preparation geometry (stage and tip positions) can be quite complex [4].


For possible SEM imaging/end-pointing methods, see Fig. 1. Ideally, all of these methods should be available, accessible  from both sides of the sample, without any limitation, because  all of them bring useful information during TEM sample


preparation process. SE detector image brings an information  about the sample thickness. In-Beam SE/BSE image helps to  navigate to the correct place during the final polishing of the  sample, because of the distinct material contrast. STEM  detector image brings integral information from the whole  thickness of the sample and can be used for final TEM imaging, even replacing dedicated TEM for bigger sample structures. EDX is able to perform e.g. a qualitative analysis of elements  inside a particle that can be an electrical defect root cause. Therefore, we have focused on development of the solution  which would address all above requirements, but which should  be simple and effective.


Figure 1: Possible SEM end-pointing detector signals.


This research refers to the preparation and observation of  TEM samples by using FIB. Whole workflow is performed insitu, without breaking the vacuum and without removing the  sample out of the chamber. SEM is used for the observation  throughout the preparation process.


Figure 2 describes an optimal TEM sample preparation  workflow, our goal for designing the TEM holder. Skipping  some steps would simplify the workflow and make TEM  sample preparation process noticeably simpler and faster. Removing the necessity of rotation of the nanomanipulator tip  would simplify the workflow too and reduce the price of FIBSEM instrument used for in-situ lift-out. See Fig. 3 for the  schematics of back-side lamella rotation by using the  nanomanipulator tip. All angles involved might be non-trivial, which depends on the direction of the nanomanipulator towards  FIB and SEM [4]. Following such lamella preparation  workflow could be complicated and less efficient. We have  solved this complex problem by developing a novel TEM  sample holder.


Figure 2: Left-side scheme describes standard approach while  right-side scheme shows the targeted one.


TEM sample is placed on TEM grid, which is attached to a  bracket with adjustable rotation angle and which allows in-situ  angle variation. This rotation angle can be varied for different  stages of the lamella processing, such as the FIB thinning, the  backside thinning or SEM / R-STEM observation. In addition, in the position of the lamella holder for the FIB thinning and for  the backside thinning, we can easily check the quality of FIB  machining by SEM observation and R-STEM detector or other  detectors by changing the main stage tilt. Similarly, by the  appropriate change of the angles of the main stage tilt and the  rotation of TEM sample holder, preparation and observation of  the lamella parallel to the surface of the original sample (planar  lamella) can be performed. The great advantage of this solution  is the simplicity of TEM sample preparation process, the  frontside – backside – planar – SEM / R-STEM observation  flexibility, and the fact that there is no need to use a rotary tip  nanomanipulator to obtain backside thinning direction. Moreover, the movement of the holder requires no installation  of any additional manual or motorized positioning mechanism.


Existing stage tilt mechanism (of TESCAN FIB-SEM) is used


also for changing the tilt angle of the novel TEM holder in-situ,


at fast speed already used by the stage mechanism and without  interrupting the chamber vacuum.


Figure 3: Schematics of back-side rotation of the lamella by  using the nanomanipulator rotation.


TEM grid cartridge (which accommodates two TEM grids) is  placed into the U-shaped holder which has predefined rotation  angles. These predefined angles together with main stage tilt  can cover wide range of geometries. Concerning the possible  working distance (WD), FIB-SEM coincidence point WD is


achievable (which is e.g. 6 mm for TESCAN S8000G). Shorter  WD is achievable e.g. for final TEM sample observation at zero  tilt angle, taking advantage of the best SEM resolution. This  variability allows user to attach TEM sample onto the grid in  virtually any possible direction. During different stages of the  lamella processing, the lamella quality can be checked by SEM  observation using various SE/BSE detectors or R-STEM  detector just by changing the main stage tilt.


When designing the variable angle holder, standard workflow  geometries were verified by using 3D model at first, see Figs. 4-5. Figure 4 is showing one possible position of the stage and  TEM lamella holder during the plain lamella attachment. Figure 5 is showing another possible position of TEM holder  for inverted lamella attachment. The grid holder has a  predefined angle towards TEM grid, they are not parallel.  After  rotating the holder 180° for inverted lamella thinning, the  thinning is performed 180° from the top surface, while the grid  bracket hardware does not interfere with FIB during the  thinning process.


In following paragraphs, we present complete workflows for  advanced TEM sample preparation techniques for  semiconductor industry using our proposed variable angle grid  holder. All of that was done in-situ without venting the chamber  and by using a simple nanomanipulator with fixed tip rotation, using standard TESCAN FIB-SEM instrument.


Figure 4: Variable angle holder position for plain lamella  attachment. 1 – SEM column, 2 – FIB column, 3 – GIS, 4 – sample holder, 5 – TEM grid holder, 6 – sample stage rotation. Real SEM Wide Field picture is shown too.


Figure 5: Variable angle holder position for inverted lamella  attachment. 1 – SEM column, 2 – FIB column, 3 – GIS, 4 – sample holder, 5 – TEM grid holder, 6 – sample stage rotation. Real SEM Wide Field picture is shown too.


Examples of various preparation workflows


Here we are showing some selected examples of TEM sample  preparation workflows. We have selected front side, back side  and planar TEM sample preparation process. More ways are  still possible due to the flexibility of the combination of stage  tilt angle/TEM holder tilt angle. During the preparation process, TEM sample can be easily observed by SEM, see Figs. 6-8 as  examples. These images were intentionally acquired in Wide  Field scanning mode, to maximize SEM field of view and to  show the position of TEM holder and the main stage towards  SEM beam.


Definition of angles is following: stage tilt angle is measured  towards the horizontal plane, TEM grid angle is measured  towards the sample carousel top plane. SEM column axis is  vertical and the angle between SEM and FIB column axes is 55° (for TESCAN FIB-SEM instruments).


Figure 6: SEM Wide Field picture of variable angle holder  position for lamellae FIB processing and in-situ front side SEM  inspection.


Figure 7: SEM Wide Field picture of variable angle holder  position for lamellae FIB processing and in-situ opposite side  SEM inspection.


An example workflow 1


Front side TEM sample preparation + SEM (R-STEM) observation:


1. Prepare the TEM sample for lift-out


2. Perform the lift-out at stage tilt angle 55°


3. Attach TEM sample at the grid holder at stage tilt


angle 55° and grid tilt angle 90°


221


10 mm


4. Perform polishing of TEM sample at stage tilt angle  55° ± FIB tapering angle


5. Change both stage tilt angle and grid tilt angle to 0°, to  get TEM lamella perpendicular towards SEM


6. Check the transparency and quality of the lamella by  SEM imaging.


7. Is the lamella finished?


8. If yes, finish the procedure. If not, change grid tilt  angle to 90° and return to point 4.


Figure 8: SEM Wide Field picture of variable angle holder  position for lamellae STEM analysis.


An example workflow 2


Back side TEM sample preparation + SEM (R-STEM) observation:


1. Prepare TEM sample for lift-out.


2. Perform the lift-out at stage tilt angle 0°.


angle 0° and grid tilt angle 70°.


4. Change grid tilt angle to -110°.


5. Perform polishing of TEM sample at stage tilt angle


55° ± FIB tapering angle.


6. Change grid tilt angle to 105°, to get TEM lamella


perpendicular towards SEM.


7. Check the transparency and quality of the lamella by


SEM imaging.


8. Is the lamella finished?


9. If yes, finish the procedure. If not, change grid tilt


angle to -110° and return to point 5.


An example workflow 3


Metrology for process development and monitoring capability  as 3D NAND layer counts increase can be effectively enabled  by an automated gas-enhanced PFIB delayering and SEM  inspection workflow. Plasma FIB tools such as the Helios G4  PFIB HXe DualBeam used for this work provide a convenient, single tool solution to access channel etch metrics as a function  of etch depth. For example, the commercially available 3D  NAND die examined here exhibits decreased etch uniformity  as a function of depth. While presumably the decrease in  uniformity does not compromise device performance, the  trends suggest improved channel etch process control will be  critical for enabling 3D NAND architectures with increased  layer counts. Furthermore, the scope of this work demonstrates  only a subset of the information-generating capability of these  kinds of workflows.


Potential extensions of automated 3D NAND delayering and  inspection workflows include mapping variation across and  within wafers due to the large sample sizes permitted. This can  permit a more global view of within-wafer etch process  variation as a function of depth and location on the wafer, thereby enabling process modifications for enhanced yield.


The authors acknowledge Sophia Weeks and Peter Carleson  for fruitful conversations and defining and implementing key  automation framework features that enable this workflow.


[1] Tilson, A., Strauss, M., “STEM/EDS Metrology and  Statistical Analysis of 3D NAND Devices,” Proc. IEEE International Symposium on the Physical and  Failure Analysis of Integrated Circuits (IPFA) (2018).


[2] Smith, N.S., Skoczylas, W.P., Kellog, S.M., Kinion, D.E., Tesch, P.P., Sutherland, O., Aanesland, A., Boswell, R.W., “High brightness inductively coupled  plasma source for high current focused ion beam  applications,” J. Vac. Sci. Technol. B 24, 2902 (2006)


[3] Carleson, P., Donnet, D., Sidorov, O., Rue, C. “Delayering on Advanced Process Technologies  using FIB,” Proc. ISTFA (2014)


[4] M. Ledoux, J. Clarke, B. Avedisian, C. Rue, and M. Adiga, Umesh M. Biedrzycki, “Gas-enhanced PFIB  surface preparation enabled metrology and statistical  analysis of 3D NAND devices,” Proc. SPIE 10959, Metrology, Inspection, and Process Control for  Microlithography XXXIII, pp. 109590I, (26 March  2019)


231


FIB Enhancement of Mechanically Polished Cross-sections


Becky Holdford


Retired Failure Analyst


pfadiva@gmail.com, Garland, TX


On mechanically polished cross-sections, getting a surface  adequate for high-resolution imaging is sometimes beyond the  analyst’s ability, due to material smearing, chipping, polishing  media chemical attack, etc..  A method has been developed to  enable the focused ion beam (FIB) to re-face the section block  and achieve a surface that can be imaged at high resolution in  the scanning electron microscope (SEM).


Mechanically polished cross-sections of semiconductor  packages are a common occurrence [1] in the industry and can  usually provide the detail needed for inspections of various  process parameters and/or failure mechanisms.  But sometimes  one needs a better surface for inspection than ion milling or wet  etching can give. Ion milling and wet etching processes tend to  attack interfaces and can cause some confusion when the  interface is the area of interest.  This paper presents a method  of FIB surface clean-up of samples that at first glance seem to  be too thick to be approached with standard FIB methods.  This  method can also clean up the curtaining (striating, waterfall, veiling, etc.) that occurs when FIB cross-sectioning into ICs  containing tungsten vias or contacts.  This method will be  referred to in this paper as the ”clean-up cut”


Discussion of Method


Standard gallium-source FIB tools are limited in the depths one  can mill to in a reasonable amount of time with an acceptable  amount of material redeposition.  This depth is usually in the  20-50µm.  Most IC package cross-sections have thickness ranges from 3mm to 15mm, with most of the material being for protection and support. At first glance, it doesn’t seem that a FIB would be able to be used on this type of sample.  But by using an un-encapsulated cross-section and experimenting with the tilt and pattern placement, it can be done.


Most FIB tools use a 52° tilt to perform the initial rough cut and  have a maximum tilt of 60°.  By using this maximum tilt and  placing the pattern box down on the section face a cut can be  made on a section that would be too thick to cut from the top  surface.  This method will remove material smear and give flat  surface to the section face.  This enables the analyst to reveal  cracks, delaminations, and voids that might be obscured by  smeared material or polishing debris.


By making an un-encapsulated mechanical cross-section and  then determining the area of interest [2], the FIB cut can be  directed at that x-plane of the vertical section face.  This is  accomplished by tilting the sample so that the section face is at  an angle to the ion beam.  Normal FIB cuts are made with the  sample face normal to the ion beam, with the ion column being  at some angle (i.e., 52º) with respect to the electron column.  In  this method, the sample is tilted a small amount (8°) with  respect to the ion column, which will be making the cut at a  small angle to the surface of the section face.  This enables an  area of interest of approximately 10-30µm in depth to be milled  into a section face that might be 50mm in depth.   This area will  also be extremely flat and free of artifacts that can be induced  by wet etching or standard broad ion beam milling methods.


Method Steps


1. The cross-section is made and mechanically sectioned into the area of interest.  The sample shown here is mounted on a piece of glass slide with Allied High Tech EpoxyBond 110™.  The glass slide piece was necessary due to the small package size in relation to the sample chuck for mechanical polishing,


2. Sample is mounted and loaded into the FIB as one would do for a normal FIB section


3. Sample is tilted to the usual angle for making a FIB cross-section, usually 52°.


4. Sample face is imaged in SEM mode to find the area of interest.  See Fig.1.


5. Tilt sample to maximum, usually 60°,


6. Image sample face again in ion mode to locate approximate area of milling box.  See Fig 2.  This image already has the area of interest milled out at the solder ball-to-package interface.


7. The polish cut is used, not the rough cut.  The pattern box will need to be positioned slightly higher than the area of interest. One will probably need to experiment to find the correct position.  Experience make this easier, as does marking the top of the sample.


8. Milling conditions on an FEI xP835 dual beam:  Ion mode = 30kV, aperture = 6600 pA (or equivalent),si.mtr file, z-depth = 10-15 μm, x and y dimensions as needed.


9. When the cut is started, the tool will probably give an information box saying the sample is tilted 8º or that the milling angle is 8º.  Acknowledge this and start the mill


10. After the pattern is complete, tilt back to 52° and image as usual.


# FIB Enhancement of Mechanically Polished Cross-sections


232


Fig.  1:  SEM image of sample at a 52° tilt


A cross-section schematic view of the section face might be  helpful in visualizing the cut, see Fig. 4.


The sample in relation to the electron and ion beam during the  standard cut is shown the Fig. 5


The sample in relation to the electron and ion beam during the  clean-up cut is shown the Fig. 6.


Fig.  2:  Ion image of sample at a 60° tilt


Fig.  3: SEM image of sample with FIB cut


Fig.  4:  Cross-section schematic of cut


Fig.  5:  Beam-sample geometry for a normal cut


233


To reduce or eliminate FIB cut striations


When doing FIB cuts on substances that have dissimilar  materials in the stack, such as an integrated circuit with tungsten  vias, the harder materials mill slower than the softer ones and a  grooved cut face appears.  This is called by various name, such   as via veiling, waterfalling, or striations. This method can also  be used to reduce or eliminate this phenomenon.


Make a normal FIB cross-section of an area of interest with the  sample tilted to the usual 52°.


1. Make the cut as usual.


2. After the section is done, tilt to 60°.


3. Draw fine milling pattern (‘polish’) box in the area  desired.  It might take a little juggling to get it at the  right spot.


4. Run the pattern.


5. Image as desired.


Examples of Use


The next section includes some images of samples enhanced or “cleaned up” using this method.


Figure 7 shows a section of silver (Ag)-filled die attach epoxy  as mechanically polished and after the clean-up cut.  The smear  is gone and the Ag particles and voids can be clearly seen.


Figure 8 shows a section of high lead (Pb) solder being used as  a die attach.  Pb is very soft and notoriously hard to  mechanically section as it smears and picks up debris from the  polishing media.


Figure 9 is higher magnification of the cut are shown in Fig. 3. This is a cracked solder-to-package interface, which was not  visible on the mechanical polished section face.


Figure 10 shows a section of a gold (Au) ball on a nickel (Ni)-palladium (Pd) plated copper (Cu) leadframe that has been ion  milled after mechanical polish.  The lower image is after the  clean-up cut.  The grain structures of all materials can be clearly


Fig.  6:  Beam-sample geometry for the clean-up cut


Fig. 7:  Ag-filled die attach


Fig.  8: high Pb solder as a die attach.  Before image has been ion  milled.


Fig. 9:  high mag, image of the solder interface


234


seen; also, the small voids between the Au and Pd that are not  readily seen in the prior image.


Figure 11 shows a standard FIB cut of an IC before and after  the clean-up.  These cuts were made on a Zeiss CrossBeam 340.


I extend much appreciation to Joseph Fafata of the University  of Connecticut for making the CrossBeam images for me and  to Valery Ray of MEO Engineering Company for introducing  us.


I thank Fred Clark, retired Texas Instruments Kilby Labs  manager for letting me have time on the Thermo/FEI xP835  Dual Beam FIB to experiment with this concept and I thank Dr. Kejun Zeng of Texas Instruments Packaging Development for  making it necessary for me to develop it


[1] B. Engel, et al., Microelectronics Failure Analysis Desk  Ref., 5th edition, 2003, pp 473-492


[2] B. Holdford, FIB Clean-up of Un-encapsulated Crosssections, Microscopy and Microanalysis 2011, Late  Breaking Poster Session,


Fig. 10:  Au ball to NiPd plate over Cu


Figure 11:  Top image:  before clean up.  Bottom image: after clean  up.


235


# 3D-Printed Samples For EXLO/INLO Practice and Training


3D-Printed Samples For EXLO/INLO Practice and Training


Zachary A. Giannuzzi and Lucille A. Giannuzzi


EXpressLO LLC, Lehigh Acres, FL USA


Kathleen A. Gehoski and William J. Mahoney


The Pennsylvania State University, University Park, PA USA


Practice and training samples have been manufactured using  3D-printing methods. These 3D-printed samples mimic the  exact geometry of focused ion beam (FIB) prepared specimens  and can be used to help master ex situ and in situ lift out  micromanipulation methods.  An additively manufactured array  of samples yields numerous samples needed for repetition and  deliberate practice necessary to master the lift out and  micromanipulation steps. The 3D-printed samples are cost  effective and negates expensive FIB time needed to prepare FIB  specimens.


It is generally accepted that it takes 10,000 hours of deliberate  practice to become an expert performer [1,2].  While many  hours of practice are indeed associated with high levels of  performance, there can be large variability in the amount of  deliberate practice needed to master a particular task [3].  There  is also a big distinction between quantity vs. quality of practice  time. However, expert mastery may not be the goal. For  example, it has been argued that it takes only about 20 hours of  intelligent practice to perform “well enough for your own  purposes” [4]. It is obvious that repetition of correct execution  is needed to achieve some level of specific task competency.  Hours of deliberate practice are indeed necessary for learning  either the ex situ or in situ lift out technique used in focused ion  beam (FIB) specimen preparation.  While the execution of  proper FIB milling steps and methods are crucial, specimen  manipulation and the lift out processes also ultimately  contribute to the entire FIB specimen preparation and success  rates.  Thus, mastering the lift out process is a critical skill in  FIB specimen preparation.


The lift out technique itself may arguably be defined as two  major skills. The first step in the lift out method is specimen  removal from the bulk sample, and the second is  micromanipulating the specimen to an appropriate grid or  specimen carrier.  When discussing the overall lift out process, it is generally understood that the method includes both the lift  out or specimen removal and specimen manipulation to its  carrier or grid. There are two well-known lift out methods  associated with FIB specimen preparation: (i) ex situ lift out


236


(EXLO) performed outside or (ii) in situ lift out (INLO), or  micro-sampling, performed inside the FIB-based instrument [5-8].


As an example of the skill learning process, the performance  target level may consist of performing one or more successful  lift outs in a “reasonable” timeframe. Deconstructing the skills  for either EXLO or INLO manipulation requires (i) performing  proper FIB milling of the specimen, (ii) familiarity with stage  functions, manipulator motion, deposition geometry (INLO  only), and hardware and software controls, (iii) familiarity with  the probe to specimen interactions, and (iv) familiarity with the  specimen to grid interactions. It is important to know what  successful lift out and specimen manipulation resembles, so it  helps to have a coach, teacher, colleague, or consultant nearby  to help with corrective actions during the learning process. Practice is imperative to achieve the desired mastery level.  As  an example, first author (ZAG) started as a summer 2018 intern  new to lift out and by the end of his second work week  successfully manipulated > 20 particles per hour to a carboncoated grid using EXLO techniques.


One of the largest hurdles in attaining sufficient repetition for  lift out practice and training is the need for expensive FIB  instrumentation time to prepare the necessary specimens. Typical instrument costs to mill a single FIB sample (depending  on the laboratory organization and rate structure. i.e., university  vs. commercial) are anywhere from ~ $50-$2000. Thus, significant costs may be incurred for FIB lift out training. In  addition, high demand for instrumentation time makes it  difficult to even access the FIB over a reasonable timeframe. Thus, the training process may take weeks or months to  complete solely due to lack of instrument access. Hence, we  sought a way to create practice and training specimens using  additive manufacturing whereby each specimen is built up  above the substrate to mimic the exact size and geometry of  conventionally prepared FIB specimens. In this paper, we show  that 3D-printed specimens can be designed and used for lift out  practice and training.  By reducing expensive FIB time needed  to create the specimens, tens of lift out attempts may be  executed by first time users on an array of 3D-printed  specimens, decreasing the cost of training, shortening the  training time needed, and improving lift out and  micromanipulation success rates. 3D-printed samples were  manufactured using two-photon polymerization which  provided the required printing resolution [9].  The 3D-printing


237


(e.g., additive manufacturing) process and applications of these  specimens for EXLO and INLO are shown below.


A 20 µm x 7 µm x 1 µm specimen mimicking the dimensions  of a typical FIB specimen confined by FIB trenches was  proposed and drawn in a computer aided design (CAD) file and  then transferred into a stereolithography (STL) file for the 3D  printing and additive manufacturing of the sample. A schematic  diagram of the additive manufactured, and 3D-printed sample  and array of samples is shown in Fig. 1a and Fig. 1b  respectively. The logo is designed to be used as a fiducial mark  for the possibility of FIB vendor scripting automation. Note that  the 1 µm thick specimen in Fig. 1 is designed with the so called “U-shape” undercut already present. That is, there is no material  designed to hold the specimen at its bottom or on either side of  it except for a small tab of material on each side toward the top  of the specimen.  This geometry mimics a FIB specimen ready  for ex situ lift out [5,8] or the so called “micro-sampling” version of in situ lift out [6,7].


Figure 1: (a) A schematic diagram of a 3D-printed sample  containing a FIB-like 20 µm x 7 µm x 1 µm specimen with Ushape undercut. (b) A schematic diagram of an array of 3Dprinted samples.


Sufficient 3D-printing writing resolution is needed to create the  1 µm thick specimen desired.  Two-photon polymerization  methods provide the resolution and step sizes needed where the  finest x,y lateral resolution is ~ 500 nm and the finest z vertical  resolution is ~ 1500 nm [9].  A commercial Nanoscribe  Photonic Professional GT was used to print the samples onto a  10 mm x 10 mm Si substrate. Each 3D-printed sample was  centered 100 µm apart to create an array of samples. Stage  control was used to move between samples, and beam scan  control was used to print each individual sample. The Si  substrate was cleaned and loaded into a custom machined  holder to accommodate up to 4 Si substrates at once. A small  drop of IP-Dip photoresist was deposited onto the center of each  substrate. The photoresist was polymerized and built up by  scanning and focusing the laser beam in x,y and at different z  heights according to the STL file. After the writing was  completed, the Si substrates were developed in AZ-EBR, rinsed  in isopropyl alcohol, and dried to leave the polymerized 3Dprinted sample array remaining on the Si substrate.


An FEI FIB 200 was used for sample FIB imaging and EXLO  specimen preparation. 30 keV Ga+ ions were used to obtain ion  induced secondary electron (iSE) images of the 3D-printed  samples. While polymeric photoresist is generally insulating, its  surface can easily be made conductive by FIB imaging at a  small dose of ~ 3 x 1015 ions/cm2 as shown in Fig. 2 obtained  using a nominal beam current of 1 nA.  This insulating to  conductive surface transformation in polymers is consistent  with an applied ion dose of 5 x 1014 – 5 x 1016 ions/cm2 and its  mechanism has been attributed to a localized surface increase  in carbon from sputtering and decomposition of the polymer  analogous to pyrolysis [10].


As shown in Fig. 2, with the necessary applied Ga+ ion dose, the sample surface grayscale brightens and thus the 3D-printed  polymer sample surface transforms from insulating (see Fig. 2a) to conductive (see Fig. 2b and also Fig. 3a). Note the 3D-printed  lift out sample confined within the additive manufactured  trench walls mimics the size, shape, and geometry of a “real” FIB specimen. The application of these 3D-printed samples for  lift out training is detailed below.


238


Figure 2: 30 keV Ga+ iSE images of (a) insulating and (b) conductive sample after applying a dose of ~ 3 x 1015 ions/cm2.


3D-Printed Samples for EXLO


For EXLO, all that is required to ready the 3D-printed samples  for lift out is to FIB mill the tabs of material holding the  specimen above the “U-shaped” designed undercut. This  procedure only takes a few seconds per sample using a small  rectangular pattern (~ 0.2 µm x 2 µm) and a beam current of  100 pA. Milling the tabs free produces a free-standing specimen  held inside its trench via only Van der Waals forces [8].  That  is, the adhesion forces between the small area edges of the  sample and the trench wall(s) are sufficient to keep the sample  in place and generally upright after it is FIB milled free.  Figure  3 shows 100 pA iSE images after the tabs have been FIB milled  free and ready for EXLO of (a) a single 3D-printed specimen  and (b) an array of 3D-printed specimens. Note the asymmetric  undercut that is also possible with the 3D-printed samples. That


is, a tab of material can be viewed at the “top” of the specimen  such that it can be used in the for practice and manipulation into  a backside configuration if desired [8]. The 3D-printed samples  FIB milled for EXLO were removed from the FIB and mounted  on an EXpressLO Nicola 640 ex situ lift out and  micromanipulation station.  Figure 4a shows a 3D printed  specimen lifted out via an EXLO probe. Once lifted out or “picked” from its trench, the specimen can be placed onto a  carbon-coated grid (Fig. 4b) or onto a self-supported slotted  grid (Fig. 4c) [8].  The 3D-printed sample manipulated to the  slotted grid (Fig. 4c) may also be further FIB milled to practice  final or low energy polishing. The conventional EXLO  processes are quick and easy and practicing on an array of 3Dprinted samples mimics the manipulation process necessary for “real” FIB-prepared specimens.


Figure. 3: 100 pA iSE images of (a) a single 3D-printed  specimen and (b) an array of 3D-printed specimens FIB milled  free for EXLO.


239


Figure 4: (a) EXLO of a 3D-printed sample after FIB milling.


(b) EXLO manipulation to a carbon-coated grid. (c) EXLO  manipulation to a patented EXpressLO grid.


As evident by the images in Fig. 4, the EXLO manipulation of  these 3D-printed polymer specimens works similarly to the  EXLO manipulation of a Si-based integrated circuit, metal, ceramic, or any other material as long as the sample, probe, and  sample carrier (i.e., grid support) has a smooth surface.  EXLO  may be applied to “any” material because Van der Waals forces  are ~ 12 orders of magnitude larger than the force of gravity for  these sample dimensions [8].  Van der Waals forces govern the  EXLO process and not electrostatic forces as previously  thought. Indeed, whenever possible, excessive attractive or  repulsive electrostatic forces should be minimized by  metallizing the tip. One can metallize the glass probe by either  sputter coating a conductive layer onto the probe [8] or by  dipping the end of the glass probe into carbon dispersed in a  solvent [8,11].  In addition, the material dependent Hamaker  constant governing Van der Waals forces varies by only 2  orders of magnitude across the periodic table and therefore any  change in material is insignificant for surface adhesion which is ~ 12 orders larger than the force of gravity on these specimens  as denoted above.  Note also that the EXLO procedure relies on  balancing surface area from lift out to manipulation. The  sample remains in the trench due to adhesion forces via just the  sample corners touching the trench wall(s) but is removed from  the trench when the larger surface area probe touches the  sample. The grid support offers even larger surface area than  the probe, so the sample is easily transferred from the probe to  its carrier.


3D-Printed Samples for INLO


An FEI Quanta 3D FIB SEM equipped with a Pt gas injector  system and an Omniprobe micromanipulator was used to  demonstrate the usefulness of the 3D-printed samples for  INLO.  Figure 5a shows a 50 pA iSE image of a 3D-printed  sample after one tab was FIB milled free.  Figure 5b shows a  100 pA iSE image of a 3D-printed sample attached to the probe  using Pt deposition and milled free from the trench. Figure 5c  shows a 100 pA iSE image of a 3D-printed sample manipulated  and attached to an Omniprobe grid using Pt deposition with the  probe FIB milled free of the specimen.   The images in Fig. 5  show the usefulness of the 3D-printed samples for practicing  INLO methods in addition to EXLO methods.  The 3D-printed  sample may also be further FIB milled to practice final or low  energy polishing.


The 3D-printed samples designed mimic the exact geometry of  FIB prepared lift out specimens and can be used for practice and  training of either the ex situ or in situ lift out process. These 3Dprinted samples mimic lamellae-type FIB specimens, but other  geometries such as plan view or atom probe types can also be  printed. 3D-printed FIB teaching aids can help new FIB users  learn lift out steps in a timely and cost-effective manner, easily  repeating lift out steps without the need for creating expensive  FIB specimens.


Figure 5: iSE images of a 3D-printed sample used for INLO  steps: (a) one material tab FIB milled free. (b) probe attached  with Pt deposition and specimen fully FIB milled free. (c) specimen manipulated to grid and attached with Pt deposition  with probe FIB milled free.


Thanks to Bob Stephano for machining the multi-substrate  sample plate.  EXpressLO™ grids and methods are covered by  US Patents 8,740,209 and 8,789,826. The 3D-printed Praxis™ specimen design, method of production, and its applications are  patent pending.  The INLO work was performed on an FEI Q3D  located at the University of South Florida.  The FIB 200 is  available via collaboration from TSS Microscopy.


[1] Ericsson K. A., Krampe R. T., & Tesch-Romer C., “The  Role of Deliberate Practice in the Acquisition of Expert  Performance,” Psychological Review, Vol 100, No. 3, (1993), pp. 363-406.


[2] Gladwell M. Outliers-The Story of Success, Little, Brown  and Company, (New York, 2008).


[3] Macnamara B. N., Hambrick D. Z., & Oswald F. L., “Deliberate Practice and Performance in Music, Games, Sports, Education, and Professions A Meta-Analysis.” Psychological Science, Vol. 25, (2014), pp. 1608–1618.


[4] Kaufman J. (The First 20 Hours - How to Learn  Anything...Fast, Penguin Group, (New York, 2013).


[5] Giannuzzi L.A., Kempshall B.W., Schwarz S.M., Lomness  J.K., Prenitzer B.I., & Stevie F.A., “FIB Lift-Out Specimen  Preparation Techniques,” in Introduction to Focused Ion  Beams, Giannuzzi L.A. & Stevie F.A. (Eds.), Springer, (New York, 2005), pp. 201-228.


[6] Kamino T., Yaguchi T., Hashimoto T., Ohnishi T. & Umemura K., “A FIB Micro-Sampling Technique and a  Site Specific TEM Specimen Preparation Method,” in  Introduction to Focused Ion Beams, Giannuzzi L.A. & Stevie F.A. (Eds.), Springer, (New York, 2005), pp. 229-246,


[7] Mayer J., Giannuzzi L.A., Kamino T. & Michael J., “TEM  Sample Preparation and FIB-Induced Damage,” MRS  Bulletin, Vol 32, (2007), pp. 400-407.


[8] Giannuzzi L.A., Yu Z., Yin D., Harmer M.P., Xu Q., Smith  N.S., Chan L., Hiller J., Hess D., & Clark T., “Theory and  New Applications of Ex Situ Lift Out,” Microsc. Microanal., Vol. 21, (2015), pp. 1034–1048.


[9] Kawata S., Sun H.B, Tanaka T. & Takada K., “Finer  Features for Functional Microdevices,” Nature, Vol. 412, (2001), pp. 697–698.


[10] Loh I.H., Oliver R.W. & Sioshansi P., “Conducting  Polymers by Ion Implantation,” Nuclear Instruments and  Methods in Physics Research, Vol. B4, (1998), pp. 337-346.


[11] Giannuzzi L.A., & Clark T., “Optimizing Van der Waals  Forces for FIB ex situ Lift Out,” Microsc. Microanal., Vol. 23, (2017), pp. 306-307.


# Low Energy Xe+ PFIB Specimen Preparation for Cs-Corrected HRSTEM Imaging


Low Energy Xe+ PFIB Specimen Preparation for Cs-Corrected HRSTEM Imaging


Lucille A. Giannuzzi, Paul A. Anzalone


TESCAN USA, Warrendale, PA USA


Jiancun Rao


University of Maryland, College Park, MD USA


Tom Hoffman, Mike McKie, Joseph Girgis, Takayuki Kuwahara


JEOL USA, Peabody, MA USA


Jamie Ford, Douglas M. Yates, Eric A. Stach


The University of Pennsylvania, Philadelphia, PA USA


Low energy (i.e., 5 keV, 3 keV) Xe+ plasma FIB methods  were applied to Si ex situ lift out specimens. Cs-corrected  STEM imaging reveals the Si dumbbell structure indicating  excellent surface quality achieved during the low energy  polishing steps.


Ga+ focused ion beam (FIB) low energy milling techniques  developed years ago are now routinely used to prepare  specimens for aberration corrected high resolution electron  microscopy [1]. Low energy polishing methods reduce ion  implantation and/or amorphization damage while decreasing  the specimen thickness [1,2]. Similar specimen preparation  methods can be applied using Xe+ ions from a plasma FIB (PFIB) source for transmission electron microscopy (TEM)


[3]. The heavier mass Xe+ ions result in a larger sputter yield, but smaller ion range, yielding fast specimen preparation of  thin specimens with reduced surface damage [2,4]. In this  work, low energy Xe+ PFIB polishing techniques are used to  minimize surface damage in Si required for visualization of  the Si dumbbell structure via Cs-corrected STEM imaging.


Since not all equipment needed was physically located within  one laboratory, we used multiple sites to perform this work. An FIB 200 (e.g., single beam Ga+ FIB) located at EXpressLO  LLC was used to mill 6 Si samples to a thickness of ~ 750 nm  using 30 keV Ga+ ions.  This thickness is well over an order of  magnitude larger than the Ga+ ion implantation range, and  thus, subsequent low energy polishing with Xe+ ions  completely removed any evidence of Ga+ ion implantation. An  EXpressLO Nicola 640 was used to manipulate all 6  specimens to a slotted grid using ex situ lift out [5].


Figure 1: (a) A light optical image and (b) iSE image of the  same specimens manipulated to an EXpressLO grid via ex situ  lift out.


Planar TEM sample preparation + SEM (R-STEM) observation:


1. Prepare the TEM sample for lift-out.


222


angle 0° and grid tilt angle 0°.


4. Change grid tilt angle to 90°.


6. Change grid tilt angle to 35°, to get TEM lamella


angle to 90° and return to point 5.


The paper demonstrates a showcase of preparation methods for  different TEM lamella types. Presented solution offers


versatility and brings significant advantage in its simplicity of


the TEM sample preparation process. Besides the standard  front-side lamella, also planar and inverted lamellae geometries  can be reached using the variable angle holder, even without the  need of nanomanipulator equipped with rotary tip. The


preparation process is done completely in-situ and end-point  detection from both sides of the lamella and using various SEM  detector signals is available.


This research was supported by the Technological Agency of  Czech Republic *TE 01020233 (AmiSpec).


[1] F. Lenrick et al., “FIB Plan and Side View Cross-Sectional  TEM Sample Preparation of Nanostructures”, Microsc.


Microanal. 20 (2014), pp. 133–140.


[2] Ch. Li et al., “An improved FIB sample preparation  technique for site-specific plan-view specimens: A new  cutting geometry”, Ultramicroscopy 184 (2018), pp. 310-


317.


[3] A. Denisyuk et al., “Artefact-free top-down TEM lamella


preparation from a 14 nm technology IC”, Conference


Proceedings from European Microscopy Congress (2016),


pp. 594-595.


[4] J. Lindsay et al, “Practicality of Single Microscope Failure


Analysis for Fault Isolation, Analysis and Advanced TEM


Sample Preparation by the Integration EBAC and EDS on


FIBSEM”, ISTFA 2017: Conference Proceedings from the  43rd International Symposium for Testing and Failure


Analysis (2017), pp. 265-269.


1 mm


Optimisation of large chunk lift-out method and lamella preparation for CBED  measurements using Xenon Plasma FIB


Miloš Hrabovský, Tomáš Morávek, Chandran Narendraraj


TESCAN Brno, s.r.o., Libušina třída 1, 62300 Brno, Czech Republic  e-mail: milos.hrabovsky@tescan.com


Jürgen Gluch, Martin Gall, Ehrenfried Zschech


Fraunhofer Institute for Ceramic Technologies and Systems IKTS, Maria-Reiche-Str. 2, 01109 Dresden, Germany


Uwe Mühle


Institute of Materials Science, TU Dresden, Helmholtzstr. 7, 01069 Dresden, Germany


As the new generation of microelectronics is pushed into  smaller spaces and the yield production is pushing to lower the  unoccupied spaces on chips, the local variation of stress has an  influence on the component’s performance. This stress comes  mainly from different thermal and mechanical properties of  the materials used especially in 3D integrations like through  silicon via (TSV) technology [1]. Through finite element  simulation [2] the internal strain profile was modelled and  based on these findings we devised a simulation model for a  large area chunk lift out, to preserve the stress inside the  material.


Standard preparation method for strain measurement is to use  a wafer dicing saw and subsequently focused ion beam (FIB) milling, to create lamellae with a defined geometry, close to  the desired TSV. This method requires different equipment  and knowledge base to achieve a lamella which is still  contaminated by Gallium. Therefor we developed our own  method based on an FE model of a large chunk lift out, where  only a Xenon Plasma FIB is utilized until the local stress  measurement using convergent beam electron diffraction (CBED) is measured in a transmission electron microscope (TEM).


Strain engineering of FET devices and advanced packing  using 3D TSV integration are both dependent on our ability to  determine the local strain in silicon used for these kinds of  applications. Integration of Copper and silicon causes a stress  distribution around the TSV, because of their different thermal  expansion coefficients and anisotropic mechanical properties. The cause of this stress has been described by a finite element  simulation [3].


CBED on a TEM is a difficult method to characterize localstress state of the sample, but it is no of the most reliable and  accurate methods [4-6]. For the CBED measurement we need  a suitable lamella with the corresponding thickness to our  primary TEM energy 200 keV which is around 200 nm to get  nicely visible and defined diffraction pattern like in the Figure


1. The preparation of such lamella changes the boundary conditions of the stress field and causes stress relaxation of the


surrounding material in the vicinity of the region of interest


[7]. Therefore, the influence of the stress on the lamella had to  be modelled using a finite element method and compared to  CBED measurement on samples prepared this way [1].


The stress state can be then calculated by measuring the  distance rKbetween the bright and dark Kikuchi lines of the  Zero Order Laue Zone (Zolz) corresponding to the analysed  lattice planes dhkl:


dhkl=(λ∙L)/rK


where λ is the wavelength of the electrons and L is the camera  length. The strain εhkl is given by:


εhkl=(dhkl-d0,hkl)/d0,hkl


where d0,hkl represents the lattice distance in the unstrained  state, measured at the reference lamella using identical  conditions.


The main motivation for using only a FIB-SEM to prepare the  sample was to reduce number of different processes involved  and to open the possibility for semi or fully automated process  in the future. Thanks to high current plasma FIB sources the  milling of large area samples has become much faster and  reliable option of preparation than ever before.


Figure 1: CBED pattern within the lamella with the (800) [1] diffraction line used for lattice plane distance measurement.


# Optimisation of large chunk lift-out method and lamella preparation for CBED measurements using Xenon Plasma FIB


223


Chip out of a Si wafer of thickness around 750 µm and 100  orientation with TSVs was used in this case study.


First step was to select our region of interest (ROI) and cover  it with a protection layer of platinum deposited by using  focused electron beam induced deposition (FEBID) followed  by focused ion beam induced deposition (FIBID). This double  layer of platinum was not only our protection layer but also a  navigation point through the whole process of milling, welding and final thinning of the lamella (for conditions see  table 1).


Table 1: Beam settings for FIBID, FEBID, glue hardening and  milling presets.


We must ensure that the copper inside the TSV is not milled  by the ion beam to preserve the strain inside it. The second  step is to prepare a set of trenches with pretilt to the  perpendicular axis (in our case 55 degree) of ±3 degrees, near  our ROI using a high current rough milling (for conditions see  table 1), the undercut trench has to be around 250 µm long, 150 µm wide and at least 100 µm deep to ensure a good  undercut at 0 degree tilt. The main trench must be slightly  deeper and wider than the undercut trench, which resulted in  the same length 250 µm, but the width is 200 µm and it is 175 µm deep to accommodate for the angle of 55 degree during  undercut at chunk thickness of 75 µm. With 100 polishing  cycles for each milling stairs with bending factor of 0,3 this  process for Silicon should not take longer than 2 hours.


The sample is than tilted back to 0 degree and undercut using  rough milling preset. The width of the undercut should be at  least 20 µm, so the redeposited material does not close the  opening back up. Once the undercut is done we highly  recommended the tilt back to 55 degree for a quick polishing  of the side of the chunk facing the main trench and the  opening left after the J undercut, to avoid uneven sidewalls  due to redeposited material of hitting the trench during lift out (the other side of the J cut will be polished during the cut off  and the undercut side of the chunk does not pose a problem  during lift out).


After the undercut is done a nanomanipulator needles needs to  be attacked to it. To avoid long process time SEMGLUE was  implemented for this process. It is important that a low energy  low current mode is used during any operation in which it is  necessary to image the glue. For this purpose, we used the  navigation preset for all our work to avoid hardening at  unnecessary times (for conditions see table 1). The needle is  simply pushed into the glue which can be placed anywhere on  any sample (we prefer a spare piece of silicon for the  adjustment of the plasma FIB and glue holding). Once the  needle is moved into the position where it touches the sample  a small glue bridge is formed between the chunk and the  needle. This small bridge has to be handed using a Glue  hardening preset for between 5 to 10 minutes, it is really  important to use the 30 keV SEM conditions to penetrate the  glue entirely so the secondary electrons can crosslink the  polymer and harden it to a point that it can be used to hold  down lamellas and chunks of material.


After the hardening is done simply use a polishing rectangle to  cut of the remaining bridge between the chunk and the rest of  the sample. Once the chunk is lifted out of the sample it will  look like the one on Figure 2.


Figure 2: Chunk of Silicon with TSV inside of it prepared by  xenon plasma FIB and attached via SEMGLUE to the  nanomanipulator needle.


The chunk is transferred to the desired grid position where it is  attached to the grid by using platinum FIBID deposition or  SEMGLUE (to apply the glue to the grid use the  nanomanipulator needle and slowly scrape some of it on the  grid finger following the same safety instructions as for the  needle attachment). It is important that the chunk is not


Beam settings


Process


Energy Current Step size Dwell time


FEBID


5 keV 1 nA


50 nm


1 µs


Navigation  5 keV 10 pA -


Glue


hardening


30 keV 1 nA


10 µs


FIBID


15 keV 240 pA 100 nm 1 µs


Rough  milling


30 keV 2 µA + 200 nm 1 µs


Rough


polishing


30 keV 100 nA 200 nm 1 µs


Polishing 30 keV 1 nA


100 nm 1 µs


Fine


30 keV 100 pA 50 nm


224


sticking out of the grid, so we recommended using slightly  thicker grids like 120 µm.


Once the chunk is cut off from the needle the ROI itself can be  thinned down to the desired thickness of around 200 nm for  the CBED measurements, with respect to the modelled strain


lamella. It is very important that the thinning doesn’t cut


through the whole chunk but follows a predefined angle of  entry, which preserves the strain inside the lamella and allows  the TEM observations and measurements (Fig. 3.).


The main entry is done using a trapezoid polygon with the  angle of around 35 degrees and depth of around 10 µm using  the rough polishing preset. After the main entry is done and  the thickness of the lamella is around 10 µm it is subsequently  thinned down more using the polishing preset, it is very  important not to cut into the TSV during this process, so the  stress is not released inside the sample.  After the lamella is  thinned down to around 500 nm it is slowly polished to the  desired thickness of 200 nm using the fine polishing preset to  ensure low curtaining (plasma FIB tend to have problems with  curtaining) and low amorphic layer (Xenon has much lower  amorphization of material than Gallium even on high  energies). Our lamella is 5 µm long, 5 µm deep and 200 nm  thick after all the process employed here. It is necessary to  have proper openings so the incoming electron beam of the  TEM for the CBED measurement is not shadowed or scattered  during the observation (to achieve diffraction we need to  employ beta tilt on the sample see reference [1] for more). If  done correctly this whole process should be under 3 hours and  should look like the one on figure 4.


Figure 3: Chunk lift-out method for stress lamella  preparation.


Figure 4: Final thinned down chunk with lamella welded on  top of a grid.


FE simulation and TEM measurement


The optimization of the process was to lower the time required  for the whole process and to still maintain the same level of  strain inside the lamella. That is why we modelled both the Hbar and the chunk using FE modelling, results can be seen on  figure 5. and 6., and from the findings we were able to obtain  the size of the chunk with length of 150 µm, height of 150 µm  and thickness of 75 µm. As you can see in the graph (Fig. 7.) the strain inside the chunk is identical in all the X, Y and Z  directions to the one of the H-bar normally used for CBED  strain measurements.


Figure 5: 3D rendering of the H-bar model for with the stress  lamella prepared by gallium FIB


225


Figure 6: 3D rendering of the chunk with lamella prepared  using Xenon plasma FIB.


Figure 7: Comparison of the strain state in both TEM  lamellae for all directions.


Figure 8: Comparison of the strain state measured in both  TEM lamellae prepared by Gallium and Xenon FIB in  different depths of the lamella.


The CBED TEM measurement on a sample prepared by wafer  dicer glued on a C grid and thinned down by Gallium and  Xenon plasma FIB can be seen on Figure 8 in three points  with different distances from the TSV and in two different  depths from the top of the lamella (0.3 µm and 1 µm). There is  a change of strain between the Gallium and Xenon prepared  lamella but is not so significant.


The Xenon plasma FIB preparation of large lamellas (chunks) for local strain analysis in Silicon using TEM CBED is  feasible, and a correction procedure of stress release caused by  the preparation of electron transparent lamellae is possible. Considering the lamella geometry and applying FE modelling  it is possible to interpret the measured data and to draw  conclusions on the original stress state before sample  preparation.


However, the slight change of strain inside the lamellae  between the Gallium and Xenon plasma FIB preparation can  be accounted to the rougher nature of the plasma FIB and that  is why the process should be monitored more carefully and the  preparation of samples using this method has to be monitored  closely.


This work was supported by the Technological Agency of  Czech Republic *TE 01020233 (AmiSpec) and CATRENE  project MASTER_3D. TSV manufacturing has been  performed by Fraunhofer IZM- ASSID.


[1] M. Hrabovský et al.; Correction of stress release during sample preparation for TEM CBED measurements,ISTFA 2018: Conference Proceedings from the 44th International Symposium for Testing and Failure Analysis(2018), 358-362.


[2] L.W. Kong, A.C. Rudack, P. Krüger, E. Zschech, S.


Arkalgud, A.C. Diebold; 3D-interconnect: Visualization of extrusion and voids induced in copper-filled throughsilicon vias (TSVs) at various temperatures using X-ray microscopy; Microelectronic Engineering 92 (2012) 24-28 Doi 10.1016/j.mee.2011.04.012


[3] Kteyan, A., Mühle, U., Gall, M., Sukharev, V., Radojcic,R., and Zschech, E., “Analysis of the Effect of TSV Induced Stress on Devices Performance by Direct Strain and Electrical Measurements and FEA Simulations,”IEEE Transactions on Device and Materials Reliability 17(2017), p. 4, doi:10.1109/TDMR.2017.2732826


[4] Wittmann, R., Parzinger, C., and Gerthsen D.,“Quantitative determination of lattice parameters from CBED patterns: accuracy and performance,” Ultramicroscopy 70 (1998), pp. 145-159, doi:10.1016/S0304-3991(97)00107- 1


[5] Morawiec, A., “An algorithm for refinement of lattice parameters using CBED patterns,”Ultramicroscopy 107(2007), pp. 390-395; doi:10.1016/j.ultramic.2006.10.003


[6] Stuer, C., Van Landuyt, J., Bender, H., Rooyackers, R.,and Badenes, G., “The use of convergent beam electron diffraction for stress measurements in shallow trench isolation structures,” Materials Science in Semiconductor Processing 4 (2001), pp. 117-119, doi:10.1016/S1369-8001(00)00110-4


[7] Vanhellemont, J., De Wolf, I., Janssens, K.G.F.,Frabboni, S., Balboni, R., and Armigliato, A., “On the assessment of local stress distributions in integrated circuits,” Applied Surface Science 63 (1993), pp. 119-125, doi:10.1016/0169-4332(93)90075-M


226


Automated gas-enhanced PFIB surface preparation enabled metrology and  statistical analysis of 3D NAND devices


Chris Hakala, James Clarke, Mark Biedrzycki, Kesley Price, Jamie Johnson, Gavin Mitchson


Thermo Fisher Scientific, Hillsboro, OR, USA


The development of vertical 3D NAND technology over the  past 5 years has been accelerated by the parallel development  of metrology techniques capable of characterizing these device  stacks. Current trends point toward a continuous scaling of  dimensions along the z-axis, involving a critical etch step with  aspect ratios of ~50:1. These high aspect ratio process steps  present both fabrication and metrology challenges where the  channel holes can bend, bow, and pinch off throughout the  stack. Work presented herein demonstrates the capability of an  automated workflow developed using the Thermo Scientific™ Helios™ G4 HXe DualBeam™ platform. The workflow  iteratively exposes desired layers within the NAND stack, collects high resolution SEM images, and performs metrology  to enable statistical analysis of trends as a function of depth  within the stack. Results will be presented from 3 sites in an  automatically delayered 72-layer 3D NAND die. Automated  SEM metrology was performed every 10 layers, capturing  more than 6000 devices. Over 19000 measurements were  made on imaged devices yielding assessment of statistically  significant trends in the planar cell area, eccentricity, and  position of the bits as a function of depth.


3D NAND


Thanks to the 3D NAND architecture, manufacturers of the  technology have a clear vision toward the future of nonvolatile flash memory. Current trends indicate further  increasing the depth of the stacks will provide a higher bitdensity within the same planar layout. Potential process issues  can manifest as bowing, bending, and pinching of the  cylindrical channel pillars, which lead to device malfunction. These types of defects typically occur during the high aspect  ratio pillar etch step. Developing a process robust to these  defects requires strict process controls and monitoring, but  detecting these types of defects is difficult using standard  metrology methods.


In the electronics domain, focused ion beam (FIB) technology  provides methods for site-specific exposure of buried devices, thereby enabling extraction of critical dimension information  from a given device. Traditional FIB methods produce  diagonal, vertical cross-sectional (Fig. 1), or plan-view slices  through a 3D NAND stack. The latter two are often used in  conjunction with TEM inspection, which yields important  information at the expense of turn-around time. [1]


Figure 1: Cross-Sectional SEM image taken on die used for  this work.


Plasma FIB


More recent developments in the realm of plasma FIB (PFIB) technology have enabled new FIB inspection workflows  relevant to 3D NAND manufacturers. Modern PFIB currents  can reach the µA range, enabling large area processing in  substantially less time than is possible using conventional  LMIS Ga+-FIB technology. [2] Plasma FIB also enables the  use of Ga+-incompatible chemistries for gas-assisted  processing. Previous work demonstrates the ability of plasma  FIB to delayer Logic and 3D NAND devices layer-by-layer, providing periodic in situ SEM inspection as a function of  depth. [3,4]


The Helios G4 PFIB HXe DualBeam provides a path toward  layer specific inspection of the 3D NAND technology  commensurate with the projected metrology needs as device  architectures scale. The delayering process enables  measurement of planar cell area, eccentricity, and position of  the bits as a function of depth. Analysis of this data provides  process insights and enables identification of defects  including, but not limited to, the critical high-aspect ratio etch  step.


Automation


High throughput process monitoring is critical for any  semiconductor manufacturing process. Development of  automated inspection techniques that approach in-line  efficiency are crucial for the continued growth of


# Automated gas-enhanced PFIB surface preparation enabled metrology and statistical analysis of 3D NAND devices


227


manufacturers. The following work demonstrates the ability of  a Helios G4 PFIB HXe DualBeam to automatically delayer  and inspect 3D NAND technology. Through improved data  volume and throughput, process engineers will be able to make  critical decisions earlier and with more certainty than ever  before.


One key enabler for automating this process is the endpoint  detection system. Endpoint detection is accomplished by  current monitoring as measured on the stage. Peaks and  troughs are observed in a plot of the current vs. time as milling  progresses through layers in the NAND structure (Fig. 2). The  endpoint detection system analyzes the plot in real-time and  detects peaks and troughs. Endpoint type can be either peak or  trough, and the number of those peaks or troughs can be  specified before the pattern is stopped. Specific layers in the  NAND structure can be delayered to and inspected utilizing  this endpoint method.


Figure 2: Graph of endpoint monitor signal with results of the  real-time peak and trough detection algorithm.


Sample


A commercially available 72-layer 3D NAND device was  purchased on the open market and de-packaged prior to in situ  modification. Sites were selected to represent physically  separated locations across the 3D NAND die (Fig. 3).


At each site, the 3D NAND stack was iteratively delayered and  imaged with the SEM in 10-layer intervals. The first SEM  images of metallized word line layers were collected at layer  12 and continued through layer 72 as illustrated in Figure 4. Selection of beginning and ending layers and sampling  frequency is configurable in the automated workflow. This  represents a sample of 14,739 devices on which more than  50000 measurements were taken. Analysis of the  measurements reveals statistically significant trends in cell  metrics as a function of channel depth and location on die.


Figure 3: Optical image of 3D NAND die as mounted in a  Helios G4 PFIB HXe DualBeam with overlay of site locations.


Figure 4: Graphic representation of sampled layers with SEM  images representing the 3D NAND device at layers 12, 42 &


72.


Recipe


Automated delayering is enabled by Thermo Scientific iFast™


Automation Software. The software uses a site processing  framework for multi-site operation. At each site, four site  processing blocks (SPBs) are executed, shown at high level  overview in Figure 5. This includes a setup block that enables  initial configuration of the workflow at that site.


The second SPB isolates the region of interest from the  surrounding circuit using the FIB to mill a frame around the  region of interest (ROI). The third SPB places and performs a  gas-assisted mill using the Dx Delayering™ etch chemistry  until the initial endpoint layer is reached. Once the initial  endpoint layer is reached the recipe proceeds to the fourth SPB  where the workflow alternates between layer removal and  SEM image acquisition. The scanning electron micrographs  are saved to disk and processed for metrology metrics  separately offline.


228


Figure 5: Screen capture of the iFast Software workflow  demonstrating the high-level site processing framework.


Metrology


For the purposes of this study, 3 types of measurements were  extracted from the scanning electron micrographs acquired  during the automated workflow (Fig. 6). The first set of  measurements was generated using an Arc Finder ellipsefitting routine in iFast Software to extract cell area, major and  minor axis lengths, and eccentricity. The second set of  measurements used the cell perimeters defined by the Arc  Finder routine for nearest neighbor measurements. Finally, an  EdgeFinder routine provided the third set of measurements: distance from edge-most cells to the edge of the word line.


The SEM measurement capabilities were evaluated on 3D  NAND devices in previous work and are calculated to provide


1.4 nm resolution and 1.04 nm 3-sigma static precision. [4]


Figure 6: Graphic representing the types of measurements  performed for the scope of this work. Edge distance  measurements were performed for both top and bottom edgemost cells.


Results & Discussion


Area & Eccentricity


Mean cell area as a function of depth (layer number) for each  delayered site is shown in Figure 7. In previous work [1,4], there were clear declining trends from top to bottom of the  stack. Within scope of the current work, mean cell areas are  generally consistent for the first 52 layers, but decrease  substantially between layer 52 and 62. This suggests that, although the channels do not pinch off near the bottom of the  stack, the channel etch uniformity could be improved. While  adequate for production of this 72-layer device, the process  will likely require modification to enable successful channel  etches as the layer count is expected to increase for next  generation 3D NAND. There is some variation in mean cell  area between sites, but all three sites exhibit the same  precipitous drop in mean cell area between layers 52 and 62.


Figure 7: Site*Layer interaction plot for area mean.


Eccentricity data (Fig. 8) shows that channel eccentricity  increases as a function of depth. Eccentricity is a descriptor of  ellipse circularity. An eccentricity of 0 indicates a perfect  circle, while an eccentricity approaching unity indicates an  increasingly elongated ellipse. The overall distribution of  eccentricity values as well as representative cells with  minimum, median, and maximum eccentricity are shown in  Figure 9. Whereas the channel areas are relatively consistent  between layer 12 and layer 52, the eccentricity increases  continuously for all three sites between layer 22 and layer 62. There is minimal site-to-site variation in mean eccentricity  values at each layer. The variation in cell eccentricity also  increases with depth. This is consistent with the conclusion  from assessment of the channel areas as a function of depth  and again suggests decreased etch uniformity as the etch depth  increases.


229


Figure 8: Left: Site*Layer interaction plot of mean  eccentricity at each layer, split by site. Right: Standard  deviation of eccentricity vs. layer.


Figure 9: Distribution of eccentricity measurements grouping  the entire experimental set of data. The colored points along  the top correspond to images below representing the  minimum, median, and maximum eccentricity measurements.


Nearest Neighbor


Nearest neighbor measurements split by the measurement type, horizontal or vertical (refer to Fig. 6), indicate differences in  distance between cells with differing separation vectors. Similar to the observations made regarding channel areas, the  mean Site*Direction interaction in Figure 10 indicates some  site-to-site differences in mean nearest neighbor  measurements, but all sites and layers exhibit similar  decreased vertical separation relative to horizontal separation.


Figure 10: Site*Layer interaction plot for nearest neighbor  mean.


Edge Distance


The edge distance measurements are summarized in Figure 11. Between layers 12 and 42, the edge distances are statistically  equivalent. Between layers 52 and 72, the mean edge distance  increases and the variation in edge distances also increases. Increasing edge distance with depth suggests that the channels  bow or bend away from the word line edges towards the  bottom of the stack. Generally, these observations are  consistent with the observations from channel area and  eccentricity as a function of depth and also suggest decreased  etch uniformity as the etch depth increases.


Figure 11: Variability chart for edge distance measurements.


230


241


Figure 1a shows a light optical image of 5 of the 6 specimens  manipulated to an EXpressLO grid. The grid was returned to  the FIB 200 and a C deposition attachment layer was added to  each sample as a precaution to prevent possible sample loss  during transport prior to Xe+ ion milling. A Ga+ ion induced  secondary electron (iSE) image of the specimens after  manipulation is shown in Fig. 1b.


The specimens were transported to the University of Maryland  where a TESCAN XEIA instrument was used for final Xe+ PFIB thinning.  The specimens were directly thinned to  electron transparency by milling on both sides of the specimen  using 5 keV Xe+ ions at 80o incidence angle from the XEIA  PFIB source as shown in the schematic diagrams in Figs. 2a,b. On the XEIA instrument, this incident angle was achieved  with a stage tilt of +/- 10o from a FIB SEM working stage tilt  of 55o (i.e., 45o for side 1 and 65o for side 2). This was  followed with a low energy polish using 3 keV Xe+ PFIB  milling at 80o incidence on each side to further thin the  specimen while replacing 5 keV damage with shallower 3 keV  Xe+ damage.  Secondary electron SEM (eSE) images of the Si  samples after 5 keV milling and 3 keV milling are shown in  Figs. 2c,d respectively. These low energy Xe+ ion polished  specimens were then transported to the University of  Pennsylvania for STEM imaging with a Cs-corrected JEOL  NEOARM operating at 200 keV.


Simultaneous bright field (BF) and high angle annular dark  field (HAADF) Cs-corrected STEM images of the low energy  Xe+ PFIB Si polished specimens were obtained and are shown  in Figs. 3a,b.  Note the obvious [110] Si dumbbell structure  indicating excellent surface quality of the Xe+ PFIB prepared  specimen.


A [110] Si HAADF STEM image and intensity profile is  shown in Figs. 4a,b respectively.  The intensity profile in Fig. 4b was obtained from the region outlined in Fig. 4a. Note the  obvious 136 pm distance of the Si dumbbell splitting as shown  indicating excellent surface quality obtained using the low  energy Xe+ PFIB polishing.


Low energy Xe+ PFIB methods were successfully used to  prepare high quality Si specimens for Cs-corrected STEM  imaging. The heavier mass Xe+ ions are stopped closer to the  surface and therefore may produce a shallower depth of  damage layer than lighter Ga+ ions at the same energy. Inert  PFIB generated Xe+ ions may usurp reactive Ga+ FIB usage  for S/TEM specimen preparation.


Figure 2. (a,b) Schematic diagrams of low energy polishing at  80o incidence angle on each side of a specimen. SEM eSE  images of Si EXLO specimens after (c) 5 keV Xe+ PFIB  milling and (d) 3 keV Xe+ PFIB milling performed on each  side.


242


Figure 3. Simultaneous (a) BF and (b) HAADF STEM images  of Si [110] dumbbell structure.


The FIB 200 is available courtesy of TSS Microscopy. The  STEM imaging was performed in part at the Singh Center for  Nanotechnology at the University of Pennsylvania, a member  of the National Nanotechnology Coordinated Infrastructure (NNCI) network, which is supported by the National Science  Foundation (Grant NNCI-1542153) and through the  University of Pennsylvania Materials Research Science and  Engineering Center (MRSEC) (DMR-1720530).


Figure 4. (a) HAADF STEM image and (b) intensity profile of [110] Si showing the dumbbell splitting.


[1]  Giannuzzi L. A., Geurts R. and Ringnalda J., “2 keV Ga+ FIB Milling for Reducing Amorphous Damage in  Silicon,” Microsc. Microanal. Vol. 11, Issue S02 (2005), pp. 828-829.


[2] Bassim N., Scott K., and Giannuzzi L.A., “Recent  advances in focused ion beam technology and  applications,” MRS Bulletin, Vol. 39 (2014), pp. 317-325.


[3]  Giannuzzi L. and Smith N., “TEM Specimen Preparation  with Plasma FIB Xe+ Ions,” Microsc. Microanal. Vol. 17, S2 (2011), pp. 646-647.


[4]  Kelley R.D., Song K., Van Leer B., Wall D. and  Kwakman L., Microsc. Microanal. Vol. 19, S2 (2013), pp. 862-663.


[5]  Giannuzzi L.A., Yu Z., Yin D., Harmer M. P., Xu Q., Smith N.S., Chan L., Hiller J., Hess D. and Clark T., “Theory and New Applications of ex situ Lift Out,” Microsc. Microanal. Vol 21, Issue 4 (2015), pp. 1034-1048.


243


Localizing IC Defect Using Nanoprobing: A 3D Approach


Jane Y. Li, Chuan Zhang, John Aguada, Christopher Nemirow and Howard Marks


NVIDIA Corporation, Santa Clara, CA, USA   janli@nvidia.com


This paper demonstrates a methodology for chip level defect  localization that allows complex logic nets to be approached  from multiple perspectives during failure analysis of modern  flip-chip CMOS IC devices. By combining chip backside deprocessing with site-specific plasma Focused Ion Beam (pFIB) low angle milling, the area of interest in a failure IC device is  made accessible from any direction for nanoprobing and  Electron Beam Absorbed Current (EBAC) analysis. This  methodology allows subtle defects to be more accurately  localized and analyzed for thorough root-cause understanding.


During failure analysis of a flip-chip IC, defect localization via  nanoprobing is normally performed from either the frontside or  the backside of the die. In certain circuit-layout scenarios, however, the information provided by planar-electrical-probing  is inadequate for accurate localization of some subtle defects. Cross sectioning of the die using FIB offers another channel for  nanoprobing to gather critical additional information for defect  localization. This multi-dimensional failure analysis approach  has proven to be invaluable in determining the root-causes of  subtle failures in advanced IC devices. A case-study is provided  to demonstrate the benefits of this approach.


Localization of failures in advanced IC devices


Devices with systematic yield issues were submitted for failure  analysis. Photon-emission microscopy (PEM), performed on  multiple chips, showed the same failure signature: abnormal  emission at the same site of similar cells. The emission image  with the called-out suspect cells at the emission sites and the  related input /output nets are shown in Fig. 1.


Figure 1. PEM image showing emission spots at failure site (a); and CAD layout showing the called-out suspect cells at the two  emission spots and the associated input and output nets across  multiple interconnect layers (b).


# Localizing IC Defect Using Nanoprobing: A 3D Approach


244


1) Analysis Approach: Frontside vs. Backside


EBAC is a technique for defect localization in metal nets. A  nanoprobe is landed on the net and monitored for current while  an electron beam is scanned over the net. By mapping the  detected current to the electron beam position, the location of  any shorts, electrical opens or resistive defects in the net can be  located.


Traditionally, EBAC is used from the die frontside. There are  several disadvantages to this approach, however: 1. Layer by  layer de-layering to expose the metal traces is both timeconsuming and labor intensive. 2. It’s difficult to maintain the  planarization of each metal layer over a large area during plapping. 3. The probe can only be landed on the highest exposed  metal layer of the net, making it difficult to detect a defect near  the end of the net or a defect causing resistive open.


The backside approach, on the other hand, is much more  effective. With the entire net preserved after silicon removal  from the die, an opportunity of landing the probe tips on both  the driver and receiver ends of the net at the transistor level is  provided for effective EBAC analysis and two-probe resistance  measurement of the net(s) of interest [2-4]. Defects near the  ends of the nets or those causing resistive opens can be found  without ambiguity. The planarity achieved with backside deprocessing also allows p-lapping to be performed layer-by-layer  upwards to expose metal traces with superb flatness over a large  area. Defects in higher metal layers are therefore exposed in a  controlled manner for maximum preservation of details for  SEM imaging and analysis [3, 4].


2) Frontside I-V characterization and SEM inspection:


One device was deprocessed using parallel lapping from the die  frontside after the die was removed from the flip-chip substrate. The goal was to perform transistor nanoprobing in the suspect  cells to check for transistor level failures. Because the top view  layer-by-layer inspection is ineffective for detecting via  interface issues, only optical inspection was performed during  de-layering to check for obvious defects. No defects were  observed. At the contact level, the transistors within the suspect  cells at the emission sites were characterized using  nanoprobing. Normal I-V characteristics were measured, ruling  out defects within the transistors themselves.


3) Backside nanoprobing and SEM inspection:


A second failure part was de-processed from the die backside. Here, the silicon substrate was removed using mechanical  thinning followed by TMAH wet chemical etching [3,4] to  expose backside of the FinFET structures in the emission area. As shown in Fig. 2, all transistors level structures were situated  perfectly near the surface within reach for SEM imaging.


To perform EBAC, further polishing was performed to remove  the gates and expose the gate and diffusion contacts. Backside  EBAC analysis was performed using a single probe-tip landing  on the drain or gate end of the nets. No abnormality was found. Figure 3 shows the results from one of the measurements. The


entire net exhibited normal continuity. The deeper (e.g., higher  metal layer) portions of the net is not shown in this image since  a low e-beam incident voltage of 0.5kV was used.


2-point IV nanoprobing was then performed between the  terminals of the nets at the contact level to measure the  resistance of the nets. One of the suspect nets was found to have  a significantly higher resistance compared to an adjacent  reference net with the same layout design. As shown in Fig. 4, further 2-point nanoprobing between terminals in this net  showed similar high resistance between terminals A-C and  terminals B-C, suggesting the presence of a resistive defect  within the common current path segment between terminals  A-C and terminals B-C as circled by the green dotted line in  Fig. 5. To localize the resistive defect along the isolated  segment, two-terminal EBAC analysis was further performed  by landing a signal probe and a ground probe on both ends of  the resistive segment, but no EBAC signal was observed. The  majority of the electrons from the incident e-beam flowed  across the resistive defect to the ground probe instead of getting  collected by the signal probe, since the resistance of the defect  was not very high. Alternative approaches were required for  further localization.


Figure 2. Schematics illustrating backside deprocessing (a); and SEM backscattered electron image of the emission area  from backside of the die (b)


Package  Substrate  Si


Package  Substrate


245


Figure 3. Backside EBAC results (SEM/EBAC overlay image)


Figure 4. IV-curve acquired from 2-point backside nanoprobing


Figure 5. 3-D schematics of the backside nanoprobing to  isolate the resistive segment


Cross-sectional Nanoprobing


To localize the defect in the common current path between  terminals A-C and terminals B-C, the sample was crosssectioned in a Helios DualBeam Xe-PFIB/SEM at the location  of the cross-sectional plane shown in Fig. 6 (a).


To achieve this, the die was first cut using a diamond saw a few  millimeters away from the area of interest (AOI), then ground  using a mechanical polishing wheel to less than 50 µm away  from the AOI. This was followed by PFIB milling to expose the  suspect part of the trace for cross sectional probing.


2-point I-V nanoprobing was subsequently performed by  landing the probes on the exposed metal 3 from the crosssection, as shown in Fig. 6 (b). The nanoprobing results shown  in Fig. 7 indicated a resistive path, further isolating the resistive  defect to be within a segment consisting of M3-V3-M4-V3-M3.


Figure 6. 3-D schematics showing the target cross section  plane (a); and nanoprobing of the resistive segment (b)


246


Figure 7. SEM image showing 2-point cross sectional  nanoprobing on the suspect net (a); and I-V curve acquired  from 2-point cross-sectional probing (b)


Within the resistive segment M3-V3-M4-V3-M3, the M4 and  M3 segments can be eliminated from previous top-down  inspection results on another chip with the same failing  signature. Therefore, the resistive defect must be at one of the  two V3 vias. In order to isolate the defect to the exact location, further PFIB low angle milling was conducted until the top edge  of M4 was exposed, as shown in Fig. 8a). This enabled  nanoprobing of individual segments contacting the two V3 vias  by probing two of the three terminals shown in Fig. 8b).


Figure 9a) shows the SEM view of the cross-section and the  three terminals that were probed. Figure 9b) shows the 2-point  IV test results. A high resistance was measured between  terminals B and C, which includes the entire M3-V3-M4-V3-M3 stack. While a low resistance was measured between  terminals A and C, a high resistance was found between  terminals A and B. That suggests the resistive defect is between  terminals A and B, namely the V3 via in between. With this  level of isolation, a cross-sectional TEM specimen could be  prepared to capture the defect.


Figure 8. Schematics showing the further target cross section  plane (a); and nanoprobing of the resistive segments (b)


247


Figure 9. SEM image showing 2-point cross sectional  nanoprobing on the suspect net (a); and I-V curve acquired  from 2-point cross-sectional probing (b)


Figure 10. TEM image of the high resistance V3 via. A Cu void  is revealed at the bottom interface.


Physical Analysis


A TEM lamella was prepared to image the resistive V3 via. The  TEM image revealed Cu voiding at the bottom interface of the  via, as shown in Figure 10.


This paper demonstrates a “3D” nanoprobing approach for  defect localization in a CMOS IC. Combining traditional silicon  de-processing techniques with the site-specific pFIB milling  makes it possible to probe any segment of a net in the IC, allowing a defect to be accurately isolated for physical analysis. This method has proven itself to be effective at isolating  difficult failures that could not be found using more traditional  approaches.


[1] Ma Y., Oh C.K., Nyi O., Zhang C., Nedeau D, Lim S.K., Chu K.M., “Nanoprobing as an Essential and Fast Methodology  in Identification of Failure’s Root Cause for Advanced  Technology”, Proc 37rd Int’l Symp for Testing and Failure  Analysis, San Jose, CA November 2013, pp.249-254


[2] K. Dickson et. al., “Electron Beam Absorbed Current as a  Means of Locating Metal Defectivity on 45nm SOI  Technology,” Proc 36th ISTFA, November 2010, pp. 413-422.


[3] Jane Y.L et. al., “Backside De-processing of Integrated  Circuits 40 nm and Below”. Proc 37th ISTFA, November 2011, pp. 242-247


[4] Jane Y.L et. al., “Capturing Defects in Flip-Chip CMOS  Devices Using Backside EBAC Technique and SEM  Microscopy”, Proc 42th ISTFA, November 2016, pp.112-118


248


A Novel Approach to Unsupervised Automated Extraction of Standard Cell  Library for Reverse Engineering and Hardware Assurance


Ronald Wilson, Rabin Y. Acharya, Domenic Forte, Navid Asadizanjani and Damon Woodard


Florida Institute for Cyber Security, University of Florida, Gainesville


{ronaldwilson, rabin.acharya}@ufl.edu, {dforte, nasadi, dwoodard}@ece.ufl.edu


Reverse engineering today is supported by several tools, such  as ICWorks, that assist in the processing and extraction of  logic elements from high definition layer by layer images of  integrated circuits. To the best of our knowledge, they all  work under the assumption that the standard cell library used  in the design process of the integrated circuit is available. However, in situations where reverse engineering is done on  commercial off-the-shelf components, this information is not  available thereby, rendering the assumption invalid. Until  now, this problem has not been addressed. In this paper, we  introduce a novel approach for the extraction of standard cell  library using the contact layer from these images.  The  approach is completely automated and does not require any  prior knowledge on the construction or layout of the target  semiconductor integrated circuit. The performance of the  approach is evaluated on two AES designs with 10,000 cells  compiled from standard libraries with 32nm and 90nm node  technologies having 350 and 340 standard cells respectively. We were able to successfully extract 94% and 60% of the  standard cells from the 32nm and 90nm AES designs using the  proposed approach. We also perform a case study using a realworld sample extracted from a smartcard. Finally, we also  investigate the various challenges involved in the extraction of  standard cells from images and the steps involved in resolving  them.


Reverse engineering is essentially defined as the in-depth  analysis of an end product to reveal its functionality and the  techniques involved in its manufacturing. This information is  exploited in several ways ranging from re-manufacturing of  legacy devices to defending Intellectual Property (IP) rights. In case of semiconductor Integrated Circuits (IC), the reverse  engineering (RE) process requires three major steps: identifying the device technology from images of the chip  taken layer-by-layer using scanning electron microscope (SEM), extracting its gate-level netlist and inferring its  functionality [1]. The first phase of the reverse engineering  paradigm involves imaging to recover the node technology  employed in its design and obtain a heuristic on the design  rules used to produce the IC. The second step involves  matching the patterns found in the active, polysilicon, contact  and metal 1 layers to a standard cell library and extraction of  the netlist. This step also involves examination of the  remaining metal layers which show how the cells are


connected to each other in the design. The final step infers the  functionality of the circuit or a sub-circuit in the design. There  are a plethora of algorithms [2,3,4,5] and automated tools [6,7,8,9] that assist in the identification and extraction of logic  elements in the circuit. RE on gate design needs active, contact and metal 1 layers [10]. Inferring cell functionality  typically only requires the metal 1 layer [11].


Even though the paradigm is relatively straight forward and  simple, there are several limitations that makes RE hard to  execute. One such limitation is the requirement of a template  standard cell library to be present to extract the gates, filler, and flip flops in the netlist. To the best of our knowledge, all  existing algorithms and tools require some heuristic on the  standard cell library to work. With the goal of RE being the  extraction of information on the product with no prior  knowledge, this limitation is counterintuitive. In this paper, we  propose a novel method to address this issue.


Figure 1: SEM image showing noise in the polysilicon layer


There are several problems associated with the extraction of  standard cells from a given device. Some of them are  described below in detail:


• Image acquisition: In some layers, especially polysilicon,the noise intensity is too high (Fig. 1). This can only be counteracted by increasing the quality of the scan. In a typical imaging modality, like the SEM, a higher quality scan would extend the imaging time frame in the order of several days [12], and even months for advanced technology nodes.


• Alignment and Stitching: Due to nature of the imaging modalities used and the scale at which images are acquired (mosaicking), the layers may be misaligned [9].


• Intra-cell Similarity: In some standard cell libraries, there are extensive similarities between different cells (Fig. 2).


This inherent similarity might cause traditional machine learning algorithms to produce inaccurate results.


# A Novel Approach to Unsupervised Automated Extraction of Standard Cell Library for Reverse Engineering and Hardware Assurance


249


• Scale: With ever increasing levels of integration in IC, the  memory and time complexity involved in processing the  amount of data extracted from one IC is nearly  intractable. This holds true, especially, when each  potential cell pattern has to be compared against all the  cells in the library.


Figure 2: (a, b) Cells showing similarity in polysilicon layer


on the 32nm dataset. (c) Complicated shapes in poly-silicon  layer on the 90nm dataset.


Our contribution in this paper is two-fold. We investigate the  similarities between multiple cells from two standard libraries  and discuss the infeasibility of machine learning based  methods on unsupervised automated cell extraction. Furthermore, we introduce a novel rule-based method that can  successfully extract the standard cell library from just the  contact layer in the IC. The results and limitations of our  approach are also discussed.


With the strict control on the availability of industry-use  standard libraries, we have based our experiments on two  standard cell libraries that can be readily reproduced: 32/28nm  Educational Design Kit [13] and Synopsys open educational  design kit [14]. These libraries contain 350 and 340 standard  cells corresponding to 32nm and 90nm node technologies  respectively. Using the libraries, an AES design was  synthesized into approximately 10,000 standard cells from  which we extract the contact layer as a segmented image. A  small section of the designs is shown in Fig. 3.


Figure 3: (a) AES design from 32nm dataset (b) AES design  from 90nm dataset


In addition, a separability test was performed on all the layers  associated with a standard cell for both datasets. The goal of  the test is to evaluate the extent of similarity between two  different cells from the same standard cell library. For layers  other than the contact layer, the images of layers where


convolved against each other and the point of maximum  correlation was recorded. For the contact layer, the N-gram  length was used. It is defined as the count of consecutive  columns of contacts in a cell. For instance, if the n-gram  length is 2, every two consecutive columns in the source cell  is compared against every two consecutive columns in the  target cell and the number of overlapping contacts is recorded. However, only the maximum number of overlapping contacts  between two cells for the chosen n-gram length is kept for the  final analysis. If the source or target cell does not have enough  contact columns to satisfy the chosen n-gram count, the cells  are ignored from the analysis. In Fig. 4 and 5, the correlation  of patterns for all cells with each other have been plotted.


As expected, the general trend for both plots are  monotonically decreasing. This can be attributed to the fact  that the number of possible combinations for each n-gram  increases with the considered length, making them more  unique in the space of all possible combinations. Another  interesting point is the major difference in correlation values  between the 90nm and 32nm datasets. The reason for this  drastic difference can be observed in Fig. 6. The contacts in  the 32nm dataset follow a grid-like arrangement with a  constant distance between each column. However, the distance  between two adjacent columns in the 90nm dataset is not  constant. This additional freedom of choosing the distance  between two columns make the combination more unique.


Figure 4: Correlation of patterns in various n-gram length for  the 32nm dataset


The raw correlation values for the other layers can be seen in  Fig. 7. As expected from the examples shown in Fig. 2, the  correlation for the polysilicon layer is much higher than any  other layer for the 32nm dataset. The 90nm dataset shows  similar correlation values for all layers. The observation  obtained from Fig. 7, supports the fact that active (diffusion), contact and metal 1 layers can be used to successfully reverse  engineer the IC and infer its functionality if the templates of  the standard cells are known. However, if it’s not available, the correlation within different layers also makes the features  extracted inherently correlated and inseparable for any  machine learning algorithm. With the primary goal for the


application of RE being the accurate and complete  reconstruction of features inside the IC, the correlation  between features must be avoided or dealt with in another  way.


Figure 5: Correlation of patterns in various n-gram length for  the 90nm dataset


Figure 6: (a) Non grid-like allocation of contacts on the 90nm  dataset in cell AND3x1. (b) Grid-like allocation of contacts on  the 32nm dataset in cell AND2x4.


Figure 7: Simple correlation plot for various layers in the


standard cell library. (PO: Polysilicon, M1: Metal 1, DL: Diffusion/Active layers)


The first step in the extraction of logic cells from the contact  layer is the detection of boundary between two cells. Typically, this can be done by considering the amount of free  silicon substrate between the columns of contacts. If the space  occupied by the silicon substrate is greater than a certain  threshold, the contact can be considered as belonging to two  different cells. There are two major flaws to this line of  thought. Firstly, some cells do have unusually long space  between adjacent contact columns and splitting them would  cause over-segmentation in the cell. Secondly, this approach  being well known, has prompted the development of several  anti-RE approaches. One of them being the insertion of  dummy but operational structures into these empty silicon  substrate locations [15]. This makes the boundary detection  solely based on the separation between contact columns  invalid.


Figure 8: Framework for the proposed algorithm


Our approach accomplishes the extraction of cell boundaries  by encoding the contacts into a vector and looking for unique  patterns in them. The framework of the proposed algorithm is  shown in Fig. 8 and the major steps discussed below.


Feature Encoding


There are two drawbacks to working on an image. The  space/time complexity involved in going through the image  and the noise introduced by the imaging modality. The spacetime complexity of the algorithm can be considerably reduced  by encoding the image into simple numerical vectors.


251


Figure 9: Illustration of features encoded by the algorithm


Each contact column in the AES image, shown in Fig. 3, is  encoded into a numerical vector using the distance between  each contact and the Vcc line. The distance is indicated as ‘d’ in Fig. 9. For instance, the red contact column in Fig. 9, would  have 8 values indicating the distance between the centroid of  each of its 8 contacts and the centroid of the Vcc line  highlighted in yellow. The Vcc line can be found either on the  contact layer or on metal 1. This should alleviate the  misalignment to a certain extent since the patterns are encoded  using a local point of reference. Following the encoding, every  three adjacent contact columns in the image are extracted and  saved along with the distances between them. This is depicted  in Fig. 9 where the distances between the columns are denoted  as d1 and d2. Even though the features are more unique with  longer sequences of columns, we have limited the count to 3. This is done to ensure that standard cells having just one  contact column can be detected. If the minimum number of  columns in a cell in the standard cell library is known  beforehand, this parameter can be changed to that value. If the  parameter is set to a value larger than the minimum sequence  length of contact columns, then all such cells will not be  detected.


Figure 10: Illustration of contacts extracted from a raw SEM  image using simple thresholding


In a typical imaging modality used in RE, like the SEM, the  contrast for metallic structures are much higher than nonmetals. This helps in the extraction of features even on noisy  low-quality images.  This is our motivation for considering  just the contact layer for the standard library extraction. In Fig. 10, a simple thresholding method was used to extract the  contacts from the SEM image. Any pixel having intensity  value less than 250 was filtered out.


Automated Extraction of Cell Height


The Vcc lines were extracted from the AES design using a  simple algorithm. It is to be noted that there exists a minimum


distance between two contacts on the Vcc line and distance  between two Vcc lines is always constant. We have exploited  this information to localize them. Firstly, we measured the  distance between contacts in the same row and calculated its  median value. Once this is done for every row in the design, the minimum value is taken. Secondly, every row that has  median separation equal to the minimum value is marked. The  respective plot is shown in Fig. 11. The periodic nature  associated with the constant separation between Vcc lines can  also be observed in Fig. 11. Since the separation between the  lines can be taken as an integral multiple of an arbitrary  integer, an arithmetic progression that best describes the  periodic nature is fitted to the plot. The common difference of  the arithmetic progression defines the cell height in the design. The result of applying this method is shown in Fig. 12.


Figure 11: Plot depicting the period nature of Vcc contact lines


Figure 12: Image showing the Vcc contact lines. Detected lines  are shown in red


Model Rules


The extraction of the standard library requires the application  of two rules. They are described below:


• The inter-contact distance rule: For any given cell, the  distance between its respective contact columns would be  the same, i.e., the d1 and d2 given in Fig. 9 would be the  same if the contact appears inside the cell. However, if the


252


columns appear on the boundary of the cell, the distance  would vary randomly. The information in this rule is  captured by the feature encoding.


• The start-end rule: The ending boundary of one cell is  always followed by the starting boundary of another cell. A contact column that doesn’t belong to a cell cannot  exist. Any detected boundary that does not satisfy this  rule will be ignored.


Since most imaging modalities used in RE captures the IC  layers in smaller images and stitches together to form a  mosaic, there are concerns for the detection of partial cells in  the contact layer. This problem is resolved by the start-end  rule since partial cells has either a beginning or an end and not  both. Partial cells detected at the edges of the image can be  ignored or flagged for further processing later.


Segmentation


Once the boundary features are detected, the cells can be  extracted from the image and added to a candidate library. However, with the application of start-end rule and presence  of noise in the image, some under-segmentation of the cell  might have occurred. To remedy this, the cells are compared  against each other. If a given cell can be expressed as the sum


of ‘n’ cells present in the library in any given order, they are


segmented.


Figure 13: Cells extracted by the algorithm. Blue lines mark  the boundary of the cell


Table 1: Summary of the results obtained from applying the  algorithm to the AES design


Node Technology


32 nm


90 nm


No. of Unique Cells  64


True Match


60 (94%)


27 (31%)


Partial Match


0 (0%)


33 (38%)


Failed Match


4 (6%)


The image shown in Fig. 13 shows the result of applying the  given rules to the segmented image. The boundaries extracted  by algorithm are highlighted in blue. Table 1 summarizes the  results of the experiment. In Table 1, True Match corresponds  to the extraction of the complete cell when compared to  ground truth. Partial Matches happen when compound cells


are detected. A compound cell is a combination of multiple  ground truth cells. Failed Matches happen when the detected  cells are over segmented versions of the ground truth cells.


As observed from Table 1, there is a significant deviation  between the cell extraction between 32nm and 90nm node  technologies. The reason for this discrepancy can be seen in  Fig. 6. The segmentation and extraction of cells is solely  depended on the encoded features. Since the AES design  based on the 90 nm node technology does not follow a gridlike arrangement of contacts, it is difficult to encode them into  a discretized feature space. Depending on the noise in the  image, the floating contact in Fig. 6 can be either included in  the current column or one of the adjacent columns. This  uncertainty in its absolute position causes the encoding to  change at times. Although inconvenient, the encoding is  necessary to reduce the complexity of the algorithm and  enable it to scale to present day billion transistor ICs.


The partial and failed matches are caused either due to oversegmentation or under-segmentation of standard cells. In the  AES design, there were situations where two standard cells  always occurred together. With the lack of variance in  distance measures for the encoded features for that specific  standard cell, they were grouped together causing a partial  match. Segmentation of cell only happen when evidence of  variation in distance in feature encoding is detected, i.e., d1 or  d2 must be different.


Figure 14: Image showing subset of similar sequences


(highlighted in red) between two different cells (a) AND2x2


(b) AND2x4


Failed Matches happen when a subset of contact columns  repeat across multiple standard cells or when variation in  encoded features occur due to floating contacts as shown in  Fig. 6(a). This can be easily remedied in design that follow a  strict grid-like allocation of contacts, thus, explaining the  higher rate of failed matches in the 90nm AES design. Fig. 14  shows an instance where the algorithm caused a failed match  due to over-segmentation.


A case study was performed on a real-world sample extracted  from a Smartcard using 190nm node technology. The image  was acquired using the TESCAN FERA3 dual-beam FIBSEM with imaging potential set at 12 kV for higher


253


penetration. Delayering was performed from the backside  using the approach described in [18]. Imaging at a higher  potential also helped reduce the influence of uneven  delayering. The acquired image is shown in Fig. 15. The other  imaging parameters such as magnification, dwelling time and  resolution were set to 100µm, 32µs/pixel and 1024x1024  pixels respectively.


Figure 15: A Raw SEM image of the contact layer


Figure 16: Binarized image of the contact layer with threshold  set at 225. All structures except the contacts are removed after  thresholding


Following acquisition, the image was binarized. Since the  contacts in the image are much brighter than the surrounding  structures, a simple thresholding was used to separate out the  contacts. No specific steps were taken to account for the  variation in size of the contacts due to depth. Any pixel in the


original image with value over 225 is taken as a pixel  belonging to a contact. The rest of the pixels are set to zero. The resultant binarized image is shown in Fig. 16. Following  the sequence of steps discussed in this paper, the image was  segmented into strips after detecting the Vcc power supply  lines. Some of the strips, after the extraction, is shown in Fig.


17. Finally, the rules were applied to the strip to extract the  standard cells. Some of the standard cells extracted are shown  in Fig. 18. The functionality of the cells was identified with  the help of a Subject Matter Expert.


Figure 17: Image showing strips of contact extracted from the  binarized image. The Vcc supply lines in the image are


removed after detection


Figure 18: (a) Some of the cells detected by the algorithm. The  conjoined cells are the result of limited data provided to the  algorithm in conjunction with the non-grid like arrangement


of contacts (b) Cells detected by the algorithm with their


functionality decoded by a Subject Matter Expert (SME). True  individual cells are highlighted in red bounding boxes.


In this paper, we were able to resolve a problem that has not  been addressed in RE and hardware assurance literatures- the  extraction of standard cell libraries from images of IC layers. With most of the existing algorithms concentrating on  matching extracted features to templates in libraries, the extent  to which effective RE can be performed was limited. We have  extended the scope of RE to ICs of completely unknown  architectures and provided a new avenue for RE research.


In conclusion, we were able to achieve our goal successfully  along with the following advantages:


254


• Extraction of the library was done only using information  from the contact layer. The features in this layer are  considerably more resistant to noise than other layers


[16].


• Using local landmarks for extracting features, we were  able to handle alignment problems in image mosaics up to  a certain extent.


• With the limited possible combination of contacts in the  layer and the encoding of images into feature space, the  number of features extracted are exponentially lower than  the number of gates in the IC thereby reducing memory  and time complexity.


• The approach is completely automated and does not  require any prior knowledge on the design rules of the  target IC. The only human interaction required is to  confirm the validity of the extracted cells. By automating  the process, we have also taken out biases and incorrect  annotation introduced by human factors.


In a future work, we will also be looking into improving the  cell extraction by incorporating information from other layers. This information will also be used to aid in automatically  identifying the cell’s functionality.


[1] Rostami, M., Koushanfar, F. and Karri, R., “A primer on


hardware security: Models, methods, and metrics”.


Proceedings of the IEEE, 102(8), 2014, pp: 1283-1295.


[2] Mark C. Hansen, Hakan Yalcin, and John P. Hayes. 1999.


Unveiling the ISCAS-85 benchmarks: A case study in


reverse engineering. IEEE Design and Test of Computers


16, 3, 72–80.


[3] W. Li, A. Gascon, P. Subramanyan, W. Y. Tan, A.


Tiwari, S. Malik, N. Shankar, and S. A. Seshia. 2013


WordRev: Finding word-level structures in a sea of bitlevel gates. In Proceedings of the 2013 IEEE ACM


Journal on Emerging Technologies in Computing


Systems, Vol. 13, No. 1, Article 6, Publication date: April


2016. 6:32


[4] W. Li, Z. Wasson, and S. A. Seshia. 2012. Reverse


engineering circuits using behavioral pattern mining. In


Proceedings of the 2012 IEEE International Symposium


on Hardware-Oriented Security and Trust (HOST’12).


IEEE, Los Alamitos, CA, 83–88.


[5]  P. Subramanyan, N. Tsiskaridze, K. Pasricha, D.


Reisman, A. Susnea, and S. Malik. 2013. Reverse


engineering digital circuits using functional analysis. In


Proceedings of the Conference on Design, Automation,


and Test in Europe. 1277–1280.


[6]  Torrance, R., & James, D. (2009, September). The stateof-the-art in IC reverse engineering. In International


Workshop on Cryptographic Hardware and Embedded


Systems (pp. 363-381). Springer, Berlin, Heidelberg.


[7] Kenneth, K. Yu, and C. Neil Berglund, U.S. Patent No.


5,086,477


[8] Ahmed, Haroon., Blythe, Simon and Fraboni, Beatrice,


U.S. Patent No. 5,191,213.


[9] Zavadsky, Vyacheslav L., Val Gont, Edward Keyes,


Jason   Abt, and Stephen Begg. U.S. Patent 7,580,557.


[10] Avery, L.R., Crabbe, J. S., Al Sofi, S., Ahmed, H., Cleaver, J. R. A., Weaver, D. J. 2002. Reverse  Engineering Complex Application-Specific Integrated  Circuits (ASICs), Proceedings of the Diminishing  Manufacturing Sources and Material Shortages  Conference (Mar. 2002).


[11] Nohl, K, Evans, D., Plotz, S., Plotz, H. 2008. ReverseEngineering a Cryptographic RFID Tag, USENIX  Security Symposium (Jul. 31 2008).


[12] N. Vashistha, M T Rahman, H. Shen, D L Woodard, N  Asadizanjani and M. Tehranipoor, Detecting Hardware  Trojans Inserted by Untrusted Foundry using Physical  Inspection and Advanced Image Processing Techniques, Publication pending in Spring Journal of Hardware  System and Security (HaSS), Tentatively December 1,


[13] Goldman, R., Bartleson, K., Wood, T., Kranen, K., Melikyan, V., & Babayan, E. (2013, December). 32/28nm  educational design kit: Capabilities, deployment and  future. In 2013 IEEE Asia Pacific Conference on  Postgraduate Research in Microelectronics and  Electronics (PrimeAsia) (pp. 284-288). IEEE.


[14] Goldman, R., Bartleson, K., Wood, T., Kranen, K., Cao, C., Melikyan, V., & Markosyan, G. (2009, July). Synopsys' open educational design kit: capabilities, deployment and future. In 2009 IEEE International  Conference on Microelectronic Systems Education (pp. 20-24). IEEE.


[15] Cocchi, R. P., Baukus, J. P., Chow, L. W., & Wang, B. J. (2014, June). Circuit camouflage integration for hardware  IP protection. In Proceedings of the 51st Annual Design  Automation Conference (pp. 1-5). ACM.


[16] Blythe, S., Fraboni, B., Lall, S., Ahmed, H. and de Riu, U., 1993. Layout reconstruction of complex silicon chips. IEEE journal of solid state circuits, 28(2), pp.138-145.


[17] Quadir, S.E., Chen, J., Forte, D., Asadizanjani, N., Shahbazmohamadi, S., Wang, L., Chandy, J. and  Tehranipoor, M., 2016. A survey on chip to system  reverse engineering. ACM journal on emerging  technologies in computing systems (JETC), 13(1), p.6.


[18] Principe, E.L., Asadizanjani, N., Forte, D., Tehranipoor, M., Chivas, R., DiBattista, M., Silverman, S., Marsh, M., Piche, N. and Mastovich, J., 2017, December. Steps  toward automated deprocessing of integrated circuits. In  ISTFA 2017: Proceedings from the 43rd International  Symposium for Testing and Failure Analysis (p. 285). ASM International.


255


A Review on Automatic Bill of Material Generation and Visual Inspection  on PCBs


Mukhil Azhagan M. S, Dhwani Mehta, Hangwei Lu, Sudarshan Agrawal, Mark Tehranipoor, Damon L. Woodard, and Navid Asadizanjani


Florida Institute for Cybersecurity (FICS), ECE Department, University of Florida, Gainesville  mukhil.mallaiyan@ufl.edu, nasadi@ece.ufl.edu


Praveen Chawla


Edaptive Computing Inc.


Globalization and complexity of the PCB supply chain has made  hardware assurance a challenging task. An automated system to  extract the Bill of Materials (BoM) can save time and resources  during the authentication process, however, there are numerous  imaging modalities and image analysis techniques that can be  used to create such a system. In this paper we review different  imaging modalities and their pros and cons for automatic PCB  inspection. In addition, image analysis techniques commonly  used for such images are reviewed in a systematic way to  provide a direction for future research in this area.


Index Terms—Component Detection, PCB, Authentication, Image  Analysis, Machine Learning


Outsourcing due to globalization is a dominant trend especially  in the electronic device and systems community. Printed circuit  board (PCB) manufacturing can cost up to millions of dollars. Therefore, many companies including Apple, Microsoft and  Amazon outsource the manufacturing [1].


PCBs form the foundation of an electronic system. They dictate  the specifications of the system such as computational power, networking capability and functionality. They are used in many  critical facilities and applications notably data centers, power  plants, hospitals, transportation, and military. This makes PCB  security extremely crucial.


Outsourcing the PCB manufacturing has given rise to a number  of vulnerabilities that did not exist before. Tampering, recycling, and cloning are just a few examples of such  vulnerabilities; a detailed taxonomy of counterfeit components  is presented in [2]. A counterfeit system can give backdoor  access to an attacker or enable other attacks such as IP piracy, aid data theft, and result in other creative attacks [1]. Although  outsourcing has reduced manufacturing costs, it has become a  serious security threat to the consumers and the companies  themselves. Fig. 1, describes the steps involved in the life cycle  of a PCB; from design to deployment and various  vulnerabilities at each stage. Malicious modifications are


possible at any stage. For instance, “in-field tampering”, which  is at the design and assembly level is very difficult to detect and  is extremely devastating. These vulnerabilities exist mainly  because it is almost impossible to fully monitor the design and  manufacturing process offshore.


While one solution is to bring stringent rules in manufacture  plants and have strict specifications during the design and  manufacture phases, the enforcement of such rules would be  impractical. It would involve cooperation across industries and  governments in various countries and would need to employ  trained supervisors to implement and monitor the process. Physical inspection, on the other hand, is a more feasible  approach as it involves only on-site verification under trusted  conditions.  Research in physical inspection is growing and  many approaches have already become mainstream  technologies for PCB verification [3] [4]; particularly for defect  detection using a golden sample. Physical inspection is mostly  noncontact and nondestructive, which makes it a favorable  approach within the community.


Physical inspection is usually employed in an “as needed” basis  as it currently requires human involvement and is a long and  time-consuming process. While there has been significant  research [4] on making it completely automated, using a bill of  materials file as an input to cross verify and validate the board  has not been attempted. In this paper, our contributions are  twofold, (i) an overview on imaging modalities is presented and (ii) image analysis techniques that can help extract the BoM automatically and analyze images for possible counterfeits are discussed in detail.


PCB Assurance Using Prominent Testing  Approaches


Conventional design and post manufacturing verification  methods cannot be readily used to detect hardware Trojans and  backdoor access points. There are various techniques such as


# A Review on Automatic Bill of Material Generation and Visual Inspection on PCBs


256


electrical testing, firmware testing, etc. that can be used to  identify some of these undesired modifications, but these  methods should be designed specific to the one type of PCB and  cannot be reused for another type. Dedicated quality assurance  agencies can provide PCB assurance services and perform these  electrical and firmware checks. However, using


conventional techniques, it is not possible to deliver a complete  vulnerability assessment. Any technique comes with a set of  limitations inherent to its methodology and none has proven to  be solely enough for verification.


Electrical testing is one of the most common verification  techniques. The functionality of the PCB is tested, and outputs  are authenticated for each component. However, this is a timeconsuming process as it requires a different set-up for different  PCBs. Hardware Trojans can be designed to trigger in specific  adversarial instances and cause performance degradation or  provide backdoor access; therefore, logic testing cannot be a


good method to detect them. The ‘Big Hack’ incident [1],


claimed such a hardware Trojan in 2018.


Another method to detect PCB vulnerabilities is firmware  testing using specification standards like JTAG (Joint Test  Action Group) [6]. While JTAG is able to identify if a PCB  deviates from its design specification, it would fail if the  maliciously implanted component is only keeping track of the  function of the PCB and not altering them. Therefore, it is  extremely challenging for firmware or electrical testing  approaches to provide a complete solution for hardware  assurance.


To have an assured PCB hardware, it is important to extract the  BoM in the first phase, and make sure there is no extra or  missing component on the board compared with the original  design. BoM can be extracted using visual inspection  techniques combined with image analysis algorithms.


Visual Inspection for PCB Assurance


Visual inspection is one of the most popular approaches for  PCB verification and authentication, and it is widely used in  various steps of the PCB lifecycle. Traditional visual inspection  is performed by a subject matter expert (SME), under controlled   conditions, and with limited aid from computer vision. They  analyze PCBs for defects and vulnerabilities, and cross-verify  their visual characteristics with a golden PCB sample. Traditionally, this is done before installation and only random  samples are tested. As the number of PCBs and the components  on the PCB grow, the approach becomes very time-consuming  and is prone to human error. Therefore, an automated approach  that can perform visual inspection is an immediate need to the  community.


The problem of PCB assurance encompasses not only defect  detection, but also detection of maliciously added components. Existing literature mainly include approaches for reliability  defect detection. Not all defects on the PCBs are due to  manufacturing errors, some are maliciously inserted to serve an  ulterior purpose. In the Big Hack news, a chip was maliciously  implanted on the motherboard [1]; it was similar to a signal  coupler in shape, but it was slightly larger and had a memory  system and a network chip within its packaging. Extracting the  BoM for such PCBs that can monitor the components’ dimension, location, and visual appearance is critical in such  cases.


Automatic Visual Inspection (AVI) is a growing field of  research, however different steps involved in AVI requires  further development and attention. AVI can be categorized into  two major areas, complementary to each other:


I. Imaging Modality: selection of an imaging mode that can  capture essential information for PCB authentication.


II. Image Analysis: detection and identification of  components/defects with 100% accuracy.


This paper will provide details on both areas in the following  sections.


Figure 1: The PCB supply chain. The red arrow represents the steps that potentially introduce defects and Trojan. The blue arrow  is the PCB inspection and quality control process that is necessary for PCB assurance [5].


257


I. Imaging Modalities


PCB assurance encompasses various levels. Defect detection on  components, identifying modifications of components, verifying netlist, are some examples of PCB assurance. Each of  these cases require specialized techniques utilizing different  spectrum of imaging. Different imaging modalities are  available for defect detection and failure analysis, that offer  both wide area imaging as well as closeup imaging. Some  modalities have a limited field of view and have inbuilt stitching  algorithms to stitch smaller images together to build a complete  picture. PCB imaging can be performed either over the surface  or through its volume. Each imaging modality can provide  additional side information and help identifying malicious  changes in a PCB faster.


There are three main categories of imaging modalities: Surface  Reflective, Surface Penetrative, and Volumetric. The following  sections will provide an in-depth discussion on these imaging  modalities, their operational costs and how they can help with  PCB assurance. Table I presents a summary of different types  of imaging modalities and in Fig. 2 examples of these  modalities are presented.


1) Surface Imaging: Within surface imaging, there are two  categories: reflective and penetrative, based on the penetration  power of the beam. For example, a digital optical microscope  will fall under reflective imaging, whereas terahertz imaging is  penetrative imaging due to its ability to image subsurface  information.


a) Reflective Surface Imaging: Reflective surface imaging  consists of sensing equipment that mainly works in the optical  spectrum and sometimes in infrared. There is a source which  emits EM radiation and a sensing equipment is placed near the  source that picks out the reflected rays to gain an understanding  of the surface characteristics. Based on these surface  characteristics, two different types of models can be built, a 2D  image or a 3D depth map. 2D images retain a high level of detail  in terms of color, texture, etc., whereas 3D images retain  information on shape, dimension and depth. Both of these are  useful for different instances of vulnerability detection and their  uses are presented below.


Digital Optical Microscope: This is the most used method for  visual inspection, quality assurance, and failure analysis of  PCBs. Digital microscopy is comparatively inexpensive and is  a practical approach to begin analysis and identify a majority of  reliability and security defects. Digital optical microscopes  enable variation in tilt, illumination, perspective, and 3D  surface imaging. Usually, the magnification of digital optical  microscope ranges from 2x to 200x, but it is also possible to  extend the range to 2400x by using special lenses.


Information such as serial numbers and components ID  numbers can be identified by a digital optical microscope. Defects such as scratches, alignment problems, damages to  package, leads, and components can be detected. Even ghost  markings often difficult to identify can be picked out. Inability  to see within packages and within layers of the board are  significant drawbacks of this modality. It usually takes seconds  to capture an image and depending on the size of the PCB and  the magnification level it can take considerable amount of time  to image all the areas on a large PCB and stitch them together. Most commercial microscopes offer good stitching algorithms  for this purpose.


Cameras: Recent advances in smartphone cameras, as well as  digital cameras, offer zoom capabilities up to 22x.


Cameras are very affordable for an end-user comparing with  most other modalities and offer great portability. Most  advantages of digital optical microscopes also translate to  cameras, except stability. Cameras either need to be mounted or  need stabilizers as compared to microscopes which offer  protection from vibrations by design. Cameras can be used for  most cases a digital optical microscope is used, but with the  trade-off of less accuracy.


While microscopes and cameras can provide 2D Images with  good resolution, they cannot accurately measure length, breadth  or depth. There are nondestructive methods that allow such  measurement of dimensions. Fig. 2 presents examples of these  modalities. These methods are able to measure with an accuracy  of 1 µm resolution in X, Y and Z axes. They are important for  reverse engineering but can also identify defects and other  properties such as flatness, angles, thickness, etc.


Patterned Light based measurement: This method is commonly  used to perform wide area 3D measurement. It uses patterned  light on the surface of PCBs to measure variations and  distortions present on the surface. Scanning is performed in  minutes and builds a 3D model; however, the main drawback is  that it does not give an optical image and cannot be used  independently to identify the components.


Terahertz


Minutes


2x-10x


3D


Identification, distinguish materials/


imaging


composition


Scanning acoustic


2x-250x


Identify integrity of materials, cracks check,


microscopy


delamination


Volumetric X-ray


Hours


Traces/Vias interconnection verification,


netlist authentication


Neutron imaging


Capacitors verification, identify materials


260


Similar to imaging modalities, the analysis methodology  depends on the modality of the image. Therefore, the algorithms  should be tailored towards the user requirements. However, irrespective of these requirements, the process of component  identification and vulnerability inspection follow a fundamental  framework, illustrated in Fig. 3. This is consolidated into the  steps below:


• Pre-Processing: Removal of noise, and unwanted data.


• Localization: Finding the location of every component.


• Feature Extraction: Identify essential features and extract  them from the image


• Classification: Classifying the board components into  traces, vias, resistors, capacitors, ICs, etc.


• Identification: Reading the markings on the board and  components (such as serial number, part number, etc.).


• Authentication: Storing the data as a BoM file and crossverifying with a golden sample.


There are numerous conventional algorithms in literature to  address each step of the framework. Various algorithms are  explained in detail in [16], however, they do not encompass  PCB verification in its entirety. The algorithms previously  published are approaches to individual problems and often  overlap in their functionality. There is no solution to address the  problem ‘as a whole’. Therefore, we present a variety of wellestablished algorithms that are complementary to each other and  we have modularized them to fit the steps of the framework


Any algorithm can be performed using traditional approaches  alone or be augmented using machine learning. With  advancement in machine learning it is now possible to have  algorithms almost entirely based on learning. For many years, machine learning was used to aid optimization in localization, feature extraction, classification and identification, however, there are now neural networks specifically for localization and  identification. To this end, we will discuss both traditional  methods and machine learning algorithms.


1) Preprocessing: Before identification and analysis, it is  important to clean up the acquired images. Noise could occur  due to a variety of reasons such as illumination, glare and fog. It can also occur due to non-planarity or manifest during the  image acquisition as sensor noise. To tackle different types of  noise, various techniques are available [16], [17]. We have  presented the most commonly available algorithms in preprocessing and their functionality.


Thresholding: Thresholding is a fundamental algorithm for preprocessing that is quick and efficient. Images, very commonly, have large components, and thresholding is the most effective  algorithm to remove a majority of noise. The main use of  thresholding is in isolating regions of interest in terms of  intensity values or in isolating connected components. However, thresholding cannot remove global noise such as  gaussian or salt and pepper noise nor local noise such as dead  pixel noise. Inability to perform region-based noise removal is


one of the main drawbacks of thresholding. Many variants of  thresholding are available from simple thresholding methods to  more complex methods like Hysteresis thresholding [18] and  Otsu’s Thresholding [19]. However, they are used for more  specific cases.


Filter-Based Approaches: Filters (or kernels) are highly  effective in capturing local neighborhood information. Filters  are pixel windows that perform various operations or  convolutions over a region that result in various  transformations. Gaussian filter [20] can perform gaussian  smoothing, Savitzky-Golay differentiation [21] filters can  identify and detect edges in an image. Median filtering and  mean filtering help remove various noise from the image such  as high frequency and low frequency information respectively


[22], [23]. Salt and pepper noise for instance can be removed  using a median filter. For optical PCB images noise, filter-based  approaches are one of the prime solutions [24]. However, the  main disadvantage of filter-based approaches is the filter size is  dependent on the PCB images and is usually selected  experimentally. This makes the inspection process difficult to  be fully automated.


Background Subtraction: Background subtraction is an  efficient pre-processing method for directly removing  unnecessary parts of the PCB image [25]. Existing background  subtraction methods used in hardware inspection include  frame/image averaging, frame/image differencing [26], [27], mean filtering [23], and eigen background subtraction [28], etc. The major drawback of background subtraction is that a  majority of techniques are sensitive to lighting and  environmental conditions. But background subtraction can  excel if the analysis can be guaranteed to run in controlled  conditions, such as in an assembly line with controlled lighting.


Morphological Operations: Morphological operations are a  collection of non-linear operations that operate on the shape of  the image. This allows region dilation, region erosion, skeletonization, etc. [7], [29]. It is used to refine the segmented  area, thus helps improve the performance later in the feature  extraction and localization step. Similar to filters, the size of  operators is experimentally chosen, and hence the drawback is  the difficulty to achieve a fully automated inspection system.


Height thresholding in a Depth Map: Using 3D depth  information, one can locate components by thresholding in Z  direction. A depth map makes localization and background  subtraction trivial, since slicing out the components that are not  at the same height with the board will be sufficient to isolate the  component and its boundary. The accuracy of this method  depends on the resolution of the measurement instrument. A  higher Z resolution results in better thresholding. However, after 3D thresholding, noise removal is needed to prepare the  image for next level of analysis.


2) Localization: Obtaining the components location  information on the PCB is as critical as measuring the


261


dimensions and the orientation of the components. Such  information is essential to verify the components on a PCB and  avoid counterfeits. There are various methods to perform  localization, but segmentation and active contouring are most  common.


Segmentation: This method is used to isolate objects in an  image and identify connected components. Once the objects are  isolated, their location can be obtained relative to the origin of  the image by calculating the distance from a reference point. The disadvantage of conventional segmentation techniques is  that, the user should define the functional parameters for  segmentation. Watershed [30], flood fill [7] are some of the  commonly used segmentation methods.


Figure 3: Image Analysis flow for automatic BoM extraction


Active contouring: Active contouring, also called snake  contouring is an approach to identify contours of objects in an  image. This allows the user to identify boundaries of an object  and record its location. Similar to segmentation, contouring is  independent of the global image characteristics and works over  a local region. The approach is adaptive and can be used in a  variety of scenarios. However, the image must be sharply  defined and of a sufficient size to be considered important to  identify contours for that object. Active contouring needs a cost  function for optimization and defining a proper cost function to  denote the contours is a challenging task.


3) Feature Extraction: In order to ensure accurate  classification and identification performance, the strong and  meaningful features of an image have to be defined and  selected. These features define an object or describe the texture  in an image ex. corners, gradients etc. Feature extraction is  traditionally performed by an engineer and is catered towards a  particular algorithm, however, recently, machine learning  approaches that can perform feature extraction (E.g., convolutional neural network) have become popular. The  commonly used feature extraction algorithms are scaleinvariant-feature transform (SIFT) [31], speed-up-robustfeatures (SURF) [32], corner detection [33], edge detection


[18], contour extraction, RGB/HSV-color-space information, etc. It should be noted that the selection of features is highly  dependent on the application, image modality and the target  object. But once the feature is sufficient to represent an object, it is mostly invariant to rotation, scale, lighting and translational  changes.


4) Classification: Classification is the process of categorizing  the components including resistors, capacitors, ports, LEDs, ICs, etc. into different classes. This will help identify  components of interest and isolate the search for markings or  vulnerabilities. There are different approaches for  classification, however, each have their own advantages and  disadvantages for PCB images.


Template Matching: It is a common approach used to classify  image patches with existing templates from a database. Templates can vary from simple to complex, for example, a  resistor can be encoded into individual components and a search  could be made in the image using an AND function. If each  template is identified in a location, then the resistor is  determined to exist at that location. Alternatively, in other  methods one instance of a resistor is used to search over the  entire image to find other similar instances. Correlation-based  algorithms such as Eigen templates [34], mean averaged  templates, or minimization algorithms [35] are examples for  this method. Since the template matching method uses the  whole image to perform correlation calculations, it is a very  time-consuming process and variant in rotation, scale, and  translation, which makes it difficult to use in an automated  fashion.


Optimization Algorithms: Identifying instances of components  by matching with an image from a database can be viewed as a  minimization problem. Many of the error minimization  algorithms are used as a tool to match images Genetic  algorithms [10], Particle Swarm Optimization Algorithms [35] and its variants [36] are examples of this method. In [10]a  genetic algorithm is used to perform template matching on PCB  components to identify the capacitors.


Optimization based algorithms provide a higher accuracy and  better match, however the major drawbacks include the multipass checks required by this method, as the algorithm usually  produces the best global match over the entire image. The  designer must remove the matched region and run more passes  to identify all instances of the component on the whole image. In addition, optimization is time-consuming, and there may be  cases where a non-optimal minimum occurs and will then  require the designer’s supervision for correction


Classifier-based learning: These approaches are usually  applied after feature extraction. The classifier analyzes and  evaluates the feature vector from the components dataset and  makes decision based on various dynamic rules. The most well262


known classifier is the support vector machine (SVM) [36]. Naive Bayes classifier [37], K-nearest-neighbor classifier, decision tree [39], etc., are also other available classifiers. Classifiers can learn the difference between the components if  trained with enough data points. A trained classifier can  instantly classify components, making it possible to do realtime analysis. However, classifiers are susceptible to outliers in  the data. Edge cases greatly deviate the classification accuracy.


Artificial Neural Networks: Neural networks are capable of  providing a high accuracy of detection. Large neural networks  are also called as Deep neural networks and learning performed  using them is popularly called ‘Deep Learning’. However, they  come with two major drawbacks; one is the need for a large  dataset for training and the other is a long training period. Depending on the hardware and the application, training the  network can take between hours to days, and the dataset  required for them should be in the range of thousands to  millions of samples and there are always uniquely shaped  components or edge cases that might not exist in the database  Recently, [40] has shown that approximately 500 images might  be enough to train an even large and deep network and classify  up to 20 different classes, which is very similar to the PCB  problem. Neural networks being semiparametric, are  autonomous by design, the network choose the best features to  classify the components negating the need for a dedicated  feature extraction step. However, the activation function has to  be decided manually when designing the network. Convolutional neural networks can provide filtering, scaling, and select texture-based features in addition to the capabilities  discussed above. With the advent of transfer learning [41], it is  becoming much easier to take pre-trained networks by giants  like Microsoft, Google and use them in scenarios like PCB  inspection. With a representative database and smart neural  network design, it might be possible to perform near 100% accuracy.


Figure 4: Dependence on data of machine learning vs deep  learning


The difference between neural networks and other machine  learning algorithms is its performance behavior with the  availability of data. Traditional machine learning performs  better than neural networks or deep learning when the available  data is limited. Once the amount of data crosses a specific  threshold, neural networks grow exponentially better. This is  illustrated in Fig.4. This threshold is usually about 5000 images  for each class of objects [49]. However, because of the


uniqueness of PCB images, it is necessary to conduct  comprehensive experiments to verify this solution.


Other Semi-supervising methods require only small number of  labeled image samples for training. Their performance in object  detection has improved recently [42]– [44], however, experiments should be conducted on PCB images for further  demonstration.


5) Identification: Classified components have to be identified  before authentication. This includes recognizing the logo, name, and ID on the components or on the board. For logo  identification image matching methods might seem appropriate  as the search area is limited after classification and number of  logos are limited in the market. Identifying the name and ID can  be performed using algorithms like optical character  recognition (OCR) [45]. Currently OCR is heavily used in US  Postal Service, car title recognition, etc. Tesseract developed by  HP is one of the mostly used OCR engines [46] however, there  are some limitations to use such engines in generating BoM on  PCBs. Font size on PCBs is usually small, text on ICs is blurry, and traces or vias on boards detected wrongfully as a character  are some of the many challenges in PCBs. Existing OCR  systems are mainly built to recognize characters from books, road sign, etc., where there is a solid background, therefore, they are not powerful enough to address the uniqueness of fonts  on PCBs and perform an accurate inspection. Hence, it is  necessary to build an OCR system that is robust to the  complexities of PCBs.


6) Authentication:


Consolidating the results from the first five steps of analysis, it  is now possible to have a detailed report of all the components, its locations, dimensions and their ID numbers. This data can  be recorded on a spreadsheet and published as a BoM. The BoM  from a device under test can be cross verified with the original  BoM, or a BoM extracted from a golden sample.


Numerous defects can potentially be detected using the  extracted BoM Such as; misaligned, misplaced, replaced and  removed components. The component images can also be  extracted from the localization step for further analysis, if  necessary. Authentication is open ended, and the authentication  procedure should be decided by the end-user depending on their  requirements.


Image Analysis is a challenging task. PCB assurance requires  inspection on various levels. Identifying a Trojan hidden in an  IC package is as important as identifying missing components. Using only an X-ray or Terahertz to identify a trojan will not  provide accurate information about the location for  authentication purposes. A complete authentication process  requires multimodal imaging across different spectrum; In  addition, a collection of algorithms is required to identify the  numerous defects. This process should optimize both time and  computational resources required, so real-time analysis can be


263


applied on assembly lines successfully replacing human  supervision. Innovations in imaging modality such as selective, intelligent microscopy and in image analysis in terms of  providing a fully adaptive system to select the right algorithm  can eventually be one of the possible solutions for PCB  Assurance.


The imaging modalities and image analysis techniques are  overviewed for PCB assurance. Our ultimate goal is to extract  the bill of material and perform visual inspection automatically  with no dependency to human supervision which can  significantly reduce the authentication process time.


Currently, there is little research in the community on the usage  of available modalities for hardware assurance. We believe to  build an ultimate PCB assurance tool, image fusion using  different modalities in an intelligent fashion is required. This  can prevent from collecting unnecessary data which increases  the complexity of the problem and computational time.


[1] “The big hack: How china used a tiny chip to infiltrate u.s. companies,” (Date last accessed 06-April-2019). [Online]. Available:


https://www.bloomberg.com/news/features/2018-10-


04/the-bighack-how-china-used-a-tiny-chip-to-infiltrateamerica-s-top-companies


[2] M. M. Tehranipoor, U. Guin, and D. Forte, “Counterfeit  integrated circuits,” in Counterfeit Integrated Circuits. Springer, 2015, pp. 15–36.


[3] S. Shahbazmohamadi, D. Forte, and M. Tehranipoor, “Advanced physical inspection methods for counterfeit ic  detection,” in40th International Symposium for Testing  and Failure Analysis, 2014, pp. 55–64.


[4] N. S. S. Mar, P. Yarlagadda, and C. Fookes, “Design and  development of automatic visual inspection system for pcb  manufacturing,”Robo


[5] K. Rebello, “Supply chain vulnerabilities.” FICS Research  Annual Conference on Cybersecurity, 2019. [Online]. Available:


https://fics.institute.ufl.edu/conference/


[6] C. Clark, “Anti-tamper jtag tap design enables drm to jtag  registers and p1687 on-chip instruments,” in 2010 IEEE  International Symposium on Hardware-Oriented Security  and Trust (HOST), June 2010, pp. 19–24.


[7] P. Malge and R. Nadaf, “Pcb defect detection, classification and localization using mathematical  morphology and image processing tools,” International  journal of computer applications, vol. 87, no. 9, 2014.


[8] S. Tang, F. He, X. Huang, and J. Yang, “Online pcb defect  detector on a new pcb defect dataset,” arXiv preprint  arXiv:1902.06197, 2019.


[9] C.-H. Wu, D.-Z. Wang, A. Ip, D.-W. Wang, C.-Y. Chan, and H.F. Wang, “A particle swarm optimization approach  for components placement inspection on printed circuit


boards,” Journal of Intelligent Manufacturing, vol. 20, no. 5, p. 535, 2009.


[10] A. Crispin and V. Rankov, “Automated inspection of pcb  components using a genetic algorithm template-matching  approach,” The International Journal of Advanced  Manufacturing Technology, vol. 35, no. 3-4, pp. 293–300,


[11] C. Szymanski and M. R. Stemmer, “Automated pcb  inspection in small series production based on sift  algorithm,” in 2015 IEEE 24th International Symposium  on Industrial Electronics (ISIE). IEEE, 2015, pp. 594–599.


[12] R. Chaganti, “Method and system for providing continuous  reference architecture and bill of material modeling,” Mar. 9, 2017, us Patent App. 14/846,375.


[13] M. Tiwari, S. Chakrabarti, D. S. Yadav, and S. Krishnamurthi, “Master bill of materials creation,” Jun. 27, 2017, us Patent 9,691,049.


[14] P. Gunther, U. C. Fischer, and K. Dransfeld, “Scanning  near-field¨ acoustic microscopy,” Applied Physics B, vol. 48, no. 1, pp. 89–92, 1989.


[15] Asadizanjani, N., Shahbazmohamadi, S., Tehranipoor, M., & Forte, D. (n.d.). Non-destructive PCB Reverse  Engineering Using X-ray Micro Computed Tomography.


[16] M. Moganti, F. Ercal, C. H. Dagli, and S. Tsunekawa, “Automatic pcb inspection algorithms: a survey,” Computer vision and image understanding, vol. 63, no. 2, pp. 287–313, 1996.


[17] Y. Zhang and H. Yu, “Convolutional neural network-based  metal artifact reduction in x-ray computed tomography,” IEEE transactions on medical imaging, vol. 37, no. 6, pp. 1370–1381, 2018.


[18] J. Canny, “A computational approach to edge detection,” in Readings in computer vision. Elsevier, 1987, pp. 184–


203.


[19] M. Sezgin and B. Sankur, “Survey over image thresholding  techniques and quantitative performance evaluation,” Journal of Electronic imaging, vol. 13, no. 1, pp. 146–166,


2004.


[20] K. Ito, “Gaussian filter for nonlinear filtering problems,” in  Proceedings of the 39th IEEE Conference on Decision and  Control (Cat. No. 00CH37187), vol. 2. IEEE, 2000, pp. 1218–1223.


[21] A. Savitzky and M. J. Golay, “Smoothing and  differentiation of data by simplified least squares  procedures.” Analytical chemistry, vol. 36, no. 8, pp. 1627–1639, 1964.


[22] H. Hwang and R. A. Haddad, “Adaptive median filters: new algorithms and results,” IEEE Transactions on image  processing, vol. 4, no. 4, pp. 499–502, 1995.


[23] A. K. Jain, Fundamentals of digital image processing. Englewood Cliffs, NJ: Prentice Hall, 1989.


[24] M. Piccardi, “Background subtraction techniques: a  review,” in 2004 IEEE International Conference on  Systems, Man and Cybernetics (IEEE Cat. No.04CH37583), vol. 4, Oct 2004, pp. 3099–3104 vol.4.


[25] M. Piccardi, “Background subtraction techniques: a  review,” in 2004 IEEE International Conference on  Systems, Man and Cybernetics (IEEE Cat. No.04CH37583), vol. 4, Oct 2004, pp. 3099–3104 vol.4.


264


[26] N. Friedman and S. Russell, “Image segmentation in video  sequences: A probabilistic approach,” in Proceedings of  the Thirteenth conference on Uncertainty in artificial  intelligence. Morgan Kaufmann Publishers Inc., 1997, pp. 175–181.


[27] W.-Y. Wu, M.-J. J. Wang, and C.-M. Liu, “Automated  inspection of printed circuit boards through machine  vision,” Computers in industry, vol. 28, no. 2, pp. 103–111,


1996.


[28] M. Piccardi, “Background subtraction techniques: a  review,” in 2004 IEEE International Conference on  Systems, Man and Cybernetics (IEEE Cat. No. 04CH37583), vol. 4. IEEE, 2004, pp. 3099–3104.


[29] E. Dougherty, An introduction to morphological image  processing, ser. Tutorial texts in optical engineering. SPIE  Optical Engineering Press, 1992.


[30] Wei Li, B. Esders, and M. Breier, “Smd segmentation for  automated pcb recycling,” in 2013 11th IEEE International  Conference on Industrial Informatics (INDIN), July 2013, pp. 65–70.


[31] P. C. Ng and S. Henikoff, “Sift: Predicting amino acid  changes that affect protein function,” Nucleic acids  research, vol. 31, no. 13, pp.


3812–3814, 2003.


[32] H. Bay, T. Tuytelaars, and L. Van Gool, “Surf: Speeded up  robust features,” in Computer Vision – ECCV 2006, A. Leonardis, H. Bischof, and A. Pinz, Eds. Berlin, Heidelberg: Springer Berlin Heidelberg, 2006, pp. 404–


417.


[33] C. G. Harris, M. Stephens et al., “A combined corner and  edge detector.” in Alvey vision conference, vol. 15, no. 50. Citeseer, 1988, pp. 10–5244.


[34] A. K. Shaw and V. Bhatnagar, “Automatic target  recognition using eigen templates,” in Algorithms for  Synthetic Aperture Radar Imagery V, vol. 3370. International Society for Optics and Photonics, 1998, pp. 448– 460.


[35] D.-Z. Wang, C.-H. Wu, A. Ip, C.-Y. Chan, and D.-W. Wang, “Fast multitemplate matching using a particle  swarm optimization algorithm for pcb inspection,” in  Applications of Evolutionary Computing, M. Giacobini, A. Brabazon, S. Cagnoni, G. A. Di Caro, R. Drechsler, A. Ekart, A. I.´ Esparcia-Alcazar, M. Farooq, A. Fink, J. McCormack, M. O’Neill,´ J. Romero, F. Rothlauf, G. Squillero, A. S .̧ Uyar, and S. Yang, Eds. Berlin, Heidelberg: Springer Berlin Heidelberg, 2008, pp. 365–


370.


Laser / White-Light Interferometry: Interferometry systems  work by using either a single beam of monochromatic light (Laser) or a spectrum of different colors (White Light, i.e., a  combination of Red, Green, Blue, etc.) to calculate the reflected  beam characteristics, and gaining insight about the reflected  surface. This modality focuses on a smaller region than  patterned light but provides slightly better accuracy.


Disadvantages of this method is the small field of view and the  need for multiple scans to cover the Full PCB. Laser  measurement systems are similar in price to patterned light  systems and cost about tens of thousands of dollars.


258


b) Penetrative Surface Imaging: This category of surface  imaging deals with imaging techniques that are able to image  below the surface. Some modalities such as thermal imaging,  otherwise called infrared imaging can image both surface level  as well as subsurface.


Thermal Imaging: This specialized method that can measure  run-time characteristics of PCBs. It uses an infrared sensor to  measure the irradiated heat from components in the infrared  spectrum. The sensors are able to sense infrared radiation from  within components packages or traces hidden behind  components. This provides information that is not usually  visible on a reflective imaging sensor. Although, Thermal  imaging cannot identify or localize components, it can measure  reliability defects such as power to-ground, low resistance, cable shorts, stressed components, faulty heat sink attachment, programming errors, defective BGAs, VCOs, decoupling  capacitors etc. Identification of hardware Trojans is also  possible by comparing the component’s heat signature with its  expected signature. Thermal imaging is usually instantaneous, similar to a camera. Depending on the resolution, the cost for  such a system can be a few hundred to tens of thousands of  dollars. But the disadvantage is the board needs to be active to  obtain data. And this can be very time consuming to  authenticate boards for a large vendor.


Terahertz Imaging: This modality utilizes the terahertz range of  the EM Spectrum to perform subsurface penetration imaging, as shown in Fig. 2. This method produces 3D models of surface  level and regions near the surface, and its main use is in  analyzing the material and its properties such as the dielectric


characteristics of components. Terahertz is a non-destructive  imaging technique and is a good supplement to be used with  optical microscopes, as microscopes offer quick surface level  imaging, while terahertz could provide simple subsurface level  imaging. Terahertz can penetrate plastics and similar  substances, but cannot penetrate metal, thus imaging the entire  PCB such as in X-ray is not possible with Terahertz. It can  identify components within packages, and possibly identify  hardware Trojans by analyzing the component signature and  comparing it with its expected signature [48].


Scanning Acoustic Microscopy: Scanning acoustic microscopy  uses sound waves to detect and identify voids, cracks, and  density changes such as delamination. This method is  nondestructive as well but has a transducer probe that can either  scan at a point or over a surface. This method is able to obtain  a resolution of about 50 microns. Since this approach requires  contact with the PCB, its path has to be designed specifically  for every PCB and is quite time consuming, both for design as  well as for probe travel [14].


2) Volumetric Penetrative Imaging: Volumetric imaging  modalities are able to view through the PCB and get information  about the inner layers of the PCB, as illustrated in Fig.2. X-ray  and certain other modalities have sufficient penetrative ability  to be able to traverse through various components and be  captured by a detector at the other side of the source.


X-Ray Imaging: X-Rays have the ability to transmit through  circuit elements due to their penetrating properties. There are  two types of imaging using X-Rays: 2D, and 3D computed  tomography (CT). 2D X-Ray is a quick approach to capture


Figure 2: Imaging Modalities and examples


259


projections of a PCB as a photographic film or a digital image. X-Ray specifications vary with the X-ray source material, filter  material and the emission voltage used. These determine what  materials the X-Rays will pass through which directly affects  the visibility of certain parts of the PCB. X-Ray CT can build  3D volumetric images from which CAD files can be extracted


[15]. X-Ray Laminography, a special case of X-Ray CT, is also  used for flat samples like PCBs.


X-Ray cannot of be directly used to identify the circuit  components, however, it can be used to detect problems with  bond wires, traces and vias in hidden layers. Counterfeit  components where their surface is deceiving can be examined  using X-ray. High Z (atomic number) materials like metals  attenuate the X-ray and can cause artifacts in the reconstructed  image that makes data extraction difficult. X-Ray imaging takes  hours to map an entire PCB, and a few more hours to reconstruct  the 3D model from the raw images. The cost for such systems  is comparably higher and is in the range of a million dollars.


Neutron Imaging: Neutron imaging is a relatively new  technology in the volumetric imaging sphere. Similar to X-Ray, neutron images can also provide 2D projections or 3D  volumetric images using computed tomography. Neutrons can  penetrate into dense materials such as metals and overcome the  main disadvantage of X-Rays, however they cannot pass  through plastic material with low conductivity. Neutron  imaging, similar to X rays, takes hours to map the entire PCB, and reconstruct a model. A neutron imaging system while not  commercially available yet, can cost upwards of a million  dollars.


While these are the commonly used techniques, it should be  noted that any imaging modality or technique can be used and  might be useful for some special cases.


Therefore, to provide maximum assurance a combination of the  modalities might be a better option. However, collecting a lot of  data has its own challenges in terms of both the acquisition time  and analyzing the large datasets. An intelligent platform which  can perform online image analysis using one modality and make  a decision accordingly for the next pass of imaging can save  time both on acquisition and computation. However, to have  such a system for analysis, the acquired images need to be  analyzed based on a set of standards or metrics that needs to be  developed in the first place.


II. Image Analysis


Researchers in the community have proposed different  approaches for automatic visual inspection, however there is no  framework proposed for such an effort. Malge et al., adopted  canonical image processing methods to detect trace level and  via level defects [7] while Tang et al., employed Convolutional  Neural Network (CNN) to detect similar defects [8]; other  researchers like Wu et al., and Crispin et al., achieved  automated detection for component placement by directly  comparing golden PCB and test PCB [9], [10]. Szymanski has  also worked on text detection for verification purposes [11]. While these are significant approaches for automated PCB  inspection, most rely on the availability of an existing golden  PCB board for direct comparison, which is not always the case  in practice.


TABLE I: Summary of Different Imaging


Modalities.


Imaging modality


Acquisition


speed


Magnification


Model  dimension


Application on components


Reflective  surface


Cameras


Seconds


2D


Localization, identification


Digital optical  microscope


12x-2500x


Localization, identification, defects analysis


White light


1x-200x


Localization, placement validation,


interferometry


dimension measurement


Laser


Localization, placement validation, dimension  measurement


Penetrative Thermal


2x-20x


Realtime performance evaluation,


surface  imaging


short/open circuits detection


[36] Mouna H., Mukhil Azhagan M.S., Radhika M.N., Mekaladevi V., Nirmala Devi M. (2018) Velocity  Restriction-Based Improvised Particle Swarm  Optimization Algorithm. In: Saeed K., Chaki N., Pati B., Bakshi S., Mohapatra D. (eds) Progress in Advanced  Computing and Intelligent Engineering. Advances in  Intelligent Systems and Computing, vol 564. Springer, Singapore


[37] J. A. Suykens and J. Vandewalle, “Least squares support  vector machine classifiers,” Neural processing letters, vol. 9, no. 3, pp. 293–300, 1999.


[38] I. Rish et al., “An empirical study of the naive bayes  classifier,” in IJCAI 2001 workshop on empirical methods  in artificial intelligence, vol. 3, no. 22, 2001, pp. 41–46.


[39] S. R. Safavian and D. Landgrebe, “A survey of decision  tree classifier methodology,” IEEE Transactions on  Systems, Man, and Cybernetics, vol. 21, no. 3, pp. 660–674, May 1991.


[40] W. Zhao, “Research on the deep learning of the small  sample data based on transfer learning,” in AIP Conference  Proceedings, vol. 1864, no. 1. AIP Publishing, 2017, p.


020018.


[41] S. J. Pan and Q. Yang, “A survey on transfer learning,” IEEE Transactions on knowledge and data engineering, vol. 22, no. 10, pp. 1345– 1359, 2010.


[42] M. Guillaumin, J. Verbeek, and C. Schmid, “Multimodal  semisupervised learning for image classification,” in 2010  IEEE Computer society conference on computer vision and  pattern recognition. IEEE, 2010, pp. 902–909.


[43] G. Camps-Valls, T. V. B. Marsheva, and D. Zhou, “Semisupervised graph-based hyperspectral image  classification,” IEEE Transactions on Geoscience and  Remote Sensing, vol. 45, no. 10, pp. 3044–3054, 2007.


[44] D. P. Kingma, S. Mohamed, D. J. Rezende, and M. Welling, “Semisupervised learning with deep generative  models,” in Advances in neural information processing  systems, 2014, pp. 3581–3589.


[45] S. Mori, H. Nishida, and H. Yamada, Optical character  recognition. John Wiley & Sons, Inc., 1999.


[46] R. Smith, “An overview of the tesseract ocr engine,” in  Ninth International Conference on Document Analysis and  Recognition (ICDAR 2007), vol. 2. IEEE, 2007, pp. 629–


633.


[47] “The fics research security and assurance (scan),” (Date  last accessed 05August-2019). [Online]. Available: https://fics.institute.ufl.edu/facilities/


[48] K. Ahi, S. Shahbazmohamadi, N. Asadizanjani, “Quality  control and authentication of packaged integrated circuits  using enhanced-spatial-resolution terahertz time-domain  spectroscopy and imaging”, optics and Lasers in  Engineering, volume 104, 2018, pages 274-284


[49] I. Goodfellow, Y. Bengio, and A. Courville,Deep learning.   MIT press,2016.


265


Redistribution layer (RDL) bonding pad over active  circuitry is utilized to re-route the original bond pad to  other location for wire bonding using RDL. The  damages in the active circuitry beneath the RDL bond  pad induced by stress from wire bonding and package  must be evaluated for reliability in the product  development. The experimental approach and test  structures are proposed in this paper. Functional fail was  detected in electrical test after reliability tests on  packaged IC. The dielectric cracking initiated by wire  bonding that corresponds to the functional fail is  identified by physical failure analysis and  Transmission-Electron-Microscopy (TEM) at a specific  location beneath the RDL bond pad. Finite element  simulations are used to analyze the wire bonding stress  distribution and circuit-under-pad design effect. The  predicted maximum stress for the dielectric cracking  matches to the location observed in the physical failure  analysis. Based on the experiment and the simulation  data, design rules for the circuit routing beneath the RDL  bond pad have been successfully developed that all  product reliability tests pass later with extend bonding  power. The results lead to significant improvements in  the robustness of circuit routing structure beneath the  RDL bond pad for dielectric cracking without  modifications of the existing processes for the product. I. INTRODUCTION


Redistribution layer (RDL) uses an extra layer of  metallization for integrated circuit to route the IO, power  or ground pads to other locations that are available for  wire bonding or bumping to the corresponding pins of  the package. In the recent development of 3D diestacking for Dynamic-Random-Access-Memory (DRAM) package, the RDL bonding pad is used to reroute the DRAM centered bond pad originally for ThinSmall-Outline-Package (TSOP) to die edge for BallGrid-Array (BGA) package and reduce the gold bond  wire cost [1]. In flip-chip package for high performance  and high density I/O, bumping pads are


normally placed in area array type. The RDL is used to  re-route the peripheral wire bonding pads to the bumping  pads without changing the placement of existing wire  bonding pads [2]. Wafer-Level-Chip-Scale-Package (WLCSP) has experienced significant growth in mobile  consumer product for small form factor and performance. Now it is also attractive to wearable and Internet-ofThings (IoT) product. The WLCSP uses an RDL process  similar to the flip-chip to re-route the original bond pad  and makes bigger pads for solder bumps [3].


In the case of wire bonding for integrated circuit (IC), the  mechanical integrity of the IC bond pad structure must  be evaluated. The risk of pad damage during bonding  and reliability degradation is high when the mechanical  strength of the pad structure is weak. Finite-elementmodel (FEM) simulation results correlate well between  the stress point and location for various dielectric  stacks, bond pad thicknesses, wire bonding parameters  and materials, and circuit-under-pad designs [4]–[7].


Typical wire bond pad that consists of a top-level metal  does not allow circuit routing beneath the bonding  region such as (Top metal -1) beneath the original bond  pad shown in Fig. 1. High density via array beneath the  Top metal within the original bond pad window may be  used to reinforce the structure and avoid possible  damage during wire bonding to the circuit routing and  active device such as IO buffer and Electrostatic  Discharge (ESD) protection [8, 9]. However, the RDL  bond pad for re-routing the original bond pad to other  location is sensitive to dielectric cracks in the circuity  beneath the RDL bond pad window. The integrity of the  metal pattern under the RDL bond pad is critical for  determining the cracking resistance for a given IC  fabrication technology and the assembly/packaging  process. Electrical short/open and leakage tests post  harsh wire bonding experiment and reliability tests were  performed on various bond pad test structures to develop  metal pattern density rules beneath the pad window for  improving the robustness to cracking [10].


266


Stress Analysis of Damage in Active Circuitry  beneath Redistribution Layer (RDL) Bonding  Pad and Improvements for Reliability


Chih-Ching Shih, Wei-Hao Hsiao, Leo Chan, Hsiao-Tien Chang, Li-Kuang Kuo, DingJhang Lin, Yen-Hai Chao, Chih-Yuan Lu


Macronix International Co. Ltd.


No.16, Li-Hsin Road, Hsinchu, Taiwan


*Corresponding Author’s Phone and Email: +886-3-5786688 cshih@mxic.com.tw


( e) Type-E: Low metal density for narrow line width with wide


space.


(f) Type-F: Low metal density for wide metal line width and various spaces.


Fig. 2. Various types ofRDL bond pad test structure.


III. ASSEMBLY WIRE BONDING TEST RESULTS


To assess the assembly wire bonding window of the  RDL bond pad structures, a bond parameter matrix with  bonding force, bond time, and ultrasonic power for a  commercial wire bonder with 0.7 mil Au wire was  proposed to optimize the wire bonding process. The  design-of-experiment (DOE) plan for the Au wire  bonding is shown in Table I.


Table I. Wire bond DOE for optimizing the bonding  process


Wire bond


DOE split Time


Force


I


Norm-50% Norm-IO% Norm-IO%


Norm-50%


Norm


Norm-50% Norm+10% Norm+IO%


Norm Norm-IO%


Norm Norm+IO%


Norm Norm+10% Norm-IO%


Norm+50% Norm-IO% Norm+IO%


Norm+50% Norm Norm-IO%


Norm+50% Norm+10% Norm


Evaluation test items after the assembly wire bonding  are wire pull, ball shear, Optical Microscopy (OM) (visual under 40X optical microscope) inspection of 1st  bond and ball shear, ball size, cratering (OM & SEM), and SEM of cross-section for remaining Al pad metal  thickness. The cratering test was used to investigate  cracking for all the pads on the test chip. The chemical  and dipping time for bond pad metal etch were optimized


268


for the IC technology to prevent creating etch artifacts  for pad cracking [ 11, 12].


The assembly tests were executed according to the  parameter matrix presented in the Table I for all types of  metal density, width and space beneath RDL bond pad  on 10 samples. We observed a pad cracking in one  specific type-C RDL bond pad assembled with high  power. The Norm+50% power is the maximum setting  of the wire bonding machine. As shown in Fig. 3, the  fail percentage of the weakest pad increased with  increasing power. Our trend of metal pattern density for  pad cracking was consistent with the harsh wire bonding  test results [10]; however, the interaction of metal  pattern density with the metal width and space for the  same metal pattern density was not discussed in this  paper. For example, our cratering test results showed  that the Type-A RDL pad in Fig 3(b) with narrow metal  line and space was significantly better than the Type-C  RDL pad in Fig. 3(a) with wide metal line and narrow  space including slots or/and holes. Both RDL pads are  with high metal pattern density for total metal area > 50% of the pad opening.


Norm+l0%


Norm+50%


The weakest pad (high


(a) metal pattern denstiy with wide metal width)


*Fail%


High metal pattern


(b) density but with narrow metal width and space


0%


I * Sfill\lle size is I Oea for each case


Fig. 3. Optical micrograph of cratering test results of RDL bond  pads after assembly wire bonding with extend power: (a) a specific  type-C pad failed the cratering test and the fail percentage increased  with increasing power. On the other hand, a type-A RDL pad in (b) with high metal pattern density but narrow metal width and space  showed no pad cracking.


For mass production, we need a better control and  tighten the wire bonding recipe. A statistical tool is used  to analyze wire pull, bond shear, and ball size/thickness  data and optimize the time, power, and force settings.


Fresh samples were used for the 2nd run of evaluation to  tighten the recipe and pass all the assembly test criteria


In fact, the dielectric cracking in the IC can lead to not  only short/open and leakage failures but also functional  failures. In contrast to the conventional bond pad test  structure with dummy metal patterning beneath the pad  metal [10], our product test vehicle with active circuitry  beneath the top metal and full functional test approach  imposed a rigorous validation for the metal patterning  rules beneath the RDL bond pad.


Known good dies were used for post assembly full  functional tests using the 1) optimized and 2) extend  power wire bond conditions. From the above assembly  test results, we observed that the dielectric cracking  initiated by the mechanical stress especially for the


extend power wire bond condition. However, the  dielectric cracking may not cause an immediate failure  in the post assembly electrical test. The packaged RDL  bond pad structures that passed the post assembly  functional tests were subjected to product reliability  stress tests evaluation.


IV. PRODUCT RELIABILITY STRESS TEST


The RDL bond pad structures are assembled in a  qualified ball-grid-array package. The product  reliability tests are device qualification tests including  additional tests for non-volatile memory device, and  package qualification tests. The package stress test  conditions are moisture sensitivity level 3 (MSL3), temperature cycling of -65 °C to + 150 °C, highly  accelerated temperature and humidity stress (HAST), and high temperature storage (HTSL) at 150 °C.


Table II. High temperature storage reliability test


results of RDL bond pads.


HTSL


Wire bond conditions


500hrs


l 000hrs


Extended Power Lot#l


1/81


3/80


Extended Power Lot#2 1/40


N.A.


Optimized, Lot # 1


0/77


Optimized, Lot #2


Optimized, Lot #3


The packaged RDL bond pad structures using the  optimized wire bond conditions passed all the product  qualification tests including the HBM/CDM ESD and  latch-up without degradation in performance. However, we observed significant differences in the HTSL test  between the optimized and the extended power wire  bond conditions. Read fails for functional failures were  observed solely in the extended power bonding  condition, as shown in Table II. The read fail is due to  OBTRIBENF signal line for controlling the output  driver at CLK falling edge stuck at low as shown in Fig.


4. The driver output at the CLK rising edge is normal.


OBTRIBENTRIBENF


Read output :OBTRIBENF= 1


"'•1--1.,.,...-, .. 1


OBTRIBENFB


Fig. 4. Electrical failure analysis indicates that the read fail is due to  stuck at low fault at OBTRIBENF signal line for CLK falling edge.


Physical failure analysis results in Fig. 5 suggest that  excessive tensile stress from wire bonding initiates the  dielectric crack in wire bond with extend power.


269


Because the dielectric material is brittle, it cracks at the  location where the maximum principle stress exceeds the  tensile strength of the dielectric material. Later in the  High Temperature Storage Life (HTSL) test, compressive stress from the Coefficient of Thermal  Expansion (CTE) mismatch between the dielectric and  metal layers caused lateral aluminum extrusion along the  cracks for the stuck at low fault.


We traced back the layout of OBTRIBENF signal line  for dielectric cracking as shown in Fig. 6. The fail site is  located beneath the edge of the bond ball in the cratering  test of the weakest RDL bond pad as shown in Fig. 3 (a). According to the harsh wire bond studies of bond pad  structures in [10], the parenthesis-shaped cracks near the  bond ball edge are typical. FEM simulation results of  wire bond process on bond pad structure in Liu et al [ 4] suggest that the mechanical stress on the bond pad  structures during the bonding process is very nonuniform in the radius direction and the maximum stress  normally appears at the bond ball edge region. Why the  specific type-C bond pad in our evaluation is more  susceptible to dielectric cracking during wire bond than  other designs of the same type? Further stress analysis  was performed to improve the robustness of RDL bond  pad to dielectric cracking for circuit-under-pad design. The results are presented in the next section.


Dielectric cracks & lateral Al


Fig. 5. Physical failure analysis results: (a) failing circuitry metal  line layout; (b), (c) SEM micrographs of the failure; (d) elemental  mapping of cross-section at the failure location showing Al lateral  extrusion.


Fig. 6. Optical micrograph (a) of cratering test for the bond ball of  the weakest RDL bond pad with extend power (Norm+50%) as shown  in Fig. 3 (a) and the corresponding metal layer layout (b). The  OBTRIBENF signal line enclosed in the circled-area is near the  parenthesis-shaped cracks that are typical in harsh wire bond studies of  bond pad structures [ I OJ.


V. STRESS ANALYSIS OF WIRE BONDING


PROCESS AND CIRCUITRY LAYOUTBENEATH


RDL BONDING PAD


The assembly and reliability test results consistently  indicate that the weakest RDL bond pad in for the  specific type-C metal patterning (high metal density with  wide metal line and various spaces including slots or/and  holes) is susceptible to dielectric crack resulting in  functional failure. FEM simulations for various RDL  bond pad structures are useful to effectively analyze the  stress in the dielectric layer beneath the bond pad. This  allows considerable reduction of the long cycle time  from designing, fabricating, assembling to testing pad  structures for verifications.


To perform an effective FEM simulation of stress  distribution in the dielectric layer of circuit-under-pad  design, the following assumptions were made for our fail  case as shown in Fig. 5:


1) The contact intermetallic effect and the bond formation due to ultrasonic energy and friction between the F AB and the bond pad are not included in this study.


2) The inertia force from the capillary transferred to the Free Air Ball (F AB) is not considered


3) The force applied to the top of the bond pad structure is static if the direct bonding force transferred to the dielectric layer is close to or exceed the breaking point for the specific type-C RDL bond pad. (In reality, the ultrasonic energy of the bonder is dynamic. The ultrasonic energy addes stress beyond that resulting from the static wire bond loading applied to the bond pad structure. )


4) The effects of the ultrasonic energy transferred to the bond pad through the capillary and the thermal effect on substrate temperature from the wire bonding stage are not included.


The above limitations in the modeling work allow  performing a relative comparison of wire bonding pad  stress effects on circuit-under-pad design for a given  wire bond condition. Optimizing the wire bond process  parameters for controlling the stress in the dielectric  layer under the bond pad below the breaking point is not  the in the scope of this modeling framework.


Both the principle and compressive stress distributions  in the circuit-under-pad structure can be predicted by the  simulation for assessing the risk to damage for wire  bonding. For dielectric cracking failure mode, we can  compare the maximum principle stress at the actual  cracking site for different circuit-under-pad designs. For  other failure mode such as silicon-to-contact interface  damage, the compressive stress must be evaluated by  simulation. Because the silicon-to-contact interface  damage is irrelevant to the failure mode of our device, we will not evaluate the compressive stress here. After  the maximum stress in the dielectric layer enclosing the  OBTRIBENF signal trace is consistent with the actual  cracking site in the specific type-C RDL bond pad, we  will continue to analyze the improvement in circuitunder-pad design by increasing the space for the


270


wide metal lines enclosing the OBTRIBENF signal line  for reducing the stress in the dielectric layer.


Bonding


tool


Sidie .._


Bond wire


Pad structure


-- --- - -·


r.


Fig. 7. (a) FEM for the bonding tool, free-air-ball and bond pad  structure; (b) The actual FEM simulation is 3D for a bond pad structure  with F AB and tool structure.


Figure 7 (a) shows the 3D FEM for the bonding tool, F AB and bond pad structure. The actual FEM  simulation in this work is 3D as shown in Fig. 7 (b). The  material characteristics used for FEM simulation ofRDL  bond pad are listed in the Table III. Figure 8 shows that  the stress predictions for the stress distribution on the  bond pad structure are non-uniform. The maximum  stress is at the edge region of the bond ball. The  maximum stress may increase as the F AB ball location  on the bond pad is shifted as listed in the Table IV. The  maximum stress changes with the F AB location because  the circuit-under-pad metal pattern beneath the RDL  bond pad is non-uniform as shown in Fig. 6 for the  specific type-C RDL bond pad.


Table III. Material characteristics used for RDL bond  pad structures analysis


Material CTE(ppm/C)


FAB


Au


RDLpad


Al


21.6


Dielectric SiO2


Metal


Via


w


4.5


Wafer


Silicon


3.2


top side view


Modulus (Gpa)


60  70


71.4  70  411


169.5


Yield stress (Gpa) Poisson ratio


0.33 (200C)


0.035


-mu•


.. ,,..


bottom side view


0.44


0.34


0.16


0.28


0.23


Fig. 8. Predicted 1 st principle stress on the specific type-C RDL bond  pad structure for (a) center bond & high power (b) shift bond & high  power, calculated using FEM simulations.


Fig. 9. Predicted 1 st principle stress distribution on the dielectric  layer enclosing the OBTRIBENF signal metal layout for the functional  fail in HTSL test, calculated using FEM simulations.


Fig. 9 shows that the maximum stress in the dielectric  layer enclosing the OBTRIBENF signal metal line of the  specific type-C RDL bond pad with F AB location  shifted is 57.4 MPa that exceeds the minimum tensile  strength of 45 MPa for SiO2 [13].


Because the strength of dielectric layer increases with  the thickness, we propose to increase the space between  the OBTRIBENF metal and the wide metal adjacent to it, as shown in Fig. 10. The predicted maximum stress at  the failing location appears to be reduced from the  original 57.4 MPa to 32 MPa, which is lower than the  tensile strength for high purity SiO2. An improved  circuit-under-pad structure can increase the margin for  wire bonding and reliability. The proposed design  improvement allows withstanding the harsh bonding  experiment and reliability tests.


signal line


Fig. 10. (a) Proposed design improvement by increasing the space  for the wide metal lines enclosing the OBTRIBENF signal line for  reducing stress in the dielectric layer; (b) current design with narrow  space that failed in cratering (Fig. 3) and HTSL stress tests (Table II) with extended power.


Fig. 11. Predicted 1 st principle stress on the dielectric layer  enclosing the OBTRIBENF signal metal layout for functional fail, calculated using FEM simulations. The predicted maximum stress at  the failing location appears to be reduced from the original 57.4 MPa to  32 MPa, which is lower than the tensile strength for high purity Si02


[13].


271


VI. CONCLUSIONS


Proper design for the circuit-under-pad layout beneath  the RDL bond pad can increase the robustness to  dielectric cracking. Not only the metal density but also  the design principles for the space of wide metal must be  developed for increasing the dielectric cracking  resistance to wire bonding stress. The finite-element  modeling work is simplified and effectively used for a  relative comparison and analyzing the wire bond stress  effects on circuit-under-pad design. Further FEM  analysis of bond over active circuitry for Cu wire  bonding and low-k dielectric that are also susceptible to  pad cracking can be studied usmg the same  methodology.


ACKNOWLEDGEMENTS


The authors would like to thanks ChipMOS for sharing  the assembly, harsh bonding test, and FEM simulation  results; Martin Lee in Macronix Package Development  for discussions of the FEM simulation; Hung-Chi Chen  in Macronix Technology Development for discussions  of the metal pattern design rule beneath the RDL bond  pad; Patrick Chen and T.Y. Chang in Macronix  Reliability Engineering for failure analysis and  reliability tests.


[I] W. Zohni, "Near term solutions for 3D memory stacking (DRAM)", Invensas Corporation, 2014.


[2] J. Fang, et al, "A routing algorithm for flip-chip design", IEEE ICCAD, 2005.


[3] J. Lau, "Recent advances and new trends in flipchip technology", Journal of Electronic Packaging, 2016.


[ 4] Y. Liu, et al, "Thermosonic wire bonding process simulation and bond pad over active stress analysis", IEEE Transactions on Electronics Packaging Manufacturing, 2008


[5] T. Hisada, et al, "Fine pitch wirebonds on ultra low-k device", Transactions of the Japanese Institute of Electronics Packaging", 2011.


[6] A. Viswanath, et al, "Numerical study of gold wire bonding process on Cu/low-k structures", IEEE Transactions on Advanced Packaging, 2007


[7] H. Tseng, et al, "Dynamic simulation for  microelectronic packaging of Al pad/underlying pad structure during copper wire bonding",


International Microsystems, Packaging, Assembly and Circuit Technology Conference, 2014


[8] M. Ker, et al, "Active device under bond pad to save I/O layout for high-pin-count SOC", IEEE


International Symposium on Quality Electronic Design, 2003


[9] W. Anderson, et al, "ESD protection under wire bonding pads", EOS/ESD symposium, 1999


[IO] S. Hunter, et al, "Use of harsh wire bonding to  evaluate various bond pad structures", European  Microelectronic & Packaging Conference, 2011


[11] V. Korchnoy, "Investigation of bond-pad etching chemistries for determination of probe/bonding related sub-pad cracks", ISTFA, 2007


[12] Y. Ruan, et al, "Sample preparation technique  for bond pad IMD (Inter-metal dielectric)


damage observation", ISTFA, 2008


[13] https://www .azom.com/properties.aspx? Article  ID =1114


272


Nanoprobe characterization of soft SRAM bit fails in advanced technologies


Satish Kodali, Chen Zhe, Chong Khiam Oh


GLOBALFOUNDRIES Inc, Malta, NY, US -12020


Phone: 518-491-1533, satish.kodali@globalfoundries.com


Nanoprobing is one of the key characterization techniques for  soft defect localization in SRAM [1-6]. DC transistor  performance metrics could be used to identify the root cause of  the fail mode. One such interesting case report is presented.


A wafer is uniquely impacted by significant SRAM yield loss.  The defects happened to be a combination of hard and soft  fails. Standard FIB cross-section on the hard fail sites and top  down delayered inspection did not reveal any obvious defects. Nanoprobing method to understand the root cause was  implemented. The sample is delayered to contact level for  probing.


Transistor IdVg Characterization


Transistor IdVg measurements did not find any abnormal  defects on the pull up (PU) and pull down (PD). Pass gate (PG) showed abnormal behavior. Figure 1 and 2 show linear  mode IdVg measurements of the pass gate in linear and log  scale, respectively. Figure 3 and 4 show saturation mode IdVg  measurements in linear and log scale, respectively. It is evident  from the data that a resistive bitline contact is showing  asymmetric IdVg characteristics in the saturation mode.


Diode Characterization


Diode measurements were performed to the bulk.  It is  identified that diode characteristics to the bulk are similar for  the fail and the reference contacts as shown in Figure 5.


Capacitance measurement between the PG and bit line contact  was performed to further understand the fail mode.


Figure 3: IdVg of the fail device compared to the reference in  Saturation mode.


Figure 4: Semi-Log scale IdVg of the fail device compared to  the reference in Linear mode


Figure 1: IdVg of the fail device compared to the  reference in Linear mode.


Figure 2: Semi-Log scale IdVg of the fail device  compared to the reference in Linear mode


273


Capacitance Measurements


Capacitance is the ratio of the change in an electric charge in a  system to the corresponding change in its electric potential. It  is referred by the formula below.


C = ΔQ/ΔV


Capacitance of a classic parallel plate capacitor with area of  the plate A, distance between plates d, dielectric constant of  the material between plates k and permittivity of free space ε0  is defined by the formula below


C = k ε0 A/d


Substrate dopant concentration NSUB with MOSCAP  Capacitance C, electron charge q (1.60219 × 10–19 C), gate  area A, permittivity of the substrate material εS, Gate Voltage  VG is given by


NSUB = 2/{q εs A2 [(Δ1/C2) / ΔVG]} [7]


CV characterization plots provide valuable information  regarding the failure mechanism. Characterizing the LDD for  implant profile would be very useful information for the  process community to understand the fail mode. Due to very  low capacitance values being measured, a parallel model CpRp is used as shown in Figure 6. Dissipation (D), defined as  the ratio of current through the resistor Rp to the current  passing through the capacitor Cp, is used to monitor the  accuracy of the data. The lower the D value, the better the  accuracy of the measured capacitance. Open Correction is  used to minimize the noise floor. High frequency in MHz  range is used to improve the accuracy of data collection [8, 9].


Experimental setup


Figure 7 shows the schematic connection of the two probes to  the DUT [7]. The cable lengths are matched for all connectors. Hp and Hc connectors are connected with T connector and are  physically routed to a nanoprobe. Lp and Lc are also  connected in a similar fashion.


Due to the complex nature of advanced devices, it is very  challenging to achieve accurate gate capacitance. Often source, drain and gate connections are shared with multiple devices. It  becomes very challenging to accurately decouple individual  capacitance. In the current work gate (Pass Gate) and drain (bit  line) of the MOSFET of interest is chosen for CV  characterization. Source and bulk were left floating. Data from  a reference site is compared to that of the fail to qualitatively  interpret capacitance variations. The capacitance measured  will provide characteristics of Gate to LDD(Lightly Doped  Drain) overlap region.


Figure 6: Model used for Capacitance measurements


Figure 7: Schematic of the connections to the DUT.


CV characterization of LDD


Characterizing the LDD for implant profile would be a very


useful information for the process community to understand  the fail mode when resistive LDD is a potential suspect.  The  two probe Capacitance – Voltage (CV) measurement is  performed between the gate (Pass gate) and drain (bit line) of  the device with source and bulk floating. Figure 8 shows the  CV data and Figure 9 shows the dC/dV data extracted from the  original CV data. dC/dV curve shows the depletion region  slope as a hump. Higher depletion region slope corresponds to  lower N type dopant concentration.  It is clear from the data  that a lower N-type dopant concentration is seen at the failing  BL contact LDD to gate overlap compared to the reference.


Figure 5: Fail and reference bitline to substrate diode  measurement


274


Physical Characterization


The TEM analysis on the failing sample did not identify any  anomalies at bit line contact. Since a dopant profile issue is  expected, an inline wafer processed at resist before implant  was cross-sectioned for SEM analysis. It is identified that the  BL/PG contacts have a high residue at the contact to fin  interface. This could potentially block the subsequent LDD  implant. Figure 10 shows the image of resist residue over fins  as potential source of implant blockage.


Upon characterizing several samples, it has been identified that  even the neighboring good devices are exhibiting similar  failing electrical behavior but to a lesser extent. Understanding  the layout of the devices can give a better understanding of the  fail mode. Figure 11 shows the SRAM topdown layout. The  bitline contacts are identified by the red arrows. The N active  area covered by the resist is shown by the red box for the PG  and dark blue for the PD and Source contacts. During the  implantation step the contacts are not built yet. Figure 12  shows the actual environment during implantation step. It is  clearly seen that the BL contacts have minimal clearance for  cleans post resist removal. Hence the chances of the resist not  to be removed completely are much higher for the BL contacts  compared to any other sites. Adding more enhanced cleaning  methodologies to remove the resist completely provides the  solution to the fail mode identified.


Figure 8: CV measurements of the reference and the fail  Pass Gate to BL contacts


Figure 9: dC/dV measurements of the reference and the  fail Pass Gate to BL contacts showing lower dopant  concentration in the LDD of the fail compared to  reference


Figure 10:  PG/BL Contacts have residue on the top right


before the implantation step causing subsequent LDD


implant blockage.


Figure 11: SRAM layout showing the BL contacts


indicated by the red arrows. The Orange boxes indicate


the BL contact regions between Pass Gates. The dark


blue boxes correspond to other contacts to N active.


275


In the current work, soft SRAM fail yield degradation issue  was presented. Nanoprobing DC characterization  measurements followed by CV measurements were done. Two  probe CV measurement between the gate and drain was  performed. Very valuable process marginality at the gate to  LDD overlap region was identified. Physical characterization  on an inline split wafer identified residual deposits on the BL  contacts potentially blocking the implant. A thorough  understanding of the layout provides a more comprehensive  model for the fail mode. Enhanced cleans for resist removal  was implemented as a fix.


Acknowledgements:


We would like to thank Kamyar Ahmadi-Majlan and Markus  Kagerer from Thermofisher Inc for providing CV  measurement application support. We would also like to thank  Liangshan Chen for Nanoprobing measurement support and  Sam Zhang for sharing his process knowledge.


References:


[1] L. Liu et al, “Combination of SCM/SSRM analysis and  Nanoprobing technique for soft single bit failure analysis”, Proc. of ISTFA, p.38-41 (2004).


[2] C. M. Shen et al, “Combine Nano-Probing Technique with  Difference Analysis to Identify Non-Visual Failures”, Proc. of  ISTFA, p.264-267 (2006).


[3] C. P. Lin et al “Nano-probing Application on  Characterization of 6T-SRAM Single Bit Failures with  Different Gox Breakdown Defect”, Proc. of ISTFA, p.517-520 (2006).


[4] R. E. Stallcup II et al “Measuring Static Noise Margin of  65nm Node SRAMs Using a 7-point SEM Nanoprobing  Technique”, Proc. of ISTFA, p.223-225 (2007).


[5] H. S. Lin et al, “An Application of a Nanoprobe Technique  in the Characterization of Advanced SRAM Devices”, Proc. of  ISTFA, p.417-422 (2008).


[6] E. Hendarto et al, “Investigation on Focused Ion Beam  Induced Damage on Nanoscale SRAM by Nanoprobing”, Proc. of ISTFA, p.445-448 (2008).


[7] Keithley application note series, “C-V characterization of  MOS Capacitors using the model 4200-SCS semiconductor  characterization system”


[8] Agilent Technologies: The Parametric Measurement


Handbook pg.160, Third Edition, March 2012


[9]K. Inoue et al, “Capacitance-Voltage Test using a SEM  Nanoprober” Zyvex instruments (2009).


Figure 12: Same layout as Figure 10 without any contact  showing the  actual environment during implantation. The red arrows shows poor clearance for cleans on both  sides for PG devices. The green arrows correspond to  good clearance.


276


Development of a Characterization Workflow for Reliable Porous Copper Films using  SEM-FIB Tomography and Advanced Image Analysis


Andi Wijaya, Jördis Rosc, Bernhard Sartory, Roland Brunner


Materials Center Leoben Forschung GmbH, Styria Austria


Barbara Eichinger, Martin Mischitz


Infineon Technologies Austria AG, Carinthia Austria


The development of a characterization workflow for reliable  pore characterization of porous metals especially for  microelectronics applications is very important. This will help  to provide design guidelines for the production and for the  improved reliability of the devices. In this paper, we set up a  workflow to accurately evaluate the porosity, of four different  porous copper materials. The porous thin films are fabricated  by using stencil printing. Within the workflow we use for the  measurement non-destructive micro-X-ray computed  tomography (-XCT) and destructive high-resolution scanning  electron focused ion beam nano-tomography (nano-FIB  tomography). The latter will be also used to calibrate the  threshold for the -XCT image data, since a direct evaluation  of the porosity from the non-destructively obtained -XCT  image data due to resolution and contrast is not possible. Therefore, we develop an indirect histogram based evaluation  method to get the porosity of the porous copper thin films. We  validate and discuss the obtained results with respect to further  studies.


The trend in the semiconductor industry is driven by  miniaturization and enhanced functionality as well as high  power densities. Moore´s law and More than Moore [1] are  keywords in this context.  Both trends lead to enhanced device  performance but also trigger challenges with respect to the  materials e.g. residual stress formation [2] or non-efficient  thermal management [3]. This of course has significant impact  on the device functionality and the reliability, since it may lead  to failure and eventually to the breakdown of the device. To  keep the trend going, it is necessary to introduce new material  concepts. One possibility, displays the use of porous materials. The use of porous materials may help to improve the  performance in e.g. die attach-, metallization-, or dielectricsapplications. However, we need the expertise about the  morphology on micro- & nano-scales. Especially the pore  properties for instance defined by the porosity, pore network  behavior, orientation, and pore distribution are important, since  those are directly related to the mechanical, thermal and  electrical behavior of the porous material. Secondly, we need to  link the expertise of the morphology obtained from the  characterization to the processing via a dynamical iterative  approach that is establish a feedback loop between the two. This  should help to provide improved design guidelines and  establish more advanced as well as reliable products.


Nevertheless, there are certain challenges connected to this  approach in terms of the right method toolbox and workflow to  quantify the pore properties. For such complex materials, 2D  characterization is not sufficient anymore and needs more  advanced microscopy approaches with respect to 3D imaging  and data analysis.


Two image based characterization methods, which are suitable  to characterize pore properties in the lab environment and on  different length scales, are scanning electron focused ion beam  nano-tomography (nano-FIB tomography) [4] and micro-X-ray  computed tomography (-XCT) [5].


Figure 1. Workflow showing the measurement of 3D data  towards the determination of the microstructure and pore  properties.


Nano-FIB-tomography shows high resolution down to the nm  scale as well as high contrast. However, disadvantages are the


277


long FIB slicing times for a representative 3D volume (about  10h), the small possible volume of interest (VOI) and the  destructive nature of the measurement. On the other hand, -XCT represents a non-destructive experimental method, shows  in comparison to nano-FIB tomography fast scanning times (about 2h) and does not need sophisticated sample preparation. It also provides larger VOIs, which can range up to the mm  scale. However, possible disadvantages are the resolution and  contrast, which are mainly determined by the focal spot size, sample material, target and detector.  Both, nano-FIB  tomography and -XCT generate artefacts in the image data. For the nano-FIB tomography, and especially for porous  materials shine through, curtain and shadowing artefacts play a  major role [6]. For instance beam hardening and ring artefact  are mainly seen in the -XCT data [7].   The correction of the  image data with respect to the various artefacts is mandatory for  the subsequent segmentation of the pore space and further  reliable analysis. Several segmentation methods are reported in  literature. According to Iassonov et al., Otsu and Ridler (IsoData) threshold methods produced adequate results with -XCT data [8]. For images obtained from light microscopy, Sezgin et al. [9] stated that cluster- and entropy- based threshold  methods are consistently better than histogram shape-, object  attribute-, spatial-, and local-based threshold methods [9]. Threshold methods are quiet popular for porous materials  segmentation.


In this paper, we develop a workflow (Fig. 1) using two image  based 3D methods namely nano-FIB tomography and -X-ray  computed tomography.  Since a direct evaluation of the porosity  from the non-destructively obtained -XCT image data is not  possible we develop an indirect histogram based evaluation  method to get the porosity of the porous copper thin films. Therefore, we use nano-FIB-tomography to calibrate the  threshold. First, we perform destructive high-resolution nanoFIB tomography, we pre-process the image data to reduce  artefacts and enhance the image quality. In the second stage, we  segment the data and find the correct threshold to separate the  pore space from the copper matrix. We use the manual  segmentation, Otsu, entropy, and IsoData and compare the  results. In the post-processing stage, we analyze the porosity. Finally, we use the nano-FIB tomography results to analyze the -XCT data with respect to the porosity of the porous thin films. We provide a critical discussion with respect to the reliable  evaluation of the 3D porosity using the two measurement  methods and discuss next steps in this context.


Material


We use porous copper foils as sample materials for our  measurements. The foils are fabricated by means of stencil  printing of the porous copper paste. The copper paste consists  of metal particles, solvents and organic components. The paste  is pressed through the apertures of a stencil and deposited onto  a Si(100)  substrate. After printing, the deposited copper is  processed at elevated temperatures and in a controlled formic  acid atmosphere. The solvent evaporates and the organic  components dissociates, enabling the metal particles to  agglomerate and to sinter until an interconnected porous copper


network is formed. By adjusting the basic paste material and  process parameters, including print pressure and speed, gas  flow, ramp rates, plateau temperatures etc., four copper foils  with different porosities and pore morphologies (A, B, C, and  D) are produced.  The thickness of these foils varies between  11 and 32 µm (Table 1).


Thickness [µm]


29.8 ± 1.1


21 ± 1.7


30.8 ± 1.7


12.4 ± 0.9


Table 1. Thickness measurement with a micrometer.


Methods: SEM-FIB and -XCT


We use a cross-beam scanning electron microscope from Zeiss (AURIGA® - CrossBeam workstation) which provides a  combination of a focused ion beam (FIB) with a scanning  electron microscope (SEM). The electron beam allows nondestructive observation of the pores, while the FIB is used for  the milling.  First, a cube is defined by ion-milling then the  vertical face of the cube is milled with the ion beam. A SEM  image of the face is taken at 54o angle by a SESI detector. We  select for the SEM imaging an acceleration voltage of 30kV and  milled the cube slice by slice with a current and voltage of 2nA  and 30kV, respectively to avoid any sample damage.  For the  analysis, we choose a volume of interest (VOI) with about 10 m x 10m x 10m. We select the location of the VOI to  neglect any influence from the surface e.g. resulting from the  deposited Pt (Fig. 2a). The cutting depth is 100 nm in zdirection. For x- and y-direction, the resolution is 10 nm and 10  nm, respectively.  From these images, we reconstruct the 3D  dataset with Avizo.


Figure 2. (a) nano-FIB tomography and (b) -XCT data of the  porous copper layers. The corresponding VOI is illustrated.


278


For the μ-XCT measurements, a nanotom m from General  Electrics (GE) is used. The voxel size is 500-700 nm depending  on the sample. The focal spot size is 800 nm, and the detector  gives 3072 x 2400 pixels. After the measurement and  reconstruction, we crop the 3D data to avoid surface  information. The VOI gives an average dimension of 5 x 106 μm3  (Fig. 2b).  We perform for statistical reasons four (X1-X4) μ-XCT measurements of sample A, four (X1-X4) measurements of sample B, three (X1-X3) measurements of  sample C, and two (X1-X2) measurements of sample D.


Data Pre-Processing


The most common artifacts of nano-FIB tomography of porous  materials are shine-through, curtaining, and shadowing [6] (Fig. 3). In particular, the shine-through artifact plays an important  role for porous materials. Those provide unwanted background  information in the image, which makes the distinction between  pore space and copper matrix within the segmentation operation  difficult. Curtaining is caused by the inhomogeneity of the  surface material and subsurface material. A shadowing effect is  caused by the distance difference for the secondary electrons, which reach the detector.  For the artefact reduction of nanoFIB tomography, Shearing et al. [10] reduces the effect of  shadowing by the lift out method. In order to avoid shinethrough and curtaining artefacts, Tallion et al. [6] infiltrated the  porous network with a low viscosity epoxy resin.


Figure 3. Various nano-FIB tomography artefacts are  presented in the in the image.


The most harmful artefact in XCT data is beam hardening [5]. The X-ray source for the -XCT system generates a  polychromatic beam where each energy spectrum has different  attenuation efficiency. The lower energy X-ray spectrums are  easier to be attenuated than higher energy X-ray spectrums. Beam hardening causes an inhomogeneity of the voxel  brightness for the same material in the image and gives false  information regarding the sample´s composition/density. In  particular, it causes negative impact when trying to segment  materials by intensity difference that is through global  thresholding (Fig. 4). Another type of artifact in XCT data  displays for instance the ring artifact [7]. We use for the  reduction of the -XCT artefacts the GE reconstruction  software Datos|x.


Figure 4. Example of beam hardening artefact within the μXCT data. It shows different gray values at different locations  on the slice and between different slices for the same materials (copper and pore).


We reduce the curtain artefact by non-local means filter using  Avizo. To reduce the shadowing artefact, we aligned the main  peak in the grey value histogram for all slices and three planes  to a defined grey value. The corresponding results before and  after the histogram shifting are shown in Fig. 5.


Figure 5. Correction operation by aligning the mode of the  histograms’ slices for the nano-FIB tomography data.  The  correction operation makes the histograms of each data more  homogeneous.


Results: Pore Segmentation/Thresholding


We segment the nano-FIB-tomography data with Otsu, Entropy, IsoData, and compare the results with the manual  segmentation result. The evaluated porosity for the different  segmentation approaches is presented in Table 2. Here, the  porosity is defined as the fraction of the void volume over the


279


total volume within the VOI. As shown in Table 2, the obtained  porosity gives different values for the different methods. This  evaluated deviation can be explained by looking at Fig. 6. Here, a representative slice grey value image obtained from the nanoFIB tomography and the segmented pore space projected on top  of the grey value image for the different segmentation  approaches is presented. The carefully performed manual  segmentation shows, that the pore space is segmented very well  from the copper matrix. In comparison to the manual  segmentation the Otsu, Entropy and IsoData approach struggle  with the accurate segmentation of the pore space due to the  shine-through artifact (Fig. 6).


Figure 6. (a) Manual method is used as the ground truth. (b) Otsu method, (c) Entropy-, and (d) IsoData method is used to  segment the pores from the nano-FIB tomography data. Examples of segmentation errors due to the shine-through  artefact are highlighted by a red circles.


The grey value image data obtained from the XCT  measurements strongly correlates with the density of the  material due to Beer-Lambert law. For the XCT data a high  density material can be associated with light grey, whereas a  low density material with dark grey or black for air.  In the next  step we used the Otsu, Entropy, and IsoData methods to  perform the segmentation, based on the different intensities for  the -XCT data. In Table 3 it can be seen that the porosity  obtained from the -XCT using Otsu, Entropy, and IsoData  deviates from the nano-FIB tomography result. A manual  segmentation of the -XCT data is difficult as shown in Fig. 4  due to the lack of contrast between the pore- and the copper  space. The use of the manual segmentation as a ground of truth  is therefore not meaningful for the -XCT data.  In order to  analyze the -XCT data and use the advantages of the -XCT  with respect to scanning time, size of the VOI and the nondestructive measurement capability we use a combination of  nano-FIB tomography and XCT. Therefore, we use the high  contrast and resolution nano-FIB tomography for calibration of  the threshold and evaluate the porosity indirectly by a histogram  based evaluation method using the XCT data (Fig. 7a and  Fig.7b).


Gray value


Figure 7. (a) The original -XCT histograms are showing  various distributions, which cause difficulties for the  segmentation operation. (b) Corrected histograms.


Nano-FIB Tomography Porosity [%] Manual


Otsu


Entropy IsoData


33.5


23.6


26.5


23.4


55.0


33.8


33.4


31.1


19.6


20.7


19.4


36.1


25.4


23.8


25.1


Table 2. Evaluated porosity using various analysis methods (nano-FIB tomography data).


In Fig. 7b, we show the different histograms for the different  measured samples. Here the shapes of the histograms for the  same material show similar behavior i.e. similar full width at  half maximum (FHMW). In addition, the FHMW of the  distribution correlates with the porosity. The larger the FHMW  is, the larger is also the porosity. For instance, sample B shows  the largest porosity and gives the largest FHMW. We aligned  the right tails of the histograms to an arbitrary value. Then we


use a threshold value obtained from the nano-FIB tomography  data for one sample as a sort of calibration. Subsequently, the  porosities of the different materials can be evaluated. With this  technique we can show that the porosities of sample A, B, and  C show similar values to the one obtained from the nano-FIB  tomography (Fig. 8). Only sample D shows a strong deviation.


Figure 8. Histogram alignment method for -XCT. The second  peak of the 2nd derivative of the histogram is aligned to a value  of 45000 (blue line). The segmentation of the pore and solid  phase is done by choosing a threshold of 37000 (red line).


Porosity (%) μ-XCT


FIB


Otsu Entropy Iso Data Histogram Alignment Average Histogram Alignment


X1 35.5


3.4


35.5


36.4


33.6


X2 39.4


39.4


30.0


X3 41.8


1.3


41.8


36.7


X4 38.9


1.8


38.9


31.2


X1 38.6


2.3


38.6


52.1


52.5


X2 38.8


38.8


X3 39.4


1.0


39.3


50.4


X4 38.5


3.7


38.4


55.2


X1 25.8


25.8


31.5


29.2


X2 27.3


27.3


26.9


X3 22.2


22.2


D X1 53.7


53.6


5.9


7.6


X2 50.3


50.2


9.3


Table 3. Segmentation results for the μ-XCT image data using  various image analysis methods as well as the nano-FIB  tomography results.


Discussion & Conclusions


We presented a workflow, which consists of the pre-processing, pore segmentation/thresholding and post-processing step to  evaluate accurately the porosity of porous copper thin films. Therefore, we used in a first attempt nano-FIB tomography. We  successfully showed that in particular the shine through artefact  causes severe problems for the segmentation of the pore space.


Commonly used methods like Otsu, Isodata or Entropy based  algorithm are not suitable for the detection.


This was shown by comparing the obtained results with the  manual segmentation. The smallest pore size shows sample D, which provides a mean value of about 178 nm [11]. In our case, we used a voxel size of 10 x 10 x 100 nm3 for the nano-FIB  tomography, which reflects the resolution limit of our  investigations. Smaller cutting depth in z-direction with the  used setup is possible, however will result in far longer  measurement times.


Since nano-FIB tomography displays a destructive method, we  also used non-destructive -XCT. The direct extraction of the  porosity from the -XCT was not possible due to the lack of  resolution and contrast. In order to take advantage of the -XCT  with respect to scanning time, the non-destructive nature of the  method as well as the possible size of the VOI, we use a  histogram based evaluation method. Therefore, we used the  threshold obtained from the nano-FIB tomography. We could  show that the porosity for sample A, B and C obtained from the -XCT data matches very well with the porosities obtained  from the manually segmented nano-FIB tomography data (Tab.3). However, for sample D, a large deviation for the  porosity obtained from nano-FIB tomography (36.1%) and -XCT (7.6%) is observed (Tab.3). According to the image data  we conclude that this deviation in sample D results from the  nano-sized behavior of the pores (~178 nm). The voxel size of  500 nm is not sufficient for sample D.


Although -XCT has certain advantage as mentioned above its  application is limited by the possible resolution and contrast. Here, nano-FIB tomography, although destructive and showing  longer acquisition times has clear advantages. However, the  manual segmentation of the pore space in order to avoid shine  through artefacts takes too long especially if we think about the  characterization in an industrial environment. The infiltration  with an epoxy resin may help but displays and additional step  in the workflow. In addition, it will only work for open porous  systems. An improvement of the image analysis would be more  straightforward. In terms of the image analysis, the automation  of the segmentation may provide here a much faster analysis  and could improve the characterization workflow. Therefore, the next step in our studies shall be the development and  application of such an automated image analysis algorithm to  shorten the analysis time and avoid the manual segmentation of  each sample as well as the transfer of the 3D data to finite  element simulations and its combination with experiments like  nanoindentation and electrical four point probe measurements


[11]. The latter shall correlate functionality with structural  properties and shall help to improve reliability.


Financial support from FFG , Produktion der Zukunft (No.


853467 “ProQualiKu”) and by the Austrian Federal


Government (in particular from Bundesministerium für  Verkehr, Innovation und Technologie and Bundesministerium  für Wissenschaft, Forschung und Wirtschaft) represented by


281


Österreichische Forschungsförderungsgesellschaft mbH and  the Styrian and the Tyrolean Provincial Government, represented by Steirische Wirtschaftsförderungsgesellschaft  mbH and Standortagentur Tirol, within the framework of the  COMET Funding Programme (No. 837900) is also gratefully  acknowledged.


[1]  W. Arden, "More than Moore White Paper," International Roadmap for Semiconductor ITRS, 2010.


[2]  R. Treml, D. Kozic, K. Zechner, X. Maeder, H.-P. Gänser, R. Schöngrundner, J. Michler, R. Brunner and D. Kiener, "High Resolution Determination of Local  Residual Stress Gradients in Single- and Multiple- Thin  Film Systems," Acta Materialia, vol. 103, pp. 616-623, 15 January 2016.


[3]  J. Broughton, V. Smet, R. R. Tummala and Y. K. Joshi, "Review of Thermal Packaging Technologies for  Automotive Power Electronics for Traction Purposes," Journal of Electronic Packaging, vol. 140, no. 4, 20  August 2018.


[4]  E. Widiatmoko, A. Mikrajuddin and Khairrurrijal, "A  method to measure pore size distribution of porous  materials using scanning electron microscopy images," The third nanoscience and nanotechnology sypposium, pp. 23-26, 2010.


[5]  D. Wildenschild and A. Sheppard, "X-ray Imaging and  Analysis Techniques for Quantifying Pore-scale  Structure and Processes in Subsurface Porous Medium  Systems," Advances in Water Resources, vol. 51, pp. 217-246, 2013.


[6]  J. A. Tallion, C. Pellegrinelli, Y. Huang, E. D. Wachsman  and L. G. Salamanca-Riba, "Improving Microstructural  Quantification in FIB/SEM Nanotomography," Ultramicroscopy, vol. 184, no. Part A, pp. 24-38, January


[7]  R. Ketcham and W. Carlson, "Acquisition, Optimization  and Interpretation of X-ray Computed Tomography  Imagery: Applications to the Geosciences," Computers & Geosciences, vol. 27, pp. 381-400, 2001.


[8]  P. Iassonov, T. Gebrenegus and M. Tuller, "Segmentation  of X-ray Computed Tomography Images of Porous  Materials: A Crucial Step for Characterization and  Quantitative Analysis of Pore Structures," Water Resouce  Research, vol. 45, no. W09415, 2009.


[9]  M. Sezgin and S. Bulent, "Survey over Image  Thresholding Techniques and Quantitative Performance  Evaluation," Journal of Electronic Imaging, vol. 13, no. 1, pp. 146-165, January 2004.


[10]  P. Shearing, J. Golbert, R. Chater and N. Brandon, "3D  Reconstruction of SOFC Anodes Using a Focused Ion  Beam Lift-out Technique," Chemical Engineering  Science, vol. 64, pp. 3928-3933, 2009.


[11]  A. Wijaya, et al., "3D Analysis Workflow to Design  Mechanical and Electrical Properties of Porous Copper


Films for Microelectronics Applications".(in  preparation).


282


Speeding up Chip Layer Imaging with a Multi-Beam SEM


A. L. Eberle, T. Garbowski, S. Nickell, D. Zeidler


Carl Zeiss Microscopy GmbH, Carl-Zeiss-Str. 22, D-73447 Oberkochen, Germany  email: anna-lena.eberle@zeiss.com, phone: +49 7364 20-0


Reverse engineering of today’s integrated circuits requires  proper sample preparation, high speed imaging and data  processing capabilities. The electron-optical design and the  data handling architecture of our multi-beam scanning electron  microscopes are scalable over a large range of beam numbers, providing sufficient imaging speed - also for the foreseeable  future. A first step in data processing for reverse engineering  on images acquired with a multi-beam scanning electron  microscope has been successfully shown in preliminary tests.


Reverse engineering of semiconductor integrated circuits (ICs) enables detection of violations of intellectual property or  adverse manipulations of product designs. The continuous  shrink of semiconductor patterns imposes several challenges  not only on the fabrication of ICs, but also on the imaging of  their structures as used in process control and reverse  engineering. Scanning electron microscopes (SEMs) can  resolve the relevant patterns of modern ICs, but so far have not  been able to achieve the throughput requirements for large  area screening at a practicable, application relevant time  frame. On top of that, the need for the analysis of more and  larger chip areas is increasing.


Using a multi-beam SEM for image acquisition increases the  throughput dramatically and therefore allows to image entire  chips. In this article, we will present high speed multi-beam  SEM imaging in context with state-of-the-art reconstruction  and analysis of modern integrated circuits.


High-Throughput Multi-Beam SEM Imaging


Commercial multi-beam SEMs are routinely used in life  sciences applications [1] and are currently explored for use in  metrology and inspection workflows in semiconductor industry


[2]. The technical setup of the multi-beam SEM is depicted in  figure 1 and has been described in detail [1]. In a nutshell, the  multi-beam SEM circumvents the throughput limitations of  standard, single-beam SEMs by using multiple electron beams  in parallel. Increasing the speed of a single-beam SEM could  be achieved by faster scanning, which in turn would require  higher beam current to still generate enough signal from the  sample. Due to electron-electron interactions, this will impair  the spot size of the electron beam and therefore the achievable  resolution. By spreading the current over multiple beams, these limitations can be avoided. Presently two different  systems with 61 and 91 beams and equipped with a standard  100 mm SEM sample stage are commercially available. Given  the increasing need for imaging larger areas in even shorter  time, further throughput enhancements of the mSEM® technology towards 331 beams are already on the way [3].


Figure 1, left: Schematics of the multi-beam scanning electron microscope. For simplicity, only seven beams are shown. Multiple  primary electron beams (blue) are scanned within a single column in parallel over the sample; secondary electron beams (green) are  detected in parallel by individual detectors. Right: Image of the secondary electron signal at the detector plane, stemming from 331  electron beams.


# Speeding up Chip Layer Imaging with a Multi-Beam SEM


283

