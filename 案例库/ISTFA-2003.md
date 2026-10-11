---
title: "ISTFA-2003.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_c8f1cbed39e1630504bc235e8468fee57295230462135641
file_size: 97557679
---

"


~15);4/2003


Proceedings of the


29th International Symposium for Testing and Failure Analysis


2-6 November 2003


Santa Clara Convention Center Santa Clara, California


Sponsored by


EDFAS Electrenic Devica Failure Amalysls Society


M_SOl:il!lrOfASM_


Published by


ASM International


Materials Park, Ohio 44073-0002


Copyright © 2003


by


ASM International@


All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any means, electronic, mechanical, photocopying, recording, or otherwise, without the written permission of the copyright owner.


First printing, OCtober 2003


Great care is taken in the compilation and production of this book, but it should be made clear that NO WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN CONNECTION


WITH THIS PUBLICATION. Although this information is believed to be accurate by ASM, ASM cannot guarantee that favorable results will be obtained from the use of this publication alone. This pUblication is intended for use by persons having technical skill, at their sole discretion and risk. Since the conditions of product or material use are outside of ASM's control, ASM assumes no liability or obligation in connection with any use of this information. No claim of any kind, whether as to products or information in this publication, and whether or not based on negligence, shall be greater in amount than the purchase price of this product or publication in respect of which damages are claimed. THE REMEDY HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND SOLE REMEDY OF BUYER, AND IN NO EVENT SHALL EITHER PARTY BE LIABLE FOR SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES WHETHER


OR NOT CAUSED BY OR RESULTING FROM THE NEGLIGENCE OF SUCH PARTY. As with any material, evaluation of the material under end-use conditions prior to specification is essential. Therefore,specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or reproduction, in connection with any method, process, apparatus, product, composition, or system,whether or not covered by letters patent, copyright, or trademark, and nothing contained in this book shall be construed as a defense against any alleged infringement of letters patent, copyright, or trademark, or as a defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN: 0-87170-788-8


SAN: 204-7586


Materials Park, OH 44073-0002


www.asminternational.org


Printed in the United States of America


Multiple copy reprints of individual articles are available from Technical Department, ASM International.


ISTFA 2003 Organizing Committee  Thomas M. Moore


Matthew Thayer


General Chair


Vice General Chair


Omniprobe, Inc.


Advanced Micro Devices


Dallas, TX


Austin, TX


Committee Members:


Committee Liaisons:


Anu Barman


Christian Boit


Publicity Chair


Past General Chair


Los Altos, CA


TUB Berlin University of Technology  Berlin, Germany


Cheryl Hartfield


Seminar Vice Chair


Sandra Delgado


Texas Instruments


EDFAS Liaison


Accurel Systems International  Sunnyvale, CA


Christopher L. Henderson


Audio Visual Chair


Richard J. Ross


Sandia National Laboratories


EDFAS President


Albuquerque, NM


IBM Microelectronics Division  Essex Junction, VT


Dan J. Bodoh


Exposition Chair  Motorola, Inc.


Ingrid J. DeWolf


A/V Vice Chair  IMEC


Leuven, Belgium


Lee Knauss


Technical Program Chair  Neocera, Inc.


Beltsville, MD


Kendall S. Wills


Seminar Chair


Texas Instruments  Stafford, Texas


Travis M. Eiles


Panel/User Group Chair  Intel Corporation


Santa Clara, CA


# ISTFA 2003 Organizing Committee


EDFAS 2003 – 2004 Board Of Directors


Richard Ross


Gary Shade


President


Vice President


IBM Microelectronics Division


Intel Corporation


Essex Junction, VT


Colorado Springs, CO


Board Members:


Committee Chairs:


Reza Abbaschian


ASM Board of Trustees Liaison


Ex-Officio Member


University of Florida


Gainesville, FL


Gainsville, FL


Daniel L. Barton


Education Committee


Secretary


Sam Subramanian


Motorola, Inc.


Events Committee


Member At Large


Thomas M. Moore


TUB Berlin University of Technology


Berlin, Germany


Edward I. Cole, Jr.


Magazine Committee


Immediate Past President


Chuck F. Hawkins


University of New Mexico


Membership Committee


Seshagiri Pabbisetty


Accurel Systems International


Sunnyvale, CA


Stafford, TX


James J. Erickson


Nominating Committee


Boeing Satellite Systems, Inc.


Los Angeles, CA


Glen P. Gilfeather


Publications Committee


Finance Officer


Website Committee


Jacob C. H. Phang


National University of Singapore  Singapore


# EDFAS 2003 – 2004 Board Of Directors


ISTFA 2003 Subcommittee Members


|ADVANCED TECHNIQUES |David P. Vallett, Chair |IBM Microelectronics |Division – Essex Junction, VT |
|---|---|---|---|

||Brennan V. Davis |Advanced |Micro Devices – Austin, TX |

||Zhiyong Wang |Intel |Corporation – Chandler, AZ |

||Jerry M. Soden |Sandia |National Laboratories – Albuquerque, NM |

||Siva Kolachina |Texas Instruments |– Stafford, TX |

||Michael R. Bruce |Advanced Micro |Devices – Austin, TX |

||Michael S. Twiford |Agere |Systems – Allentown, PA |

||Jim Cargo |Agere Systems |– Allentown, PA |

||Ted H. Hasegawa |National Semiconductor |Corp. – Santa Clara, CA |

|AUDIO VISUAL |Christopher L. Henderson, Chair |Sandia National |Laboratories – Albuquerque, NM |

||Ingrid DeWolf, Vice Chair |IMEC – Leuven, |Belgium |

||J. Joseph Clement |Sandia National |Laboratories – Albuquerque, NM |

||Tom Libbey |National |Semiconductor – Arlington, TX |

|PANEL / USER GROUPS |Travis M. Eiles, Chair |Intel Corporation |– Santa Clara, CA |

|SEMINAR |Kendall S. Wills, Chair |Texas Instruments |– Stafford, TX |

||Cheryl Hartfield, Co-Chair |Texas |Instruments – Dallas, TX |

||JoAn S. Hudson |University |of Oregon – Eugene, OR |

||Susan Li |Advanced Micro |Devices – Sunnyvale, CA |

||Tracy D. Myers |LSI Logic |Corporation – Gresham, OR |

||Chris Richardson |LSI Logic |Corporation – Fort Collins, CO |

||Rosalinda M. Ring |Intel |Massachusetts, Inc. – Hudson, MA |

||William E. Vanderlinde |Laboratory for |Physical Sciences – College Park, MD |

||Brent A. Wahl |Agilent |Technologies – Newark, CA |

||Jeremy A. Walraven |Sandia |National Laboratories – Albuquerque, NM |

||Bradley A. Waterson |Analog |Devices – Cambridge, MA |

|CIRCUIT EDIT |Ted C. Tessner, Chair |FEI |Company – Hillsboro, OR |

||Michel Dibattista |Intel |Corporation – Santa Clara, CA |

||Ted Lundquist |NP Test – |San Jose, CA |

||Nicholoas Antoniou |FEI Company |– Peabody, MA |

||Loren F. Vermont |Department |of Defense – Fort Meade, MD |

|DIE LEVEL FAULT ISOLATION |Philippe Perdu, Chair |CNES – Toulouse, |France |

||Dan J. Bodoh|||

||Jerome Touzel |Infineon Technologies – Munich, Germany |Infineon Technologies – Munich, Germany |

||Robert E. Lamothe |R&L Technologies, Inc. – Annapolis, MD |R&L Technologies, Inc. – Annapolis, MD |

||Jacob C. H. Phang |National University of Singapore – Singapore |National University of Singapore – Singapore |

||Ted Lundquist |NPTest – San Jose, CA |NPTest – San Jose, CA |

||Christopher L. Henderson |Sandia National Laboratories – Albuquerque, NM |Sandia National Laboratories – Albuquerque, NM |

||Martine Simard-Normandin |MuAnalysis, Ottawa – Ontario, Canada |MuAnalysis, Ottawa – Ontario, Canada |

||Felix Beaudoin |Thales Microelectronics – Toulouse, France |Thales Microelectronics – Toulouse, France |

||Peter J. Jacob |EMPA Swiss Federal Labs – Duebendorf, Switzerlan |EMPA Swiss Federal Labs – Duebendorf, Switzerlan |

||Scott R. Lovell |Analog Devices – Wilmington, MA |Analog Devices – Wilmington, MA |

|DISCRETES & PASSIVES |Gary M. Molle, Chair |Kaiser Electronics – San Jose, CA |Kaiser Electronics – San Jose, CA |

||James J. Erickson |Boeing Satellite Systems, Inc. – Los Angeles, CA |Boeing Satellite Systems, Inc. – Los Angeles, CA |

||Stan Silvus |Southwest Research Institute – San Antonio, TX |Southwest Research Institute – San Antonio, TX |

||Gary Ewell |The Aerospace Corporation – Los Angeles, CA |The Aerospace Corporation – Los Angeles, CA |

||Michel J. Cozzolino |Boeing Satellite Systems, Inc. – Los Angeles, CA |Boeing Satellite Systems, Inc. – Los Angeles, CA |

Motorola, Inc. – Austin, TX


d


# ISTFA 2003 Subcommittee Members


FA PROCESS


Richard J. Ross, Chair


IBM Microelectronics Division – Essex Junction, VT


Richard E. Anderson


Sandia National Laboratories – Albuquerque, NM


Steven R. Hoffman


Tillamook Watershed Resource Ctr. – Bay City, OR


Tan-Chen Lee


Taiwan Semiconductor Manufacturing Company, LTD. Hsin-Chu, Taiwan


Tracy D. Myers


LSI Logic Corporation – Gresham, OR


Christian Plougonven


Consultant, Samois sur Seine – France


Rosalinda M. Ring


Intel Corporation – Hudson, MA


METROLOGY AND


MATERIALS ANALYSIS


William E. Vanderlinde, Chair


Laboratory for Physical Sciences – College Park, MD


Bryan Tracy


Advanced Micro Devices – Sunnyvale, CA


Edward Coyne


Analog Devices – Limerick, Ireland


Ying Zhou


Intel Corporation – Hillsboro, OR


Gerry Scilla


OPTICAL TECHNIQUES


R. Aaron Falk, Chair


OptoMetrix, Inc. – Renton, WA


Victoria J. Bruce


Advanced Micro Devices – Austin, TX


Jim Cargo


Agere Systems – Allentown, PA


Tim A. Hazeldine


Ultratec Manufacturing, Inc. – Santa Ana, CA


Steven Kasapi


Optonics – Mountain View, CA


Thomas Kujawa


Hypervision – Fremont, CA


Ted Levin


Winfield Scott


MEFAS, Inc. – Lake Forrest, CA


Paiboon Tangyungyong


Lawrence C. Wagner


Texas Instruments – Dallas, TX


OPTOELECTRONIC  DEVICES


Daniel L. Barton, Chair


Robert J. Herrick


Agilent Technologies – San Jose, CA


Jie Xue


Cisco Systems, Inc. – Salem, NH


Massimo Vanzi


University of Cagliari – Cagliari, Italy


Kei-Wean Yang


Tektronix, Inc. – Beaverton, OR


PACKAGE LEVEL  ANALYSIS


Rajen C. Dias, Chair


Intel Corporation – Chandler, AZ


Deepak Goyal


Intel Corporation – Chandler , AZ


Rama Goruganthu


Omniprobe Inc. – Dallas, TX


Douglas Hunt


POSTER


Sandra Delgado, Chair


Accurel Systems International  – Sunnyvale, CA


Perry Martin


Martin Testing Laboratories – North Highlands, CA


David H. Su


Taiwan Semiconductor Manufacturing Company, LTD.  Hsin-Chu, Taiwan


Jack D. Henderson


Naval Surface Warfare Center – Crane, IN


Felix Beaudoin


Thales Microelectronics – Toulouse, France


Wayez Ahmad


Intel Corporation – Sacramento, CA


SAMPLE PREPARATION


Edward P. Keyes, Chair


Semiconductor Insights – Ottawa, Ontario, Canada


Michael W. Ruprecht


Infineon Technologies – Williston, VT


Mark E. Kimball


Maxim Integrated Products – Beaverton, OR


Ray F. Haythornthwaite


SPM


Peter J Harris, Chair


Digital Instruments Veeco – Santa Barbara, CA


Andy Erickson


Multiprobe Corporation – Santa Barbara, CA


Konrad Jarausch


Intel Corporation – Santa Clara, CA


Jeff McMurray


IBM Analytical Services – Hopewell Junction, NY


SYSTEM LEVEL ANALYSIS Jeff Birdsley, Chair


Dell Computer Corporation  – Round Rock, TX


Roger Bjork


Robert V. Knoell


Visteon Corporation – Dearborn, MI


Charlie Zhai


Tom Worley


Sridhar Canumalla


Nokia Mobile Phones – Irving, TX


TEST


Jerry M. Soden, Chair


Rob Aitken


Artisan Components – Sunnyvale, CA


Amy G. Chu


Anne E. Gattiker


IBM Corporation – Austin, TX


University of New Mexico – Albuquerque, NM


Anjali Vij


Texas Instruments – Stafford, TX


YIELD ENHANCEMENT


Thomas Taylor, Chair


Infineon Technologies – Sandston, VA


Alfredo Herrera


Ines Thurner


Infineon Technologies – Munich, Germany


Cary A. Gloor


LSI Logic Corporation – Fort Collins, CO


Preface


# Preface


The ISTFA conference proceedings are an integral part of technical libraries, failure analysis (FA) laboratories and related industries. In this 29th edition, you will find a comprehensive reference of the state-of-theart research, development, tools and techniques presented at ISTFA 2003.


The theme of this year's conference is"Technology Readiness", which has several facets. Most of the attendees at this conference use or are familiar with the International Technology Roadmap for Semiconductors (ITRS), which presents technology forecasts as well as requirements for the means to analyze and characterize these developing technologies. Even in times of prosperity, we have been concerned that we are behind in our efforts to ensure on-time readiness of critical analytical capabilities to support a diverse array of new technologies including sub-100nm device geometries,Cu+low-k interconnect stacks, stacked die packages, MEMS and nanotechnology. It has been a constant challenge to balance the demands of quarterly revenue goals and limited resources with the clear need for continued longer-term development. The current recession in our industry has added yet


additional pressure to these readiness efforts and has caused us, as an industry, to carefully consider how we execute on development projects. In addition, the increased realization on a global scale of the threat of terrorism has established new priorities for the semiconductor technology industry. Initiatives in worldwide intelligence collection and sharing,surveillance, security monitoring and counterterrorism all represent new requirements and new opportunities for the semiconductor industry.


For the many volunteers that have worked to organize ISTFA 2003, the proceedings are part of the climax of a year of hard work. An organization such as ISTFA relies on the energy and dedication of its volunteers. In return, the experience provides an opportunity for valuable networking, refining organizational skills, broadening technical knowledge and for career growth. I encourage anyone interested in participating to get involved. This will be time well spent.


Dr. Thomas M. Moore


General Chair, ISTFA 2003


moore@omniprobe.com


X


Table of Contents


Session 1: Advanced Techniques


# Table of Contents


Scanning Magnetoresistive Microscopy for Die-Level Sub-Micron Current Density Mapping....................... 2


B. Schrag, X.Y. Liu, M.J. Carter, G. Xiao, Micro Magnetics Inc., Providence, Rhode Island, USA


High Resolution Current Imaging by Direct Magnetic Field Sensing .............................................................. 6


S. Woods, N.M. Lettsome Jr., A.B. Cawthorne, L.A. Knauss, Neocera, Inc., Beltsville, Maryland, USA; R.H. Koch, IBM T.J. Watson Research Center, Yorktown Heights, New  York, USA


Fault Isolation of High Resistance Defects Using Comparative Magnetic Field Imaging............................... 9


A. Orozco, E. Talanova, A. Gilbertson, L.A. Knauss, Neocera, Inc., Beltsville, Maryland, USA; Z. Wang, L. Skoglund, D.G. Smith, R. Dias, Intel Corp., Chandler, Arizona, USA


High Resolution Backside Thermography Using a Numerical Aperture Increasing Lens............................ 14


S. Thorne, S. Ippolito, M. Eraslan, B. Goldberg, M.S. Ünlü, Depts. of Physics and Electrical  and Computer Engineering and the Photonics Center, Boston University, Boston,


Massachusetts, USA; Y. Leblebici, Swiss Federal Institute of Technology of Lausanne,


Microelectronics and Microsystems Institute, Lausanne, Switzerland


Session 2: Optical Techniques


Study of Critical Factors Determining Latchup Sensitivity of ICs Using Emission Microscopy.................. 19


F. Stellari, P. Song, M.K. McManus, A.J. Weger, IBM T.J. Watson Research Center, Yorktown Heights, New York, USA; R.J. Gauthier, K.V. Chatty, M. Muhammad, IBM  Microelectronics, Essex Junction, Vermont, USA; P. Sanda, IBM Systems Group,


Poughkeepsie, New York, USA


New Applications of Thermal Laser Signal Injection Microscopy (T-LSIM) .................................................. 25


R.A. Falk, N. Bauersfeld, OptoMetrix, Inc., M. LaPierre, S. Elliott, Fairchild Semiconductor


PC Card Based Optical Probing of Advanced Graphics Processor Using Time Resolved


Emission........................................................................................................................................................... 36


H.L. Marks, T. Ton, NVIDIA Corporation, Santa Clara, California, USA; J.A. Block,  S. Kasapi, C. Shaw, Optonics, Inc., Mountain View, California, USA


Time-Resolved Optical Measurements from 0.13µm CMOS Technology Microprocessor Using a


Superconducting Single-Photon Detector...................................................................................................... 40


F. Stellari, P. Song, A.J. Weger, M.K. McManus, IBM T.J. Watson Research Center, Yorktown Heights, New York, USA


IC Diagnostic with Time Resolved Photon Emission and CAD Auto-Channeling......................................... 45


R. Desplats, A. Eral, F. Beaudoin, P. Perdu, CNES-THALES Laboratory, Tolouse, France; A. Chion, ST Microelectronics, Crolle, France; K. Shah, T.R. Lundquist, NPTest, Inc, San  Jose, California, USA


Session 3: Package Level Analysis 1


3D X-ray Computed Tomography (CT) for Electronic Packages.................................................................... 56


Z. Fu, D. Goyal, J. Thomas, Intel Corporation, Chandler, Arizona, USA; A. Crawley,  A. Ramsey, X-Tek Systems Ltd., Tring, Hertfordshire, United Kingdom


High-Angle Electron Microscopy Technique for Analysis of Thin Film Contamination on IC


Package Exteriors............................................................................................................................................ 62


T. Barbieri, J. Schaper, P. Dimuzio, Motorola Semiconductor Products Sector, Tempe, Arizona, USA


Solder Bump Defects in Ceramic Flip Chip Packages and Their Acoustic Signatures ................................ 68


K. Ramanujachar, D. Rusli, R. Agarwal, J. Widaski, Texas Instruments, Stafford, Texas, USA


Copper Bond Over Active Circuit (BOAC) and Copper Over Anything (COA) Failure Analysis................... 76


D. Nguyen, B. Davis, C. Lewis, Dallas Device Analysis Operation, Texas Instruments Inc., Dallas, Texas, USA


Investigation of Bond-Pad Related Inter-Metal Dielectric Crack.................................................................... 82


Z. Song, T. Tun, C.K. Oh, S. Redkar, B.H. Er, Failure Analysis Group, QRA, Chartered  Semiconductor Manufacturing Limited; C.P. Soo, C.H. Goo, Yield Enhancement


Department, CSP, Chartered Semiconductor Manufacturing Limited


Session 4: Sample Preparation 1


Enhanced SEM Doping Contrast..................................................................................................................... 87


C.Y. Lin, J.H. Lee, Taiwan Semiconductor Manufacturing Company, Hsin-Chu, Taiwan


Interconnect and Gate Level Delayering Techniques for Cu/Low k Technology Failure Analysis............... 90


H. Wu, J. Cargo, B. Dutt, T. Bucha, J. Serpiello, Agere Systems, Quality Organization, Product Analysis Lab, Allentown, Pennsylvania, USA


Backside Deprocessing of CMOS SOI Devices for Physical Defect and Failure Analysis ........................... 99


S. Prejean, J. Shannon, Advanced Micro Devices, Austin, Texas, USA


A Novel Approach to Front-Side Deprocessing for Thinned Die after Backside Failure Isolation............. 105


D. Nguyen, C. Phan, J. Conner, M. Smith, J. Drummond, Dallas Device Analysis Operation, Texas Instruments Inc., Dallas, Texas, USA


Session 5: System Level Analysis


Dynamic Infrared System Level Fault Isolation ............................................................................................ 111


J.A. Naoum, J. Rahardjo, Y. Taffese, M. Chagny, J. Birdsley, J.C. Woo, A. Morris, Dell Inc., Austin, Texas, USA


X-ray Laminography Benchmarking and Failure Analysis of Solder Joint Interfaces ................................ 120


B.A. Thomson, N.J. Armendariz, Intel Corporation, Hillsboro, Oregon, USA


XRF Correlation of Board Reseats Due to Intermittent Failures from the Use of Thin Gold Plating


finish on the Contact Fingers........................................................................................................................ 125


D. Stein, V. Hernandez, M.A. Nailos, Dell Inc., Austin, Texas, USA


Session 6: Metrology and Materials Analysis 1


Real Time SEM Imaging of FIB Milling Processes for Extended Accuracy on TEM Samples for


EFTEM Analysis............................................................................................................................................. 132


P. Gnauck, U. Zeile, P. Hoffrogge, G. Benner, A. Orchowski, W.-D. Rau, LEO Electron  Microscopy Group, Oberkochen, Germany


A Method for Exact Determination of DRAM Deep Trench Surface Area .................................................... 140


J. Russell, Infineon Technologies, Linkou,Taiwan; Y.-W. Tseng, ProMOS Technologies  Inc., Hsinchu, Taiwan


A Review of TEM Observations of Failures of the Memory Cell in a Deep Trench Capacitor DRAM ......... 144


J.-L. Lue, J. Lee, E. Chen, J.-S. Luo, ProMOS Technologies Inc., Hsinchu, Taiwan


The Effect of TEM Specimen Preparation Method on Ultra-Thin Gate Dielectric Analysis......................... 153


A.Y. Du, C.H. Tung, Institute of Microelectronics, Singapore; B.H. Freitag, FEI/Philips  Electron Optics Applications Laboratory, Eindhoven, Netherlands; W.Y. Zhang, S. Lim, Systems on Silicon Manufacturing Co. Pte. Ltd., Singapore; E.H. Ang, D. Ng, TECH


Semiconductor Singapore Pte Ltd., Singapore


Forward Scattered Scanning Electron Microscopy for Semiconductor Metrology and Failure


Analysis.......................................................................................................................................................... 158


W. Vanderlinde, Laboratory for Physical Sciences, College Park, Maryland, USA


Session 7: Failure Analysis Process


Contributions of a Formal Analysis Metaprocess to Breakthrough Failure Analysis Results ................... 167


S. Ferrier, K.D. Martin, D. Schulte, The Hewlett-Packard Company, Corvallis, Oregon, USA


SRAM Failure Analysis Strategy ................................................................................................................... 177


P. Egger, C. Burmer, Infineon Technologies, Munich, Germany


VLSI Design for Functional Failure Analysis in the < 90 nm and Flip-Chip Era .......................................... 184


Y. Weizman, E. Baruch, Motorola Semiconductor Israel - Product Analysis & Characterization


Identification of an IDDQ Failure Mechanism Using a Variety of Front and Backside Analytical


Techniques..................................................................................................................................................... 191


J. Shearer, K. Le, X. Yang, M. Cleeves, A. Meeks, Matrix Semiconductor, Santa Clara, California, USA


Novel Application of Transmission Electron Microscopy and Scanning Capacitance Microscopy


for Defect Root Cause Identification and Yield Enhancement..................................................................... 197


P. Tangyunyong, T.A. Hill, C.Y. Nakakura, J.M. Soden, E.I. Cole Jr., R.S. Flores,


M.R. Shaneyfelt, R.C. Dockerty, T.J. Headley, M.J. Rye, Microelectronics Development  Laboratory, Sandia National Laboratories, Albuquerque, New Mexico, USA


Session 8: Metrology and Materials Analysis 2


Contact Failure Due to Particulate Defect in a 0.13 µm CMOS Process ...................................................... 206


S. Bagchi, V. Arunachalam, J. Saenz, J. Beck, L. Duncan, J. Conner, Motorola Inc., Austin, Texas, USA


Microhardness Testing on Via Fill Material for Via In Pad Technology....................................................... 209


N.J. Armendariz, Intel Corporation, Hillsboro, Oregon, USA; C. McCormick, Intel  Corporation, Chandler, Arizona, USA


Application of ToF-SIMS to Airborne Organic Contamination Analysis...................................................... 215


D. Lu, A. Trigg, Z. Xing, R. Kumar, C.K. Chang, Institute of Microelectronics, Singapore


Session 9: Test 1


Yield-Modeling and Test Oriented Taxonomy of IC Structure Deformations .............................................. 222


W. Maly, T. Zanon, T.J. Vogels, Carnegie Mellon University, Pittsburgh, Pennsylvania, USA


Analysis of IC Manufacturing Process Deformations: An Automated Approach Using SRAM Bit


Fail Maps ........................................................................................................................................................ 232


T. Zanon, M. Ferdman, W. Maly, Carnegie Mellon University, Pittsburgh, Pennsylvania, USA; K. Komeyli, Intel Corporation, Santa Clara, California, USA


Electrical Failure Analysis and Characterization of Leakage Paths Leading to Single Cell


Failures in 128Mbit SDRAMs ......................................................................................................................... 242


M. Versen, A. Schramm, Infineon Technologies AG, München, Germany


Session 10: Posters - Case Studies


A Study on Fluorine-Induced Corrosion on Microchip Aluminum Bondpads............................................. 249


Y.N. Hua, S. Redkar, R. Dickinson, S.S.L. Peh, Chartered Semiconductor Mfg. Ltd., Singapore


Advanced Process Defect Detection by Using Dynamic Bias Condition and MCT Camera....................... 256


C.-W. Wu, J.-H. Lee, Taiwan Semiconductor Manufacturing Company, Ltd., Taiwan


Via Chain Failure Analysis Using a Combination of E-Beam and Optical Beam Techniques .................... 259


S. Perungulam, A. Gleason, Texas Instruments Inc., Stafford, Texas, USA


Session 10: Posters - ESD Failure


ESD Failure Signature Differences in the Devices Core Logic and Protection Structures - A Case


Study .............................................................................................................................................................. 262


L.G. Henry, ESD-TLP Engineering Consultants, Fremont, California, USA


ESD: Correlation between Electrical Signature and Failure Modes............................................................. 272


V. Korchnoy, B. Lisenker, I. Posimeinik, Intel Israel Ltd., Haifa, Israel


Session 10: Posters - Sample Prep


Semi-Automated Cross-Section Preparation Process for Complex Multi-Face Perimeter Samples.......... 278


T. McDonald, Intel Corporation, Hillsboro, Oregon, USA


FIB Micro-Pillar Sampling of Si Devices and its 3D Observation................................................................. 282


T. Yaguchi, T. Kamino, Hitachi Science Systems, Ltd., Ibaraki, Japan; T. Ohnishi,


T. Hashimoto, Hitachi High-Technologies Corp., Ibaraki, Japan; K. Umemura, Central  Research Laboratory Hitachi Ltd., Kokubunji, Japan; K. Asayama, Renesas Technology  Corp., Tokyo, Japan


Recent Developments in Automated Sample Preparation for FESEM......................................................... 288


R.R. Cerchiara, P.E. Fischione, J.J. Gronksy, W.F. Hein, D.D. Martin, J.M. Matesa,


A.C. Robins, D.W. Smith, E. A. Fischione Instruments, Inc., Export, Pennsylvania, USA


Wet Delineation of SEM Samples Having Cu Interconnects ........................................................................ 297


J.B. Lai, Y.P. Wang, J.Y. Kung, Y.C. Fu, R.L. Hwang, D. Su, Taiwan Semiconductor  Manufacturing Company, Hsin-Chu, Taiwan


An Evolution in Plastic Decapsulation Process Improvement..................................................................... 301


N.S. Somcio, A.J. Komrowski, L. Curiel, C.R. Silvis, D.J.D. Sullivan, LSI Logic Corporation, Fremont, California, USA


Session 10: Posters - Techniques


Obtaining Low Contact Resistance for Physical Sub-Micron Fault Isolation.............................................. 305


C.A. Waggoner, D. Smith, The Micromanipulator Co., Inc., Carson City, Nevada, USA


Near IR Continuous Wavelength Spectroscopy of Photon Emissions from Semiconductor


Devices........................................................................................................................................................... 311


W.B. Len, Y.Y. Liu, J.C.H. Phang, D.S.H. Chan, Centre for Integrated Circuit Failure  Analysis and Reliability (CICFAR), Faculty of Engineering, National University of


Singapore, Singapore


Defect Isolation and Characterization in Contacts by Using Primary Voltage Adjustment........................ 317


Y.-S. Chen, J.-H. Lee, Taiwan Semiconductor Manufacturing Company, Ltd., Taiwan


A Flexible, Low Cost Test System for Failure Analysis of High Power Mixed Signal ASICs...................... 320


T. Kolasa, J.C De La Torre, L. Bertram, Motorola SPS, Tempe, Arizona, USA


Photoemission and OBIRCH Analysis with Solid Immersion Lens (SIL) .................................................... 325


I. Arata, S. Sakamoto, Y. Yokoyama, H. Terada, Hamamatsu Photonics K.K., Hamamatsu, Shizuoka, Japan


Session 11: Circuit Edit for FA, FI and Debug


Voltage Contrast like Imaging of N-Wells ..................................................................................................... 331


C. Boit, K.R. Wirth, Technische Universität Berlin, Fakultät IV, Institut für Hochfrequenzund Halbleiter-Systemtechnologien, Berlin, Germany; E. Le Roy, NPTest, Inc., San Jose, California, USA


Improvements of Secondary Electron Imaging and Endpoint Detection in Focused Ion Beam


Circuit Modification........................................................................................................................................ 338


V. Ray, N. Antoniou, A. Krechmer, A. Saxonis, FEI Company, Peabody, Massachusetts, USA


Modeling Secondary Electron Emission from High Aspect Ratio Holes..................................................... 343


Q.S. Wang, M.A. Thompson, W. Schultz, T.R. Lundquist, NPTest, San Jose, California, USA


The Impact of Feature Packing Density on FIB Editing of Advanced Technology Ics................................ 348


H. Marchman, S. Herschbein, C. Scrudato, C. Rue, L. Fischer, IBM Corp., Hopewell  Junction, New York, USA; M. Abramo, IBM Corp., Essex Junction, Vermont, USA


Small Via High Aspect Ratio Circuit Edit: Challenges, Techniques and Developments............................. 355


V. Ray, N. Antoniou, R. Balasubramanian, N. Bassom, M. Clabby, T. Gannon, C. Huynh, G. Tiani, FEI Company, Peabody, Massachusetts, USA


Session 12: Die Level Fault Isolation


Improved SRAM 6T Bit Cell Failure Analysis Using MCSpice Bit Cell Defect Modeling............................. 363


R. Mulder, S. Subramanian, E. Widener, T. Chrastecky, Motorola Inc., Austin, Texas, USA


Laser Stimulation Applied to Dynamic IC Diagnostics ................................................................................ 371


F. Beaudoin, THALES Microelectronics, Toulouse, France; R. Desplats, P. Perdu,


CNES,Toulouse, France; A. Firiti, G. Haller, L. Dufayard, ST Microelectronics, Rousset, France; P. Vedagarbha, T. Lang, NPTest, San Jose, California, USA; D. Lewis, IXL,


Université Bordeaux, Talence, France


Speed Path Analysis: A Connection Between Speed Degradation, Silicon Dislocations, and Light


Induced Voltage Alteration ............................................................................................................................ 378


D. Davis, Texas Instruments Incorporated, Stafford, Texas, USA


Fault Localization of a Scan Shift Problem on Integrated Logic Designs ................................................... 384


C. Burmer, P. Egger, A. Huber, Infineon Technologies, Munich, Germany; H. Cerva,


Siemens, Munich, Germany; D. Petit, F. Grellner, ALTIS Semiconductor, Corbeil-Essonnes, France


Application of Scan Based FA and Advanced Passive Voltage Contrast Technique in Defect


Isolation.......................................................................................................................................................... 391


M.B. Schmidt, LSI Logic Gresham Campus, Gresham, Oregon, USA; N.J. Saujauddin, Silterra Malaysia, Kedah, Malaysia


Session 13: SPM Techniques


Quantitative Interpretation of Scanning Capacitance Microscope Images as Two-Dimensional


Dopant Profiles .............................................................................................................................................. 398


J.J. Kopanski, J.F. Marchiando, National Institute of Standards and Technology, Gaithersburg, Maryland, USA


Advanced Analysis of Thin and Ultrathin SiO2 Films and SiO2/Si Interfaces with Combined


Atomic Force Microscopy Methods. ............................................................................................................. 406


W. Frammelsberger, G. Benstetter, University of Applied Sciences Deggendorf,


Deggendorf, Germany; T. Schweinboeck, Infineon Technologies, Munich, Germany;  R. Stamp, J. Kiely, University of the West of England, Bristol, United Kingdom


Fault Localization in Contact Level by Using Conductive Atomic Force Microscopy................................ 413


J.C. Lee, J.H. Chuang, Taiwan Semiconductor Manufacturing Company, Ltd., Hsin-Chu, Taiwan


Characterization of Interconnect Defects Due to Electromigration Using Scanning Thermal


Microscopy..................................................................................................................................................... 419


E.X.W. Wu, X. Zheng, J.C.H. Phang, Center for Integrated Circuit Failure Analysis and


Reliability, National University of Singapore; L.J. Balk, Lehrstuhl für Elektronik, Bergische  Universität Wuppertal, Germany; J.R. Lloyd, IBM Thomas J. Watson Research Center, Yorktown Heights, New York, USA


Session 14: Optoelectronic Devices


Failure Analysis of Vertical Cavity Surface Emission Laser Diodes ........................................................... 426


F. Siegelin, C. Brillert, Infineon Technologies AG, Munich, Germany


Indium Tin Oxide (ITO) Film Removal Technique for Failure Analysis on Packaged


Optoelectronic Devices ................................................................................................................................. 431


S. Elliott, J. Gordon, P. Plourde, Fairchild Semiconductor, South Portland, Maine, USA


Session 15: Discretes, Passive


MIM Capacitor Reliability Fault Identification Using IR Microthermography and Automated Deprocessing: A Case Study............................................................................................................................. 437


J. Steele, T. Remmel, S. Wilson, M. Nair, P. Sanders, S. Kiefer, M. Sutton, W. Paulson,  S. Bigelow, D. Qualls, D. Gajewski, M. Martin, J. Walls, Motorola Semiconductor Products  Sector, Tempe, Arizona, USA


Magnetic Emission Mapping for Passive Integrated Components Characterisation.................................. 440


O. Crepel, Y. Bouttement, P. Descamps, C. Goupil, LaMIP Philips Semiconductors Caen; P. Perdu, R. Desplats, CNES Toulouse; F. Beaudoin, Thalès Toulouse; M. Guirardel,


LAAS-CNRS Toulouse


Session 16: Sample Preparation 2


Backside Imaging and AFM Profiling of Tunnel Oxide, Poly 1, ONO and Poly 2 Layers on Flash


Devices........................................................................................................................................................... 447


K. Upadhyaya, P. W. Blacker, Flash Products Group, Intel Corporation, Folsom, California, USA


Sample Preparation Techniques for Analysis and Debug of Circuits with Cu Inductors and Thick


Organic Dielectric .......................................................................................................................................... 452


M. Sutton, S. Kiefer, S. Wilson, M. Nair, P. Sanders, J. Steele, W. Paulson, Motorola   Semiconductor Products Sector, Tempe, Arizona, USA


Laser Interferometer Specimen Preparation of PCB Assembled Components at Second Level


Interconnect for In-plane Shear Strain Measurements................................................................................. 456


W.J. Cunningham, Intel Corporation, Hillsboro, Oregon, USA


A Novel Fault Isolation Technique for Identifying Deep Sub-Micron Defects ............................................. 465


F. Bundhoo, S. Kasivisvanatha, National Semiconductor Corp, Santa Clara, California, USA


Session 17: Yield Enhancement


Failure Analysis Case Study in 0.18µm Flash Memory Devices and Root Cause Identification ................ 471


W.-R. Chen, M.-S. Wu, C.-L. Chu, Quality Engineering Center, Macronix International Co., Ltd., Hsinchu, Taiwan


Characterization of Sub 130 Nanometer Gate Length SOI MOSFET Devices Exhibiting Short


Channel Effects.............................................................................................................................................. 478


T. Kane, M.P. Tenney, J. Bruley, IBM Microelectronics, Hopewell Junction, New York, USA


Session 18: Test 2


Mechanical and Electrical Characterization of an IC Bond Pad Stack Using a Novel In-Situ


Methodology .................................................................................................................................................. 486


C.D. Hartfield, Texas Instruments, Dallas, Texas, USA; J.J. Broz, Point Technologies, Inc., Boulder, Colorado, USA; T.M. Moore, Omniprobe Inc, Dallas, Texas, USA


A Multi-Stage Approach to Fault Identification Using Fault Tuples............................................................. 496


R. Desineni, T.J. Vogels, K.N. Dwarakanath, T. Zanon, R.D. Blanton, W. Maly, Center for  Silicon System Implementation, Pittsburgh, Pennsylvania, USA


Power Supply Noise Analysis Using Neural Network and Genetic Algorithm Based on Automatic


Test Equipment .............................................................................................................................................. 506


E. Liau, Infineon Technologies AG, MP Technology & Innovation, Munich, Germany;  D. Schmitt-Landsiedel, Technical University Munich, Institute of Technical Electronic, Munich, Germany


Chair:


# Session 1: Advanced Techniques 


Dave P. Vallett • IBM Microelectronics Division • Essex Junction, VT


Copyright © 2003 ASM International®


p 2-5


All rights reserved.


DOI: 10.1361/cp2003istfa002


www.asminternational.org Proceedings from the 29th International Symposium for Testing and Failure Analysis, 2-6 November, 2003, Santa Clara, California


## Scanning magnetoresistive microscopy for die-level sub-micron current density mapping


Scanning magnetoresistive microscopy for die-level sub-micron current density  mapping


B. D. Schrag, X. Y. Liu,  M. J. Carter, and Gang Xiao


Micro Magnetics Inc., Providence, RI


Abstract


In this paper, we will present a new technique for fault  isolation and failure analysis in integrated circuits based on a  scanning magnetoresistive imaging system.  By detecting the  stray magnetic fields at the surface of a chip using magnetic  sensors with sub-micron spatial resolution, we are able to  obtain a full map of in-plane current densities, resolving  features smaller than 100 nanometers.  We will briefly discuss  the capabilities and limitations of the technique and will  present results on a variety of frontside and backside samples.


Introduction


Magnetic imaging techniques have found numerous practical  applications in many areas of science and technology [1].  In  addition, recent advances in the emerging field of spintronics  have created new and powerful magnetic devices with the  potential to have a significant impact on both industry and  academia.  Sensors based on the giant magnetoresistance (GMR) effect, first discovered in 1987, have already become  the standard in the personal computer hard-disk drive (HDD) market, while an even newer type of sensor, the magnetic  tunnel junction (MTJ), discovered in the mid-1990s, has been  shown to have several significant advantages over GMR  technology.  We have built on these sensing technologies to  develop a new imaging tool for mapping current densities in  thin film conductors.  Our tool is non-invasive, operates under  ambient conditions, and is capable of spatial resolution better  than 100 nm.  In this paper, we will discuss the application of  this tool for the purposes of fault isolation and failure analysis  in integrated circuits.


Experimental Details


The basic operation of our system has been described  elsewhere [2] and will be briefly summarized here.  A  magnetic sensing element is raster scanned either in contact  with or at a fixed height above the sample.  The sample can be  driven using a wide variety of powering options.  The sensor  output is boosted using one of several preamplification circuits  built into the on-board electronics, and the amplified signal is


demodulated and sampled in real-time by a data acquisition  board.  Data is acquired in either a time-based or encoderbased manner, depending on the particulars of the scan.  After  the magnetic field map is acquired, we use a modified form of  an algorithm developed by Roth [3] to create a map of current  densities.


We use magnetoresistance-based sensors to measure the  vertical component of magnetic field at the surface.  Sensor  packages based on both magnetoresistive (MR) and magnetic  tunnel junction (MTJ) sensors are manufactured in-house.  The choice of sensor is dependent on the application. Our  sensors are designed for both front side and flip chip  applications.  More information about our  sensor design and  performance can be found elsewhere [4-5].


Results


Mouse bites in a quarter-micron-pitch conductor


We will illustrate the technique with a number of examples,  starting with simple test structures and continuing on to scans  of operational IC samples.  Figure 1 displays results taken on a  quarter-micron-pitch test structure.  The scan was made in  contact mode, with an estimated distance between the currentcarrying layer and the sensor of 200 nm.  Figure 1(a) shows  the raw magnetic field image above this sample, with large  positive (negative) magnetic fields represented by areas of red (blue).  Figure 1(b) maps the current density J (= √Jx2+Jy2) of  the same area plotted using the same color scheme.  This  sample was fabricated with a physical defect in one edge with  a width of one-half of the conductor pitch (125 nm).  The  resulting anomaly in current flow is easily seen in Fig 1(b), and a zoomed-in view of this area is shown in Fig 1(c).  We  also imaged an identical sample with a similar, yet smaller (63  nm) defect.  The presence of the smaller defect was readily  apparent from the field data, although its signature in the  current density maps was less striking than that of the defect  seen in Fig 1(b).


In order to detect very small perturbations in current density, such as those created by “mouse bites”, both the sensor  resolution (set by its active area) and the sensor-to-sample  distance z are critical;  as a rule of thumb, the larger of these  two values limits the resolution of the technique.  In this case,


5111m


0.5 μm


Figure 1: (a) False-color representation of the magnetic stray  field  above a quarter-micron-pitch patterned  conductor. (b) Calculated current density map of the same 10x10 µm area.


(c) Zoomed-in view of the current density near a 125 nm   mouse bite defect.


the intrinsic resolution in the primary scan direction is less  important than z, which is nearly as large as the defect size.  In  this case, we have found that for defects of size d, detection is  straightforward if the ratio z/d is smaller than ~3, while a  sufficient signal-to-noise ratio (SNR) and careful examination  allows detection of much smaller defects down to z/d ~ 6-10.


Localization of breakdown in a cross-point array


Figure 2(a) shows the CAD layout of a test structure for


2μm


investigating dielectric breakdown.  This sample consists of  two perpendicular arrays of metal fingers (width 1 µm, spacing 1 µm) separated by a thin layer of insulating material.  This cross-point architecture creates a two-dimensional array  of pixels at which the two metal layers overlap; this array is  seen in the lower right of the CAD image.  Under normal  conditions, this structure is non-conductive, but the sample  which was scanned showed a resistance of ~400 Ω, indicating  a probable breakdown of the dielectric layer.  Figure 2(b) shows the raw magnetic field map at the surface of this sample  as scanned using an MR sensing element.  In this case, the  field map immediately shows the nature of the failure, as the   magnetic field signature pinpoints a single defective pixel as  in (c).  The sample was powered at 300 µA RMS at 500 kHz  for this scan.


Current mapping in an operational logic chip


We have also imaged current densities in operating integrated  circuits.  Figure 3(a) shows an optical image of section of a


Figure 2:  (a) Above: CAD image of a cross-point test  structure.  (b) Middle:  Raw magnetic field image above the  sample provides the "smoking gun" by localizing the failed  pixel. (c) A zoom-in on the failed area localizes the exact  location of current transition between levels to within one  micron.


logic chip.  Figure 3(b) shows the current density map of this  same area which was reconstructed from the stray magnetic  field data.  This scan, taken with a magnetoresistive sensing  element in contact with the sample, covered an area of 9 mm2  with micron-scale resolution.


IC samples can be imaged in a number of other ways; for  example, by powering the chip normally while applying the  AC modulation to a pin other than the power pin, which will  allow visualization of the current flow only in a selected  section of the sample.  We have used this method to image  current through sets of pins whose electrical characteristics are


Figure 3:  (a) Above: optical image of a small section (~3x3  mm) of an operational logic chip and (b) Below: current  density map of the same area.


found to deviate from expected values.  In many cases, the  current distribution in a given sample may be very  complicated; therefore, the best way to diagnose a fault is  often to compare the current distribution of the failed device to  that of a known good chip.  Many chips have on-board  components which filter out high-frequency signals, so care  must be taken to choose a frequency which is low enough to  be admitted into the inner workings of the IC.  Alternatively, the sample can be powered in a way which circumvents such  elements.  Our sensors have an extremely wide operating  frequency range, from DC up to several GHz, which usually  allows the selection of an appropriate frequency.


Figure 4 shows the optical and current density images taken  on an operating SRAM sample powered at 2.5VDC with a AC  200 mVRMS voltage.  The current enters the sample at two  wire bond pads, seen to the left of the optical image.  To  obtain good results, it is often easiest to begin imaging by  scanning the area where current first enters the multilayer  structure, such as at a bond pad, and then to follow the current  throughout the chip, until it disperses or disappears into the


Figure 4:  (a) Zoomed-in optical image of an operating SRAM  sample.  The white box indicates the region of interest (with  the true aspect ratio). (b) Current density image of this ROI.  This map is presented with a skewed aspect ratio for clarity.


lower levels of the package.  In the sample shown in Figure 4, the current amplitude can be seen to slowly wane as it flows  toward the right edge of the image.  This indicates that the  current is leaking off through many of the active components  into the die, as opposed to shorting all at once through a single  location.


Figure 5:  Left: Magnetic field distribution of the full die of a  flip-chip sample.  The strong field signatures across the center  of the package are created by the introduction of power from  the package level to the chip itself.  Right:  Current density  image of a FIB-induced short at the lower right of the sample (the location of this area is indicated by the black box in the  first image).


Figure 6:  Field image and current density map of a flip-chip  test structure.  The current enters at a point in the package  near the top left of the image and then flows into a test  structure on the die, before exiting through another point at  the top right.  The horizontal lines on each image indicate the  boundary of the die.


Imaging of flip-chip samples and packages


We have also imaged samples in a flip-chip configuration.  The relatively large separation between the current-carrying  layers and the magnetic sensor (~100 µm) limits the spatial  resolution of the technique in comparison with front side  scanning.  However, for many types of failures, this reduced  resolution is sufficient to make a clear diagnosis of the  problem.  Figures 5 and 6 show results obtained on two such  samples.  These images were acquired using an MR sensor  fabricated in-house with a voltage sensitivity over twenty  times better than our magnetoresistive sensors.  This increase  in sensitivity allows for much faster scan rates and for the  detection of smaller current densities.  Figure 5 gives the  magnetic field profile of an SRAM chip with a FIB-induced  short.  The short appears as a faint field signature in the lower  right of the die in Figure 5(a), but is readily imaged with a  more detailed scan, as in Fig. 5(b).  This sample carries a 900 µA RMS AC current.  Figure 6, in comparison, displays the  current density profile of an entire flip-chip device and the  adjacent package area.  This sample carries a 700 µA RMS  AC current.  In Figure 6, the location of the current path can  be clearly traced through the entire chip, and can therefore be  compared with the chip layout to localize potential problems.


Conclusions and Future Work


We have demonstrated promising applications of a new  current-mapping technology based on miniaturized  spintronics-based magnetic sensors.  The high spatial  resolution of our sensors allows us to resolve features down to  50 nm.  For front-side applications, we can expect deep  submicron resolution in most cases, and the technique has the


1mm


advantages of operation at ambient conditions and noninvasiveness.


Acknowledgements


The authors wish to thank Wayne Ford, Mike McIntyre, Dave  Vallett, and Zhiyong Wang for samples and technical  assistance.  We also wish to thank Dave Vallett and Zhiyong  Wang for helpful discussions.


References


1. M. R. Freeman and B. C. Choi, Advances in magnetic  microscopy, Science, 294, 1484 (2001).


2. B. D. Schrag and Gang Xiao, Submicron electrical  current density imaging of embedded  microstructures, Appl. Phys. Lett., 82, 3272 (2003).


3. B. J. Roth, N. G. Sepulveda, and J. P. Wikswo, Jr., Using a magnetometer to image a two-dimensional  current distribution, J. Appl. Phys. 65, 361 (1989).


4. X. Y. Liu, C. Ren, and Gang Xiao, Magnetic tunnel  junction sensors with a hard-axis bias field, J. Appl. Phys. 92, 4722 (2002).


5. X. Y. Liu and Gang Xiao, Thermal annealing effects  on low-frequency noise and transfer behavior in  magnetic tunnel junction sensors, submitted to Appl. Phys. Lett. (2003).


p 6-8


DOI: 10.1361/cp2003istfa006


## High Resolution Current Imaging by Direct Magnetic Field Sensing


High  Resolution Current Imaging by Direct Magnetic Field Sensing


S.I. Woods, Nesco M. Lettsome, Jr., A.B. Cawthorne, L.A. Knauss


Neocera, Inc., Beltsville, Maryland, USA


R.H. Koch


IBM T.J. Watson Research Center, Yorktown Heights, New York, USA


Two types of magnetic microscopes have been investigated  for use in high resolution current mapping. The scanning  fiber/SQUID microscope uses a SQUID sensor coupled to a  nanoscale ferromagnetic probe, and the GMR microscope  employs a nanoscale giant magnetoresistive sensor. Initial  scans demonstrate that these microscopes can resolve current  lines less than 10 µm apart with edge resolution of 1 µm. These types of microscopes are compared with the  performance of a standard scanning SQUID microscope and  with each other with respect to spatial resolution and magnetic  sensitivity. Both microscopes show great promise for  identifying current defects in die level devices.


Scanning SQUID microscopy has proven that magnetic field  sensitive probes can be powerful tools for imaging current  flow in electronic devices [1,2]. Through its extraordinary  sensitivity to magnetic fields, the superconducting quantum  interference device (SQUID) can detect small currents even if  they are buried hundreds of microns below a sample surface. The spatial resolution of the scanning SQUID microscope (SSM), however, has historically been limited to lengths  greater than several microns as it is difficult to fabricate  functioning SQUIDs with dimensions smaller than this scale. In this paper, we present initial data on two types of magnetic  microscopes with the potential to image submicron magnetic  and current-carrying features: an SSM integrated with a  ferromagnetic fiber and a microscope employing a giant  magnetoresistance (GMR) sensor.


The idea behind the fiber SSM is to magnetically couple a  ferromagnetic wire with an etched tip to a SQUID. The tip, which can be etched to a radius of around 10 nm, is used as a  probe to deliver fine spatial resolution, the wire as a guide to  channel magnetic flux from sample to SQUID, and the  SQUID as a sensitive detector to measure disturbances from  the probe. With optimized transmission from tip to SQUID, high magnetic sensitivity and submicron resolution could be  obtained. This novel form of SSM is a hybrid device which  combines the strengths of scanning SQUID microscopy and  scanning probe microscopy. A number of research groups


have recently attempted to develop such a microscope, but  have not in general succeeded in demonstrating spatial  resolutions better than 100 microns in current carrying  samples [3, 4]. We show in this work that the fields produced  by current features smaller than the SQUID dimension can be  mapped by an appropriately designed SSM with flux-guide.


The GMR microscope depends upon a sensor which is  intrinsically less sensitive to magnetic fields than the SQUID, but is readily miniaturized to the nanoscale. These  magnetoresistance sensors are routinely fabricated with  dimensions perpendicular to the sensing direction of 30 nm by  200 nm. These devices are routinely used to sense submicron  bits in hard drives, and recent papers have demonstrated  magnetoresistive-sensor microscopes with submicron  resolution [5, 6]. If such a sensor can be brought within about  1 micron of currents to be measured, it has the magnetic  sensitivity to map out submicron current lines carrying about 1  mA or more of current.


Some details of these magnetic microscopes will be described  below and initial results on some simple test structures will be  presented. The expected capabilities of these microscopes in  magnetic sensitivity and spatial resolution will be discussed as  well as their relative advantages and disadvantages.


Microscope Design


Both microscopes share a common hardware base, built  around the existing structure of a Neocera Magma C10  scanning SQUID microscope. The fiber/SQUID microscope  uses a ferromagnetic metal probe 100 µm thick and 5-10 mm  long, electrochemically etched to a tip with submicron  diameter. This probe resides entirely in air, and its end is  attached to a window at the bottom of a cone housing a  SQUID. Figure 1 is a picture showing the region near the  probe, including the sample stage below and the SQUID cone  above. The SQUID sensor is isolated at around 77 K in  vacuum and the distance between the flux-guide and SQUID  can be adjusted to maximize the magnetic response of the  microscope. Measurements are made using the existing  SQUID electronics of the Magma microscope. An optical  shear force feedback method is used to scan the etched tip  over the sample in near-contact (separation distance of less


than 100 nm). Use of this feedback method means that  topography data can be acquired on the sample at the same  time as the magnetic data.


Figure 1: Picture of the flux-guide fiber attached to the SSM  vacuum cone.  The SQUID is located within the cone about  100 µm from the end of the fiber.


For the GMR microscope, we have tested a range of  commercial GMR read heads as potential scanning sensors. In  all cases, the GMR sensor has been attached to a cantilever  which allows the sensor to be scanned over the sample in soft  contact. The cantilever is attached to the SQUID microscope  housing by an easily mounted bracket.  In this way, the  sensitive SQUID can be used for large area scans to locate  regions of interest, and then the GMR sensor can be used to  perform high resolution scans in these regions. The sensors  were dc-biased at currents between 3 and 10 mA and readout  of the signal was made in the frequency range 1-10 kHz.


Scanning


Initial scans with both the fiber/SQUID and the GMR sensor


have been performed on small current structures with multiple


well-defined features. In the two sets of scans below, it is  demonstrated that current lines 10 µm apart can be welldistinguished. The “edge resolution” for these current lines is  about 1 µm, with significant gradients of magnetic field  measured across this distance. Figure 2a is an image of a


serpentine taken with the flux-guide SSM. The current lines  are 10 µm wide and 10 µm apart, and the peak-to-peak current  applied was 3 mA at around 10 kHz. Figure 2b is a fast  Fourier transform (FFT) current inverse [7] of the magnetic


field image, exhibiting the presence of 5 current lines about 10 µm wide each separated by 10 µm. Assuming reasonable  values for the size of the tip and height of the tip above the


surface, we find from this data a value for flux transmission  along the flux-guide fiber to be 10-4.


GMR microscope results are shown on a forked structure in  figure 3. A 10 µm current divides into two parallel current  paths 10 µm wide and 10 µm apart.  In figure 3a, the magnetic


field data was obtained in a scan where the peak-to-peak  current was 75 mA at a frequency of around 10 kHz.  Figure  3b shows a current inversion of the same region. In this scan, the distance from the sensor to the current lines was about 10 µm, requiring fairly high currents for quality imaging. From  this data, it appears that the magnetic response of the GMR  microscope during the scans was about 4 µV/G.


Figure 2: a) magnetic field image from the SSM with fluxguide of a serpentine of 10 µm current lines separated by 10 µm. b) current image of the serpentine calculated from the  magnetic field data.


Figure 3: a) magnetic field image from the GMR microscope  of a current fork with 10 µm current lines separated by 10 µm. b) current image of the fork calculated from the magnetic field


data.


A further scan with the GMR microscope shows that a  structure with 3 µm lines 2 µm apart can be well-resolved. In  figure 4a, magnetic field data was obtained in a scan with


peak-to-peak current of around 13 mA at a frequency of 10


kHz. Figure 4b shows the current inversion of this magnetic  data.  The linewidth of most of the visible lines is 3 µm in this  image.


Noise Data


In addition to scanning data, noise data was taken on the  SQUID and GMR sensors to help quantify what is the best  performance to be expected from them. Figure 5 shows noise  spectra for the SQUID and GMR sensors used, demonstrating  that the SQUID is four to five orders of magnitude more  sensitive than the GMR sensor over a wide frequency range.


Figure 4: a) magnetic field image from the GMR microscope


of a current structure with 3 µm current lines separated by as  little as 2 µm. b) current image of this structure calculated  from the magnetic field data.


This means that if the SQUID can image a 10 µA current line  with good signal to noise at a distance of 100 µm, the GMR  sensor will need to use 1 mA of current and approach closer


than 1 µm to achieve similar magnetic clarity. An unanswered  question, however, is what is the best flux transmission that


can be achieved over the length of the flux-guide. At this time, the flux transmission along 8 mm of wire is around 10-4, but


more work needs to be done to determine what the optimal  value can be.


1000


10000


1x10-11 1x10


Field Noise Density(Tesla)


-10 1x10-9 1x10-8 1x10-7 1x10-6 1x10-5 1x10-4 1x10-3


GMR Sensor


SQUID


Frequency (Hz)


:


Figure 5: Comparison of field noise from a GMR sensor and a  SQUID sensor of the types used for magnetic scans.  The field  sensitivity of the SQUID is about 5 orders of magnitude better.


Discussion


The potential spatial resolution of the fiber/SQUID  microscope and GMR microscope would appear to be  comparable. The fiber tip can be etched to about a 10 nm  radius, whereas the GMR sensor measures 10s of nanometers  by about 200 nm. It must be noted, however, that scanning in  contact with a sensor may make it difficult to deconvolve  surface topography from magnetic data. Using a feedback  mechanism allows one to separate topography from the bare  magnetic signal by scanning at different heights above the  surface.


Some primary advantages of the fiber/SQUID microscope  over the GMR microscope are the potential for higher


magnetic sensitivity by leveraging the superior sensitivity of


ab


the SQUID, the ability of the fiber geometry to probe cavities  and avoid wirebonds, and the use of height feedback to gather  separate surface topography data. The primary advantages of  the GMR microscope are that it utilizes a room temperature  probe which requires no cooling or vacuum space, and the  large commercial infrastructure for hard drive heads  guarantees these sensors will become smaller and more  sensitive with time. Although height feedback has some  advantages, moving in contact with a cantilever allows for  faster scans.


Conclusion


Our initial scans with a fiber/SQUID microscope and a GMR  microscope demonstrate that current lines separated by 10 µm  can be discerned with an edge resolution of about 1 µm. The  present limitation to demonstrating submicron resolution is the  need for appropriate samples with small features and less than  1 µm between the current lines and sample surface. Further  results will be presented once these samples are fabricated or  acquired. The flux-guide SSM and GMR microscope have  excellent potential as tools for locating die level defects and  could play a complementary role to standard SSM with a bare  SQUID. The standard SSM has unsurpassed current sensitivity  and the ability to examine circuits buried 100s of microns, but  is limited to applications where spatial features are larger than  a micron and for global imaging of current densities. The  microscopes described here have the potential to detect  submicron anomalies in magnetic fields created by current  defects, as long as the probe can be brought within 1 µm of the  current lines. These microscopes could be ideal for wafer level  studies or examination of deprocessed samples.


d ....tad ...


1.  L.A. Knauss, et al., Scanning SQUID Microscopy for  Current Imaging, Microelectronics Reliability, 41(8), 1211-29 (2001).


2.  David P. Vallett, Scanning SQUID microscopy for Fault  Isolation, ISTFA 2002, 391-396 (2002).


3. Y. Tavrin and M. Siegel, New type of HTS-SQUID  microscope for operation without shielding, Inst. Phys. Conf. Ser., No. 158, 719-722.


4.  Tatsuoki Nagaishi, Kenichi Minamimura, and Hideo  Itozaki, HTS SQUID Microscope Head with Sharp Permalloy  Rod for High Spatial Resolution, IEEE Trans. on Appl. Supercond., 11 (1), 226-229 (2001).


5.  S.Y. Yamamoto and S. Schultz, Scanning magnetoresistance microscopy (SMRM): Imaging with a MR Head, J. Appl. Phys., 81(8), 4696-4698 (1997).


6.  B.D. Schrag and Gang Xiao, Submicron electrical current  density imaging of embedded microstructures, Appl. Phys. Lett., 82(19), 3272-3274 (2003).


7. J.P. Wikswo, Jr. in SQUID Sensors:  Fundamentals, Fabrication and Applications (edited by Harold Weinstock), pp. 629-695, Kluwer Academic Publishers, Dordrecht, The  Netherlands (1996).


p 9-13


DOI: 10.1361/cp2003istfa009


## Fault Isolation of High Resistance Defects using Comparative Magnetic Field Imaging


Fault Isolation of High Resistance Defects using Comparative Magnetic Field Imaging


Antonio Orozco, Elena Talanova, Anders Gilbertson, and L.A. Knauss


Neocera, Inc., Belstville, MD, USA


Zhiyong Wang, Lars Skoglund, David G. Smith, and Rajen Dias


Intel Corp., Chandler, AZ, USA


As integrated circuit packages become more complicated, the  localization of defects becomes correspondingly more  difficult. One particularly difficult class of defects to localize  is high resistance (HR) defects. These defects include cracked  traces, delaminated vias, C4 non-wet defects, PTH cracks, and  any other package or interconnect structure that results in a  signal line resistance change that exceeds the specification of  the device. These defects can result in devices that do not run  at full speed, are not reliable in the field, or simply do not  work at all. The main approach for localizing these defects  today is time domain reflectometry (TDR) [1]. TDR sends a  short electrical pulse into the device and monitors the time to  receive reflections.  These reflections can correspond to  shorts, opens, bends in a wire, normal interfaces between  devices, or high resistance defects. Ultimately anything that  produces an electrical impedance change will produce a TDR  response. These signals are compared to a good part and  require time consuming layer-by-layer deprocessing and  comparison to a standard part.  When complete, the  localization is typically at best to within 200 microns.


A new approach to isolating high resistance defects has been  recently developed using current imaging. In recent years, current imaging through magnetic field detection has become  a main-stream approach for short localization in the package


[2] and is also heavily utilized for die level applications [3]. This core technology has been applied to the localization of  high resistance defects. This paper will describe the approach, and give examples of test samples as well as results from  actual yield failures.


The details of the physics behind the procedure will be  discussed seperately but we will try to give an intuitive  explanation of the detection procedure. Current imaging is  based on the measurement of the magnetic field generated by  current carried in the structures of the device under test (DUT).


The spatial magnetic field distribution B(r) is related to the  spatial current density distribution J(r) by Ampere’s law:


'3


'


)


(


3 dr


r


SIS


J


B


−


×


∝


This is a fundamental realtionship between the magnetic field  distribution and the current density.


Typically, a HR defect is the result of a geometrical change in  some circuit element such as a delamination process, crack, void, etc. Clearly, the current distribution will be affected by  such geometric alterations and correspondingly affect the  magnetic field distribution as sketched in Figure 1 for a failing  controlled-collapse chip connection (C4) bump.


Substrate


Die


Delamination


Good


Fail


Figure 1: Illustration of current distribution in a good and a  delaminated (failing) C4 bump.


In this situation, one expects to see a small change in the  magnetic field distribution around the defect as compared with  that in a good part. A detailed image comparison between the  good and failing parts would then be able to detect this  difference and subsequently locate the defect region. The  question now is how big is that magnetic anomaly and how  can it be detected.


To get some insight into these details, a simple 1 dimensional  model of a infinitely long wire of finite width was used. We  simulated  a mouse bite in the wire by changing the width of a  segment of the wire. The magnetic field was then computed  for a line scan of both the good and defective wires at some zdistance above them. This simple model presents the  advantage of having an analytical solution that allows us to


understand the behavior of the magnetic anomaly as we  change several critical parameters such as the defect size, zdistance, and noise level.


0.000012


defect size


0.00001


40-50


8x10-6


30-50 20-50


6x10-6


4x10-6


Figure 2: Maximum intensity of the magnetic anomaly in  Tesla (T) as a function of the z-distance for three different  defect sizes (the label shows the difference in width used to  simulate the defect, for example 20-50 means 30µm metal is  removed form a 50µm wide line).


The plot shown in Figure 2 summarizes these results.  The  maximum of the residual field (i.e., the strength of the  magnetic anomaly in Tesla) is plotted as a function of the zdistance (mm). The three different curves correspond to three  different defect sizes (large to small from top to bottom) and  the horizontal red dashed line represents a noise level (~ 20  nT) just as a reference to the eye. This residual field vanishes  gradually as we move away from the defect region.  It is clear  that the intensity of the residual field must be larger than the  noise level for the technique to be able to detect the defect. The need for a highly sensitive magnetic sensor such as the  SQUID is obvious.


When it comes to real 2D images, like the ones typically  obtained with the scanning SQUID microscope, we need  additional analysis tools to be able to extract the meaningful  information and disentangle it from other differences arising  from small experimental variations, etc. A comparative image  analysis (CIA) tool has been developed to compensate for  experimental and enviromental variances and extract the real  magnetic anomaly associated with the HR defect.


With the help of a finite element method simulation engine we  could extend our study  to real 3D structures and simulate 2D  images similar to the ones obtained with the SQUID  microscope. As an example, Figure 3 shows the resulting  magnetic anomaly after comparative imaging analysis for a  simple rectangular trace (black line) with a mouse bite in the  form of a rectangular cut (light blue box).


The magnetic field anomaly caused by the defect appears as a  gaussian-shaped peak (red region) and disapears gradually as  we move far from the defect (yellow/green region) finally  vanishing into the background noise as shown in figure 3.


Figure3: Simulated magnetic field image comparison result  for a 3D rectangular trace with a box cut-out.


A  variety of defect types including different sizes, geometries  and circuit elements (via, metal traces, PTH, etc.) and under  different scanning conditions (z-distance, current applied, etc.) were simulated. The results proved that in all cases we can  expect to see a distinctive magnetic anomaly (signature) with a   shape and intensity that depends on the defect geometry and  on the surrounding current elements. Without loss of  generality, we can expect to detect either a peak or a dipolelike magnetic feature.


Experimental


The localization of high resistance defects through current  imaging is accomplished through a detailed comparison of  good and failing parts. The differences in magnetic field  explained above are small and therefore require a very careful  analysis between the good and failing parts. This requires  improvements over conventional technology in two areas.  First, the instrumentation for current imaging requires more  precise automated control of the sample setup and data  acquisition.  The scan conditions must be as similar as  possible between the good and failing parts, so that an  effective comparison can be made.  Secondly, even with  careful sample setup and data acquisition, there will still be  misalignments between the two images, and potential signal  differences due to different working distances, or even part  deformations, for example warping.  These differences need to  be sorted out from the differences due to the high resistance  defect.  For this, advances have been made in comparative  image analysis to assist in the identification of failing defects.


2x10-6


z


0.020.04


0.08


0.12


Results on Test Structures


One of the difficulties encountered in developing this  approach was the availability of known defects. Typically  these defects cannot be known until layer-by-layer  deprocessing is complete, which ultimately destroys the  sample. To solve this problem, defects of different types were  fabricated via laser trimming to produce stable defects with  known locations.  Defects were created in vias, PTHs, and  metal line traces. 3D magnetic field simulations were also  calculated on these structures to help in understanding the  defect signature and verify that it was detected in actual scans.


Via Crack


A via structure in a long via chain was modified by laser to  have a horizontal cut in the middle of the structure.  The laser  system was then used to deposit a resistive bridge across the  via.  A picture of this can be found in Figure 4, where we can  see a top view of the surface of the package showing the laser  opening to expose the vertical structures and also a crosssection image showing the damaged via in more detail.


Figure 4: Package via chain exposed by laser and then laser  damaged for use in our scanning SQUID microscope HR  study.


To help us understand what to look for in the resulting image, a finite element simulation engine was used to calculate the  expected result using the 3D CAD design of this exact  structure. Then, the same CAD structure was modified to  introduce the cut and filling material as in the real case. For  both cases, the magnetic field was computed and compared. Figure 5 shows the CIA results from the good and failing parts  as determined by simulation.


The magnetic signature for this case can be clearly identified  as a pair of blue (dip or negative) and red (peak or positive) lobes (encircled in yellow) as shown in figure 5. The magnetic  centroid of this dipole-like feature corresponds to the location  of the defect.


Figure 5: CIA results corresponding to the simulated HR via  damage.


When scanning this part with the current imaging system, the  CIA for the good and failing parts produced the image in  Figure 6.


Figure 6: CIA results corresponding to the actual HR via  damaged part.


The real image agrees very well with the simulation in shape, and even with the tilt of the red and blue lobes (encircled in  black). The other features in the image are of lesser intensity  than the defect which allows the correct feature to be chosen  in this image.  The origin of these additional features is clear  from Figure 4; it was necessary to remove part of the package  to expose the vertical vias. A more extensive damage than that  on the via itself was induced in the part, and from that point of  view, part of the via chain was damaged. This damage can be  detected on the image as well.


Top view


Cross-section


Damage


Trace Crack


As a second example, a metal trace was edited in a similar  way. The trace was cut all the way through and a layer of  resistive material was deposited to reconnect the circuit, as  shown in Figure 7.


Figure 7: Picture of the HR metal trace damage.


Figure 8 shows the CIA results for this part showing the  magnetic anomaly (peak shape and location pointed by an  arrow).


Figure 8: CIA results corresponding to the HR metal trace  damage


.


Results on Real Yield Failures


The technique has demonstrated its capability to detect  specially fabricated defects.  Now, the final test is to apply it  to real yield failures with suspected HR defects in unknown  locations. The technique was applied to several different  failing parts. As an example, we will present here the results  for three different types of failures: a metal trace crack, a  suspected C4 bump failure, and a suspected via delamination.


Figure 9 shows the CIA results for the central portion of a  metal trace serpentine. The difference in resistance between a  passing and failing part was about 6 Ω (~17% increase). The  image suggests multiple damage spread over the serpentine  structure, visible in the image as multiple blue bumps aligning  on top of the serpentine’s turns. The large increase in  resistance observed is consistent with the presence of multiple  damage sites for this particular type of structure. Failure  Analysis (FA) deprocessing confirmed the results from CIA.


Figure 9: CIA results for a HR failing package metal trace  serpentine.


C4 Bump Failure


A second example is a C4 bump failure. Figure 10 shows the  region of interest from the CIA resulting image overlaid on  top of the CAD for the particular structure involved.


Figure 10: CIA results corresponding to the HR C4 bump  damage overlaid on top of the CAD.


The metal trace connecting to the failing bump is marked with  the dashed yellow line as shown in figure 10. The C4 bump is  connected at the end of it before the green grid. The centroid  for the magnetic anomaly is the black dot, aligning very well  with the position of the bump.


D


The density plot shown in Figure 10 does not present  adequately the relative intensity of the magnetic anomaly. A  better way of doing that is by using a 3D representation as in  Figure 11, where the z axis is the magnetic field intensity  corresponding to the CIA results in Figure 10. We plot the  absolute value of the magnetic field zoomed-in around the  anomaly location for the sake of clarity. The two peaks  associated with the defect are clearly visible. This result was  also verified by FA.


(a)


(b)


Figure 11:  (a) Zoomed-in magnetic field imaging showing  blue red lobes. (b) Zoomed-in 3D version of the CIA results  presented in Figure 10 and (a) .


Via Delamination


Finally, a suspected package via delamination failure was  investigated using the CIA technique. Figure 12 shows the  CIA results. The centroid of the magnetic anomaly (black  cross-hair) corresponds very accurately with the position of  the via. This result was also confirmed by FA.


Figure 12: CIA results for a via delamination problem. The  black cross-hair locates the centroid of the anomaly and thus, the defect location.


All of the above results demonstrate that this technique is  currently able to localize the defects to within 30 microns and  approaching 20 microns.


Comparative magnetic field imaging is a new non-contact and  nondestructive technique that has been demonstrated to  localize high resistance defects in package substrates and  interconnections. It has been shown to localize high resistance  defects to within 30 microns, which is an order of magnitude  improvement over TDR and without destruction of the sample. As this technique is further developed, we expect to be able to  apply it to more defect types and fully automate the analysis  process.


Acknowledgments


The authors would like to thank Diego Diaz and Arlene  Aguinaldo for providing real high resistance samples.


[1] D. T. Searls, D. Anura, E. Dy, and D. Goyal, Time  Domain Reflectometry as a Device Packaging Level  Failure Analysis and Failure Localization Tool, ISTFA  2000


[2] R. Dias, L Skoglund, Z. Wang, and D. Smith, Integration  of SQUID microscopy into FA flow, ISTFA 2001.


[3] D. Vallett, Scanning SQUID Microscopy for die level  fault isolation, ISTFA 2002


p 14-17


DOI: 10.1361/cp2003istfa014


## High Resolution Backside Thermography using a Numerical Aperture Increasing Lens


High Resolution Backside Thermography using a Numerical Aperture Increasing Lens


S. Thorne, S. Ippolito, M. Eraslan, B. Goldberg, M.S. Ünlü


Depts. of Physics and Electrical and Computer Engineering and the Photonics Center,  Boston University, Boston, MA, USA


Y. Leblebici


Swiss Federal Institute of Technology of Lausanne, Microelectronics and Microsystems Institute,   Lausanne, Switzerland


As the feature size in integrated circuits (ICs) become smaller, the techniques we use to localize defects must also progress to  the level that they can resolve potential errors. Additionally, because most errors cannot be identified by visual inspection  alone, it is necessary to develop techniques, such as  thermography, with the capability of localizing failures to the  specific component or defect at fault. This paper will review  the theory and application of an advanced subsurface (through  the substrate) analytical technique for IC failure analysis –solid immersion lens thermal emission microscopy.


Thermal microscopy has become one of the most useful and  powerful tools in IC failure analysis. Design and  manufacturing errors can cause short-circuits or other  component malfunctions that result in uneven heating, leading  to poor chip performance or even complete failure. Thus, the  goal of thermal microscopy is to localize a failure to the  specific faulty component.


Standard non-contact optical resolution is limited by  diffraction to about half the wavelength of light. This  limitation is particularly problematic when topside  metallization requires near-infrared (NIR) imaging through the  backside or substrate of the Si IC because Si absorbs  wavelengths shorter than about 1 µm. So while Si IC  technology has achieved process scales of 0.l3 µm, standard  subsurface imaging offers many times that, 3 – 5µm,  in lateral  spatial resolution. In addition, Si IC’s can consist of many  working layers, demanding longitudinal resolution capable of  localizing heat to a specific layer.


Thermal emission microscopy is a non-contact optical  microscopy technique that measures the spatial distribution of  temperature in a sample by collecting infrared photons emitted  by the sample. According to Stephan-Boltzmann’s law, optical  power emitted per unit area is proportional to the absolute  temperature of the sample to the fourth power. Thus, the  intensity of the collected light can be used to determine the  temperature of the sample. IC’s operating under normal  conditions emit mid-infrared photons, restricting the  diffraction limited spatial resolution to three microns and  greater. [1]


Clearly, the solution to creating a higher-resolution imaging  technique is to develop a microscopy system not confined by  the diffraction limit.  One way to do this is by using a solid  immersion lens.


Theory and experimental method


The solid immersion lens technique is based on using a  transparent (at the wavelength of interest) semi-spherical lens, or Numerical Aperture Increasing Lens (NAIL), where the  object space is either at the interface of the lens or embedded  within a similar material. The solids used are high index  materials (2.0 < n < 3.5). With the combination of λ/n  wavelength reduction and numerical aperture increase, diffraction limited resolution increases of greater than 10 (~n2) in the lateral direction and greater than 30 (~n3) in the  longitudinal direction have been demonstrated, together with  factors of 10 increase in light gathering ability. Recently, we  have implemented such a solid immersion microscopy  technique for subsurface imaging and have achieved lateral  resolution as small as 0.23µm. [2,3]


The NAIL is used in conjuction with a confocal microscope  shown in Figure 1. Scanning is accomplished by using a x, y, z  piezoelectric stage and is controlled by computer.


Figure 1:NAIL confocal scanning microscope.


The microscope is equipped with a mirror  to allow for  inspection as well as thermal scanning.  The mirror reflects the  near-infrared wavelengths to an InGaAs camera for visual  inspection. Mid-infrared wavelengths are transmitted to a  cooled 50 µm diameter Indium Antimonide detector for  thermal emission microscopy.


The thermal sample has an Al line and pads on a 1mm thick  undoped silicon substrate. To allow for subsurface imaging, the wafer is double side polished. The line is patterned to 1µm  wide, 0.1µm deep, and 20µm long and Joule heated to create a  lateral and longitudinal spatial distribution of temperature. This didtribution is of dimensions small enough to  demonstrate the approximate improvement in spatial  resolution of our system. However, to determine the exact  resolution limit of the system, the thermal distribution must be  exactly known. [4] To eliminate noise, a lockin detection  scheme is used; the sample is driven at approximately 900Hz. The second harmonic is detected, because power is a function  of voltage squared.  Finally, the sample is flip-chip mounted   to a standard printed circuit board and placed on the scanning  stage.


Directly over the line, the NAIL is placed on the backside of  the substrate.  The NAIL has a radius of curvature of 1.61mm  and a center thickness of 1.07mm, optimized for the sample  substrate thickness of 1mm. The mid-infrared achromatic  objective lens has NA = 0.25, giving in the NAIL microscope  a NA = 3.06, determined by the depth of the substrate and the  diameter of the lens. This represesnts a significant  improvement in the collected solid angle, allowing for  increased spatial resolution.


Results and Discussion


Improvement in inspection resolution and magnification are  shown in Figure 2.  A NAIL inspection image of the 1µm line  taken with the InGaAs camera is shown in Figure 3(a). Using  the InSb detector, the NAIL thermal emission image of the


same line’s Joule heating distribution is shown in Figure 3(b).


Figure 2: Inspection images using standard microscopy (a) and NAIL microscopy (b).  Shown are aluminum double lines  and electrical pads imaged using an InGaAs camera.


Figure 3: 1µm patterned Al line imaged using NAIL and (a) InGaAs inspection camera and (b) InSb detector of the  emission due to Joule heating.


These images are taken at best focus. The optical power  emitted due to Joule heating follows Stephan Boltzmann’s  Law, thus areas with more optical intensity have greater  temperatures.


In order to determine the lateral resolution of the NAIL  thermal emission microscope, we take a line cut of the thermal  emission image in Figure 3(b). The line cut is shown in Figure


4. The signal distribution is a convolution of finite spatial  distribution of the sample’s thermal emission and the line  spread function of the NAIL microscope. The full-width-athalf-maximum (FWHM) of the detector response is 1.6µm, giving a lateral resolution of at least 1.6µm. This is a  significant improvement over conventional thermal emission  microscopy.


Figure 4: Thermal emission  line cut of 1µm patterned Al line  using NAIL microscope. FWHM is 1.6µm, showing a  significant improvement over traditional thermal emission  microscopy.


20µm


In order to determine the longitudinal resolution, a step-wise  scan in z is taken. This is accomplished by determining how  the collected intensity from a thermal spot changes as the  system is defocused; shown in Figure 5. Again, the resolution  is a convolution of the spatial distribution of the sample’s  thermal emission and the line spread function of the  microscope.  The FWHM of the positive defocus values show  a longitudinal spatial resolution of 5.2µm.  Compared to the


Detector Response (V)000000


-0


traditional limit of 18µm, the NAIL gives a significant  improvement. The theorectical limit for longitudinal resolution  is determined by:


Longitudinal resolution = λo / (n sin2 θc)


where λo is the wavelength used, n is the refractive index of  the material, and θc is the maximum collected angle.


Figure 5: Spot intensity as a function of defocus distance. The  FWHM from positive defocus is 5.2µ.m.


Finally, in order to test the capabilities of the microscope  system, intensity collected from a thermal image was  measured with changing modulation frequency.  Figure 6  demonstrates that as frequency increases towards 10kHz there  is negligible increase in background noise, while the peak  thermal response falls only slightly, indicating that NAIL  thermal emission microscopy is a good candidate for varying  modulation frequencies and applications.


0 1 2 3 4 5


0


1000 2000 3000 4000 5000 6000 7000 8000


Modulation Frequency (Hz)


Maximum Response


Minimum Response


Figure 6: Detector response as a function of modulation  frequency. Maximum response is the largest collected thermal  intensity, while minimum response is the associated  background noise.


Conclusions


10


We have shown that with the application of NAIL


microscopy, the spatial resolution of subsurface thermal


emission microscopy can be improved to new record levels.


We have demonstrated lateral spatial resolution of better than


1.6µm and longitudinal resolution of 5.2µm. By increasing the  numerical aperture of the microscope, we have shown that it is


signal (V)


possible to improve resolutions beyond the diffraction limits.  NAIL technology has the potential to yield the same gains


when applied to other microscopy techniques as well.  We are


」


currently investigating methods by which shorter wavelengths


-10010


can be used to perform thermography, and thus spatial


defocus (um)


resolutions can be improved to the fabrication limits.


This project is sponsored by the National Science Foundation  under Award Number 0210752 (NIRT: Advanced


Characterization Techniques in Optics for Nanostructures).


We would also like to thank Tugba Demirci for help in design  and Philippe Flückiger and the entire staff at the Center of


Microtechnology at EPFL for help in the fabrication of test


samples.


1. J. Kolzer, E. Oesterschulze, and G. Deboy,  Thermal  Imaging and Measurement Techniques for Electronic  Materials and Devices, Microelectric Engineering, 31, 251-270 (1996)


2. S. Ippolito, B. Goldberg, and M.S. Ünlü, High  Spatial Resolution Subsurface Microscopy, Applied  Physics Letters, 78 (26), 4071-4073 (2001)


3. B. Goldberg, S. Ippolito, L. Novotny, Z. Liu, M.S. and Ünlü, Immersion lens microscopy of photonic  nanostructures and quantum dots, IEEE JSTQE, 8 (5),  1051-1059 (2002)


4. D. Cahill, W. Ford, K. Goodson, G. Mahan, A. Majumdar, H. Maris, R. Merlin, S. Phillpot, Nanoscale thermal transport, Journal of Applied  Physics, 93 (793), (2003)


Important addresses


Shawn Thorne


University of California, Berkeley


Hearst Memorial Mining Building


(510) 642 - 3956


E-mail:  sthorne@uclink.berkeley.edu


M. Selim Ünlü


Boston University


8 Saint Mary’s St.


Boston, MA 02215


Tel: (617) 353-1712


Fax: (617) 353-9917


E-mail: selim@bu.edu


R Aaron Falk • Optometrix, Inc. • Renton, WA


# Session 2: Optical Techniques


p 19-24


DOI: 10.1361/cp2003istfa019


## Study of Critical Factors Determining Latchup Sensitivity of ICs using Emission Microscopy


Study of Critical Factors Determining Latchup Sensitivity of ICs  using Emission Microscopy


Franco Stellari, Peilin Song, Moyra K. McManus and Alan J. Weger,


IBM T.J. Watson Research Center, Yorktown Heights, NY, USA


Robert J. Gauthier, Kiran V. Chatty, Mujahid Muhammad,


IBM Microelectronics, Essex Junction, VT, USA


and Pia Sanda


IBM Systems Group, Poughkeepsie, NY, USA


In this paper we discuss the use of Emission Microscopy (EMMI) to examine the events leading to latchup for various  Input/Output (I/O) pins of a test chip in order to study the  factors that impact latchup sensitivity of VLSI chips. The goal  of our study is to identify and characterize the structures that  are most prone to latchup in test chips, thus providing  countermeasures to be used to improve the overall latchup  resistance of commercial chips. As it has been shown in  literature [1-3], EMMI can be used to localize areas that are  latching up. Here we focus our attention on electrostatic  discharge (ESD) into I/O pins, which may lead to latchup  inside I/O circuits or in their proximity.


Latchup has been, and continues to be, a potential concern  for CMOS technologies. This issue has become more serious  with the reduction of transistor dimension and spacing. Although many techniques for avoiding the risk of latchup  have been developed in the past [4], they have often been  designed specifically for a particular technology. Therefore, an  in-depth evaluation of the structures most sensitive to latchup  ignition, as well as the understanding of the variety of possible


triggering mechanisms, is compulsory.


The latchup structure stems directly from the parasitic  bipolar transistors (npn and pnp), which are structurally  inherent to any bulk CMOS technology. Fig. 1 shows how  these transistors are connected to form a pnpn structure called a  Silicon-Controlled Rectifier (SCR). This structure is usually  inactive but can be turned on in various ways. If the SCR is  turned on, its positive gain feedback loop can cause a high  current to flow through a low resistance path that is formed  between VDD and ground. However, with proper process and  layout design, CMOS chips can be operated under relatively  harsh conditions without ever encountering latchup.


Prior literature [4-6] showed that there are two major  categories of latchup events depending on whether the trigger  is internal or external to the circuit. The former consists of  supply voltage or ground bounces, due to abrupt variation in  current consumption, and voltage spikes due to transmission  line reflections. The external causes are generally one of the  following: bad supply voltage regulation, radiation effects, such as x-rays and cosmic rays, and ESD at the I/O interfaces (cable discharge) with injection of majority/minority carriers  into the silicon substrate.


In this paper, we will investigate latchup that may occur in  the I/O circuits of the chip, as well as the logic circuitry in its  neighborhood, subject to electrostatic discharge due to external


p+


n+


RSX1V


RSX2


√


RNW1


RNW2


n-well


p- substrate


STI


IPIN古=口


h+


VDD


VDD丁


ESD diode


substrate contact


n-FET


p-FET


n-well contact


↓


inverter output inverter input


STI丁


RSX


VDD RNW立


IPIN


WW


npn47日 I pnp


Figure 1: (a) Cross-section of the parasitic bipolar transistors (npn and pnp) created in a standard CMOS process.


(b) The transistors are connected to form an SCR structure that can be turned on by majority carriers injected from an external source (Ipin), thus leading to latchup.


triggering sources (cable connection/disconnection). In this  case, current is injected to or withdrawn from the silicon  substrate by means of the ESD protection diode connected to  each I/O pin that is forward biased.


Latchup


All the pins of the particular 0.13µm bulk technology (1-2Ωcm p- wafer) were shown to be latchup resistant for positive  current injection (majority carriers). In this case, any p-type  diffusion connected to the I/O pad typically gets forward biased (see Fig. 1(a)): usually ESD p-type diodes and output driver pFETs. In either case, anytime a p-diffusion inside an n-well is  connected to an I/O pad, the p-diff/n-well junction (Fig. 1(a)) becomes the emitter/base junction of a horizontal or vertical  pnp transistor, while the substrate forms the collector terminal. As a result, holes are injected into the p-type substrate  increasing the local potential, and potentially leading to the  triggering of latchup. Large substrate contact rings around any  p-type diffusions inside each n-well connected to I/O pads are  effective in inhibiting the latchup induced by major carriers. This ensures a very low substrate resistance, i.e. the current  injected into the substrate is effectively collected by substrate  contacts before reaching n-type diffusions. Such a strategy can  easily be implemented during the design of a new I/O circuit  and therefore does not constitute a big challenge.


On the contrary, preventing latchup due to the injection of  minority carriers (electrons) into the substrate is much more  challenging and will be studied in detail in the experiments  presented in this paper. In this case, n-type diffusions  connected to the I/O pad become forward biased and inject  electrons into the p-type substrate (see Fig. 2(a)) which diffuse  until collected by n-type diffusions or recombined in the p-type  substrate itself. Unfortunately, the recombination length of  electrons in a 1-2Ω-cm p-type substrate is on the order of  20-30µm, and they can diffuse more than 500-600µm before  disappearing. If the electrons are collected by neighboring nwells in the logic, the local n-well potential may decrease  enough to allow the diffusion of holes within the n-well that is  connected to VDD, and latchup may occur.


Electrical and optical testing


JEDEC78 specifications [7] constitute the fundamental  standard for verifying latchup resistance of I/O circuits. Its  application is based on the injection of a fixed amount of  current through the pins under test in both pulsed or DC mode. The test current is chosen to be equal to two possible values: IDDQ+100mA or IDDQ-100mA, where IDDQ is the quiescence  current of the chip when it is not running. After the test signal  is removed from the pin, the current absorbed from the supply  voltage is monitored in order to check for an abrupt increase, which would point to a latchup event that occurred somewhere  in the chip (one or more SCR structures turned on and  conducted a lot of current from VDD to ground). Although the  previous method is very effective in verifying the chip  resistance to latchup, it does not provide the fine granularity for  locating the precise latchup area and identifying the triggering  mechanism, thus making it ineffective for this study of the  critical factors that determine the latchup resistance of a new  chip.


In this paper we present an innovative method based on a  slight modification of the JEDEC78 technique. While  complying with the previous latchup testing method (the  conclusions regarding the latchup sensitivity of each pin are the  same for both methods), it allows us to make an extensive use


RSX1


n-well p- substrate


IPIN1


▲VDD


n+STI


guard ring


eSTI


een-FET


一


口


RNW


=


npn


不


pnp


Figure 2: Some of the minority carriers (electrons) injected into the silicon substrate (Ipin) by the ESD protection diode(left hand side) may escape guard rings and trigger the ignition of a latchup process in the nearby logic.


CCD


5x


power supply


pin current


HTflip-chip


board


package


Figure 3: Schematic of the electrical and optical setup used for testing latchup onset.


of EMMI optical acquisitions in order to locate the latchup area  inside or outside the I/O pin being tested. During the test, both  the power supply compliance and the pin current can be varied  continuously with very fine steps, and acquisitions can be taken  at any desired bias.


Fig. 3 shows a schematic of the electrical and optical setup  used for the experimental measurements. The circuit under test  is flip-chip packaged on a Temporary Chip Attach (TCA) carrier, providing free access to the backside of the chip: the  optical inspection is performed through the silicon substrate  without risking obstruction of the light due to metal  interconnections. The power supply current is monitored with a  current meter, while each pin is stimulated with a variable  current source. The time-integrated images of latchup emission  are collected with an emission-based microscope using the  Hamamatsu C4880-21 back-illuminated CCD camera [8]. The  good quantum efficiency of the camera in the near-infrared  region of the spectrum, combined with the thinning of the chip  substrate down to about 100µm, allow an effective detection of  the latchup light emission due to electron-hole recombination.


With this enhanced technique, it is possible to study the  triggering of the parasitic SCR structure, as well as the  spreading of the latchup across different parts of the circuit. Both the test current injected into the I/O pin and the  compliance current of the power supply are precisely controlled  in order to monitor the different phases of latchup ignition (in  the structures that are more sensitive to latchup) and spreading (towards nearby or far away logic circuitry). Such an approach  permits one to avoid damaging the chip during the test because  of excessive power dissipation. If necessary, external cooling  can also be provided to the chip by blowing air under pressure  onto the silicon backside surface.


Fig. 4 shows an optical acquisition taken with the CCD  camera and overlaid to the layout of circuits in the  neighborhood of the I/O pin being tested. Several emission  areas are visible in the image, both inside and outside of the  perimeter of the I/O circuit. Inside the I/O, the emission comes  from three different structures that are also shown in the


schematic in Fig. 5: the ESD protection diode, which is  forward biased by the current withdrawn from the pin, the  ballast resistor of the output buffer and the four pull-down  transistors of the output buffer that are also conducting current. An intense emission is also seen to be coming from several  latchup regions just outside of the I/O perimeter: two small  neighboring areas below the I/O pin and one very extended  region on its right hand side. Such a latchup event is triggered  by minority carriers (current withdrawn from the pin), which  are not completely collected by the guard ring surrounding the  I/O circuit and diffuse towards logic circuitry in the  neighborhood, thus activating parasitic SCR structures.


As it will be discussed in the next sections, the shape and  extension of the latchup regions in Fig. 4 are introduced by the  particular distribution of n-well/substrate (NWSX) contacts, which absorb the electrons from the substrate, and of  decoupling capacitances, which do not participate in the  latchup. Moreover, among all the I/Os tested in this study, no  other bright spots were detected inside the I/O circuitry, thus  proving that the design and layout of the I/O circuits in this


0.13µm technology are fully latchup resistant.


Latchup spreading


Fig. 6 shows the case study of a different I/O: CCD images  were taken at different values of current compliance on the  power supply: the larger the current available, the larger the  area of spreading of the latchup. This observation appears to be  in contradiction with what was shown in previous literature [4,6]. In fact, one would have expected that nothing limits the  current in the parasitic SCRs, after they have been turned on, due to the positive gain of the feedback loop. Therefore, when  the current starts flowing, the gain of the loop increases  causing more current absorption from the power supply until  the chip is locally burnt out. In contrast, for the circuit under  test, the amount of current that each SCR structure can carry  tends to saturate. Therefore, the compliance value determines  the number of parasitic bipolar transistors involved in the  latchup, i.e. the extension of the latchup area. This  characteristic is extremely helpful for studying the onset and  identifying the structures that are most sensitive to latchup by  means of a quasi-static analysis of the events. Different


Figure 4: The optical emission is overlaid to the layout of the circuit. Light is seen coming from the ESD diode and ballast resistor inside the I/O circuitry, while emission from latchup is visible below and on the right hand side of the I/O pin.


Vdd


Ipin


pull down


ph


ph之K


BR


Figure 5: Schematic of the output buffer showing the two ESD protection diodes. High pin current can lead to emission from pull-down transistors and the ballast resistor (BR), aside from that coming from the ESD diode.


I/O circuitry


ballast resistor


latchup


ESD


pull-down


transistors 1


logic P circuitry


possibilities, such as the series resistance in the power grid or  reduction in the gain of the positive feedback loop of the SCR  due to high current level, are under consideration to fully  understand the observed phenomenon.


Fig. 6(a) is the image that corresponds to a pin current of  90mA (the power supply compliance is set to 200mA), which  is just below the threshold to trigger the latchup. Light  emission is emanating only from the ballast resistor and the  forward biased ESD protection diode inside the I/O circuitry. Once the pin current is increased to 100mA, a latchup event is  ignited in the circuitry just above the I/O circuit, as shown in  Fig. 6(b). By increasing the compliance current from (b) 200mA to (c) 300mA and (d) 400mA, the latchup spreads  progressively further from the I/O circuit. It is, however, interesting to observe that the latchup area appears to be  contained by the NWSX contact bar on the right hand side “A” and the decoupling capacitances on the left hand side. In fact, the former are an effective center of recombination for the  minority carriers that are injected into the silicon substrate and  that cause latchup ignition. On the other hand, decoupling  capacitances do not participate in the latchup because they do  not contain structures sensitive to latchup.


Latchup crossing decoupling capacitance


Fig. 7 shows a false-color image of the latchup for the same  I/O circuit at a higher compliance current (500mA). In this  condition, the latchup can actually cross the decoupling  capacitances and reach other regions of the logic circuitry on  the other side. In a real application, it is very difficult to keep  the compliance current very small and therefore this behavior  must be taken into account and studied further.


Fig. 8 provides a 3D map of the emission intensity due to the  latchup shown in Fig. 7 (note that bright emission coming from  the ESD protection diode saturated the CCD pixels in that  region). Since the light emission measured with the CCD is the  result of electron-hole recombination, it can be effectively used


to depict the density of minority carriers in the silicon  substrate, which corresponds to a certain recombination rate. Therefore, the amplitude and colors in Fig. 8 show that the  latchup emission is more intense in the region just above the  I/O circuit. Near the ESD diode, the contribution of the  electrons injected into the pin and escaping from the guard ring  is stronger. Moving further away from the I/O circuitry, the  emission reaches a constant intensity level due to the  uniformity of the circuitry involved in the latchup. However, the top part of Fig. 8 shows that the latchup can cross the  decoupling capacitances where the NWSX contact bar “B” ends. If we carefully look at Fig. 8, we can also see that the  minority carriers start diffusing underneath the decoupling  capacitances (see ellipse in Fig. 8) as soon as the NWSX bar  adjacent to the I/O circuit “C” ends. It must be noted that, even  though the capacitances cannot actively contribute to latchup  because they do not contain any parasitic SCR structures, they  do not obstruct the diffusion of carriers. The density of  electrons underneath the decoupling capacitances depends on  many factors such as the latchup intensity, the size of the


(c)


(d)


Figure 6: Sequence of time-integrated images of light emission overlaid to the circuit layout. From left to right, the power supply compliance current is progressively increased, causing the latchup area to grow in size.


Figure 7: False-color image of the emission acquired when latchup crosses the decoupling capacitances.


logic  circuitry


ballast  resistor


I/O


M 销货品 品面品品品decou capacitancespling


circuitry


NWSX  contacts


“A”


“B”


“C”


u


logic


Is"


A


Im


I/O O


e 0


alatchup


“B” P


15logic  circuitry


I/O  circuitry


a


张


b


n


是到易


apacitancesdecoupling c


plingnces capacitaoudec


logic  3月月自由


s


1


decoupling capacitances


“S1”


“S2”


decoupling capacitance (compared to the recombination length  of the minority carriers in the p-type substrate), and the  presence of NWSX contact bars.


Fig. 9 shows two cross-sections of the emission intensity for  the same I/O pin. If an NWSX contact bar exists on the left  hand side of the decoupling capacitance, the density of  minority carriers exponentially decays to the bulk equilibrium  value and, as a result, latchup cannot be triggered on the other  side. However, when such a protection is not in place (see the  top of Fig. 8), the electrons can cross the unprotected  decoupling capacitances. Two latchup peaks are then visible on  each side of the decoupling capacitances in the cross-section “S1” in Fig. 9. The density of electrons between the peaks, underneath the decoupling capacitances, remains also higher  than the equilibrium level. Once latchup is triggered on the left  hand side of the decoupling capacitances, it acts as a secondary  source of minority carriers, thus spreading the latchup towards  the left-bottom corner of Fig. 7.


Effect of NWSX contact distribution


During the experiments on the test chip, NWSX contacts  were confirmed to be very efficient in collecting electrons that  diffuse in the silicon substrate, thus providing an effective way  of preventing latchup from igniting and spreading (see Fig. 6). We also showed in the previous section that they must be used  to block the diffusion of minority carriers across decoupling  capacitances. However, it must be noted that their capability of  recombining electrons is limited: intense current injections let  latchup spread in areas protected by an insufficient density of  NWSX contacts.


Fig. 10 shows the study of another I/O pin. When 80mA is  withdrawn from the pin (see Fig. 10(a)), latchup is triggered in  the region directly above the ESD protection diode “R1” (also  visible in the image), due to its proximity to the source of  minority carrier injection. When the pin current is increased to  200mA, a second latchup region “R2” appears in the image (see Fig. 10(b)), “R1” and “R2” being separated by an NWSX  contact bar. Given the level of current injected into the pin, the  number of NWSX contacts used around the I/O circuit appears  insufficient to block all the minority carriers. On the left hand  side of “R1”, the NSWX contact bar is preventing latchup  spreading because fewer electrons can diffuse underneath the  decoupling capacitances without undergoing recombination.


Figure 8: 3D map of latchup emission acquired at 500mA of compliance current. The boxes show the positions of the decoupling capacitances.


0 10 20 30 40 50 60 70 80 90 100


0 30 60 90 120 150


Horizontal spatial position (µm)


"S1" "S2"


NWSX contacts


decoupling


"B"


"A"


Figure 9: Horizontal cross-section of the light emission extracted from Fig. 7: “S1” is taken where the latchup crosses the decoupling capacitances, while “S2” is taken in a region protected by the NWSX contacts.


Figure 10: Two configurations of latchup area are shown. Depending on the amount of pin current that is used, (a) a single latchup area can be triggered or (b) a second region of the circuit can be affected.


decoupling  capacitances


Emission intensity (a.u.)


ballast


ncesdecoupling capacita


resistor


“R2”


“R1”


capacitances


NWSX


“R1”decoupling capacitances


Fig. 11 shows a plot of the total current absorbed by the  circuit during the latchup test. The two abrupt increases of IDD, “jumps”, correspond to the ignition of latchup in region “R1” and “R2”, respectively. These types of electrical charts can be  obtained very quickly and they are very effective in identifying  the I/O pins that suffer from multiple latchup events. In all  cases, latchup ignites in a limited area isolated from the rest of  the circuit and then suddenly spread further when the NWSX  contacts are not able to contain the latchup.


Fig. 12 shows another example of inadequate density and  distribution of NWSX contact bars. A pin current of 400mA  was initially applied to the I/O circuit in order to trigger the  latchup in the surrounding circuitry. After the test, the  compliance current was kept at 1A, a value typical for the  circuit operation, while the pin current was removed. As a  result, only the latchup areas light up in Fig. 12. The 3D image  clearly shows that the latchup distributes equidistantly around  the NWSX contact bars in the region outside the I/O circuit (minimum energy state). The spreading of latchup towards  neighboring regions is simplified by the specific layout of the  NWSX contacts with many discontinuities in the vertical bars. In fact, the minority carriers can diffuse freely, and find wide  unprotected regions where the latchup can be self-sustained. A  higher density of NWSX contact with a “grid” layout was  demonstrated to be effective in preventing the spreading of  latchup in a newer generation of the test chip.


Application Setup


Measurements were made using an Optonics EmiScope-I system which has been described elsewhere [4-6].  One of the benefits of this system is the large opening of the chamber area of the light-tight box.  As with most diagnostic systems designed to mate with ATE, the column is attached to a large vibration isolated table.  The EmiScope-I, however, is designed such that a significant portion of the table-top can be customized and used as a customer or design-specific insert.


This, coupled with the ability of the z-stage to move the final optics above the tabletop, easily allows for the design of fixturing capable of suspending a PC motherboard or peripheral card in place above the chamber opening.  In our case, we have designed a dual level bracketing fixture which holds the PC motherboard as well as the product graphics card in a stacked parallel configuration.  As shown in Figure 1, we are able to stack the PCBs by using right-angle extension for the AGP bus.  We were also able to setup alignment pins on the fixture.  This allows repeated place/remove/replace steps that kept the DUT in the same general location which reduced the realignment procedures after a device change or fixture modification.  The same alignment pins were also used for any ATE load board configuration to again assist in the consistent critical alignment setup.  The ability to have the DUT PCB above the surface of the tester enabled connectors to external devices such as monitors and sensors.


Measurements


As with most dynamic diagnostic techniques, the timing measurements are sampled relative to a reference trigger which is synchronous to the DUT activity.  Providing such a trigger is usually not a challenge when using ATE or an analogous stimulus source since the trigger can easily be generated within the test program and is naturally synchronous to the master clock and to activity within the DUT.  The challenge arises when there is no longer direct control over the test program as is often the case for PC based testing.  In order


to meet this requirement we made use of an external stimulus source with circuitry designed to establish a phase-locked loop with an external signal (Tektronix HFS 9003 Programmable Stimulus Source).  The HFS 9003 was then phase-locked to an on-card clock synchronous to the internal DUT clock.  Finally,the reference trigger signal was programmed and generated from this external source.  One of the benefits in using the Optonics EmiScope-I was the minimal set of timing constraints required.  As with e-beam testers, the EmiScope-I only required a trigger signal indicating the start of the test loop.  If, however, LVP was to be used, there would be the added requirement of a highly accurate, synchronous clock input to the diagnostic system.


Device Preparation and Cooling


In order to perform optical probing through the silicon substrate it is necessary to thin the substrate to approximately 00 um.  Additionally, obstructions must be removed in order to facilitate optical device access.  The removal of the silicon thermal mass and external heatsink generally forces the limiting of the speed at which the DUT is stimulated to avoid overheating the device.  In order to overcome these issues we have progressively improved our thermal control techniques by introducing the novel use of a Peltier cooler attached to the backside of the peripheral card PCB using thermally conductive epoxy or thermal pad.  Each generation of thermal control has enabled device operation at a higher data rate.  The latest implementation utilizes the peltier system supplied by Silicon Thermal. (See Figure 2)  These systems vary in power from 60 Watts to 120 Watts of cooling power and use either a fan or a water heat pump to remove the excessive heat generated with this technique.  Use of the fan cooling system caused additional vibration which cannot be tolerated in the submicron probing required.  Moving to the water circulating closed loop system resulted in minimal vibration and maximum heat removal.  The resulting chip temperature went from 105-135 degrees C to a manageable 34 degrees C running at maximum frequency and power (about 35 Watts in this case).


Using the techniques outlined in this abstract we have succeeded in using dynamic emission analysis for in-situ first silicon and prototype design debug and failure analysis of 0.13 um advanced process graphic processors.  Sample data showing n- and p-channel acquisitions is shown in Figure 5.


This data was acquired using a test loop length greater than 50 us and a power supply voltage of 1.3 volts.  The n-channel acquisition was approximately 5 minutes.


We have shown capability to do in-situ probing using time resolved emission.  The results presented demonstrate the ability for dynamic emission analysis for PC-based probing,and also show the ability to obtain high bandwidth, low jitter measurements at reasonable acquisition times using test conditions typical of application-based testing.


[1]


J. C. Tsang, J. A. Kash, and D. P. Vallett,"Optical tools for measuring timing and switching in silicon ICs: Status and future challenges," in IEEE Industrial Research Highlights, vol. 2001: IEEE, 2001.


[2]


J. A. Kash and J. C. Tsang, "Dynamic Internal Testing of CMOS Circuits Using Hot


Luminescence," IEEE Electron Device Letters,vol. 18, pp. 330-332, 1997.


[3]


S. Kasapi, C.-C. Tsao, K. Wilsher, W. Lo, and S.


Somani, "Laser Beam Backside Probing of


CMOS Integrated Circuits," Microelectronics


Reliability, vol. 39, pp. 957-61, 1999.


[4]


J. Vickers, N. Pakdaman, and S. Kasapi,


"Prospects of Time-Resolved Photon Emission as a Debug Tool," presented at ISTFA, Phoenix,AZ, 2002.


[5]


E. B. Varner, C.-L. K. Young, H. M. P. Ng, S. P.


Maher, and T. M. Eiles, "Single Element Time


Resolved Emission Probing for Practical


Microprocessor Diagnostic Applications,"


presented at 28th International Symposium for


Testing and Failure Analysis, Phoenix, AZ,


2002.


[6]


E. B. Dan Bodoh, Kris Dickson, Ron Wang,


Tim Cheng and J. V. Nader Pakdaman, Dan


Cotton, and Birk Lee, "Defect Localization


Using Time-Resolved Photon Emission on SOI Devices that Fail Scan Tests," presented at


International Symposium on Testing and Failure Analysis, Phoenix, AZ, 2002.


MOTHERBOARD


AGP SLOT


-STAINDOFF


P/N 20-100407-00


Liquid Coolingof Peltier


Table Top


-FRAME


ALIGNMENT PIN P/N 20-100406-00


P/N 20-100406-0


Objective Lens


-DUT


MOUNTED ON GRAPHICS CARD 4X


Figure 1 Motherboard Fixture


BOSNGU JTING CWALLERBMOLS OTMTE


Figure 2  Silicon Thermal Cooling System


Figure 3  PC Frame holding AGP Graphics card to Motherboard


Time/dac Bms


Bin with 19 5313 pe


poedichow


AM


cur204z10mhz


5 ns/ div


Figure 4  Acquisition Waveforms


p 40-44


DOI: 10.1361/cp2003istfa040


## Time-Resolved Optical Measurements from 0.13µm CMOS Technology Microprocessor using a Superconducting Single- Photon Detector


Time-Resolved Optical Measurements from 0.13µm CMOS Technology   Microprocessor using a Superconducting Single-Photon Detector


Franco Stellari, Peilin Song, Alan J. Weger and Moyra K. McManus


In this paper we examine the use of the Superconducting  Single-Photon Detector (SSPD) [1] for extracting electrical  waveforms on an IBM microprocessor fabricated in a 0.13µm  technology with 1.2V nominal supply voltage. Although the  detector used in our experiments is prototype version of the one  discussed in [1] demonstrating lower performance, we will  show that it provides a significant reduction in acquisition time  for the collection of optical waveforms, thus maintaining the  usability of the PICA technique for present and future low  voltage technologies.


The Picosecond Imaging Circuit Analysis (PICA) technique


[2], based on the collection of near infrared light (NIR) emitted  by hot-carriers in the transistor channel, has been demonstrated  to be an invaluable method for detecting timing-related faults  in backside packaged ULSI circuits [2]. Many innovative  applications of the PICA technique have been developed in the  past years, based on the detection of light emission due to offstate leakage current [3], oxide tunneling current and carrier  recombination [4], thus leading to completely new application  areas and even more contributions to quick turn around times  for circuit debugging and defect isolation. However, the  continuous trend of the modern semiconductor industry  towards smaller devices and lower supply voltages [5] is  causing significant changes in the intensity and spectrum of the  light emitted by present generation ICs: the total detectable  light decreases exponentially with the electrical field in the  transistor, and linearly with the lateral dimension of the FET. In particular, the progressive shift of the spectral distribution of  the emitted light towards longer wavelengths [6] makes the use  of the conventional PICA technique based on the use of the  Mepsicron detector [7] more challenging, due to its lack of  sensitivity in the NIR region of the spectrum.


Need for innovative NIR detectors


Due to the importance and advantages offered by the PICA  technique over other testing methods, which are often invasive  and may lead to damage of the circuit under test, a significant  amount of effort has been devoted in recent years to the


development of innovative detectors. Two that demonstrated  significantly better quantum efficiency (QE) in the NIR region  of the spectrum are the SSPD [1] and the InGaAs Avalanche  Photo-Diode (APD) [8]. Unfortunately, all these detectors offer  only single-point detection capability as opposed to the  imaging capability of the Mepsicron PMT. The latter permits  the parallel acquisition of waveforms from hundreds of  transistors in the same field of view. Nevertheless the new  detectors are suitable for effective use in PICA systems due to  their much faster acquisition times, while intense work is  carried out on the development of an imaging detector with  extended NIR sensitivity.


In this paper, the SSPD is used to test an IBM  microprocessor fabricated in a 0.13µm technology with 1.2V  nominal supply voltage. The measurements were taken with a  prototype of the detector discussed in [1]. The System  Detection Efficiency (SDE) of the prototype is about ~0.02% at


1.3µm-wavelength, compared to >4% for the commercially  available version of the tool, which has a 10µm×10µm detector  area. The upgraded detector permitted an acquisition over 200  times faster than that possible with the prototype on the same  system. Fig. 1 shows the system detection efficiency of several  detectors. Compared to the Mepsicron PMT used in the


0.8


1.0


1.2


1.4


1.6


0.01 System detection efficiency [%]0.11100


Wavelength, λ [µm]


InGaAs APD


commerical SSPD


S-25


SSPD prototype


emission spectrum


Figure 1: Comparative chart of the system detection efficiency of Mepsicron PMT ( ) [7], SSPD prototype ( ),commercially available SSPD ( ) [1], and InGaAs APD ( ) [8]. An emission spectrum [6] is also shown in the image as a reference.


original PICA systems, which has negligible sensitivity beyond


1.1µm, the SSPD has a very slowly decaying efficiency that  extends well in the NIR region of the emission spectrum, thus  allowing the detection of the low-energy photons that are not  absorbed by the silicon substrate. The dashed line in Fig. 1 is  the ideal quantum efficiency of the detector without the optical  band-pass filter that is added in front of the detector to block  ambient light and thermal photons, which do not correspond to  switching transitions of the IC being tested. The performance  of the SSPD detector (in terms of SDE, Dark Count Rate (DCR) and jitter) can be tuned by means of the bias current of  the NbN meander [1] depending on the application. The  prototype detector is fabricated with a 10nm-thick stripe line  bent in a serpentine shape (meander) of 4µm×4µm, and it is  characterized by a lower DCR (due to the area factor) and a  higher critical current to maintain the superconductive state. The latter guarantees a larger amplitude of the electrical signal  detected from the front-end electronics and therefore a slightly  better time resolution during optical waveform reconstruction. The best SDE of the novel detector can be achieved at a bias  current that results in a 1000cps DCR. However, DCR can be  reduced more than one order of magnitude by decreasing the  bias current of the detector with a very small loss of SDE (~10% variation). At low count rates, corresponding to  emission from a p-FET transistor, the noise is dominated by the  detector DCR and therefore the reduction in the DCR results in  more than a factor 3 improvement in the SNR of the optical  measurements.


Challenges to improve optical tools


Optical testing of future generations of microprocessors is  also raising new challenges besides the photodetector  improvement: higher optical magnification lenses with high  numerical aperture (NA) are required for the identification of  individual transistors; effective cooling systems allowing the  concurrent luminescence acquisition need to be developed; new  design for test (DFT) features aimed at the use of emission tool  testing need to be investigated and implemented on-chip.


Nowadays several types of lenses are being developed and  tested, such as the Solid Immersion Lens (SIL) [9] shown in  Fig. 2. This type of lens combined with specific aberration  corrected objectives provides a very high NA (>2): the higher  the NA, the better the emission collection efficiency. Although  experimental tests look very promising, integration with  cooling systems is still a concern and must be fully


demonstrated in a real life application. Present microprocessor  chips can easily consume more than 100W of power during  normal operation [10], due to both dynamic power and  increasing leakage current contribution. Such a power must be  managed by innovative cooling systems that allow the  detection of the light from the backside of the chip, i.e. no  conventional heat sink is permitted.


In general, before time-resolved emission tools can be used  to measure on-chip electrical waveforms, the fault location  must be roughly known. Repetitive patterns that exercise the  failing sub-circuit are required for Time-Correlated SinglePhoton Counting (TCSPC) measurements of the very faint  luminescence emitted by the transistors. This requires that the  chip under test have some DFT features that help us isolate the  suspect circuit. Scan design, logic built-in self-test (LBIST), and array built-in self-test (ABIST) are commonly used [11] to  drastically reduce the time required to isolate the failing subcircuit and also to improve the circuit testability.


Testing setup


Fig. 3 shows the schematic of the electrical and optical setup  used during the test of the microprocessor. The circuit under  test is packaged using a Temporary Chip Attach (TCA) socket  mounted on a test board that provides supply voltage and  ground, as well as access to the I/O pins that are required to run  the test. In order to collect hot-carrier NIR emission, the TCA  package must be opened, the silicon substrate thinned down to  about 100µm and polished for backside analysis. An IMS  tester, scanning in the bit pattern, is used to initialize the chip  state and operation; an HP8133A pulse generator is used to  provide the reference clock to the chip and the trigger signal for  the PICA technique [2]. The board is mounted upside-down  over a Laser Scanning Microscope (LSM) that can image the  circuit for navigation, as well as collect the emission and focus


Solid Immersion


Lens


Emission source


Silicon


substrate


NA=tanθ


Figure 2: Silicon Immersion Lens (SIL).


LSM


PMT


SSPD


3-position mirror


lens


optical coupling


circuit under test


temporary chip attachment


test board


optical fiber


power suppy


IMS tester


light tight enclosure


Figure 3: Schematic of the electro-optical setup used for testing the microprocessor: the board with the chip is mounted upside-down on the LSM. A 3-position mirror focuses the emission onto the Mepsicron PMT, or into the optical fiber connected to the SSPD.


it onto the Mepsicron PMT or into the optical fiber that is  connected to the SSPD (see Fig. 3), housed in a cryostat.


Before taking PICA measurements, extensive work was  performed by means of the ABIST engine in order to isolate  the area of interest. Moreover, thanks to the high scannability  of the chip, the circuit operation was reprogrammed in order to


countsPhoton


repeat the failing condition every few clock cycles, thus  permitting a testing loop of 128ns (or less) during the optical  acquisitions. Such short loop duration is especially important  for Mepsciron acquisitions that require the observation of an  elevated number of switching transitions in order to detect  photon events.


0 n


Detector comparison


U


Fig. 4 shows a 60-minute time-integrated image of the d山 luminescence taken with the Mepsicron PMT. The emission


was overlaid on the LSM image of the circuit where the bright


spots, in false color, represent the gates emitting light. This


preliminary acquisition from the area of interest is very useful


in order to localize possible candidates that we want to analyze


by means of the SSPD single-point detector. This procedure


can, in fact, significantly reduce the total number of


measurements necessary for isolating faults. However, in order


to use the Mepsicron PMT and keep the acquisition time short,


the supply voltage had to be raised to 1.8V, which will not


represent the real failing condition.


Fig. 5(a) shows the time-dependent optical waveform


contained in the Mepsicron data set. The signal was extracted


from the local clock buffer of the chip (see the circle in Fig. 4)


and each peak corresponds to the falling edge of the switching


transitions, as in the conventional PICA technique. The delay


between consecutive peaks is 2ns and corresponds to the clock


period. The imaging capability of the Mepsicron permits the


parallel acquisition of optical signals from all the transistors in  the field of view during the same measurement. Such an  advantage makes it easy to compare different waveforms for  extracting delays and skews, and allows the concurrent  evaluation of different hypotheses regarding possible causes of  the failure. Moreover if multiple devices in the field of view are  fired at the same time, their optical waveforms can be easily  summed up (in phase), thus significantly improving the SNR. Recently, a technique based on correlation of photon arrival  time and position was developed in order to improve SNR of  Mepsicron acquisitions and keep acquisition time short [12]. The Spatial Temporal Photon Correlation approach (STPC-3D) classifies all detected photons as either noise (to be discarded)


素族


or as signals (to be kept). The technique permits a significant  improvement of the SNR of the time-integrated image of the  emission, which allows emission sites to be more easily  identified, and as a result the acquisition time is cut down from  hours to minutes.


Fig. 5(b) shows a 2s SSPD acquisition of the same clock  driver working in the same operating conditions (note that the  SSPD does not require the chip to run at 1.8V, the acquisition  was taken at this voltage for easy comparison to the  Mepsicron). One immediately notices that the amplitude of the  signal is fairly similar to the Mepsicron measurement shown in  Fig. 5(a), in spite of the 1800 times shorter acquisition time  used for the SSPD measurement. Fig. 5(b) also shows that the  peaks are much better defined, due to the factor-two  improvement in SNR that is guaranteed by the detector.


Detector performances for low-voltage acquisitions


The much higher collection efficiency of the SSPD allows  optical acquisition to be taken at low supply voltages, below


4


Figure 4: 60-minute Mepsicron acquisition of the hotcarrier luminescence from a 0.13µm technology chip at 100x magnification. The time-integrated emission is overlaid to the LSM image of the chip. The bright spots identify the switching gates, and the circle highlights the local clock driver used to compare the Mepsicron to the SSPD.


0 2 4 6 8 10 12 14 16 18 20 22 24 26 28 30 32


0.0


0.1


0.2


0.3


0.00


80.05 0


00.10 s0.15


0.20


Time [ns]


Figure 5: Measurement of the optical waveforms from a local clock driver of the chip running at 500MHz and


1.8V with: (a) Mepsicron PMT (1 hour) and (b) SSPD (2 seconds).


clock driver  local clock buffer


the nominal value for circuit operation (1.2V). Fig. 6 shows  that measurements at 1V supply voltage can be effectively  taken. An excellent SNR can be achieved with just a 30  minutes acquisition at such a low voltage (in Fig. 6 we kept the  500MHz frequency to simplify the comparison with the  previous Mepsicron acquisition). By increasing the clock  frequency to the normal operation of 2GHz, a significant  reduction in acquisition time is easily achieved as well.


Fig. 7 shows real-life acquisitions (10-minutes of duration) of two optical waveforms from two different inverters of the  chip under test. The supply voltage is set to the nominal value  of 1.2V; the chip is set to run at 1.6GHz. The loop cycle is  64ns while a 50ps low pass filter has been applied to the data  shown in Fig. 7. The low jitter of the system (detector and  front-end electronics) in evaluating the photon arrival time  allows an accurate estimation of the baricentrum of each  switching transition. Based on the formulas after Lo et al. [13], it is possible to estimate a time resolution better than 20ps with  1-minute acquisition time or better than 10ps if the  measurement time is increased to 5-minute.


Fig. 7 shows also that the optical waveforms are in very good  agreement with electrical simulations of the circuit, thus  verifying the accuracy of transistor models and parasitic  capacitance estimations. Due to the extended sensitivity of the


detector in the NIR region of the emission spectrum, the SSPD  is also effective in detecting transition due to p-FETs. This  capability greatly simplifies the evaluation of pulse durations  and propagation delays between falling and rising edge of  different signals.


Extensive tests of the repeatability of acquisitions over a few  days were also performed. The results showed that over many  hours, there is less than 2.5ps-rms of jitter among waveforms  from different acquisitions taken in the same region of the chip.


Fig. 8 shows that a time resolution of about 50ps-FWHM (Full Width at Half Maximum) can be achieved by measuring  the switching transition of a minimum size inverter. During the  measurement, the chip was running at its nominal voltage of


1.2V and the on-chip PLL was bypassed in order to exclude its  jitter from the measurement.


In this paper we have shown that the SSPD can be effectively  used for testing the electrical signals inside a state of the art


0.13µ IBM microprocessor working at the nominal supply  voltage of 1.2V or below. About 2000 times improvement is  demonstrated for the prototype SSPD in comparison with the  Mepsicron PMT. Various optical waveforms were acquired and  compared with the circuit working at its nominal conditions. A  record FWHM of about 50ps was also demonstrated by using  the prototype detector. The performance demonstrated to date  extends the applicability of the PICA technique to present and  future technology with lower VDD and faster transition times.


The authors wish to thank Steve Wilson and Phil Wu, of  IBM Server Division, for graciously providing the  microprocessor chips used in the presented measurements, and  for support during the preparation of the test board and  electrical setup.


0.4


0.6


Figure 6: The high quantum efficiency of the SSPD prototype allows acquisitions (30 minutes in this case) to be taken at supply voltages as low as 1V, below the nominal operating condition of 1.2V.


17.8


17.9


18.0


18.1


~


-


-18.2


18.3


18.4


0 1 2 3


y


o


d4


5


Figure 7: SSPD acquisition of the optical waveforms coming from the circuit under test running at the nominal voltage of 1.2V. The extended sensitivity of the detector in the NIR range of the spectrum allows the observation of both n- and p-FETs.


20


40


60


80


100


120


140


160


1 3 5


t


7 9 11


Time [ps]


50ps-FWHM


Figure 8: A 50ps-FWHM resolution was demonstrated by measuring a minimum size transistor (dashed line is a gaussian fitting of experimental data). The chip is running at 1.2V while the clock is externally proved.


T im e [ns ]


1 55ps


66ps


[1] W.K. Lo, et al., “Next-Generation Optical Probing Tools  for Design Debug of High Speed Integrated Circuits”, ISTFA, vol. 28, 2002, pp. 753-762.


[2] P. Song, et al., "Diagnostic techniques for the IBM S/390  600MHz G5 microprocessor", ITC, 1999, pp. 1073-1082.


[3] S. Polonsky, A. Weger and M.K. McManus, “Picosecond  Imaging Circuit Analysis of Leakage Currents in CMOS  Circuits”, ISTFA, 2002.


[4] A. Weger, et al., “Transmission line pulse picosecond  imaging circuit analysis methodology for evaluation of  ESD and latchup”, IRPS, 2003.


[5] S. Thompson, et al., “A 90 nm Logic Technology  Featuring 50nm Strained Silicon Channel Transistors, 7  Layers of Cu Interconnects, Low k ILD, and 1um² SRAM  Cell”, IEDM Tech. Dig., 2002.


[6] S. Rusu, et al., “Backside infrared probing for static  voltage drop and dynamic timing measurements”, ISSCC, 2001, pp. 276-277.


[7] W.G. McMullan, S. Charbonneau and M.L.W. Thewalt, “Simultaneous subnanosecond timing information and 2D  spatial information from imaging photomultiplier tubes”, Review of Scientific Instruments, vol. 58, no. 9, 1987, pp. 1626-1628.


[8] J. Vickers, N. Pakdaman and S. Kasapi, “Prospects of  Time-Resolved Photon Emission as a Debug Tool”, ISTFA, vol. 28, 2002, pp. 645-653.


[9] S.M. Mansfield and G.S. Kino, “Solid immersion  microscope”, Appl. Phys. Lett., 1990, vol. 57, pp. 2615.


[10] J.D. Warnock, et al., “The Circuit and Physical Design of  POWER4 Microprocessor”, IBM J. Research and  Develop., vol. 46, no. 1, 2002, pp. 27-49.


[11] W.V. Huott, et al., “Advanced Microprocessor Test  Strategy and Methodology”, IBM J. Research and  Develop., vol. 41 no. 4/5, 1997, pp. 611-627.


[12] R. Desplats, et al., “Automated PICA Transistor  Channeling and Spatial-Temporal Photon Correlation for  Faster IC Diagnosis”, IRPS, 2003.


[13] W.K. Lo, S. Kasapi and K. R. Wilsher, “Comparison of  Laser and Emission Based Optical Probe Techniques”, ISTFA, 2001.


p 45-54


DOI: 10.1361/cp2003istfa045


IC Diagnostic with Time Resolved Photon Emission and CAD Auto-channeling


Romain Desplats, Alban Eral, Felix Beaudoin, Philippe Perdu


CNES-THALES Laboratory- 18 avenue Edouard Belin - 31401 Toulouse Cedex 9, France


Alain Chion


ST Microelectronics, 850 rue J Monet, 38926 Crolle, France


Ketan Shah, Ted Lundquist


NPTest, Inc, 150 Baytech Drive, San Jose, CA


The use of time resolved photon emission (TRPE) to  compare internal measurements with simulations can  dramatically reduce the time required for IC analysis.  During  debug, this technique makes it possible to probe only  transistors of interest. Two limitations must be overcome: precise location of transistor photon emission areas and  distinction between photons emitted by closely spaced  transistors. Otherwise results may be seriously biased. Introducing CAD auto-channeling for TRPE makes it possible  to generate virtual layers where emissions are expected. As a  result, transistor TRPE areas can be automatically located and  emission from nearby transistors is taken into account, thus  significantly reducing the duration of IC analysis.


The increasing density and complexity of high–speed  integrated circuits makes fault diagnosis complex.  Sources of  problems range from process defects and tolerances to design  errors and cross-talk.  Fault diagnostics are limited by  inaccurate or incomplete fault models.  Direct measurements  inside the device are used to compare signals from a  manufactured device with expected or simulated ones.


Time resolved optical probing tools have been developed  to tackle the validation of new IC generations.  Optical access  to active areas of the device is often achieved through the  backside silicon due to the high density of metal routing.  The  time resolved photon emission (TRPE) detector records the  time of individual photons emitted during switching of CMOS  transistors.  Acquired data contains timing information about  transistor commutations.  To acquire commutation data from a  specified node, alignment with the CAD database is often  necessary.


In this paper, we used emission microscopy to characterize  the ignition and spreading of latchup in a series of I/O pins. Many different I/O environments were examined in order to  understand the effect of different parameters contributing to  latchup ultimately improving latchup resistance design. By  means of this novel adaptation of the JEDEC78 testing  procedure, the circuit structures and devices most prone to  latchup were identified. We also showed that minority carriers  can diffuse underneath lines of decoupling capacitances, if the  recombination length of the minority carriers is comparable  with the size of the capacitances.


The authors wish to thank Steve Wilson, Joe Eckelman, John  Hryckowian and Phil Wu, of IBM Systems Group, for  graciously providing the test chips used in the presented  measurements, for insight and helpful suggestions in test  methodology, and for support during the preparation of the test  board and electrical setup.


[1] T. Kessler and F.W. Wulfert, “Diagnosing latch-up with  backside emission microscopy”, Semiconductor International, no. 7, 2000.


[2] T. Aoki and A. Yoshii, “Analysis of latchup-induced  photon emissions”, IEEE Trans. Electron Dev., vol. 37, no. 9, 1990, pp. 2080-2083.


[3] P. Salome, C. Leroux, J.P. Chante, P. Crevel and G. Reimbold, “Study of a 3D phenomenon during ESD stress in  deep submicron CMOS technologies using photon emission  tool”, International Reliability Physics Symposium, 1997, pp. 325-332.


[4] R.R. Troutman, “Latchup in CMOS technology”, Kluwer  Academy Publisher, Boston, MA, 1986.


[5] H.B. Bakoglu, “Circuits, interconnections, and packaging  for VLSI”, Addison Wesley publications, 1990.


[6] M.J. Hargrove, S. Voldman, R. Gauthier, J. Brown, K. Duncan and W. Craig, “Latchup in CMOS technology”, International Reliability Physics Symposium, 1998, pp. 269-278.


[7] “JESD78 latchup testing standard”, Electronic Industry  Association JEDEC standards, Arlington, VA (www.jedec.org).


[8] “C4880-21 user manual”, Hamamatsu Photonics K.K.


-300 -250 -200 -150 -100 -50


0 20 40 60 80 100


120 140


latchup in "R1"


current,1DD[mA]Supply


80mA


quiescence


current


200


Pin current, Ipin [mA]latchup in "R2"


200mA


Figure 11: The current absorbed by the chip shows a double “jump” when the latchup ignites in the region “R1”and then in “R2” (no latchup is observed for positive Ipin).


Figure 12: 3D map of the latchup emission for a different I/O pin. The image shows the self-sustained latchup after the external test current was removed from the pin.


300,ESD


p 25-35


DOI: 10.1361/cp2003istfa025


## New Applications of Thermal Laser Signal Injection Microscopy (T-LSIM)


New Applications of Thermal Laser Signal Injection Microscopy (T-LSIM)


R. Aaron Falk and Neil Bauersfeld


OptoMetrix, Inc.


Mark LaPierre and Shawn Elliott


Fairchild Semiconductor


Thermal laser signal injection microscopy (T-LSIM) (aka TIVA and OBIRCH) has shown considerable promise in stateof-the-art digital integrated circuits. The technique has been utilized to locate shorts, leakage currents, problem vias, and timing issues in these devices. However, little has been published on the utility of this technique for analog and mixed signal devices. In this paper we demonstrate the application of T-LSIM on two different analog devices with defects that conventional FA technology and fault isolation techniques were unable to locate. Analog devices produce several unique challenges to the basic T-LSIM technique as typically utilized in the digital regime. Extensions of the basic T-LSIM technique were utilized to locate the failures, which produced unexpected results. The T-LSIM technique has proved essential in the quick identification and localization of failure sites.  The T-LSIM technique provides the failure analyst with the analytical power not previously available on conventional fault isolation tools such as emission microscopy and liquid crystal.


Lasers interact with semiconductor devices by producing photocarriers and heat. Both effects have been utilized in semiconductor failure analysis to localize defects using an array of techniques: OBIC [2], OBRICH [3], LIVA [4], TIVA[5,6], SEI [5,6], SCOBIC [7], XIVA [8], etc. All techniques


involve injecting a localized laser signal into the


ANODE


影MAIN TERM 2Pin6


semiconductor device while recording the device response. ALED


MT2


generalized concept of laser signal-injection microscopy(LSIM) covers all the current techniques, as well as those to


CATHODE25N/LTRIAC


come.


Pa al


N/C3


4MF1MAIN TERM1


Recording the device response takes on many forms, from sensitive monitoring of the circuit power draw to recording pass-fail conditions during active test. In a typical laserscanning microscope, the injected signal is simply an impulse


(TRIAG SUBSTRATE)'DO NOT QONNECT


of heat or photocarriers as the laser spot is scanned over the circuit. In the following tests the IC device impedance was monitored using highly sensitive techniques while the laser was scanned over the device. This process forms an image of the device impedance changes with coordinates corresponding to the laser position on the device. The laser wavelength, 1340 nm, was selected to only produce heating in the test device. A


reflected light image is obtained simultaneously from laser light scattered during the scan. These two images are perfectly correlated and can be used to relate device response to the physical position within the device.


Past efforts in LSIM have primarily focussed on digital devices. This paper demonstrates both the utility of LSIM when applied to analog devices and the rich array of behaviors that occur.


Triac Opto-Isolator Investigation


Device Description


The first Fairchild device examined is an optically isolated triac driver. As shown in Figure 1, the device contains a gallium arsenide (GaAs) infrared emitting diode and a light activated silicon bilateral switch (detector chip) that functions as a Triac (like a back to back SCR). The devices were designed for interfacing between electronic controls and power Triacs to control resistive and inductive loads for 115/240 VAC operations. These two chips are packaged into a single optoisolated dual in line package (DIP). The physical layout is shown in Figure 2.


Figure 1  Circuit schematic showing input LED and output TRIAC detector.


The gate terminal on the output triac detector chip is light activated and optically coupled to the GaAs infrared light emitting diode (LED). With the input LED turned off, there is no gate current and the two terminal Triac (anode MT1 to anode MT2) acts as an open circuited switch (high impedance). In the high impedance state with no gate current, the Triac electrical characteristics are a symmetrical forward and reverse breakdown voltage around +/- 400 volts (VDRM) with typical blocking current of 10 nanoamps (IDRM). When the input LED is on, there is sufficient gate current and the Triac switch becomes closed circuited (low impedance MT1 to MT2) allowing current flow in both directions.


Figure 2:  Optical photo showing input  LED and output TRIAC detector chip


Failure Indications


The device failed the parametric test VDRM46 (+ pin 4 to - pin 6) on the output detector Triac chip. The VDRM46 test measures the off state (LED off) terminal voltage of the Triac. Curve trace analysis while biasing + pin 4 (MT1) with respect to –pin 6 (MT2) showed an early breakdown voltage. The specified minimum VDRM46 breakdown voltage is 400 volts,but the failing devices in question had VDRM values between 200 and 300 volts (see Figure 3). Biasing the Triac device in the opposite polarity (+pin 6 to –pin 4) showed the device to function properly. Only one side of the symmetrical Triac device appeared to be electrically degraded.


Test Procedures and Results


A significant concern with testing the Triac device was typical operating voltages of several hundred volts. The sensing electronics were not designed to standoff such a large DC voltage. Testing needed to be performed at relatively low voltages. Although, the early V DRM46 (+ pin 4 to - pin 6)


breakdown was seen in the negative bias IV curves, positive bias (+ pin 6 to - pin 4) was also tried. The triac was seen to“turn on” at relatively low voltages in the reverse bias direction VDRM46 with ~ 90 mA current at – 1.5 volts. Initially,photocarrier LSIM (P-LSIM) was considered a good candidate for testing as the resultant photovoltaic effect samples the quality of the PN junction. The 10X images below for the defective device showed considerable asymmetry between the two contacts. This asymmetry was not seen in the “known good” reference sample (See Figure 4). Also seen in the defective sample was a slightly mottled appearance in the areas of induced photocurrent.


Figure 3:  Curve trace showing Triac VDRM46 breakdown voltages.


Although the P-LSIM results indicated something had occurred to upset the device symmetry, there was no clear indication of a specific defect sight. The mottling indicated potential sites, however, these non-uniformities appeared throughout the device and may have been caused by residual material known to be present on the device surface. A significant additional drawback to P-LSIM technique is that the area under the contacts could not be probed.


Thermal laser signal injection microscopy (T-LSIM) was not previously known for its ability to probe for junction defects.


Fortunately, a simple mouse click allows us to switch laser wavelengths and thermal injection as tried. An initially fuzzy signal image was brought into sharper focus when the microscope focus depth was reduced by ~ 3 microns. Images of these signals at 10X and 50 X are shown in Figures 5 and 6.


Note that signals are seen in the 50X image even in the contact areas. Clear evidence of a thermal effect. A “known good”reference device also showed some similar T-LSIM signals,but at much lower density.


Reflected light


Failing Device


Asymmetrical P-LSIM image


Reference Device


Symmetrical P-LSIM image


Figure 4:  Reflected light, and P-LSIM images of failing and reference devices.


T-LSIM image at –1.5 volts


Overlay of T-LSIM and reflected light image


Figure 5:  10X images of defective Triac device


T-LSIM image at – 1.5 volts


Figure 6:  50X images of defective triac device


The appearance of T-LSIM signals in this device was very puzzling at first. Clearly some mechanism other than the typical resistance change of materials with temperature was occurring. The crystalline appearance of the T-LSIM signal at 50X suggested that silicon crystal defects were responsible for the early device breakdown. This assumption was validated by later physical examination. These results suggest thermal signal generation physics in which the device current is modulated by changes in the junction work function due to the silicon crystal defects. Specifically, the proportional current flowing through the device is given by





 ∆


kT E


I exp


(1)


The scanning laser produces a change in temperature, T,which will produce a uniform change in I throughout the device, except in areas where the work function, ∆E, is significantly different. The silicon defects supplied the change in work function that was imaged via T-LSIM.


Triac Failure Analysis Results


Fault isolation techniques emission microscopy and liquid crystal analysis were unsuccessful in isolating the failure.


Microprobing was also unsuccessful since the photo base junction was not accessible (no metal contact to the base). The


failing device was deprocessed to silicon and a silicon defect etch was performed. A visual inspection afterwards revealed silicon defects between the N emitter and P base regions on the pin 6 side of the Triac detector chip, Figures 7 and 8. The location of the silicon defects correlated to the locations identified during the TIVA analysis.


Figure 7:  Low magnification image of deprocessed Triac showing silicon defects.


Figure 8:  High magnification image of deprocessed Triac showing silicon defects.


Darlington Opto-Isolator Investigation


The second Fairchild device examined was a voltage/current


Output Darlington


threshold detection optocoupler. This device consists of an Aluminum-Gallium-Arsenide (AlGaAs) LED connected to a threshold sensing input buffer IC that is  optically coupled to a high gain Darlington output. The output of the Darlington is TTL and CMOS compatible. These three chips are packaged into a single opto-isolated dual in line package (DIP). Figures 9 and 10 show the device schematic and physical layout respectively.


Figure 9:  Circuit Schematic of Opto-Isolator showing input buffer chip, input LED, and Darlington output detector chip.


The input buffer chip is capable of controlling threshold levels over a wide voltage range (0 to +/- 300 volts AC or DC) with a single external resistor. The low logic input state is specified as a threshold current between +2.4 mAmps (+Ith) and –1.2 mAmps (-Ith) or a voltage threshold range between + Vth


(+3.8 VDC or 5.0 VAC) and –Vth (–2.5 VDC or -3.7VAC).


Threshold current/voltage values greater than +Ith/+Vth and –Ith/-Vth are specified as a high-level logic input state. When a low-level input state is applied to the input buffer chip, the input LED turns off. This causes the output Darlington


mitter


detector chip to remain in a high logic output state (high impedance from output to ground). When a high-level logic input state is applied to the input buffer chip, the LED will turn on. The LED will in turn couple to the Darlington detector chip causing a low-level logic output state to be observed on the output (low impedance from output to ground).


P Base


Figure 10:  Optical photo of Opto-Isolator showing location of input buffer chip, input LED, and Darlington output detector chip


Input Buffer


AC1


8Vcc


The device failed function (output intermittent low) when an intermediate low-level threshold was applied to the input


DC+2


7NC


buffer chip. The low-level threshold is specified as a threshold current range between +2.4 mAmps (+Ith) and –1.2 mAmps (-Ith) or a voltage threshold range between + Vth (+3.8 VDC or


DC-3


，6Vo


5.0 VAC) and –Vth (–2.5 VDC or -3.7VAC). The device in


Inpot


。


LED，


question failed only at intermediate low-level input threshold


V


AC4


Output5GND


currents/voltages (see AC and DC curve traces in Figures 11 to 14). The devices operated properly at all other input


Darlington


threshold values. Analysis of the electrical characteristics of the input LED and the output Darlington ruled them out as the cause of the failure. The cause of this “glitch” was narrowed down to the threshold sensing input buffer die.


AC CURVE TRACE


DC CURVE TRACE


REFERENCE DEVICE


WIN(V)


2.00vidyMARKER( 2.500mA .5.0049V.5.0811V0.80w/divCURSOR(-1.300mA ..0130v.-9.9480V]Vout(v)


VIN(v)


1.0vidirMARKER( 200.0UA, 5.0000V.1.3820V)0.50vidiv


LED OFF


110.00.


5.00


10.00


OUTPUT


8.00，


9.00


6.00-Output


4.00


8.00


460


肌


4.66.


+wth


2.00-


4ith3.00


6UO


3.00


0.00.


+


15.00


-Vich th


-4.00.


Input


6.00


1.00


2.00


-1.00


-8.00.LED ON


LED ON


-10.606.0mb 40-3.020-100.0


IIN (ma)


IIN(UA)


1.00maldiv


40.00uA/division


to2.03.0406.0ma0.00


0.0090.0


200.0280.0


400.0


6.60


INPUT


12.00


.200


7.66.


Vout(v)


Figure 11:  Curve trace of reference device showing proper


Output transition at  +/-Ith


Figure 12:  Curve trace of failing device showing output level glitch at intermediate threshold +/-Ith when LED is supposed to be off.


Figure 13:  Curve trace of reference showing +Th behavior at


1.48-1.8 VDC.


FAILING DEVICE


WIN (v)CURSQR(2.400mA.5.0068Y,10.027V] Wout(v)


2.00w/divMARKER(-1.400mA..0180Y，-4,0029V0.50vidlw


1.0ridiw


10.00+


8.00+


9.00'


6.00+


*-Output Glitch →


4.00.


+VIh补血


0.00:


Wth th


=4.00-


600-


声h v-Vith


Gitch


Glitth


-10.00


6.0ma -4.039 29-1.00.01.02.03.04.0 N (ma)


IN (uA)


1.00ma/d


40.COmpdly1siom


5.0ma


0.0080.0


200.0280/0


466.00.0p


200-


3.00-


4.00,*


6.00，


Output


7:00


8.00.


.4.00


MARKER(280.0UA ..0740V,1.5050V0.50wdiv CURSOR(370.0uA. 5.0000V.9.9911V )Vout(v)FAILING DEVICE


Figure 14:  Curve trace of failing device showing +Th behavior at 1.4-1.8 VDC


The nature of the device failure made it unclear what, if any,LSIM effect might appear. The LSIM sensor was placed over the input buffer chip of the device. This arrangement is different from the usual monitoring of the device bias lines. TLSIM images were then obtained as the input voltage was varied in the region where the switching failure occurred. It


was hoped that thermal stimulation of the sensitive area of the circuit would shift the bias point sufficiently to cause the circuit to produce a useful signal. The richness of the results can only be adequately described through a computergenerated movie (available at www.optomet.com). The selected image sequences in Figures 15 - 17 indicate a portion of the device behavior.


The first sequence of images runs from 1.480 to 1.600 volts in


0.024 volt steps, representing every twelfth frame of the 60 frame movie. The first frame of the movie is identical with the LSIM signals obtained with a “known good” reference. On the reference device the signals did not change for this voltage range. On the failing device the richness of behavior over such a small input voltage range was striking. In the forth image of the sequence, the areas that produce dark spots with white tails in images 2 and 3 blank out and the rest of the device shifts into a hyperactive state (fail state with output low). The diagonal bars seen in the image suggest that the device is oscillating. In the next two images, the hyperactive state


relaxes and a new set of signals resolves to a single small signal (image 6) not seen in the first image (recovering ~output transitioning high).


The next two sets of images show details over a limited range with 0.004 volt steps (every other frame of movie). The first sequence shows the changes in signal strength occurring in the signals that appear prior to the hyperactive state (failing state).


The second detailed sequence shows how the hyperactive state resolves down to the single localized signal.


1.480 VDC (pass – output high)


1.504 VDC (output transition low)


1.528 VDC (begin fail - output low)


1.552 VDC (mid fail – output low)


Appearance suggests device oscillation.


1.576 VDC (end fail – output low)


1.600 VDC (output transition high)


Figure 15:  T-LSIM images of device response between 1.480 to 1.600 volts in 24 millivolt steps (transition from pass-fail)


1.510 volts


1.514 volts


1.518 volts


南


1.522 volts


1.526 volts


1.530 volts


Figure 16:  T-LSIM images of device response with input threshold ramp between 1.510 to 1.530 volts in 4 millivolt steps (output transition from high to low ~ failure state).


1.560 volts


1.564 volts


1.568 volts


1.572 volts


1.576 volts


1.580 volts Figure 17: T-LSIM images of device response with input threshold ramp between 1.560-1.580 volts in 4 millivolt steps(output low and beginning to transition high ~ recovery state).


The dark signals with white tails seen in the images prior to the hyperactive state are indicative of a transistor state being modulated by the laser thermal injection. This was later identified as the failing NPN transistor. This modulation effect has been seen using P-LSIM in digital circuits, however, TLSIM generally does not produce such strong effects. The later sequences also indicate strong interaction between the device and the thermal signal injection. Clearly, the defective device was not being maintained in a stable state.


At intermediate input threshold values between 1.48 and 1.60 volts, a strong TIVA signal was seen at an internal NPN transistor that is part of the latching circuitry. The NPN transistor is critical in determining the output signal to drive the LED. As the device begins to fail, the signal at this NPN transistor begins to get stronger. When the device is failing(glitch – output low) the NPN transistor drives the output drive circuitry resulting in the other rich TIVA signals seen(“hyperactive state”). As the device begins to recover, the


signal at this NPN transistor becomes weaker as the output becomes stable (output returning to the normal high state).


For analog devices, use of a reference device is often


desirable. Figures 18 and 19 show overlays of the response of a known-good device and a failed device at below threshold


input voltages. Both devices show a T-LSIM response in the upper left quadrant. The failed device shows additional signals not seen in the known-good reference.


Input Buffer Chip Failure Analysis Results


The "glitch" failure was caused by defects in the silicon crystal lattice on the input buffer die. This “glitch” momentarily turned on the output die at intermediate low-level input threshold currents/voltages. The TIVA signal above (left photo) showed a single NPN transistor turning on during the output “glitch” on the failing device. This structure did not turn on with the reference device. Microprobing showed leakage on this NPN transistor collector-emitter. Deprocessing


to silicon followed by a silicon defect etch revealed silicon defects at the emitter implants of the failing NPN transistor on the input buffer die (see Figures 20 and 21).


号


Figure 18:  Overlay image of input buffer chip of known-good device showing T-LSIM response in upper left quadrant.


Figure 19:  Overlay image of input buffer chip of failed device showing additional T-LSIM response in upper right quadrant.


• LSIM techniques are of significant value for location and analysis of defects in conventional analog and mixed signal devices.


• Analog devices demonstrate a rich set of behaviors with bias voltage and operating conditions.


• The ability of the LSIM tool to vary parameters while performing sequential image acquisitions (i.e. movies) is important in understanding and communicating the defect signals.


• Comparison to a “known good” reference device is often required to fully analyze the defect.


• LSIM techniques significantly reduce the amount of microprobing needed during failure analysis by isolating failure sites not detected by traditional fault isolation methods, thus greatly reducing analysis time.


Figure 20:  Low magnification image of silicon defects.


Figure 21:  High magnification image of silicon defects.


1. For a review and further references see: K. BernhardHofer, D.L. Barton, and E.I. Cole, Jr., "Flip-Chip and Backside Techniques", Microelectronic Desk Reference 4th Edition, 487-503 (1999)


2. 1.Tony Wilson "Theory and Practice of Scanning Optical Microscopy", Academic Press, London (1984)


3. K. Nikawa and S. Inoue, "Various Contrasts Identifiable from the Backside of a Chip by 1.3 um Laser", ISTFA 387-392 (1996)


4. E.I. Cole, Jr., J.M. Soden, J.L. Rife, D.L. Barton, and C.L.


Henderson, "Novel Failure Analysis Techniques Using Photon Probing with a Scanning Optical Microscope",IRPS, 388-98 (1994)


5. E.I. Cole, Jr., P. Tangyunyong, and D.L. Barton,"Backside Localization of Open and Shorted IC Interconnections", IRPS, 129-136 (1998)


6. E.I. Cole, Jr., P. Tangyunyong, D.A. Bensonand D.L.


Barton, TIVA and SEI Developments for Enhanced Front and Backside Interconnection Failure Analysis", ESREF(1999)


7. M. Palaniappan, J.M. Chin, J.C.H. Phang, D.S.H. Chan,C.E. Soh, G. Gilfeather, “Application of Single Contact Optical Beam Induced Currents (SCOBIC)”, ISTFA 17-21 (2000)


8. R.A. Falk, “Advanced LIVA/TIVA Techniques”, ISTFA,59-65 (2001)


p 36-39


DOI: 10.1361/cp2003istfa036


## PC Card Based Optical Probing of Advanced Graphics Processor using Time Resolved Emission


PC Card Based Optical Probing of Advanced Graphics Processor using Time Resolved Emission


Howard Lee Marks, and Tung Ton


NVIDIA Corporation, Santa Clara, CA, USA


Jeffrey A. Block, Steven Kasapi, and Chris Shaw


Optonics, Inc., Mountain View, CA, USA


Internal node timing probing of silicon integrated circuits(ICs) has been a mainstay of the microelectronics industry since very early in its history.  In recent years, however, due in part to the increase in the number of interconnection layers and continued proliferation of packaging techniques exposing only the silicon substrate, conventional probing technologies such as e-beam and mechanical probing have become cumbersome or impractical.  In an effort to continue transistor-level probing, backside optical probing technologies have been developed and adopted [1].  Chronologically, such techniques include picosecond image circuit analysis(PICA)[2], laser voltage probing (LVP)[3], and dynamic or time-resolved emission (TRE)[4].


In typical examples of backside probing the device under test(DUT) relies on device stimulation from automatic test equipment (ATE) or equivalent bench top setup.  This generally requires a specially designed DUT card designed to accommodate a low-profile socket and lid.  The DUT card,which is significantly smaller than the tester motherboard, is designed to fit within the chamber opening of the probe system in order to interact with the optical column.  Tester stimulation of packaged parts, however, does not address the need to probe the DUT in-situ and in the intended application,such as a PC board.  It is often desirable to probe the DUT under conditions typical of the final product or running standardized application based tests.


We present here this application and have addressed some of the challenges associated with PC card based optical probing and show successfully performed time-resolved emission on a second-generation advanced graphics processor in a standard graphics card.


Traditionally there have been a number of issues associated with the probing of devices installed on a PC motherboard or peripheral bus card.  Most commercially available probe systems provide limited chamber access.  A common constraint is that the chamber size is small and microscope ztravel is limited; make it very difficult to introduce a PC motherboard and peripheral card into a location where the final optics are able to interact with the DUT.  Another constraint is that it is necessary to establish a reference trigger signal that is synchronous with the DUT activity (system clock, for example) in order to adequately sample the


electrical activity at the location of interest.  In the cases of ATE or bench-top setups it is generally easy to meet such requirements since the trigger signal can be generated within the test program.  Finally, during probing it is often necessary to provide some means of removing heat from the DUT.


Traditional techniques involving varieties of heat-conducting“heat spreaders” in contact with a thermal reservoir will not work because of the cluttered and populated regions near the DUT when probing on PC motherboards or peripheral cards..


While the CAD layout is used to align metal lines with  great accuracy for front side analysis, it is not as precise for  backside location of an area in the vicinity of a transistor  channel which may be smaller than 100 nm. In addition, access to the CAD layout is confronted with proprietary issues  and processing and transfer resources involved with extremely  large files.  Another important limitation encountered using  TRPE is that detector spatial resolution (e.g., 1 µm) is much


larger than the latest IC technologies (e.g., 0.1 µm). Consequently, probing a single transistor without photons  contributed from its neighbors is not always possible. Contributions from nearby emitting transistors must be taken  into account for device analysis.


The first problem to be resolved concerns the spatial  location of transistor TRPE areas, which do not appear in the  CAD layout as metal lines do. The second problem concerns  the backside alignment of the device with the CAD layout. One issue concerns the detector spatial resolution and the  other concerns the size and processing time of the CAD  databases. Finally, the last problem we address in this  document concerns emission from nearby transistors which  bias the signal of interest. To successfully use TRPE for a  device with millions of transistors, each probing measurement  must be obtained with great confidence (no cross talk) and as  fast as possible.


We will start with a review of the TRPE principle in order  to define exactly where (and when) photons may be emitted  by transistors. With this knowledge we can then transpose this  area definition onto the CAD layout. Then, we will present a  3D technique (space and time) which takes photon emission  from nearby transistors into account to quickly obtain high  quality timing measurements. Applications will be presented  on a STm 0.12 µm – 1.2 Volt device.


Time Resolved Photon emission Principle


Time Resolved Photon emission (TRPE) utilizes  naturally occurring light emission from switching FETs. The  TRPE detector records the time (t) at which individual photons  are emitted, and, therefore, contains timing information (see  Figure 1) useful for debug and failure analysis of integrated  circuits.


Testing and validation of logic devices is often  performed using signals defined by voltage levels. A sequence  of 0s and 1s describes the input or output waveform for any  point in a circuit. Internal probing of a device with either an ebeam prober or a laser voltage prober makes it possible to  measure the logic waveforms inside the device itself. Comparison of these measurements with simulation reveals  disparities when a problem exists.


TRPE, on the other hand, records photons emitted due to  current variations rather than voltage/logic states. . The signal


0.9 1、


peaks obtained with TRPE do not reproduce the logical


0.8<


waveforms typically associated with simulation results.  In


≥0.7


part, this disparity is caused by the difference in the number of


20.5-00.6


photons emitted from nMOS and pMOS devices.  To first


Z0.4-


order, the difference in emission efficiency is related to the


difference in electron and hole mobilities under the channel.


0.2、


Detector


4么


50


PIXEL0


-50


-50PIXEL


G


Figure 1.  Photon emission with TRPE.  Photons are emitted, mainly  from the drain end of the channel, during transistor commutations.  For Backside analysis, the device under test is upside down.


According to Tsang et al.  [1], photon emission in silicon  devices (indirect bandgap) is primarily related to the  generation of hot electrons (and hot holes). For field effect  transistors, the generation of hot carriers results from gaining  sufficient kinetic energy under a strong electrical field  [2]. Such a field exists in the depleted region of a transistor  channel under saturation conditions. In CMOS technologies  this condition occurs briefly during commutations (0 to 1 and  1 to 0). In an NMOS transistor the location of the highest  probable source of photons for TPR is at the border of the  space charge zone with an extension toward the drain side (see  Figure 1)  [3]. For a PMOS transistor, it corresponds to the  source side.  In the case of a 0.1 µm technology, the region, where hot carriers have the highest velocity, is smaller than  the gate width itself (100 nm).


However, the region over which photons from a highly  localized source is considerably larger than the source itself. Figure 2 shows the theoretical estimate of the spot size due to  emission at a wavelength of 1 micron.  The size of the Airy  disk is 1.22 microns in diameter.  In addition, we have made  an experimental determination of the spot size using standard  static photon emission techniques using a Hamamatsu Phemos -1000.  We have determined that photons from a highly  localized source are collected over an area of 3 microns x 3  microns surrounding the emission site.  These widths are then  used to calculate the size of the regions in which one can  expect to collect emissions from a single source.


-100-100


Figure 2.  Modeling  of a photon emission spot for a point source  transistor (0.1 µm technology. The maximum Airy disk diameter Φ is  given by Rayleigh criteria:


1.22 λ⋅


Φ


with λ=1 µm.  In practice, photons can be collected more than 3 µm away.


NN


TRPE (1 dimension) vs PICA (3 dimensions)


The PICA detector not only records the time of each  acquired photon but also its spatial (x,y) position. Consequently, several transistors may be acquired during the  same acquisition. PICA is very valuable for precise timing  characterization of transistors in the same field of view since  the time reference is exactly the same for all of them. In  practice, the quantum efficiency of the PICA detector is much  lower than that of TRPE. Hours are needed with PICA while  only minutes suffice with TRPE. The limitation of TRPE, however, concerns its lack of spatial resolution. Spatial  resolution is improved by restricting the field of view of the  detector with blades (razor blades) down to less than 1 micron. With CAD auto-channeling, optimal reduction of the field  of view (with blades) is automatically calculated. However, even with the blades closed down to show only a small area  around a transistor of interest, parasitic emission for nearby  transistors affects the measurements. This limitation is taken  into account and will be detailed in the STPC-3D processing  paragraph (Spatial Temporal Photon Correlation). Throughout  this document we will use some PICA acquisitions to  demonstrate the spatial extension of the area where photon  emission is detected around a transistor


Using the Circuit CAD Layout for TRPE


Device debug using PICA requires the identification of the  transistors of interest and their respective (x,y) locations.  This  process can be performed manually from the layout.  However, in many cases, the transistors of interest are  identified based upon the logical net to which they are  connected.  Use of the net name to select and isolate these  transistors requires the use of cross reference information  which links the net names to the shapes in the layout that  comprise the net.  Once the transistors are identified and  located, the locations of the preferentially emitting regions of  the circuit can be specified.


To define accurately the window in which photon may be  collected, let us look back briefly at the theory.


CAD Auto-channeling for TRPE


For large integrated circuits, manually adjusting the  window size for each transistor is a painful process. It is not  only time consuming but also a source of errors. In a 0.1 µm  technology, transistors are separated by less than a few  microns.


In order to automate this process, we have developed a  technique which uses a few layers of the existing layout to  generate localized regions where photons may be collected  from individual emission sites.  These regions are placed in a  virtual layer containing the pertinent CAD information for the


>


purposes of TRPE and PICA.  The advantages of this  technique are threefold.  First, the TRPE window sizes are  quickly defined.  Secondly, proprietary information about the  specific circuit design can be withheld if necessary.  Thirdly, the new layout is contained in a considerably smaller file,


In


minimizing computing resources associated with PICA and


BG


TRPE analysis.


Automatic TRPE Transistor Channeling from CAD


One of the challenges in defining a windows for TRPE


channels is to find the active areas of transistors; i.e., the gate, which is located under the polysilicon, between the drain and  source diffusions. As shown in Figure 4, the polysilicon “rectangle” is much longer than the transistor gate itself. Using Booleans operators (NOT, OR, AND), we have worked


on two techniques to extract TRPE channels from the CAD  layout. The first one is based on the gate areas as emitted  locations. The second one is based on the transistor diffustion  areas to cover the emitted locations. The choice between each  technique depends on the available information since a CAD  layout may not contain all layers. Before describing these  techniques, we have summarized the TRPE channel creation  process in a diagram (see Figure 3).


Polysilicon


Diffusion


Nwell


P-MOS


N-MOS


Figure 4.  Example of a basic CAD layout for a CMOS inverter gate.  The circuit is described as a set of polygons (rectangles) for each  layer used in the manufacturing process.


Figure 3.  Diagram of automatic TRPE Transistor Channeling from CAD. If the schematic is available, TRPE channels can be accessed using


their names. Our experience gave best results using diffusion layers to generate virtual layers for TRPEN+ and TRPEP+ channels.


CAD


Database


ULayout Only


Layout + Schematic


METUIST


TRPE channels  names


LEGEND


LAYGUY


POLY : Polysilicium (gate)DIFF : Diffusion area


NWELL : n-type


Enlargement


TRPE CAD  layout with  virtual layers


Example of a CMOS  structure (#7)


TRPEN+ channels


after x5 factor


enlargement


TRPEN+ with


Poly overlay


Virtual layers (contoured) with  POLY overlaid


Virtual  layers  from  DIFF


TRPEN+ TRPEP+


TRPE channels using transistor gates


In CMOS technology, an NMOS transistor is defined in  the layout as a polysilicon N-gate between N+ diffusions (drain and source), over a P-substrate or P-well. In a  symmetrical manner, PMOS are made with a poly P-gate  between two P+ diffusions over an N-well (see Figure 4)


Identifying the N-gate and the P-gate is possible once N+ and P+ diffusions have been differentiated (see Figure 5).


NMOS


N+DIFFUSION: DIFFUSION AND PSUBSTRATE  NGATE: POLYSILCON AND N+DIFFUSION PMOS PMOS P+DIFFUSION: DIFFUSION AND NWELL  PGATE: POLYSILICON AND P+DIFFUSION


Figure 5.  Boolean rules for transistor electrode identifications


Since the Booleans rules may be added to the technology  file with the appropriate syntax, the two layers, NGATE and  PGATE may be generated with any CAD software. and  converted to a small GDSII layout, containing only two virtual  layers and a fiducial one (e.g. PAD layer) for alignment.


TRPE channels using diffusion layers


In several CMOS technologies, transistors may be


constructed with multiple gates in parallel (fingers). Therefore,


the above approach may differentiate two fingers of the same


transistor as two TRPE channels. To overcome this limitation,


all gates included in the same diffusion area are recognized as


one TRPE channel.


Since the “inclusion” is not a Boolean rule, it must be


done in a post processing step. Using Matlab, we take an SGD initial GDSII file containing polysilicon, NWELL and diffusion


layers. We successively apply the NOT, AND, OR Boolean


rules and the inclusion in order to generate two TRPE


channels (i.e., TRPEN+, TRPEP+) In the application presented


in this publication, each TRPE channel is the size the diffusion


of transistors (see Figure 7).


TRPE channels with the Schematic


In addition to this geometric localization of TRPE  channels, it is often useful to have the electrical names of the  various gates and transistors to be analyzed. These names are  not available in the layout but in the schematic of the circuit. By processing the layout and the schematic together with  Layout versus schematic (LVS) options, electrical numbers  from the schematic are attached to each polygon in the layout. Using the generated cross-referenced file, each polygon of the  layout corresponding to a transistor can be identified from its  electrical name  [4].


In our opinion, this second approach is necessary for  automatic TRPE probing. From the design, a list of candidates  can be probed and measurements can be automatically  compared to references until the fault has been diagnosed  [5]. Using Cadence Dracula 4.6 as an example, we implemented  this approach using only the following 4 files as inputs: 6NXREF.DAT (cross-referenced file) POLY.DAT, DIFF.DAT and NWELL.DAT. Our goal was to work with


small files, transmitted by email from the design center to our  Service Lab. This was possible since the TRPE reduced layout  did not contain proprietary information concerning the device  or the technology.


Resizing CAD Channels for TRPE


As described earlier, photons can be collected more than  3 µm away from the 0.1 µm width transistor gate. As a result, an enlargement factor may be applied to extend the CAD  channel area to match the size of the TRPE collection window. However, more complex geometries (rectangles with rounded  edges) may be calculated using additional parameters to match  the TRPE detector geometry.


Resizing TPRE channels is very important (see Figure 3). Before enlargement, many photons appear to be outside  channels. As a result, a much longer acquisition time would be  necessary if one did not realign and resize the TRPE  acquisition window. For TRPE channels after enlargement, most photons are included in each channel. In addition, alignment errors have a more limited impact since the  enlarged windows still enclose each photon spot.


With Automatic TRPE Transistor Channeling from CAD, we have resolved our two first problems: the spatial location  of transistor TRPE and CAD database handling (IP, resources, and alignment). Now, we may tackle the last problem: emission from nearby transistors which biases the signal of  interest. If we look again at TRPE channels again after  enlargement; we can see that they overlap two by two. It  means that in the common area photons may come from two  possible sources and must be correctly reattributed either to  the upper or lower transistor.


RESIZE Gate by β


Figure 6.  Re-sizing the transistor gate polygons to obtain TRPE  transistor channels.


Spatial and Temporal Photon Correlation for  TRPE


The next problem we face is that detected photons cannot  always be associated with the switching transistor of interest.  Some photons may come from areas where no transistors are  nearby.  These photons correspond to background noise.  Current TRPE analyses, especially with PICA, are based on a  lengthy acquisition time in order to increase the signal above  the noise level (see Figure 7).  In time, as the circuit test  pattern is looped synchronously, the signal rises higher and  higher above the background noise.  PICA acquisitions can  take hours and it would be advantageous to reduce  significantly the acquisition time.


To tackle this challenge we have developed a spatial  temporal photon correlation approach.  The objective of this  technique is to classify all detected photons as either noise or


as signals.  The remaining photons contain only meaningful  information and some transistor commutations or events  appear after just minutes of data acquisition.  In the  application presented later in this document, STPC-3D was  conducted with 1 million photons. This corresponds to 40  minutes of acquisition for this 1.2 V – 0.12 µm technology. As  a comparison, regular analyses were conducted. However, to  have a descent signal, 80 hours of PICA acquisition were  necessary.


4096


Figure 7.  Raw data- Regular PICA image obtained after 12 minutes


of acquisition (300 K Photon).  The Azuma device is a 0.18 µm


technology (1.8 V) with a substrate thickness of 20 microns.


Principle of Spatial Temporal Photon Correlation


During PICA acquisition, the device test pattern is looped  in order to increase the signal to noise ratio.  All detected  photons are tagged with their 3D coordinates: space (x,y) and  time (t).  If a photon comes from a switching transistor, it must  be correlated simultaneously in space (in a transistor area) AND in time (in a commutation time frame).  If a photon is  not correlated to its neighbors in both space and time, then the  photon is considered noise and is given less weight in the


o0


1024


2048


3072


analysis. .  Based on this 3D property of correlated photons, an  additional parameter called the weight is added to the (x,y,t) coordinates of acquired photons.  The weight corresponds to  the significance of photons or to the correlation value. The


higher the weight, the higher the probability of being a signal. (see Figure 8) On the right hand side of , representation as a  function of the weight instead of as a function number of  photons enhances the signal level.


To extend the “simple” 3D correlation to STPC-3D for


TRPE in general, we separated the weight attribution process  into: 1-Spatial correlation of photons and 2:-Temporal/frequency correlation (see Figure 9 step 3 and 4). This improvement was made possible by the CAD auto3072


channeling process which enhanced spatial cancellation of  noise from nearby transistors and background.


00


3072#74096


T


The tn)


Any Data


T (ps)


Spatial and


Correlated Data


.0


Temporal (3D) weight attribution principle


12


SOLZ


Before


After


9060


Figure 8.  3D representation of the photon weight attribution for spatial temporal photon correlation.  The color of photons corresponds to their  weight, from dark blue (weight=0) to red (high (x,y,t) correlation value).For a given area, the raw data photons were placed in time (a-left).  Photons (b-center) were correlated in space and time with their weight indicated by color


Figure 9.  STPC-3D Processing diagram using CAD auto-channeling


for TRPE (spatial (x,y) and timing( t) information are processed


separately to meet TRPE requirements.


For TRPE systems which record only timing events (i.e.,


NPtest SSPD or Credence Emiscope), spatial correlation is


obtained by probing the transistor of interest and its


surrounding area with at least two measurements. The


surrounding photons are used to evaluate the noise floor and to 4096remove bias signals from nearby transistors. As we mentioned  earlier, we have chosen here to present STPC-3D for PICA


since x,y,t can be displayed on an image to give the reader a


better understanding of this approach. Also, due to the low


quantum efficiency of the current PICA detector, the


efficiency of each step of STPC will appear clearly. Again, for


technologies with VDD lower than 1 Volt, the signal to noise


3.


ratio with TRPE is similar to PICA. STPC-3D for TRPE then  becomes valuable.


5 12


In order to present STPC-3D we will start from the spatial


M


correlation (Figure 9 step 4). Spatial processing was detailed  before and calculation of the timing weight is done by looking  in a dt interval with dt define follow:


2100 2120


( ) ( )


weight


Median


Max


_


(Equation 1)


2060 2080


2020


1680


2040


1700


Spatial Correlation (Step 3)


198019601940


Y coordinate19201560


Xcoordinate


1580


1600


1620


1640


2000


1660


After CAD autochanneling for TRPE, the areas where  photons may be collected are defined for all transistors. Around each area, a contour window is outlined. See Figure  10, Figure 11, Figure 12 and Figure 13.


After interpolation of the weight of photons from the  contour to the inside window, the noise level from the  signal+noise is removed, thus obtaining a signal level (see  Figure 15 and Figure 14). This process can be viewed as  removing the DC component on a scope and keeping only the  AC signal.


Figure 10.  Representation of the weight of photons as a function of  space in the area obtained after CAD autochanneling with 100K  photon (6 minutes of acquisition). In the inside window, photons  come from signal and noise.


Figure 11.  Representation of the weight of photons as a function of


space for one transistor (#7) after spatial interpolation on the


weights of signal+noise photons inside the channel CAD


autochanneling with 100K photon (6 minutes of acquisition). In the  inside window, photons come from signal and noise.


#


1024 g0


1- Spatial


Processing  TRPE channels


from CAD


2-Timing  Processing (t weight)


3- Spatial


Correlation +


4-Temporal  Corration


5-Optimal  commutation  times extraction


Figure 12.  In the contour window photons mainly comes from


background noise or bias signal from nearby transistors.


X coordinate


Figure 13.  The background noise for transistor #7 is interpolated  inside the TRPEN+ channel.


2.5


119


2.


1.5


19 5


M1


0.5、


00.511.5samlhunmer22.533.5


x10*


Y coordinate


Figure 14.  Spatial correlation. The noise level calculated from the  outside window is removed for transistor #7. The signal level is quite  different from the theoretical Airy disk presented in Figure 2.


Figure 15.  Spatial correlation. The noise level calculated from the


outside window is removed to keep only the signal level.


Temporal/Frequency Correlation (Step 4)


After spatial correlation, commutations may start to  appear in the timing domain. The challenge is to keep the


peaks which are lower than the remaining noise level. To do  that we introduce a dt (or delta T) parameter which  corresponds to the timing error brought by the jitter (e.g., dt=30x2.5 ps). If a high number of photons are collected in the  same dt time frame, they have a good probability of coming


2


from the same commutation.


To detect more signals from noise, a correlation is done in


the frequency domain. Transistor commutations occur with a


15


limited bandwidth. At very high frequencies, events come


v1


from randomly collected photons i.e. noise. Also, at low  frequencies, background noise or bias signals may be removed


0.5


[6]. The results obtained from the Fourier transform are  applied as a sliding window in time. See Figure 17.


2100


2050


19501560


1.8


160016201640


Resut in photons number of chip n22


Figure 16.  Timing information represented in photon number for


1950156015801600162016401660


transistor #7. At best, with 100K photons, 2 photons arrive at the  same time.


gg古


名


0.0 2400


2200


1800


粤


1600 1400


05001000150020002500300035004000


Figure 17.  Timing information for transistor #7 represented in  weight (a.u.) before (blue) and after (green) temporal/frequency  correlation (step 2).


‰0.511.522.533.5


Sample nummer


x104  Figure 18.  Timing information for transistor #7 after local max  computation (step 3).


Optimal commutation times extraction (Step 5)


The last step of STPC-3D for TRPE consists in extracting  local maximum peaks to find the optimal commutation times  see Figure 18. If two peaks are close to one another (e.g., 5 ps) the will be recognized as one. Optionally a threshold may be  applied to remove remaining bias signal (e.g., parasitic  commutations). To assist the user with this task, we have  developed a statistical and mathematical function for  processing the signal. Finally, commutations can be compared  to simulation or reference measures  [5].


Benefit For Circuit Designers


Since the layout can be automatically processed, the whole  EDA database for TRPE characterization is no longer  required.  The advantages are twofold.  First, proprietary  information in the full layout does not need to be disclosed, which is not just important for outsourcing but also for  optimizing control of the IP.  Second, the TRPE transistor  channeling layout can be sent by email and instantly processed  on a TRPE system and then kept available for reference for  failure analysis if field returns occur.


Once we know where photon emission occurs, the TRPE  field of view is optimally set to validate the most critical 台


transistors.  The next challenge is to extract timing  information from TRPE acquisition in order to rapidly check if  a transistor is commuting or not and if its timing signature  corresponds to design simulation or not.


Zo


STPC-3D Application to a 0.12µm – 1.2 V


146MM0


Technology


To demonstrate STPC-3D on an application, we have  chosen a difficult case study: a 0.12µm STm device. In the  next figures results of STPC-3D are presented for this 0.12µm


唱0.5IhI22533.5性11I]h.IIIII


– 1.2 V STm device.


To demonstrate the technique, we have acquired PICA


x104


data on a 0.12 micron VLSI circuit operating at 1.2 V.  Two  sets of data were acquired.  The first data set consisted of an  80 hour PICA run with no CAD Auto-channeling STPC-3D  analysis.  These results are shown in Figure 19.  The second set  of data was acquired in 40 minutes using the techniques we


25


have described.  These results are shown in Figure 20 to Figure  26


E144a


222。。as款b121..2自tt1.....1 te**0* *0** * ......


36


. . . .. .。自0.....


145RM


日


200.120813000**


00311680


694CX2476 124086440


D h


**工


Figure 19.  Regular PICA image obtained after 80 hours of


acquisition (120 M Photon).  The device is a 0.12 µm technology with  VDD=1.2 V with a substrate thickness of 35 microns.


*069


mococ月拾叁拾贰


Figure 20.  For STPC-3D, 1 million of photons are used. This  corresponds to 40 minutes of acquisition instead of 80 hours. In  addition the final results in also improved.


3000


30


。000口0口口。0000000000口a000


2800


2600%%08o80088%0to0%888中 24000口00b口00口0000口000600口口


石


2200E0000000000000000000000000000000D000000000000000000000 2000


1600df88凸88888名b6d88888


1400to88888B8名吊6%%d8凸吕8日


120005001000150020002500300035004000


Z900


IIIIIIIIIIIIIIIIIIIIIIIIIIIIIIIIII


9


Figure 21. TRPEN+ channels for the STm device. They are more


1500


than 318 n-transistors in the field of view.


100025002600 2700 280029003000 3100 3200330034003500


Figure 22.  Representation of the weight of photons as a function of


space in the area obtained after CAD autochanneling with 1M


photon (40 minutes of acquisition) for a selection of transistors. In  the inside window, photons come from signal and noise.


Figure 23.  In the contour window photons mainly comes from


Figure 24.  Spatial correlation applied to a selection of transistors  for clarity purpose. These transistors come from the center left region  of the acquisition. The noise level (bias signal and background noise) calculated from the outside window has been removed to keep only


the signal level.


Z0t8


道


Figure 25.  Timing information for transistor #7 represented in


weight (a.u.) before (blue) and after (green) temporal/frequency


correlation (step 2). Peaks are visible (green).


Figure 26.  Timing information for transistor #184 after local max  computation (step 3).Compared to the expected commutation


diagram, the 4 peaks detected after a 40 minute acquisition match the  simulation


Discussion: STPC-3D for 1 Dimension TRPE


The first challenge of the STM device was the spatial  distance between transistors. As one can seen in Figure 19 the  two center lines correspond to overlapping TRPE emission in  this PICA image. For each TRPE channel photons coming  from the transistors located to the left and right must be  removed (bias signal). This underlines the role of spatial  correlation step. The second limitation comes from the low  voltage used (1.2 Volts). As a result the quantum efficiency  will be extremely low. With regular TRPE (one dimension) or  PICA (three dimensions) techniques low voltage translate into  long or very long acquisitions. We have again chosen to  display PICA data in order to give a good scale for  comparison of STPC-3D with regular processing: Better  results are obtained after 40 minutes of acquisition instead of  leudoue|ysoaewojqxeo udjurs duel)qqne(e upe yeJs degelu osaoni)tuaeu(joJoydu 18


80 hours. This corresponds to a time reduction of 120 – two


29


orders of magnitude. For on dimension TRPE analysis we  believe that from 1 Volt or lower, STPC-3D starts to add  significant value.


A general problem with category 1 bumps arises from the  geometrical dimensions of the UBM stack. Due to chemical  consumption of the UBM constituents, discontinuities in  coverage of the bump die contact interface result. This  manifests itself as a contact resistance problem during testing. Fig 4 is a SEM  picture of  a bump associated with a pin  identified as failing  contact resistance tests. The part failed  after 312 hours of reliability testing at 150C.  The arrow in the


Fig 1. Typical output from the bump-mapping


program that automates mapping of solder


bumps corresponding to failing pins in a


tester data-log. Several tens of bumps (in


dark blue) can quickly be identified from over


a thousand possible bumps.


Fig 2  Delaunay triangulation of a randomly generated set of points ( in blue). This triangulation technique is the basis of automated  pin identification.


Fig 3  Screen shot  from program developed to identify bump numbers and corresponding pin-names.


The identification is based on Delaunay triangulation.


SEM picture highlights discontinuities in the UBM stack


which results in contact resistance issues.


Continuity (opens) issues arise when the volume of the


category 1 solder bump is insufficient to ensure good electrical


continuity between the solder bump and the ceramic package


via. An example of a open’s failure that can arise as a result  is


documented in Fig 5. The arrow in this figure points to the


open interface at the junction of the bump and ceramic 超超盐盐盐盐package via.


|...n a..|盘||
|---|---|---|

|U|ALOO|. . . ...|

|Die |Metallization ||

CR


odtH


01


Category 2  solder bump defects.


We have already mentioned that in category 2 solder


bumps the UBM is constituted by a thick copper stud and a


thin TiW layer. In this section we document defects that


can afflict any one of the several interfaces present in this


multi-layered structure. Fig 6 shows a solder bump in


which the Aluminum cap between the TiW layer and the  chip metallization is damaged (arrow). In this case the  Aluminum cap is damaged only on a section of its length, but this defect still constitutes a reliability issue.  The part  had undergone 8 hours of burn in.


Fig 7  documents a category 2 solder bump defect which


resulted in every pin of the device failing opens test. Crosssectional analysis of the bumps revealed that the solder bumps  of the device did not make any electrical contact to the die due  to an intervening layer that remained un-etched during  assembly. The layer normally protects the passivation of the  die and is etched out in those areas where contact has to be  made to a solder bump. On this device the layer remained  everywhere and caused an opens failure. Fig 8 compares the  acoustic signal captured with the transducer centered on a  normal bump( in blue) with that of defective bump (in red). There is a section of the signal from the anomalous bump that  dips below the signal from the normal bump and is highlighted  in the figure.


Fig 4. SEM image of  a solder bump die


interface with a discontinuity ( red arrow) in


the underbump metallization. This caused a


contact resistance problem.


Fig 5. SEM image of a solder bump, package via interface with a discontinuity ( red circle). The open interface is a consequence of insufficient solder


volume.


Tin –lead solder bump.


Fig 6   SEM image of a solder bump where in the


Aluminum cap between the TiW and die


metallization was damaged.


Fig 7  SEM image of an unetched layer between the


solder bump TiW and die that caused the pin to fail


opens testing.


Copper UBM layer


Al cap


The copper stud of the category 2 solder bump is also  vulnerable to diffusion and hence chemical consumption. Reliability studies indicate that the copper would begin  dissolving into the solder leading to gradation in the copper  stud composition. This dissolution process continues until  there exists no distinct copper stud. In the final limit the  copper depleted interface opens up and this results in an opens  failure. The sequence described above is illustrated in Figures  9 , 10 and 11. In Fig 9, the part was subjected to a 375 hour  bake prior to burn in. The gradation in the composition of the  copper stud is clearly seen in the backscatter SEM image .


The part in Fig 10, has been subjected to 96 hours of burn in. A distinct copper stud is no longer present in the solder bump. Finally in Fig 11, the open interface that results when the part


04-


is subjected to 391 hours of burn in is documented. The TiW


YF


layer is now no longer in contact with the solder bump and a


02-


open interface has developed.


nwsm


01-


an


2-


公司


05F


Acoustic signals from the solder bump in the three stages are  compared  in Figures 12, 13 and 14. The differences between  the acoustic signals corresponding to the solder bump with the  graded copper stud and no distinct copper stud may be  attributed to the different sequence of interfaces presented to  the acoustic beam as it traverses down the solder bump stack. The dip at the beginning of the acoustic signal corresponding  to the bump with the open TiW solder interface can be


Fig 8. Acoustic signal from a good bump ( blue)


compared with the signal from a bump with the


unetched layer( in red). The dip in the signal of the  defective bump is indicated.


Fig 9 SEM image showing gradation in


copper stud after part was subjected to a 375


hour bake.


Fig 10. SEM image of a solder bump in which no distinct copper stud is observed. Part had been subjected


to a 96 hour burn in.


Fig 11. SEM Image showing an open TiW, solder interface that results when the part is subjected to 391 hours of burn in.


attributed to the fact that the acoustic beam experiences a


reduction in material density as it traverses the die, TiW solder  bump interface.


0.2-


0.4-


0.1-


0.3-


0pnn


0.2-0.1-


-0.1-


-0.2-


-0.3-


-0.2


0.45-2 -1.5-1-0.500.5


-0.3


025首-15-1-0500.511.522.5x107


04


In Fig 15  the copper stud solder bump interface  is open and  the associated pin fails opens testing. The reason for the open  copper stud, solder interface can be surmised by noticing that


there is solder leaking into a crevice at the interface between  the underfill  and the ceramic substrate. This crevice drains


at


solder from the bump ultimately causing the opens failure. Fig  16 compare the acoustic echo from a good solder bump (in  blue)  and the bump with the open copper stud solder interface ( in red). The negative going peak in the defective solder  bump is highlighted.


11.522.5


八 J4-05


02-0


J'--4*


5-


Fig 12. Acoustic echo from a solder bump with a graded copper stud.


Fig 13. Acoustic echo from solder  bump with  no  distinct copper stud


Fig 14. Acoustic echo from a solder bump with an open TiW solder bump interface.


Fig 15 : SEM Image showing an open solder bump ,


copper stud interface. A crevice at the underfill,


-04


substrate interface drains solder from the bump.


Fig16 : Comparison of acoustic echoes from a normal


solder bump ( in blue) and a solder bump with an


open copper stud , solder interface ( in red). The


negative going peak in the defective solder bump is


highlighted.


台


萌


Validation of a design is not always possible with fault


Weight


diagnostic tools. Some defects may be inaccurately defined or


古


not modeled at all. Time resolved photon emission (TRPE) of  the device can compare measurements with simulations to  dramatically reduce validation and debug time.


We have developed a new method for optimal CAD autochanneling to generate virtual layers containing areas (TRPE  transistor channels) where photon emission emissions are


123


56


expected. The generated file does not contain any proprietary


x 104


information about the technology and can be sent directly to  analysts using TRPE thereby solving the two limitations of  accessing the CAD layout: proprietary issues and resources  involved with extremely large files.


Our approach not only speeds up the analysis process but


Temporal histogram after frequential noisecut for chip n* 184


also reveals the necessity of considering not only one


transistor but also its neighbors which also contribute to the


18


photon emission measured signal. This contribution is taken


16


into account in our CAD auto-channeling technique. Consequently, comparison between TRPE measurements and


14


simulations results in a better match.


iz


Finally, we have demonstrated the application of CAD  auto-channeling for the spatial temporal photon correlation


Weight古


(STPC-3D) technique to extract signals from noise from the


8


first few photons of a TRPE acquisition.


6


[1] J.  C.  Tsang J.  A.  Kash and D.  P.  Vallett, "Picosecond  Imaging Circuit Analysis", IBM J.  RES.  DEVELOP.44 (2000)


of234567B Sample nummer


[2] V.  Fischetti, S.  E.  Laux and E.  Crabbé, "Understanding HotElectron Transport in Silicon Devices: Is There a Shortcut?", J.  Appl.  Phys., vol.  78, No.  2, pp.  1058-1087, 15 July 1995


[3] R. Desplats et Al., “Automated Pica Transistor Channeling and  Spatial-Temporal Photon Correlation for Faster Ic Diagnosis”, IRPS2003.


[4] R. Desplats, T. Dargnies, J-C. Courrege “Automatic  determination of optimal FIB operations for improved circuit  probing and fast reconfiguration”, ISTFA, 12-16 November  2000 Seattle (USA).


[5] R. Desplats et Al., “Fault Localization using Time Resolved  Photon Emission and STIL Waveforms”, ICT, September 2003.


[6] A. Eral, “Spatial Temporal Photon Correlation STPC-3D”, CNES internal report. June 2003.


Rajen Dias • Intel Corporation. Chandler, AZ


# Session 3: Package Level Analysis 1


p 56-61


DOI: 10.1361/cp2003istfa056


## 3D X-ray Computed Tomography (CT) for Electronic Packages


3D X-ray Computed Tomography (CT) for Electronic Packages


Zezhong Fu, Deepak Goyal* & Jeffrey Thomas


Intel Corporation, CH5-263,  5000,  W. Chandler Blvd., Chandler, AZ 85226, USA


Alan Crawley & Andrew Ramsey


X-Tek Systems Ltd., 64-66 Akeman Street, Tring, Hertfordshire, HP23 6AF, U.K.


Next generation assembly/package development challenges  are primarily increased interconnect complexity, density, and  multi-layer/multi-stacked packages with ever shorter  development time.  The results of this trend present some  distinct challenges for the analytical tools and techniques to  support this technology roadmap.  The key challenge in the  analytical tools and techniques is the development of nondestructive imaging for improved time to information. The 3D  X-ray Computed tomography (CT) system named “X-Tek  NGI” has been co-developed by Intel and X-Tek to address  this need.  The current paper will discuss the configuration and  several applications where this tool has been applied  successfully to solve current package technology development  issues and provide package construction analysis (including  enabled components). This paper will discuss the details of the  system configuration, examples together with the current  limitations and future direction for non-destructive package  failure analysis.


The key drivers for the non-destructive imaging, results of  literature search and evaluation of key analytical techniques  currently available have been discussed in detail in reference


[1].  Requirements of a 3D imaging capability and critical  breakthroughs required for development of such a capability  have been summarized [1].  In order to address this capability  gap it was identified that the standard assembly imaging  techniques of x-ray radiography/Tomography need to be  extended into the next generation.  For x-ray techniques, goals  of 1-micron maximum spatial resolution and z-axis resolution  with geometric magnification of >1000X appears to be  attainable based on theoretical specifications from several  industry vendors. Generally there is a trade-off with reduced


S--AP SOURCE


sant


DETED OR


spatial resolution and poorer contrast when the x-ray  penetration is increased.  The use of a transmission signal for  standard x-ray radiography (2D-imaging) precludes viewing  subtle defects such as C4 (controlled collapse chip connect) bump fatigue cracking and BGA (ball grid array) solder ball


fatigue cracking in the multi-layer interconnects packages.  Thus 3D-imaging capability has been identified as a must have  for detection of the defects mentioned above.


The primary driver for 3D x-ray Tomography is the need to  have sub micron resolution in X, Y, and Z planes while  maintaining high geometric magnification to detect submicron sized defects.  Package fail mechanisms such as C4  and BGA solder fatigue, Cu migration and trace cracking, micro voiding in C4 and BGA solder joints all present  challenges to non-destructive imaging due to the small size of  the defect (typically <1micron) and the complex geometries of  the packages such as multi-layer stacks and materials resistant  to x-ray penetration (for example thick Cu heat sinks, dense  solders and multi-layer interconnects).


Several years of development work between Intel and X-Tek  has resulted in the Next Generation 3D Computed  Tomography x-ray (X-Tek NGI 3D CT X-ray) tool being  developed.  This equipment is the first of its kind and has  tremendously enhanced the package FA (failure analysis) capabilities at Intel.  This tool is capable of producing  reconstructed 3D models of x-ray images that can be  manipulated and sliced to view the plane of interest nondestructively. This tool has achieved the milestones of  resolution (<1µm resolution) and magnification (>1600X in  2D mode).


Figure 1.  Schematic representation of a typical CT  configuration.  X-ray source and detector remain stationary.  Sample is rotated in X-ray field of view.


X-ray  source


Sample 妇


True CT, as shown in Figure 1, has also been demonstrated. This has enabled the non-destructive inspection of defects  such as C4 bump bridging, bump cracking and study of solder  ball (BGA) defects and geometries.


This paper will discuss several applications where this tool has  been used successfully to solve current package technology  development issues and provide package construction  analysis. The examples presented will include non-destructive  cross-sections of C4 bumps to reveal the depth and geometry  of the defects and 3D images of the multi-stacked die  packages and multi-layer interconnects. Several of these  results were not obtainable by other analytical methods  including destructive cross-sectioning. While there has been  significant progress in the development of the 3D CT  applications there are still several factors limiting the success  of this technique that need to be addressed. These examples  will be discussed in detail together with the current limitations  and future direction for non-destructive package failure  analysis.


System configuration (X-Tek NGI 1)


The X-Tek NGI has several key features that distinguish it  from the rest of the commercial x-ray market. The equipment  is capable of performing ‘Real Time Microfocal Radiography’ as well as 3D or ‘Volumetric Computer Tomography – (CT)’. Microfocal Radiography refers to the ability to view a  magnified x-ray image of an x-ray transparent object.  First, the electron source for the NGI is produced by a thermionic  Lanthanum Hexaboride (LaB6) filament vs. a Tungsten  filament, which is typically used for x-ray applications.  The  LaB6 filament produces a smaller diameter electron beam  which results in a smaller spot size at the target, which in turn  improves resolution.  The LaB6 filament also has a much  higher brightness (10X) when compared to a typical Tungsten  filament while running at a much lower temperature (1700 deg  K) as compared with 2600 deg K for a standard Tungsten  filament. This has two advantages, (1) there is less thermal  spread of electron velocities, which makes for better focusing  and (2) allowing shorter exposure times and greater image  contrast thereby also promoting longer filament life. In  addition the anode power is ~2 watts. The second and most  distinguishing feature of the NGI is in the way the data for the  3D models is collected – true CT mode.  Most 3D x-ray  systems use a Laminography technique in which the sample  typically remains still while the ‘focal point’ of the x-ray  source and detector are synchronously moved in the X-Y  plane resulting in a collected series of off-axis 2D images, as  illustrated in Figure 2.


The 2D images are combined to form a 3D model in which the  area of interest is in sharp focus and the surrounding areas are  blurred. This allows the end user to focus on specific planes in  the package with reasonable clarity; the main disadvantage is  the artifacts caused by the blurring of surrounding layers. The


CT technique (as shown in Figure 1) involves physically  rotating the sample while capturing 2D images at predetermined θ increments.  The 2D images are re-constructed  to render a true 3D model showing all internal features.  No  data or focal area is blurred out and the resultant 3D model  can be manipulated to clearly see any internal plane from any  viewing angle. Other distinct features of the system are a 6  axes manipulator, a digital detector, and custom designed  software for 3D CT reconstruction of the micro-electronic  applications. While, some or many of these features can be  found in other systems, this system remains unique in the way  all of the above features have been brought together in one  tool.


Figure 2.  Schematic representation of typical digital  laminography system configuration.


As previously mentioned, several successful applications have  been demonstrated with X-Tek NGI 1 tool.  These results will  be discussed in the following section.


Failure Analysis Applications


Figure 3 shows a CT reconstructed image of C4 solder bump  shorts (Sn/Pb) failure that was a result of the assembly  process.  The objective of the analysis was to show a clear xray view of the failure without physically cutting through the  area of interest (locally non-destructive).  The failure was  isolated on the sample by hand probing and the sample was  trimmed to a workable size (~3mmx3mm) for CT imaging.


This is an example of a fairly low resolution scan (>20u  feature resolution) which required ~1.5 hrs to acquire and  reconstruct the data.


SnPb solder


Plane 1


Plane 2


Complete view  of package


Au wirebonds


Plane 3


Plane 4


BGA


Plane 5


Plane 6


C4


Via  stack


PTH


Package


Layers


Figure 3.  3D CT image showing C4 bump short.


3D Modeling


3D x-ray models have also been used to correlate between  topographic views (such as achieved through planar grinds) and cross-sections.


CT imaging of multi-layer/multi-stacked die packages have  been evaluated and found to be very promising. Various  features such as Au wire bonds, µ-BGA, and other package  features at different Z layers have been clearly imaged using  CT techniques.


Figure 4.  Schematic of a multi-layer/multi0stacked die  package showing multi-stacked die and multiple layers of  interconnects.


Figure 4 shows a schematic of a multi-layer/multi-stacked die  package while, Figure 5 shows CT imaging of this package  type. Figure 5 below illustrates the capabilities of CT in  resolving different planes and features of interest shown in  Figure 4.  As previously discussed, once a 3D CT model is  complete, it can be manipulated to view any internal plane at  any viewing angle. The same CT model can be used to view a  selected area of interest from both grindback and cross-section


perspectives. Package information such as multiple layers of  interconnects, and multiple routing features can also be clearly  illustrated using the CT technique.


Figure 5.  The images above show the view of various planes  in the multi-layer/multi-die stacked package corresponding to  the planes marked in Figure 4 above. The features of interest  are also noted in these planes.


Figure 6.  CT reconstruction illustrating a package features  including package via, PTH and C4 bumps.


Figure 6 illustrates a package internal features including the  C4 bump interconnect and the multiple layers of Cu routing  and inter-layer connections (package via) and plated through  holes (PTH).


Construction analysis of complex structures such as packages  mounted on sockets that have been BGA mounted on PCB can  also be performed using the CT technique. Figure 7 illustrates  a CT model of a socket used to mount a pin grid array package  on the printed circuit board (PCB). The 3D X-Ray imaging  was useful in detecting open contacts between pin and socket


Plane 1  Plane 2 Plane 3


Plane 4  Plane 5  Plane 6


socket


Pin


by having the ability to rotate the reconstructed image to view  the open location.


Figure 7.  3D CT image of the socket used for mounting the  package to a PCB. The key features illustrated here are the  socket contacts with the package pin, the BGA and the PCB  PTH.


Figure 8.  3D CT images demonstrating C4 bumps, package  via and chip capacitors mounted on the PCB. Also the bottom  image shows the entire thickness of the PTH and the package  via in 3D mode.


Figure 8 above shows a 3D CT model of a C4 package  mounted on a PCB. Adjacent to this are a few chip capacitors  and they are also evident in this 3D model. In addition the  package PTH and via as well as C4 bumps are also clearly


imaged. These images demonstrate the effectiveness of the 3D  CT imaging in non-destructively identifying different features  and failure mechanisms (if present) on the packages and  packages mounted on PC boards.


Based on the above results, usefulness of x-ray tomography  for non-destructive imaging of both package defects and  features has been demonstrated. Also, as shown in this section, the X-Tek NGI phase 1 tool has been successfully applied to  various aspects of failure analysis and package level  construction analysis.  The X-Tek NGI system represents the  state of the art 3D X-ray tomography capabilities that were  designed with package failure analysis needs in mind.


Limitations of the current system:


In 2D, magnification of  >1600x is achieved by having the  sample as close to the x-ray source as possible while keeping  the detector as far from the source as possible. Conventionally, the requirements of CT require that all the angular views of  the sample be included, during the full rotation of the sample  in the beam. For this to be achieved, it is usually necessary to  move the sample away from the source – so as to achieve full  rotation within the beam. However, the result of moving the  sample away from the source results in lower magnification.  Geometric Magnification is given by the ratio of  (d1 + d2)/d1  as shown in Figure 9.


0 0


SO


Source


Figure 9. Magnification calculation in X-ray imaging. This  figure also illustrates the difficulty in obtaining high  magnifications in the CT mode with large samples, as the  sample to source distance (d1) has to be increased.


CT acquisition requires that the entire sample be kept in the  field of view as it is imaged throughout 360° of rotation.  This  requirement increases the source to object distance due to the  space needed for sample rotation.  This means that although  the resolution of the system still meets specification (<1u), the


Via


d1 **


d2


Feature of interest


Detecto r


d1


magnification is not adequate to detect the smaller defects due  to the large source-to-object distance necessary to rotate the  sample in the X-ray field of view.


CT imaging also requires adequate x-ray penetration through  the sample from all angles of rotation.  Dense materials such  as solders (Pb and Sn) and heat sinks (typically Cu) add to the  difficulty of achieving this x-ray penetration.  In addition to  the penetration and geometry concerns, throughput time (TPT) is quite long (typically 3 hours) due to the extensive image  corrections, and calculations needed to perform CT. The short  term solution to the problems with x-ray penetration and  sample geometry have been resolved by physically trimming  the sample size down to something more suitable for CT  acquisition (3x3mm is typical).  For current CT system (XTek NGI 1 or phase1 system) capabilities, it is more useful to  think of defect size vs. sample size rather than absolute  resolution.  Typical defect detection is ~5micron to 10 micron  when the sample is trimmed to 3mmx3mm for image  acquisition.


Challenges for Next Generation X-ray imaging  Development


Region of Interest (ROI) CT System:


To meet the dual requirements of imaging a relatively large


object and achieving micron-scale resolution in the region


of interest, a “region-of-interest (ROI)” CT scanner is


proposed for the package level applications. There are


several approaches (including the one suggested by


Nalcioglu, et al. [2]) that need to be investigated and the


best solution for the package level inspection with multilayers of interconnects needs to be identified.


It is well established that if the CT scanner does not cover  the entire object under inspection, the features of the object  outside the field of view cast artifacts into the reconstruction  region. First acquiring a low resolution CT data set of the  entire object and then acquiring a high resolution data set for  the region of interest may eliminate this effect.  The x-ray  attenuation due to objects outside the region of interest  would be subtracted from the region of interest projections, making possible an artifact free reconstruction of a small  field of view within the larger object.  This is schematically  illustrated in Figure 10.


The Region of interest CT scanner concept has several  important advantages:


• It will greatly reduce the size of the image data set by  requiring micron-scale sampling only in the region of  interest.


• Performing low resolution imaging over a large sample  followed by high resolution ROI imaging over a fine  sampling region may result in reduced data acquisition  time. For 3-D images the data acquisition time is roughly


proportional to the reciprocal of the voxel size, or the  reciprocal of the detector spacing cubed.


• It will greatly reduce the image reconstruction time by  constraining the high-resolution reconstruction to the  region of interest.


• It will permit the use of a low intensity micro-focus x-ray  source for the region of interest while permitting the use  of a high intensity larger anode spot x-ray source for the  remainder of the object.


It will greatly reduce the detector cost by limiting the  sample volume (number of pixels required is significantly  reduced).


Figure 10.  A schematic diagram of an ROI (Region-ofinterest) CT scanning system.


The development of the current tool took several years and  strong efforts from several participants including X-Tek  and Intel. Based on the above results, usefulness of x-ray  tomography for non-destructive imaging of both package  defects and features has been demonstrated. A variation of  the traditional approach has been suggested to overcome the  limitations of the current system and meet the challenges of  a high resolution and low throughput time CT imaging  system. A region-of-interest CT scanner system is  suggested to meet the high resolution, low throughput time  need.


In this method a coarse scan is completed for the entire  object, then a second fine resolution scan is conducted for a  specific region-of-interest. Reconstruction algorithms, with  subtraction of objects outside the region of interest, will  need to developed as well to make it possible to reconstruct


Full Field of View


Region of Interest


Fine Sampling Coarse Sampling


the small volume, artifact free. Although, a lower power  micro-focus x-ray sources may be used for the region of  interest, a higher power source may be necessary for the  coarse scan depending on the materials in the IC package. This will also require development of sources that will meet  the needs of ROI scanning. Hence, it is clear that this may  require significant development in the fields of both  hardware and software for an ROI imaging system.


The authors would like to acknowledge Gay Samuelson, Bruno Clark, Martha Neustadt, and Ruth Deacon of Intel for  their support. Additionally, the authors would like to thank  Roger Hadland of X-Tek Systems Limited for various  discussions.


1. D. Goyal, “X-Ray Tomography for Electronic  Packages”, Proceedings of the 26th International  Symposium for Testing and Failure Analysis, 2000, p


49.


2. Nalcioglu, et al. “Limited Field of View Reconstruction  in Computerized Tomography,” IEEE Transactions on  Nuclear Science, Vol. NS-26, No. 1, 1979.


p 62-67


DOI: 10.1361/cp2003istfa062


## High- Angle Electron Microscopy Technique for Analysis of Thin Film Contamination on IC Package Exteriors


High-Angle Electron Microscopy Technique for Analysis of Thin Film  Contamination on IC Package Exteriors


Thomas Barbieri*, Jake Schaper*, and Pete Dimuzio†


Motorola Semiconductor Products Sector, 2100 E. Elliot Road MD EL315, Tempe, AZ 85284, USA  *Arizona Product Development and Analysis Laboratory


†


Radio Products Division


Yield loss during final evaluation was occasionally associated  with low level leakage current between neighboring pins on a  Motorola IC product. A series of simple experiments on reject  samples indicated that the source of the leakage was on or near  the package surface and likely to be due to a conductive film  on the backside of the package between the leads. A technique  was developed to detect and analyze the film using high tiltangle and low accelerating voltage on the SEM and EDS. The  shallow penetration depth of the electron beam permitted  observation of a thin and continuous film on the backside of  the failed package. Likewise, the EDS sampling volume was  constrained to the outermost layers of the specimen surface, such that a significant signal was generated from the identified  film, even at low accelerating voltage. An EDS line scan  across a surface region containing the film resulted in an  excellent correlation between increased levels of metallic  elements gold and copper and the presence of the film.


There are numerous analytical techniques for determining the  presence and composition of contaminant surface films (SIMS, Auger Spectroscopy, FTIR, XPS, cross-sectional  analysis [1]). However, some of these techniques are  destructive to the sample; some require extensive sample  preparation, and some require long periods of time for data  acquisition. When visual inspection with compositional  analysis and rapid turnaround time is required, one usually  thinks of Secondary Electron Microscopy (SEM) in  conjunction with Energy Dispersive Spectroscopy (EDS). However, such analyses are commonly performed at  accelerating voltages ≥10 kV and with stage-tilt angles ≤45º. These operating parameters result in electron sampling depths  of one micron or greater [2], which is not favorable for surface  thin-film analysis. Under such circumstances, the majority of  the probe electrons would not be sampling a suspected surface  contaminant layer, and any image or X-ray signal coming  from this layer would likely be hidden within a stronger signal  coming from the bulk material below the layer.


It is well known that accelerating voltages of ≥10 kV are  usually necessary to generate strong enough EDS signals from  a specimen to yield significant results. However, performing


EDS analysis at lower accelerating voltages (1.5-5 kV) can  yield significant advantages. Such advantages include greatly  improved spatial resolution, heightened volume sensitivity, and more accurate detection and resolution of emitted X-rays  from light elements [3]. Additionally, non-conductive  specimens usually require a conductive surface coating (Au, AuPd, C) be applied prior to analysis to prevent surface  charging. Surface charging is a phenomenon that occurs  within non-conductive materials when electrons from the  incident electron beam cannot be conducted out of the sample  and build up within the area under examination. Charging is  characterized by extremely bright areas which are difficult to  image due to excessive contrast. Such electron buildup also  results in the generation of an electrical field that affects and  can distort the incident electron beam, and as such can cause  image distortion and drift [4]. Charging is usually prevented or  eliminated by the application of thin layer of conductive  material, such as Au or C, which is sputtered or evaporated  onto the surface of the specimen. Unfortunately, applying such  a coating to the surface would be an obvious hindrance when  searching for a thin-film contaminant on the surface, especially when the possibility exists that the contaminant  could be composed of the same elements as were used to  generate the surface coating. Furthermore, the X-ray signal  from the coating could overlap and obscure a more important  signal from the surface contaminant.


Sample case: Defect localization


The procedure described in this paper was developed during a  failure analysis investigation of an IC product assembled  within a leadless package. Yield loss during final evaluation of  these parts is continuously monitored to identify cost  improvement opportunities.  Failures were occasionally  observed to have low level leakage current between  neighboring pins.


The sleep current test for the IC utilizes two adjacent device  pins, which are a digital circuit source VDD and digital circuit  ground.  The device is programmed into a sleep mode state  and the current is then measured through the digital source  VDD pin referencing the digital circuit ground pin.  Acceptable sleep current operating range is between 100ua to  800ua. Suspect surface contaminant devices exhibited sleep  current >4ma.  The sleep current test was highlighted because  it is one of the first tests performed in the final test program.


Other functional tests of the IC also failed on suspect surface  contaminant devices.


It is important to note that all pins on this package are  susceptible to the surface contamination.  Any artificial  connection (leakage) between pins would cause an increased  current reading and other possible functional failures. A series  of simple experiments in surface level cleaning on reject  samples, including ultrasonic cleaning in an acetone bath, DI  water rinse, and vacuum oven bake-out, resulted in  improvement (reduction) in the current measurement. These  results indicated that the source of the leakage was on or near  the package surface and gave rise to a theory that a conductive  film existed on the backside of the package between the leads. Unfortunately, visual inspection using an optical microscope  did not reveal any indication of such a layer. Figure 1 shows  an optical micrograph of the surface of a bad specimen versus  a good specimen. No anomalies are observed on the bad  specimen. A quick and simple analysis was therefore required  to confirm the existence of the proposed layer before  venturing on to more thorough and time-intensive analytical  techniques.


High energy analysis


SEM analysis was performed on a JEOL 6301 FESEM  mounted with an EDAX “Phoenix” EDS system. Initial  analysis of failed specimens was performed using an  accelerating voltage of 10 kV. One specimen was sputtercoated with a thin layer of gold to prevent charging and to  assist with imaging and EDS analysis. Since construction of  the lead bumps in the package involves a gold layer, (see  Figure 2) there was a possibility that the contamination layer  could have been composed of gold due to some variation in  the manufacturing process. Therefore, a second specimen was  left uncoated to eliminate any confounding of the EDS data. Visual identification was not made of a surface layer during  inspection of either specimen; however, the charging behavior  of the uncoated specimen lent some credence to the proposed  existence of a conductive surface layer. As can be seen in  Figure 3, extensive surface charging has occurred on the  specimen due to the high accelerating voltage and lack of a  sputtered surface coating. Even so, areas of the surface  adjacent to the lead bumps are dark and are not charged up at  all, suggesting the presence of a conductive material that has  prevented incident electron build-up by conducting them to  other areas of the package (perhaps to the lead bumps and into  the internal circuitry of the device). This lack of charging  around the bumps is not observed on passing parts.


EDS analysis was also unsuccessful in detecting the presence  of any significant contamination on the surface of a failing  specimen relative to the surface of a passing specimen. Figure  4 shows a comparison of EDS spectra collected under  identical conditions from a failed specimen and a passing  specimen (both specimens were gold-coated). The two spectra  are identical in appearance and do not contain any elements  beyond what was expected (oxygen, carbon, aluminum, and


 EDAX, Inc; 91 McKee Drive, Mahwah, NJ, 07430


silicon are all components of the mold compound, and the  gold signal is from the sputtered conductive coating).


200 μm


Figure 1: Optical images collected from  the mold compound  surface of a passing part (a) and part suffering from sleep


current leakage (b). The object on the right side of each image  is the edge of a lead bump. No differences are observed.


Figure 2: Cross-section of package lead bump, showing  construction layers.


Unfortunately, EDS analysis at 10 kV of the uncoated  specimens was unsuccessful due to excessive charging and  image drift.


gold


palladium


nickel


palladium  Mold compound


1mmF1 L01


1mm F1 L01


AZPDAL10KVX2014mm


AZPDALT0RvX2014mm


Figure 3: Top-down views at 10kV accelerating voltage of a passing part (left) and a part suffering from sleep leakage current (right). Charging is evident on both parts, however a significant portion of the surface remains uncharged around the lead bumps of the


failing part.


Si


C


Al


PdSb


HUHNfrpe-atleteau wlahreaded man hsa


wdo aan


Ni


0.80


2.40


3.20


4.80


5.60


6.40


7.20


8.


PdSbdnnh


|0.80|160|2.40|3.20|4.00|4.80|5.60|I 6.40|7.20|学 8.|
|---|---|---|---|---|---|---|---|---|---|

|Figure 4: EDS spectra collected from the package surface of a passing part (top) and failing part (bottom), using an acce |Figure 4: EDS spectra collected from the package surface of a passing part (top) and failing part (bottom), using an acce |Figure 4: EDS spectra collected from the package surface of a passing part (top) and failing part (bottom), using an acce |Figure 4: EDS spectra collected from the package surface of a passing part (top) and failing part (bottom), using an acce |Figure 4: EDS spectra collected from the package surface of a passing part (top) and failing part (bottom), using an acce |Figure 4: EDS spectra collected from the package surface of a passing part (top) and failing part (bottom), using an acce |Figure 4: EDS spectra collected from the package surface of a passing part (top) and failing part (bottom), using an acce |Figure 4: EDS spectra collected from the package surface of a passing part (top) and failing part (bottom), using an acce |Figure 4: EDS spectra collected from the package surface of a passing part (top) and failing part (bottom), using an acce |Figure 4: EDS spectra collected from the package surface of a passing part (top) and failing part (bottom), using an acce |

leration


voltage of 10 k and 0° stage tilt. No significant differences are observed between the two spectra. Specimens were coated with a thin  layer of gold to assist with SEM analysis.


Low energy, high-angle analysis


We were able to by-pass many of the obstacles of working at  standard conditions by using a high-angle, low energy  technique. Accelerating voltages of 1.5-3 kV have sample  depths a factor of ~5-15 less than at 10 kV with constant tilt


[2], resulting in greater sampling of the surface relative to the  bulk. By tilting the specimen to an angle of 60°, an even  greater volume of near-surface x-rays and secondary electrons  will be generated (simulations of electron sampling volumes  are shown in Figure 5). Imaging a defective part under these  operating conditions instantly revealed the presence of a thin


and continuous film on the backside of the failed package. Figure 6 is a micrograph captured from a bad specimen at 60° and 1.5 kV. The surface contamination appears as a bright, broken (yet still continuous) film on the surface of the mold  compound. Since this image was collected using a Secondary  Electron Imaging (SEI) detector, the brighter contrast of the  film relative to the mold compound suggests a higher density  of electrons in the film as compared to the substrate, a clue  that the film may be metallic or composed of large atomicmass elements [4].


Passing part


Au


Failing part


Microns


Figure 5: Electron interaction volumes for (a) 10kV  accelerating voltage and 0º tilt, (b) 3kV accelerating voltage  and 0º tilt, (c) 3kV accelerating voltage and 60º tilt [5]


Figure 6: Low energy, high angle SEM image of specimen  surface, showing presence of a thin contaminant film


Interaction Volume Simulation


EDS analysis was necessary to confirm these suspicions. The


0.000


accelerating voltage had to be increased to 3 kV in order to


0.007


generate an appreciable overall signal, as well as to increase


0.014


the possibility of exciting and generating characteristic X-rays  from a greater variety of potential elements. A general rule of


0.021


thumb is to use an accelerating voltage set at a factor of 1.3


S0.028


greater than the energies of the characteristic X-rays the


10.0350七


researcher is attempting to generate[3], therefore a slight  increase in the accelerating voltage significantly increases our


N0.042=


chances of exciting the elements within the contaminant layer


0.049-


without increasing our sampling volume much farther below


0.056-


the surface. An EDS spectrum was collected from an area of  mold compound between two lead bumps where the surface


0.063-


film was observed on the SEM. These two lead bumps also


0.0700.0350.028 0.021 0.014 0.007 0.000 0.007 0.014 0.0210.028 0.035


demonstrated low level leakage currents between them during  final test. An EDS spectrum collected in this region, shown in  Figure 7, revealed the presence of copper and gold (note that a


sputtered gold coating was not applied to this specimen).


At  this point, EDS mapping of the area in question is usually


0.000-


performed in order to qualitatively verify the results. An EDS


map uses color coding to display element distributions within


a SEM image, presenting the analysis data in a format that is


easy to interpret by the casual reader. However, a high quality  map normally takes anywhere from one to several hours,


s0.028 u


depending upon numerous factors such as accelerating


0 I 0


0.035


voltage, probe current, and desired image quality, and this


N0.042。


only applies to maps generated with accelerating voltages of  10-30 kV. At <5 kV, the detected X-ray counts-per-second


0.049 -


(CPS) are much too low to generate a quality EDS map within


a reasonable period of time, especially within a typical failure


analysis lab where there may be one electron microscope for  multiple users.


0.0700.035 0.028 0.021 0.014 0.007 0.000 0.007 0.014 0.021 0.028 0.035


In this situation of low energy EDS collection, an EDS line  scan provided the confirmation that the foreign film was  indeed the source of the previously detected gold and copper  signals. Instead of collecting data from an entire field at one  time (as is the case with an EDS map), a line scan is a function


Lead bump


Brighter,


0.050-


broken film


0.100


0.150


S0.200 a


N0.300÷


0.350-


0.250


0.400-


0.450-


100Pm国L01


0.5000.250 0.200 0.150 0.100 0.050 0.000 0.050 0.100 0.150 0.200 0.250


AZPDAL 1.5KVX37013mm Die edge


0X


CuL


SiKAuM


|0.30|0.60|0.90|120|150|1.80|2.10|2.40|2.70|3.|
|---|---|---|---|---|---|---|---|---|---|

|Figure 7: EDS spectrum collected from region containing the contaminant film. Accelerating voltage was 3 kV. D |Figure 7: EDS spectrum collected from region containing the contaminant film. Accelerating voltage was 3 kV. D |Figure 7: EDS spectrum collected from region containing the contaminant film. Accelerating voltage was 3 kV. D |Figure 7: EDS spectrum collected from region containing the contaminant film. Accelerating voltage was 3 kV. D |Figure 7: EDS spectrum collected from region containing the contaminant film. Accelerating voltage was 3 kV. D |Figure 7: EDS spectrum collected from region containing the contaminant film. Accelerating voltage was 3 kV. D |Figure 7: EDS spectrum collected from region containing the contaminant film. Accelerating voltage was 3 kV. D |Figure 7: EDS spectrum collected from region containing the contaminant film. Accelerating voltage was 3 kV. D |Figure 7: EDS spectrum collected from region containing the contaminant film. Accelerating voltage was 3 kV. D |Figure 7: EDS spectrum collected from region containing the contaminant film. Accelerating voltage was 3 kV. D |

etected  characteristic X-rays include the Carbon, Oxygen, and Silicon K-series, the Copper L-series, and Gold M-series.


built into EDS software systems that performs a series of point  scans at locations equally spaced along a linear path, with the  operational parameters of the electron beam held constant. Figure 8 shows the location and direction of a line scan  performed over the surface, sampling the contamination film  at numerous locations. The operating parameters for this scan  are listed in Table 1. The generated line scan data is charted in  Figure 9. The correlation between the line scan data and the  SEM image is excellent; both a copper signal and a gold signal  are detected in areas with the film, and the signal vanishes in  areas without the film. These results confirm that the thin film  is indeed composed of copper and gold and is likely  conductive enough to be the cause to the leakage currents  between the lead bumps.


10PmF3L01 Table 1: Operational parameters for EDS line scan used to AZP0AL 3.0KUX75013mm


generate data shown in Figures 9 and 10.


|EDS Line Scan Settings ||
|---|---|

|Accelerating Voltage = 3.0 kv ||

|Emission Current = 12 µA ||

|Probe Current (maximized) = 0.6-1.2 nanoA ||

|Data points collected = 1000 ||

|Time Constant = 100 µs ||

|Dwell Time = 2000 millisec ||

As is the case for EDS maps, an EDS line scan can monitor


and record the signals from multiple elements and save them


for further manipulation by the user at a later date. As an


example, during the execution of the line scan which


generated the plot shown in Figure 9, characteristic X-ray 0112132425364748595106116127138148159169signals from carbon and oxygen also were collected. This data  could not be plotted alongside the raw data from copper and


gold, as the CPS of carbon and oxygen dwarf those of copper


and gold. However, when the copper and gold data is


normalized and plotted with carbon, as it has been in Figure


10, it is observed that the carbon signal tracks inversely with


the copper and gold signals. This suggests that wherever the


thin film exists, it inhibits the detection of carbon. This signal


attenuation indicates that the characteristic X-rays emitted by


Figure 8: Location of EDS line scan which passes across  areas with the surface film and regions without. The arrow  shows the direction of progression of the scan.


Figure 9: Quantitative line scan results from region shown in  Fig. 8. Region of line scan is embedded in the chart to assist  with direct comparison. Note increasing signals from Au and  Cu correlate well with the presence of the surface film.


carbon had to pass through the copper and gold layer before  reaching the detector. In other words, it confirms that the


0 ectedts detcoun510152025


distance (microns)


Cu Au


Figure 10: Normalized EDS line scan data, showing how the  carbon signal from the mold compound tracks inversely with


the copper and gold signals.


metallic film lies on top of the packaging material.


As a final verification of these results, an identical analysis  was performed upon a passing part from a manufacturing lot  that did not suffer any of these defects. Under SEM  examination at low accelerating voltages, the contamination  layer seen on the failing specimen was not observed. High  angle, low voltage EDS point scans and line scans using the  procedure described above failed to detect any significant  copper or gold signals from the surface across a distance of  120 microns. It was concluded that the copper-gold layer was  not present on this specimen.


Additional analysis on failing parts and passing parts  reinforced the initial results. In a matter of a few hours, we  were able to provide strong evidence that parts from lots that  suffered from sleep leakage currents between lead bumps  exhibited a thin layer of conductive metals on the backside  surface of the package. Both of the detected metallic elements  are present during final manufacturing of the failed devices, so  their presence in the contamination layer was not unlikely. With this evidence in hand, it was now considered prudent to  proceed with further, more time consuming analyses to obtain  an accurate compositional and dimensional profile of the  contamination layer in order to determine final root cause and  eliminate it. At the time that this article was written XPS  analysis had already confirmed the presence of these metallic  elements, as well as several others, including tin, palladium, and chromium.


Summary


By combining high stage-tilt angle, low accelerating voltage


SEM imaging with low voltage EDS measurements, rapid


results can be obtained in the search to detect thin film


contamination layers on specimen surfaces. The improved


spatial resolution of low energy analysis performed with a


properly calibrated instrument allows for excellent correlation  between the line scan measurements and the visual images.


This technique has since continued to prove useful for analysis


of other thin films and small surface particles. It is also ideally  suited for situations where specimen charging is likely at the  higher accelerating voltages often necessitated by EDS, but


usage of a conductive coating (Au or C sputter) is undesirable.


1. L. C. Feldman and J. W. Mayer, Fundamentals of  Surface and Thin film Analysis, P T R Prentice Hall  (1986)


2. P. Hovington, M. Lagace, D. Drouin, and R. Gauvin,


1228


L


l


Electron Range at Low Energy (Eo<10 KEV): Atomic  Number Dependant?,  Microsc. Microanal., 8 (Suppl. 2), 704CD-705CD (2002)


3. E. Boyes, Pros and Cons of Low Voltage SEM EDX  Elemental Analysis, Microscopy Today, v11 #1, 5-10 (2003)


4. M. T. Postek, K. S. Howard, A. H. Johnson, and K. L. McMichael, Scanning Electron Microscopy: A  Student’s Handbook, Ladd Research Industries (1980).


5. Electron Flight Simulator, manufactured by Small  World and distributed by SPI Supplies, ver3.1 (1987).


850100150200250


p


i


o300350


400


Cu normalized Au normalized


p 68-75


DOI: 10.1361/cp2003istfa068


## Solder bump defects in ceramic flip chip packages and their acoustic signatures.


Solder bump defects in ceramic flip chip packages and their acoustic  signatures.


Kartik Ramanujachar, Darwin Rusli, Reena Agarwal, James Widaski


Texas Instruments, 12203 South West Freeway, Stafford, Texas 77477.


Solder bumps are frequently the sites of defects that cause  continuity failures in ceramic flip chip packages. In concurrent  technology the solder bump is a multi-layered structure  containing several interfaces. Conventional c-SAM imaging  alone cannot delineate subtle bump defects. In this article we  present experimental results that document the nature of  interface defects in multi-layered solder bumps as well as their  acoustic signatures. The acoustic signatures obtained from  defective bumps are contrasted with the signals obtained from  pristine bumps and the sensitive nature of these signatures to  defects is highlighted.


Concurrent  ceramic flip chip packages for high performance  microprocessors can have hundreds of solder bumps. These  multilayered bumps are often sites of continuity issues with  the package. In this contribution we attempt to document the  defects that arise in the  solder bumps of microprocessor  ceramic flip chip packages.


This article is divided into three distict sections. The first  section concentrates on automated bump identification. In this  section techniques that we have developed to rapidly identify  solder bumps for physical failure analysis, given failing pinnames from a tester data-log are discussed.  In this section a  novel triangulation technique for bump identification is  illustrated. In the second section we present results of physical  failure analysis on solder bumps identified as anomalous  during testing of microprocessor packages. In this section we  also present acoustic signals obtained from many of these  anomalous bumps and contrast the same with normal bumps. A number of SEM micrographs are presented which document  the multitude of defects that can afflict a solder bump and lead  to continuity failures.  In the final section we present results of  transfer matrix simulations that attempt to model the acoustic  frequency response of bumps wherein defects have been  computationally introduced. These results emphasize the  sensitive nature of the frequency response to bump defects. Preliminary results obtained by analyzing actual acoustic  signatures with wavelet-based techniques are presented.


Section 1: Automated bump identification.


Physical failure analysis of continuity failures begins with the  identification of solder bumps that correspond to failing pins  documented in a tester data-log.  This task would typically  involve identifying a few to several tens of solder bumps from  over a thousand possible bumps. Automated identification  enables quick targeting of suspect bumps for both nondestructive analysis (using Scanning Acoustic microscopy  (SAM) and X-Ray) and cross- sectional sample preparation. In  this section we discuss two techniques.  The first addresses the  issue of generating bump maps with suspect bump solder  bumps highlighted given failing pin names in a data-log. The  second solves the issue of obtaining pin-names and bump  numbers corresponding to any given bump in a bump map.


Automating the generation  of a bump map containing  suspect bumps from a tester data-log.


Tester data-logs of pins failing continuity testing may contain  a few to several tens of pin names. When a few pins are  involved manual identification of corresponding solder bumps  is feasible but this is impractical when more that 10 failing  pins are involved.


The approach we have used to tackle this problem is the  following. A look up table of all solder bumps co-ordinates  and their corresponding pin-names is generated.  Obviously  such a look up table is part specific, so  look up tables have to  be generated for all the different devices that potentially need  to be analyzed. The look up table in essence ties a pin name to  the x-y co-ordinate of  the corresponding solder bump. The  tester datalog is then extracted with a script that identifies  failing pin names and outputs these names in a format  compatible with that used for pin–names in the look up table. The formatting of the pin-names is essential as the names  assigned to the pins in tester data-logs often differ from the  source used to generate the look up table. With the failing pin  names extracted from the datalog,  vectorized string matching  alogorithms are used to match failing pin-names with x-y coordinates from the look up table. The x-y co-ordinates so  identified can be used to generate a bump map of suspect  solder bumps. An example is illustrated in Fig 1.


1210*


08油:


0.


-0.2-*


-0.4


-06


-0.8


雪-0.80.6-0.4-0.200.20.40.60.8


Mapping solder bumps to corresponding pin names.


Often during the analysis of package cross- sections we need  to quickly identify the pin-name corresponding to a given  solder bump.  This problem is the converse of the problem  addressed in the previous section. We have solved this  problem with a geometrical construct referred to as Delaunay  triangulation. The concept is illustrated in Fig 2. Delaunay  triangulation of a set of data-points ( in this case the solder  bump x-y co-ordinates) is accomplished by constructing  triangles whose vertices consist of three chosen points such  that the circum-circle of that triangle does not enclose any  other point in the original collection.


0.9


00-g


0.7


03


咕0.1020.30.4 0.5 0.6 0.7 0.8 0.9


An automated pin identification program has been developed  around this triangulation concept. The program utilizes the


look up table of x-y co-ordinates discussed in the previous  section and displays a bump map. When a bump is selected, the co-ordinates of user input are captured and used to identify


from the look up table, the bump closest in x-y co-ordinates to


the user input, a task achieved through Delaunay triangulation. Fig 3 show a screen captured from the program. Both pin  names and bump numbers can be quickly identified.


Bump


x一


Number


1683


Pin Name


vdd


-09


11 -0.50


0.51 x 104


start


Section 2 : Solder bump defects and their


acoustic signatures.


In this section we present the results of cross-sectional  analysis on solder bumps identified as suspect using the  techniques described in the preceding section. In many case  we also present acoustic signals captured with the acoustic  beam of a Scanning Acoustic Microscope(SAM) centered over  the bump of interest. We have analyzed ceramic flip chip  microprocessor packages with two distinct varieties of solder  bumps. These two distinct classes of solder bumps differ in the  chemical constitution and thickness of their under bump  metallization (UBM). In the first category of solder bumps, the  UBM is a copper, a refractory diffusion barrier, Aluminum  stack only a few hundred Angstroms thick. In the second  category of solder bumps  the UBM is constituted by copper  and Titanium Tungsten with the overall thickness approaching  several microns. All solder bumps are tin, lead based.  We  document defects at several interfaces in the both categories of  solder bumps.


Category 1 solder bump defects.


In today’s electronic industry of shrinking circuit boards and  shrinking semiconductor integrated circuits (IC), semiconductor companies have to be creative in providing  devices with more circuitry on less silicon.  One consideration  that has to be taken into account is the power dissipation of the  smaller IC that requires high power supply voltages.  BOAC/COA processes allow routing and bonding to thick top  level metallization on the LinBiCMOS (LBC) technology  node.  Thick metal top Copper increases the current carrying  capacity of the metal lines to the external pins.  The two major  benefits of  stacking the thick Copper on top (BOAC/COA) are: 1) it decreases the line width needed in the lateral  Aluminum metallization underneath and, 2) the ability to stack  Copper vertically  helps decrease real estate and  results in  reduced chip size (Figures 1-2).  Moreover, top Copper metal  lines can also be used anywhere as interconnecting circuitry or  Copper over anything (COA).  Although there are similarities, BOAC and COA represent two different processes.  BOAC  represents growing copper over any underlying Aluminum  metallization, which required external access to a node of  interest.  COA represents Copper over anything but bonding to  the Copper top layer is not necessary.  In other words, COA is  a process that can provide an extra metal level.  In this paper, we will refer to BOAC process, but the reader should know  that similar failures are seen on both processes.


Figure 1: Optical image of a decapsulated conventional die.  Bond pads are distributed on the perimeter of the die, and no  BOAC.


Figure 2:   Optical image of a decapsulated BOAC.  Arrows  point to bond pads, which are located far inside the die, and  Copper traces, which provide interconnection between Metal  lines.


From the Failure Analysis (FA) point of view, in addition to  the typical failure mechanisms associated with die fabrication, testing, packaging and abnormal biasing, BOAC raises some  new challenges for FA: 1. BOAC metal covers much of the  underlying active circuitry. This restricts not only visual  inspection, but also photon emission during Photon Emission  Microscopy (PEM or EMMI) analysis. 2. Liquid Crystal  Analysis is greatly hampered not only by the inherent heat  dissipating characteristics of the thick copper metal itself, but  also the addition of a tremendous amount of heat during  normal power operating conditions (most BOAC parts are  high power devices).  This makes hot spot isolation difficult at  best.


It is important for FA to draw the distinctions of whether the  defect comes from biasing conditions (customer related  issues), packaging related issues, bond wiring issues, COA/BOAC process issues, fab processing issues, or design  issues.  The focus of this paper will be the identification of the  COA/BOAC process related issues as a root cause for failure.


In this paper, FA techniques and approaches on un-passivated  BOAC will be discussed, and a generic BOAC/COA process  will be explained.


BOAC/COA Process


BOAC/COA process1 begins with a finished device fabricated  with a Silicon Nitride (Si3N4) protective overcoat (PO).  Via  openings in the PO are then etched to the top native layer  metal. This will allow the interconnect path to the Copper top  metal. A Titanium-Tungsten (TiW) barrier layer is then  deposited across the wafer followed by the deposition of a thin  Copper (Cu) seed layer. Next the thick photo-resist is  patterned and then Copper is plated to the Copper seed layer.  In the BOAC, a Nickel (Ni) layer then added protects the  Copper from corrosion and allows the formation of a good  inter-metallic to the Gold ball bond.  Palladium (Pd) on top of  the Nickel protects the Nickel from oxidation and is easily  displaced during the bonding process.  Copper seed pattern is  then etched out (Figure 3).  Bonding wires can be bonded  directly to the PdNiCu traces (Figure 2).  The device is then  subjected to packaging without further passivation.  For the  COA process, step 5 may not be necessary, because there is no  bonding to the Copper top layer.


Figure 3: Overview of BOAC process.  Step 1 is the finished  die.  Step 2 is the Copper contact patterning.  Step 3 is the  deposition of the Copper seeded TiW layer.  Step 4 is the  plating of the Copper Bonding.  Step 5 plates another Ni and


Unit I


Unit 2


Pd for bond ball contact.  Step 6 is the removal of Copper


SLAA


seeded TiW layer.


AUNDaKI


0Om


Carwent


Commert


Un-passivated Copper traces posed a challenge to


decapsulation step for FA.


Approach to Failure Analysis (FA) for BOAC


FA for BOAC follows the traditional FA process of package  inspection, failure verification, I-V curve trace analysis of all  pins, decapsulation, failure re-verification, visual inspection, fault isolation, defect identification, and root cause analysis (Figure 4).  A more detailed description of a FA process flow  can be found in the ASM’s Microelectronic Failure Analysis  Desk Reference Fourth Edition2, written by Seshu Pabbisetty.  The paper will follow the FA process flow in Figure 4.


Figure 4: Failure analysis process flow.


Failure Verification/Curve Trace


Phatoresist


SI3N4 Overcoat


Cu Seed


The first step in FA is to verify the reported failure.  Failed  devices from internal or external customers are subjected to  failure verification.  This is normally accomplished using a


见


bench test setup recreating the failing mode.  The purpose of


Metal Buses


failure verification can also be identifying the related failure


3


circuitry.


Cu Bond


Bonding laerface


Removed


The next step is the I-V (Current-Voltage) curve trace


Cu Seod


analysis.  Similar to any metal-metal failures, failures  associated with BOAC often result in continuity failures,


Tr


shorting or leakage between pins (Figure 5).   Once the failure  has been confirmed, the failed device is then inspected for any


package related damage.  The curve traces in Figure 5 are  actual results from known cases of TiW bridging.  Both early  breakdown and resistive shorts between pins can be an  indication of BOAC issues.


Figure 5:  I-V characteristics comparison between a known  Good device and a failed device.  Both units have the same  pin-to-pin failure.  Curve trace on the left (Unit 1) indicates  early pin-to-pin breakdown.  Curve trace on the right (Unit 2) indicates a pin-to-pin short.   TiW bridging was subsequently  observed in both of units.


Failure  Verification


Bench Test


Package  Inspection


Optical, SAM, & X-ray


Curve Trace


Analysis


Decapsulation


Nitric/Sulfuric


Die Inspection


Fault Isolation


EMMI, LC, etc.


Defect Identification


Optical Insp., Deprocessing, FIB, SEM, etc.


Root Cause  Analysis  Re-verification


Package Inspection-Non Intrusive Analysis


After the failure verification step, a package integrity  inspection is done.  This consists of an optical inspection of  the package, Scanning Acoustic Microscopy (SAM) analysis  for package delamination, and X-ray imaging analysis of  bond-wires.  Depending on the severity of the BOAC failure, package delamination resulting from the shorting in the  BOAC metal, is frequently observed during SAM analysis.   This is due to mold compound overheating near the shorting  area.  As shown in Figure 6, package delamination can be  observed directly above the TiW bridging of Copper BOAC.


Figure 6: Scanning Acoustic Microscopy image.  Square  encloses the delamination area directly above a TiW bridging  of BOAC.


High resolution X-ray imaging can also be used to inspect  BOAC Copper traces.


The next step after package inspection is decapsulation.  Most  package materials are made from plastic mold compounds, for  example, Plastic Lead Chip Carrier (PLCC), Plastic Quad Flat  Package (PQFP), Thin Quad Flat Pack (TQFP), SOIC, etc.


The standard package material removal procedures use  chemical etches such as concentrated Nitric and/or  concentrated Sulfuric acids at high temperatures.  During  decapsulation of BOAC parts, Nitric acid alone was shown to  rapidly attack the Copper metal.  Nitric acid is a much  stronger oxidizing agent than Sulfuric acid 3.  It was also  found that concentrated Sulfuric Acid will attack the Copper  metal, but at a much slower rate.  These attacks will  compromise a device’s functionalities by increasing resistance  on the Copper top bonding metallization.


Empirical testing resulted in a solution to the metal attack  problem.  A ratio mixture of Nitric to Sulfuric acid was found  to not compromise the speed of decapsulation yet significantly  reduce the rate of the Nitric attack on the Copper.  Decapsulation of BOAC parts has been highly successful


using this procedure. It was also discovered that a quick drop  of fuming Sulfuric after decapsulation can also clean up minor  residue trapped between the copper traces.


Once a part has been decapsulated successfully, detailed  inspection of the die is necessary for any obvious BOAC  related issues.


Visual inspection may be done using both optical and  Scanning Electron Microscopy (SEM) to check for obvious  anomalies and any surface residue associated with BOAC.


BOAC process related issues, such as TiW bridging, which  result in low Ohmic failures and electrical overstress (EOS), can be seen optically with careful examination.


Case History 1


In a recent case, observation of the TiW can be seen  immediately after decapsulation.  SEM and Energy Dispersion  Spectrum (EDS) elemental analysis were used to further  confirm the presence of Titanium Tungsten (TiW) bridging (Figure 7).


Figure 7: Optical and SEM inspection reveals TiW bridging.


The introduction of COA/BOAC increases the level of  complexity for device fault isolation.  Since the Copper top  metallization covers much of the underlying circuitries, removing the Copper can result in a loss of functionalities.


Depending on the amount of BOAC, front side FA can  sometimes be accomplished with incremental Copper removal  using high ratio of concentrated Nitric to concentrated Sulfuric


acid at room temperature.  Ball bonding to Copper has been  found to remain good, with careful application of concentrated  Nitric acid to the BOAC device for less than 5 seconds.  This  is done to remove internal Copper traces that are blocking the  underlying active circuit.  Bear in mind that this will leave  intact the TiW barrier metal to continue the electrical paths, but the current carrying capabilities will be greatly diminished. Testing or fault isolation of the circuitry in this state can be  accomplished in a low power mode only.


Further FA can also be done selectively by internal probing  the circuitry after removing the Copper and TiW barrier metal  completely.   Hydrogen Peroxide (H2O2) is used to remove the  TiW layer.


Since much of the active circuitry is blocked by BOAC, FA  can also be done from the backside of the device.


Defect Identification/Root Cause Analysis


BOAC is a top metal layering, and most top level of the  metallization involves power supply circuitry.  Shorting of this  top metallization most likely will result in EOS damage.  Following EOS damage is package delamination, degraded  mold compound, metal re-flow, and damage to the  neighboring metallization.  EOS damage associated with  BOAC does not normally involve transistor level damage.


BOAC/COA Failure Mechanism


Some of the issues related to COA/BOAC have been found to  be from TiW bridging, Palladium bridging, mismatch of  Coefficients of Thermal Expansion (CTE’s) of Copper to  Aluminum, and bonding of Copper causing cracking in the  underlying metal and thus leakage.  Defects from the bridging  between the Copper top metal buses often yield Electrical  Overstress (EOS) signatures.  Differentiation of the EOS  caused by the COA process and biasing conditions can be  difficult.


Quantitative results


Failures resulting from TiW bridging, which causes shorting  between minimum pitch Copper bond traces, can be identified


%


after the proper removal of the package material.  As


Hom 140


mentioned above, TiW bridging would normally result in EOS  damage.  However, there are cases where TiW bridging can  cause functional failure.  Suspected TiW residue can be  observed by removing BOAC with Nitric Acid, which does  not attack TiW.  As well, EDS elemental analysis would be


ZOMAi 8BWXU00aub


done to determine the composition of the anomalies.


Case History 2


In this case, TiW bridging resulted in EOS damage in the form  of degraded mold compound (Figure 8).


us scae s8 as care 0000kw之


Depending on the magnitude of the failure and the current  clamp on the power supply, BOAC/COA related defects are  usually limited to the surface of the die and should not cause


damage far down to Polysilicon layer.   The sample in this  case was layer-layer deprocessed down to Silicon.  Damage  can only be observed at top level Aluminum metallization.


Figure 8:  TiW bridging results in EOS damage.  Arrows point  to EOS site and residual TiW.


Case History 3


An example of TiW bridging, which caused functional failure, is shown is this case.  TiW bridging resulted in power supply  leakages during the power up mode.  The TiW bridging was  detected through careful examination of the top level  metallization in the area of failing circuitry.  Further SEM  inspection and elemental analysis were used to confirm the  TiW defect (Figures 9).


During the un-powered mode, this low level of internal  shorting between the Copper top metal lines can not be  detected by external probing and curve tracing.  The failure  can only be seen under certain operation conditions, which  requires the activation of the involved Copper top  metallization.


kev


Figure 9:  Square enclose the area where elemental analysis  was taken.  Circle captures the large count of Tungsten (W) present.


Case History 4


In this case Palladium (Pd) bridging has been found to cause  shorting between Copper top bonding metallization.  A thin  layer of sputtered Palladium (Figure 10), not visible under  bright-field microscopy observation, however, was shown to  be etched away using concentrated Nitric and Sulfuric acid.  These parts that failed due to Palladium bridging often  recovered after package removal using Nitric and Sulfuric  etches.


The thin palladium re-deposition was found to typically cause  from 5kΩ to 100kΩ resistive shorts across the adjacent  Copper leads.  Because the thin Palladium film was easily  removed during decapsulation, fault isolation was limited  topside analysis at wafer level or backside analysis on  packaged parts.  The preferred technique on packaged parts is  to back grind the device through the die while monitoring the  resistive leakage failure.  Auger analysis was used to  determine the elements present between the mold compound  and the protective overcoat.  The creation of Palladium was  found to be from the re-deposition by a sputtering mechanism, during wafer plasma etch cleaning in preparation for ball wire  bonding.


Figure 10: Palladium redeposit during plasma bond pad  cleaning.


Case History 5


In the early part of the development of the BOAC process, mismatched Coefficients of Thermal Expansion (CTE) and  mechanical stress of BOAC were found to cause damage on  the underlying metallization.


In this case, BOAC CTE mismatch between the package and  the Copper created mechanical stress, eventually resulting in  inter-dielectric breakdown under thermal cycling.  The  package was placed under static stress from the start, since it  is encapsulated at 175°C.  At room temperature of 25°C, the  device is already -150°C from the point of encapsulation.


Most of the stress occurred at the edges and corners (boundary  conditions) of the Copper top metallization.


The break down of inter-dielectric resulted in extrusion of  underlying Aluminum metal lines and caused inter-metal  layers short.  Defects can be found using Liquid Crystal and  SEM cross section examination of the area immediate to the  Copper bonding (Figure 11).


Figure 11: Aluminum extrusion due to inter-dielectric cracks  from mechanical damage associated with mismatched  Coefficients of Thermal Expansion.  Aluminum extrusion can  be seen on top of protective overcoat, Si3N4.


Case History 6


In addition to mismatched CTE, Copper top exerted the  physical stresses downward and deformed the underlying  metal during temperature cycling. It was found that the  greatest damage was done and the most movement occurred  during the cold to hot transition during temperature cycling (Figure 12).


Figure 12: Stress induced damage to underlying metallization  and caused cracking and Aluminum extrusion between metal  layers.


Case History 7


BOAC can also affect the bond wire process.  Mis-bonding  can result in shorting between the ball-bond and neighboring  BOAC (Figure 13).  This failure resulted in a continuity


failure at test.  Curve tracing, proper packaging removal, and  SEM inspection were done to isolate the damage area.


Figure 13:  SEM image indicates shorting between ball-bond  to neighboring Copper BOAC.


While BOAC posts some challenges in terms of accessing the  underlying circuitry, these challenges can be overcome by the  use of combinations of Nitric and Sulfuric mixes and/or  Backside Analysis.


In Figures 17 and 18 solder bump shorts caused by  misalignment between the die and substrate is  illustrated. Due  to the shear forces exerted during the assembly operation the  solder bumps are misaligned with respect to the substrate  contacts (Fig 17). In an extreme instance of misalignment  solder bump shorts can result. ( Fig 18).


Section 3 :  Spectral analysis of  acoustic  signatures from solder bumps.


Acoustic signals from solder bumps contain valuable  information about the state of various interfaces encountered  by the probing ultrasonic beam. Unfortunately time domain  information in the acoustic signal is difficult to interpret due to  the presence of reflections from numerous interfaces and  concomitant convolution effects. In the concluding section of


this paper we discuss the possible use of spectral ( frequency)  domain information in the identification of  solder bump  defects prior to cross- section sample preparation.  In broad  terms this section attempts to highlight the utility of frequency  analysis by first exhibiting the results of transfer matrix based  simulations of the spectral response of computationally  introduced defects and secondly by displaying results obtained  using wavelet based analysis of  two spectra documented in  the preceding section.


Transfer Matrix simulation of the frequency response of  solder-bump defects.


The propagation of an ultrasonic wave through a multi-layered  structure in physical terms corresponds to the propagation of a  strain wave through the structure. The strain wave is reflected  at every interface that marks the periphery between layers of  differing density. The stresses that accompany the propagation  of the strain wave can be calculated by solving the waveequation.  One approach to the solution of the wave equation  is the transfer matrix approach that utilizes results from  potential theory[1,2]. In essence the propagation of the strain  wave is modeled by maintaining the continuity of stresses and  velocities at interfaces and relating the potential in one layer to  another via a transfer matrix whose elements are dependent on  parameters like material density, wave frequency, incidence  angle and material thickness. The transfer matrix approach  assumes invariance in the X-Y direction for wave propagation  in the Z dimension.


Figures 19 and 20 display the frequency response of  computationally introduced defects obtained using the transfer  matrix based approach on structures whose dimensions and  physical properties were chosen to reflect the transverse  dimensions of category 2 solder bumps. Attenuation effects  have not been taken into account due to the lack of physical  data, but can easily be incorporated into the calculation. In  both figures 19 and 20 the material stack considered for  simulation was constituted by the die (with metalization), solder bump and substrate. In figure 19 an air interface (crack) has been introduced at the interface between the Al cap layer  and solder bump. In Figure 20 a similar air interface has been  introduced at the interface between the die and the substrate. Of note is the distinct difference between the peaks in the two  spectra with the peaks shifting to higher frequency as the air  interface recedes into the structure.  This simple example  illustrates the benefits of frequency analysis of the acoustic  signals from solder bumps.


Spectral analysis of solderbump acoustic signals using  wavelets.


The nature of the acoustic echo with its non stationary power  spectrum suggests frequency analysis with basis functions  other than sinusoids (Fourier analysis) may reveal potentially  useful information. This possibility is explored in this section.  Wavelets enable frequency analysis with basis functions  chosen to match the temporal nature of the signal of interest  more closely than sine and cosine functions.


Fig 17: Solder bump substrate misalignment caused


by shear stresses applied during  service of the part.


Fig 18 Solder bump shorts that result when bumps are  extremely misaligned with respect to the substrate.


x10yrabnauoXi asdousaj oaoieoxe ps nqsiuetaq nud! uiaueoa 8


In addition wavelets circumvent the necessity to window the  time domain information as would be necessary with Fourier  analysis. In Figures 21 and 22 are presented some initial


cn


results with wavelet spectral analysis of the acoustic


un


signatures corresponding to solder bump defects shown in


Figures 11 and 15 respectively. In Fig 21 the wavelet


ID


coefficients of the acoustic wave corresponding to the defect


in Fig 15 is presented.  A Morlet wavelet has been chosen as  the basis for the coefficient computation. In the bottom section


of Fig 21 the wavelet coefficients are presented as a function


of the scale ( a parameter roughly analogous to frequency) . At  small scales the wavelet coefficients indicate the excellent


1922.12.22.32.42.56


similarity between the Morlet basis function and actual


frequency


x108


acoustic signal. It is also interesting to note that across a  number of scales in the low scale regime the wavelet  coefficients display similar structure indicating the fractal  character of the acoustic signal.


Fig 22 displays the wavelet power spectrum computed for


three different acoustic signals by averaging the wavelet


coefficients for the entire signal across all scales. This can be


conceptually thought of as analogous to the traditional Fourier 0


power spectrum. Two interesting observations can be made


about the wavelet power spectra. In concurrence with the


prediction of the transfer matrix calculation, the solder bump


-0.425-2-1.5-1-0.500.511.522.5 defect in Fig 11 (red curve) has a peak at a lower scale (lower


Absolute Values of Ca,b Coefficients for a = 1 234 5...x10-7 pseudo frequency) as compared to the defect in Fig 15 ( green


curve). In Fig 15 the air interface is on average deeper in the


structure as compared to that in Fig 11.  The power spectrum


of a good bump (black curve) is also shown for comparison.


e


This illustrates that power spectrum analysis is a sensitive way


to identify and classify solder bump defects.


time (or space) b


50100150200250300350400450500


We have discussed methods to automate bump identification  and exhibited a number of defects that can occur in solder  bumps of ceramic flip chip packages as well as their acoustic  signatures. The promise of wavelet power spectrum analysis  of the acoustic signature from solder bump defects has been  highlighted.


good bump


0.025


8X10年Frequency response for crack at Al cap bump interface


Bump-Die-int copper-solder-int


7


0.02 -


0.015-


on


0.01


reflectivityis w


0.005


0102030405006070


1.922.12.22.32.42.5


Fig 19 Transfer matrix calculation of  reflectivity when an air interface is introduced at the Aluminum  cap, solder bump interface.


Fig 20 Transfer matrix calculation of


reflectivity when an air interface is introduced


at the solder bump substrate interface


Fig 21 Wavelet transform of acoustic signal corresponding to defect shown in Fig 15. The similarity in structure of the wavelet coefficients of the signal at small scales can be clearly observed.


Wavelet scale


Fig 22 Wavelet power spectrum for three different acoustic  signals. The red curve corresponds to the defect in Fig 11  and the green curve to the defect in Fig 15. The black


curve  is from  a good bump.


The authors would like to acknowledge the many useful  discussions that they have had with other members at the  Houston Device Analysis Laboratory. Discussions with  Kendall Scott Wills, Omar Diaz Deleon, and Siva Kolachina  have greatly helped to formulate the material of this  contribution.


1. Folds D.L. , Loggins.C.D. “Transmission and reflection of  ultrasound waves in layered media” Journal of the Acoustic


society of America 62 (5) p 1102-1109 ( 1977).


2. Brouard B., Lafarge D., Allard J.F. "A general method of  modeling sound propagation in layered media", Journal of  sound and vibration (183), p129-42  (1995).


p 76-81


DOI: 10.1361/cp2003istfa076


## Copper Bond over Active Circuit (BOAC) and Copper over Anything ( COA) Failure Analysis


Copper Bond over Active Circuit (BOAC) and Copper over  Anything (COA) Failure Analysis


Dat Nguyen, Bob Davis, and Corey Lewis


Dallas Device Analysis Operation, Texas Instruments Inc., Dallas, TX, USA


Issues related to BOAC often result in EOS damage involving  degraded mold compound and Pin-to-Pin leakage.  These  typically show up as continuity failures at the ATE level.  Furthermore, the EOS damage does not propagate down to the  transistor level.  Consequently, continuity FA involving  BOAC technology is approached differently to preserve  Copper bonding.


Fault isolation involving BOAC requires the strategic removal  of Copper traces and selective analysis of the failed circuitry.  Liquid crystal and micro-probing have been used effectively  in failure isolation.  Furthermore, SEM/FIB/EDS/Auger are  required to make the necessary conclusion on BOAC related  failures.


Acknowledgment:


The authors would like to thank Taylor Efland and the TI’s  BOAC/COA (PDI) process development folks for their  valuable inputs into this paper.


References:


1. T. R. Efland et al., LeadFrameOnChip offers  Integrated Power Bus and BOAC Circuit,


Proceedings of 2001 International Symposium on  Power Semiconductor Devices & IC, Osaka, Japan.


2. J. Ross, C. Boit, D. Staab, Microelectronic Failure  Analysis, Desk Reference, 4th edition, p 3, ASM  International, Materials Park, OH, (2002).


3. R. Burns, Fundamentals of Chemistry, 3rd edition,  Prentice-Hall Inc., New Jersey (1999).


p 82-85


DOI: 10.1361/cp2003istfa082


## Investigation of Bond-pad Related Inter-metal Dielectric Crack


Investigation of Bond-pad Related Inter-metal Dielectric Crack


Z. G. Song, T. Tun, C. K. Oh, S. Redkar and B.H. Er


Failure Analysis Group, QRA, Chartered Semiconductor Manufacturing Limited


C. P. Soo and C. H. Goo


Yield Enhancement Department, CSP, Chartered Semiconductor Manufacturing Limited


Bond-pad is an important structure of a microelectronic  device because it plays the role of enabling the device to  communicate with other external devices. Its integrity  directly affects the performance of the microelectronic  device. This paper presents our investigation on bond-pad  Inter-Metal Dielectric (IMD) crack issue. Our  investigation has considered the following factors: top via  pattern (sea of vias/without vias) for bond-pad, top metal  thickness (8 kÅ /9 kÅ /10 kÅ) and probe overdrive force (30 um/50 um/70 um). The bond-pad IMD cracks were  exposed and decorated by chemicals (Aqua Regia and  Hydrochloric acid), and inspected by an optical  microscope. A scoring system was designed to assess the  dependence of the bond-pad IMD crack severity on the  above-mentioned factors. The investigation results  showed that the IMD crack severity is strongly dependent  on the probe overdrive force, top via pattern, and only  slightly on top metal thickness.


There are many issues related to bond-pad, for example, fluorine contamination causing bond-pad corrosion and  non-stick bond-pad, which have been well published [1, 2]. A bond-pad issue we encountered recently was  cracking of the  Inter-Metal Dielectric (IMD), which  caused infant mortality (IM) failure for several units. Bond-pad related IMD crack could be caused by probing  during wafer sort and wire bonding during assembly, and  is also dependent on the bonding process parameters. To  the best of our knowledge, there is no paper discussing  about the IMD cracking issue.


Our investigation on the bond-pad related IMD crack  issue was initiated by failure analysis for several units  suffering from infant mortality (IM) failure. When  compared with good units, the failing units had high  resistance for most pins. Initially, it was suspected that the  defect was due to an aluminum (Al)-gold (Au) intermetallic compound, which could be formed at the  interface between aluminum bond-pad and gold-bond-ball  at high temperature [3]. Cross-section was performed  through these bond-pads of high-resistance pins for a  packaged unit with such IM failure to investigate the  origin of these defects. Instead of the suspected presence


of Al-Au intermetallic compound, IMD cracking was  found underneath most of the bond-pads (see Fig. 1). A  second unit was decapsulated chemically and the goldbond-ball was etched away by Aqua Regia (3 parts of HCl (37%) : 1 part of HNO3 (69%)). IMD crack was again  observed at bond-pad area for most bond-pads (see Fig. 2). With other parametric study involving pre- and post  sort, final test after assembly and after IM stress testing, all other possibilities, such as resistive film on bond-pads, bond-pad metal corrosion, were eliminated except the  bond-pad related IMD cracks. Therefore, we believed that  the IMD crack was responsible for the high resistance of  most pins. Subsequently, we conducted a thorough  investigation to understand the root cause of the bond-pad  related IMD crack.


Fig. 1 Cross-section view of IMD crack underneath


bond-pad for an IM failing unit.


Fig. 2 Optical picture of IMD crack at bond-pad


area for another IM failing unit.


Experimental Procedures


The device is fabricated on 200 mm wafers with 0.18 µm  CMOS technology. It has two metal layers of Al(Cu) interconnect and one layer of poly. The IMD is a plasma  deposited oxide. The bond-pad size is 100 µm x 100 µm, with sea of vias connecting metal 1 to metal 2. The vias  are  0.36 µm with a  pitch of 1.2 µm. For analysis of the  bond-pad IMD crack issue, our investigation has  considered the following factors: top via pattern (sea of  vias/without vias) for bond-pad, top metal thickness (8 kÅ /9 kÅ /10 kÅ) and probe overdrive force (30 µm/50 µm/70 µm), which are believed to have  an impact on  bond-pad IMD crack. Table 1 summarizes the split  scheme for three wafers.


Table 1: Split scheme


|Factor |Level |Wafer ID |Wafer ID |Wafer ID |
|---|---|---|---|---|

|Factor |Level |1 |2 |3 |

|Top via pattern |Sea of vias |√ |√ |√ |

|Top via pattern |Without vias |√ |√ |√ |

|Top metal |8 kÅ |√ |||

|thickness |9 kÅ ||√ ||

|thickness |10 kÅ |||√ |

|Probe |30 µm |√ √ |√ √ |√ √ |

|overdrive |50 µm |√ √ |√ √ |√ √ |

|force ||√ √ |√ √ |√ √ |

|force |70 µm |√ |√ |√ |

0234387890123236蓝192028否82722382


☑


&


6异


861


Fig. 3 Wafermap showing the units with sea of vias


and without vias, and also the units probed


with different probe overdrive force (30 µm/50


µm/70 µm).


The wafers with different top via pattern and different  thickness of top metal were prepared in our Fab. The units  with different top vias pattern were fabricated in the same  wafer (see Fig. 3). The units without top vias were  realized by just skipping the photolithography step for top


via patterning. These wafers were then subjected to  probing with different overdrive forces on different row  of reticle field  using an in-house prober with tungsten  needles (also see Fig. 3).


After probing, these wafers were ready for bond-pad  related IMD crack checking. Since Aqua Regia was used  for removing gold-bond-ball for packaged unit analysis, to be consistent with packaged unit analysis, the waferlevel units were also etched by Aqua Regia for 15  minutes, followed by hydrochloric acid for 4 minutes at  room temperature. To easily quantify the severity of the  cracks, a scoring system with optical microscope  inspection is designed. The cracks in each bond-pad are  classified into two levels. Cracks in level 1 are narrow  and short (see Fig. 4 for example) and they will be  assigned 1 point each. Cracks in level 2 are wide and  long, or more than one crack line (see Fig. 5 for example) and they will be assigned 2 points each. Twenty-six bondpads have been inspected for each die. The total scores, representing the crack severity, are the sum of cracks in  level 1 plus twice of cracks in level 2 of the twenty-six  bond-pads.


Fig. 4 Example of optical picture of IMD crack in level 1.


Fig. 5 Example of optical picture of IMD crack in level 2.


PDAaProbe overdrive force: 70 um  296Probe overdrive force: 50 um  Probe overdrive force: 30 um


With sea  of vias


Without □vias


Figs. 6 and 7 show the probe mark and the resultant IMD


8 0


crack on two bond-pads. It is found that the location of


县


the IMD crack is correlated to the location of the probe


8 3


mark. For example, Fig. 7 clearly shows that if the probe


mark shifts from bond-pad center, the IMD crack  correspondingly shifts from the bond-pad center too. On  the other hand, the convex of the arc-shape crack is the  direction opposing  the probing direction. As shown in  Fig. 6, the probing drives from left to right and the convex  of the arc-shape crack is toward right, while as shown in  Fig. 7, the probing drives from right to left and  the  convex of the arc-shape crack is toward left. This  demonstrates that the IMD crack is caused by probing  during wafer sort.


Fig. 6 Optical pictures showing the probe mark and the


resultant IMD cracks on a bond-pad


Fig. 7 Optical pictures showing the probe mark and the


Total crack scores severity


Figs. 8, 9 and 10 are the plots of IMD crack severity  dependence on the probe overdrive force on the units with  sea of vias and without vias, and with top metal thickness  of 8 kÅ /9 kÅ /10 kÅ, respectively. It is clearly seen that  the crack became severer significantly when probe  overdrive force increases. This is expected, as stronger  probe overdrive force will exert higher stress onto the  IMD. It is also seen that the crack becomes worse for the  units with sea of vias. It is probably due to the presence of  vias, which are W ‘rods’.  These W ‘rods’ are very stiff  and tend to protrude from the IMD.  These W ‘rods’ experience the transmitted stress non-equally, making the  bond-pad IMD crack easily. This result implies that ring  of vias at bond-pad peripheral should be better than sea of  vias at bond-pad center in preventing bond-pad related  IMD crack.


0 1


10 X15 020人


35


30um


50um


70um


Probe overdrive force


Sea of vias Without via


Fig. 8 IMD crack severity dependence on probe


overdrive force on the units with sea of vias


and without vias. (top metal thickness of 8 kÅ)


0 5


0 e


8 S15 D20 025


S 5


8 n


Sea of vias


丬


Without via


Fig. 9  IMD crack severity dependence on probe


and without vias. (top metal thickness of 9 kÅ)


0 5 10 15 20 25 30


Fig. 10 IMD crack severity dependence on probe


and without vias. (top metal thickness of 10 kÅ)


Figs. 11 and 12 are the plots of IMD crack severity  dependence on the top metal thickness for different probe  overdrive force on the units with sea of vias and without  vias, respectively. One can see that there are more cracks  on the unit with top metal thickness of 8 kÅ when  compared to the unit with top metal thickness of 9 kÅ or  10 kÅ, while the crack severity does not varied much  between units with top metal thickness of 9 kÅ and 10  kÅ. For thinner top metal, such as of 8 kÅ, more IMD  cracks observed can be a consequence of lesser  cushioning from the bond-pad metal. When top metal  thickness reaches 9 kÅ and beyond (e.g. 10 kÅ), the  cushioning effect of the top metal may have been


saturated. Further study is needed to determine if a  threshold exists and why.


0 Total severity scores crack5 10 15*y20 25 30 35


8kA


9kA


10kA


Top metal thickness


70um 50um 30um


Fig. 11 IMD crack severity dependence on top metal


thickness for the units subjected to probing


with different probe overdrive forces (with sea


of vias)


scores severity crackTotal


10 15 20 25


Fig. 12 IMD crack severity dependence on top metal


with different probe overdrive forces (without


vias).


In comparing Fig. 3 and Fig. 4 with Fig. 2, it is  worthwhile to note  that the bond-pad IMD cracks are  severer for packaged units than those for wafer-level  units. It is because the wire bonding during assembly and  subsequent reliability test can make the existing minor  cracks, resulting from probing, worse.  The severe bondpad IMD crack will cause high resistance for the pins, leading to an IM failure.


In conclusion, the results from the present investigation  clearly show that the bond-pad IMD crack severity is  strongly dependent on the probe overdrive force, top via  pattern and only slightly on top metal thickness. Wire  bonding during assembly and subsequent reliability test  may make the existing minor cracks resulting from  probing worse. The severe bond-pad IMD crack will  cause high resistance for the pins, leading to an IM  failure.


1. D. Grman, R. Hauert, E. Hollander and M.


Amstutz, “Surface–analysis of Fluorine


Contamination on Microchip Bondpads”,Solid


State Technology, 35 (2), 43-47 (1992).


2. H, Y. Chen, Z. Q. Mo, L. H. An and Y. N. Hua,


“Application of Auger electron spectroscopy


and X-ray photoelectron spectroscopy analysis in


failure analysis of wafer fabrication”, Surface


Review and Letters, 8 (5), 435-439 (2001)


3. R. J. Gale, “Epoxy Degradation Induced Au-Al


Intermetallic Void Formation in Plastic


Encapsulated MOS Memories”, Proc. Rel. Phys.


Symp., 22, 37 (1984).


# Session 4: Sample Preparation 1 


Edward Keyes • Semiconductor Insights, Inc. • Ottawa, Ontario Canada


p 87-89


DOI: 10.1361/cp2003istfa087


## Enhanced SEM Doping Contrast


Enhanced SEM Doping Contrast


C.Y. Lin, J. H. Lee


Taiwan Semiconductor Manufacturing Company


Yield Enhancement Service Department.


No. 25, Li-Hsin Rd., Science-Based Industrial Park Hsin-Chu, Taiwan 300, R.O.C.


Scanning electron beams provide a superior method of failure  analysis by observing the voltage contrast (VC) both in frontend and back-end processes. Back-end VC tells us both  metal/via open/short issues. Front-end VC tells us not only  open/short issue but also additional doping information. A  case on the application of passive voltage contrast (PVC) on  doping information was studied. This paper explains the  mechanism producing passive voltage contrast and describes  three methods of sample preparation and provides examples of  the results achieved.


Passive voltage contrast was observed in Scanning Electron  Microscope (SEM) by Song et Al[1]. The SEM voltage  contrast comes from the electron-beam charging up the sample  surface, altering its potential and hence changing the  secondary electron (SE) emission kinetics. When the SEM low  energy electron beam scans a specimen, the specimen will be  charged-up positivily because the number of emitted SEs are  more than the primary incident beam in the absence of a  current path to ground[2]. These positive charges will set up  an surface electrostatic field and affect the behavior of the  emitted SEs.


For a P+ implant region, P+ and N-well form a diode. When  the SEM low energy electron beam scans, the beam induced  positive charges induce a positive potential on the P+ surface  region. When the accumulated potential is greater than the  forward voltage, the diode is turned on and the positive  charges will drain off to substrate through the N-well. Less  SEs are attracted back by surface potential and more SEs  reach SEM detector. This makes the P+ region brighter in  SEM images. For an N+ implant region, the N+ and P-well  also form a diode but vertically reversed to P+/N-well diode. As the electron beam scans, the accumulated potential reverse  biases the diode. Thus positive charges cannot not drain off to  the substrate. More emitted SEs are attracted back to the  surface and less SEs reach the SEM detector. So the N+ region  normally appears darker than the P+ region.


P+/P-wells and N+/Nwells do not from a diode like structure.  They are simply heavily doped  semiconductor which behave  like vertical resistors. Thus electron and hole characteristic  difference is the reason in SEM contrast. For a P+ implant  region, the beam induced positive surface charges drain off a


lot to substrate. Less SEs are attracted back by surface


potential and more SEs reach SEM detector. This makes the


P+ region brighter in SEM images. Besides, less surface


charges drain off to substrate in N+ area and appears  darker


then P+ area.


Secondary electrons (SEs) are sensitive to ionized dopant  distributions. The SEM could be used to view the dopant  profiles from semiconducting materials surface. Significant  contrast can be seen on freshly cleaved doped silicon, and it  has been found that contrast is enhanced after a chemical  treatment. This removes the oxide layer and passivates the  surface by saturating dangling bonds with hydrogen [3]. The  major purpose is to change the silicon surface state. Ammonium fluoride solution (5 grams of NH4F crystals in  30ml of water) is selected here because it has been shown to  produce an atomically flat surface [4] in comparison to HF, which is more commonly used for this purpose. In this study, the bare silicon samples are dipped in NH4F solution and the  SE voltage contrast is inspected in the SEM.


Experiment


In our experiment, a HITACHI SEM S4700 is our major tool. With its good in-the-lens SE detector, the SE image contrast of  different dopants is sharp and clear. We also set a standard  SEM operating condition to view the VC images for different  methods. That is accelerating voltage 1KV, emission current  15 uA.


In this study, 0.22um and 0.15um logic chips were used as  examples. We used three methods to prepare the samples for  P/N SE voltage contrast imaging on doped silicon regions. These are manual polishing, Ar-sputtering and wet solution  etching.


Manual Polishing


Manual polishing removes the layer above the silicon, then a  NH4F dip is the most convenient and easy way to remove the  remainder of the layer on the silicon surface. However, it is  very hard to prepare a precise position in a chip. Without  careful inspection, over-polishing or under-polishing would  lead to a failed sample preparation. Also the repeatability is  poor. Fig.1 shows the result.


Ar-Sputtering


After removing the layers above the doped silicon, we use Arsputtering to change the silicon surface state. The Ar-sputter  uses a High Density Plasma (HDP) like mechanism to  bombard the silicon surface, thus also slightly damaging the  implant region. This method produces the poorest results. As  we can see from Fig.2, only the N/P well contrast is shown. The implant detail is not seen at all.


Wet Solution Etching


The final is method uses wet solution to remove all the layers  above the silicon before dipping in NH4F solution to change  the silicon surface state. The advantage of wet solution etching  is its overall convenience. It is easy to handle and leads to a  great result. The most important advantages are its large  sample size and repeatability. As we can see from Fig3 and  Fig.4, very detailed implant information is showed, including  P+/N+, P/N well, N+- Nwell and P+-Pwell.


F8PEW同企


5ne32面


The results of the three methods are summarized and  compared in Table1. We find that the key to doping contrast  enhancement is to remove the layer above the silicon clearly  and effectively. Generally this layer is a metal-silicide  compound in the recent CMOS technology. Removing this  layer, we can change the silicon surface state in various ways. Here we studied three methods to change the silicon surface  state, and concluded that wet solution etching followed by a  NH4F solution dip is the best way to enhance SEM doping  contrast.


||Method |N/P Well |N+/P+ |Repeatability |Sample |
|---|---|---|---|---|---|

||Manual polish |Medium |Medium |Poor|size |

||Ar-sputter |Poor |Poor |Medium |Small |

Poor


Medium


Wet solution etching


Large  P-well


N-well


P+


回


N+ - N-well


P+ - P-well  N+


Fig.3 Wet etching SE image on a 0.22um TiSi product. All implant information is shown clearly.


Table1. Summary and comparison table of three  methods in this study.


N+ - N-well  n


P+ - P-well


N+


P-Well


Fig.4 Wet etching SE image on a 0.15um CoSi product. All implant information is shown clearly.


Fig1 Manual polishing and NH4F dip   on a 0.15um CoSi product.


N+/Nwell  MD


P+  川


N当


77%。ny


P+/PWell


P-well


Fig.2 Ar-sputtering on a 0.15um CoSi product.  Only the well information is shown.


P+  (N-Well)


N+  (P-Well)


1. Application of contact-level ion-beam induced


passive voltage contrast in failure analysis of static


random access memory


Z.G. Song, J.Y.Dai, S.Ansari, C.K.Oh, S.Redkar


Proceeding of 9th IPFA 2001  [103-106]


2. Simple calculation of energy distribution of lowenergy secondary electrons emitted from metals


under electron bombardment.


M.S.Chung, T.E.Everhart


I.Appl. Phys.  Vol45, pp707-709, 1974


3. Enhanced SEM Doping Contrast on an H    passivated Silicon Surface


S L Elliott, R F Broom, C J Humphreys, Cambridge


University, http://www-hrem.msm.cam.ac.uk


4. Comparison of Si(111) surfaces prepared using


aqueous solutions of NH4F versus HF


GS. Higashi, RS. Becker, YJ. Chabal, AJ.Becker,


Appl Phys Lett 58[15] pp.1656 –1658, 1991


5. Front-end processing defect localization by contactlevel passive voltage contrast techonique and root


cause analysis.


Proceeding of 9th IPFA 2002  [97-100]


p 90-98


DOI: 10.1361/cp2003istfa090


## Interconnect and Gate Level Delayering Techniques for Cu/ Low k Technology Failure Analysis


Interconnect and Gate Level Delayering Techniques for  Cu/Low k Technology Failure Analysis


Huixian Wu, James Cargo, Barry Dutt, Tony Bucha, and Joe Serpiello


Agere Systems, Quality Organization, Product Analysis Lab


Room: 20E-229A, 555 Union Blvd., Allentown, PA 18109, USA


Phone: 610-712-5998, Email: hwu7@agere.com


Abstract: In this paper, Failure Analysis (FA) challenges,


reliability issues, and new failure modes for copper technology


will be presented.  Deprocessing techniques for copper


technology have been developed and will be discussed. Front


side and backside FA deprocessing techniques for copper


layers and low k inter-level dielectric (ILD) layers including:


reactive ion etching (RIE), parallel polishing, chemical


mechanical polishing (CMP) and a combination of these


techniques will be discussed. In addition, novel gate level


deprocessing techniques will be presented.


1. Introduction


Copper interconnects and low k dielectrics have been  introduced in advanced IC technology to reduce the  interconnect resistance, improve the resistance to  electromigration and reduce RC delay and cross talk effects. The introduction of new materials in integrated circuits makes  physical failure analysis more challenging. Moreover, as  technology shrinks, defects can be smaller and more subtle, creating additional challenges for defect localization and  physical failure analysis. It is also increasingly important to  understand new failure modes and reliability issues related to  Cu/low k technology and develop FA techniques accordingly.


In this paper, several front side and backside deprocessing  techniques will be presented.  The deprocessing techniques  include wet chemical etching, RIE, parallel polishing, chemical mechanical polishing (CMP) and a combination of  these techniques. Characterization results of CMP  deprocessing will be presented as well as gate level  deprocessing techniques for Cu/low k devices.  Finally, some  case studies will be provided.


2. Failure Modes and FA Challenges


FA challenges will result from new failure modes and  reliability issues associated with the integration of Cu and low  k dielectrics, barrier metal and high k gate dielectrics. Soft  defects and non-visual defects associated with advanced


technology brings additional challenges for electrical defect


localization and physical failure analysis:


Some failure modes associated with the integration of copper  interconnect, low k dielectric and high k gate dielectrics include:


• Metalization level failure modes: copper corrosion, contamination, interface diffusion, electromigration, stress  migration, self heating, joule heating, stress voiding, copper  extrusion, via voiding, interface adhesion


• ILD failure modes: cracks, interface adhesion, delamination, moisture adsorption, intra-level and inter-level leakage, biastemperature instability, mechanical weakness, low thermal  conductivity, and breakdown of the low k dielectrics


• Gate level failure modes: breakdown of the gate dielectrics, soft  breakdown (SBD), stress induced leakage current (SILC), direct  tunneling, hot carrier injection (HCI), trap assisted tunneling (TAP), negative bias temperature instability (NBTI), interface  instability


• Integration issues: thermal-mechanical issues, interface  adhesion, CTE mismatch, chemical reaction, Joule heating  effects


As the technology continues to scale down, defect size tends to  decrease and as the circuits become more complex, subtle  statistical variations may become significant failure mechanisms


[1]. Thermal/electrical instabilities become more significant in  advanced technologies. Failure mechanisms, not visible with  microscopes, will occur more often in smaller technologies. Detection and characterization of non-visual defects will be an  FA challenge. Potential non-visual defects could be associated  with the following: NBTI (Negative Bias Temperature  Instability), Intra-level or Inter-level leakage (Especially for the  Cu/low k technology), instability with Cu/low k integration, high  resistance via or contact, stress induced leakage current (SILC), trap-assisted gate dielectric leakage current, gate induced drain  leakage current, sub-threshold leakage current, interface  instability related to high k gate dielectrics, Charge migration, short channel effects, interface adhesive problems and so on.


Copper interconnects are softer than aluminum and delayering  copper presents several challenges including maintenance of  global uniformity, dishing of metal interconnect, copper  smearing, and erosion of copper and dielectrics. For  delayering low k dielectrics, parallel polishing has limitations  due to non-uniform and low removal rate. The conventional  wet chemicals used for ILD etching are not suitable for some  low k dielectrics. RIE may be an alternative, however, there  are still some challenges for RIE of low k materials including  etch selectivity, RIE grass, surface roughness, and  optimization of the process parameters. In this work, several  deprocessing techniques for Cu/low k technology including  parallel polishing, wet chemical etching, CMP and RIE are  discussed.


3. Chemical Mechanical Polishing (CMP)


3.1 Deprocessing of copper metal layers -- CMP


Deprocessing of copper by CMP presents several challenges  to the FA analyst since copper is easily corroded is softer than  aluminum and smears easily while polishing. Figure 1 shows  an example of how copper smears when polished improperly. In addition, copper CMP can create defects in the inter-level  and intra-level dielectric materials. Particle contamination on  the polishing pad may result in severe scratches during  deprocessing.


In this work, different polishing parameters were characterized  and the process optimized. Figure 2 shows CMP deprocessing  of copper using an optimized process.


Figure 1. Image showing copper smearing


Figure 2. Image showing CMP of copper/low k sample


3.2 Characterization of CMP process


Patterned wafers were used for characterization of the CMP  process using parallel polishing tools from Allied  Technologies. The polishing parameters investigated include  slurry chemistry, polishing pad type, pressure, and pad  rotation speed. The type of slurry and polishing pad type  chosen play a significant role in the dishing, recess and  erosion performance. Several types of slurry chemistry and  polishing pads were investigated including 0.05 and 0.06  micron Colloidal Silica Suspension slurry, diamond slurry and  copper CMP slurry (Planar Solutions - CU10K2). Copper  CMP slurry works the best in our applications. Moreover, pad  rotation speed and pressure have a significant impact on the  CMP process. We found lower pad rotation speeds and lower  pressure can reduce problems in the CMP delayering process. Lower pad rotation speed and lower pressure avoids overpolishing of copper, thus reducing dishing and erosion.


The polishing time to remove the same amount of copper  material was recorded at different polishing conditions. Figure  3 shows the impact of pressure on polishing rate at different  pad rotation speeds. The copper layer was 300 – 400 nm thick.  A lower pad rotation speed (75 to 100 RPM) and a lower  pressure reading (0.1 mm) are best however this reduces the  polishing rate and takes more time. Therefore, a multi-step  CMP technique, with different polishing conditions, can be  extremely useful for deprocessing copper layers. Lower  pressure and lower pad rotation speed are used in the final step  to avoid over-polish of copper.


0 50


Polishing Time (seconds)


100 150 200 250


Pressure reading (mm)


75RPM


150RPM


100RPM


Figure 3: Polishing rate vs. pressure reading


4. Deprocessing of Inter-level Dielectric (ILD) Layers – Reactive Ion Etching


Agere 30.0kV 15.7mmOk SE(M) 6/21/02 15:151


With technology continually scaling down, the RC  propagation delays become dominant in the overall chip delay. Low k materials are being used for ILD materials so as to  improve the RC delay, and reduce the cross talk and power  dissipation, as well.


Several techniques such as wet chemical etching, parallel  polishing, and dry etching could be used for the delayering of  ILD materials for FA. The concerns for wet chemical are  isotropic etching and difficulty in controlling the etch process. Parallel polishing has limitations due to its non-uniform  process and low removal rate for low k materials.  With  technology continually scaling down, RIE may be an  extremely viable alternative due to certain advantages over  parallel polishing and wet etching. These include high spatial  resolution based on the anisotropy, high selectivity of the  etching process, capability of etching devices with much  smaller geometries and the ability of RIE to accurately control  the etching process. However, there is not much work reported  for RIE of low k materials for FA and many challenging issues


Agere 30.0kV 13.5mmx3.0K SE(U) 9/10312:472.31um


remain. These include but are not limited to etch selectivity, surface roughness, and the optimization of the process  parameters. Effective recipes for getting a clean surface, high


selectivity and high etch rate are necessary for carrying out


RIE of the ILD materials.


We have characterized the RIE process of low k dielectrics [2]. The optimized recipe for RIE of Black Diamond TM material is: CF4 of 50 sccm, O2 of 2 sccm, chamber pressure of 50 mtorr, RIE  power of 60 Watts and ICP power of 300 Watts.


With the optimization of the RIE process, high etch selectivity, low damage, and a clean surface free of RIE grass can be  achieved. Figure 4 and 5 show some SEM images of the RIE  deprocessing. The low k dielectric in Figure 4 and 5 is Black  Diamond TM material.


Figure 4.  SEM image of 0.13 um Cu/low k technology


Figure 5.  SEM image of 0.13 um Cu/low k technology


5.  Gate Oxide Integrity and Gate Level  Deprocessing


The ability to perform physical FA at the gate level has  become increasingly important with the increased number of  different potential gate level defects, such as soft breakdown  of ultra thin gate oxide, SILC, TAT. In this section, gate level  deprocessing techniques will be presented.


u(


5.1  Gate Dielectrics Integrity Issues


e With scaling of gate dielectric and introduction of high k gate 8e dielectrics, soft breakdown of the gate dielectric becomes a


serious concern for advanced CMOS technologies. In soft 3 breakdown, there is an abrupt jump of conductivity at the low


field but not at high field. Gate current is noisy after soft


breakdown, exhibiting a random telegraph type of noise behavior


[4].   Detection of soft breakdown is a challenge for the FA


process. Tunneling AFM (TUNA) is an ultra-low leakage current


imaging tool, that can be used for localization of gate level


defects, soft breakdown path, detection of dielectric thickness


variations, and study of gate dielectric integrity issues. To


perform TUNA on a failing device requires removal of the


polysilicon gate and exposure of the gate oxide.


High k gate dielectrics are being introduced due to the


unacceptably high gate leakage currents in ultra-thin


conventional gate oxide. With the introduction of high k gate


dielectrics, the stability of the high k/silicon and high k/poly-Si


interfaces become a serious issue and concern. High interface


defect density affects the device characteristics and reliability.


Mobility degradation and hot carrier charge trapping present


additional challenges in high k integration.


To detect physical gate defects and study gate dielectric integrity,


a poly-Si etch process to expose the gate dielectric is important


and critical.


SelectivityEtch


5.2 Wet chemical etching of poly-Si


Wet etching is normally used to remove gate poly-Si for FA. Concerns with this method are its isotropic nature and over-etch  problems. The correct wet chemistry should have high polySi/SiO2 etch selectivity. Characterization of the wet etching  process is also critical.  KOH, TMAH, and Chlorine hydroxide  are all possible poly-Si etch chemistries due to their controllable  etch rate and high poly-Si/SiO2 etch selectivity.


In this work, 30% wt TMAH was used for poly-Si etch to expose  gate oxide. The poly-Si etching process was characterized at  different temperatures. Figure 6 shows the impact of temperature  on the etch rate of poly-Si and gate oxide. Figure 7 shows the  impact of temperature on poly-Si/SiO2 etch selectivity. Etch  selectivity increases as the temperature decreases.


1.0E-01


1.0E+00 y1.0E+01 w


1.0E+02


1.0E+03


1.0E+04


70


90


Temperature (degree C)


Poly


Gate Oxide


Figure 6. Temperature vs. the etch rate of poly-Si and gate  oxide


1.0E+01


Temperature (C)


Figure 7: Temperature vs. poly-Si/ SiO2 etch selectivity


Figure 8. Image of gate oxide after poly-Si etching


Figure 8 and 9 are images of gate oxide in 0.13 um technology  Cu/low k device after poly-Si etch process.  The poly gates


have been completely removed without damage to the gate


oxide or substrate.


Figure 9. Image of gate oxide after poly-Si etching


5.3  Special FA Techniques for Detection of Gate  Oxide Defects – Case Studies


A new gate oxide (GOX) defect decoration technique was  developed to avoid some of the limitations of deprocessing by  mechanical polishing, where it is difficult to get planar results


over a large area.  The technique also facilitates individual  gate specific substrate decoration as a result of compromised  GOX.


The technique was used on a failing device where electrical  analysis, E-beam probing and FIB analysis had determined  that a particular clock node was shorted to VDD, causing  device failure.  The short was further isolated to a specific  group of 14 transistors and was believed to be related to a  GOX issue, based on previous analysis. The specific device  topology caused uneven removal of dielectric by polishing, however the poly-Si had to be exposed to allow the poly-Si to  be etched. Therefore this new technique was developed and  worked well.


.0kV 13.2mm x45.0k SE(M) 6/11/08 17:50


667


Figure 10 shows the process flow. It contained the following  steps: Mechanically polish the device down to the W2 level, mill an FIB hole through the poly metal dielectric into the  specific poly-Si region connecting to the suspect gates.  Figure  11 shows the image of FIB holes at W2 level. In this case, M1  was left intact to prevent the individual gates from charging.  The device was then placed in heated KOH solution to  laterally etch the poly-Si, still surrounded by dielectric, to etch  the poly-Si gate and allow substrate decoration (in an inverted  pyramid pattern along the crystal plane) through any existing  GOX void.


POLY


FIB SHAFT


W1


SUBSTRATE


SUSPECT GOX VOID


1.  FIB mill shaft into suspect POLY gates after polishing through W2


KOH ETCH


GOX VOID AND SUBSTRATE DECORATION


300kV 13.2mm x30.0k SE(M) 6/11/031754


1.00um'


2.  KOH etch will tunnel through POLY and potential GOX void and decorate substrate


Figure 10. Images of the Process Flow


GAAGADhn..


Figure 11. Image of FIB holes at M1 level


Figure 12. Result of gate oxide pinhole after the device was  stripped to substrate – note decoration into the substrate


Figure 12 and 13 show result of gate oxide pinhole after the  device was stripped to substrate (note: decoration into the  substrate).  Special care was taken to not allow a gate to float  after cutting off the source/drain connection that would allow  charging and potential FIB induced GOX breakdown – the  very defect this technique was trying to detect.


A test sample was prepared to qualify the technique. The  sample was polished to W2 and FIB holes milled to specific  gates (in the region between the P-channel and N-channel  transistors in inverters) using CAD navigation. A few gates  were deliberately damaged using FIB induced charging while


other “protected” transistors were left connected at their  source/drains to prevent damage. The sample was subjected to  a 15 second KOH etch/decoration, stripped to substrate (HF), and inspected on the SEM. During SEM analysis, the selected  FIB damaged gates exhibited evidence of GOX breakdown (substrate etching); other protected gate regions that were  milled showed no substrate etching. The technique worked  successfully on the test sample and was then used successfully


006000m


on the failing device.


0601agnnninnn一一


Agere 10.0kV 14.1mm x150k SE(U) 4/29/02 16:31 '|| 200hm


Figure 13. Result of gate oxide pinhole after the device was  stripped to substrate – note decoration into the substrate


6.  Backside Failure Analysis and Case Studies


EITI Agere 10.0kV 14.1mm x40.0k SE(U) 4/29/02 16:31750nmEI


Conventional front side defect localization in IC devices has  become less and less effective with an increase in the number  of metallic layers. Electrical defect localization in devices with  Circuit Under Pad (CUP) structures, devices with a high  number of metallization levels and Flip-Chip Ball Grid Array (FCBGA) packages, can more easily be carried out from the  backside of the die. Development of backside failure analysis  techniques is increasingly important. Three major steps are  involved in the backside FA process: backside sample  preparation, backside defect localization, and backside  physical analysis.


A combination of mechanical milling (Chip-Unzip TM) and  RIE techniques has been employed for silicon thinning, which  is a critical step in the backside sample preparation process


[3]. In this process, RIE can be used for final silicon thinning  after mechanical milling to achieve more precise control of  thickness of the remaining silicon die while still preserving the  electrical integrity of the device.


FIB Edits


Figure 14 is a low power optical image of the backside of a  failing device packaged in a PBGA after the backside sample  preparation process.


Several backside defect localization techniques and tools have  been used in the industry, such as Light-Induced Voltage  Alteration (LIVA), Thermally-Induced Voltage Alteration (TIVA), Optical Beam Induced Resistance Change


(OBIRCH), Picosecond Imaging Circuit Analysis (PICA), Laser Voltage Probing (LVP), Fluorescent Microthermal  Imaging (FMI), and Photo Emission Microscopy (PEM). After  backside sample preparation and backside defect localization, backside physical failure analysis becomes increasingly  critical to find the root cause of the failure.


Figure 14. Low power image of package after backside  sample preparation


In certain package types, after the backside sample preparation  process, there is a cavity in the backside of the package  containing the die. Deprocessing the whole package from the  backside is time consuming. Moreover, some artifacts and  defects could be introduced during deprocessing of the entire  package.  To over come these problems a diamond-saw was  used to precisely cut into the cavity along the edge of the die  and separate the chip from the rest of the package. Figure 15 is  the low power optical image of the backside die after the  sawing step.


Figure 15. Low power optical image of the backside die  after sawing of the package


Further silicon thinning was performed using RIE processing  until the remaining silicon thickness was approximately five  microns. The characterization of this process has been  described in our previous work [3].The device was then  polished to smooth the backside silicon die. TMAH wet  chemical etching was used to selectively remove silicon  material over gate oxide due to its high Si/SiO2 etch  selectivity.  The advantages of TMAH over mechanical  polishing for removing the silicon substrate are as follows: removing silicon without damage to gate oxide, better  uniformity across the die, and better control of backside  deprocessing. The Si/SiO2 etch selectivity varies with different  temperatures and at different TMAH concentrations. As  mentioned previously, etch selectivity decreases with an  increase in temperature.


02


Figure 16. Optical backside image of the whole die


Figure 16 shows a low power optical image of the entire die  just after TMAH etching of the remaining silicon. The entire  die was exposed uniformly without damaging the gate  dielectrics


Figures 17 and 18 show high power optical images of the  device during further backside deprocessing.  A combination  of CMP and RIE was used to deprocess the metallization  levels. The CMP method used on the backside is similar to the  one described above for front-side FA.


Figure 17. Backside optical image


Figure 18. Backside optical image


Figures 19 shows SEM images of the device after RIE etching  of the low k ILD to expose the copper metal runners. The  anomalies were observed under SEM analysis and are believed  to be EOS damage.


D.OkV 118mmx13okSE(M512/0312:451.67um


Figure 19. SEM image of M5 runners at defect site


7.  Conclusion


In this work, several front-side and backside deprocessing  techniques for copper and low k technology were developed  and discussed including: reactive ion etching (RIE), parallel  polishing, chemical mechanical polishing (CMP) and  combinations of these techniques. The combination of RIE and  CMP techniques works well for deprocessing copper and low  k ILD layers.  Moreover, gate level deprocessing techniques  involving FIB assisted wet etching were also developed. These  techniques allowed successful resolution of several  challenging FA problems.


Reference:


[1] Lawrence C. Wagner, “Failure analysis challenges”, pp. 36-41, 2001 IPFA


[2] Huixian Wu, James Cargo, Carl Peridier and Joe Serpiello, “Reliability issues and advanced failure analysis deprocessing  techniques for copper/low k technology”, pp. 536-544, 2003  IRPS


[3] Huixian Wu and James Cargo, “Characterization of  reactive ion etching of silicon substrate for backside failure  mode analysis”, ISTFA 2002


[4] T. Sakura, H. Utsunumyia and et al., “ A detailed study of  soft- and pre-soft-breakdowns in small geometry MOS  structures,” pp. 183- 186, IEDM Tech. Dig., 1998


p 99-104


DOI: 10.1361/cp2003istfa099


## Backside Deprocessing of CMOS SOI Devices for Physical Defect and Failure Analysis


Backside Deprocessing of CMOS SOI Devices for Physical Defect and Failure  Analysis


Seth J Prejean, Joseph Shannon


Advanced Micro Devices, Austin, TX, USA


This paper describes improvements in backside deprocessing  of CMOS (Complimentary Metal Oxide Semiconductor) SOI (Silicon On Insulator) integrated circuits. The deprocessing  techniques described here have been adapted from a previous  research publication on backside deprocessing of bulk CMOS  integrated circuits [1]. The focus of these improvements was  to provide a repeatable and reliable methodology of  deprocessing CMOS devices from the backside.


We describe a repeatable and efficient technique to deprocess  flip chip packaged devices and unpackaged die from the  backside. While this technique has been demonstrated on SOI  and bulk devices, this paper will focus on the latest SOI  technology.  The technique is useful for quick and easy access  to the transistor level while preserving the metal interconnects  for further analysis. It is also useful for deprocessing already  thinned or polished die without removing them from the  package. Removing a thin die from a package is very difficult  and could potentially damage the device. This is especially  beneficial when performing physical failure analysis of  samples that have been back thinned for the purpose of fault  isolation and defect localization techniques such as: LIVA (Laser Induced Voltage Alteration), TIVA (Thermally Induce  Voltage Alteration), SDL [2] (Soft Defect Localization), and  TRE (Time Resolved Emission) analysis.


An important fundamental advantage of deprocessing SOI  devices is that the BOX (Buried Oxide) layer acts as a  chemical etch stop when etching the backside or bulk silicon. This leaves the transistor active silicon intact for analysis. Further delayering allows for the inspection of the active  silicon, gate oxide, silicide, spacers, and poly. After  deprocessing the transistor level, the metal layers are still  intact and, in most cases, still electrically connected to the  outside world. This can provide additional failure analysis  opportunities.


Advances in the manufacturing of semiconductor devices are  inevitably followed by innovations in failure analysis  techniques out of sheer need to have viable solutions for fault  isolation. Failure analysis continues to play a key role in the  production of reliable integrated circuits by providing root  cause and driving corrective actions, so FA analysis  techniques must evolve along with IC production technology. The trend of backside failure analysis is prevalent throughout


the industry as many IC (Integrated Circuit) manufacturers are  moving towards flip-chip packaging. This type of packaging  improves the package to silicon electrical interface providing  better signal integrity for higher circuit performance. However, it makes traditional front side electrical fault  isolation virtually impossible. This is mainly due to the fact  that die must be electrically disconnected from the package in  order to access the front side of the circuitry. There are some  inherent advantages to backside analysis and deprocessing  such as quicker and easier access to the transistor level and  having an electrical connection to the circuitry while  deprocessing in the package. Techniques have been adapted  for backside analysis such as Photon Emission Microscopy  and TRE as well as laser intrusive techniques (LIVA/TIVA) for hard and Soft Defect Localization (SDL). Once a defect is  localized it is the analyst’s job to physically deprocess and  determine the root cause of the failure. This can be done from  the backside without removing the die from the flip-chip  packaging.


This paper presents an improved technique for deprocessing  both packaged and unpackaged SOI devices from the  backside. The process includes mechanical parallel polishing  of the bulk or backside silicon to within microns of the BOX (Buried Oxide) layer. This is followed by chemical removal of  the


remaining


silicon


with


TMAH  (Tetramethylammoniumhydroxide) to expose the BOX layer. Once exposed, the BOX layer can be removed chemically or  with RIE (Reactive Ion Etching) to expose the active silicon  layer of the transistor. From this point there are several options  for analysis. The silicon can be imaged in the SEM to see twodimensional dopant profiling with image contrast between ntype and p-type silicon.  This phenomenon has been known for  decades [3] but until recently has not proven itself to be useful  for failure analysis. This paper will discuss initial findings on  this experimental technique and suggest further development  as an analysis tool.


After analysis of the active silicon the remaining poly and  metal interconnects can be deprocessed using the RIE method  as well as parallel polishing. This deprocessing technique is  continuously being developed and improved. The  development is mostly in line with the needs for failure  analysis, some of which will be presented as case studies for  this paper such as ESD damage analysis, dopant profiling, and  general inspection for defects.


Backside Deprocessing Techniques


The initial preparation of the samples varies depending on  whether or not the die is packaged and what type of packaging  material is used. This section will go through the scenarios  that were researched.


Sample Preparation


Depending on what type of sample is being deprocessed the  beginning steps may differ. The most involved preparation is  for deprocessing an unpackaged die from the backside. The  same glass slide technique [1] is used. The die is attached to  the glass slide, with the circuit side to the glass, using an  epoxy adhesive [4]. Lead solder bumps are removed prior to  adhering to preserve planarity. Once the epoxy is cured the  sample is ready for polish. Most other packaged samples can  be polished without any additional preparation.


Parallel polishing the backside silicon is done to remove as  much silicon as possible without polishing through the BOX  layer. In many cases the backside silicon will have already  been polished to some thickness but can still be polished  thinner. The more planar the polish the thinner the silicon can  be polished. The idea is to leave a minimal amount of silicon  for the TMAH step. This will reduce deprocessing time and  prevent over exposure to the chemicals that can adversely  affect the deprocessing because of reaction inhibiting issues. Some planarity issues have been seen in organic packages. The die actually takes on a convex shape with the center being  higher than the edges. This has been attributed to the lack of  rigidity in the organic packages.


After polishing, TMAH is used to remove the remaining bulk  silicon. As previously published there are some package  interference issues [1] with the chemicals when deprocessing  organic packages. Therefore the organic package must be  sealed using a hot glue wax [5] leaving only the surface of the  backside silicon on the die exposed. It is also helpful to cut  away some of the package with a diamond saw. Care must be  taken not to fracture the thinned die. This will provide easier  SEM analysis too. Ceramic packages and glass slide mounted  samples have been found to withstand the chemicals and  therefore should not require any special preparation.


A solution of 3:2 TMAH / IPA (Isopropyl Alcohol) heated to  83 degrees C can be used [1]. This will keep the boiling point  low and is known to create anisotropic etching [6]. However  we have not seen any issues when using straight TMAH at 83  degrees C, while at the same time the etch rate is faster [1].  The TMAH will stop etching once the BOX layer is exposed.  The BOX acts as an etch stop for silicon removal since it is  known that TMAH etches oxides at 1/1000 the rate of silicon


[6]. The time to etch the remaining silicon will depend on its  thickness. In Ref. 1, it was shown that the TMAH/IPA and  TMAH only solution could etch silicon at 0.5 um/min and


0.79 um/min respectively. Once the BOX is exposed the active  silicon is still intact and can in fact be imaged through the  BOX using an AFM (Atomic Force Microscope). The areas of


active silicon can be differentiated by height data through the  BOX as seen in the AFM image below. It is suspected that this  is caused by natural stresses.


Figure 1: This is an AFM image (surface height data) of the  backside of the BOX layer after the silicon has been removed  with TMAH. Height difference is less than 1nm. The  impression of the squares of active silicon beneath the BOX  can be seen.


Once all of the silicon is removed the circuitry can be seen  optically. The image below shows some of the circuitry as the  silicon is etched away in a square lattice-like pattern.


Figure 2: Optical Microscope picture of the circuit backside  as the silicon is being etched in a square lattice-like pattern.


The BOX removal step is done using either the RIE method or  chemically using a 10:1 solution of H20: HF (Hydrofluoric  Acid). The RIE method is our preferred method for this paper. Using a calibrated, standard oxide removal RIE recipe the  BOX is etched until the active silicon is exposed. During the  BOX removal process the sample is inspected in a SEM to  verify that the BOX is completely removed. This inspection


Circuitry


process led to a discovery of the phenomenon known as “Secondary Electron Dopant Contrast” [3]. This effect is seen  when a very thin layer of BOX remains and the sample is  inspected in the SEM, the n-type doped silicon has a different  contrast when compared to p-type doped silicon. This will be  discussed later in the paper. After the BOX is completely  removed the active silicon is exposed for inspection as well as  the STI (Shallow Trench Isolation). The images below show  the stages of BOX removal.


Figure 3: This SEM image shows the backside of the  transistors with a thin layer of BOX remaining. Notice the  contrast differences between silicon boundaries. P-type is  brighter than N-type.


Figure 4: This SEM image shows the backside of the


transistor after the BOX layer is completely removed.


The next step is active silicon removal. This can be done


either with the RIE method or TMAH method. The RIE


method is preferred. The same oxide RIE recipe is used to etch  the silicon. The TMAH method is also done the same as


before with a 3:2 solution of TMAH / IPA or straight TMAH  both at 83 degrees C. A short etch time is needed to remove


the active silicon, with 30 second to 1 min etch intervals and  inspection between intervals is recommended. Once the active  silicon is removed the silicide and gate oxide of the transistors  will be exposed. This provides an excellent method for ESD


silicide damage analysis as will be shown later in the paper.


Below is an image of the silicide and exposed gate oxide after  the silicon removal step.


Figure 5: This is a SEM image of the backside of a transistor  after active silicon removal. The gate oxide and silicide


remain exposed.


The remaining steps for deprocessing are still under


development. The proposed techniques are layer-by-layer


polishing, RIE method used to etch ILD layers, or a


combination of both.


The steps listed above have been proven on SOI technology


and have also been used for failure analysis and fault isolation.


Case Studies in Backside Deprocessing


ESD Failure Analysis


Backside deprocessing was used very successfully in  analyzing ESD damage on the K8 microprocessor devices.  Because of the difficulties of deprocessing SOI units from the  front-side, determining root cause of ESD failures was very  difficult.  But from the backside, it was simple and easy.


The first step was to thin a unit from the backside and  electrically isolate the short with TIVA. After the exact failing  location was found, the same unit was thinned further.  See


P-type Si


N-type Si


Silicide


Gate


pictures below for examples of ESD damage from the  backside.  Note that the pinholes in the gate oxide are easily  identifiable.  Also, we can see that the CoSi   reflowed under  the gate.  This damage would not have been visible using  standard front-side deprocessing methods.


Figure 6: Backside SEM Image of ESD damage caused by  stress testing. Notice silicide re-flow across the transistor  gate.


Infrared Thermography


The First Law of Infrared Thermography


Infrared Thermography is defined as “the acquisition, storage  and evaluation (analysis) of radiated energy using an infrared  imaging device. Different levels of this radiated energy from  the scene viewed are displayed as different colors on a video  monitor” [2], most of the infrared devices used in the industry  include some type of imaging software for the user to interface  and analyze the image on the scene. The color palettes  available in the software can be chosen to represent the levels  of radiated energy seen by the infrared camera and displayed  on the screen.  Having said this, many users are tempted to  move the cursors on their screen over a certain object on the  display and acquire a reading of what appears to be the  temperature of a component on the SUT. This is an incorrect  assumption.  The first law of infrared thermography states “Infrared Instruments measure the energy radiated from the  first 1/1000 inch of the surface of an object” [2]. They do not  measure temperature which can be calculated using the  onboard computer most imaging devices are equipped with. Therefore, the Infrared Camera does not measure or ‘see’ temperature.  Furthermore, it is important to understand that “Infrared radiation in general, will not pass through a solid or  a liquid, but will pass through a vacuum or a gas very easily”


[2]. Having said that, note that the Infrared Camera “does not ‘see through’ most solids or liquids.  In addition, in most cases  the IR camera can sense the total radiated energy from both  the emitted energy from an object due to its temperature and  the reflected energy from the object’s surroundings.


All theories leading to what we now know as IR thermography  were developed by using a theoretical object known as a  Blackbody, which is a perfect emitter and perfect absorber; it  emits a maximum amount of energy at all temperatures in all  wavelengths. Basically IR thermography, as everything else in  the world, is dependent on the existence of energy.


Energy, Temperature and Heat


Energy is nothing else than the capacity of a system to do  work and it is measured in Joules. Energy itself can be broken  down in two types, kinetic energy and potential energy. IR


thermography is dependent on Kinetic Energy which is energy  in motion. This leads to another important term in IR  thermography, temperature.


Temperature is defined as “a measure of the average kinetic  vibrational energy of the molecules of a substance” [2].  Four  temperature scales have been developed since the 1600’s until  now; they are Fahrenheit, Kelvin, Rankin and Celsius. Fahrenheit uses the freezing point of a solution made up of salt  and water solution as it’s starting zero point. The Celsius zero  degree point is based on the freezing point of fresh water. Kelvin and Rankin are known as the absolute temperature  scales, both starting at zero degrees.  The following table  represents the relationship between the four temperature scales.


Table 1: Relationship between the Temperature Scales


Kelvin Celsius Rankin Fahrenheit


373.15


671.7


212


273.15


491.7


32


-459


Fahrenheit is the temperature scale used in the United States, however most, if not all of the temperature based applications  in the world use the Celsius scale for temperature  measurements.  The mathematical relationship between the  Celsius and Fahrenheit scales is as follows:


Tf = (1.8 x Tc) + 32


(1) Similarly, the relationship between the Kelvin and Celsius  scale is as follows:


Tk = Tc + 273.15


(2)


Stephen-Boltzmann’s law shows the impact that temperature  has in the amount of energy radiated by an object. It states that  the radiated energy by an object is directly proportional to the  fourth power of its absolute temperature by the StephenBoltzmann constant σ = 5.67 x 10-8 J/(s m2 K4). Mathematically this can be expressed as:


Q= σT4


(3)


Therefore from (3), a small change in temperature leads to a  big change in the energy radiated by an object.


Having discussed the main building blocks of temperature, we  are lead to one of the most significant forms of energy. Heat is  essentially the transfer of energy due to a difference in  temperature between molecules.


Heat Transfer


The transfer of heat will occur if and only if there is a  difference in temperature between two molecules. At a high  level this can be stated at the difference in temperature  between two objects. Heat transfer will not occur if two


objects are at the same temperature. This condition is known  as thermal equilibrium. Heat transfer can mainly be explained  by the first and second law of thermodynamics. The first law  of thermodynamics states that energy cannot be created nor  destroyed, but it must be conserved. This means that when  energy transfer (heat) occurs, it must travel from one point to  another. This brings us to the second law of thermodynamics  which states that heat always travels from a point of higher  temperature to a point of lower temperature. This law applies  until both points are at thermal equilibrium or reach the same  temperature.


Heat transfer can happen by conduction, convection, change  of state or radiation. Conduction is defined as the transmission  of energy from a point of higher temperature to a point of  lower temperature through a conducting medium. For  conduction to occur there must be some sort of matter (a solid  liquid or a gas) present as well as a difference in temperature  between the molecules of the matter. This is better explained  by Joseph Fourier’s law for conduction:


q” = -k ∆T/ d                                           (4)


Where, (q”) is the heat transfer rate or a flow equal to thermal  conductivity (-k), thickness of the material (d), and  temperature difference (∆T).  Converse to conduction, convection is identified by its finger like, uneven pattern and  defined as the transmission of energy from a region of higher  temperature to a region of lower temperature by the circulation  of currents though a liquid or a gas. For convection to occur  there must be a difference in temperature, pressure and the  presence of a medium such as a liquid or gas. Although for  conduction to occur, molecules must be in contact, in  convection, the molecules need not to be in contact since heat  can occur by the movement of these molecules.  Mathematically, the effect of convection can be expressed as:


q = h (Ts - T∞)


(5)


Where (q) is heat transfer, (h) is the convection heat transfer  coefficient and the temperature difference is derived from  Newton’s law of cooling. Next we have heat transfer by  change of state; this is simply the transfer of energy when an  object is changing to or from a solid to a liquid to a gas or the  other way around. Finally, we have heat transfer by radiation  which is defined as the transfer of energy, through a gas or a  vacuum, from solids or liquids at higher temperatures to one at  a lower temperature by alternating electromagnetic waves. For  heat transfer by radiation to occur, there must be a difference  in temperature, a solid or liquid and a medium such as a gas or  a vacuum2. This takes us to the topic of radiation.


Radiation and the Electromagnetic Spectrum


To further understand IR thermography a key term of the  theory must be defined.  Recall, the Infrared Camera can only ‘see’ the radiated energy or infrared radiation of an object. Radiation is the energy transmitted, through a gas or a vacuum, by alternating electromagnetic waves constantly traveling at


3x108m/s or the speed of light (c).  All objects above absolute  zero will radiate energy in some form. This is due to the fact  that the molecules move at temperatures above 0oK therefore  objects are constantly releasing energy by emitting  electromagnetic radiation, and acquiring energy by absorbing  some of the infrared radiation that is incident on them from  other objects.   Note that electromagnetic radiation is the type  of radiation related with electric and magnetic fields resulting  from the transmission of energy due to the acceleration of an  electrical charge and does not depend on a change in  temperature. Electromagnetic radiation, however, is dependant  on the wavelength (λ) and the frequency (ƒ) of  electromagnetic waves. Mathematically this can be shown as  follows:


λ = c/ƒ


(6)


This leads to the electromagnetic spectrum, particularly the  infrared section which is found at wavelengths from 1–1000  microns (1x10-6meters). The human eye, however, cannot see  at this wavelength range and IR cameras can only ‘see’ in a  small portion of this wavelength area of the spectrum, 1 - 6  microns, and  8-14 microns.  In addition, there should be  minimum temperature sources around for the human eye and  the infrared cameras to ‘see’. The following table summarizes  the above.


Table 2: Relationship between wavelengths, minimum  temperature of sources, the human eye and IR devices.


Eyes Near  wave  IR


Short   wave IR


Long  IR


Wavelength (µ)


0.38 -0.72


0.79 -1.7


2-6


8-14


Temperature (oC)


525


275


-25


-35


This means that for the human eye to be able to see an object   we must be in the visible portion of the electromagnetic  spectrum that lies from 0.38- 0.72 microns and there must be a  temperature source around with a minimum temperature of  525oC, for example industrial fluorescent light bulbs. On other  hand, for short wave IR devices to work in the range of 2-6  microns, they must have a temperature source in proximity of -25oC as is the case of the IR camera utilized in this study. Note from table 2 that as the temperature decreases, the  wavelength increases. This assertion can be confirmed by the  German physicist Wilhelm Wein, who derived Wein’s law:


λmax= 2898 / T  (microns/Kelvin)               (7)


Wein’s Law expresses the wavelength at which an object  emits a maximum amount of energy at any given temperature. Furthermore, Max Planck established a theory which relates  temperature, radiated energy and wavelength. Planck stated  that electromagnetic radiation exists in discrete packets known  as photons. Planck’s Law describes the spectral distribution of


energy as a function of wavelength for any specific  temperature. Mathematically it is shown as:


Q(λ) = (2 h c2 / λ5) * [1/(e(hc/λkT) -1)]                (8)


Where, h= 6.64x 10-34 J*s, and it is known as Planck’s  constant. Now a clear relationship between temperature, energy, wavelength and frequency can be established. As  temperature increases, the energy increases, the wavelength  decreases and from (2) the frequency increases.


Emissivity


In reality Emissivity plays a big role in what can be seen  through the lens of an IR camera. Without knowing the  importance of emissivity, IR analysis can be misinterpreted  leading to erroneous results. Emissivity is the ratio at which an  object emits energy vs. the energy radiated by a blackbody at a  given temperature and wavelength. “The emissivity of an  object is determined by five features, the material of the object, the surface condition of the object (first 0.001 in), temperature  of the object, wavelength viewed, and the geometry of the area  viewed.” [2] The first two being the main features to  determine emissivity. Therefore to perform a good analysis of  an IR image, it is important to remember that, the higher the  emissivity of the SUT (low reflection), the more closely the  thermal image represents SUTs temperature. Conversely, the  lower the emissivity of an SUT (higher reflection) the more  closely the thermal image represents the SUTs surroundings. However, if the SUT is at ambient temperature or at the same  temperature of its surroundings, the emissivity characteristics  disappear.


The IR Camera


In order to be able to obtain a clear and accurate image and  analysis of the SUT, a high performance IR camera was used  as our infrared imaging device. The IR camera is a midwavelength (Short wave IR) infrared camera that “consists of  a Striling-cooled Indium Antimonide (InSb) Focal Plane Array (FPA). The FPA is a 320x256 matrix or ‘staring’ array of  detectors that are sensitive in the 1.0µm to 5.4µm range. The  standard camera configuration incorporates a cold filter that  restricts the camera’s spectral response to the 3.0- 5.0 micron  band. The FPA is enclosed in an all-metal evacuated dewar  assembly cooled by a closed-cycle Stirling cryocooler, and is  thermally stabilized at a temperature of 77K.


The IR Camera operates the InSb FPA in a single output, full  frame, and 6Mpixel/sec mode. The full 320x256 FPA operates  at a frame rate of 60Hz, 12bit digital data stream in an NTSC  camera configuration.” [3] But no matter how good the  camera is, it has to be complemented by the appropriate  software in order to acquire, analyze and achieve the dynamic  IR approach.


The OEM Software


The software used to interface between the IR camera and the  PC is a package that includes programs useful to create


emissivity maps and apply them to similar images of the same  type. Since our dynamic infrared approach focuses on relative  comparisons instead of absolute comparisons, emissivity maps  were not critical. The OEM software was used to acquire the  real time images and adjust the desired temperature level and  span. With this, one would be able to take relative or absolute  temperature measurements at different points of the SUT in  the screen. The software also included the capability to align  images on top of each other by picking certain points on an  image template. However, it was only useful for frame by  frame images and not real time or recorded videos as dynamic  infrared requires. Mechanical alignment methods were utilized  to maintain the registration of the SUT. This allowed us to put  the SUTs at the exact same position and perform accurate  comparisons between same types of systems.


Although the OEM software package was very useful for IR  thermography analysis, additional software had to be created  for developing the desired real time infrared video subtraction.


Dell Developed Dynamic IR video Subtraction Software


Lab-View version 6.1 along with Vision Development  Module from National Instruments and AVI Library from  Graftek Imaging Inc. were interfaced to develop the AVI  video subtraction software. The function of the program is to  take the AVI files obtained from the OEM program, break  them into frames and perform an automated frame by frame  subtraction (pixel by pixel arithmetic operation) between the  frames of a good known SUT and a suspect SUT; later joining  the resulting frames to form a new single AVI file that  represents the video subtraction result between the good  known and suspect SUT. The features include a frame per  second (FPS) option to decrease the playback speed, and a  subtraction option given the choice of normal subtraction or  absolute subtraction. Based on the default color palette used in  this study, a brighter color (approaching white) represents a  higher temperature and a higher pixel value. On the video  subtraction result, a bright color indicates color temperature  differences and dark color indicates the equivalent temperature. If there is a difference in temperature between the good SUT  and bad SUT, the video subtraction result will show it in  bright color. The use of absolute subtraction will reduce the  need to do the subtraction process twice (first subtracting bad  SUT minus good SUT, and secondly subtracting good SUT  minus bad  SUT) as it shows the absolute difference between  two boards.  Figure 1 shows the main menu of the video  subtraction software:


Figure 1: AVI video subtraction software Main Menu.


Dynamic IR


The Dynamic IR approach is a real-time, video based analysis  for time-dependent and test specific failure isolation. Single  video analysis of a suspect SUT, side-by-side video  comparison analysis, and video subtraction analysis between a  good know and a suspect SUT are the main analytical methods  for the Dynamic IR approach.


The remainder of this paper focuses on the experiments  conducted to demonstrate the effectiveness and advantages of  the Dynamic IR fault isolation approach as well as the lessons  learned from this experience.


Dynamic Single Video FET isolation in a known Parallel  Circuit


A suspect system was received with the symptom of a three  second shutdown. Resistive measurements at the motherboard  level revealed that the failure was due to a low resistance path  from B+ (Vin) to ground among a group of six FETs in  parallel located in the processor power-up circuitry.  However, it was difficult to non-destructively isolate the failure down to  a single component since all FETs shared the same power rail. In normal operation it would be expected that all six FETs  exhibit the same thermal signature as they are all the same  type and in parallel to each other, therefore the same amount  of current would flow across them. Since current flows  through the path of lowest resistance, it is expected that a  thermal signature will exhibit itself across the component with  low impedance. With this in mind, the suspect SUT was  placed under the IR camera zooming in to the location of the  six FETs on the board.  A window of three seconds was  available to identify the failure.  A trigger was set for the  software to start recording the real time IR video from the time  of powering up the system until the shutdown occurred. The  real time video was then saved into AVI file format and into a  sequence file in case future editing would be needed (such as  analysis under a different color palette).


The analysis on the suspect SUT video revealed a thermal  event in one of the FETs, as expected, isolating the failure to a  single component on the motherboard.


The use of static image analysis to try to isolate this failing  component may not have been possible. Dynamic IR, however, has its strength in easing the analysis of time dependant  failures as well as failures that do not exhibit themselves  permanently. This type of failure could have been missed if  static analysis was used due to the short amount of time that  the thermal event occurred. The dynamic IR approach allowed  the analyst to review the video and quickly and accurately  isolate the unique thermal signatures. Figures 2.1a and 2.1b  depict frames from portions of the video that was used to  analyze and isolate the failing component on the motherboard. Figure 2.1b shows the thermal event that led to the fault  isolation.


Figure 2.1a: Video frame of failing FET in a parallel  circuit during OFF state.


Figure 2.1b: Video frame of failing FET in a parallel  circuit during thermal event.


Contrary to the above example, sometimes the failing node is  not known. Identifying failure locations under these  ambiguous circumstances can be simplified by the use of  Dynamic Infrared fault isolation, as the following two  examples show:


Dynamic internal short isolation on an IC with protection  circuit


A system was received with a no video symptom. Preliminary  analysis showed that the suspect SUT system was able to  finish POST (Power-On Self Test). The suspect SUT was  placed under the IR camera focusing on the motherboard as a  whole. A trigger circuit, as the one shown in Figure 3.0, was  built to keep the timing sequence the same between the  suspect SUT and the exemplar SUT. Employing the trigger  circuit, once AC power is applied, the SUT will have auxiliary  power (SUT transition from G3 to S5 state) and the top  2N7002 N channel MOSFET turns ON sending a trigger  signal (low voltage logic) to the PC (with the IR camera  software) for the software to start recording.  Through an RC  circuit, the lower 2N7002 N channel MOSFET will receive a  delayed turn-on of 3 seconds, sending a signal to the SUT that  simulates the power button being pressed to turn ON the SUT (SUT transition from S5 to S0 state).


Figure 3.0: Trigger circuit


The real time videos were then saved into AVI file format and  into a sequence file. The same was done for a good known  SUT.  Figures 3.1 and 3.2 show the thermal events on the  suspect and exemplar SUT at t=4.2s. Note that there are  several components that experience a thermal event on both  suspect and exemplar SUT which makes it more difficult to  isolate the failure down to a single component.


The two videos were subtracted to reveal the difference. Figures 3.3a and 3.3b depict the resulting video from the  subtraction at t=4.2 s and t=7.5s respectively.


Figure 3.1: Video frame of the failing IC (Q13) at 4.2s  on the suspect SUT.


Figure 3.2: Video frame of the IC (Q13) on a good SUT  at 4.2s.


Figure 3.3a: Video frame of the subtraction result at  the failing time at 4.2s.


Figure 3.3b: Video frame of the subtraction result after  the failing time at 7.5s.


The analysis of the result showed that a component labeled  Q13 (a quad AND gate for video buffer) had a different  thermal event than it’s counterpart in the good know SUT. It  was seen that on the bad SUT Q13 thermally emits for a  moment during the transition from G3 to S5 (auxiliary power  only) and again during the transition from S5 to S0 (SUT  turned ON by pressing the power button) (t=4.2s).  In the S0  state (SUT ON) (t= 7.5s), Q13 is electrically off on both the   failing and exemplar boards, therefore as seen from the video  subtraction in Figure 3.3b, there is no thermal difference  between suspect and exemplar SUT at this point in time. After  Q13 was isolated as a failure location, further investigation  revealed that Q13 has a current protection circuit, which turns  off the device in case of failure.


It would have been very difficult and time consuming to try  and isolate this failure using Static IR due to the fact that the  failing node was not known, the thermal event was temporary, time dependent and revealed itself as a momentary thermal  emission at two different states of operation. Contrary to Static  IR, this is where Dynamic IR fault isolation holds its strength. A one time recording of the failing SUT and the good known  SUT was enough to produce a resulting subtracted video of  the two SUTs isolating an ambiguous failure to a single  location.


Dynamic open circuit fault isolation using side by side  video comparisons


A suspect SUT was reported to have a networking failure. Preliminary analysis revealed that the system failed to connect  to the network. The main area of focus for analysis was on the  NIC circuitry. The network chip uses one differential pair to  transmit and one differential pair to receive at speeds of  10Mbit or 100Mbit. It uses two differential pairs to transmit  and two differential pairs to receive at a speed of 1Gbit; each  line in the pair is connected to a resistor. The opposite ends of  the resistors of each pair connect together and to ground  through a capacitor.


The suspect SUT was placed under the IR camera, zooming in  to the NIC circuitry.  The network test software was run on a  good and suspect SUT. This test consisted of transmitting and  receiving large files through the network at 10Mbit. A 10  second video was recorded of the good known SUT to reveal  the network activity in the motherboard based on the thermal  pattern. The same was done for the suspect SUT. The good  known sample showed that if the system was transmitting, the  resistors connected to the transmit pair emitted a dynamic  thermal signature as shown in Figure 4.1a.


Figure 4.1a: Video frame of emitting resistor pair during  transmit.  Thermal event occurs in exemplar SUT.


Similarly when the system was receiving, the resistors  connected to the receive pair emitted a dynamic thermal  signature as shown in Figure 4.1b.


Figure 4.1b: Video frame of emitting resistor pair during  receive. Thermal event occurs in exemplar and suspect  SUT.


Dynamic IR fault isolation was conducted by comparing, side  by side, the IR videos of a good known and suspect SUT. The  failing SUT revealed that both resistors connected to the


receive pair emitted when receiving data but only one resistor  connected to the transmit pair emitted when transmitting data. Refer to Figures 4.1a and 4.2 for comparison:


Figure 4.2: Video frame of single blinking resistor during  transmit mode on suspect SUT. Note the absence of a  thermal event on the second resistor.


This behavior suggested that no current was flowing through  the second resistor on the transmit pair. After the failure was  isolated, further investigation revealed that the resistor was not  soldered properly. Once the resistor was re-soldered, the  system was able to function correctly at every speed.


The static IR approach is not effective in this case as it is not  capable of capturing the changing states of the resistors (ON  and OFF). Conversely, the Dynamic IR fault isolation  technique provides the capability to capture the continuous  activity of the resistors.


Dynamic short circuit fault isolation: Cause and Effect


A suspect system was received with a POST failure. Preliminary analysis using the on system quad-pack diagnostic  LED’s suggested that the system was having a power up  failure. The suspect SUT was placed under the IR camera  focusing on the motherboard as a whole. A trigger (see Figure


3.0) was set for the software to start recording a real time  video of the power-up sequence of the board from the time the  power button was pressed (S5 to S0) until 12 seconds  thereafter. The real time video was then saved into AVI file  format and into a sequence file. The same was done for a good  known SUT (Figure 5.1).


The resulting subtracted AVI file revealed a thermal  difference. The analysis of the result identified a high-side  Power FET and a current sense resistor on the defective SUT  heating up immediately after power up and gradually  dissipating heat (Figure 5.2a).


Figure 5.1: Video frame of good known SUT during  power up.


Figure 5.2a: Video frame of subtracted result at t=3.8s


In about 1.2 seconds the resistor emits less while the FET  continues to emit at the same rate (Figure 5.2b).


Figure 5.2b: Video frame of subtracted result at t=5s


Within nine seconds the FET began dissipating less heat (Figure 5.2c).


Figure 5.2c: Video frame of subtracted result at t=9.1s


Shortly thereafter, the components stopped emitting and no  visible heat signature was evident.


After the fault was isolated to the two components, further  analysis revealed a high impedance (63 Ω) short to Ground on  the 12V Core line indicating that the faulty component was the  high-side FET Q1B2 which was shorted. As the investigation  continued, it was found that the current sense resistor is  utilized for short circuit protection. The current through this  sense resistor feeds into all the high-side power FETs and it is  monitored by an on board controller. In normal operation the  controller turns OFF the high side FETs and turns ON the low  side FET when the load current goes beyond threshold.  In this  incident, because of the short in one of the high-side FETs, switching did not occur, the lower side FET never turned ON, causing the load current to exceed it’s limit, therefore the  current sense resistor exhibits a thermal event for a short  period of time. Furthermore, the excess current discharges the  capacitors at the CPU core circuitry output causing the shorted  FET to dissipate heat slower than the sense resistor.


Static IR would not have been efficient in the analysis of this  failure, as it is not able to reveal the different states of a failing  component and the effect on other components via a thermal  event; especially if the thermal event is temporary. Dynamic  IR, however, was able to capture the power-up sequence of the  failure, point the user to a couple of suspect circuits that, with  deeper investigation and the aid of  video analysis, helped in  the isolation of the failure and the understanding of it’s effect  on other components sharing the same circuitry.


Summary and Conclusions


From infrared thermography theory and the experiments that  were completed, the following can be concluded:


• Dynamic IR is a real-time, video based analysis method  for time-dependent and test specific failure isolation.


• Dynamic IR system level fault isolation is more effective  than the Static IR approach for three major reasons:


o The ability to identify temporary failures occurring at  unknown points in time


o The shorter amount of time required to isolate a  temporary thermal event


o The ability to capture the changing states of  components while dynamically stressing a system


• Dynamic IR consists of three methods of video analysis: o Single video analysis of a suspect SUT as seen in  Figure 2.1b used when the failing node is known, but  not the exact location


o Side-by-side video comparison analysis used when  the failing circuitry is known, but the failure within  the circuitry is not obvious, as seen in Figures 4.1a  and 4.2


o Video subtraction analysis between an exemplar and  a suspect SUT used to highlight differences between  a suspect and exemplar SUT when little is known  about the failure, as seen in Figures 3.3a, 3.3b, 5.2a,


Figure 7: Backside SEM image of ESD damage caused by  stress testing. Notice pinhole.


Secondary Electron Dopant Contrast in the SEM


During the development of the backside deprocessing  techniques an interesting phenomenon was discovered. It was  found that at the BOX removal step if the BOX was not  completely removed and a thin layer of oxide remained the  SEM showed a contrast difference between n-type and p-type  silicon. Once the remaining BOX layer was removed the  contrast was usually too faint to detect. Also p-type silicon


appeared brighter than n-type silicon. Below is a SEM image  of the dopant contrasting.


Figure 8: SEM image of dopant contrast effect. Notice areas  of p-type active silicon appear bright compared to areas of ntype active silicon.


After researching this effect it was found that this has been


seen before on transistor cross sections. Cordelia P. Sealy,


Martin R. Castell and Peter R. Wilshaw have published very  detailed research [6] about this effect and have also explained  the following reason why p-type is brighter than n-type.


Brighter contrast in a SEM is a result of larger Secondary


Electron yield. P doped silicon requires less energy to generate  Secondary Electrons thus producing more SE’s for a given


beam energy. N doped silicon requires more energy to


generate Secondary Electrons resulting in a lower yield than P  doped silicon for the same given beam energy. The difference  in the band structure of N vs. P doped Silicon can explain why  the latter requires less energy for yielding secondary electrons. The Ionization energy, or the energy required to take an


electron from the top of the valence band to just outside the


semiconductor and to the SE detector, is inherently different


between n-type and p-type silicon due to the doping


characteristics. The explanation of why the contrast is seen


better through the oxide layer could be that in order for the


electrons to travel through the oxide they must have more


energy. This would magnify any difference is band structure  by raising the energy needed for a secondary electron to travel  to the SEM detector. For a given beam energy, electrons


moving out of n-type material require more energy to reach


the SEM detector. More electrons from the p- type material


have adequate energy to reach the SEM detector thus giving a  higher SE yield. This energy difference can be seen in the


band diagram below.


CoSi


Spacer


pinhole


Figure 9: Band diagram of p-type and n-type silicon.


The above diagram shows that the energy required to move


from EV (energy at vacuum) to ESEM (energy required to reach  the SEM detector) is less for p-type (delta Ep) than n-type


(delta En) silicon. Also delta Ep is above the energy required to  get to the SEM detector, ESEM. The energy delta En shows that  more energy is required for a SE from the n-type material to  reach the SEM detector. Below are some more images taken in  the SEM that show dopant contrasting. Notice the difference  in contrast at the undoped channel silicon.


Figure 10: SEM image showing dopant contrast from the  backside of the transistor.


Figure 11: SEM image showing dopant contrasting in an  SRAM memory array.


This technique is currently being researched to attempt to


develop this into a useful dopant analysis technique. The


biggest issue is resolution and sensitivity to dopant


concentration. In our research, the image contrast improves as  the acceleration voltage of the SEM is decreased. Research [3] has shown this technique can provide .05 - .1um resolution.


Imaging has been done on dopant concentrations in the range  of 1017 to 1018 /cm3 on cross section transistor silicon [3]. This  resolution should only improve as dopant concentration


increases [3] with technology scaling as designers push the


performance and speed of the transistor while reducing the


critical dimensions. Dopant contrast could be developed into a  quantitative analysis tool for dopant concentration


measurement of active silicon [3]. The SE emission intensity  has been proven to be logarithmically proportional to dopant  concentration [3]. This could prove to be a very useful


analysis technique for chasing “invisible” defects like dopant  issues.


Future Development


Backside Atomic Force Microscopy


An additional analysis technique is backside SCM through the  BOX layer. The silicon, which is still electrically connected to  the package through the pins when deprocessing packaged  devices, can be biased while the AFM scans over the surface  as it measures capacitance. This capacitance should vary with  material, silicon vs. STI and with dopant type p vs. n. The  capacitance should also vary with dopant concentration  allowing SCM to map lightly doped vs. heavily dope regions. Once the gate oxide is exposed the AFM could be used to  accurately measure the width of the oxide by detecting the  change in step height between spacers and gate oxide.


EV  EVac  ESEM


∆Ep


∆En


n-type


p-type


Channel


N-type P-type


Deprocessing


Research and development of these deprocessing techniques  will continue as well as development of more analysis  techniques for backside FA. While this is still a fairly new  area the development is rapidly growing.


In conclusion, this technique has proven to be a reliable and  efficient method of deprocessing CMOS SOI devices from the  backside. It also provides a new angle of looking at defects in  failure analysis as well as another tool in the analyst’s toolbox. Using backside deprocessing is a safe and easy alternative to  deprocessing already thinned devices without removing them  from package. Finally, the ability to inspect all layers of the  transistor, BOX, active Si, silicide, spacers, oxide, and poly  while keeping the metal interconnects intact has been shown  and provides a means for development of new FA techniques.


The authors would like to acknowledge Matt Thayer for the  use of his lab and equipment, as well as the help of his staff, Manuel Gonzalez, Donna Wallace and Wayland Seifert. The  authors would also like to thank Mike Santana for his AFM  work and Brennan Davis as research team leader.


1. Seth Prejean, Victoria Bruce, and Joyce Burke,


CMOS Backside Deprocessing With TMAH / IPA as  a Sample Preparation Procedure for Failure


Analysis, Conference Proceedings from the 29th


International Symposium for Testing and Failure


Analysis, 317-323, (2002)


2. Michael R. Bruce, Victoria Bruce, David Eppes,


Jacob Wilcox, Edward I. Cole Jr. Paiboon


Tangyunyong, and Charles F. Hawkins, Soft Defect  Localization (SDL) on Ics, Conference Proceedings  from the 29th International Symposium for Testing


and Failure Analysis, 21-27, (2002)


3. Cordelia P. Sealy, Martin R. Castell and Peter R.


Wilshaw (2000) Mechanism for secondary electron  dopant contrast in the SEM. Journal of Electron


Microscopy 49(2): 311-321


4. Epoxy used to mount die. Epoxy Bond 110 (Item No. 71-100000) by Allied High Tech. Products


5. 3M Jet-Melt TM Adhesive 3797-PG/3797-TC


6. Frank Zachariase, CMOS Front-End Investigation


over Large Areas by Deprocessing from the Back


Side, Conference Proceedings from the 27th


Analysis, 237-241, (2001)


p 105-109


DOI: 10.1361/cp2003istfa105


## A Novel Approach to Front-side Deprocessing for Thinned Die after Backside Failure Isolation


A Novel Approach to Front-side Deprocessing for Thinned Die  after Backside Failure Isolation


Dat Nguyen, Cuong Phan, Jeff Conner, Martin Smith, and John Drummond


With the move to system on the chip (SOC), devices are made  with counts of hundreds of pins.  Bond wire and packaging  solutions for these high pin counts have been flip chip and ball  grid array (BGA).  In addition to the high pin counts, multimetal layers and dummy metal layers, added for chemical and  mechanical planarization (CMP), have hindered the use of  front-side failure analysis (FA).  In these situations, access to  devices with full functionality testing can only be done from  the back side.


While backside FA can be done successfully, gaining access  to isolated defects can be cumbersome and difficult.  Due to  the limitation of photon emission through Silicon [1], it is  necessary to prepare a FA sample and to thin the sample’s  backside to less than 100µm.  Furthermore, with today’s low  power devices, leakages have gone down to the nano-Ampere  region.  Thinned sample preparation has become a necessary  step to get higher sensitivity for fault localization from the  backside.


Thinned samples pose an issue with the removal of the die  from the package, and with gaining access to the defect  location.  While there are techniques for gaining access to the  defect from the backside utilizing Tetra-Methyl-AmmoniumHydroxide (TMAH) [2], there are cases where preference is  given to approaching the defect from the front-side.


In this paper, a novel approach for safe handling of the thinned  die from the front will be described.  The technique can also  be successfully applied to preserve cracked die.


Backside Reconstruction Consideration


During the process of constructing support for the thinned die, considerations went into what kind of materials were to be  used for the support of the thinned die.  Re-deposition of SiO2  or Si3N4, to thicken the backside of Silicon, is not an option, since the deposition process required high temperature (above  300°C), which could cause die cracking.  Epoxy  as a widely  used material in the failure analysis lab for encapsulation  purposes  was investigated first.  Va rious epoxy materials  and  epoxy thicknesses were compared.


Moreover, due to the fragile nature of the thinned die, it is  important to have strong supportive materials and good  bonding to the Silicon surface.  In additions, during the sample


backside reconstruction process, it  is necessary to trim, cut, and polish the sample into easily manageable dimensions.   Also, during the front side deprocessing, the die is exposed to  heat and acids.  Therefore, backside supporting materials need  to possess these four characteristics:


- Good bonding to Silicon surface,


- low Coefficient of Thermal Expansion (CTE),


- withstand the mechanical stresses (tensile strength),


- resistance to acids.


Epoxy’s bonding properties to Silicon can be tested by placing  the cured epoxy -silicon sample in an oven for several hours at  100°C.  The temperature is the normal heat treatment  temperature of the sample during the deprocessing process.  The epoxy material should have a low CTE to prevent over  expansion, which may result in die cracking during the heat  treatment.  As mentioned above, the epoxy should be as strong  as possible to absorb mechanical shock during the cutting, trimming, and polishing process of backside sample  preparation.  Epoxy’s CTE and tensile strength can be found  from the vendors.  Resis tance to acid properties should also be  considered, since front side deprocessing requires the use of  strong oxidizer such as Nitric and Sulfuric acids.  Cured epoxy  sample should be exposed to a tiny amount of Nitric and/or  Sulfuric acids for observation.


Selection of the epoxy materials for the most part came from  experiments.  Different types of epoxies were tried along with  various thicknesses.  Regular casting epoxy which is   transparent, hard, and dense was first investigated.  For  thicknesses less than 5 mm, the supporting epoxy would crack  during handling.  In addition, bonding between the regular  epoxy and Silicon surface was poor (Figure 1).


In order to improve the results the regular epoxy was  thickened substantially.  With the thickening, die cracking and  epoxy separation were still observed during the front side  deprocessing.  Adding a heavy duty epoxy bottom layer was  done next (Figure 2).  With this technique, it is difficult to get  even die surface for polishing, and die cracking was still  observed during high temperature Nitric acid etch.


Figure 1: Application of regular casting epoxy for backside  Silicon support.  Image at the top shows a crack in the epoxy  during device trimming by a diamond saw.   Image at the  bottom shows a separation of epoxy from the Silicon surface  during normal heat treatment at around 100°C.


Figure 2:  Thickened layer of regular epoxy image is at the  top.  At the bottom is an example of combining heavy duty  epoxy and regular casting epoxy.


Heavy duty epoxy  has shown to bond well to Silicon.  Besides, heavy duty epoxy also has high tensile strength, low  CTE, and is resistant to acids.  The CTE value of the heavy  duty epoxy used is about 10.0x10-6/°C.  Normal epoxy has at  least twice that of the CTE of heavy duty epoxy  [3].


In additions, heavy duty epoxy alone is not adequate to keep  the thinned die in place.  A metal plate was selected to stack  over the epoxy to lock it in place.  Kovar metal plate was  selected.  Kovar, which is an iron based alloy with nickel and  cobalt, has CTE values in the range of 3.25 x10-6/°C to 5.0  x10-6/°C, which is close to that of amorphous Silicon CTE  value of 2.5 to 3.5 x10-6/°C [4], at the temperature range of 30  to 100°C.  Kovar has the lowest CTE value compared to any  other metal.  Table 1 lists the thermal properties of various  materials which were under consideration for backside  support.  Kovar metal plates are abundant since they are  widely used as heat sinks for Silicon devices.  A piece of  Silicon, cut out from a scrap wafer without back grind, was  also attempted in the place of Kovar metal plate.  Silicon back  support was subjected to the same tests and the results showed  that it can be used in the place of Kovar.  However, Kovar is  preferred over Silicon for its tensile strength and conductivity.


Table 1: Thermal conductivity properties of various materia ls  under consideration for backside support [5].  Note that  absolute values of CTE for Epoxy and Kovar must be obtained  from the vendors.


Sandwiching heavy duty epoxy between the thinned die and  the Kovar metal plate further lock the epoxy in place and  reduce the expansion. The success of this selection is  described in the following section.


Thinned Die Reconstruction Process


As mentioned above, in order to do an effective back side FA, the sample is thinned down to less than 100µm.  In this report, a flip chip sample with die size of 16mm x 16mm is used to  demonstrate the technique.  The heat sink on the back side of  the flip chip sample was first removed using a razor blade.  The backside is then thinned down by parallel lapping (figures  3-4).  The thinned backside sample is then subjected to fault  isolation such as emission microscopy (EMMI), Liquid  Crystal, Light induced voltage alteration (LIVA ), temperature  induced voltage alteration (TIVA ), etc.


Once the defect has been isolated and deprocessing is needed  to get to the defect, the backside of the sample is reconstructed  for front-side preparation.  The process of the backside  reconstruction and front-side deprocessing includes 1) adding  a grounding strap, 2) applying heavy duty epoxy followed by


CTE       PPM/K


Thermal  Conductivity


PPM/K


W/mK


Silicon 2.5-4.1


150


Alumina


6.7


Aluminum


23


218


Copper


17


Epoxy


10-54


1.7


Kovar


3-5.9


Kovar metal plate, 3) curing of the epoxy , 4) trimming of the  sample to manageable size, 5) removing of the front-side  package materials by parallel lapping and acid etches.


Figure 3: Optical image of the front-side flip chip.


Figure 4: Optical image of the flip chip backside after  thinning to ~40µm.


Since Epoxy  is an insulator, the first step is to provide  grounding to the Silicon backside.  A grounding strap addition  to the backside is necessary for better imaging on the scanning  electron microscope (SEM) and focus ion beam (FIB) tools .  Double sided Copper or Aluminum tape is used as a  grounding strap.  A small piece of conductive tape is used to  apply to both the die and to the Kovar metal plate (Figure 5).   After adding the grounding strap, heavy duty epoxy is applied  to the backside of the sample.  Kovar metal plate is then  placed on top.  Kovar metal plate and epoxy are compressed to  the backside of the sample for support  (Figure 5).


The sample is finally allowed to cure over a warm (40°C) surface for several hours.


Figure 5: Optical images of flip chip backside with Aluminum  tape, heavy duty epoxy and Kovar metal plate for thinned die  backside support.


Front-side Deprocessing


The Kovar metal plate and Epoxy  supported backside sample  is then trimmed into shape for ease of handling using a  diamond saw (Figure 6).


Figure 6: Optical image of trimmed sample after backside  reconstruction.


The sample’s front-side access requires the removal of the  package material.  The front-side package material removal  can be done by parallel lapping down close to the surface of  the Silicon Nitride protective overcoat (PO).  Further removal  of the package materials can be done using concentrated Nitric  and/or Sulfuric acids at high temperature.  The front-side is


now accessible for all regular deprocessing methods such as  parallel lapping and acid etches (Figure 7).


Figure 7: Optical image of front-side package removal.  Picture on the Left, the sample was front-side parallel lapping  close to the die surface.  Picture on the Right, the sample  package materials were further removed with concentrated  Nitric at 90°C.


Examination of the Results


The finished backside reconstruction sample was cross  sectioned for examination using a diamond saw (figures 8-9).  The sample was intact and no die cracking was observed  optically.  The cross-sectioned sample was further polished for  further SEM examination (Figure 10).  The entire length of the  sample was examined, and no micro cracking was observed.


Figure 8: Optical inspection of cross-sectioned thinned die  reconstruction.


Figure 9: Optical inspection of a reconstructed thinned die  cross-section.  This image is 90° counter-clockwise from  Figure 7.


Figure 10: SEM cross-section  examination.


Furthermore, the reconstructed sample with exposed PO, such  as the one in Figure 6, was subjected to heat stress test.  The  test was designed to simulate the temperature treatment of the  sample during the front side deprocessing.  The typical  temperatures are in the range of 90°C to 140°C.  The sample  was subjected to 6 hours of bake with hourly temperature  increases, ranging from 90°C to 140°C.  No cracking of the  thinned die was observed (Figure 11).


Figure 11: Optical image of backside reconstructed sample.  Sample was subjected to 6 hours of baking with temperatures  ranging from 90°C to 140°C.


Front-side deprocessing was then applied to the backside  reconstructed sample.  The die bumps and PO were removed  using parallel lapping and Plasma etches, respectively.  Hydrofluoric acid and an ultrasonic bath was then used to  remove the rest of the metallization for examination purpose (Figure 12).  The sample remains intact.


Figure 12: Optical examination of front side deprocessed  sample down to bare Silicon after backside support.


Materials used for backside reconstruction have to withstand  all standard chip deprocessing techniques.  Especially  important properties are therefore good bonding to Silicon  surface, having low CTE, withstanding the mechanical  stresses (tensile strength); and being resistant to acids.


Reconstruction of the backside of the sample can be done with  the application of heavy duty epoxy and Kovar metal plate.


Backside reconstructed sample withstand the mechanical  stresses such as diamond saw, cross-sectioning polish, and  ultrasonic.  The sample also withstand the heat stress during  the application of acid etches.


The technique has proven to be easily applied and highly  reliable.  The technique provides a solution for front-side  deprocessing for both high pin count BGAs and flip chips.


The authors would like to thank Bilal Abd-AlRahman for his  helpful inputs into this project/paper.


1) D. Davis, O. Leon, C. Hughes, S. Pabbisetty, R.


Parker, C. Scott, C. Todd, J. Widaski, G. Wilhite, S. Wills, and J. Zhu, “Advanced Microprocessors


Through Backside Approaches ” p 472, 24th ISTFA


Proceedings, 1998


2) S. Liebert, “Failure Analysis from the Backside of a  Die”, p 177, 26th ISTFA Proceedings, 2000.


3) H. Lee and K. Neville, Handbook of Epoxy Resins, p  6-27f; p 17-15ff, McGraw-Hill Book Company, New  York, New York (1967).


4) J. Fabian and P. Allen, “Thermal Expansion and


Gruneisen Parameters of Amorphous Silicon: A


Realistic Model Calculation”, Physics. Review


Letters, p 79, Vol. 1885, State University of New


York at Stony Brook, Stony Brook, New York


(1997).


5) C. Zweben and K. A. Schmidt, “Advanced


Composite Packaging Materials”, Electronic


Materials Handbook, p.150, ASM International,


Materials Park, Ohio (1989)


Jeff Birdsley • Dell Computer Corporation • Round Rock, TX


# Session 5: System Level Analysis 


p 111-119


DOI: 10.1361/cp2003istfa111


## Dynamic Infrared System Level Fault Isolation


Dynamic Infrared System Level Fault Isolation


John A. Naoum, Johan Rahardjo, Yitages Taffese, Marie Chagny, Jeff Birdsley, John C. Woo and  Aaron Morris


Dell Inc.  Austin, Texas, USA


The use of Dynamic Infrared (IR) Imaging is presented as a  novel, valuable and non-destructive approach for the analysis  and isolation of failures at a system/component level.


Over the years, the Failure Analysis (FA) community has  strived to develop low cost, efficient and time saving methods  for the non-destructive isolation of failures. In the PC industry, more complicated designs and smaller, highly populated  systems are an ever-increasing challenge for timely and  effective FA.  Due to these constant technological  advancements and changes in the incoming System Under  Test (SUT), many tools have become obsolete and are no  longer effective for FA.


Utilizing a test setup integrating an IR camera and image  subtraction software, static IR system level fault isolation is a  proven FA approach [1]. This approach is implemented by  placing a known good SUT and then a suspect failing SUT  under the IR camera.  Both are electrically exercised into a  known time static mode, and then a snapshot thermal image of  each SUT is acquired. These images can be subtracted  providing a method for isolating differences in the thermal  signatures between known good and suspect systems.  This  technique provides a non-destructive but limited approach in  isolating a failing component on the SUT.  Limitations of the  static approach include the inability to detect “timedependent” or “test specific” failures (that are not easily  detectable in static environments), the lack of real-time  comparisons, and the time consumption required for the SUT  to stabilize in a known static state in order to capture a  relevant image.


A more effective approach has been developed through the use  of Dynamic IR Imaging for system level fault isolation. Similar to the static IR approach, a good known SUT and then  a suspect failing SUT are placed under the IR camera. In  contrast to the static approach, the failure analyst does not  have to wait for the SUT to stabilize in a known static state  before acquiring the thermal image.  In addition, timedependent and test specific failures can be identified.  In any  exercised state, a real time thermal image can be captured


immediately and saved in an Audio/Video Interleaved (AVI) file format. This saves time and allows the investigation of  dynamic, time-based failure conditions through the captured  thermal images. While no commercially available software  has been identified to subtract two AVI files, Dell has  developed a method to separate two AVI files into frames, subtract the individual images frame by frame and reconstruct  the result into a third AVI file, thus allowing a dynamic image  subtraction comparison for the isolation of time-based system  level failures that may be specific to a particular dynamic  condition.


This paper will briefly review the theory of IR thermography  including the environmental (i.e. room temperature vs. SUT  temperature) and material (i.e. differences in emissivity) constraints that have to be taken into account. It will describe  in detail how this Dynamic IR Imaging approach is useful in  isolating time-based or test specific failures.  It will also  describe the software and the programming methods used to  achieve Dynamic image subtraction. . It will discuss the  advantages and disadvantages of conducting Dynamic IR  Imaging analysis using the AVI file format. It will conclude  by summarizing the results of our experiments and stating the  advantages as well as disadvantages of using this Dynamic IR  Imaging system level failure isolation approach.


Infrared technology was discovered in 1800 by the astronomer  Sir William Herschel. After a series of experiments; “Herschel  discovered invisible infrared rays off the red end of the visible  spectrum” [2].  For the years to come many physicists such as  Joseph Stephan, Ludwig Boltzmann, Max Planck among  others, helped further develop this discovery, into what is  presently known as one of the fastest evolving methods for the  non-destructive analysis of a device under test: Infrared  Thermography. There are unlimited applications for the use of  Infrared Thermography but it all comes down to one basic  idea: “all objects above absolute zero (-459 oF, -273oC) give  off invisible infrared radiation” [2].


The following manuscript builds its foundation on the use of  infrared thermography applied to Dynamic Infrared system  level fault isolation. Based on the theory of IR thermography, and the use of an Infrared Camera, a series of comparative  time-dependent experiments, using computer motherboards as  the systems under test, were conducted. The results were  obtained by developing a video subtraction software tool for  the comparison of video recordings of a good known system  versus a failing system under test.


The sections to come will describe and discuss the theory, methods and results in using the Dynamic Infrared approach, concluding with the summary of the results and the  opportunities for improvements.


standards in the set require a double read time.  After  creation of the calibration program, a test read of 30 seconds  is made on the last four standards in each set to verify the  accuracy.  We set a limit of +/- 5% for the top (gold) layer  and +/- 10% on the second (nickel) layer.  If any of these  limits are exceeded, a re-calibration is performed on that  standard location.


XRF machine aperture selection for creation of a  calibration program should be based on the sample being  read.  The general rule of thumb is to select an aperture that  is about 1/3 of the sample width.  This leaves sufficient  sample area on either side of the measurement site.  Using  the largest aperture that fits these guidelines will result in  the most precise reading.  Smaller size apertures will result  in lower count rates yielding wider variation.


If the finger is narrow or the selection of available apertures  is limited, bromine from the board can impact the  measurements by artificially increasing the gold readings. (See Figure 4 for the energy spectrum.)   As a result, many  XRF machines include numerical filtering to compensate for  the influence of the bromine.


The highlighted peaks in the spectrum in Figure 4 show an  area of overlap between the Au Lβ and the Br Kα regions of  interest. Measurements were made on a bromine reference  to determine the contribution bromine makes in the Au  region of interest.


Figure 4: Area of spectral overlap between Au and Br


To determine the bromine effect, we performed the  following study.  Fingers were selected on a test board and  read edge to edge across their length with two different  calibration programs.  One program included a numerical  filter for the bromine influence while the other program  didn’t.


The gold plating thickness represented in the program  without bromine compensation shows a bathtub curve when  read edge to edge across the width.  See Figure 5.


25 30 35 40 45 50 55


Thickness


Gold Plating    across finger


Figure 5: Au readings across the finger without bromine  compensation


The same finger was read with a program which includes  the bromine compensation. It shows a much flatter plating  level across the width.  See Figure 6.


Au Thickness              with Bromine Compensation


Figure 6: Reading across the finger with bromine  compensation


In order to determine which program better represents the


actual gold plating, we selected fingers for a single line XRF  reading across the width (See Figure 7).  Both programs


(with and without Bromine compensation) show a midfinger thickness of around 36 microinches.


Au Thickness   in microinches


Comparison of GOLD Readings  with w/o Br and w/Br compensation


w/o Br w/Br


Figure 7: Comparison of gold reading across the finger  with and without bromine compensation


We metallurgically sectioned the fingers from the board, backplated them with an edge protection metal (to maintain  the true gold thickness) and mounted the sample areas in  epoxy.  The sample mount was ground, polished and  chemically etched.  Measurements were then taken on one  gold finger in the cross-section with a SEM (Scanning  Electron Microscope).  The Au thickness at the left side of  the finger (Figure 8) read 36.40 micro-inches. The Au  thickness in the middle of the finger measured 36.91 microinches Figure 9. Near the right side the thickness measured


35.93 micro-inches (figure 10).  Based on this empirical  data, the program utilizing bromine compensation more  accurately matches the true plating thickness of the gold  plating layer.


Figure 8: SEM image showing Au plating at the left end of  the Au finger


Figure 9: SEM image showing Au plating in the middle of  the finger


Figure 10: SEM image showing Au plating at the right end  of the finger


Accuracy and Precision:


A check to determine the accuracy and precision of the XRF  instrument was performed.  One of the standards (44 micro  inches of Au) was selected for 100 reads in a single spot and  100 random reads across a grid on the surface.  The  resulting data was then plotted in Figure 11 and Figure 12  The center point of the graphs is 44 micro-inches and the  outer circle is 46.2 micro-inches (max limit + 5%). The  measurement results on both graphs are very close to the  target thickness of 44 micro-inches, establishing both  accuracy and precision on the XRF tester.


100 readings on the same spot


44.00


46.00


234567891011121314151617181920212223242526272829303132333435363738394041424344454647484950


51


52 53 545


5758


596061


6263646566676869707172737475767778798081828384858687888990919293949596979899100


Mean = 44.3


StdDev = 0.2671


USL =  46.2


LSL =  41.8


Sigma Capability = 8.612 Cpk = 2.3708


Cp = 4.7542


D.P.M. = 0.000


Figure 11: 100 readings were made on the standard at one  spot


100 Readings in 100 random spots


5960


616263646566676869707172737475767778798081828384858687888990919293949596979899100


Mean = 43.9821


StdDev = 0.3234


Sigma Capability = 8.248 Cpk = 2.2493


Cp = 2.2678


Figure 12: 100 readings were made on the standard at 100  random spots


Sample Parameters:


The orientation of the sample in the chamber also impacts  the reading.  The board should be positioned with the length  of the fingers parallel to the y axis in the chamber. Hardware configuration of the detector and proportional  counter dictates this optimal orientation. Laser focusing in  this machine insures exact Z positioning of the standards  and the test samples.


Case Study:


The option card with the high reseat failure rate was  manufactured using raw boards from four different suppliers. By reviewing the process fallout data, it was determined that  reseat failures were occurring with only two of the four raw  board suppliers used in the manufacture of the option card.  A sample option card utilizing a raw board from each of the  four different board suppliers was obtained.  XRF testing  was performed across the contact fingers of each board to  determine if there was a correlation between gold thickness  and the reported failures rates.


Based on the XRF test results, a relationship between the  suppliers of the failing raw boards and the process fallout  was apparent.  The boards experiencing high reseat rates  were found to have very thin plating of contact finger gold (Suppliers #3 and #4).  See Figure 13.


Based on this empirical data, option cards manufactured  with bare boards that averaged 1.7 micro-inches (Supplier #3) and 2.22 micro-inches (Supplier #4) of gold showed  excessive reseat failure rates due to high contact resistance  of the plating interface.  This anomaly was not observed on  the option cards manufactured with bare boards measuring


6.23 micro-inches and 9.94 micro-inches of gold plating.


To determine the proper selection of contact finger plating  thickness, one must also consider other factors which can  affect the long term usability of a plating finish.  The  number of insertions/removals of the card during its test and  end use can impact the plating finish.  The use environment (humidity, heat, etc) also needs to be considered when  specifying the plating requirements.  These external factors  will accelerate the oxidation of the nickel (and copper, if the  nickel itself is thin) resulting in high contact resistance.


GOLD Thickness on Contact Fingers


0 2 4 6 8 10 12


Supplier #1 Supplier #2 Supplier #3 Supplier #4


Figure 13: Comparison of the gold plating thickness on the  four different raw cards


Conclusion:


Intermittent continuity of contact fingers is one of the more  difficult failures to identify in a high volume production  process.  Proper determination of the application/end use  needs with qualification and control of the supplier base for  raw cards will greatly reduce the occurrence of marginal  plating thickness issues.


X-ray fluorescence is a preferred method of measuring  plating thicknesses because it saves time versus traditional  metallurgical methods, in addition to being accurate and  non-destructive.


There are several factors which impact the accuracy and  repeatability of XRF plating thickness measurements.  Knowing what these factors are and knowing the


limits/features of the XRF tester can minimize errors in  plating measurements.


1. J.P. Willis, Course on Theory and Practice of XRF  Spectrometry, Lecture notes Week 1 and 2,


Department of Geology, University of Western


Ontario, (August 1991)


2. EDAX DX Prime Training Course, EDAX


International, (December 7-11, 1998)


3. XRF-4000 and XRF-5000 Series User manual, XPert for Windows TM Software Releases v1.05


Veeco UPA Technology, (August 1996)


# Session 6: Metrology and Materials Analysis 1 


William E. Vanderlinde • Laboratory for Physical Sciences College Park, MD


p 132-139


DOI: 10.1361/cp2003istfa132


## Real Time SEM Imaging of FIB Milling Processes for Extended Accuracy on TEM Samples for EFTEM Analysis


Real Time SEM Imaging of FIB Milling Processes for Extended   Accuracy on TEM Samples for EFTEM Analysis


P. Gnauck, U. Zeile, P. Hoffrogge, G. Benner, A. Orchowski, W-D. Rau


LEO Electron Microscopy Group, Carl-Zeiss-Str 56, D-73447 Oberkochen, Germany


We present application examples of site specific energy  filtered transmission electron microscopy (EFTEM) analysis  using advanced focused ion beam (FIB) specimen preparation  techniques. Specifically, we address topics such as throughput  and reliability enhancement by chemically assisted broad ion  beam milling and on-line monitoring of the etch process. We  discuss how integrated elemental analysis by EFTEM can be  used to gain quantitative information on the broad variety of  new material systems currently entering front end and back  end of the IC manufacturing process line.


The accelerating pace of device integration results in extreme  demands for quantitative analysis in process development, yield ramp-up and process control with spatial resolution and  elemental sensitivity at the very limits of currently available  instrumentation. Historically, the high resolution performance  of TEM analysis has been hampered by long turn around times  for the required sample preparation. Meanwhile the routine  use of FIB systems for “trench” and “lift-out” preparation  techniques allows for an enormous increase in the efficiency  of TEM analysis.


The standard FIB cross sectioning is basically a blind process. The sample surface is imaged with the FIB before cutting to  determine the area of interest. Then the sample is milled and  polished with predefined milling patterns. Without the  possibility of simultaneous monitoring of the milling process  the area of interest is easily destroyed. The capability of  CrossBeam technology to image the sample in real time at  high resolution during the ion milling process using a field  emission e-beam enables the operator to perform extremely  accurate site specific cross sections. The milling and polishing  process can be stopped exactly at the detail of interest e.g. in  the very center of a certain transistor in a semiconductor  device. In TEM sample preparation the real time SEM  imaging allows for very tight control of the sample  thickness/transparency and the danger of destroying the fine  lamella is reduced to a minimum. The FIB lift-out technique


allows thin membranes to be extracted from bulk material, which saves sample pre-thinning time and is very successful in  the preparation of site specific cross sections and planar  samples. To a large extent TEM sample preparation can be  automated by using scripts and macros. However, the best  compromise concerning time and accuracy is achieved if  different samples are pre-thinned automatically overnight to a  thickness of about 1µm and then polished manually under  high resolution SEM observation. For the final investigation of  the TEM lamellae energy filtered analysis allows for optimum  image contrast even for thicker samples or heavy material  structures in back-end analysis since the chromatic blur from  inelastically scattered electrons can be eliminated. By  selecting appropriate energy loss windows element specific  contrast enhancement and quantitative determination of 2D  composition distributions can be achieved. Moreover, using  the small probe size of current FEG instruments, spectroscopic  analysis in STEM and nanoprobe modes can reveal  composition and interface properties on the sub-nanometer  scale.


TEM Sample Preparation


Conventional TEM preparation techniques


Conventional preparation techniques for cross sectional TEM  samples are a combination of mechanical grinding polishing  and ion milling (Fig. 1). These techniques suffer from the fact  that they are very time consuming and that it is extremely  difficult to do site specific cross sections. Conventional ionmilling techniques for TEM specimen preparation are  essentially blind. Thus, it is left to chance whether the  specimen detail of interest is suitable for TEM-imaging (many  specimen areas are too thick). Even if subsequent ion milling  of TEM specimens is possible in external ion milling stages it  is a tedious and mostly uncontrolled procedure. Because  continuous high resolution control of the ion milling process is  not possible, the specimen areas of interest may easily be  destroyed.


Fig. 1: Steps during the cross sectional TEM preparation  using dicing, grinding, dimpling, polishing and broad ion  milling.


TEM Sample Preparation using FIB


Introduction of the focused ion beam technique into TEM  sample preparation was a big advantage regarding time  consumption and the possibility of being site specific. The  sample surface is imaged with the FIB before cutting to  determine the area of interest. Then the sample is milled and  polished with predefined milling patterns (Fig. 2). In the final  step the sample can be cut out of the substrate and transferred  to a TEM grid. But as only the sample surface is imaged even  the standard FIB cross sectioning is basically a blind process. Without the possibility of simultaneous high resolution  monitoring of the milling process the area of interest is easily  destroyed.


Fig. 2: Steps during TEM sample preparation using a FIB: 1. Sample definition and rough milling 2. Fine milling and final  polish 3. Cut and lift out.


TEM Sample Preparation using the CrossBeam technique


The solution for the problems described above is the  combination of a FIB system with a high resolution field  emission SEM to allow high resolution real time imaging of  the ion milling process. In this case a detail of interest cannot  be missed or destroyed. Another advantage of this approach is  the charge compensation on insulating materials as ceramics, oxides and resist material.


To do the sample work the LEO1540XB CrossBeam  Workstation was used. The system combines a high resolution


GEMINI Field emission column with a CANION 31+ FIB  column. The tool was equipped with a five channel gas  injection system (GIS) for deposition and enhanced etching  and with an annular STEM detector to perform brightfield and  darkfield STEM imaging at sub nanometer resolution.


Fig. 3: Geometrical layout of the LEO CrossBeam system. The  electron and the ion beam coincide at a crossover point 5mm  below the objective lens of the SEM.


Electron Optics


To examine nonconductive samples like photo resist, oxide  layers, ceramics etc. in their natural state (i.e. without  significant sample preparation like coating etc.) in the SEM  the technique of low voltage scanning electron microscopy (LVESEM) is used. The operation at low electron energies  reduces the charging of the sample and gives a very accurate  information of the very surface of the specimen. However the  resolution of a standard SEM is drastically reduced at low  beam energies.


The probe size dp of an electron optical system is given by:


Sp


So


with the virtual source size dSo, the chromatic aberration disc  dC, the spherical aberration disc dSp and the diffraction error  dD.


Chromatic aberration:


The focal length depends on the electron energy. Due to the  energy spread of the electron gun this results in a disc of least  con fusion with the diameter


α⋅


∆


⋅


E E


Where CC is the chromatic aberration coefficient,  ∆E the  energy spread of the gun, E the beam Energy and α the  aperture limiting semi angle.


Sample


GIS


SEM


FIB


Spherical aberration:


If parallel beams are incident on an electron lens, those further  from the optical axis are focused closer to the lens: The  resulting beam diameter in the Gaussian image plane, which is  the focal plane for the paraxial rays, is 2 CS α3 and in the plane  of least confusion the diameter is


0 αS


S


d =


Diffraction error:


The beam limiting diaphragms in the probe forming lenses  that limits the aperture to keep the spherical aberration  acceptably small causes a diffraction pattern to be formed in  the focal plane with the diameter


α


λ


6.0


(4)


The beam aberrations are minimized by the special design of  the GEMINI lens [1]. Due to the design as a combination of a  magnetic lens together with an electrostatic immersion lens (Fig. 4), the aberration coefficients decrease with decreasing  electron energy (Fig. 4). This results in an ultrahigh resolution  even at very low energies down to 100eV.


0 5 10 15 20 25


Beam Energy [KeV]


Cs


Cc


Fig. 4: Design and aberration coefficients of the GEMINI  lens: Due to the design as a combination of a magnetic lens  together with an electrostatic immersion lens spherical and  chromatic aberration coefficients CS and CC scale with the  beam energy. The dotted lines represents the constant  aberration coefficients CS and CC of a classical magnetic  electron lens.


The schematic layout of the electron optics of the Gemini  column is displayed in Fig. 5. The electron beam is generated  by a Shottky field emission gun. This kind of emission system  is characterized by a high brightness, a low energy spread and  a small virtual source diameter. The probe forming is done  mainly by a magnetic electrostatic compound lens. The  condenser lens which is located directly below the gun area is  mainly used for adjusting the optimum beam aperture in the  low voltage operation. This results in a crossover free beam  path with minimum Boersch effect and a minimized energy  spread ∆E. The beam current is adjusted by the use of a  software controlled electromagnetic aperture changer.


Another benefit of this design is the absence of a magnetic  field at the sample. Therefore the electron optical and ion  optical properties of the area between sample and final lens of  the SEM never change regardless of focusing or EHT change  on the SEM. This is an essential feature for the real time SEM  imaging of the ion milling process.


Fig. 5: Schematic layout of the electron optics of the GEMINI  column (right) and the light optical analogon of the column (left). The gray lenses represent the magnetic condenser lens  and magnetic part of the objective lens. The white lenses  represent the electrostatic immersion lens. Please note: This  light optical analogon is only a rough approximation of the  real electron optical properties of the system.


Ion Optics


The schematic layout of the ion optics is displayed in Fig. 6. Gallium ions (Ga+) are extracted from a high brightness liquid  metal ion source and then accelerated to an energy of 5 keV - 30 keV. The ion emission is regulated by an extractor. The  electrostatic condenser lens collimates and focuses the ion  beam depending on the operating mode: Crossover beam path  for highest beam current or non-crossover for best imaging  performance. After passing the condenser lens the beam  current is defined by a set of software controlled mechanical  apertures. By using the different apertures in combination with  different condenser settings the probe current can continuously  be adjusted in the range between 1pA for and 50nA. The  objective lens is designed as an electrostatic einzel-lens  system. It focuses the beam onto the specimen surface. At the  normal working distance of 12mm a resolution of better than  7nm can be achieved.


magnetic lens


electrostatic lens


condenser lens


apertures


Fig. 6: Schematic layout of the ion optics of the CANION 31  FIB column. The ion beam is generated by the LMIS and  focused onto the specimen by an electrostatic two lens system. Crossover beam path for highest beam current on the left and  the normal collimated beam path for optimum imaging  performance on the right.


Imaging modes


The CrossBeam system can operate at three different imaging  modes. By blanking the ion beam and only using the electron  beam for imaging the system operates as high resolution field  emission SEM. The second imaging mode uses the ion beam  while the electron beam is blanked. The FIB imaging mode is  used for grain analysis, voltage contrast imaging and the  defining of milling areas. The last imaging mode is the so  called CrossBeam operation mode: Both beams are turned on  and while the ion beam is milling a defined area, the SEM is  used to image the milling process at high resolution in real  time. This enables the operator to control the milling process  on a nanometre scale and to perform extremely accurate cross  sections and device modifications.


SEM imaging


If the system is used as a high resolution SEM only the ion  beam is blanked and the secondary electron (SE) signal is  synchronized to the SEM scan. In this operational mode the  system can be used as a high resolution FE-SEM with no  limitations. Figs. 4 and 5 show the principles of operation of  high resolution low kV SEM images in this operating mode.


Fig.7: SEM imaging: The ion beam is blanked and the SE - signal is synchronized to the SEM scan.


Fig.8: High resolution low voltage (800V) SEM image of an  uncoated photo resist structure on a silicon wafer


FIB Imaging


If the system is used as a FIB only the SEM beam is blanked  and the signal is synchronized to the FIB scan. This mode is  used for channelling contrast imaging, voltage contrast  imaging and for defining milling patterns on the sample  surface.


LMIS


condenser lens apertures


objective lens  specimen


SED


Fig. 9: FIB imaging: The electron beam is blanked and the SE


- signal is synchronized to the FIB scan.


Fig. 10: FIB imaging: Channelling contrast and voltage  contrast in a semiconductor sample.


CrossBeam operation


To monitor the ion milling process in real time at high  resolution in the SEM the CrossBeam operation is used. Both  beams are turned on and while the ion beam is milling a  defined area, the SEM is used to image the milling process at  high resolution in real time. This enables the operator to  control the milling process on a nanometre scale and to  perform extremely accurate cross sections (Fig. 13) and device  modifications.


This mode also provides an easy way to compensate charging  on non conductive samples. The sample is irradiated by the  positive ion beam and the negative electron beam at the same


time. The result is an easy way of charge compensation on the  sample surface.


Figure 11: CrossBeam operation: Both beams are scanned  completely independent form each other and the SED Signal is  synchronised to the SEM scan. This results in the CrossBeam  operation feature: The ion milling process can be imaged  using the SEM in real-time.


Another benefit of this mode is the easy control of the  specimen thickness during ion milling.


Inlens Detector


ET-Detector


eeeeFig 12: Geometrical position of the sample and the detectors  during ion milling in the CrossBeam. The Inlens detector is  located in front of the sample and records information about  the sample surface. The ET (Everhard – Thornley) detectector  is located behind the the sample and records SE that are  emittet from the backside of the sample.


As the sample gets thinner the primary electrons start  penetrating the sample and generate secondary electrons on  the backside. These electrons can be detected by using the


Everhard-Thornley detector which is geometrically located  behind the sample (Fig. 12). This signal gives a direct  information about the thickness of the sample: The thinner the  sample, the brighter the image. To do exact measurements of  the sample thickness the brightness of the signal can be  calibrated for certain materials [2]. At the same time the  sample surface can be imaged using the inlens detector which  is geometrically located in front of the sample and collects  mainly secondary electrons the are emitted from the sample  surface (Fig. 12). By combining both signals during the ion  milling in a split screen mode the complete information about  the sample (location, surface detail and thickness) can be  displayed at the same time (Fig. 13).


Fig. 13: Live imaging of semiconductor TEM sample during  ion milling in split screen mode. While the Inlens detector on  the left displays information about the sample surface the  Everhard-Thornley detector signal on the right provides  information about the transparency at the same time.


Fig. 14: Live imaging of a TEM sample during ion milling. While the location of the sample can be montored at high  prcission (the plugs are cut exactly in the center), the electron  transparency can easily determined by the brighter contrast (note different brightness for different elements).


The real time imaging enables extremely accurate and site  specific cross sections. Fig. 15 displays an example of a sub µm defect in a semiconductor sample that could be located by  using the live imaging possibilities of the CrossBeam. The


image was taken using the STEM mode of the CrossBeam  system.


Fig. 15: 30kV brightfield STEM image of a Semiconductor  structure.


EFTEM Basics


Electron scattering in specimen


During elastic scattering at the specimen atoms, primary  electrons with E0 energy are scattered at large angles Θ  without losing any measurable energy. Inelastically scattered  electrons only scatter at small angles, but lose energy and thus  change their wavelength. Elastically scattered electrons remain  monoenergetic and display an energy bandwidth δE which  largely defines the cathode. The bandwidth of inelastically  scattered electrons, on the other hand, increases drastically  with greater mass and specimen thickness.


5.2b and 5.2c


• To perform a good analysis of an IR image one must  consider the following:


o The higher the emissivity of an object (low  reflection), the more closely the thermal image  represents the SUT temperature


o  The lower the emissivity of an SUT (higher  reflection) the more closely the thermal image  represents the SUTs surroundings


o  If the SUT is at ambient temperature or at the same  temperature of its surroundings, the emissivity  characteristics disappear


• The IR camera must be complemented by the appropriate  software in order to acquire, analyze and achieve  Dynamic IR analysis.


• Additional opportunities to improve Dynamic IR include: o Real-time video alignment


o Aligning specific logic functions or test timing  sequences on the SUT with image acquisition


1. J. Swart, J. Woo, R. Zumwalt, J. Birdsley and Y. Taffese, ISTFA 2002, pp. 631-641.


2. Advanced Infrared Resources, Level 1 Infrared  Thermography Manual, Rev. 0302, Canada, pp 1-70


3. Indigo Systems, Merlin Mid User’s Guide, Publ No. 414-0001-10 Version 1.1, pp.1


p 120-124


DOI: 10.1361/cp2003istfa120


## X-ray Laminography Benchmarking and Failure Analysis of Solder Joint Interfaces


X-ray Laminography Benchmarking and Failure Analysis of Solder Joint  Interfaces


Barbara A. Thomson,  Norman J.  Armendariz


Intel Corporation, Hillsboro, OR, USA


A new generation X-ray laminography (XRL) automated Xray inspection (AXI) tool was evaluated for surface mount  technology (SMT) assembly defect detection and was  qualified using formal “benchmark” comparative analysis  processes.  In addition, defect characterization was performed  using the XRL AXI system in manual X-ray inspection mode  to correlate various failure modes and mechanisms at SMT  solder joint interfaces for selected non-destructive failure  analyses and technology development.


Since ball grid array (BGA) solder joint quality is a great  concern in board assembly, test technology development and  failure analysis teams explored the use of XRL AXI as a  method to detect and monitor BGA ball abnormalities using  XRL AXI-generated solder ball images and measurements. It  was found that XRL AXI was able to successfully discern  differences in the shape, location and diameter of the suspect  BGA solder balls from XRL AXI horizontal image planes (slices) for physical failure analysis and reliability issues not  previously detected using conventional X-ray transmission or  electrical methods.  Subsequent metallographic x-sectioning  correlated the XRL AXI mages to the physical condition of  the suspected second level interconnect (SLI) solder joint  location.


X- Ray Laminography


X-ray laminography is an automated X-ray inspection  technology, which is used primarily for in-process highdensity surface mount technology board assembly verification, i.e., at the second-level interconnect.  XRL is a programmable  radiographic 3-D technology, which essentially provides a  focused image slice at a selected plane of a solder feature and  analyzes the images using a set of algorithms. Subsequent data  processing provides measurement data for both process  monitoring and feedback, as well as for supplementary  electrical and materials failure analysis information.  It is  especially useful in cases where in-circuit test (ICT) has  diminished feasibility due to loss of test-point access, test  development time-constraints, and increasing product  complexity. Another capability of XRL technology is its use  as a non-destructive metrology for selected failure analysis


and, more importantly, preventive failure analysis before  reliability issues escape into the field and fail. A comparison  of the mechanics of XRL and conventional transmissive X-ray  is shown in Figure 1.


Figure 1:  Shows a schematic comparing conventional (XRT) X-ray transmission (L) vs. (XRL) X-ray laminography (R).  The XRT shows all the components in the field of view as  compared to the XRL which looks at a defined plane, or “slice”, of interest.  Source: Agilent Technologies.


When the XRL AXI system is used in the in-process  manufacturing environment, it is programmed for each printed  board assembly (PBA) design. The programming inputs  include PBA CAD data and a library of algorithms that  provide measurement parameters for each type of solder joint.  Table 1 shows XRL AXI data processing algorithms and their  respective measurement parameters. The program is then “tuned” using a set of known good boards to accurately  capture solder joint defects with a minimum of “false calls”.


Typically all boards that have suspected failures will then be  routed to an off-line X-ray debug and review station, where a  trained technician will view the X-ray images of the indicted  solder joints, and determine the status of each call.


Table 1: XRL AXI algorithms and measured parameters. Source: Agilent Technologies.


Gullwing


Heel, toe, center thickness, average solder  thickness (volume)


J-Lead


TAB


Heel, toe, and center thickness, fillet length


SOT


Fillet and under-pin thickness, average  solder thickness (volume), component  rotation


Radius and circularity at pad, ball, and


package, annular ring thickness


Passive Chip Average solder thickness (volume), offsets, polarity (PCap only)


Fillet and barrel average solder thickness  and radius


LCC


Fillet volume and diameter


Solder Paste  Volume, average solder thickness, pad  coverage


Comparative Benchmark Study


Intel Corp. performed a comparative benchmark evaluation of  two 3-D AXI systems which use different methods to capture  and analyze X-ray images. One system used XRL technology  while the second supplier used digital tomosynthesis which  acquires a set of digital pictures of each solder joint and then  digitally synthesizes a 3-D image of that joint. The AXI  benchmark vehicle used was a complex motherboard with  9300 solder joints including components such as chip scale  packages (CSP), micro-BGA, BGA sockets, fine pitch SMT  connectors, and fine pitch ICs. The double-sided active board  design provided additional complexity to X-ray imaging due  to overlapping components on both sides. The two AXI  suppliers were required to develop and debug a complete test  for the benchmark vehicle in 24 working hours over several  days under the supervision of Intel personnel. The test was  then implemented on a set of boards so that parameters such as  test times, false call rates, defect detection capabilities, and  hardware and software capabilities could be measured and  compared. Suppliers were also rated on global hardware and  software support capabilities, system costs, and improvement  roadmaps (Table 2). Intel selected the XRL AXI system at the  conclusion of the evaluation.


Table 2: Benchmark criteria categories for AXI supplier  selection are shown.


Supplier Capability • System cost


• Supplier service/support


• Customer installed base


• Product maturity


Tester Capability • Test development tools


• Debug and CAD tools


• Physical board constraints


• Camera capabilities


Manufacturing


Capability


• Test time/beatrate


• Maintenance requirements


• Operator/debug interfaces


• Safety/EHS


• Data collection


Quality and  Reliability


• Alpha and beta rates


• Solder defect/problem detection


• Hardware and Software reliability


• MTTR and MTBF


XRL AXI Technical Certification


Additional technical certification of the Agilent XRL AXI tool  was conducted to evaluate use in Intel circuit board  manufacturing sites in high and low volume environments and  assess value as a failure analysis tool. A complex server board  with double-sided configuration, including 1000 passive  components on the secondary side, was used as the technical  certification vehicle, Table 3.


Table 3: The technical certification evaluation test vehicle  used was a complex double- sided server board.


The AXI test program for the technical certification board was  developed by an Intel test engineer trained in AXI test  development on the Agilent 5DX.  Data from three kits  totaling 296 boards of production level server base boards  built at Intel’s System Manufacturing facility was captured for  the certification. Each board was tested twice: once postreflow and once post-wave, for a total of 592 board test runs. At post reflow, solder joints for all SMT components were  inspected at XRL AXI, while at post-wave, both SMT and  through-hole components were inspected. In both cases, the  XRL AXI step was passive and data was captured, but no  repairs were made. The boards were then passed down to the  next assembly step.  Results are shown in Table 4.


Westville Base Board


Post-Reflow Post-Wave


Number of Components


2,400


2,500


Number of Solder Joints


12,400


14,500


Number of Nodes Board size


12" x 13" double-sided  3,900


Server Base Board


Table 4 shows the results of the server base board evaluation  portion of the AXI technical certification. Data in yellow did  not meet certification goals. DPMO = Defects per million  opportunities (false calls per million solder joints tested). UPH = Units per hour.


Post-reflow


Post-wave


Test time (align/map/test)


< 2 min.


1 min. 51 sec.


2 min. 23 sec.


Board disposition time


1 min. 46 sec.


1 min. 21 sec.


Beatrate (whole module)


> 25 UPH


30 UPH


23 UPH


MCBA (mean cycles between assists)


> 100 cycles


MCBF (mean cycles between failures)


> 2000 cycles


Alpha rate (solder joint level)


< 2000 DPMO


510 DPMO


731 DPMO


Beta rate (component level)


< 10%


0.5%


3%


Actual


296 cycles no failures


Targets


XRL AXI met all certification goals for boards tested at postreflow, but two goals were not met on boards with SMT and  through-hole tested post-wave. This was due to the longer test  and inspection times related to the increased number of solder  joints inspected and reviewed after the wave process step.  XRL AXI was also compared to other test steps, including  manual (or human) visual inspection (MVI) and in-circuit test (ICT). XRL AXI was found to detect a far greater number of  defects and solder abnormalities than the other two techniques.  1442 out of 1450 defects were detected at the XRL AXI step, with 8 test escapes. This correlates to a 0.5% beta (test escape) rate. Defects detected by XRL AXI, MVI, and ICT are shown  in Figure 2.  Figure 3 shows the details of defects that escaped  detection at the XRL AXI step, but were detected at ICT or  MVI.


0 10 20 30 40 50 60


Short Shift/Skew passive


Open Missing Void Insufficient Lifted Pin Shift/Skew IC


BGA ball misaligned


Post-reflow assembly defects found @ AXI, MVI, ICT (not shown: 1254 squeeze balls)


MVI or ICT   AXI + ICT   AXI + MVI    AXI ONLY


Figure 2: Solder joint defects detected at XRL AXI, MVI, and  ICT on server test vehicle post-reflow boards are compared. Not shown in the chart are over 1200 solder balls or “squeeze  balls” detected at XRL AXI which occurred due to poor design  of solder paste stencil. Only squeeze balls over 0.010” in  diameter were counted.


0 1 2 3 4 5 6


Short


Open


Insuff.


Post-reflow defects not detected @ AXI


Figure 3: Details of the defects that were not detected by the  XRL AXI system at post-reflow are shown.


The chart in Figure 4 shows the results of defect detection at  the post-wave step, including inspection of both SMT and  through-hole solder joints. At post-wave, a total of 896  components with assembly defects were found by XRL AXI, MVI, and ICT. AXI detected 879 out of 896 defects, with 17  test escapes, or a beta (test escape) rate = 17/896 = 2%. One  interesting note is that out of the 1254 squeeze balls found at  the post-reflow step, only 671 remained at the post-wave step. Apparently the solder balls migrate and possibly melt during  wave. Some were found to have become lodged between the  pins of IC devices.


0 10 20 30 40 50 60 70 80


Short Missing Shift/Skew passive


Void Insufficient Lifted Pin TH lead not thru


Shift/Skew IC


Post-wave assembly defects found @ AXI, MVI, ICT(not shown: 671 squeeze balls)


MVI or ICT   AXI + ICT   AXI + MVI  AXI ONLY


Figure 4: Server board solder joint defects detected by XRL  AXI, MVI, and ICT at the post-wave step. Not shown are more  than 600 squeeze balls detected at XRL AXI.


The solder joint defects not detected at XRl AXI at the postwave step are shown in Figure 5.  A greater number of  defects  were missed at this step due to the difficulty in detecting  insufficient solder on through-hole components.  Detection  could be enhanced with greater experience in programming  the XRL AXI system.


0 1 2 3 4 5 6 7


TH insuff TH lead not thru


IC short TH short


TH missing


TH excess


IC insuff.


Post-wave defects not detected @ AXI


Figure 5: Details of the solder joint defects not detected by  XRL AXI at the post-wave step are shown.


Conventional X-ray transmission images are presently


difficult to interpret on PBAs with various socket features and  components placed on both sides of a PCB with resulting


images showing all features in field of view and with no depth  perception.  Rotating or 3D tilting did not readily reveal subtle  misalignments or changes in ball diameter or geometry that


XRL appears to provide the analyst in this regard.


Like 2-D transmissive X-ray equipment, the XRL AXI manual  inspection technique can be accomplished in just a few


minutes and, unlike the XRL AXI automated production


mode, requires no programming and little or no expertise or


training. Once a circuit board is loaded into the XRL tool, the  operator can adjust the z-height of the board with respect to


the X-ray beam and effectively move the horizontal plane of  vision or “slice”, so that the resulting live X-ray image shows  the suspect solder joint. The advantage of manual mode is that  the thin plane of focus can be moved in any x, y or z direction  through the solder joint to gain a more complete view of the


joint, producing virtually an unlimited number of slice views. BGA ball defects can most readily be detected by viewing two  horizontal slices, one slightly above the midpoint of the ball, and one near the pad on the PCB.  In automated production


mode, XRL AXI will usually be programmed to capture these  two slices. Figure 6 shows the two slices.


Slice 1


Slice 2


Component


PCB


Figure 6: The two XRL AXI slices typically viewed in both


automated mode and manual (failure analysis) mode are


shown. Normally formed ball (L) compared to abnormal ball (R). Note that the abnormal ball has lifted, and the horizontal  measurement along slice 1 is too large and the pad slice 2


measurement is too small.


XRL AXI detected physical anomalies on experimental central  processing unit (CPU) sockets with BGA solder balls


assembled (soldered) to a printed circuit board (PCB).  These  anomalies, however, were not considered electrical failures,


since current in-circuit test (ICT) did not discern an electrical  open or high resistance failure, but were considered solder


joint reliability risks. Thus XRL provided an opportunity to


perform preventative failure analysis, as seen in figures 7-11. Optical microscopy (OM), using a side view microscope (nonintrusive imaging) and a subsequent x-section, was performed  to verify and understand these physical discrepancies.


Figure 7: BGA array XRL images from a region near the PCB  pad (L) and from the same region but taken at a plane near  the center of the BGA solder ball (R) both of which show a  irregular shaped and shifted solder ball.


Figure 8: Side view optical image of the solder ball anomaly  described in previous XRL images (L) and subsequent xsectional view from a region taken near the center of the BGA  solder ball (R) showing a defective socket “paddle” which  resulted in a crushed solder ball. ICT electrical testing would  not have detected this solder joint reliability concern, since it  was sufficiently connected for electrical conduction.


Figure 9: XRL AXI image from a BGA array plane taken  through the center of the solder balls (L) and an OM side view  image of same solder ball at corner (R).   Note the smaller  diameter and elongated ball.


D1


Figure 10:  XRL AXI images from a plane near the center of  CPU socket solder ball array-slice 1 (L) and from a plane  near the PCB pad-slice 2 (R).  A comparatively largerdiameter (L) and smaller diameter (R) solder ball observed at  BGA pin D-1. The dashed arrows represent the plane for  physical x-section along row D.


XLR  Slice 1


XLR  Slice 2


Figure 11: The OM x-sectional view of the CPU socket on


PCB row D (upper and L) from Figure 9 and closer view of  D1 showing where XRL AXI planes 1 and 2 were taken of the  suspect solder ball on socket paddle  with a physical and


electrical open (R).


New generation XRL AXI systems provide excellent solder  quality benefits in production circuit board manufacturing  environments. The addition of an XRL AXI system to a circuit  board assembly line was shown to greatly increase detection  of solder joint defects and process problems previously  undetected at the traditional MVI and ICT test and inspection  steps. Using the XRL AXI system in off-line manual  inspection mode proved valuable as a non-destructive method  for off-line failure analysis of BGA defects. BGA solder ball  abnormalities found in the XLR images were confirmed to be  defective upon cross sectioning the indicted solder joint. The  ability to view virtual X-ray image slices real-time, in a  variety of z-axis heights along a solder joint, allowed the  failure analysis engineer to better determine the value of  subsequent cross sectioning of the joint.


1. David K. Lehmann, X-ray Systems for Optimizing  PCB Inspection, Circuits Assembly, p 35, February


2. Stig Oresjo, Defect Levels for Different Component  Types at the PCBA Manufacturing Process, SMTA  Conference 2000.


3. Frank Silva, 2-D or 3-D X-ray: Examining the  Factors Involved in Choosing an AXI System for the  Post Reflow Testing of Soldered Connections, Advance Packaging, p 29, August 2000.


4. Glen Leinbach, Finding BGA Opens in Production, Circuits Assembly, p 36, March 2000.


5. Colin Charette, The Economics of AOI and AXI for  EMS Providers, Circuits Assembly, p 44, November


2001.


6. David Mendez, Development of an Integrated  Overlapping ICT and X-ray Inspection Process, IPC  SMEMA Council, APEX 2001


7. Mike Teska, Fine Line PCB Assembly Leads to New  Test Issues, Electronic Packaging & Production, January 1998.


8. Steve Bonham, Wayne Singbell, No Single Test  Strategy,  Circuits Assembly, November 1997.


9. Arlene Hagio, X-ray Simplifies Test of Dense Boards, EETimes, September 1996


p 125-130


DOI: 10.1361/cp2003istfa125


## XRF Correlation of Board Reseats due to Intermittent Failures from the use of Thin Gold Plating finish on the Contact Fingers


XRF Correlation of Board Reseats due to Intermittent Failures from the use of  Thin Gold Plating finish on the Contact Fingers


Dan Stein, Victor Hernandez and Mary Ann Nailos


Dell Inc.  Austin, TX USA.


This paper correlates the reseat failure rates of a PCI option  card to the use of thin gold plating across the contact fingers.  This failure mechanism results in increased contact  resistance and is often misdiagnosed due to its intermittent  failure mode.


As many new manufactures appear in Asia, the push for  global competitiveness to achieve high volume and reduced  costs can result in insufficient plating finishes being applied  to the contact fingers.  Compounding this problem is the  fact the many companies use multiple raw board suppliers to  meet these volume requirements.    Many times the end user  of the option card is unaware of the wide variation in  contact plating thickness that may be present from one raw  board source to another.


Intermittent failures are one of the most common defects  experienced in high volume assembly.  Unless properly  diagnosed, these failures can be attributed to finger debris, rework flux, solder paste contamination and even connector  related issues.  The typical fix, whether approved by the  process or not, is for the manufacturing assembler to reseat  all of the option cards and memory into the Motherboard  connector sockets.  Unless the proper troubleshooting  approach is followed, isolating the true root cause of the  actual failure can be missed.


The difficulty in identifying the reseat problem is  compounded by the fact that the failures are often  intermittent in nature.  While reseating may temporarily  achieve sufficient mating between the board’s contact  fingers and the connector contacts, it provides no long term  fix.  These unnecessary reseats also reduce the long-term  durability of already thin plating affecting customer  satisfaction and warranty costs.


In the paper, we will expand on the theory behind the XRF  plating thickness testing, including:


• System theory


• Test calibration


• Part orientation


• Test measurement criteria


Additional analysis of metallurgical cross-sectioning was  performed to correlate the XRF test readings to the actual  plated layers.  The measurements were completed by use of  a SEM (Scanning Electron Microscopy).


Introduction:


This paper is based on an actual case history that occurred in  our production process.  A reseat failure rate of 5x the  normal rate was reported on an option sound card.  Numerous theories were proposed as to the root cause for  the spike in failures; contact finger contamination, software/driver issues, connector mating issues and board  thickness.  It wasn’t until XRF plating thickness testing was  performed on the contact fingers of the boards that the true  nature of the failure was understood.


XRF Theory


X-ray fluorescence spectroscopy is a useful analytical  technique because it is a non-destructive method of element  identification and thickness measurement.  The  instrumentation consists of a high voltage generator  providing power to an X-ray tube.   The X-rays generated in  the tube bombard the surface of a sample giving off  secondary X-ray radiation that are of characteristic  wavelength and energy of each element present in the  sample. The wavelengths or energies are then separated in a  spectrometer.  A detector measures the characteristic X-ray  and the output is either plotted as a spectra, identifying the  elements present (qualitative analysis) or are counted by a  scalar/timer for quantitative analysis (See Figure 1).  Energy  intensities of known standards are compared to unknowns  for quantitative analysis.


Figure 1: X-rays from the source (X-ray tube) bombard the  sample, producing secondary X-rays that are detected and  sorted by energy to produce a spectrum of the elements


present.


X-ray radiation is defined as electromagnetic radiation with  a wavelength of ≈10-5-100Å.  The characteristic X-ray  radiation of the elements present is produced when the  sample is bombarded with X-rays originating in the X-ray  tube.  The high energy x-ray radiation causes electrons to be  ejected from inner shells, causing outer shell electrons to  move into the vacancies.  X-ray energy is given off as an Xray photon in the transition from outer to inner shell (See  Figure 2).


Figure 2: X-ray radiation from a high energy source  bombards an atom, causing electrons to be ejected. X-ray  energy is given off when electrons from outer shells move to  inner shells to fill the vacancies.


The energy given off is related to the nuclear mass and the  difference in energies between the electron orbitals involved.


During measurement, the XRF spectrometer detects the  secondary (fluoresced) X-ray emissions released when the  sample is exposed to the X-ray source. These pulses are  sorted by energy into 1024 channels in the analyzer. The  characteristic X-ray energies for each element are found at  different channels or regions of interest (ROI). Several


spectral regions of interest may be present for one element  due a number of energy transitions between electron orbitals (See Figure 3 below).


Figure 2 X-ray spectrum of Au/Ni/Cu on circuit board. Note  the multiple regions of interest (ROI).


In quantitative analysis, the number of pulses at each  channel in the ROI for the elements being measured are  counted (cps) and compared to a set of calibration standards  of known thickness and the same composition. With the aid  of a computer, the thickness of the unknown sample can  easily be obtained.


Calibration:


Proper calibration of the instrument is critical to obtaining  accurate and repeatable results.  A combination of plated  and foil standards are used to establish a calibration program.  These standards are available in many thicknesses and  material combinations from the equipment supplier.  The  coating thickness of each standard is the thickness  equivalent of a coating weight per unit area.  The calculation  of the thickness equivalent is based on the theoretical  density of the coating material.  The weight per unit area of  each listed standard has been determined by comparing it  with master standards.  The master standards were prepared  using a balance and weights which are traceable to the  National Institute of Standards and Technology (NIST) in  Washington, DC.


These standards require careful handling and need to be  checked annually for re-certification.  Selection of the  proper plating ranges will improve the measurement  accuracy.  We use two different sets of gold/nickel/copper  plating standards.  Each set consists of 13 individual  standards of various thicknesses and metal combinations.  One set is for thin gold plating which covers a low range of


2.83 to 10.50 micro inches.   The other set covers a higher  range of 16 to 83 micro inches of gold plating.  Initial test  readings are made which then determine the appropriate  measurement program to use for that board.


We use a measurement time of 90 seconds on each standard  location to create the calibration program.  The two layer


Image contrast by electron selection


EFTEM selects electrons not only according to their scattering  angles, but also according to energy and energy bandwidth. The conditions for contrast generation are therefore much  better than in  conventional TEM (CTEM), particularly with  specimens consisting of light elements. The filtering out  according to energy and energy bandwidth does not have an  adverse effect on the resolution, contrary to smaller lens  aperture diaphragms. The filtering out according to energy and  energy bandwidth does not have an adverse effect on the  resolution, contrary to smaller lens aperture diaphragms.


Element information of scattered electrons


If specimen atoms are ionized during the inelastic scattering  process, energy losses which are characteristic for the element  will result. These appear as absorption edges in the energy loss  spectrum. Fine structures in the energy loss spectra convey  information on adjacent atoms and permit chemical bonds to  be analyzed. This makes energy loss analysis ideal for the


chemical characterization of minute specimen structures. The  X-radiation hν generated during the inelastic scattering  process is used for X-ray microanalysis (EDX) both in


EFTEM and CTEM. [3].


TEM


EFTEM


Fig 16: Imaging in the conventional TEM (CTEM) and in the  energy filtered TEM (EFTEM)


An EFTEM can be operated in different imaging modes:


Global imaging


The spectrometer breaks down the electrons according to their  energy (green with, red without energy loss), but the slit is not  in the beam path. The second projective system combines all  electrons into joint imaging. The results corresponds to the  quality of CTEM images, where the advantages of the filter  are not utilized.


Elastic imaging


The slit is in the beam path. High voltage is set to rated  voltage, e.g. 100 kV. The slit allows only electrons without  energy loss to pass. All electrons which have lost energy due  to inelastic scattering are filtered out. This mode enhances the  contrast for all imaging modes such as brightfield, darkfield  and diffraction.


Inelastic imaging


The slit is in the beam path. High voltage is increased by the  required energy ∆E. The slit position and the spectrometer  current remain constant. The slit allows only electrons to pass  that have lost the ∆E energy and are therefore back to the rated  voltage. This mode is used for imaging with selective contrast


on thin and thick specimens.


Fig. 17: Imaging modes in an EFTEM: Global imaging (left), elastic imaging (center) and inelastic imaging for elemental  distributions (right).


EFTEM Applications


This section shows the application of CrossBeam milling, TEM and EFTEM imaging on a  multi layer sample (layer  stack: Si substrate, SiO2 100nm, Ta 20nm, Cu 200nm and  TiAl 44nm).


To protect the sample surface the sample was coated with a  1µm layer of tungsten. By using the real time imaging the  sample was uniformly thinned to electron transparency (Fig. 18).


Fig. 18: TEM Lamella during ion milling. The image displays  a mixed signal between Inlens detector and ET detector. The  multilayer structure is clearly visible.


After performing a lift out the sample was transferred to a  carbon coated TEM grid and image in the TEM. The elastic  brightfield imaging gives a first impression about the layer  stack. However not all of the layers can be resolved clearly


(Fig. 19). By using low loss imaging the whole stack can be  displayed clearly. (Fig 20).


Fig. 19: Zero loss imagingof the sample. Only 3 layers of the  expected five layers are visible. The Ta layer is not visible.


Fig. 20: Inelastic imaging (Cu pre-edge) of the same sample. All layers are clearly visible.


By using the elemental specific imaging (ESI) the whole  chemical information about the layer stack can be displayed. (Figs. 21, 22)


Fig  21: Elemental specific imaging (ESI) Copper is displayed  in blue Oxygen in red.


Fig. 22: Elemental specific imaging (ESI) Copper is displayed  in blue Titanium in red


REFERENCES


1. E. Weimer, J. P. Martin: “Development of a new ultra high  performance scanning electron microscope”, 13th Int. Congr. on Electron Microscopy ICEM, Vol. 1, pp. 67-68 (1994).


2. G. Auvert, “FIB Dual-Beam Sample Preparation for TEM  Observation”, Microscopy and Microanalysis 2003, San  Antonio, TX, August 3 – 7, 2003.


3. R.F. Egerton, Electron Energy-Loss Spectroscopy in the  Electron Microscope, Plenum Press, New York, 1986.


Si Substrate


Cu


Ti Al


W (cap)


SiO2


Ta


p 140-143


DOI: 10.1361/cp2003istfa140


## A Method for Exact Determination of DRAM Deep Trench Surface Area


A Method for Exact Determination of DRAM Deep Trench Surface Area


Jeremy D. Russell


Infineon Technologies, Linkou,Taiwan


Yuan-Wei Tseng


ProMOS Technologies Inc. Hsinchu, Taiwan


A technique is described which allows the precise  measurement of the surface area of the dielectric layer of a  DRAM deep trench (DT) capacitor.  It uses precision FIB  sectioning, and allows determination with arbitrary accuracy.  It can be used for measuring random DTs in a region of  interest for process monitoring, and can also be used for a  single target trench in the case of failure analysis.


The capacitance of the deep trench (DT) of a DRAM cell is an  important parameter in determining the retention-time for a  cell.  It is most important to maximise this capacitance, but  within the constraints of not causing electrical failures, such as  trench to trench shorts.


Currently, this capacitance is characterised in two ways – electrically by directly measuring the capacitance on a teststructure, or indirectly it can be evaluated by making crosssections and extrapolating to get the expected capacitance  gain.  There are also some elegant ways of using processing  effects such as resist fill to estimate the volume and indirectly


measure the node area [1].  For electrical measurements, when the process is changed in order to optimise the  capacitance, it is normally necessary to wait one month.  Faster feedback can be obtained using special short-loop  processed wafers, but this is only possible on a limited amount  of product, and involves extra production complexity.


For constructional analysis, the feedback is very fast, but the  measurements obtained give only a limited correlation to the  actual final capacitance because only a few characteristic  features of the DT are measured, such as depth, critical  dimension, etc.  However, these do not take into account the  possible variation in the overall profile of the DT.  For  example, it is known that the DT is oval at the top, may be  rectangular partway down, before becoming round again at the  bottom.  There may also be unevenness in the DT sidewall  which changes the surface area, but which would not be


accounted for.  All this information is difficult to take into  account in simple construction analysis that just measures  cross-sections.


Use of these existing techniques has limitations for  development speed of process changes and fine-tuning.  It  also limits the feedback speed for process fluctuations, such as  DT etching performance which might affect DT capacitance, but which would only be caught at inline electrical test, much  later.


For finished products, failure analysis of retention fails may be  suspected to be due to too little DT capacitance if DTs are too  small, or misshapen.  However, it is almost impossible to  know what is the actual capacitance of a cell, or how much a  given DT deformation will contribute to lowering the  capacitance.


The technique described here [2] allows determination of the  DT dielectric surface area with great precision.


Theory


In principle the capacitance of a deep trench is given by:


ox


DT t A


εε


In practice, high dielectric constant materials are  incorporated (to enhance the trade-off between capacitance  and tunnelling currents, for example).  These are accounted  for by summing the capacitance contributions in series.  The  thickness of the dielectric layer normally does not change very  much, and can be determined by TEM in the actual deep  trench, and monitored in the production line by standard inline  metrology techniques, such as elipsometry.  Also, as the DT  poly doping and the outdiffused buried plate have similar  doping concentrations, the contribution from the depletion  layers is small.  However, due to the small thicknesses  involved, it is normally necessary to use some form of  correction factor to obtain capacitance values from the


measured node dielectric area.


Imaging and data collection


This technique depends on being able to make precise topdown sections of the DT very effectively in the focussed ion  beam, which are subsequently imaged in the scanning electron  microscope.  The images are then processed in order to  extract the DT structures, and measure the perimeter of the DT  at the depth of each slice.  The total surface area is calculated  by summing the areas of the DT surface between each slice (given by multiplying the inter-slice distance by the average  perimeter).  By using information from cross-sections to  measure the depth of the top of the dielectric below the  isolating collar and the depth of the DT, the calculation  precision can be improved.  For calculation of the DT  capacitance, the NO layer can also be measured by TEM.


The steps in the process are detailed as follows:


1. Prepare a suitable sample by cleaving so that the DTs  are near the top edge, and are inserted into the


focussed ion-beam tool such that the length of the DT  is horizontal in the FIB.


2. Prepare a sample in one of three ways, depending on  the application (Figure 1):


a. Make a precise, shallow angled slanted FIB  cut so that the depth of a particular location  along the cut can be calculated from the


distance along the cut via


θ


tan


x


(see Figure 1 for explanation of terms).  SEM images can then be taken by using the  precision of the stage to drive to specific  locations and acquire the images.  The


whole process can be easily automated.


b. For a more precise measurement, make a  step-series of cuts at increasing, precise  depths (then tilting to record the SEM image


each time).


c. For failure analysis of a single DT, the fail  address is identified, a cross-section is made  near to the location of the fail cell, and then  the sample tilted to make the FIB cuts.  These are done in a series, with an SEM  image taken at each step.


3. The FIB images are normally too flat, and the  dielectric layer too thin to resolve it.  Therefore it is  decorated in-situ using XeF2.  This enhances the  visibility of the NO, enabling clear imaging of the  DT section. The images are saved in a series with  standard names, and then imported into a PC with


suitable image processing capabilities.


4. In order to calculate the capacitance, it is also


Figure 1:  Geometry and means of making FIB cuts from the cross-section (right) to give the plane-view images (left).


( )( )θ


tan sin


==


Serial  Cut


Angle  Cut


Images were taken at  different depth.


θ  x


necessary to know the dielectric layer thicknesses, which can be done by TEM for the general case (Figure 2), then assume that the thicknesses do not  change much, or correlate to inline monitor wafer


measurements to ensure consistency.


Figure 2:  TEM image showing node dielectric thicknesses – in this case nitride and oxide layers.


Image processing


Image processing is performed as follows (Figure 3):


a. Background correction (to remove shading of the  image from the SEM imaging process and due to the  edges of the FIB cut.),


b. Segmentation, whereby the brighter NO outline is


separated from the darker background.


c. Noise reduction using a median filter to give a smooth, continuous binary shape for the DT outlines, but also  some shapes from the background decoration, noise, DT voids, etc.


d. Using methods of mathematical morphology [3], detect  each individual shape, and measure its perimeter, eliminating shapes that intersect the image margins.


From the shape size distribution, the correctly detected DT  outlines can be selected and differentiated from the artefactual  shapes due to decoration noise, etc., which have a much  different size distribution.


Calculations


From the last step of the image processing, a results table is  obtained, as shown in Table 1.  The detected objects consist  of valid DTs and artefacts, but it is easy to distinguish them  because the latter are much smaller, and do not fit to the  biggest size distribution.  For each image, its depth is either  known precisely in the case of a step cut, or if a slanted cut is  used, it is calculated from the slant angle and distance from  the surface via:


Figure 3:  Image processing sequence – from top to bottom:After background correction; segmentation; noise removal;shape identification and classification.


The upper region of the trench has a collar oxide to isolate the  capacitor from the devices in the silicon surface.  This depth  is determined from the plain view images of can also be  precisely measured from SEM cross-sections.  The area is  then calculated by summing the areas of the dielectric between  each section as follows:


bottom


P


∑


where P and d are the perimeters and depths of the slices, and  Abottom is a small correction factor for the bottom of the DT.


To calculate the capacitance, the usual equation [1] is used.  In the case of the node dielectric being made of multiple  layers, these layers are simply combined in series, e.g. –


total


However, in practice, there is not exact agreement – probably  due to the thin dielectric having different values of ε compared  to the bulk, and also differences in doping on either side of the  node.  To account for this at a particular technology node, a  correction factor is calculated by averaging over a number of  test wafers.


Table 1:  Table of results from a measurement after image  processing.  The coordinates are relative to the image  corner.


O bj#  C ente r-X  C ente r-Y P erim eter 1 0 .148737 0 .231699 0.966003 2 0 .367066 0 .227647 0.958738 3 0 .588402 0 .222298 0.939188 4 0 .797343 0 .226866 0.938005 5 1 .006056 0 .223592 0.919621 6 0 .556316 0 .109474 0.024452 7 0 .406667 0 .114667 0.002000


In Table 2, can be seen the results of several measurements.  As the correction factor is so close to 0.5, it was initially  believed it might be due to some calculation error, especially  as it is consistent between processes A and B which have  different node dielectrics.  However, a rigorous check, and  measurements on process C (170nm) show that this is not the  case. The processes A and B are at the 140nm technology  node (but two different lines), while process C is at the 170nm  node.  It can be seen that a very consistent correction factor


exists at a certain technology node, and also once it is  calculated, there is excellent consistency between the  calculated and electrically measured results.  In this case, the  results can be used to show that the capacitance on the kerf  test structure and the nearby product DTs have consistent  capacitance.  There is no other easy way to verify this the  validity of a test-key design.


Table 2:  Measured values of capacitance using electrical  measurements and the new technique for surface area.


A Centre, product


35.7


A Centre, kerf


34.46 5.51


35.2


A Edge, product


4.22


26.9


A Edge, kerf 27.97 4.29


0.492


27.4


B Centre, product


5.15


33.9


B Centre, kerf


34.40 5.28


34.8


B Edge, product


5.24


34.5


B Edge, kerf 34.24 5.17


0.502


34.0


C Centre, kerf


39.94 6.21 0.574  -


A technique has been reported which allows the accurate  measurement of deep trench surface area.  This allows  fast and accurate feedback for process monitoring,


development and failure analysis without waiting for


electrical testing results.


JDR would like to thank J.F. Walsh for the many  discussions that we enjoyed, better luck to Liverpool  next season.


1. Zi-Jing Tsai, Hui-Ming Mao, Ying-Huan Chuang, YouBi Lee, Taiwan Patent TW507311.


2. J.D. Russell and Y-W. Tseng, Taiwan Patent applied for.


3. R.C. Gonzalez and P. Winz Digital Image Processing  Adison Wesley, Reading, Mattachusetts, (1977).


p 144-152


DOI: 10.1361/cp2003istfa144


A Review of TEM Observations of Failures of the Memory Cell in a


## A Review of TEM Observations of Failures of the Memory Cell in a Deep Trench Capacitor DRAM


Deep Trench Capacitor DRAM


Jen-Lang Lue, Jack Lee, Esther Chen and Jian-Shing Luo


ProMOS Technologies Inc., Hsinchu, Taiwan


Application of the high resolution of Transmission  Electron Microscopy (HRTEM) plays a very  important role in structural analysis and materials  characterization for process evaluation and failure  analysis in the Integrated Circuit (IC) industry. We  summarize TEM observation experience of the  common memory failures of a BEST deep trench cell  with an N-MOS gate used in CMOS DRAM  technology. Memory cell failures are categorized into  three areas for discussion – the deep trench (DT) capacitor, the transfer gate (GC), and the borderless  bit-line contact (CB) between a transistor and a bit  line.  Typical examples that occurred in these three  areas are presented and provide a basic  understanding of normal DRAM cell failures.


The one-transistor, one-capacitor (1-T) cell has been  universally used since the middle 1970s because it  has the highest circuit density.  The density of  DRAMs has quadrupled every three years since then  through the advances in process and circuit design  technology [1-2]. Now 256Mbits are in mainstream  production and production will soon enter the era of  512Mbits.  In the IC industry, TEM application plays  a very important role in structure analysis and  materials characterization for process evaluation and  failure analysis because of its extremely high  resolution and ability to provide better material  contrast.  Features such as thickness of thin films (NO dielectrics, gate oxide, barrier liner, etc.), interface inspection, dislocation, micro defect, etc. all require TEM analysis.  Any abnormality in the  structure/feature might cause the failures in the IC  operation.


In this paper, we will review normal failures in the  memory cell of a BEST (BuriEd STrap) deep trench  cell with N-MOS gate in CMOS DRAM technology [3-4].  These failures are typically detected in  electrical tests and subsequent TEM observation is  used to determine the physical cause of the failures. Failures in the memory cell occur in three areas - the


deep trench (DT) capacitor, the transfer gate (GC), and the borderless contact (CB) between the  transistor and the bit line.  Five failure modes in the  deep trench capacitor area are examined, namely the  thinner film of NO capacitor dielectrics, the ASG (arsenic-silicate glass) residuals remaining in the  sidewall of NO dielectric region, the abnormal  interface of poly 1-Si and poly 2-Si in the trench, the  presence of dislocations in the p-n junction, and the  striation in the profile of DT.  Three failure modes in  the transfer gate are examined, namely the abnormal  growth of the gate oxide, poly-Si footing, and WSix  extrusion.  In the contact area, the electrical short  between CB and GC, the open circuits between CB  and substrate, and other defects in the CB are  examined.  In total ten failure modes in the memory  of a BEST deep trench cell will be discussed.


DRAM Basics


In general, a basic DRAM cell consists of a  MOSFET that operates as a switch, and a capacitor  that stores charges and maintain memory.  The cell is  able to hold binary information in the form of stored  charges on the capacitor – logical one and logical  zero.  The basic DRAM circuit as shown in figure 1  allows the write and read operations in the DRAM  cell [1-2].  Application of a sufficiently high voltage  to the word line to turn on the switch, and then  application of a voltage corresponding to the write  data from the bit line to the capacitor performs the  write operation.  Applying a sufficiently high voltage  to the word line to turn on the switch performs the  read operation.  A signal voltage (±∆V) is developed  on the bit line, depending on the stored data at the  capacitor, is distinguished by a sense amplifier on the  bit line.  The refresh operation is a must for DRAM  to return the stored charges and maintain its data  because various leakage paths cause the stored  capacitor charges to deplete.  The cell is read before  the stored voltage has become excessively decayed, and then it is rewritten by utilizing the resultant read  information so that the voltage is restored to its  initial value.  A succession of read-rewrite operation  at a given time interval retains the data.


Figure 2 presents the schematic cross-section of a  deep trench capacitor DRAM cell in use for a BEST  cell with an N-MOS gate in CMOS DRAM  technology manufactured in our factory [3-4].  Deep  trench capacitors are formed in the substrate Si after  etching deep holes, about 8 µm, into the wafers.  The  capacitor consists of the polysilicon storage node (poly 1), which fills the trench, the NO (nitride-oxide) dielectric layer on the trench wall, and a N-buried  plate, which acts as a storage plate.  The N - buried  plate is formed using ASG (arsenic-silicate glass) out-diffusion from trench walls into substrate Si  before NO dielectrics are applied.  The first N+ polysilicon (poly 1) is deposited after NO dielectric  formation and is then recessed to a point below the  P-well.  The SiO2 trench collar is formed after the  recessed first polysilicon fill (poly 1) to a point  below P-well for isolating the node trench polysilicon (poly 2) from the p-well substrate.  The second  polysilicon fill is then deposited and recessed to a  certain level.  Then a further collar-etch process is  used to gain a larger window for buried strap  polysilicon (BS poly-Si) to maintain low resistance in  the connection between the poly2 and the storage  node diffusion.  The N+ out-diffusion from the BS  polysilicon merges with the node source-drain to  complete the contact.  Afterwards the shallow trench  isolation (STI) is formed to isolate the BS poly-Si in  the deep trench from the passive word line (WL).  The well implant is conducted before gate conductor (GC) formation. The N-MOS transfer gate, called the  GC stack, is a stacked structure of Si/SiO2/PolySi/WSix/SiN. The sidewall oxide (SWOX) and spacer  nitride on sidewalls of transistors are formed after  the GC is made.  A borderless bit-line contact (CB) is  designed for connecting with the source/drain and a  bit line.  Before CB is formed, a junction implant is  applied for source/drain formation.  CB is made of  polysilicon or tungsten (W), depending on the  technology node.  For 0.14 µm or below, tungsten is  incorporated.  If it is made of W, a barrier/glue layer  of Ti/TiN liner is formed before the W deposition.  Basically all mentioned above are to form the basic  structure of a deep trench capacitor DRAM cell. However, any abnormality in the structure/feature, especially in the paths among bit-line contact, transistor, and capacitor might cause the electrical  failure in the DRAM cell operation


Figure 1: A basic DRAM circuit – one MOS


transistor and one capacitor.


Figure 2: A schematic diagram shows the crosssection of a deep trench capacitor DRAM cell.


Results and discussion


The Deep Trench Capacitor


Five examples are presented in the deep trench  capacitor area, including the thinner film of NO  capacitor dielectrics, the ASG residuals in the  sidewall of NO dielectric region, the abnormal  interface of poly 1-Si and poly 2-Si in the trench, the  presence of dislocation in the p-n junction, and the  striation in the profile of DT.  The five physical  failures examined in this paper generally cause the


Bit line


Word line


Storage node


Capacitor  Cell plate


MOSFET


high current leakage that results in the functional  fails or retention problems.


1. When a capacitor is formed, the capacitance can


be expressed as [5]:


C= Kε0A/d


(1.1)


Where K is the dielectric constant of the dielectric  material, ε0 is the absolute permittivity of a vacuum, A is the area of conducting plate, and d is thickness  of dielectric.  The NO dielectric is optimized to  achieve the maximum capacitance with minimum  leakage.  It must also endure the maximum operating  voltage without breakdown, and therefore the Nburied plate is normally biased at 1/2 bit-line voltage  to reduce the maximum field in the dielectric. The  thinner NO dielectric, the higher trench capacitance  and the greater capability to sustain longer retention  time, but there is a limit.  If this film is too thin, it  will not work reliably even at a low voltage and a  high leakage current occurs causing dielectric  breakdown.  Figure 3a shows a very thin NO film in  the capacitor compared with the normal thickness  illustrated in figure 3b.  Normally this film should be  around 40Å,but in  this case the film is only about  10Å.  Along with the detection of the thin film, one  can see that epi-Si growth into poly1 has not been  stopped by the NO dielectric – a clear indication that  NO dielectric is too thin.


Figure 3: (a) A very thin NO dielectric layer in the  trench capacitor was seen to cause dielectric  breakdown  (b) A normal thickness and profile of  NO dielectric in the trench capacitor.


2. The ASG residuals in the trench are very common  failures, especially in the beginning development of a  new process technology. This ASG oxide residue will  lower the dielectric constant of the NO dielectric  while effectively increasing the dielectric thickness.  From equation 1.1, the lower capacitance in the  capacitor is produced so that the electrical failure  with a retention problem is measured.  Figure 4  shows the typical TEM images of cross-sectional  view and planar view with the ASG residuals  remaining in the trench sidewalls.  It is clear to see  that in the NO dielectric region there is an ASG  residue between substrate Si and NO dielectric layer  as compared with the normal profile shown  previously in figure 3b.  As mentioned above, the Nburied plate is formed using ASG out-diffusion from  trench walls into the substrate Si before the NO  dielectric is formed.  After the N-buried plate is  formed, an etching process of “ASG strip” must be  conducted to ensure there is no ASG remaining on  the trench sidewalls.  Note that most ASG residuals  are in the corners of the trench as shown in planar  view in figure 4b, because the corners are the likely  dead zones for the etching process.  Actually  optimizing the etching recipe to avoid producing the  dead zones can solve this problem.


Poly1-Si  Epi-Si


NO dielectric


Epi-Si


Figure 4: (a) A cross-section image showing ASG  residuals in the sidewalls of NO dielectric region.


(b) A planar image showing ASG residuals in the  sidewalls of NO dielectric region.


3. An abnormal interface layer between Poly 1- Si  and Poly 2 – Si is a very common failure in the  trench node as shown in figure 5a.  This abnormal  interface layer was identified as an oxide that  remained after the trench collar oxide strip process  was completed and before the poly 2 fill was initiated.  As compared with the normal one in figure 5b, the  high resistance between P1 and P2 caused difficulty  during the read and write operation of the charges, and produced one of the electrical SCF (single cell  failure) fail modes during testing.


Figure 5: (a) In the deep trench capacitor area, an  abnormal interface layer between Poly 1- Si and Poly  2 – Si. (b) A normal profile between Poly 1- Si and  Poly 2 – Si.


4. The striation in the profile of DT is also a very  common failure in the trench node.  Deep trench  capacitors are formed in the substrate Si after etching  deep holes, about 8 µm, into the wafers.  The  sidewalls in the deep holes are supposed to be round  and smooth after etching.  In some cases etching  abnormalities occur creating uneven surfaces called “striation” in the sidewalls.  These striations hinder  the deposition of the NO dielectrics and the collar  oxides creating variations in the wall thickness and  sharp corners in the layers related to failures.   A  thinner film in the corner within the trench collar  creates a higher electric field than that of a thicker


Poly -Si


ASG   residue


Trench


collar oxide


Seam


Poly1-Si


Poly2-Si


NO


dielectric  Trench


collar


Interface  layer


and round one of a normal profile illustrated in figure  6b.  So a higher leakage current occurs from poly 2  to the substrate Si and causes electrical failure.  This  process abnormality often leads to single cell failures (SCF), which are one of the major yield detractors  during testing.  Figure 7 is another example of a  cross-section TEM image showing the striation of  deep trench profile at trench NO dielectric region.


Figure 6: (a) A planar view of TEM image showing  the striation at trench collar (b) a normal profile at  trench collar.


Figure 7: A cross-section of TEM image showing the  striation at NO dielectric region.


5. It’s well known that stress combined with  nucleation sites in the silicon can create dislocation [3,6].  The presence of dislocation defects in the p-n  junction will cause high current leakage.


Figure 8 shows dislocation in the intersection of  outer collar tip, BS poly-Si, and substrate Si as  indicated by the arrow.  This causes the junction  leakage of S/D to the substrate and a retention time  loss problem in the cell.  Before BS poly-Si  deposition, a 7Å thick nitride layer is deposited in  order to inhibit the interaction between substrate Si  and BS poly-Si.  The thickness of the thin nitride  layer is optimized to minimize the increase of  electrical resistance at the interface while ensuring it  is thick enough to stop the physical interaction  between substrate Si and BS poly-Si.  The  temperature of the BS poly-Si deposition is an  important parameter regarding the stress on the  substrate.  If this temperature is not optimized, unexpected stress will remain in the interface of  substrate and BS poly – Si.  In addition, the triple  intersection of trench collar, BS poly and substrate Si  is usually a site of stress concentration that creates  dislocation.  Optimizing the temperature for nitride  deposition and BS poly-Si deposition can solve this  problem.


Trench  collar


Striation


Poly 1-Si


The Transfer Gate - GC


In the transfer gate, the examples of abnormal  growth of gate oxide, poly-Si footing, and WSix  extrusion are discussed.  These features may cause  SCF failure


1. In a NMOS gate, thickness of gate oxide is a very  important parameter for device performance.  Figure  9 shows a TEM image of a borderless bit-line contact  CB between two NMOS transistors at the active area.  This GC on the right side has an abnormal and  thicker gate oxide than the normal one on the left  side.  This causes the Vt (threshold voltage) to  increase in the failed GC, and it causes the failure in  the cell operation.  The abnormal gate oxide  thickness of the failed GC causes an electrical failure, SCF1, when tested.


It is well known [5] that gate oxide (SiO2) is formed  by a thermal oxidation process on the silicon surface, so if the thick oxide layer of the failed GC was  formed during the gate oxide formation process, the  consumption of the substrate Si should be more than  that of normal one.  Therefore, the height of the  interface between gate oxide and substrate Si of the  failed GC should be lower than that of normal one.  However, no obvious difference between right and  left-side transistors on Si consumption is shown in  the image.  In addition, the thickness of polysilicon  and WSix of the failed transistor, and the height of  WSix differ from the normal transistor.  This  indicates that the abnormal gate oxide could be from  the oxidation of poly-Si during following thermal  process (e.g., the thermal process forms sidewall  oxide of GC) due to cracks between poly-Si and  thermal gate oxide.


Figure 8: The presence of dislocation in the p-n  junction.


Figure 9: A TEM image showing a thick gate oxide


at failed GC.


2. A failure mode with the signature of “GC-CB  short” occurs very often in DRAM products.  The  failure modes observed for this fail type are SCF0, and flip bit fail with bit-line fail signature.  The  shorted cell is always at logical 1 and can’t be  changed to logical 0 because it is always pulling the  same as WL voltage and reading 1, and it always  fails at zero.  Two common types of GC-CB shorts, poly Si footing and WSix extrusion are presented  here from the TEM point of view.


Figure 10 is a typical example of GC-CB short, showing poly-Si footing contacting the CB tungsten  at its bottom.  This type of failure can be easily  observed from a SEM (scanning electron microscope) image as seen in figure 11.  Initially follow-up TEM  analysis was requested to clarify the root cause of the  problem, but now process/integration engineers have  a clearer understanding of SEM images and can use  SEM images to interpret such failures.  In general  micro masking during mask open of GC WL main  etch and various cleaning stages causes the GC-poly  Si footing to form [7].  Insufficient GC WL etch time  by integrated variation of the GC stack also causes  the GC-poly Si footing to form [7].


Figure 12 shows another typical example of GC-CB  short.  The WSix extrusion has caused it to short to  CB tungsten.  In this case, WSix extrusion is not the  only cause of the short, but it really enhances the risk


BS Poly-Si


Trench   collar


Dislocation


for shorts due to the normal irregularities of the CB  related processing. The WSix extrusion is strongly  related to the Si/W ratio and the thermal process for  SWOX formation.


Figure 10: A TEM image showing GC-poly-Si


footing at bottom to short CB


Figure 11: A typical SEM image showing GC-poly-Si  footing at bottom to short to CB


Figure 12: A TEM image showing WSix extrusion to  short with CB


The Borderless Bit-Line Contact - CB


Along with CB to GC shorts previously discussed, open circuits between CB and substrate, and defects  in the CB are also common types of failure modes.  Most of the failure modes with the signature “CB  open” will cause twin-bit failure in the electrical test.


The failure of twin bits with a “CB open” signature is  also a common failure mode in DRAM products. The  root cause for this failure is due to the high resistance  at the contact area of CB to substrate Si.  When this  occurs, the two cells can’t be written and read, i.e., data from the bit-line is not able to flow into the  capacitor while GC is turned on and no ∆V signal  voltage or smaller signal voltage is available for the  sense amplifier to detect for the normal read  operation.  Figure 13 shows the inadequate etching  during the CB etching process that has caused the  CB to be open to substrate Si.  It’s obvious that a  residue of the SiON barrier remains at the bottom of  the CB.  For this case the CB etching process  window is not enough to cover integration variation  in the previous layers.


Figure 14 is another typical example of a contact  area problem.  Before W is deposited into the CB, a  thin layer of TiSix/TiN liner is deposited into the CB  as a barrier/adhesion layer for further W deposition.  As seen in figure 14, the quality of TiSix/TiN liner at  the failed address is different as compared with the  normal one in figure 15.  Voids appear to have been


CB


SiN


WSix


Poly-Si


found at the contact interface.  A further  compositional analysis by EDS (energy dispersive  spectrometer) found fluorine in the contact area, which indicates the voids were probably produced  due to the reaction of fluorine with the TiSix/TiN  liner.  The fluorine may come from the gas of WF6  during W deposition process.  This problem can be  solved by the optimization of the gas flow of WF6  during the W deposition process.


As devices continue to shrink, the process window  for CB etching becomes ever smaller.  Trying to  prevent the CB-GC short by altering the process  might increase the risk for CB open failure.  How to  optimize or maintain quality control through the  ever-changing CB process is always an interesting  challenge for process and integration engineers.


Figure 13: A TEM image showing the residue of the  SiON barrier at the bottom of the CB.


Figure 14: A TEM image showing an abnormal


TiSix/TiN liner at the failed address.


Figure 15: A TEM image showing a normal profile of  TiSix/TiN liner at bottom of the CB.


TiSix


TiSi


TiN


The above reviews important TEM observational  experiences with common failures in the memory of  a BEST cell with an N-MOS gate in CMOS DRAM  technology.  Although this is not a comprehensive  look at all modes of failure within a DRAM cell, it  does account for the most common failure modes.  Moreover it clearly demonstrates the benefit of TEM  observation to identify and correct the problems that  occur during fabrication of DRAM cells.


The authors would like to present our thanks to the  colleagues at Department of Physical Failure  Analysis in ProMOS for their insightful discussion  and support.


Reference


1. K. Itoh, VLSI Memory Chip Design, Springer.


2. Betty Prince, Semiconductor Memories, Second


Edition, John Wiley and Sons (1997)


3. E. Adler, J. K. DeBrosse, S. F. Geissier, S. J.


Holmes, M. D. Jaffe, J. B. Johnson, C. W.


Koburger III, J. B. Lasky, B. Uoyd, G. L. Miles, J.


S. Nakos, W. P. Noble, Jr., S. H. Voldman, M.


Armacost, and R. Ferguson, IBM J. Res. Develop.


Vol. 39, No.1/2, January/March (1995) p167-187.


4. Nesbit L., Alsmeier J., Chen B., DeBrosse J.,


Fahey P., Gall M., Gambino J., Gernhardt S.,


IshiuchiH., Kelinhenz R., Mandelman J., Mii T.,


MorikadoM., Nitayama A., Parke S., Wong H. and


Bronner G., International Electron Devices


Meeting IEDM (1993) p627-30.


5. Hong Xiao, Introduction to Semiconductor


manufacturing Technology, Prentice Hall.


6. J. P. Hirth and J. Lothe, Theory of Dislocations,


2nd edition.


7. J. D. Russell, Y. J. Chew, H. M. Chen, C.


Giethermann, and Z. H. Zhuo, Proc. 27th ISTFA


(2001) p131.


p 153-157


DOI: 10.1361/cp2003istfa153


## The Effect of TEM Specimen Preparation Method on Ultra-thin Gate Dielectric Analysis


The Effect of TEM Specimen Preparation Method on Ultra-thin Gate  Dielectric Analysis


A. Y. Du1, C. H. Tung1, B. H. Freitag2,   W. Y. Zhang3 S. Lim3 E. H. Ang4 and Danny Ng4


1 Institute of  Microelectronics, 11 Sceience Park road, Singapore Science Park II, Singapore 117684.  2 FEI/Philips Electron Optics Applications Laboratory, Building AAE, 5600 KA Eindhoven,  Netherlands.


3 Systems on Silicon Manufacturing Co. Pte. Ltd., 70 Pasir Ris Drive 1, Singapore  519527.


4 TECH Semiconductor Singapore  Pte Ltd., 1 Woodland Industrial Park D, Singapore 73879.


The three typical TEM specimen preparation methods are  investigated for two different ultra-thin gate dielectric  materials analysis. The results show that the mechanical  polishing with short time, low angle ion milling is best  specimen preparation method for both samples. FIB finial  thinning can be used for SiON gate dielectric specimen  analysis, but is not suitable for HfO2 gate dielectric analysis. After FIB thinning, severe Ga and Pt contamination on the  specimen surface is found when using HR-STEM/HAADF  imaging.


The semiconductor process technology has scaled down to  130 nm technology and below, with the gate oxide thickness  has also been reduced to below 2nm.  The 1.5nm gate oxide is  used in 130 nm technology devices. [1] Due the high leakage  current and reliability issue for ultra-thin nitrided silicon  dioxide gate dielectric, the high-k materials such as hafnium  dioxide and HfAlOx have been proposed as possible near-term  replacement for silicon dioxide as gate dielectric material. [2,3]  For ultra-thin gate oxide layer, TEM is  one of the most  promising techniques  to study and characterize the related  process and yield issues. [4] However, there is little report on  the effect of TEM specimen preparation method on the gate  oxide analysis.  In this work, we study the effect of three  different TEM specimen preparation methods on two different  gate dielectric materials.


Two ultra-thin gate dielectric samples are used in this work.  The structure of sample #1 is Si substrate + 10Å oxynitride +2KÅ undoped poly Si. The structure of sample #2 is Si  substrate + bare oxide +30Å HfO2 (without anneal) + 2 KÅ  undoped poly-Si.


Three typical TEM specimen preparation methods  are used to prepare the TEM specimens for this work. They  are:


A. mechanical polishing  + ion milling ( less than 5 min., at   low angle < 4o).


B. Mechanical pre-thinning + FIB final thinning.


C. FIB thinning + lift-out and carbon film support.


All specimens used are from the same wafer at the wafer  center and near each other.  The high resolution TEM (HRTEM) was performed with Philips CM 200 FEG TEM.  And high resolution STEM (HR-STEM) analysis was  performed with Tecnai G2 ST with field emission gun (FEG).


Results and discuss:


HRTEM images quality is mainly controlled by the TEM  sample preparing method. In this work, the HRTEM images of  Si substrate and ultra thin gate oxide layer is used to evaluated  the final TEM sample quality.


Fig 1 shows TEM images of the sample #1 for three different  methods. The images are taken from the same sample  thickness range (measured by EELS) from the three different  samples.  It is obvious that the FIB thinning has induced  severe HRTEM image lattice fringe quality degradation.  Fast  Fourier Transform (FFT) of the Si substrate is used to evaluate  the HRTEM image quality.  It is obvious that the FIB thinning  has induced high noise background, as demonstrated in Fig 1.


It is known that there is a very thin amorphous layer, less than  20Å, on the top surface of specimen with low angle ion  milling. But in FIB prepared specimens, about 200~300Å  amorphization layer on the surface of specimen is inevitable  using 30KV Ga source FIB milling4. The amorphous layer and  rough interface on both side of the specimen both degrade  HRTEM and HR-STEM   image quality. Fig 2 shows HRTEM  results of samples #2 prepared by the three different sample  preparation techniques. FFT’s and their intensity cross  sections are also shown to demonstrate the signal to noise ratio  in each case.


The lift-out method specimen introduces more background  noise in HRTEM images due to extra amorphous carbon  supporting film. This has been observed in FFT of Si substrate  as shown in Fig 1 and Fig 2. In sample #2, except for the  similar effect observed previously on FIB thinning induced the


HRTEM image quality degradation, it is also found that the  FIB thinning has induced another effect on high-K materials  interface.


In the HRTEM image of specimen prepared with mechanical  polishing + ion milling, a white interface layer at interface of  Si substrate/ HfO2 can be observed clearly.  However, this  layer was not observed in FIB thinning specimens, comparing  Fig 2(a) and 2(b,). HR-STEM/PEELS analysis showed the  white layer to be native oxide layer, can be either SiOx or  HfSiOx. The reason for the disappearance of the white layer in  FIB prepared samples remained to be studied.


HR-STEM analysis was performed on sample #1 and 2 for  both mechanical polishing + ion milling and pre-thing FIB  milling specimens.   The results show that the FIB thinning  can introduce severe degradation of the HR-STEM images. The atomic columns are barely visible in most of the cases. Fig 3 show the HR-STEM/HAADF images of sample#1 with  specimen prepared with method A and B. FIB also introduced  severe contamination issue. Local contaminant patches of Pt  and Ga are observed in STEM HAADF images for both  samples # 1 and #2, as seen in Fig 4. These Ga and Pt  contamination cannot be removed with normal TEM plasma  cleaning process.


Fig 1.  HRTEM images of sample #1 with three different  specimen preparation methods. Si substarte area used for  FFT is shown with red box. The corresponding FFTs  are  shown at top corner of the HRTEM images. (a) method A,


(b) method B and (c) method C.


Fig 2. HRTEM images of sample #2 with three different specimen preparation methods. The areas of Si substrate for FFT are marked  with red box. The FFT of Si substrate is shown at top corner of HRTEM image.  . and the corresponding histogram profiles of FFT


patterns are also shown on the left side to indicate the signal to noise ratio of HRTEM image.  (a) HRTEM image with method A, and (a1) is the histogram profile of  FFT across the blue line as seen in FFT. (b) and (b1) are method B. (c) and (c1) are  method C.


Fig 3.  HR-STEM/HAADF image degradation due to FIB  thinning. (a) HR-STEM image of specimen with method A, (b) for method B.


Fig. 4: FIB induced local patches of Pt and Ga  contaminations, which is readily observed in STEM HAADF  images.


HR-STEM technique is sample surface sensitive. The carbon  contamination is one of the root causes for images degradation  for specimen kept long enough in TEM.  Plasma cleaning is


essential for all HR-STEM studies. Fig 5 clearly shows the


effect of plasma cleaning on STEM imaging.  On the other


hand, plasma cleaning is not necessary for conventional


HRTEM imaging.


Fig. 5:  The plasma clean can improve HR-STEM images  quality. (a) after 2 min. plasma cleaning, and (b) the same  sample prior plasma cleaning.


Different TEM specimen preparation methods affect the TEM  analysis results for ultra-thin gate dielectric layers.  The  mechanical polishing with ion milling is the best method for  all HRTEM and HR-STEM analyses.


The FIB pre-thinning and lift-out method can be used for  preparing TEM specimens for ultra-thin gate oxide layer  thickness measurement, provided the artifacts are properly  controlled.  Both pre-thin FIB and FIB lift-out are not suitable  for HfO2/Si interface studies as the interface native oxide (SiOx) can totally disappear due to sample preparation  artifacts. The root cause of this effect remained to be studied.


Severe Pt and Ga contamination in FIB thinning specimen is  observed.  FIB thinning also introduced severe HR-STEM  image degradation due to amorphization effect.


Acknowledgement


This work has been supported under the Singapore Wafer  Technology Consortium (WTC) project #2. The project  members include Systems on Silicon Manufacturing Co. Pte. Ltd (SSMC), TECH Semi-conductor Pte Ltd, and Institute of  Microelectronics (IME) Singapore.


1. S. Thompson, M. Alavi, M. Hussein, P. Jacob, C.


Moon, M. Prince, S. Sivakumar, S. Tyagi, and M.


Bohr. “130 nm Logic Technology Featuring 60 nm


Transistors, Low-K dielectrics and Cu interconnects,” J. Intel Technolgy, 6, 5 (2002).


2. G. D. Wilk, R. M. Wallace and J. M. Anthony. J.


Appl . Phys. 87, 484 (2000).


3. L. Kang , B. H. Lee, W. J. Qi , Y. Jeon, R. Nieh, S.


Gopalan, K. Onishi and J. C. Lee, IEEE Electron


Device Lett. 21, 181(2000).


4. A.J. Mardinly, Institute of Physics Conference Series  No. 164, Proceedings of the Microscopy on


Semiconductors Materials Conference Oxford, 575-584, 1999.


p 158-165


DOI: 10.1361/cp2003istfa158


## Forward Scattered Scanning Electron Microscopy for Semiconductor Metrology and Failure Analysis


Forward Scattered Scanning Electron Microscopy for


Semiconductor Metrology and Failure Analysis


William E. Vanderlinde


Laboratory for Physical Sciences  College Park, Maryland, USA


Continuing decreases in electron device feature size have  strained the resolution limits of scanning electron microscopy (SEM). In this paper a simple method is demonstrated for  producing significantly improved resolution in SEM imaging  without making any special sample preparation or  modifications to the SEM. This method images with the lowloss forward scattered electron signal by using a modified  sample holder. The method was found to be particularly useful  for observing low atomic number materials such as photoresist  and molecular semiconductors in their natural state, i.e. without sputter coating.


Semiconductor manufacturers are now shipping product with  sub-100 nm features. Measuring features and defects in this  size range has become a challenge for the scanning electron  microscope. Some manufacturers have begun routinely using  TEM (transmission electron microscopy) for metrology below  200 nm. 1 This is quite disappointing since the SEM should, in  principle, be capable of providing more than enough  resolution for these features.


Modern field emission SEMs have a nominal spot size as  small as 1 nm. However, it is very rare that 1 nm resolution is  realized in everyday imaging. Typically a SEM service  engineer will demonstrate the microscope resolution by using  very high beam voltage such as 30 kV to image a special “resolution standard” which consists of gold islands on a  carbon substrate, commonly referred to as a “gold-on-carbon” sample, see Fig. 1 which is at 500,000X (!) magnification.  Imaging a more typical sample such as an electronic device  will generally produce an image with much lower resolution  that may not meet the needs for modern failure analysis and  metrology.


It is sometimes possible to achieve very high resolution by  sputter coating a very thin layer of metals such as Au, Au/Pd, Cr, or Pt. Typically such coatings provide a better image, not  only because they eliminate charging but because they also  increase the surface emissivity of the sample and reduce the  secondary electron range, resulting in a better image of the  sample surface. About 10 nm of metal is required to produce a  continuous sputtered film, but this amount of metal may  obscure surface detail and cause image artifacts from the grain  structure of the sputtered metal, and is therefore unacceptable  for imaging at 1 nm resolution, see Fig. 2.


100 nm


Mag = 500,000X


Figure 1: Secondary electron image of gold islands on a  carbon substrate shows that very high resolution SEM images  are possible under the right conditions.


Mag = 100,000X


Figure 2: Secondary electron image of aluminum metal sputter  coated with 10 nm of Au/Pt. The image has high resolution  but the original surface detail is obscured and the sputter  coating grains introduce artifacts seen as jagged dark lines.


In order to achieve ultra-high resolution in the SEM, three  conditions must be satisfied: 2


1. The electron beam must be finely focused to a small spot at  the surface of the sample.


2. The electron beam current must be high enough to produce  sufficient signal so that visible contrast is achieved in the  image.


3. The signal used for imaging must originate very close to the  impact area of the beam on the sample.


Conditions 1 and 2 are satisfied when the electron source is  operating at high brightness, which is maximized when the  electron source is at high beam voltage. However, high energy  electrons have a large range in most materials and when they  are backscattered from deep in the sample towards the surface  they may exit the sample at a significant distance from the  probe location, see Table 1. Thus condition 3 is not satisfied at  high voltage since the backscattered electrons are not closely  correlated with the probe, and they also produce secondary  electrons as they exit thus reducing the spatial correlation  between the secondary electrons and the probe. If the beam  voltage is reduced so as to decrease the range of the electrons, then the brightness of the electron source is reduced and it is  not possible to achieve a small spot with sufficient beam  current (conditions 1 and 2). For the special gold-on-carbon  sample all three conditions are satisfied at high beam voltage  because gold has a very high backscatter coefficient and  carbon has a very low backscatter coefficient, thus incident  electrons are usually either reflected from the gold surface or  lost in the carbon substrate. However, it is very difficult to  find ordinary samples that will meet the three conditions.


Beam energy


(keV)


Spot size (nm) Electron penetration  range in aluminum (microns)


2.4


0.028


3.5


0.22


1.3


0.41


1.1


1.32


4.19


8.24


Table 1: Electron beam spot size (per the manufacturer 3) and  penetration range (from the Kanaya-Okayama formula 4) as a  function of electron beam energy.


One solution to these problems is to create a very thin sample  and image using the transmitted high energy electrons. In  recent papers 5,6 it was demonstrated that a simply constructed  sample holder can produce a high resolution transmitted image


in an unmodified SEM. However, this approach does require  thinning samples to less than 100 nm which requires  significant effort.


An alternate method for satisfying the three conditions for  ultra-high resolution SEM is to image using low-loss  electrons. When a high energy electron beam enters a sample  at very high tilt angle, a significant fraction of the incident  electrons will be forward scattered from the sample surface  with relatively little energy loss. The electrons with the  smallest energy loss will have experienced the smallest path  length through the material and thus will be highly localized to  the beam impact area. The low-loss signal is typically detected  by a large acceptance angle (~45 degrees) energy-filtered  detector placed below the sample, as developed by Wells at  IBM. 7-9 However, this requires the expense and complication  of adding a special detector to the microscope chamber. Interestingly, some very high spatial resolution “low-loss” images were obtained by Broers using a very different set-up. Broers 10 used a very small acceptance angle (2.6 degrees  semi-angle) detector in the forward scattered position, and  although it was equipped with an energy filter he left the filter  turned off while obtaining very high resolution images! This  suggests that a narrow collection angle may be a more  efficient method of selecting the high resolution low-loss  electrons than energy filtering.


Sample Holder Design


In this paper a simple method for collecting the forward  scattered beam is demonstrated which does not require an  energy filtered detector. The sample is mounted to a special  holder (see Figs. 3-5) which places the sample at high tilt  angle to the beam. The forward scattered high-energy  electrons will strike a gold reflector that then creates  secondary electrons that are collected by the SEM chamber’s  regular secondary detector. The holder is designed with the  sample surface pointed away from the secondary detector so  that only the forward scattered electrons contribute to the  image. Note the similarity to the STEM-in-SEM holders  previously published. 5,6


Fig. 3: Design for sample holder with integrated detector for  forward scattered electrons.


Fig. 4: Optical image of the front of the sample holder.


Fig. 5: Optical image of the back of the sample holder.


This technique does not provide any energy filtering of the  forward scattered electrons, so it will be referred to as “forward scattered electron imaging” rather than “low loss  electron imaging.” However, it is expected that the best  resolution will be achieved when imaging only with the  forward scattered electrons that travel the minimum distance  through the sample. These electrons will tend to have the least  lateral scattering, so in order to achieve the best imaging a  relatively small gold target was chosen and the remaining  surfaces of the aluminum holder body were painted with  electron absorbing carbon paint. A graphite “beam stop” was  also added behind the holder. In this design, the gold target  was 4 mm wide which only allowed electrons with a  horizontal or vertical deflection of less than 10 degrees to hit  the gold target.


The major drawback to this technique is that the sample  normal is at very high tilt angle (70o) to the electron beam. Thus the image is highly foreshortened along the vertical axis,


by about a factor of three (1/cos 70o = 2.9).  Also, the lateral  spatial resolution of the image will be somewhat better than  the vertical spatial resolution. However, this is not a major  disadvantage for certain types of metrology. If structures such  as sub-0.1 micron poly lines are oriented orthogonal to the tilt  axis, the line width and edge profile can be measured with  very high precision. Since the forward scattered high energy  beam is relatively unaffected by sample charging, it is also  possible to image insulating materials like photo-resist or spinon-glass at high beam voltage.


Experiments were conducted in a LEO 1550VP field emission  scanning electron microscope with nominal beam diameter of  1 nm at 30 kV. This SEM was not modified in any way other  than the introduction of a special sample holder. The “FSEI” holder is shown in Fig. 3-5. The body of the holder was  machined from stock aluminum. The sample is mounted to a  highly tilted surface near the top of the holder and held in  place by metal clips. The sample surface is pointed away from  the chamber secondary electron detector so that only the  forward scattered electrons contribute to the image. The best  images were achieved at working distance of 2.5 mm or less, so it is necessary that the feature of interest be mounted near  the top of the holder. The maximum sample size for this  holder was about 1 cm by 1 cm, although larger holders could  be built. To use the sample holder in FSEI mode the stage tilt  must be zero and the stage must be rotated so that the back of  the holder points towards the chamber secondary electron  detector. The sample cannot be re-oriented except by  removing it from the vacuum chamber and remounting it.


0.7 micron and 0.2 micron polysilicon gate samples were  prepared from a finished loose die by plasma etching to  remove the passivation and then an HF dip to remove the  metal and dielectric layers. An image was first taken with the  die face pointed towards the secondary electron detector (SED) which produced a normal secondary electron image. The holder was then rotated 180o so that the die surface was  pointed away from the SED, and the only signal reaching the  detector was from secondary electrons produced by the  forward scattered electrons striking the gold reflectors.


Images taken using high beam voltage on uncoated samples  typically have very poor contrast and little surface detail as  seen in Fig. 6. However, when exactly the same beam  conditions (30 kV, 4 mm working distance, 30 micron  aperture, 70o tilt) were used in forward scattered electron  imaging mode, the resulting image was far superior, see Fig.


7. The image contrast and surface detail are both greatly  improved. Please note that this is an uncoated sample imaged  at 30 kV. In many cases coating a sample is undesirable since  the coating may obscure fine detail or interfere with  microanalysis by energy dispersive x-ray or scanning Auger


spectroscopy. Therefore it is useful to have a very high  resolution technique that does not require sputter coating the  sample.


Fig. 6: 700 nm poly lines on silicon, uncoated, 30 kV beam  energy, 70 degrees tilt, secondary electron imaging.


Fig. 7: 700 nm poly lines on silicon, uncoated, 30 kV beam  energy, 70 degrees tilt, forward scattered electron imaging.


One disadvantage of using high tilt angle is the difficulty in  keeping the entire sample in focus due to limitations in the  depth of field, particularly at the short working distances  required for optimum resolution. Thus in Fig. 7 the top part of  the image lacks the sharp focus seen in the bottom of the  image. However, many electron microscopes have a feature  called dynamic focus which allows the electron beam focus to  be automatically adjusted as it rasters across a surface. This  works quite well if the surface is flat as seen in Fig. 8. Most of  the images in this paper were done using dynamic focus.


Figure 8: 700 nm poly lines on silicon, uncoated, 30 kV beam  energy, 70 degrees tilt, forward scattered electron imaging. Dynamic Focus was used to keep the entire sample in focus  despite the high tilt angle.


In order to test the resolution of the forward scattering method  with smaller feature sizes, a sample with 200 nm gates was  imaged, see Fig. 9. This 200,000X magnification image is  slightly less sharp than the 100,000X images. Since the human  eye can resolve about 0.2 mm, one expects that 2 nm  resolution will result in a completely sharp 100,000X image, and 1 nm resolution will result in a completely sharp  200,000X image. Therefore the resolution of these images  appears to be between 1 and 2 nm.


Mag = 200,000X


Fig. 9: 200 nm polysilicon lines on silicon, 30 kV beam  energy, 70 degrees tilt, forward scattered electron imaging.


Photoresist


Photo-resist is a highly insulating material that is typically  imaged in the SEM either with a metal sputter coating or at  low beam voltage (~ 1 kV). However, the forward scattered  low loss electrons with close to 30 keV energy are much less  sensitive to sample charging than are the low energy


secondary electrons with less than 50 eV energy, therefore it is  possible to image uncoated resist with a 30 kV beam using the  forward scattering technique.


A photo-resist layer 1 micron thick on silicon dioxide was  patterned and developed with a test structure, and then imaged  with a 30 kV electron beam using the forward scattered  technique, see Figs. 10 and 11. No charging or sample damage  was observed. Since the resist has a lower density than silicon  or metals the incident beam should tend to penetrate deeper  into the sample before being scattered towards the detector. Thus it was expected that the spatial resolution and surface  sensitivity would be reduced when imaging resist compared to  imaging other semiconductor materials. However, Fig. 11 at  40,000X is quite sharp and surface sensitive, which is a very  surprising result.


To test the limit of the technique on fine resist features, a  PMMA (poly methyl methacrylate acid) e-beam resist layer  250 nm thick was patterned by electron beam lithography with  50 nm lines, see Fig. 12. Although the contrast in this  200,000X image is marginal the 50 nm lines are clearly  visible, which is a remarkable result since very fine resist  structures such as this are almost always sputter coated before  imaging. Imaging of uncoated resist lines below 100 nm  represents a new metrology capability.


25 microns


Mag = 850X


Fig. 10: Photo-resist on silicon dioxide, uncoated, 30 kV beam  energy, 70 degrees tilt, forward scattered electron imaging.


0.5 micron


Mag = 40,000X


Fig. 11: Photo-resist on silicon dioxide, uncoated, 30 kV beam  energy, 70 degrees tilt, forward scattered electron imaging.


Fig. 12: PMMA e-beam resist on silicon dioxide, uncoated, 30  kV beam energy, 70 degrees tilt, forward scattered electron  imaging.


Nanostructures


In a further attempt to test the capabilities of the forward  scattered imaging technique, various nanotechnology samples  were collected. Fig. 13 shows a nanodevice called a “break  junction.” A 50 nm wide gold wire was written by electron  beam lithography and then electro-migrated to create a small  gap. Various organic molecules can be applied across the  junction so that electrical properties can be measure on very  small organic samples.  In Fig. 13 the 25 nm break in the gold  wire is clearly visible, as is a 10 nm thick layer of amorphous  carbon film crossing the junction.


Fig. 13: Break junction, uncoated, 30 kV beam energy, 70  degrees tilt, forward scattered electron imaging.


Fig. 14 shows a test structure written by using spin-on-glass as  an e-beam resist. Since spin-on-glass is an organic insulating  material this sample was almost as challenging to image as  photoresist, but the quality of the image is quite good. Figs. 15  and 16 are carbon nano-filaments, 50 nm in diameter.


Fig. 17 is from an actual failure analysis problem, an  investigation of the grain structure of pentacene, an organic  semiconductor. In Fig. 17 a 50 nm thick pentacene film covers  the top of a gold electrode on the left side of the image, and  covers thermal oxide on the right side of the image. The grain  size is reduced on the gold electrode which affects device  performance. It was also noted that 50 nm diameter extrusions  of pentacene occur at the gold / oxide interface.


200 nm


Fig. 14: Spin-on-glass, uncoated, 30 kV beam energy, 70  degrees tilt, forward scattered electron imaging.


Mag = 50,000X


Fig. 15: 50 nm diameter carbon extrusions, uncoated, 30 kV  beam energy, 70 degrees tilt, forward scattered electron  imaging.


Mag = 300,000X


Fig. 16: 50 nm diameter carbon extrusions, uncoated, 30 kV  beam energy, 70 degrees tilt, forward scattered electron  imaging.


Fig. 17: Pentacene thin film on gold (left) and oxide (right), uncoated, 30 kV beam energy, 70 degrees tilt, forward  scattered electron imaging.


Image correction


The use of high tilt angle foreshortens the image resulting in  image distortion such as the compressed letter “P” in Fig. 10. However it is easy to correct this distortion by resizing the  vertical scale of the image with a graphics program, as shown  in Fig. 18. Some scanning electron microscopes have this  feature labeled as “tilt correction”. Note that image correction  works well for very flat samples but any features that protrude  out of the flat plane of the sample will be severely distorted by  this procedure.


Fig. 18: The image from Fig. 9 was re-sized in the vertical  direction by 3x to restore the letter “P” to correct the image  distortion produced by the high tilt angle.


When discussing a new imaging technique, one always asks  the question: what physical effect produces the contrast in the  image? In forward scattered electron imaging, electrons will  be scattered towards the target when they undergo collisions  with atoms in the sample. In this aspect the technique is more  similar to TEM (transmission electron microscopy) than to  SEM, since TEM contrast is also based on electron trajectories  being changed through scattering by atoms in the sample. One  might almost be tempted to refer to forward scattered imaging  as “glancing angle TEM” especially since the magnification  achieved by this technique are most often associated with  TEM imaging.


When high energy electrons impact a sample at high tilt angle, as many as 50% of the electrons are scattered off the surface  by a single scattering event near the point of impact, and these  electrons will thus carry very high resolution and surface  sensitive imaging information.  7


The images produced by forward scattered electron imaging  are in many cases superior to the low loss electron images  published in the literature. This is true despite the very simple  hardware used for forward scattered electron imaging. This


confirms that collection of a small solid angle of the forward  scattered beam is more effective at selecting the highresolution and surface sensitive electrons than selecting out  the low-loss electrons with an electron energy filter. This  explains the excellent “low-loss” images Broers achieved with  his energy filter turned off.


In the case of forward electron scattering, electrons will be  scattered towards the target when they undergo either elastic  or inelastic collisions with atoms in the sample. In the case of  low-loss imaging, only the inelastic collisions will result in the  electrons being collected or not by the detector. Since the  combined scattering cross-section for elastic and inelastic  collisions is higher than for inelastic collisions alone, that may  explain why the forward scattered technique is highly  effective compared to low-loss imaging. A detailed discussion  of how electron scattering theory applies to this problem is  outside the scope of this paper but may be forthcoming in a  different venue.


High energy electron beams will sometimes damage sensitive  materials such as polymers. However, in taking several dozen  very high magnification images on polymer films, damage  such as melting, vaporization, or electrostatic discharge was  never observed, despite using slow scan at 200,000X and  focusing and stigmating at 800,000X with 1/3 partial field. The lack of damage is somewhat surprising, but may be  explained by the high tilt angle which distributes the deposited  energy across a large surface area. Also, the energy absorption  per path length falls as the beam energy increases so the actual  energy deposition at the point of impact is less for higher  beam energy.


For the electron microscope used in these experiments, the  spot size increases very little as the beam energy is decreased  from 30 keV to 10 keV. Since the mean free path for electron  scattering decreases as the beam energy decreases from 30  keV to 10 keV, it might be expected that using lower beam  energy could produce scattered electrons that are more highly  localized to the beam spot and thus produce higher resolution  forward scattered images. However, reducing the beam energy  also reduces the number of secondary electrons created in the  gold targets and thus reduces the contrast of the image. In  practice, forward scattered electron imaging at 10 keV and 20  keV was found to produce poor images.


A new technique has been demonstrated which enables very  high resolution imaging in the SEM using forward scattered  electrons. A self-contained sample-holder/detector is  described that allows this technique to be performed in an  ordinary unmodified SEM. Approximately 1 to 2 nm  resolution images were obtained on uncoated polysilicon  gates, photoresist, and nanodevices. Dynamic focus and image  correction were used to compensate for the high tilt angle. This is a promising new technique for sub-100 nm metrology.


I would like to thank Leslie Lorenz and George Dearstine who  machined the STEM-in-SEM holder, and Adarsh Kumer who  provided gold films used as reflectors. Stephanie Getty, Tobias Durkop, Yung-Fu Chen, and Mihaela Breban provided  the nanodevice samples. The e-beam resist sample was  prepare by Kosta Vlahacos and the photoresist sample was  prepare by Steven Brown.


1. L. Tsung, A. Anciso, R. Turner, T. Dixon, and N. Holloway, Proceedings of ISTFA 2001, p. 299-302 (2001).


2. Joseph I. Goldstein, Dale E. Newbury, Patrick Echlin, David C. Joy, A. D. Romig, Jr., Charles E. Lyman, Charles  Fiori, and Eric Lifshin, Scanning Electron Microscopy and Xray Microanalysis, A Textbook for Biologists, Materials  Scientists, and Geologists, 2nd  Edition, Plenum, New York, 1992, p. 219.


3. Private communication, Peter Gnauck, LEO Electron  Microscopy GmbH.


4. Joseph I. Goldstein, Dale E. Newbury, Patrick Echlin, David C. Joy, A. D. Romig, Jr., Charles E. Lyman, Charles  Fiori, and Eric Lifshin, Scanning Electron Microscopy and Xray Microanalysis, A Textbook for Biologists, Materials  Scientists, and Geologists, 2nd  Edition, Plenum, New York, 1992, p. 89.


5. W. E. Vanderlinde, Proceedings of ISTFA 2002 pp. 77 (2002).


6. E. Coyne, Proceedings of ISTFA 2002 pp. 93 (2002).


7. O.C. Wells, Appl. Phys. Lett. 19 (7) p. 232-235 (1971).


8. O.C. Wells, Appl. Phys. Lett. 49 (13) p. 764-766 (1986).


9. O.C. Wells, F.K. LeGoues, and R.T. Hodgson, Appl. Phys. Lett. 56 (23) p. 2351-2353 (1990).


10. A.N. Broers, B.J. Panessa, and J.F. Gennaro, Proceedings  of the Eighth Annual Scanning Electron Microscope  Symposium (SEM/1975), IIT Research Institute, Chicago, p. 233-242 (1975).


# Session 7: Failure Analysis Process 


Richard Ross • IBM Microelectronics • Essex Junction, VT


p 167-176


DOI: 10.1361/cp2003istfa167


## Contributions of a Formal Analysis Metaprocess to Breakthrough Failure Analysis Results


Contributions of a Formal Analysis Metaprocess to Breakthrough Failure  Analysis Results


Steve Ferrier, Kevin D. Martin, Donald Schulte, Ph. D


The Hewlett-Packard Company  1000 NE Circle Blvd


Corvallis, OR 97330


541-757-2000


Application of a formal Failure Analysis metaprocess to a  stubborn yield loss problem provided a framework that ultimately facilitated a solution.  Absence of results from conventional failure analysis techniques such as PEM (Photon  Emission Microscopy) and liquid crystal microthermography frustrated early attempts to analyze this low-level supply leakage failure mode.  Subsequently, a reorganized  analysis team attacked the problem using a specific toplevel metaprocess.(1,a)


Using the metaprocess, analysts generated a specific unique  step-by-step analysis process in real time.  Along the way, this approach encouraged the creative identification of  secondary failure effects that provided repeated  breakthroughs in the analysis flow.  Analysis proceeded  steadily toward the failure cause in spite of its character as a  three-way interaction among factors in the IC design, mask  generation, and wafer manufacturing processes.  The  metaprocess also provided the formal structure that, at the  conclusion of the analysis, permitted a one-sheet summary  of the failure's cause-effect relationships and the analysis  flow leading to discovery of the anomaly.


As with every application of this metaprocess, the resulting  analysis flow simply represented an effective version of  good failure analysis.  The formal and flexible codification  of the analysis decision-making process, however, provided  several specific benefits, not least of which was the ability  to proceed with high confidence that the problem could and  would be solved.  This paper describes the application of  the metaprocess, and also the key measurements and causeeffect relationships in the analysis.


a Metaprocess: A process whose function and purpose is to create


another process.


Historically, the literature in the Electronic Device Failure  Analysis field has focused on the discipline's measurements  and equipment to the relative neglect of the analysis process  and methodology.  The few efforts to describe the process  have suffered from the difficulty of attempting to  simultaneously create a general, widely applicable process  description and also a tool that recommends specific, practical analysis operations.  Recent work(1) has generated  a candidate solution (termed a metaprocess), which was  applied to the analysis problem described in this paper.   Here, the intent is to demonstrate the application of this  metaprocess to a particular yield problem, describe the  specific contributions of the metaprocess, and identify the  resulting analysis flow and outcomes.


No claim is made of a new way of performing failure  analysis.   Rather, this approach attempts to contribute to  effective analysis methodology by constructing a context  for application of the same analysis steps applicable to any  problem.


Manufacturing and Failure Mode


The yield failure mode, labeled VDD Leakage, occurred in a  specific printhead IC manufactured in a 1.0µm single-poly  three-metal CMOS process.  Although this is a relatively  simple wafer process, the mode's characteristics conspired  to counteract any real benefit from the process simplicity.  Up to 80% of the IC's manufactured exhibited a slightly  elevated (but definitely anomalous) supply leakage current  in a standby configuration compared to comparable IC  designs.  The anomalous leakage current revealed itself as a  sloppy cumulative current distribution curve (Fig. 1) compared to the clean curves of non-failing designs (Fig. 2).


IDD


Σ<x


Figure 1:  Cumulative distribution of failing design leakage  behavior of wafer lots with only 20% of IDD currents falling below 200nA.


Figure 2:  Cumulative distribution of leakage behavior of related but non-failing design with IDD of over 90% of devices  falling below 200nA.


Another fact stood out at the outset as a clear clue.  The  leakage did not occur on the susceptible design when it was  manufactured in an older wafer process with significantly  heavier n-well doping.


Early failure analysis indicated no correlating liquid-crystal  transitions, a result consistent with the leakage levels of  approximately 1-5µA.  Other traditional analysis  measurements (including a search for correlating photon  emission) also proved unsuccessful.  In spite of months of  yield loss without a resolution, the team responsible for  yield refused on principle to simply raise the test limit and  redefine this product as 'good'.


Application of the Metaprocess


The problem was eventually returned to the IC's designers, and a task force assembled across design and manufacturing  organizations to solve the problem.  The ensuing analysis  was guided chiefly by a cyclic metaprocess, summarized in  Fig. 3.  This metaprocess performed a critical three  functions for the analysis effort.


Function 1. The metaprocess provided a constant focus on


(a) the nature and details of the cause-effect network that  the failure had created, (b) the analysis path, and (c) the  location (status) of current analysis activity on that path.


The metaprocess provided this function through the  canonical form of the E/C/C Question, "Does <the selected  specific possible prior cause> Exist, Correlate with <the  known, observed failing behavior>, and Cause that  behavior?  For example, at one point the question became: "Does the possible gate oxide short exist, correlate with the  known quadratic IDD leakage, and cause that leakage?"  Depending upon the answer to this question, one of the  following three cases applied:


I.


The analysis path is false (in this example, the  possible cause, a gate short, did not exist);


II.


The analysis path is near the main cause-effect  relationship (the possible cause, a gate short, existed and correlated with the observed quadratic  IDD behavior);


III.


The analysis path is at the main cause-effect  relationship (the possible cause, a gate short  existed, correlated with the known IDD behavior, and was related to the behavior as cause and effect  by a specific physical law of transistor operation).


Function 2.  The metaprocess directed focus evenly on both  halves of any good analysis: measurement and prior cause  postulation.  The former tempts many analysts to neglect to  focus on possible prior causes.  The Correlation List step (middle bottom) forced consideration of possible causes for  the observed behavior, and then focused analysis  measurement design to the goal of detecting secondary or  side effects of those possible causes.(2)  This repeatedly


Figure 3:  Cyclic metaprocess used during solution of  VDD leakage problem.


Figure 4:  IDD(VDD,T) for a failing IC, with a superimposed flat


1.0uA test limit surface.


drove innovation and inspired creative analysis approaches.  Conversely, the Measurement step (middle top) disciplined  the construction of the Correlation List to treat possible  prior causes arising from the failure's anomalous behavior  rather than from speculation.


Function 3.  The metaprocess provided application points  for methodical analysis logic.  At some points during  analysis, behavior that correlated with failure differed very  little from behavior that did not.  The metaprocess  facilitated the use of logical principles able to accurately  distinguish fine differences, such as the Contrapositive  Testb and Inductive Proof.c


Analysis Flow


The following section describes the overall analysis flow  arising from the metaprocess, including some details of its  application.


A. Failure Mode Verification and Characterization


In verifying failure mode, analysis began with a focus on  the causes and effects operating in the failing IC, incorporating the first function informed by the  metaprocess described earlier (providing a constant focus  on the nature and details of the cause-effect failure-created  network, the analysis path, and the location of current  analysis activity on that path).  The metaprocess loop was  initiated, as Fig. 3 indicates, at the E/C/C Question step.


b Contrapositive Test: The test of a statement P by seeking a valid  consequent Q that is false.  P=>Q means that any ~Q=>~P.  In FA  terms, if a sure effect is truly absent, its cause is absent.


c Inductive Proof: The proof of a statement P by sufficient demonstration of valid and true consequents Qn without exception: for  n>sufficient limit, P=>Qn and all Qn are found true.  In FA terms, if  the first predicted side effect is present, test for the next.  If sufficient side effects are present without exception, declare the common cause of all side effects proven and therefore present.


E/C/C Question:  Does the reported VDD leakage exist, correlate with the complaint, and cause this IC to be  categorized as a failure?


Measurement:  Under conditions matching the failed test, the die under analysis exhibited anomalous IDD(VDD,T) current (Fig. 4).


Interpretation:  Voltage and temperature behavior of the  anomalous current matched the complaint behavior.


E/C/C Answer:  VDD leakage existed, correlated with the  complaint, and caused the IC to be categorized as a failure.


Figure 1: Frontside emission microscopy on SRAM cell area


Many metal layers including fill structures make an exact  localization of the failure nearly impossible. Also switching to  the chip backside is not a real solution. On highly integrated  technologies one emission spot covers up to ten possible faulty  transistors.


Global fault localization for SRAMs can be easily done by  using the test results and generating a physical fail bit map. This information will be used in our SRAM analysis strategy  as a starting point.


On one hand, simple top down preparation on the concerned  location gives no conclusive result in many cases but is very  fast. An experienced FA engineer can deprocess and inspect  every concerned layer within one day. One the other hand  microprobing on FIB pads gives a good failure hypothesis for  further physical preparation but is very time consuming (and  approximately a factor of three to five on cost). The proposed  SRAM analysis strategy will guide the FA engineer to do a  reliable job in a reasonable time.


In this paper a technology and layout independent SRAM  failure analysis strategy will be presented. It is based on a  previous SRAM analysis flow for a specific SRAM design [2].


Requirements and global analysis flow


The starting point for every failure analysis job on memories  is the physical fail bit map. It can be calculated from the result  of external test algorithms applied with an ATE if the SRAM  can be tested ‘through the pads’ and taking the descrambling  of the memory into account.  Also very common are memory  built-in self test (MBIST) [3]. Using the diagnosis mode of the  MBIST a physical fail bit map can be delivered. Additional  necessary informations are voltage and temperature  dependencies. Failures only at high temperatures can point out  to possible problems with leakages. Low voltage and low  temperature failures might indicate failures at interconnects.  In the SRAM analysis strategy, the failing test algorithm (checkerboard, walking ‘1’…) and the used background  patterns are also taken into account to cover the impact of one  SRAM cell to the neighboring SRAM cells [4].


The SRAM failures are classified by the pattern formed by the  failing cells of the physical fail bit map.


Figure 2: SRAM analysis flow - overview


Figure 2 shows an overview of the analysis strategy with the  pattern formation as a starting point. We distinguish several  typical failure signatures such as bit line (BL) or word line (WL) oriented failures, single cell failures (SCF) or clusters of  SCF. The failure analysis strategy for these signatures is  different in each case and will be described for bit line  oriented failure and SCF later.


Horizontal and vertical pair cell failures (HPC, VPC) are  special kinds of clusters for which we can assume a clear  failure hypothesis from the layout of the concerned SRAM  cells. We define vertical pair cells as two SRAM cells with  common bit line contacts. The physical failure hypothesis for  this specific case is very simple and localized inside the bit  line / bit line bar (BL/BLB) interconnect.


However, there are some global SRAM failures which exhibit  at the physical fail bit map no significant pattern. Examples  for this are the total failing of an SRAM IO (several bit lines  multiplexed to one IO of the SRAM macro) or failures of the  decoder logic circuit which will cause the failing of large  blocks of the SRAM area. These failures will be dealt like  functional failures and the standard analysis flow is used, including global fault localization using emission microscopy, TIVA, EBEAM measurement or laser voltage probing. One  example for this approach will be shown later.


Case studies


This paper focuses on three different failure signatures (SCF, bit line oriented failures and global SRAM fails) and describes  the detailed analysis strategy used and shows case studies for  this specific failure signatures.


Bit line oriented failure


The bit line oriented failures are distinguished into three types: partial and full fails of bit lines and a specific electrical failure  signature called 511+1 (figure 3).


Figure 3: Different bit line oriented failures


Figure 4: Detailed analysis flow for partial fails of bit lines


A very specific failure is the 511+1 signature. On a SRAM  with 512 rows (word lines) 511 cells at one bit line fail stuckat 0 and one cell stuck-at 1 using a march 10 test algorithm


[4]. The only possible physical failure is a short between  BL/BLB interconnect and the word line at the location of the  stuck-at 1 failing SRAM cell using a NMOS selection  transistor. During the test of row x, the word line is forced to  high for the selection of the row. With the above mentioned  failure hypothesis the cell will fail stuck-at 1. If any other row  is selected the word line x is forced to zero and will cause a  stuck-at 0 failure signature.


On full fails of bit lines, two possible failure locations are  likely: a low ohmic short at the cell array or a failure located at  the bit line logic (precharge, discharge, multiplexer). To  distinguish the two failure locations, global failure localization  methods are necessary. Due to the high density of metal lines  at the SRAM area, backside methods such as emission  microscopy or TIVA will be chosen.


Figure 4 shows the detailed analysis strategy of partial bit  lines fails. The dependency on voltage or temperature of the  physical fails signatures gives a first indication for a failure  hypothesis. If the amount of failing SRAM cells varies by  voltage or temperature, the first guess is a failure at the bit line  logic and global backside failure analysis techniques are used.  With a voltage and temperature independent fail signature, the  physical failure hypothesis is an open located near the first


failing cell. The device will be delayered by means of surface  parallel polishing into the VIA level above the bit lines. Inspection of the concerned area using optical microscopy or  SEM (depending on technology) will be done.


Figure 5 shows a SEM image of a partial bit line failure on a  device fabricated in deep sub-micron technology.


Figure 5: SEM image of partial bit line failure


All metal layers above the bit line level were removed by  surface parallel polishing and the inter-metal-oxide (IMOX) was removed step by step using RIE plasma etching. Inspection with SEM shows missing metal due to a local  process fault exactly at the location of the first failing SRAM  cell at the concerned bit line.


Single cell failures (SCF)


Single cell failures are a real challenge for failure analysis  especially when step by step delayering and inspection comes  to no conclusive result. Also, the microprobing approach is  very time consuming. Therefore we decided on the strategy  used by taking into account the availability of several failing  devices with the same electrical failure signature (figure 6).


Figure 6: single cell fails


Using the delayering approach, possible faulty layers were  extracted from the layout of the SRAM cell. All metal layers  above the first possible failing layer are removed by surface  parallel polishing. At every possible faulty layer, voltage  contrast with SEM or FIB in comparison to the neighboring  cells and inspection with SEM are performed. If no obvious  feature is observed, the layer is removed by polishing or wet  chemistry.


However, if the delayering approach failed or only a limited  set of devices with the same electrical failure signature is  available, microprobing on single SRAM cells has to be done  to get a physical failure hypothesis (figure 7). In a first step, the possible faulty layers are extracted from the layout. In  order to have access to the single SRAM cell, all layers  excluded by layout consideration mentioned above are  removed by surface parallel polishing. To get electrical access  to the concerned SRAM cell via the BL/BLB interconnects the  word line for this row has to be connected to Vdd (NMOS  selection transistor) and the word line (n-WL) of the  neighboring SRAM cell using the same BL/BLB interconnect  has to be blocked by connecting it to Vss.


Figure 8 shows the FIB preparation for microprobing on a  single SRAM cell in a deep sub-micron technology. The  device was surface parallel polished into the VIA layer and an


Figure 7: microprobing approach


insulator was deposited by FIB. Bit line, bit line bar, Vdd and  Vss are connected via FIB pad; the word line is forced to Vdd  and the n-WL to Vss. The size of the FIB pads is  approximately 3 µm x 3 µm. Figure 9 shows the result of  microprobing on a failing SRAM cell. A short of the bit line to  Vss is clearly visible.


Figure 8: FIB pads for microprobing a single SRAM cell on a  deep sub-micron technology


Figure 9: V-I-characteristic of BL/BLB versus Vss


The physical root cause of this electrical failure signature was  a local polysilicon patterning defect causing a short between  gate poly and source (Vss) (figure 10).


If the V-I-characteristic of BL/BLB is without objection, the  toggling behavior of the concerned SRAM cell will be


measured. Therefore the SRAM cell will be powered up by


supplying Vdd and Vss. Forcing a low at BL,  a high signal at  BLB can be measured and vice versa. The toggling current of  the SRAM cell can be measured by applying a voltage ramp  from high to low at BL/BLB and measuring the current


flowing in or out the SMU (Source Monitor Unit). Figure 11  shows a typical toggling behavior of a SRAM cell fabricated  in a deep sub-micron technology.


Figure 10: pattering defect inside SRAM cell causing short


Figure 11: measurement of toggling current


Global SRAM failures


In few cases the physical fail bit map does not give failure


localization especially if large SRAM blocks fail. Therefore  the normal analysis strategy is to perform global fault


localization by emission microscopy or other tools and


techniques. After localizing the failing block, a hierarchical  approach (figure 12) is used.


Figure 12: hierarchical fault localization for global SRAM failures


An example for these global SRAM failures is the failing of


all bit lines connected to one SRAM IO buffer (schematic


shown on figure 13). Due to layout considerations, the failure


cannot be located inside the SRAM cell array.


Figure 13: schematic of SRAM In-Out buffer


This kind of electrical failure signature appeared after burn-in. Global fault localization by using emission microscopy and


TIVA failed, no additional signal was detected. Therefore the  device was depassivated and EBEAM probing was performed  for localizing the failing block. The signals of the several


blocks inside the in-out buffer and the output of the


multiplexer were not covered with metal lines but not all can  be probed in the top metal layer. To allow measurements at


deeper metal levels with EBEAM, small holes were formed


with the FIB to get access to the signals. The functional test


program for stimulation of the failure was reduced to a read - write access of the concerned SRAM block in order to


minimize the measurement time and to improve the accuracy  of the EBEAM measurement.


Figure 14 shows the results of the EBEAM measurement. The  output of the sense amplifier (measurement point M2) of the  failing block shows no difference in comparison to a reference  block of the same SRAM while the output of the SRAM IO


structure (measurement point M3) of the failing block does not  change. This leads to the failure hypothesis that the output


buffer between the measurement points M2 and M3 of the  SRAM IO is failing.


With this global fault localization, the possible failing


transistors can be reduced to approximately 10. The failing  part was step-by-step deprocessed by surface parallel


polishing and inspected with SEM.


Figure 15 shows the physical root cause of this failure. A  metal extrusion causes a short of an internal signal of the  output buffer versus Vss.


Figure 14: results of EBEAM measurement


Figure 15: physical root cause: metal extrusions causing short  of two metal lines


The SRAM analysis strategy used at the Infineon Munich FA  department is shown. Thanks to the standardization of the


work flow, this approach significantly fastens SRAM analysis  and improves the quality of the analytical work. The knowhow of SRAM analysis can be easily transferred to other FA  locations.


The authors would like to thank S. Pauthner for FIB pad


preparation and K. Mittler for visualizing the SRAM analysis  strategy.


Many thanks to the Munich FA team for the fruitful


discussions.


Thanks to the management of the FA lab in Munich especially  F. Bruns and S. Görlich for the assistance to this work.


1. J.-Y. Glacet, F. Lee : Embedded SRAM Bitmapping  and Failure Analysis for Manufacturing Yield  Improvement, Proc. of the 26th. ISTFA 2000


2. C. Brillert et. al. : SRAM Failure Analysis Flow, Proc. of the 27th. ISTFA 2001


3. Kinoshata, K. and Saluja, Built-in Testing of  Memory using on-chip compact testing scheme, Proc. Of IEEE International Test Conference (1984)


4. R. Kunin A.J. van de Gore, Testing Semiconductor  Memories, ComTex Publishing, Gouda, The  Netherlands, (1998)


p 184-190


DOI: 10.1361/cp2003istfa184


## VLSI design for functional failure analysis in the < 90 nm and flip- chip era


VLSI design for functional failure analysis in the < 90 nm   and flip-chip era


Yoav Weizman, Ezra Baruch


Motorola Semiconductor Israel – Product Analysis & Characterization


In recent years, two new techniques were introduced for flip  chip debug; the Laser Voltage Probing (LVP) technique and  Time Resolved Light Emission Microscopy (TRLEM). Both  techniques utilize the silicon’s relative transparency to  wavelengths longer than the band gap. This inherent  wavelength limitation, together with the shrinking dimensions  of modern CMOS devices, limit the capabilities of these tools.


It is known that the optical resolution limits of the LVP and  TRLEM techniques are bounded by the diffraction limit which  is ~1um for both tools using standard optics. This limitation  was reduced with the addition of immersion lens optics. Nevertheless, even with this improvement, shrinking transistor  geometry is leading to increased acquisition time, and the  overlapping effect between adjacent nodes remains a critical  issue. The resolution limit is an order of magnitude above the  device feature densities in the < 90nm era. The scaling down  of transistor geometry is leading to the inevitable consequence  where more than 50% of the transistors in 90nm process have  widths smaller than 0.4um. The acquisition time of such nodes  becomes unreasonably long. In order to examine nodes in a  dense logic cuicuit, cross talk and convolution effects between  neighboring signals also need to be considered. In this paper  we will demonstrate the impact that these effects may have on  modern design.


In order to maintain the debug capability, with the currently  available analytical tools for future technologies, conceptual  modification of the FA process is required. This process  should start on the IC design board where the VLSI designer  should be familiar with FA constraints, and thus apply features  that will enable enhanced FA capabilities to the circuit in hand  during the electrical design or during the physical design  stages. The necessity for reliable failure analysis in real-time  should dictate that the designer of advanced VLSI blocks  incorporates failure analysis constraints among other design  rules.


The purpose of this research is to supply the scientific basis  for the optimal incorporation of design rules for optical  probing in the < 90nm gate era.


Circuit designers are usually familiar with the nodes in the  design which are critical for debug, and the type of  measurement (logic or DC level) they require. The designer  should enable the measurement of these signals by applying  certain circuit and physical constraints. The implementation of  these constraints may be done at the cell level, the block level  or during the integration.


We will discuss the solutions, which should be considered in  order to mitigate tool limitations, and also to enable their use  for next generation processes.


With the advent of multi metal layer processes, flip chip  packaging and the continuous shrinkage of critical geometries, the ability to access internal nodes during probing and silicon  microsurgery has become increasingly difficult.


Therefore, in recent years several design hooks were  developed to circumvent these difficulties. These design  hooks, also known as design for debug (DFD), are designed  into the silicon circuit, and are generally divided into two  categories; design for engineering modifications (i.e. FIB) and  design for probing.  In the first category, we may find spare  logic cells with special backside/frontside access and  spare  lines routed across the chip to distribute the signals from the  spare cells without adding considerable RC delay. Also  counted in this category are hooks for backside mechanical  probing. Elaborated discussion on various types of DFD for  easier silicon microsurgery can be found in ref 1. The need for  design for probing on the other hand is emerging from the  continuous shrinkage of transistor geometries, and is  becoming critical in < 90nm processes due to the optical  limitations of the probing tools. During the last 3-4 years in  which the flip-chip packaging and multi-metal layer devices  became customary designs, backside tools became an essential  part of failure analysis laboratories. The first limitation that is  encountered by the analyst is the difficulty in resolving small  geometries from the backside. The active regions look like  gray clouds already blurring in 0.13um designs. Nevertheless, the use of accurate stages and CAD overlay capability, which  are essentially incorporated into any modern backside tool,


could alleviate spatial resolution issues. Optical probing tools  also suffer deficiencies in acquisition capability and  interference effects due to shrinking transistor dimensions.


Currently there are two diagnostic tools that are used for  backside probing, the first is the laser voltage probing (LVP) and the second is Time Resolved Light Emission Microscopy (TRLEM). The LVP is an IR probing technology (2) that  provides a way to measure voltage waveforms directly from  the P-N junction. The small optoelectronic interaction that  occurs between the focused beam and the junction can be  measured stroboscopically to determine the voltage variations  at the internal signal node. This technology was the primary  and only solution during the early days of flip-chips. TRLEM


(3) technique was developed more recently, and is becoming a  customary tool for debug. The TRLEM is a non-invasive, passive optical method for measuring electrical switching of  CMOS transistors and so far is the only solution for SOI  probing.


Resolution limit


Shrinking device geometries in integrated circuits are made  possible by improving optical lithography, which is driven  mainly by decreasing the wavelength of the exposure source. However, optical probing relies on the transmission of light  through the silicon substrate. Therefore, due to the strong  absorption at photon energies greater than the band gap of Si. the wavelength cannot be less than the band gap (~1.1 um). As  a result, backside tools have degraded spatial resolution of the  device features in modern technologies.


Spatial resolution is degraded in optical probing systems  because it is limited by diffraction. A circular lens that will  focus light to a spot with radial intensity distribution I(r), is  given by


νν )(


I ∝


Where


2NArλπ


ν ≡


And


sin(


ϕ


NA ≡


where J1 is the first order Bessel function, r is the radial  coordinate in the focal plane, λ is the optical wavelength, n is  the refractive index of the media (1 for air), and ϕ is half the  total acceptance angle of the lens. The numerical aperture of  the lens NA, determines the size of the focus spot and is the  critical parameter for determining the diffraction limit of the  lens.


The ability to resolve two adjacent spots separated by the  distance dr , is given by the Rayleigh criteria as:


NA


dr


This criteria represents the best possible resolution for a  staring optical system. Scanning systems can improve on this  resolution by 20-30% (5).


Figure 1 – image taken with (a) and without (b) the liquid  immersion lens by the LVP system (100X, 1.3NA). This diode  array represents 0.4um diodes arrangement. A central diode  with 4 neighboring diodes in various spacing ranging between


0.2um  to 1.6um. From the image it appears that without the  immersion lens one can observe two separated diodes only if  they are separated by more then 0.8um. With the immersion  lens it is possible to start resolve the diodes when the distance  is above 0.4um.


Figure 2 – image taken with and without solid immersion lens  by the TRLEM system (100x, no data on NA). This array of  diffusions with increasing distances between the lines.


A diffraction limited optical system is one in which all other  limits to the resolution are smaller than the diffraction limits.


Most modern objective lenses are diffraction limited in the  center of their field  ( of view.


For optical probing, improvement in resolution can be made  only by increasing the numerical aperture. Since sin(ϕ) cannot  exceed unity, and is already in the region of ~0.90 for the  highest resolution objectives available, there is not much gain  in increasing the marginal angle. The greatest benefit is gained  by increasing the refractive index through which the marginal  rays travel. This has been done through the use of liquid  immersion objectives (for the LVP), and more recently by  solid immersion lenses (SIL – for the TRLEM). Figures 1 and  2 show comparisons with and without the use of immersion  lens for liquid immersion lens in the LVP system and with  solid immersion lens in the TRLEM system. The improvement  in resolution certainly makes the orientation easier, however, even with this improvement the Rayleigh criteria still does not  allow the resolution of dense areas as demonstrated in figure


3. Measurements done with the liquid immersion lens using  the LVP technique (6) show that signal was not degraded due  to the incorporation of the lens. In the case of small features  the initial probing noise level (Ni in equation 5) is even better  due to the localization of the beam. With regard to TRLEM  coupled to the DUT with SIL, no data was published on the  effect on the signal acquisition time. Since the SIL is not  totally transparent to the entire emission spectra (0.8-1.3 um) it is expected that the SIL will degrade the quantum efficiency  of the system.


Figure 3 – demonstration of the optical limitations inherent in  IR analytical probing systems with (dotted circle) and without (solid circle) immersion lens (a) Dense probe diodes  measured using the LVP system (beam diameter -FWHM


0.7um/0.55um). Circle containing 3 diodes with considerable  risk of cross talk (b) Dense logic measured using TRLEM with  risk of cross talk or convoluted signals. The circle denotes the  light collection region.


A perfect diffraction limited optical system may still be unable  to produce diffraction-limited images. The object being  imaged is part of the optical system and can also degrade the  total resolving power. For backside imaging, the curvature and


the roughness of the back surface of the silicon can  significantly reduce image quality. However, even a perfectly  polished sample can introduce aberrations in the image quality  at high numerical apertures. Aberrations such as coma and  astigmatism, will occur as the image spot moves away from  the optical center, therefore, mainly affecting the image  quality and not probing capability. The effect of silicon  thickness could also be corrected by the use of a correction  ring in the objective, improving considerably the spherical  aberrations.


Scaling effects


Scaling effects have presented real challenges for optical  probing from the backside since gate geometries were reduced  below 0.25um (5 years ago!). However failure analysis since  these times relied on the fact that large detection regions, i.e. transistors. were accessible for most of the important nodes. As dimensions are reduced this option becomes limited only to  signals attached to moderately large buffers. Such buffers are  normally attached to major buses routed between major  modules in the device, hence relying on such buffers (w>3um) for debug will ensure only a very small coverage of the nodes  across the device. This is represented in the gate width  distribution of n-type transistors in a typical logic test case of  90nm process device shown in figure 4.


Figure 4- This distribution diagram represents the relative  occurrences of gate with specific gate-length combination  across a test case device. This specific device (a  communication processor) with 1.3 106 transistors was  designed at 0.13µm and scaled to 0.09µm. We took into  account only logic N-type with minimum gate Leff (total 4.7  106 transistors) memory bitcells were excluded. The relative  occurrences of gates with w>3µm is approximately 6%.


Approximately 5% of the signals are coupled to buffers with  widths between 3um>w>1um. These signals are fairly easy to  probe with the TRLEM, however, acquisition time  together  with the preparation  time required for orientation is estimated  to take 20-30min per signal, with a state of the art detector at


nominal voltage (1V), moderate timing resolution and optimal  loop length. The rest of the nodes (approximately 90%) are  either not possible to probe or requires acquisition times of  more than 1-3hr per waveform.


Acquisition time


Acquisition time depends on the test pattern loop length, the  ambient noise level, the modulation strength of the signal, the  edge transition time and the acquired timing accuracy. These  parameters could be formulated (7) in the case of LVP into the  following equation for the acquisition time


(SNR


N


mT


loop


acq =


where m is the pixel resolution making up the LVP waveform, Tloop is the test pattern loop length, Ni is the initial background  noise level in ppm, SNR is the signal to noise ratio (1/10 to  achieve timing resolution of 1/10 of rise time), and S is the  signal strength. With 0.13um process, signal levels of around  500ppm could be detected for a loop length of around  100µsec. However, with the decrease in the signal level for the  next process generation (without reduction in the pattern  length) the acquisition time becomes substantially longer, and  adverse effects such as position drifts become critical. Experiments done on diodes of various areas show that there  is no direct relation between the diode size and the reflected  signal as long as the diode contains the beam HWHM. However, when the beam size exceeds diode limit, edge  complicated effects influence the measurement in an erratic  way. The effect of applied voltage on the signal strength (S) shows stable linear dependence. LVP measurements of signals  as low as 0.8V are possible.


Recent developments of time-differential LVP (11) that  improve significantly the noise cancellation technique may  extend the usage of the LVP to the next generation; however  further scaling does not allow practical debug without DFD  that stretches the layout minimum sizing. Another drawback  unique only to the LVP is the inherent invasiveness of this  technique. It has been reported (7) that the photocurrent  expected while probing with the mode-locked laser is ~1uA, such current was not an issue with large nodes; however with  smaller nodes this current might alter the acquired waveform. However this effect should not be observed as long as the on  currents are on the order of several hundreds of uAmps.


The elaborated (3) equation for the TRLEM is given by:











 ∆+


∆∆


sig


dk


res total


sig loop


acq


R


t t


R T


2 2


Where ∆ttot rdk  is the number of dark counts within the width  of the event (∆ttot) per loop and ∆tres is the timing resolution.


Rsig is the number of signal counts within the width of the  event per loop.  The terms in Equation 6 are usually  simplified.  In the limit cases where  Rsig >> ∆ttot rdk  Eq. 6  leads to 1 / Rsig relation; when  Rsig << ∆ttot rdk  leads to 1 /


R2sig relation. In the world of small transistors (w<1um) we  normally operate in the dark-count limited regime where the


acquisition time is quadratic in the signal count rate. The  signal count rate Rsig  can be described as:


∫


∞


Ω


dE


E


w


FET


(7)


Wher α(E) is determined by silicon substrate absorption, optics transmission and quantum efficiency of the detector. wFET is the transistor width and Ω is the solid angle for light  collection. Rsig increases linearly with the transistor width w. The probability RFET that a transistor will emit a photon  during an event depends on the hot electron energy  distribution within the channel and the current. The hot  electron distribution in turn depends on the electric fields  within the channel. Device scaling typically attempts to  maintain a constant electric field in the channel and hence hot  carriers energy tail will remain unchanged (8); as a result, the  emission should remain approximately constant as well. However, Rusu et al. (9) have shown that the device emission  decreases approximately by a factor 2x with each device  generation from 0.25 um to 0.13 um. Similar degradation is  anticipated with the transition to 0.09um. This dictates at least  4x  increase in acquisition time even before we consider the  scaling effect on width of the transistors. The major reason  why scaling does not maintain the constant emission is  because of the inability of scaling technologies to scale oxide  thickness at same rate as Leff and at the same time a greater  decrease in Vdd.


As emission grows exponentially with 1/Vdd, therefore the  dependence of acquisition time on bias voltage is dramatic. In  cases in which failure occurs in voltages lower than nominal  by 0.1V, we expect a 3x-5x  increase in the acquisition times  for 0.13 to 0.09um processes, respectively. Emission intensity  observed from low power devices is by a factor of x3 smaller  in comparison to high power devices due to lower operating  voltages and lower doping concentrations.


Interference effects


The interference between neighboring signals is another acute  problem resulting from shrinking geometry. This problem  became critical in the <90nm processes as demonstrated in  figures 3 and 4.


B. Analysis Flow Generated by the Metaprocess


The main part of the analysis follows.  After the E/C/C  Answer that validated the failure mode, a Correlation List  was next constructed.  This step addressed two (non-E/C/C) questions:


1. What possible prior causes may create the confirmed  VDD leakage?


2. What other effects do each of these possible prior  causes imply?


This step began by implementing the second function  described earlier (directing focus evenly on both  measurement and prior cause postulation).  This was  approached through brainstorming, through research into  failure cause-effect relationships, and through developing a  thorough understanding of the intentional, designed causeeffect relationships applied by the technology.  The  Correlation List for this analysis consisted (in part) of the  items in Table 1.  Note that the side effects represent the  behaviors available for the next measurement(s), and yield  actual prior causes.


Selection:  Items from the Correlation List were selected  for further analysis based upon a set of prioritization


Table 1:  First Cycle Correlation List  Possible Prior Cause of Known


Failing Behavior (VDD leakage)


Predicted or Known  Correlating Side Effect  of Prior Cause (at Left)


Quadratic IDS(VGS)


Transistor on-state


Negative IDS(T)


Quadratic IDS(VGS) Negligible IDS(T)


Gate Oxide short


Strong photon emission


Reverse-biased diode leakage


IDS~V1/2


Forward-biased diode leakage


IF~eV


Subthreshhold current


IDS~eV


Resistive anomaly


I=V/R (linear) I >~ 1mA


Latchup current


Latching effect (hysteresis)


principles. Analysis then proceeded to the E/C/C Question  step and subsequently through the next section of the  metaprocess.  Early IDD(VDD) results (as described) immediately ruled out several of the items on the  Correlation List (such as resistive anomalies) using the  logical principle of the Contrapositive Test.  Since these  were disproved, they were not pursued. The transistor onstate selection presented the most promise; therefore the  analysis pursued that path.


E/C/C Question:  Does an anomalous transistor on-state  exist, correlate with the known VDD leakage and its  characteristics, and cause the VDD leakage?


Measurement:  Anomalous IDD(VDD,T) exhibited quadratic  voltage dependence (Figs. 5 and 6).


Interpretation:  Quadratic voltage dependence was  observed to be consistent with the behavior of an MOS  transistor which is turned on, and corresponded to the wellknown dependence of the source-drain current IDS on the  gate voltage VGS in saturation:(3)


IDS = µεoxW/2Ltox (VGS-Vt)2      (1)


This correspondence supported the possibility that the VDD  leakage was caused by an anomalous transistor on-state.  In


fact, (1) describes a physical law that would permit the  declaration of such an MOS structure (once found) to be a  cause for the leakage.


Measurement:  In answering the E/C/C Question, the  measurement and interpretation steps may be repeated as  many times as necessary.  This next measurement (Fig. 7) indicated that the anomalous IDD (VDD,T) possessed positive  temperature dependence.  Reasons for this characteristic  were not fully apparent during this phase of the analysis, but possible explanations arose near the end of the analysis  from the observed root anomaly.  Even more importantly in  the short term, this characteristic helped localize the failure  site (described shortly).


Interpretation:  This observed temperature behavior was  the opposite of that expected from a transistor.  Normally, channel mobility µ, which dominates(4) the temperature  dependence of the saturated MOS drain current ID, decreases with increasing temperature.(5)  Therefore, the  structure that was causing the anomalous current to flow  should not be solely an MOS transistor.  Nonetheless, the  quadratic I(V) behavior represented an indicator of MOS  transistor involvement that could not be dismissed.  This  conflict was resolved by postulating a structure that  included an MOS transistor, but also incorporated other  components whose temperature dependence dominated that  of the transistor.  Such a structure could be postulated while  leaving its particular components unspecified for the  moment.


Measurement:  Next, a new photon emission measurement  was performed, which again exhibited no emission signal, even at higher voltages and temperatures that significantly  increased the failing VDD leakage.


Interpretation:  System tests verified that the PEM systems  used in these measurements were capable of detecting  emission from forward-biased diode structures passing  currents in the single-digit microampere range.  Recombination rates of MOS transistors were expected to  fall below this range, and therefore any such emission  would remain undetected.  This negative result did,


Figure 7:  2-D plot of the data in Figure 5, exhibiting  positive leakage temperature dependence.


Figure 5:  Plot of the square root of IDD(VDD,T) exhibiting  a linear relationship to VDD axis (note straight surface  grid lines in lighter area).


Figure 6:  2-D plot of the data in Figure 5, indicating the  quality of linear fit to Sqrt(IDD) in higher-VDD regimes.


however, definitively rule out a gate oxide short (whose  stronger emission should have been detected).  The logical  principle of the Contrapositive Test immediately demanded  this conclusion.


E/C/C Answer:  A circuit anomaly that includes a transistor  on-state exists, correlates with the confirmed VDD leakage, and causes it.


Correlation List: The Correlation List (Table 2) was next  constructed.  This list contains possible prior causes for the  just-confirmed behavior (the anomalous transistor on-state), and also includes other side effects (effects other than  observed VDD leakage) of those possible prior causes.  In  clarification of the reset signal entry noted in Table 2, it was  known from earlier work that the external reset pin could  turn off the leakage on failing dice, which led to the reset  state as a possible prior cause in the electrical domain.  The  Table also includes normal transistors in an abnormal on  state due to abnormal electrical conditions, as well as  abnormal (unintended) transistors.


Selection:  The correlation of the reset pin state with the  observed VDD leakage was selected.  This prior cause  postulated that the test, which was expected to set the reset  pin to an active state, actually set it to an inactive state  thereby allowing the leakage to occur.


In order to summarize the next several metaprocess steps, an E/C/C Question was framed concerning the selected  PPC (Possible Prior Cause); that is, the reset pin state's  correlation to the leakage: does an incorrect reset condition  exist, correlate with the leakage, and cause it?  Following  this, a measurement determined that the normal reset state


(rather than the incorrect state) correlated with leakage.  This ruled out incorrect reset pin setup during testing and, in terms of the E/C/C Answer, that this possible prior cause  did not exist.  (Note that this did not mean that the  correlation of the reset pin state to the failure was ignored, but rather that a test error creating the leakage by an  incorrect reset pin state was ruled out.)


From the metaprocess flow, the next step would be to make  a new selection from the same Correlation List since the  prior cause of the same known effect was still under  examination.  In order to pursue the remaining Correlation  List items (as described), however, it was necessary to  resolve the question of exactly which structure was causing  the leakage.


The most important methodology question at this stage in  any analysis is: how can more information about the causeeffect relationships involved in the failure be obtained?  This question drives the most challenging and significant  operation within typical analysis flows: localization.  Localization is valued as the only effective way to gather  extensive information about the effects created by a defect.  The ultimate purpose of localization is to provide greater  access to the cause-effect network immediately surrounding  the defect.


During a localization operation, the analysis makes no  progress down the cause-effect chain.  Instead, the analyst  spends time and effort working to place the known failure  behavior characteristics at some location in the IC's  physical structure.  This means that the analysis remains at  the same point in the cause-effect chain while the spatial  correlation of the failure's known behavior is identified.


In this case, PEM and Liquid Crystal provided no signals  for localization.  The IC was too complex to perform  electrical localization in the design's own cause-effect  domains (blocks' effects on other blocks), and the network  of metallization was too dense to easily permit Focused Ion  Beam (FIB) cut localization of the leakage path (from the  topmost die level).


The discipline imposed by the Correlation List step (demanding enumeration of all possible secondary effects  of the possible prior causes) yielded a return at this point.  The leakage's positive temperature coefficient (Figs. 5-7) should be local to the anomaly site.  The analysts therefore  sought to locate this characteristic in the die interior.


E/C/C Question:  Does a local thermal effect exist, correlate with the observed global IDD temperature  characteristics, and cause them?  With this question in  mind, a local heater similar to that illustrated in Fig. 8 was  built.  Its tip diameter (defining its spatial resolution) was  large at 1000µm, but this still represented a relatively small  region of the IC.


Table 2:  Second Cycle Correlation List  Possible Prior Cause


(PPC) of Known Failing


Behavior (OnTransistor)


Predicted or Known


Correlating Side-Effect of Prior  Cause at Left


Reset forced to abnormal state  should produce global leakage


Incorrect reset signal state  during test setup causes  normally-off transistor to  be on


Reset forced to normal state


should eliminate global leakage  Electrical anomaly will appear in  fabricated IC


Observed global I(V) will occur at  a local region in the IC


Normal transistor  otherwise wrongly  activated


Observed global I(T) will occur


locally


Physical anomaly will appear in  fabricated IC


Abnormal transistor  created and active


Observed global I(T) will occur  locally


Measurement:  Using the topside airflow heater, a topside  temperature rise was impressed at various points across the  IC, and a very slight rise in IDD leakage as a function of the  heater position was observed.  Considerable effort was  required to separate the signal from the noise, and only a  few data points per day resulted.


Interpretation:  Although not all regions were examined  due to the laborious process involved, results obtained  suggested that approximately 90% of the IC area could be  ignored, and that the analysis could focus on a relatively  small region at the top of the die.  A plot of the signal as a  function of die location appears in Fig. 9.  The region at the  left of the figure is at the top of the die.  This interpretation  confirmed that the effect named in the Correlation List (Table 2), a localized IDD(T,x,y), did exist and correlated  with the global failure behavior.  Since no physical law  demanded that this thermal characteristic caused the  observed leakage, only the first two sub-questions could be  answered positively for this possible prior cause.


E/C/C Answer:  A local thermal effect exists, correlates  with the failure behavior, but does not cause it.


Since an effect (but not the prior cause itself) had been  localized, the next step was to revisit or reconstruct the  Correlation List.  To proceed effectively at this point, however, improved access to the cause-effect network  around the specific defect or anomaly was needed.  To gain  this access, material was built using a custom metal mask.  Failing wafers built with this mask routed their (anomalous) supply current through a middle metallization sandwich  layer.  A FIB cut then confirmed the thermal map's results.  A typical cycle through the metaprocess took shape as  described next.


Correlation List:  Localization can be executed without  much elaboration.  It should be understood and developed, however, as a series of loops through the Fig. 3  metaprocess.  To enable this, the Correlation List indicated  in Table 3 was constructed.  Localization then continued  based upon the Correlation List items identified.


Selection:  IDD current path in analog circuitry section.


E/C/C Question:  Does a current path in the analog circuitry  section exist, correlate with global failure characteristics, and cause them?


Table 3:  Second Cycle Correlation List, 1st Mod


Possible Prior Cause of


Known Failing Behavior


(On-Transistor)


Electrical anomaly will appear in  fabricated IC


Observed global I(V) will occur in  analog circuitry


Observed global I(V) will occur in  digital circuitry


Observed global I(V) will occur in  custom circuitry


Normal transistor otherwise wrongly activated


Observed global I(V) will occur in  standard cell circuitry


Observed global I(V) will occur at  the transistor


Observed global I(T) will occur at  the transistor


Figure 8:  Local topside airflow heater capable of producing approximately 10°C rise in die temperature  over a region of 1-2mm.


Figure 9:  ∆IDD (x,y) generated by local topside heating.


p-well


Figure 12:  Locations of three layout factors.


Measurement: All but the bottom (more resistive) refractory metal layer was removed mechanically (by probe  scrub) and measurements made for possible resulting  voltage drops.


Interpretation: Results exhibited no voltage drops along  any VDD metallization path to the analog circuitry.


Measurement: Focused Ion Beam (FIB) cuts isolated  current paths between the external VDD pin and analog  circuitry.  Global IDD was then re-measured.


Interpretation: External current exhibited original  characteristics as a function of voltage (anomalous current  was not eliminated by the FIB cut).


E/C/C Answer: A current path in the analog circuitry does  not exist.


At this point, current localization was pursued on multiple  devices by FIB and other means until it was traced, first to a  region of standard cells, then to a half-row within the  region, and finally to two similar standard cells in the row (Fig. 10).  This region was broadly consistent with the  thermal map in Fig. 9.  Correlation of the two cells to the  leakage was demonstrated by tying the local  implementation of the reset line of each cell to the lowcurrent state.  These FIB modifications produced  approximately a 50% reduction of the anomalous IDD  leakage for each cell.  To further localize the current path, the local reset within the cell was isolated before and after


an inverter, and the post-inverter signal was found to  correlate while the pre-inverter signal did not.


At this point the root anomaly was seen for the first time.  The mask-generated layout in the area related to the postinverter signal was inspected, and the structure depicted in  Fig. 11 was observed.  This figure has key structures  annotated with three vertical polysilicon paths traversing an  n+ guardring.  These structures are not intentional (designed) transistors.


This structure stood out because it appeared to provide an  unintended biased and transisting path from the p+ regions  through a channel across the n+ guardring, and across the  depletion region at the p-well boundary to the p-well region.  Three anomalous factors (Fig. 12) interacted to create this  path:


1. A mask generation algorithm created a very small  extension of the p+ regions to the vertical polyilicon  crossing the guardring (two instances, left and right);


2. An n+ guardring removed field oxide and created  conditions for channel formation;


3. An apparent reduction in well doping expanded the  depletion region to contact the channel area.


At this point the failure was, to a large degree, considered  localized.  Since localization held the analysis substantially  in place on the cause-effect network, however, it was  appropriate to recall the analysis status in terms of the  metaprocess loop.  This review made it clear that some  evidence now existed to address the E/C/C Question: "Does  an abnormal transistor exist, correlate with the known VDD  leakage, and cause it?"  That evidence suggested that such a  transistor did exist, did correlate with the known VDD  leakage, and did cause it.


Here another opportunity to apply methodical logic arose, representing the third function of the metaprocess described  earlier (providing application points for methodical analysis  logic).   Inductive Proof must be invoked to prove that a  possible prior cause is an actual cause.  When predicted  side effects are always found, the decision to declare the  PPC proven by induction rests entirely with the analyst.  There is no objective criterion for the number of validated  side-effect predictions.  For some on the team, the number


Figure 10:  Localization of leakage to two standard cells.


Figure 11:  Structure of interest in mask generation  layout of both leaky standard cells.


of validated predictions was simply not yet sufficient, and  so additional side effects were sought that would remove  any doubts about the anomaly's role.


Unfortunately, FIB access to further localize or exercise the  local circuitry was not possible.  The analysis therefore  again turned to the Correlation List (Table 4) to predict, select, and measure other secondary effects of the observed  set of adjacent anomalies.  The List made it clear that if a  transistor source, channel, and drain existed in the region of  the apparent anomalies, definite changes in the surface  doping at regions 1 and 3 should exist.


The construction of this region virtually guaranteed that  region 2 would exhibit characteristics of a doped channel, but it was apparent that much could be learned from  comparing the first and third regions with the channel.  (These statements all represent implications in support of  inductive proof.)  The Correlation List again led  immediately to the E/C/C Question, "Do the transistor  source, channel, and drain exist in the fabricated IC at the  region of the anomaly, do they correlate with the observed  failing behavior, and do they cause it?"  A measurement  was required to make these possible side effects visible.


Local high-resolution surface doping measurements of the  region with Scanning Capacitance Microscopy (SCM)(6,7) on an Atomic Force Microscope (AFM) would serve the  purpose. The SCM technique can provide very high spatial  resolution mapping of semiconductor surface doping.  This  information, combined with precise AFM topographic  measurements revealing field oxide extents, identified the  ends of the parasitic channel, other local doping variations, and also depletion region widths.


These results  (Measurement) are illustrated in Fig. 13, and  confirmed the availability of a current path through the  anomalies capable of producing the observed leakage  current (Interpretation).  The results satisfactorily  demonstrated the "abnormal transistor wrongly activated" in the modified Correlation List.  That is, they provided the  last positive indicators demanded by the analysts' application of inductive proof to show that "an abnormal  transistor structure at coordinates (x,y) exists, correlates


with the original VDD leakage, and causes it."  (Final E/C/C  Answer)


C.  Corrective Action and Graphical Summary


This analysis successfully identified the anomaly causing  the VDD leakage.  It remained to determine whether this  anomaly also explained other initial failure characteristics.


The low local power dissipation explained why no Liquid  Crystal signal was seen.  Photon emission was probably not  observed due to equipment sensitivity to the mechanism.  The high doping level of the old process explained why the  same design fabricated in that earlier process exhibited no  leakage.  This probably occurred because the higher doping  reduced the depletion region width (Fig. 13, Region 3) sufficiently to prevent contact between the depletion region  and the channel.


Finally, from Fig. 13 and the dependence on well doping, it  is clear that the anomalous positive leakage temperature  dependence is caused not through channel resistivity, but  rather through characteristics of the depletion regions  adjacent to the channel.  During leakage, the greatest  influence on current levels probably occurs in Region 1 of  Fig. 13, where doping concentrations evidenced by SCM  appear to be near intrinsic levels.  Thermally generated  carriers there will increase the carrier density in this region, lowering its resistivity and passing more current into the  channel.


Circuits modified to remove this structure exhibited no  anomalous VDD leakage, demonstrating that this analysis (summarized in Fig. 14) had identified the root anomaly.


Table 4:  Second Cycle Correlation List, 2nd Mod


Correlating Side-Effect of  Prior Cause at Left


Transistor source, channel and  drain occur in fabricated IC


Other components create  observed current threshold


Figure 13:  AFM surface (topographic) and SCM doping results (flat, doping shown through contrast) from  suspicious region.  Region 1: P+ region connects to  channel through region that is at least depleted, and  possibly inverted.  Region 2: Channel region clearly  reaches from the p-well at far right, extending leftward  past the edge of field oxide (top topography surface  edge delineated by vertical line extending to SCM data  surface) to connect to the Region 3 channel (doubleheaded arrow at right).


Figure 14: One-sheet full-analysis summary showing cause-effect relationships from root anomaly to failure mode, including intermediate cause-effect relationships and the analysis path that evaluated them.


Failure analysts who repeatedly find correct causes for  difficult failures come to be known as clever analysts.  While such reputations may be well deserved, cleverness of  this sort can and should be formalized and taught to those  not yet possessing such a reputation.  A well-constructed, careful analysis methodology provides a teachable  formulation for the 'cleverness factor' (which consists  chiefly, in the authors’ opinion, of discovering, understanding the nature of, and making use of the large  network of cause-effect relationships which can lead to the  failure's cause).  It also provides a foundation for rigorous  use of all available equipment during analysis.


The example explored in this paper also demonstrates the  fact that the analytical equipment set and manufacturing  process simplicity do not by themselves guarantee analysis  success.  In fact, both of these elements were present while  this problem went unsolved.


This analysis case study illustrates application of a  previously developed metaprocess (described earlier as a  general process which creates a specific process in real  time) for Failure Analysis.  In addition to providing a wellorganized, reliable approach to the analysis, this  metaprocess provided the following specific benefits at  various points:


• It prompted a wider characterization of the original


failure mode and identified the leakage's temperature


characteristic.  This characteristic provided the first


localizable failure signal;


• It immediately led to proper consideration and rapid


dismissal of a wide range of failure mechanisms


(including latchup and reverse-biased diode leakage.)


This saved considerable time and effort without


compromising breadth;


• It prompted the expansion of a list of secondary effects


created in the cause-effect chain, from root anomaly to


failure mode.  Each effect in this column of the


Correlation List represents another candidate


measurement which could help lead to the root anomaly;


• It provided a series of characteristics that the root


anomaly needed to match, including the involvement of


an anomalous transistor on-state and the requirement that


the anomaly must also include other electrical


components.  These characteristics provided positive


confirmation of the correct anomaly when it became


evident.  (The point of analysis, of course, is not to find


the defect, but to find the right defect among the many


spurious anomalies that any IC will contain.)


Thanks for technical assistance are due to many individuals  who assisted with this investigation.  In particular, we  would like to thank Dr. Mark Johnson for insightful  assistance with SCM execution and results interpretation.  Thanks are also due to Mr. Adam Ghozeil for constructive  discussions, exceedingly clear thinking and idea generation  at key points in the process, as well as development of the  special metal mask that proved very helpful in the analysis.


1. Ferrier, S.  "A Standardized Scientific Method  Approach for Failure Analysis Application," 2002  Proceedings of the International Symposium for  Testing and Failure Analysis, pp. 341-347.


2. Ferrier, Steve, "Trying to See in the Dark," Electronic  Device Failure Analysis News, May 2003, p. 25.


3. Gray, Paul R. and Robert G. Meyer, Analysis and Design of Analog Integrated Circuits, p. 64, eqn 1.175, John Wiley & Sons, New York, New York (1993).


4. Gray, Paul R. and Robert G. Meyer, Analysis and  Design of Analog Integrated Circuits, p. 64,eqn 1.174, John Wiley & Sons, New York, New York (1993).  Note that the temperature dependence appears through  k, which is directly proportional to the mobility µ.


5. Grove, A. S., Physics and Technology of Semiconductor Devices, pp. 110, 347, John Wiley & Sons, New  York, New York (1967).


6. Born, A., C. Hahn, M. Löhndorf, A. Wadas, Ch. Witt, R. Wiesendanger, "Application of Scanning Probe  Methods for Electronic and Magnetic Device Fabrication, Characterization and Testing", J. Vac. Sci. Technol. B, 14, 3625 (1966).


7. C. C. Williams, "Two-dimensional Dopant Profiling by  Scanning Capacitance Microscopy," Annu. Rev. Mater. Sci 29, 471 (1999).


p 177-183


DOI: 10.1361/cp2003istfa177


## SRAM Failure Analysis Strategy


SRAM Failure Analysis Strategy


P. Egger, C. Burmer


Infineon Technologies, Munich, Germany


The area of embedded SRAMs in advanced logic ICs is  increasing more and more. On the other hand smaller structure  sizes and an increasing number of metal layers make  conventional failure localization by using emission  microscopy or liquid crystal inefficient. In this paper a SRAM  failure analysis strategy will be presented independent on  layout and technology.


Due to the minimum structure sizes used in most cases for  SRAM cell design and the large density of critical layers in  SRAM cells, SRAM failure analysis plays an important role  for yield enhancement [1] and for investigation of reliability  problems.


The starting point of a typical failure analysis is global fault  localization by means of liquid crystal thermography, TIVA (thermal induced voltage alteration) or emission microscopy. However, on complex logic designs in the sub-quarter micron  regime fault localization is a real challenging task. Figure 1  shows a frontside emission microscopy image with an  emission spot on an SRAM area.


Figure 5 – Effect of cross talk between adjacent diodes  carrying shifted signals on LVP waveform acquisition. The  diodes dimensions marked with dotted squares (0.4x0.4 um  distanced by 0.2um). When we sweep the beam across the  diodes row we receive practical elimination of the signal in  the center diode.


The term cross talk is often used for this interference, however  the photon interference involved in optical probing is much  more complicated than in the typical electrical crosstalk case. The effects of optical cross talk becomes significant when  device geometry starts to be much smaller than the FWHM of  the probing beam or the acquisition region. Another condition  is that an interfering source must be contained in the  acquisition perimeter of the probing beam, with sufficient  active region. We must keep in mind that while the transistor  size is reduced to be well below the acquisition perimeter, the  diffraction limit does not allow us to distinguish between  sources contained in this perimeter. Therefore any signal  produced in this region will be probed as a single waveform. At the same time one should recall the limit stated previously  with regard to the minimum acquisition size. Eventually, even  if the acquisition perimeter contains several elements their  individual signal is not measurable; therefore the interference (without going into special cumulative cases) is also  immeasurable. As a result the two aspects of shrinkage are  correlated strongly. The LVP signals may also cancel each  other as in the case of n and p active regions that generate  complementary modulations. Figure 4 demonstrates the  interference effects between 3 neighboring 0.4x0.4 um n-type  diodes spaced 0.2um apart from each other. A waveform of  250 ppm was acquired at the extreme diodes; however as we  approach the center structure the signal intensity reduces, the  reason for this attenuation is not clear.


As for TRLEM the emitter scaling strongly affects the  detection capability (even more strongly than for the LVP), and therefore the acquisition perimeter can contain at most 2-3  efficient emitters. Although cancellation of two  complementary signals is not possible since we probe only  transitions, one cannot t always rely on the temporal resolution  of the system due to the following concerns:


1. The two signals may have consecutive timing that  can smear the transition peak.


2. Even if the two events are resolvable the correlation  between the event and the transistor may be doubtful.


3. Sub-threshold leakage and gate leakage becomes  significant in these processes and additional  background may corrupt the measurement.


Figure 6 – Simple example of macro optimized for TRLEM  probing enabling measurements of rise and fall edges events


(a) show the SPICE modeling of the circuit in (b). Notice that  the circuit is optimized in terms of space load delay and  switching currents. The inverters should be spaced at least 1  um from each other with sufficient keep out zone around. The  space required for the implementation of such macro may be  large (~4 um2).


Design for debug


The analysis and discussion in the previous sections clearly  indicate the difficulty of debugging 90nm gates in terms of  acquisition time and interference. In this section we intend to  discuss some solutions to overcome this difficulty. The need  for shorter debug cycle is now critical for faster time to market  of new products. Therefore the times in which design and  failure analysis were two separate links in the VLSI  development flow are over. DFD was already implemented in  the past for LVP in the form of probe diodes. However, the  guideline was usually implemented during the physical design  process only with strict limitations on cost in terms of device  performance and area. In other words designers allowed the  placement of diodes for probing, as long as these were placed  in empty silicon areas and the signals’ capacitance was not  altered significantly. In some cases designers were reluctant to  allow any modifications on their final design and their design  was left with very limited debug capability.


Out1


Out2


Figure 7 – Simplified schematic of flip-flop(FF) cell for  demonstration of DFD incorporated into one of the basic  library cells. The inverters marked by the square are critical  to localize any failure that originates or propagates through  this cell. The marked inverters require minimum widths for  good measurement, and should also be distinct from other  regions. The inverters marked by i and cl are not an inherent  part of the FF structure, however they are necessary for  debug. The data in the buffer could be probed in previous  stages and the clock buffer could be common for several cells.


Design for testability is an example of how debug capability  was incorporated into the design despite the cost of 10-15% in  die area (9). Scanable cells are now replacing most of the  regular design to increase test coverage. In some cases, test  coverage is a compromise between device performance  delivered to the customer and robust testability. This  compromise is acceptable due to the appreciation that failure  analysis could compensate for the insufficient coverage and  for bugs in the scan chain itself. The recognition that failure  analysis is critical in the device release process and even more  for customer returns is not questionable, therefore the only  question is the cost.


As mentioned earlier the LVP probe diodes are the simplest  and least costly DFD solution. The cost of diodes  implementation  may be small, if diodes are implemented into  the library cells design. The designer is usually required to  decide which node is critical for probing and attach a diode to  this node. This diode structure is translated into a special  probing diode with minimum size to allow fast acquisition and  clear area around it in physical design. This flow is fairly  mature and proven for 0.13um and up processes with no  significant need to stretch the probing diode much above the  minimum sizes allowed by the design rules for the  width of  the active area and the clear distance around the diode. In


0.09um however the diode must exceed considerably from the  minimum diffusion area. Design rules allow small diodes such  as 0.15x0.15um or even smaller. Probing such diodes was not  yet successful without even considering the fact that such  feature size could not be resolved (or even observed) from the  backside. Therefore it is expected that probe diodes in the


0.09um process will have more significant cost in die area


TRLEM probing poses a difficult challenge for DFD. As  could be seen in figure 6, designing a special probing structure   will require at least 4um^2 of area in order to obtain  acceptable coverage for rise and fall time of this signal. Implementation of such wasteful solution will inflate the  design unjustifiably. A more acceptable solution is to  implement lower width limit on critical nodes. Once again the  decision on which node is considered critical is done in the  early stages of design, and circuit designer must implement  this width limitation to the library cells of the new process. The implementation is especially costly for flip-flop (FF) design, these cells capture about 25-40% of the logic area. General limitation of the minimum gate size in the FF will add  normally approximately 10-20% additionnal  area to the cell. If we prudently consider the important signals in the cell we  can reduce the deviation to less than 5%. An example for  design for debug consideration is shown in figure 7. The  number of special debug buffers are limited to the minimum  necessary to localize the failure.


The development of new FA tools and methodologies  frequently lags behind the rapid advancement in the field of IC  process technologies. If only present tools are to be used for  future process technologies, critical designs may be left  without reliable post silicon debug tools.


We presented the risks of not incorporating DFD in future  processes, and the acceptable solutions that will have a minor  impact on die size


The decision of how much die area to spend on DFD must be  based on economics factors but this decision is difficult to  take. DFD costs are fairly straightforward to measure (die  area, performance and effort) but in contrast most of the  benefits are difficult to quantify, especially at the time the  decision is made.


At present it appears that the improvement in tools acquisition  efficiency is much slower in comparison to the reduction in  the signal magnitude. As a result the acquisition time is  increased considerably. Using the present analytical tools, signal measurement capability will inevitably reach its limit in  the next generation process (65nm). The solutions suggested  here are conservative, and require simply that the acquisition  region be kept large enough for measurement. In order to  maintain the rule that no more than 10%-15% increase of die  area is required, debug features must evolve, for example, to  encompass more efficient emitters or to analytical systems of  different scope


1. Livenghood R. H. and Medeiros D., Design for


(physical) debug for silicon microsurgery and


probing of flip-chip packaged integrated circuits, Test  Conference, 1999. Proceedings. International , 1999


cl i


2. Paniccia, M.; Eiles, T.; Rao, V.R.M.; Wai Mun Yee, Novel optical probing technique for flip chip


packaged microprocessors, Test Conference, 1998.


Proceedings. International , 18-23 Oct 1998


3. Vickers J., Pakdaman N., and Kasapi S., Prospects of  Time-Resolved Photon Emission as a Debug Tool,


Proceedings of the 28th ISTFA 2002


4. Tsang, J.C.; Kash, J.A.; Temporal characterization of  CMOS circuits by time resolved emission


microscopy, Device Research Conference Digest,


1997. 55th , 23-25 Jun 1997 Page(s): 24 –25


5. R. A. Falk, Optimizing Backside Image Quality,


6. T. M. Eiles, Liquid immersion objective for high


resolution optical probing of advanced


microprocessors, Proceedings of the 27th ISTFA


2001


7. Lo W., Kasapi S. and Wilsher K., Comparison of


Laser and Emission based optical probe techniques, Proceedings of the 27th ISTFA 2001


8. Tsang, J.C.; Fischetti, M.V., Why hot carrier


emission based timing probes will work for 50 nm, 1  V CMOS technologies, Microelectronics Reliability


vol.41, no.9-10 p.1465-70 Sept.-Oct. 2001


9. S. Rusu, S. Seidel, G. Woods, D. Grannes, H.


Muljuno, J. Rowlette, and K. Petrosky, IEEE


International Solid-State Circuits Conference, 2001,


p. 276.


10. Carbine, A.; Feltham, D.; Pentium Pro processor


design for test and debug


Design & Test of Computers, IEEE , Volume: 15


Issue: 3 , July-Sept. 1998


Page(s): 77 –82


11. W. Lo, K. Wilsher, R. Malinsky, N. Boiadjieva, C.


Tsao, M. Leibowitz, H. Deslandes,  Next-Generation  Optical Probing Tools for Design Debug of High


Speed Integrated Circuits, Proceedings of the 28th


ISTFA 2002


p 191-196


DOI: 10.1361/cp2003istfa191


## Identification of an IDDQ Failure Mechanism Using a Variety of Front and Backside Analytical Techniques


Identification of an IDDQ Failure Mechanism Using a Variety of Front and Backside  Analytical Techniques


Jim Shearer, Kim Le, Xiaoyu Yang, Monty Cleeves, Al Meeks


Matrix Semiconductor, Santa Clara, CA, USA


This is a case study using a variety of failure analysis  techniques to solve an IDDQ problem.  This product is  fabricated using a 3-metal-layer 0.25 µm CMOS process with  the addition of Matrix’s proprietary 3-D memory layers. [1]  During the technology transfer from Foundry A to Foundry B, one challenge that presented itself during the development of  the product was high standby current, IDDQ.   IDDQ ranged from  about 1.5 mA to over 25 mA and was well over the design  target.  The IDDQ problem was early on traced to the CMOS  layers below the 3-D memory.


Various analytical techniques were used to isolate the source  of IDDQ leakage on our product.  The failure analysis used both  top and backside analytical techniques, including: liquid  crystal, PEM (photon emission microscopy) from both front  and back, dual-beam FIB (focused ion beam) cross-sectioning, FE-SEM (field emission scanning electron microscopy) imaging, PVC (passive voltage contrast), microprobing of  parallel-lapped samples, and SCM (scanning capacitance  microscopy), and FE-SEM.  Many of these methods have been  used jointly in previous papers. [2]  This paper discusses how  the application of each of the techniques narrowed down the  search for this IDDQ leakage path.


Liquid Crystal Analysis


Liquid crystal analysis was performed on both packaged and  wafer-level dice to identify the IDDQ current path.  VDD was  pulsed on and off using the step generator output of a curve  tracer. The liquid crystal analysis identified large spots in  repeating CMOS circuits throughout the die.  Unfortunately, the liquid crystal analysis lacked the spatial resolution to  pinpoint the source of the leakage.


Emission Microscopy Analysis


Both topdown and backside emission microscopy using  emission microscopes employing CCD-detectors was also  performed, but was not effective.  However, backside  emission microscopy using an emission microscope equipped  with a Mercad (HgCdTe) detector [3] provided transistor-level  identification of many of the emission sites as shown in Fig. 1.   The emission sites appeared to be near the p+ source/drain


contacts of a PMOS transistor in a particular circuit.  It was  extremely interesting that, although many such identical  circuits existed on the chip, the only ones exhibiting the  emission sites happened to be in close proximity to a large  poly-plate capacitor.


Figure 1: Photon emission sites observed during backside  emission microscopy using a Mercad detector.  The emission  sites occur in identical repeating structures near the large  decoupling capacitor (inside black rectangles), but none  appear in the same structures away from the capacitor (arrows).


Dual Beam (FIB/SEM) Cross-sections


In a dual beam FIB/SEM successive precision FIB crosssectional cuts may be performed on a chip while being  monitored using a FE-SEM.  Dual beam cross-section slices  were performed on multiple emission sites – covering both the  x-direction and y-direction.  No physical defects were found.


Parallel-lap / Passive Voltage Contrast


The layout of an area of interest in the IC including where  emission sites were observed is shown in Figure 2.  To further  study the areas of photon emission near the p+ source/drain  contacts (area “A” in Fig. 2), a sample was parallel-lapped  down to the contact layer just above the poly, as shown in  cross-section in Fig. 3, and passive voltage contrast was  performed using a FE-SEM.  In this technique, the bottom of  the die is grounded via the SEM stub and the chip is “biased” using the scanning electron beam at a low accelerating voltage (typically 1 kV). The sample surface being scanned by the  electron beam becomes charged positively at low primary  electron voltages. Differences in secondary electron image  contrast observed on conductors typically indicate differences  in conductivity to the substrate.  A striking difference was  observed between the source/drain contacts of suspect PMOS  transistors (situated near the large poly capacitors) and  identical “good” PMOS transistors (away from the large poly  capacitors). This is shown in Figs. 4 and 5. The relative  brightness of the source/drain contacts of the PMOS  transistors located near the poly capacitor indicated that they  were not charged positively and that a leakage path to the pdoped substrate existed.


Figure 2: Layout of the circuit identified by the PEM work.  The squares with the x’s are contacts.  The black rectangles  indicate the FIB probe pad placement on the parallel-lapped  samples.  The “A” node connects the PMOS transistors  source/drain contacts (gate floating).  “B” is the p+ substrate  tap.  “C” is the nwell tap.  The vertical line labeled D - D  identifies the location of the dual beam cross-section shown   in Fig. 3.  The star identifies the emission site.


Figure 3: Dual beam (FIB/SEM) cross-section of the p+ island through the source/drain contacts.  The silicon has  been decorated.  The line indicates the parallel-lap target  used for the passive voltage contrast and microprobe sample.


The source/drain contacts of the PMOS transistors away from  the poly capacitor (and which also had not produced emission  sites during the PEM work) appeared dark, indicating a much  lower leakage to substrate.  Poly gate contacts at both sites  appeared dark, indicating negligible gate oxide leakages.


Microprobing of Parallel-Lapped Samples


Having identified a likely leakage path from the PMOS  contacts to the substrate, probe pads were attached to various  nodes in the circuit to facilitate microprobing.  Microprobe  pads were attached to the source/drain contacts of the suspect  PMOS transistors, the p+ substrate tap contacts, and the nwell  tap contacts as shown in Fig. 2.  The pads were probed using  needles with 0.1 µm tips as shown in Fig. 6.


The circuit was biased with the nwell tap at 3.6 V, the p+ substrate tap at ground, and the source/drain contacts swept  from 0 to 3.6 V.   This represents the bias conditions this  structure would see during IDDQ testing.  The results of  electrical testing are shown in Fig. 7.  Source/drain leakages to  substrate were greater than 10 µA on a typical failing location.  Leakages less than 10 pA were observed on good sites.  Microprobes performed on a wafer that had been processed up  to the contact step revealed that the anomalous leakage paths  were present initially and not induced by subsequent fab  process steps.


Scanning Capacitance Atomic Force Microscopy (SCM)


Two dice were mechanically cross-sectioned through the  PMOS island along a row of source/drain contacts.  One was  cross-sectioned through a structure near the poly capacitor.


Figure 4: Passive voltage contrast image of an emission site.  The PMOS source/drain contacts (identified with the white  rectangle) appear bright, indicating a leakage path to the pdoped substrate.  The relative location of the poly capacitor is  also indicated.


Figure 5: Passive voltage contrast image of a “good” structure away from the poly capacitor.   The PMOS  source/drain contacts (identified with the white rectangle) appear dark, indicating negligable leakage to the p-doped  substrate.


The other was cross-sectioned through a structure away from  the capacitor.  Atomic force microscopy, using a capacitance  probe tip, was performed along the cross-section surface. [4]  Figure 8 shows the expected doping profile.  On a good  PMOS structure, the nwell provides sufficient isolation  between the p+ source/drain diffusion and the p-doped  substrate below as illustrated in Fig. 9.  On a leaky PMOS  structure, the p+ source/drain diffusion was not completely  enclosed within the nwell and connected to the p-doped  substrate, creating a short as shown in Fig. 10.


Figure 6: Microprobing a parallel-lapped sample with FIBapplied probe pads.  The tiny rectangular structures are the  probe pads.  The long yellow-green structure near the left side  of the image is the poly capacitor.


SEM Inspection of Nwell Mask Resist Profile


An examination of the layout shows identical nwell overlap of  the island on structures near and away from the capacitor.  It  appeared that the problem was related to photolithography.


SEM analysis of a wafer pulled from the line after the  application of the nwell resist mask revealed that the resist  appears closer to the isolation island on structures that are  closer to the poly capacitor.  Closer examination on the SEM  revealed that the PMOS islands near the capacitor have a near  vertical resist profile (~0.1 µm), but PMOS islands away from  the capacitor have a shallow slope (~ 1.1 µm).  Refer to  Figures 11 and 12.  At the energies used for the ion implant, the thin resist near the base of the sidewall won’t stop the ntype ions.  Thus, the effective nwell boundary is further from  the island on “good” PMOS structures than on “bad” structures.  The root cause of this IDDQ failure mechanism was  an insufficient nwell isolation width around the PMOS islands.  The differences in nwell isolation between good and bad  PMOS structures was caused by differences in the photoresist


Figure 7: IV curves obtained from a failing die at bad and good PMOS transistor sites.  The chart shows source/drain  current as a  function of applied voltage.  The bad sites exhbited leakages that were 6 orders of magnitude greater than the good sites.


Figure 8: Expected doping profile for the PMOS island.  The


nwell doping completely surrounds the island providing


isolation between the p+ source/drain region and the


substrate.


slope, which in turn was affected by the placement of nearby  structures.


Further SEM examination of test structures revealed that the  resist slope was shallower for wide resist lines and steeper for  narrow resist lines as shown in Fig. 13.


The narrow resist lines correlate to the narrow nwell mask  photoresist pattern that exists between nwell boundaries  surrounding the poly capacitor and nearby PMOS islands.  For  PMOS islands away from the poly capacitor, the nwell  photoresist pattern is wide, correlating to the wide resist line  on the test structure.  This explains why the nwell photoresist  slope around PMOS structures near the poly capacitor was  steeper than the nwell photoresist slope around PMOS  structures away from the poly capacitor.


Corrective Actions


This leakage path was eliminated using the following two  corrective actions:  1)  The resist is now pre-treated prior to  ion implantation to produce a consistent resist sidewall profile.  2) The Nwell boundaries were adjusted in the next Nwell  mask revision.


Figure 9:  SCM image of a good PMOS structure.  A clear  gap exists between the p+ source/drain diffusion and the p  substrate.


Figure 10:  SCM image of a leaky PMOS structure.  The p+ source/drain diffusion clearly bridges to the p substrate.


Figure 11: SEM image of the photoresist pattern near a p+ island adjacent to a poly capacitor area.  The two-headed  arrow shows the spacing between the base of the resist and the  edge of the p+ island.  The sidewall of the resist has a steep  appearance.


Figure 12:  SEM image of the photoresist pattern near a p+ island away from the poly capacitor area.  The longer twoheaded arrow shows the spacing between the base of the resist  and the edge of the p+ island    The sidewall of the resist has a  shallow appearance.  The high energy n-type ion implant is  able to penetrate the thin resist near the base, causing the  effective spacing to be even greater.  The shorter arrow shows  the additional distance to the “effective” resist edge.


Figure 13:  SEM image of the photoresist pattern near thin  and thick resist lines (e-test structure).  The sidewall slope is  shallow on wide resist patterns and steep on narrow resist  patterns.


Conclusions and Summary


The use of a number of failure analysis techniques was  employed to identify the root cause of a major IDDQ leakage  failure mechanism in our first product.  The paper describes  the techniques and how they contributed to a final solution.


Additionally, it has been shown that something as subtle as a  change in photoresist slope can have a profound impact on  device electrical parameters such as IDDQ.


A significant observation is that different foundries have  different fabrication processes and these may cause different  photoresist profiles.  A change between foundries may  necessitate the use of different design rules.


The work presented in this paper represents the teamwork of  many people, who we are extremely privelidged to work with.  First, and foremost to be acknowledged are the individuals  within the design, process, product, and test engineering  groups, assigned to tackle this problem, including (but not  limited to)  Mark Johnson, Alper Ilkbahar, Bendik Kleveland, Matt Crowley, Kedar Patel, Johan Knall, Bill Orso, Chris  Petti, and the process engineers at our foundry.  We are  extremely grateful to our mentors, Richard Anderson and  Rosalinda Ring for their careful review of this paper and  valuable inputs.  In addition to the above individuals, we  would like to thank Melissa Selcher, Mike Vyvoda, Dan  Steere, and Liza Toth for reviewing the paper in various stages  of development.  Regarding the specific failure analysis  activities, we would like to acknowledge and thank the  following persons:  Joe Greger of Hypervision, the late Robert  Ling of AMER for his expert parallel-lapping, Tina Hsu for  her precision cross-sections, Xiuhong Han of Accurel for the  dual beam cross-sectioning, Fang Wu of Accurel for the FIB


application of probe pads, and Gordon Chao of Charles Evans  Associates for the AFM/SCM work.


1. M. Crowley et. al., “512Mb PROM with 8 layers of


Antifuse/Diode cells,” ISSCC 2003 Proceedings, p. 284.


2. J. Colvin, A. Roy, "Identification and Analysis of Parasitic  Depletion Mode Leakage in a Memory Select Transistor,"


ISTFA 2000 Proceedings, p. 247.


3. B. Davis, “A Comparison of Backside Emission


Microscopy Systems,” ISTFA 2000 Proceedings, p. 173.


4.  K. Jarausch, J. F. Richards, L. Denney, A. Guichard, P. E  Russell, “Site Specific 2-D Implant Profiling Using FIB


Assisted SCM,” ISTFA 2002 Proceedings, p. 467.


p 197-204


DOI: 10.1361/cp2003istfa197


## Novel Application of Transmission Electron Microscopy and Scanning Capacitance Microscopy for Defect Root Cause Identification and Yield Enhancement


Novel Application of Transmission Electron Microscopy and    Scanning Capacitance Microscopy for Defect Root Cause


Identification and Yield Enhancement


P. Tangyunyong, T. A. Hill, C. Y. Nakakura, J. M. Soden, E.  I. Cole Jr., R. S. Flores, M. R. Shaneyfelt,  R. C. Dockerty, T. J. Headley, and M. J. Rye


Microelectronics Development Laboratory, Sandia National Laboratories, Albuquerque, NM, USA


Transmission electron microscopy (TEM) [1] and scanning  capacitance microscopy (SCM) [2] have become common  failure analysis tools at Sandia for new product development, process validation, and yield enhancement.  These two  techniques provide information that cannot be obtained with  other analytical techniques.  The information provided by  these two techniques has been instrumental in identifying the  root causes of several yield-limiting defects in CMOS IC  technologies at Sandia.  This paper describes an example of  how TEM and SCM have been used to identify the root causes  of SOI device failures. The corrective actions taken to reduce  defects and improve yield are also described.


Recently, the yield of a 64K SRAM lot manufactured in  Sandia’s 0.35 µm, partially-depleted SOI technology was low. Electrical testing indicated that the quiescent power supply  current (IDDQ) of these devices was within the nominal limit. Most of the yield loss in this lot was due to functional failures  that exhibited several interesting characteristics:


1)   A strong voltage dependency with more failed bits being  observed at higher VDD.


2)   A small density of the failed bits within a given die, typically one or two bits in a 64K SRAM array.


3)   A layout dependency with one version of the SRAM  being less susceptible to failure than the other two  versions.


4)   A pattern dependency with bits from dies within the same  wafer failing the same way – stuck high or stuck low.


5)   A read-disturb bit flip behavior. For example, during the  write cycle, a “1” is correctly written to the memory, but  during the read cycle, the “1” stored previously will flip  to a  “0.”


The failed bit locations of several of these SRAMs were first  identified with electrical testing.  Before deprocessing, these  SRAM devices were analyzed using various failure analysis  techniques such as optical inspection, inspection with  scanning electron microscopy (SEM), light emission  microscopy, thermally-induced voltage alteration (TIVA) [3], light-induced voltage alteration (LIVA) [4], and soft defect  localization (SDL)  [5].    However, none  of  these  techniques


provided any conclusive information about exact defect  locations within the failed SRAM cells.


Several of the failed SRAMs were subsequently deprocessed  by immersing them in a 50% hydrofluoric acid (HF) solution  for several seconds to remove the metal interconnects,  interlevel dielectric (ILD) layers, and polysilicon layers and to  expose the silicon islands.   Following the HF dip, the samples  were thoroughly rinsed with de-ionized water and dried with  nitrogen.  Although the metal lines, contacts, vias, and  dielectric layers are removed during the HF dip, the  polysilicon lines remain intact.  The polysilicon lines were  subsequently removed using adhesive tape.  Finally, the  samples were rinsed and ultrasonically cleaned in isopropyl  alcohol.  A typical SEM image of exposed donut-shaped  NMOS islands is shown in Fig. 1.


1. L. Giannuzzi et al., Mat. Res. Soc. Symp. Proc. Vol. 480, (1997), 19.


p 209-214


DOI: 10.1361/cp2003istfa209


## Microhardness Testing on Via Fill Material for Via In Pad Technology


Microhardness Testing on Via Fill Material for Via In Pad Technology


Norman J. Armendariz


Carolyn McCormick


Intel Corporation, Chandler, AZ, USA


Via in pad PCB (Printed Circuit board) technology for passive  components such as chip capacitors and resistors, provides the  potential for improved signal routing density and reduced PCB  area. Because of these improvements there is the potential for  PCB cost reduction as well as gains in electrical performance  through reduced impedance and inductance.  However, not  long after the implementation, double digit unit failures for  solder joint electrical opens due to 0603 capacitor “tombstoning” began to occur.  Failure modes included via fill  material (solder mask) protrusion from the via as well as “out


gassing” and related “tombstoning,”


This failure analysis involved investigating a strong  dependence on PCB supplier and, less obviously, manufacturing site. Other factors evaluated included via fill  material, drill size, via fill thermal history and via fill amount  or fill percent. The factor most implicated was incomplete  cure of the via fill material.  Previous thermal gravimetric  analysis methods to determine level of polymerization or cure  did not provide an ability to measure and demonstrate via fill  cure level in small selected areas or its link to the failures.  As  a result, there was a metrology approach developed to  establish this link and root-cause the failures in the field, which was based on microhardness techniques and noncontact via fill measuring metrologies.


Via in Pad (VIP) Technology


Via in Pad technology for advanced PCB applications has  many attractive features such as:


• Increased routing area and reduces layer count


• Better electrical performance


• Improved heat transfer


• Low inductance path for capacitors


• EMI (Electro-Magnetic Interference) reduction (if used  with planes on the outer layers)


This makes it a extremely desirable as a board technology, especially if it could be implemented in a cost effective  manner at PCB suppliers, Figure 1.


Figure 1:  The  VIP P land structure incorporates the via into  the land pad significantly reducing the device foot print  leaving more room for routing and/or closer spacing as  compared to standard land pattern.


The PCB process flow relative to VIP includes applying the  via fill material to the PCB using a stencil printing process. The plugging material is then cured (hardened) by placing the  PCB’s on racks in an oven.  The potential for incomplete


curing exists at several points during these steps.


Figure 2: shows the basic VIP process from PCB supplier  fabrication process to SMT assembly.


Passive Via In Pad (VIP  P) Standard Passive Device


Land/Via structure


VIP P Failure Modes


Each of the PCB failure defects as they were received from the  assembly sites or from development activities were  photographed and/or x-rayed and documented in terms of their  process history before performing any destructive analyses.  In  addition selected, “as-received” PCBs, failed and non-failed  PBAs (Printed Circuit Board Assemblies), components and  via fill materials were retained and archived for comparative  or baseline analysis as needed.


The resulting predominant failure modes associated with PCB  VIP P components after surface mount technology (SMT) assembly reflow are illustrated and described in the following  Figures 3 through 7:


Tombstone


Figure 3: Top view of a ceramic capacitor in an upright or “tombstoned” condition (L) with via fill material protruding  from the adjacent via in pad and x-sectional view  (R).


Solder Drip


Figure 4: Top view of a VIP exhibiting ”solder drips” on the  PCB’s secondary side (L) and x-sectional view (R).


Overfill


Figure 5:  Top view of a “shifted”  ceramic capacitor on a  VIP exhibiting ”soldemask overfill” of the VIP (L) and a xsectional view (R).


Blowhole


Figure 6: shows a top view of a ceramic capacitor on a VIP  exhibiting out-gassing or “blowhole” of a VIP (L) and a xsectional view (R).


Insufficient Solder


Figure 7: Top view of a resistor on a VIP exhibiting ”insufficient solder” of a VIP (L) and a x-sectional view  showing solder entrained  (R). In some cases, the components  were completely missing.


VIP Supplier DOE Analysis


The appearance of via fill material (solder mask) protrusion  from the surface of the PCB was the most obvious failure  signature associated with tombstoned capacitor failure modes, Figure 8.


Figure 8: VIP P via plug fill material protrusion from the  surface of the PCB after reflow.


Capacitor tombstoning excursions occurred in all 3  manufacturing sites usually resulting in line yield losses of up  to 5 or 6%. Figures 9 and 10 demonstrates that these  excursions were highly PCB supplier dependent.  Various


PCB suppliers (S1-S5) were evaluted for their respective unit  fail percent with respect to VIP-P.  Two suppliers had the bulk  of the issues.


Figure 9:  shows the PCB supplier dependence of tombstoned  capacitors.


Figure 10: shows the correlation between via fill percentage  and tombstoning frequency variability between suppliers.


Capacitor tombstoning was hypothesized to be the result of  one or more factors including reflow profile, outgassing  of fill  material, outgassing of air in the via, outgassing of via  contaminants, outgassing of  solder paste flux, via plug fill  percentage and via barrel finish hole size (FHS).


Design of experiments (DOE) were performed with certain  key variables, such as reflow profile, via fill material (varying  solid contents), drill size and  PCB thermal history.  The key  data proving fill percentage was linked to high SMT yield loss  was the microhardness test.


Microhardness Testing


Microhardness measures a materials resistance relative to  another significantly harder material or indentor with a given  geometry by applying a load for a given amount of time, then  measuring the area of the indentation created.  The surface


area of the indentation is found from its diagonal length, which the user measures through the microscope on the  microhardness tool.  A Vickers hardness indentor with a  square-based pyramidal diamond geometry, which has a face  angle of 136° was the standard selected. The following  equation is used to calculated the Vickers hardness value:


Where:   HV = Vickers hardness


F = Test load (N)


S = Surface area of an indentation (mm2)


d = Average diagonal length of  indentation (mm)


θ = Face angle of the pyramidal  indenter (°)


Failure Mechanism


The via fill material starts as a mixture of long chain  monomers and solvent combination that allows it to flow into  the vias during fabrication of the PCB. When heat is added to  accelerate the process, the solvent volatilizes and outgases as  the monomer chains cross-link or polymerize. This should  occur during the cure step in the board processing, but the  solvent can leave during any step where heat is applied to the  board.


The hardness is a measurement of the cohesive mechanical  modulus strength of the material, which is related to the bonds  within the material.  Therefore, the hardness should be able to  quantify the degree of polymer chain cross-linking, which is a  measure of the degree of cure.


The components on VIP areas of interest were first  photographed and then cross-sectioned through the center of  the via and polished to a typical metallographic sample finish.  Microhardness measurements were then performed on the  soldermask material inside the via at five equidistant points  along the via length regardless of the via fill percent. The  position within the via was recorded for each hardness  measurement location. The amount of soldermask or via fill  was measured from the bottom of the copper trace on the  secondary side (zero point) up to the bottom of the meniscus  formed by the soldermask on the opposite side, Figure 11.


Figure 11: X-sectional view of a VIP structure on its side  showing the major features and the microhardness indentation   locations  within the via filling material (soldermask).


Taking the hardness at various plug locations within the vias  provided cure information at specific locations not previously  possible with thermal analysis methods.  The resulting  hardness measured was confirmed to be lowest (less-cured) in  the center.  More importantly, the hardness was even lower in


vias with greater fill percent.


Figure 12: X-sectional views of two vias  filled to 35 and 82%  and their corresponding microhardness vs. via fill percent  profiles taken at five locations shown.  The via fil  material  appears softer, i.e., less-cured, ,in the center region for both, and significanlty lower for the  82%r filled sample.


Data was obtained for each PCB supplier which exhibited the  failure modes, as well as, defect free assemblies.  The resultant  microhardness data set also showed a strong dependence on  via fill percent, Figure 12.  The various failure modes or  defects occurred based on the amount of via fill percent.  For  example, the tombstoned capacitors occurred in vias with high  via fill (low hardness/cure) and conversely, insufficients  and/or missing components occurred at low via fill percent


(high hardness/cure).   Thus, each of the major failure modes  could be explained and characterized by the via fill hardness  and via fill percent.


Figure 13: shows the center hardness vs. the via fill% for via  material Type A and the critical fill percentage required to  prevent excursions in SMT. This became the CTF parameter.


The DOE’s helped discover that the tombstoning root cause  was uncured via fill material with low via fill hardness clearly  linked  to the high excursion rate. This key result is clearly  shown in Figure 13. This was brought on by overfilling the  vias with the plugging material.  From this it became clear that  failure mechanism was uncured via fill material out-gassing in  reflow, causing fracture of the via plug in the center and  subsequent projection out of the via hole, Figure 14. Reflow  peak temperature and drill size effects were considered minor  influences, but the thermal processing itself was fundamental  to the failure mechanism.


Figure 14: VIP P failure mechanism involves heating the  uncured via fill material as the PCB traverses reflow.  The via  plug outgases, fractures, separates and is projected out of the  hole.


Although the via fill percent can be used as a controlling


parameter, it needs to be characterized for each material type, since, different via materials have different cure sensitivities. >80% fill  leads


to Excursions


<80% fill Prevents  Excursions


Critical


hardness


PC401


Via Fill %


Before Assembly


After Assembly


By Tombstones


Void


Many Voids


Almost Blowhole


Blowhole F/A


Tombstone F/A


Drips F/A


Missing F/A in Baseline  Insufficient F/A


401


Missing F/A in Baseline Insufficient F/A


ill  l


r i


ill


riti l


EFFECT OF VIA FILL MATERIAL TYPE


10 20 30 40 50


VIA FILL %


Figure 15: shows that via fill% and center hardness (cure) also depends on the via material used (Types A, B and C).


Nondestructive Via Fill Measurement


An automated OCMM (optical coordinate measurement  machine) method using a Mitutoyo QVH 606 was developed  in order to provide more detailed information regarding the  amount of via fill in PCB vias and in a non-intrusive manner  without having to perform tedious x-section measurements for  VIP P PCB process development.


The OCCM measures each individual via’s depth from the  surface of the PCB to the top (meniscus) of the via fill  material.  The via fill is then the difference PCB thickness and  the via depth measured, Figure 16.


Figure 16: X-sectional view of a PCB VIP structure and the  1200 VIP features the OCCM measured.  The via fill  distribution in this particular PCB ranged from 60 to 100 %.


The capability of the tool to measure the via fill was  determined by performing an MCA (measurement capability  analysis) on a single desktop PCB with thirty-five (35) vias  known to vary in depth from 0.002 to 0.042 inches with each  via repeatedly measured nineteen (19) times, Figure 15.


Figure 17: shows the MCA results “Depth into Via” vs. the  corresponding “Via Fill Percent.” The measured values begin  to lose accuracy below approximately 30 % via fill or about


0.040” into the via from the surface of the 0.062” thick PCB.


The capability of the tool to measure the via fill was  determined by performing an MCA (measurement capability  analysis) on a single desktop PCB with thirty-five (35) vias  known to vary in depth from 0.002 to 0.042 inches with each  via repeatedly measured nineteen (19) times, Figure 17.


Microhardness testing proved to be key to confirm the failure  mechanism and OCCM via fill measurements demonstrated  the actual via fill capability of the PCB suppliers.  However, both are rather painstaking metrologies suited more for  materials development and failure analysis that do not readily  lend themselves to high volume PCB supplier process control  with out significant investment.  A simpler method of


controlling the via plug cure was required.


Since, the critical to function parameter was via fill  percentage,  it seemed natural to use it as a method of  controlling via plug cure at the PCB supplier.  The final  metrology downselected for process control was x-section fill  percentage because it was readily available at the PCB  suppliers and it had good metrology capability and  microhardness and/or non contact measurements could still be  performed off-line, if and when required.


Applying the microhardness metrology for failure analysis  resulted in identifying via fill cure and controlling via filling  percent as the critical-to-function (CTF) parameter, which is  also based on the via material type.


The observation was that failed assemblies had softer via plug  material at the center, which directly correlated to the via plug  fill %.  With this data available, the root cause was determined  and a strategy was developed to control the tombstoning and  related out gassing defects.


This metric was used to qualify all of the PCB suppliers for  VIP P technology and invoked supplier capability.  The final  qualification result was that all suppliers had  a Cpk > 1.3 and  the total yield loss for the factories went from 5 % down to


0.033%.


Cynthia Smith*, William J. Cunningham, Randolph J. Miller  and Daryl Sato


1. C. H. Harper, R. Sampson, Electronic Materials & Processes Handbook,” 2nd Ed. McGraw-Hill, New  York, 1994.


2. G. L. Kehl, “Principles of Metallographic  Laboratory Practice,” 3rd Ed. McGraw-Hill, New  York, 1994.


3. J. McElroy, J. Fisher, “NEMI Roadmap Points to  Increasing Density of PWBs and Emergence of  Microvia Technology,”  Future Circuits International, Issue 5, Technology Publishing Ltd, London, 1999.


* University of Illinois at Urbana-Champaign


p 215-220


DOI: 10.1361/cp2003istfa215


## Application of ToF-SIMS to Airborne Organic Contamination Analysis


Application of ToF-SIMS to Airborne Organic Contamination Analysis


Dong Lu, Alastair Trigg, Zhenxiang Xing, Rakesh Kumar and Chang Kuo Chang


Institute of Microelectronics, Singapore


Airborne molecular contamination poses a serious  problem for advanced wafer fabrication as the  devices are continually scaled down. The amount of  this contamination may be only a few monolayers, which are extremely difficult to detect by the  commonly used analytical techniques, such as FTIR. ToF-SIMS has extremely high surface sensitivity for  the analysis of trace contaminants on wafer surfaces. The high mass resolution of ToF-SIMS is also a  powerful tool for the identification of the  contaminants. In the current study, ToF-SIMS is  used to monitor the build-up of airborne amine  contamination on Black Diamond1 surfaces. It has  been found that cleaning of the Black Diamond  surfaces using wet chemicals can lead to photoresist  poisoning. Thermal desorption-GC-MS analysis  revealed that wet cleaning would result in the  accumulation of hydrocarbons on the Black Diamond  surfaces. ToF-SIMS shows that amines can build up  gradually on the Black Diamond surfaces after wet  cleaning, probably via airborne molecular  contamination. For the Black Diamond wafers which  did not go through the wet cleaning process, there  was no significant increase of amines on the wafer  surfaces. The amount of amines on the Black  Diamond surfaces depends on the chemicals used in  the cleaning processes and the wafer storage  conditions. The level of amine contamination can be  significantly reduced after the samples are heated up  to 300˚C for a few minutes in inert atmosphere.


Airborne molecular contamination poses a serious  problem for advanced wafer fabrication as the  devices are continuously scaled down. Introduction  of the copper and low k process has made the


1 Black Diamond is the trade name of a Low K material from  Applied Materials.


problem even more acute. Among the four types of  the airborne molecular contaminants, i.e. acids, bases, condensables and dopants, bases are  particularly harmful to deep-UV lithography due to  photoresist poisoning.


Deep-UV lithography based on chemically-amplified  photoresists is currently employed to produce  devices with feature sizes smaller than 250nm. Chemically-amplified resist systems can provide the  required high sensitivity via photo-chemically  induced acid-catalyzed reactions. Acid generated by  photolysis undergoes a large number of reactions  without being consumed. However, any loss of the  photoacid would result in incomplete reaction and  lead to photoresist poisoning [1].


Amines are one of the major culprits, which can lead  to the loss of the photoacid via the neutralization of  the acid. Sometimes, the amines on the wafer  surfaces may be caused by airborne molecular  contaminants, which are normally at very low  concentration.


Currently, airborne molecular contamination is  mainly monitored in two ways: 1) monitor the trace  contaminants in the air; 2) study the outgassing  behavior of the materials used in the clean room. Both methods emphasize the air quality in the clean  room rather than directly  investigating the  contaminants on the wafer surface. The drawback is  that the airborne molecular contaminants in the air  may or may not result in the contamination of the  wafer surfaces.


Recently, during a wafer fabrication process, it was  noticed that photoresist poisoning occurred after the  Black Diamond layer on the wafer surface was  subjected to cleaning with wet chemicals. However, photoresist poisoning was not observed for the same  Black Diamond wafer which did not go through the  wet cleaning process. Contamination of the Black  Diamond surface during or after the wet cleaning  was suspected to be a possible cause.


In the current study, thermal desorption-GC-MS and  ToF-SIMS are used to study the Black Diamond  surfaces before and after the wet cleaning to identify  the possible organic contamination. ToF-SIMS is


used to monitor the build-up of airborne molecular  contaminants on the Black Diamond surfaces. The  extremely high surface sensitivity of ToF-SIMS  enables the detection of trace contaminants on the  wafer surfaces. The high mass resolution of ToFSIMS is very powerful in the identification of the  contaminants[2]. The mechanism for the formation  of the organic contamination and the effects of  storage conditions on the Black Diamond surface are  also  investigated.


Sample details


Blank wafers with the Black Diamond layer of  500nm were used in the current study. Two  commercial chemical solutions, named as Wet A and  Wet B respectively, were used for the wet cleaning of  the Black Diamond samples.


GC-MS analysis


Thermal desorption-GC-MS analysis was performed  on the blank Black Diamond wafers before and  immediately after wet cleaning. Thermal desorption  was performed at three temperature ranges: 60-150˚C, 150-350˚C and 350-650˚C using a Frontier  Lab’s Double-Shot Pyrolyser attached to the GC-MS  system. The blank Black Diamond wafers were cut  into small pieces to fit into the sample cup, which  was lowered down to the furnace of the pyrolyser for  thermal desorption. The outgassing species from  each temperature range were collected in a cold trap  cooled with liquid nitrogen and introduced into the  GC-MS system at the end of each thermal desorption  step. HP 6890 GC and HP5973 MS were used for  GC-MS analysis.


ToF-SIMS Analysis


An ION-TOF IV ToF-SIMS  instrument was used to  characterize the Black Diamond surfaces before, immediately after and one week after wet cleaning. A  pulsed primary ion beam of 15 keV 69Ga+ was used  for the ToF-SIMS analysis. The primary ion dosage  density was 2.8X1012 ions/cm2, which is within the  static limit of 1013 ions/cm2.


It has been noticed during ToF-SIMS analysis that  there are day-to-day variations in the relative  intensity of the ion fragments. ToF-SIMS data from  the same batch of samples are collected at the same


time and under the same experimental conditions in  order to avoid systematic errors.


Result and Discussions


Thermal Desorption-GC-MS analysis


Figures 1-3 display the GC-MS results obtained for  the Black Diamond samples without wet cleaning  and immediately after wet cleaning using Wet A and  Wet B. Hydrocarbons of C14 – C17 and C14 – C16 were  detected on samples cleaned with Wet A and Wet B  respectively at the thermal desorption temperature of  60-150˚C.  Hydrocarbons of C14 – C19 and C14 – C18  were detected on samples cleaned with Wet A and  Wet B respectively at the thermal desorption  temperature of 150-350˚C (Figures 2 and 3). The  amount of the thermally desorbed hydrocarbons is  fairly small, which is reflected in the low intensities  of GC peaks assignable to the long-chain  hydrocarbons. At 350-650˚C, no outgassing species  can be detected on the Black Diamond surfaces after  wet cleaning with Wet A or Wet B. In comparison, no outgassing species were detected in all three  temperature ranges for the sample without wet  cleaning (Figure 1).


It seems that the wet cleaning process has resulted in  the accumulation of a small amount of hydrocarbons  on the Black Diamond surfaces and these  hydrocarbons are able to desorb completely at  temperatures below 350˚C.  It should be pointed out  that no other organic species were detected from the  chemically cleansed sample surfaces apart from the  hydrocarbons.


Figure 1 GC chromatogram obtained at different  thermal desorption temperatures from Black  Diamond sample without wet cleaning.


4.00 6.00


8.00 10.00 12.00 14.00 16.00 18.00


0  200000  400000  600000  800000


Time--> Abundance


350-650˚C


150-350˚C


60-150˚C


Figure 2 GC chromatogram at various thermal  desorption temperatures obtained from Black  Diamond sample immediately after cleaning using  Wet A.


Figure 3 GC chromatogram at various thermal  desorption temperatures obtained from Black  Diamond sample immediately after cleaning using  Wet B.


ToF-SIMS analysis of freshly prepared samples


ToF-SIMS analysis was carried out on the Black  Diamond surfaces before and immediately after the  wet cleaning using Wet A and Wet B. Figures 4-5  shows the ToF-SIMS spectra collected from the  Black Diamond surfaces before and immediately  after the wet cleaning process. There is little


difference between the two ToF-SIMS spectra before  and after the wet cleaning. The base peak at mass 28  is due to Si while most of the other ion fragments can  be attributed to hydrocarbons, Si or silicon oxide. There is little evidence of the presence of other  organic species.


m ass /  u


x10


0. 5


1. 0


1. 5


2. 0


2. 5


3. 0


3. 5


Figure 4 ToF-SIMS spectra of the Black Diamond  surface without and immediately after wet cleaning  using Wet A.


Figure 5 ToF-SIMS spectra of the Black Diamond  surface without and immediately after wet cleaning  using Wet B.


Thermal desorption GC-MS analysis reveals that  hydrocarbons are the only outgassing materials found  on the Black Diamond surfaces after wet cleaning   and no outgassing materials can be detected on the  Black Diamond surface without wet cleaning. ToFSIMS analysis shows that there is little difference in  the ion fragments on the Black Diamond surfaces  before and immediately after the wet cleaning. It


4.00 6.00 8.00 10.00 12.00 14.00 16.00 18.00


Without


cleaning


Cleaned with Wet


Cleaned with Wet B


Without cleaning


0  300000  600000  900000


appears that wet cleaning itself has not introduced  significant amount of organic contaminants other  than the hydrocarbons.


ToF-SIMS analysis of samples after storage


The Black Diamond wafers with and without wet  cleaning were analyzed again using ToF-SIMS after  storage in a plastic wafer box for one week. Figures  6-7 show the ToF-SIMS spectra collected from the  Black Diamond surfaces after one week storage in  the wafer box without and with wet cleaning using  Wet A and Wet B.


Figure 6 ToF-SIMS spectra of the Black Diamond  surfaces with and without wet cleaning using Wet A  after one week storage in a plastic wafer box.


Figure 7 ToF-SIMS spectra of the Black Diamond  surfaces with and without wet cleaning using Wet B  after one week storage in a plastic wafer box.


There is a significant difference in the ToF-SIMS  spectra collected from the Black Diamond wafers  with and without wet cleaning. For the Black  Diamond surface without wet cleaning, there is not  much change in its ToF-SIMS spectrum after one  week storage.  The majority of the ion fragments are  either due to hydrocarbons or  related to Si or silicon  oxide. For the Black Diamond surfaces with wet  cleaning, the intensities of the amine-related ion  fragments have increased substantially after one  week storage in the wafer box. The amine-related  peaks that have shown significant intensity increase  include CH4N (m/e= 30), C2H6N (m/e= 44), C3H8N (m/e= 58) and C4H10N (m/e =72).


It should be pointed out that the Black Diamond  surface areas used for ToF-SIMS analysis were not  in direct contact with any surfaces of the wafer box  or any other surfaces. It would be interesting and  important to know how the amines contaminants can  get onto the Black Diamond surfaces after storage  while no amine contaminants have been detected for  the freshly prepared Black Diamond surfaces with or  without wet cleaning. It has been noticed in our lab  that amine contamination can also build up gradually  on oxide surfaces stored in the same plastic wafer  box or other types of sample boxes. If amine  contamination can accumulate progressively on two  types of dielectric surfaces stored in different  containers, the most likely mechanism would be via  airborne molecular contamination.


Semi-quantitative


analysis


of


amine


contamination


A semi-quantitative method was adopted to evaluate  the amine contamination on the Black Diamond  surfaces. The intensities of the four amine-related  ToF-SIMS peaks, i.e. CH4N(30), C2H6N(44), C3H8N(58) and C4H10N(72),  are normalized against  the intensity of Si(28) peak. The semi-quantitative  analysis was performed for all the Black Diamond  surfaces investigated in the current study, i.e. 1) freshly prepared Black Diamond surface without wet  cleaning; 2) Black diamond surface without wet  cleaning after  one week storage in the wafer box; 3)  freshly prepared Black Diamond surface immediately  after the wet cleaning using Wet A and Wet B; 4) Black Diamond surfaces after the wet cleaning and  one week storage in the wafer box. The intensity of   Si(28) peak is taken to be 100% and the relative  intensities of each amine fragment are presented as a  percentage of the Si(28) peak. The semi-quantitative  result is summarized in Table I for the freshly  prepared Black Diamond samples and in Table II for


Normal


TiSi2


formation regions Abnormal


TiSi2  growth In VSS contact


Fig. 1: SEM image of NMOS islands showing abnormal and  normal titanium silicide formation.


Several regions on the NMOS islands are dark gray and  appear as depressions in the otherwise raised island.  These  regions correspond to areas of titanium silicide (TiSi2) formation that were removed by the HF etch during sample  preparation.  The SEM image of the failed device in  Fig. 1  shows a discontinuity, or break, in the TiSi2 layer at the  rectangular VSS contact region.  The break is a raised feature, as indicated by the arrow in Fig. 1 and appears to be the result  of incomplete silicide formation.  TEM images of a failed die  before deprocessing (Fig. 2) confirmed that the break  corresponded to a region of no TiSi2 growth.  This type of  TiSi2 break at VSS contact regions was found on a large  majority of the bits with functional failures.


W contact


silicide break


BOX


Si substrate


Fig. 2: Low-magnification (a) and high-magnification (b) TEM images showing a silicide break (denoted by the arrow) at the VSS contact of a failed SRAM cell.


AFM and SCM


The VSS regions were imaged with atomic force microscopy (AFM) and SCM for both functioning and failed devices.  Since the density of failed VSS contact sites is relatively low (typically one or two sites in a 64K SRAM array), this enabled  several "good" devices to be imaged from areas adjacent to the  failed devices on a single sample, eliminating any question as  to whether experimental conditions were contributing to  differences in the SCM images.  The top-down AFM image in  Fig. 3(a) shows the topography of a functioning or “good” NMOS island.  The SCM image of Fig. 3(b) shows the  corresponding carrier distribution for the functioning NMOS  island.  The heavily implanted n+ source/drain regions are


clearly defined and isolated from one another by the lightly  doped p-body region.  The SCM image also shows the VSS  contact being comprised of a p+ body tie sandwiched between  two n+ source areas of adjacent transistors.  Even though all  regions in the VSS contact are heavily doped, the darker SCM  contrast in the p+ body tie region is clearly distinguishable  from the lighter contrast in the n+ source areas.


Fig. 3: Top-down images of an NMOS island in a functioning


SRAM array showing (a) topography (AFM) and (b) carrier


distribution (SCM) at the VSS contact region.  The silicide  regions (dark gray) in (a) show uniform TiSi2 formation, while  the heavily-doped source/drain regions are separated by


clearly defined p-body regions.


In contrast, Fig. 4 shows top-down (a) AFM and (b) SCM  images of a failure site in an island adjacent to the NMOS  island in Fig. 3.  The AFM image of the failed device, Fig. 4(a), shows a discontinuity, or break, in the silicide layer at the  VSS contact region, similar to that observed in the SEM image  in Fig. 1.  The break is a raised feature, as indicated by the  arrow in the topographical line scan of Fig. 4(c).  In addition, this feature is centered approximately at the interface between  the n+ source and p+ body tie.  Accompanying the break in the  silicide is an anomalous spreading of carriers, seen in the SCM  image of Fig. 4(b).  These carriers appear to spread through  the lightly p doped channel region of the adjacent NMOS  transistor.


Fig. 4: Top-down (a) AFM and (b) SCM images of the VSS  contact region of a defective NMOS island in a SRAM array  that failed functional testing.  The topographical image in (a) shows abnormal silicide growth, with a discontinuity, or  break, in the TiSi2.  Adjacent to the TiSi2 defect, the SCM  image in (b) shows carriers spreading through the lightly  doped channel region of the device.  (c) Topographical line  scan across the VSS contact showing the break in the silicide  layer (denoted by the arrow).


Although the results of the top-down SCM images identify  carrier spreading as the signature of the failed SRAM cells, they do not fully explain the actual failure mechanism.  To  address this, cross-sectional SCM imaging of both functional  and defective NMOS islands was performed, and the results  are shown in Fig. 5.  The cross section was taken along the  edge of a row of NMOS islands, including one island with a  defect site in the TiSi2 as seen in Fig. 4.


Cross-sectional samples were prepared by standard polishing  procedures using diamond-coated lapping films on a polishing  wheel.  Failed devices were isolated by electrical testing and  then marked with a laser scribe to ensure the device of interest


was correctly targeted.  Next, the die containing the defect site  was mounted on a polishing stub using hot wax and then  polished with lapping films, starting with a 15-µm particle size  disk and incrementally reducing the particle size to 0.1 µm.  The final polish was performed with colloidal silica slurries to  obtain a scratch-free surface and form the passivating oxide  layer.  Site-specific preparation requires repeated optical  inspection and careful attention so that a finished surface is  obtained at the site of interest without cutting past the device.  After polishing, the sample and polish stub were attached to a  custom sample holder that was mounted directly on the SCM  system for imaging.


Fig. 5: (a) Schematic representation of the cross-section  through the VSS contact region of an NMOS island, showing a  p+ body tie sandwiched between two n+ source regions of the  adjacent transistors.  Cross-sectional SCM images across the  VSS contact region of NMOS islands from (b) functional and


(c) failed SRAM devices.  The cross section of the defective  device in (c) shows an abnormal dopant distribution near the  defect that may be attributed to dopant diffusion from the  overlying BPSG through the TiSi2 break.


Fig. 5(a) is a schematic representation of the device cross  section that shows the two adjacent n-type MOSFETs  separated by a p+ body tie region on an NMOS island.  The  SCM image in Fig. 5(b) shows a pair of transistors at the edge  of a defect-free NMOS island.  Similar to the schematic in Fig. 5(a), the SCM image of Fig. 5(b) shows two pairs of lightcolored, n-type source/drain regions separated by a darkcolored p-body, each pair corresponding to an NMOS  transistor.  The two transistors are separated from each other  by the p+ body tie at the center of the image.  In contrast, the  defect site in Fig. 5(c) shows a marked difference in SCM  contrast at the source area of the transistor adjacent to the  defect.  The location of the defect (indicated by the arrow) shows a discontinuity in carrier distribution, while the contrast  to the right of the defect suggests that p-type carriers dominate  at the n+source  (i.e., the n+ source is being counter-doped to p  type) and are also encroaching on the channel of the adjacent  transistor. The counter-doping at the source and carrier  encroachment in the channel region could be one of the  mechanisms that causes the cell to fail functionally.  The  functional failure could also be the result of high source  resistance due to the TiSi2 break in the VSS contact.


The abnormal carrier spreading may be attributed to the  diffusion of p-type dopants from the overlying ILD, which is  made of silicon dioxide doped with phosphorous and boron  and is commonly known as borophosphosilicate glass (BPSG).  In this model, boron from the BPSG diffuses through the  break in the silicide layer and into the source and channel  regions of the adjacent transistor, changing the carrier  distribution in the device.


The action taken to correct the abnormal silicide growth was  to replace the existing BPSG oxide layer with an undoped, high-density plasma (HDP) silicon dioxide layer.  The initial  reason for choosing the HDP oxide was the absence of  dopants in the film, eliminating the possibility of dopants  diffusing through the silicide break.  In addition, the HDP  oxide is deposited at a much lower substrate temperature of  ~ 450 °C versus ~ 850 °C for the BPSG oxide.


After implementing the process change to HDP oxide, the  yield on the SRAMs increased significantly in subsequent lots.  In addition, all the functional failures in subsequently lots no  longer exhibited the same characteristics described in the  Introduction section, and they were found to be the results of  other processing defects such as gate oxide short and metal  short that were not related to silicide break.  It appeared that  switching to HDP had eliminated silicide breaks in the VSS  regions.


The effects of HDP on the silicide formation are still not well  understood.   The silicide growth chemistry at the VSS contact  is, however, extremely complex. It is postulated that the  silicide layer in the VSS region is not well formed and changes  in the process temperatures in the subsequent ILD deposition


can affect and alter the silicide formation in this region.  More  data and discussion of the silicide formation in the VSS contact  will be presented in the next two sections.


Layout Dependency


The elimination of silicide breaks by switching to the HDP  oxide suggests that the differences in process temperature  contribute to the break formation; however, the consistent  location of the breaks at the VSS contact suggests that SRAM  cell layout also plays a role in forming this defect.  As  previously mentioned, the VSS contact consists of a p+ body tie  region sandwiched between two n+ source regions of the  adjacent transistors; therefore, the contact has two n+/p+ junctions on either side of the body tie.  The two junctions are  identical in every way except for very slight lithographic  misalignments due to the inherent overlay tolerance of the  lithographic tool.  This results in a slight overlap and counter  doping between the n+ and p+ regions on one of the n+/p+ junctions and a slight “underlap” (or separation) on the other  junction.  Interestingly, all the breaks observed in the silicide  layers from all the failed SRAM cells occur only on the “overlap” junctions, confirmed by TEM analysis.  Fig. 6  shows a TEM image of a typical VSS contact.  One interesting  feature in this image is an implant dislocation band in the p+ body tie region, which was not observed in the n+ regions. This dislocation band provides an internal alignment marker, showing the lithographic misalignment.  Fig. 6, for example, shows that the p+ body tie region is shifted to the right of the  contact.


The effects of dopant distribution at the n+/p+ junctions on  silicide formation at the VSS contact were further investigated  by examining the silicide profiles of a “good” VSS contact (Fig. 7) adjacent to the failed VSS contact shown in Fig. 2.  Even in the “good” contact, the silicide profiles are quite  different between the “overlap” and “underlap” junctions.   The silicide profile in the “underlap” region is fairly uniform, in contrast to the large variation in silicide thickness in the “overlap” region (Fig. 7).  There is a small area (indicated by  the arrow in Fig. 7) in the “overlap” region where the silicide  thickness is smallest.  This area corresponds approximately to  the silicide  break location observed in the “failed” VSS contact  in Fig. 2.


As mentioned previously in the Introduction section, one  version of SRAM (version 3) is more immune to functional  failure than the other two versions of SRAMs (version 1 and  version 2) and there are fewer titanium silicide breaks in the  VSS regions in this version.  The main difference between the  version 3 SRAM and the other two versions is the width of  both p+ and n+ implant regions in the VSS contact area, shown  in Figure 8.  Version 3 SRAMs have a narrower p+ region and   a wider n+ region than the other two versions. This slight  change in the width of implant regions appears to affect the  silicide growth profiles in the VSS contact. A more detailed  discussion of layout-dependent silicide growth will be  presented in the next section.


Implant dislocation


Fig. 6: TEM  image showing the implant dislocation in p+ body tie region at the VSS contact.  This implant dislocation  band provides an internal marker showing the lithographic  misalignment.


Si  substrate


“overlap”  n + /p +


junction


“ underlap ” n + /p +


“overlap”  n + /p + junction


j cti  (a)


Fig. 7:  Low-magnification  (a) and high-magnification (b) TEM images showing titanium silicide profile at the VSS  contact of a “good” SRAM cell that is adjacent to the failed  cell in Fig. 2.  The arrow in (b) indicates the area where the  silicide thickness in minimal in the contact.  This area  corresponds approximately to the TiSi2 break location  observed in the “failed” VSS contact in Fig. 2.


VSS contact


region


NMOS Islands


Fig. 8:  Comparison of the VSS contact layout between (a)  version 1 and version 2 SRAMs and (b) a version 3 SRAM. Version 3 SRAM has a narrower p+ region and a wider n+ region than the other two versions.


Results from a Short-loop Lot


To further understand the effect of dopant distribution on  silicide formation, two wafers from a short-loop lot, one with  HDP and the other with BPSG oxide, were analyzed.  These  wafers were made with an intentionally exaggerated  lithographic misalignment in the VSS contact region, resulting  in a large overlap and counter doping between the n+ and p+ regions on one of the n+/p+ junctions and a large “underlap” (or separation) on the other junction.


Several samples from each wafer were randomly selected for  deprocessing, optical/SEM inspection, SCM analysis, and  TEM analysis.  No TiSi2 breaks were observed in any of the  analyzed samples.  This is not surprising since the density of  the failed bits in a given die is small, typically one or two in a  64K SRAM array.  Electrical testing is normally used to  identify and localize failed bits in the SRAMs in a fullyprocessed lot.  However, in this short-loop lot, the devices  were not fully processed and functional; consequently, electrical testing could not be used for fail bit identification  and localization.


TEM images of a VSS contact region of a typical version 1  SRAM with BPSG oxide is shown Fig. 9.  Fig. 9 clearly  shows that differences exist in both TiSi2 uniformity and  formation depth between the “overlap” and “underlap” regions.


“underlap” n+/p+junction


“overlap” n+/p+


(c)(b)(a)


Fig. 9:  Low-magnification  (a) and high-magnification (b) scanning transmission electron microscopy (STEM) images  showing a typical TiSi2  profile at the VSS contact of a version  1 SRAM cell in the BPSG oxide wafer of the short-loop lot. The arrow in (b) indicates the area where the silicide  thickness is smallest in the contact.  The TEM image in (c) was  taken from the same area in (b) with the sample tilting  significantly to show the grain boundary.  The grain boundary  location corresponds to the area where the silicide thickness  in smallest (indicated by the arrow in (c)).


In the “overlap” region, TiSi2 forms near the initial silicon  surface, indicated by the dashed line in Fig. 9(a). There is also  a variation in TiSi2 thickness in the “overlap” region (Figs. 9(b) and 9(c)).  In Fig. 9(c), the sample was tilted significantly  to show the grain boundary (denoted by the arrow).   The  location of the grain boundary corresponds to the area in the  TiSi2 layer where the thickness is smallest in the “overlap” region.  Overall, the TiSi2 profile in the “overlap” region  resembles that observed in Fig. 7 for a “good” VSS contact. Interestingly, the grain boundary location observed in Fig. 9


(c) is approximately the same for all the samples that have  been analyzed.  In the “underlap” region, TiSi2 forms at a  depth below the initial silicon surface.  The TiSi2 layer is also  more uniform in this region, compared to the “overlap” region. The differences between the “overlap” and “underlap” regions  may be related to the local changes in diffusion coefficients of  Si and/or Ti that significant affect the silicide formation in  these regions.


As a comparison, the TiSi2 profile of a VSS contact of a typical  version 3 SRAM is shown in Fig. 10.  Version 3 SRAMs have  a narrower p+ region and a wider n+ region in the VSS contact  than the other two versions.    In the “overlap” region, the  silicide also forms near the initial silicon surface.  There is,


however, less variation in TiSi2 thickness in this SRAM  compared to the version 1 SRAM shown in Fig. 9.  In


addition, the grain boundary observed in Fig. 9(c) is not


present in this SRAM.   In the “underlap” region, TiSi2 again  forms at the depth below the initial silicon surface.  The TiSi2  is also relatively uniform in this ‘underlap” region.   The


differences observed in the “overlap” region between version  1 and version 3 SRAMs clearly indicate the importance of cell


layout in affecting the silicide formation.


“overlap” n+/p+junction


Fig. 10:  Low-magnification  (a) and high-magnification (b) STEM images showing a typical TiSi2 profile at the VSS contact  of a version 3 SRAM cell in the BPSG oxide wafer of the  short-loop lot. The TEM image in (c) was taken from the same  area in (b) with the sample tilted significantly.


TEM analyses were also performed on the HDP oxide wafer  for both version 1 and version 3 SRAMs.  The TEM results  obtained from this wafer are quite similar to those from the  BPSG oxide wafer shown in Figs. 9 and 10.


It appears that the chemistry of TiSi2 growth is very complex, and particularly sensitive to the n+/p+ junctions of the VSS  contact.  In other areas such as n+ or p+ source/drain regions, these n+/p+ junctions do not exist, and the TiSi2 profiles are  uniform in both thickness and formation depth for both BPSG  oxide and HDP oxide wafers, as shown in Fig. 11.  The TiSi2  formation also occurs near the initial silicon surface (Fig. 11).


n+ source/drain area


Fig. 11:  STEM image showing a typical TiSi2 profile at a n+ source/drain region  in the BPSG oxide wafer of the shortloop lot. The TiSi2 in this region is uniform in both thickness  and formation depth.


SCM images were also acquired on both wafers.   There is  little difference in the carrier profiles between the BPSG oxide  and HDP oxide wafers.  The differences between version 1  and version 3 SRAMs are also very small.   Fig. 12, for  example, shows the top-down SCM images of both version 1  and version 3 SRAMs with BPSG oxide.   In both SRAMs, differences exist in carrier profiles between the “overlap” and “underlap” regions.   In the “overlap” region, a slight carrier  spreading was observed, while no spreading was observed in  the “underlap” region.


The results from the short-loop lot clearly suggest that  complexity in TiSi2 originates and occurs primarily in the  p+/n+ junctions, particularly in the “overlap” region.  In the “overlap” region, the variation in TiSi2 thickness strongly  depends on the relative width of p+and n+ areas, as evidenced  by the difference between version 1 and version 3 SRAMs.  In  addition, the consistent location of the grain boundary at the  location where the silicide thickness is smallest in the “overlap” region for both BPSG and HDP oxides strongly  suggests that SRAM cell layout plays an important role in the  TiSi2 growth.  The silicide profile in the “overlap” region also  looks remarkably similar to that observed in the VSS contact of  a “good” SRAM cell shown in Fig. 7.   The grain boundary  observed in Fig. 9(c) appears to be the weakest point in the  silicide layer of the “overlap” region where the silicide break  is most likely to occur. The probability of occurrence of the


silicide break, however, most likely depends on the process  temperatures. Because the process temperature is higher for  BPSG than for HDP oxide (850 °C versus 450 °C), the  likelihood of silicide break is probably larger for the BPSG  oxide.


“underlap” n+/p+


n+ source/drain regions


Fig. 12: Top-down SCM images of the VSS contact region of


(a) a version 1 SRAM and (b) version 3 SRAM in the BPSG  oxide wafer of the short-loop lot.


TEM and SCM were used to identify the root cause of TiSi2  breaks in the VSS contact of an SRAM cell.  The TiSi2 break  originated in the “overlap” n+/p+ junction of the VSS contact  and was the result of abnormal silicide growth in this region.  Accompanying the break in the silicide layer was an  anomalous spreading of p-type carriers into the adjacent  NMOS transistor.  The corrective action taken to eliminate the  TiSi2 break was to replace the existing BPSG oxide layer with


an undoped, high-density plasma (HDP) silicon dioxide layer.  Results from a short-loop lot strongly suggested that both cell  layout and process temperature played an important role in the  silicide growth at the n+/p+ junctions in the VSS contact.


The authors thank Rich Anderson, Chuck Hembree, and Dan  Kammler for reviewing the manuscript. The authors  acknowledge the wafer Fab employees at the Microelectronics  Development Laboratory for fabricating the devices.  Sandia is  a multiprogram laboratory operated by Sandia Corporation, a  Lockheed Martin Company, for the United States Department  of Energy under contract number DE-AC04-94AL85000.


[1] David B. Williams and Barry C. Carter, Transmission  Electron Microscopy: A Textbook for Materials Science, Plenum Press, New York  (1999).


[2]    R. N. Kleiman, M. L. O'Malley, F. H. Baumann, J. P. Garno, and G. L. Timp, Scanning Capacitance  Microscopy Imaging of Silicon Metal-OxideSemiconductor Field Effect Transistors,” J. Vac. Sci. Technol. B 18, 2034 (2000).


[3]   E. I. Cole, Jr., P. Tangyunyong and D. L. Barton, Backside Localization of Open and Shorted IC  Interconnections," 36th IEEE International Reliability  Physics Symposium, 1998, pp. 129-136.


[4]  E. I. Cole, Jr., J. M. Soden, J. L. Rife, D. L. Barton, and  C. L. Henderson, Novel Failure Analysis Techniques  Using Photon Probing with a Scanning Optical  Microscopy, 32th IEEE International Reliability Physics  Symposium, 1994, pp. 388-398.


[5]   M. R. Bruce, V. J. Bruce, D. H. Eppes, J. Wilcox, E. I. Cole, P. Tangyunyong, and C. F. Hawkins, Soft Defect  Localization (SDL) on ICs, Proceedings of 28th  International Symposium for Testing and Failure  Analysis, 2002, pp. 21-27.


# Session 8: Metrology and Materials Analysis 2 


Bryan Tracy • AMD • Sunnyvale, CA


p 206-208


DOI: 10.1361/cp2003istfa206


## Contact Failure due to Particulate Defect in a 0.13 µm CMOS Process


Contact Failure due to Particulate Defect in a 0.13 µm CMOS Process


Sandeep Bagchi, Valli Arunachalam, Javier Saenz, James Beck, Lupe Duncan and Jim Conner


Motorola Inc., Austin, TX


Random single bit failures were encountered in cache areas of  Motorola’s 0.13 µm CMOS products under development. Extensive in-line probe data and end-of-line probe data in  conjunction with failure analysis indicated the presence of  particles at the upper surface of tungsten contacts. This paper  describes how TEM based techniques were used to analyze the  origin of the defect which in turn enabled process optimization  and yield improvement.


Random single bit failures were detected in the cache area  through end-of-line electrical testing and failure analysis. Focused ion beam (FIB) cross sectioning and scanning  electron microscopy (SEM) of the failure location indicated  the presence of particles near the top of the contact. Figure 1  illustrates such a defect found by FIB-SEM.


Figure 1: FIB-SEM image of the defect.


In-line detection of such defect particles was also attempted. A  typical in-line inspection data is shown in Figure 2. Transmission electron microscopy (TEM) based techniques  were utilized for the detailed analysis of the defect  morphology and chemistry. Details of the TEM analyses  follow.


Figure 2: A defect seen by in line optical inspection


TEM Analysis


Cross-sectional TEM specimens of several defects were  prepared by FIB milling and in-situ specimen lift-out  technique [1]. The specimens were analyzed in a 200 keV  field-emission source TEM, equipped with scanning  transmission electron microscopy (STEM) and energy  dispersive x-ray spectroscopy (EDXS) capabilities. An  overview TEM image of one of the defect particles is shown  in Figure 3 below.


Figure 3: Overview TEM image of a defect.


200nm


A few noteworthy observations were made with respect to the  morphology and possible elemental atomic numbers (Z) of   the materials comprising the particle. The contrast in the  particle varied between light and dark regions. Keeping in  consideration that elements of higher Z scatter more strongly  than the elements of lower Z, and more scattering translates to  a darker contrast in TEM images, this gave us an initial  indication of the distribution of elements in the particle. We  deduced that the lighter contrast regions contained a lower Z  element, while the presence of a higher Z element in the  particle coincided with a darker contrast. The shape of the  defect was indicative of a “flake” of metallic nature that had  somehow curled or bent into the folded configuration seen in  the TEM images. The elemental composition of the particle  was analyzed by EDS techniques. STEM-EDXS analysis with  elemental area maps yielded the data presented in Figure 4  below.


Figure 4: STEM-EDXS elemental maps of the defect shown in


Figure 3.


The above elemental maps showed that Ti and W were the  elements present in the particle. The Cu elemental map  showed no presence of that element in the particle. This was  important, as it ruled out the subsequent Cu metallization   processes as the possible source of  the particle. Results of  further spot EDXS analysis of selected regions of the particle  are presented in Figure 5. It also indicated the distribution of  Ti and W in the particle, with the region between two  segments of the folded particle containing elements  characteristic of the SiO2, the inter-layer dielectric (ILD) material.


Figure 5: Spot EDXS data from indicated areas of the defect. 1 – Strong W, no Ti; 2 – Strong W, no Ti; 3 – Strong Ti, W;  4 – Strong Si, O, some Ti.


During our extensive investigations of several such defects, not all of them manifested themselves quite as distinctly in the  TEM images as the one discussed so far. Due to inherently  smaller size, or from difficulty in containing the fullest extent  of the defect in the TEM specimen during careful preparation, we encountered situations where the defects were present in  indistinct and discontinuous fashion. An example of such a  situation is presented in Figure 6 below.


Figure 6: A defect, manifested in indistinct and discontinuous  fashion.


50nm  20nm


Figure7: STEM-EDXS linescans through the defect shown in  Figure 6. The vertical line in the intensity profiles corresponds  to the signal from the position of the notch marker on the  vertical linescan indicator on the STEM image. Carbon  contamination during high-magnification TEM imaging  obscured the defect in the STEM image above.


Elemental EDXS posed a challenge for the analyst, as there  was insufficient material present to yield a conclusive  elemental map. In such instances, it was useful to perform  STEM-EDXS linescan analysis through the defect area, as the  counting statistics were much better in comparison. Figure 7  above shows the linescan data from the defect. Ti signal was  clearly seen in the defect area, which confirmed it to be  similar in nature to the defect described earlier. Unlike the  previous defect, W was not found to be associated with this  defect. The absence of Cu and Ta signals from the area again  led us to conclude that the interconnect metallization   processes were not the source of the defect.


The presence of Ti and W in the particle provided important  clues as to its origin. In our process W is used as a contact  metal, while a lining of Ti and TiN is formed in the contact  sidewalls to provide good adhesion. From the above analyses, we concluded that the particle originated from the contacts  themselves, and not from any extraneous source. The curled  shape of the particles also led us to conclude that a “peeling” of the W and Ti/TiN during the subsequent processing of  deposited contact materials was responsible for the generation  of these defects. Based on our findings, suitable corrective


steps in our contact process modules are being implemented.


l i


Cleaned with Wet  A


the Black Diamond samples after one week storage  in a wafer box. It is clear that the amount of amines  is negligible for the Black Diamond surfaces without  wet cleaning (with or without storage) and  immediately after the wet cleaning using Wet A or  Wet B. For the Black Diamond surfaces which had  been stored one week after the wet cleaning, however, there is a significant increase in the relative  intensity of the amine fragments.


It can be concluded that the wet cleaning itself does  not introduce the amine contamination, even though  it can result in the accumulation of a small amount of  hydrocarbons onto the Black Diamond surface. The  hydrocarbons on the Black Diamond surface can  facilitate the accumulation of the airborne molecular  amines during storage. Storage does not seem to  affect the Black Diamond surface which has not gone  through the wet cleaning process, probably due to its  chemical inertness.


Removal of the amine contamination


Amines have been found to be harmful to the deepUV lithography by causing  photoresist poisoning. ToF-SIMS analysis has confirmed that amines can  build up gradually on Black Diamond surfaces after  the wet cleaning process, especially for the wafers  cleaned using Wet A. It is imperative that a solution  be found to remove the amine contamination from  the Black Diamond surfaces in order to reduce  amine-induced photoresist poisoning.


In the current study, it was found that heating up the  Black Diamond to 300˚C for five minutes in nitrogen  atmosphere can effectively remove the amine  contamination from the Black Diamond surface. Figure 8 shows the ToF-SIMS spectra of the Black  Diamond surfaces with and without heating one week  after wet cleaning with Wet A.


0. 2


0. 4


0. 6


0. 8


1. 2


Figure 8 ToF-SIMS spectra of the Black Diamond  surfaces with and without heating one week after wet  cleaning with Wet A.


It can be observed that there is a significant  reduction in the intensities of amine-related ion  fragments. Table 3 shows the semi-quantitative ToFSIMS result.


Amine-induced photoresist poisoning has been well  known. However, the mechanism for the formation  of this amine contamination is still not well  understood. In this study, it has been found that wet  cleaning of the Black Diamond surfaces can  introduce a small amount of hydrocarbons, which  could be responsible for the gradual accumulation of  amine species via airborne molecular contamination. The amount of amines on the Black Diamond  surfaces depends on the chemicals used in the  cleaning processes and the wafer storage conditions. The amount of amine contamination can be  significantly reduced after the samples are heated up  to 300˚C for a few minutes in nitrogen atmosphere. Airborne organic contamination poses a serious  problem for the advanced wafer fabrication as the  devices are continually scaled down. Introduction of  the copper and low k process has made the problem  even more severe. ToF-SIMS was used successfully  in the current work for the analysis of airborne  molecular amine contamination on Black Diamond  surfaces. This information is valuable for materials  selection, process control and failure analysis. The  same technique may also be extended to study the  surface organic contamination of other surfaces and  wafers cleaned using other chemicals.


1. H. Ito, IBM J. Res. Develop. 41-1/2, 69-80


2. T.Fister, T. Schuerlein and P. Lindley, ToFSIMS: Surface Analysis by Mass Spectrometry,  P673, Eds. J.C. Vickerman and D. Briggs, IM  Publications and SurfaceSpectra Limited, (2001)


Without heating


Heated to 300˚C


Table 1 ToF-SIMS result on freshly prepared Black Diamond surfaces  Ion fragments (Mass) Without cleaning


Cleaned with Wet A Cleaned with Wet B


CH4N (30)


1.93 ± 0.16a


2.62  ± 0.13


2.27  ± 1.05


C2H6N (44)


8.20  ± 0.89


6.39  ± 0.16


6.95  ± 2.37


C3H8N (58)


21.42  ± 2.49


15.72  ± 0.29


19.6  ± 7.58


C4H10N (72)


11.32  ± 1.10


8.49  ± 0.49


10.73  ± 4.34


a: ToF-SIMS analysis was carried out in three areas for each sample and the data presented is the average the three  measurements.


Table 2 ToF-SIMS results on the Black Diamond surfaces after one week storage


Ion fragments (Mass) Without cleaning


1.39 ± 0.11


4.19 ± 1.00


2.04 ± 0.16


4.04 ± 0.21


19.99 ± 4.01


7.44 ± 0.66


10.44 ± 1.13


59.85 ± 10.99


25.59 ± 1.64


4.23 ± 0.27


34.02 ± 7.74


14.38 ± 0.98


Table 3 ToF-SIMS results on the Black Diamond surface cleaned with Wet A with and without heating  Ion fragments (Mass) Without heating After heating


1.71 ± 0.17


3.04 ± 1.13


3.86 ± 1.39


1.13 ± 0.16


# Session 9: Test 1 


Jerry Soden • Sandia National Laboratories • Albuquerque, NM


p 222-231


DOI: 10.1361/cp2003istfa222


## Yield-Modeling and Test Oriented Taxonomy of IC Structure Deformations


Yield-Modeling and Test Oriented Taxonomy of IC Structure Deformations


W. Maly, T. Zanon, and T. Vogels


Carnegie Mellon University,  Pittsburgh, PA


This paper proposes a taxonomy of process-induced deformations of IC structures. Such a taxonomy is envisioned as a foundation for yield modeling and development of test strategies, as well as, for design of ICs with redundancy. It is proposed to address the rapidly growing complexity of interaction between process-induced deformations of IC structures and steadily shrinking geometry of deep submicron ICs.


Integrated Circuits (ICs) must be tested due to sometimesunacceptable process-induced random deformations of one or more of its layers. Therefore, we often ask a fundamental question to properly handle test development as well as yield learning: Which of the deformations cause tester-detectable malfunction of the IC or, simply, an IC failure? In this paper,we propose a new taxonomy of process-induced deformations,which should be instrumental in answering this important question [1, 2].


Deformation, Fault and Failure


Since the subject of this paper cuts through a number of traditionally disjoint domains, it is useful to begin with a short review of the terminology and basic concepts used in the body of the paper.


IC manufacturing is a sequence of inherently unstable processing steps resulting in a "sandwich" of conducting, semi-conducting and isolating layers. Regardless of the achieved level of perfection in the control of all IC processing steps, physical characteristics of any point in a fabricated device are different from the characteristics of a corresponding point in any other device, and different from the expected and the desired characteristics speciﬁed for the product. In this paper we call this difference a deformation of the IC structure.


Deformations of IC structures may or may not inﬂuence the behavior of the fabricated device. If they do, then there are two options: (a) the deformed circuit misbehaves in an unacceptable way or (b) the behavior's abnormality is tolerable. We call the difference in behavior between unacceptably deformed structure and the "perfect" IC structure a fault.


Finally, we call failures those IC malfunctions that are detectable on the tester or in-system. Note that not all faults are detected by either the tester or in the system in which the fabricated IC is used.


Yield, Quality of Test and Reliability


The correctness of an IC behavior is assessed several times during the lifespan of a product via test. But testing is imperfect and the tester may reject fault-free ICs or may accept ICs that have faults. In order to fully understand the impact of test imperfections on yield estimation, test-quality and circuit-reliability assessment, one needs to capture the relationship between yield loss (measured by the wafer and ﬁnal tests), the number of escapes, or some other measure of IC reliability, and the attributes of both, IC layout and process induced deformations of fabricated devices. Key elements of this relationship are strong functions of the complex interplay between characteristics of the deformation and the affected circuit. The most important aspect of this interplay is closely tied to the geometry of both, deformation and the circuit's layout.


Fig. 1 illustrates the essence of this observation. A small shift in the location of the same cluster of defects (shown on the left side of Fig. 1) causes a big difference in the electrical consequences of its presence (Fig. 1a-c). Note that the particular electrical misbehavior of the affected circuit strongly depends on details of the geometry of both, layout and defects.


Figure 1. Cluster of defects placed in three different locations of a short metal (Al) bus.


Probability of Fault


From the above, we conclude that conscious control of yield loss, reliability levels and quality of a given test strategy is conditioned by the ability to estimate the probability of IC faults.


And such a probability is a function of deformation characteristics and geometry of IC layout.


Goal of this paper


To address the issue "Which deformation causes tester detectable IC malfunction", one must ﬁrst asses the probability of an IC failure in terms of interaction between geometry of the deformation and geometry of IC layout. This paper attempts to make a ﬁrst step towards this goal by discussing geometry and extent of IC deformation and proposing a methodology to describe them in a fashion suitable for applications in yield and test.


Deformations


This section presents a collection of real-life examples of the IC structure deformations that may result in tester detectable IC malfunctions. Such a collection is presented here to form the basis for a generalization of process-induced IC deformations characteristics discussed in the subsequent section of this paper.


Gradual Deviations of Physical Parameters


There exist plenty of examples for a gradual change in physical parameters across a layer formed on the surface of a silicon wafer. Such gradual changes are typically results of a slowlyﬂuctuating process condition such as temperature. As an example, Fig. 2 shows a colored picture of a silicon wafer (wafer map) after thermal oxidation. Different shades in the picture indicate different oxide thicknesses, highlighted with superimposed contour lines. In general, all physical parameters of IC layers can be depicted as wafer maps such as the map shown in Fig. 2. Such maps can characterize a particular wafer, as well as, describe statistics for any set of wafers (for instance, mean value of a parameter for a speciﬁc lot of wafers).


Figure 2.  Picture of a 200 mm silicon wafer after thermal oxidation. Different shades represent different oxide thicknesses (source: Philips).


Regions of Missing and Extra Material


Regions of extra or missing material that are added or subtracted from the pattern deﬁned by IC design geometry - are the most often recognizable reasons for the test to fail and thus yield loss. Deformations of this kind, usually called "spot defects", are assumed to be "killers," i.e., deformations, which are likely to cause circuit mal-function and yield loss.


There are many types of deformations in general. Figures 3-5 attempt to illustrate, via 24 examples, a large diversity of geometries of the boundaries of deformations.  Each shown example uses  either an SEM or an optical image. All examples are taken from industry. Where necessary, layers are annotated.


Below each image, we list the cause, the electrical consequence (EC), and the layer(s) involved.  Among the electrical consequences are extra or missing connections and extra or missing devices. Most of the examples also show the contamination and the deformed regions.


Based on the collection of pictures in Figures 3-5, one should make ﬁrst the observation that the shown deformations have well deﬁned boundaries.  Further, some of the deformations are very different from the traditionally accepted vision of what a small rounded "spot defect" should look like.


The geometries of the regions deﬁned by the deformations’boundaries span a wide range of shapes and sizes.  Shapes vary from the "perfect" circle, such as a pinhole (Fig. 5a), to the stretched rectangle, such as scratch lines (Fig. 5c) or stringers(Fig. 4e).  Sizes vary from the small, such as a pinhole (Fig.


5a), to large area deformations affecting multiple lines (Figs.


3c or 5f) or transistors (Fig. 3f).


Furthermore, some of the shapes of the deformed regions can be easily described by circles (Figs. 4d, 3h, 5g) while others do not ﬁll out their enclosing circle (Figs. 5f, 5e, 3g) and require a more sophisticated description.


Some of the deformed regions actually consist of multiple components (Figs. 3g, 3a, 5c). While the components may be detected or observed as separate defects, they are caused by the same deforming event and must be treated together. Finally,one can notice that not all deformations shown in Figs. 3-5 cause failures. For instance, deformations shown in Figs. 5f, g and h are very likely not to affect the behavior of the affected circuit (at least in a short period of time after fabrication).


It is worth highlighting a few categories of deformations that cannot be well described by a spot defect, the typically assumed notion of a circular region of a small size with missing or extra material. A very distinct category of deformations with clearly deﬁned boundaries contains stringers, represented by the example in Fig. 4e. Stringers are very thin "wires" bridging non-equipotential IC regions, which are difﬁcult to detect by standard optical techniques. They are formed as a result of a few random events occurring in the process at speciﬁc locations of the layout. In addition, they have a relatively large spectrum of resistances. They also typically involve many nets in the circuit. But the most important characteristic of a stringer is that speciﬁc features of the IC layout determine its location and its shape replicates a portion of the layout geometry.


Another important category of deformations worth highlighting contains scratches of various kinds (e.g., Figs.5c and d),which also have characteristics very different from the typical spot defect. This is especially true for scratches generated by Chemical-Mechanical Polishing (CMP) techniques. And scratches may be of various sizes, usually causing the whole spectrum of shorts and opens.


Finally, one should mention large size deformations. They introduce opens and shorts to larger number of IC nets and,therefore, may cause complex circuit behavior. They may also have very complex forms and shapes (see examples in Fig. 3c and Figs. 5e and f). For a more elaborate discussion see [3].


Taxonomy of Deformations


The taxonomy proposed in this paper begins with the distinction between boundless and bounded deformations.  On the one hand, we use the term boundless to describe deformations


(such as oxide thickness shown in Fig. 1) whose only boundary is the edge of the silicon wafer.  (These deformations mostly contribute to parametric yield loss.) On the other hand,bounded deformations have a clearly deﬁned boundary inside the wafer area.


We propose for boundless deformations a methodology to describe the magnitude of the deformation as a function of the wafer coordinates.  We assume for bounded deformations that the magnitude is large enough to cause circuit malfunction and we focus on the geometry of its boundary. In the following two subsections we describe both categories of deformations in more detail.


Boundless Deformations


As was mentioned in the introduction, the key objective for the adequate description of IC structure deformations is to capture the set of deformations' characteristics that is sufﬁcient for estimation of probability of IC failure and this way for obtaining yield, escape-levels and reliability estimates. In the case of boundless deformations such a characteristic would be the information about the magnitude of the deviation of the value of an IC layer parameter with respect to the value of this parameter used in the design speciﬁcation. Ultimately, the value of the deviation must be known as precisely as possible for all locations (i.e., x,y coordinates) of fabricated wafers.


Hence, we propose that each boundless deformation is seen as a two-dimensional stochastic process.  Realizations of such a random process deﬁne the spatial distribution of a parameter of interest on the IC manufacturing wafer. Each such realization can be modeled as a sum of spatially periodic functions.  Each function can mimic the impact of a speciﬁc subset of processing steps (e.g., lithography, implant etc.).


Hence, the essential feature of the above approach is that in the proposed conceptual model a deformation is seen as a sum of periodic functions with a large spectrum of spatial frequencies and all having radial or x-y periodicity. Fig. 6 illustrates this using a sequence of wafer maps. Each map depicts the extent of a boundless deformation by using different shades of colors.


Fig. 6a shows the wafer map of a deformation as the circuit designer sees it. It is also shown here that the design process acknowledges a certain amount (+10% - 10%) of deviation of this parameter as acceptable. Figs. 6b and c show examples of two different realizations of a portion of the stochastic process that mimics "spatially slow" phenomena. Fig. 6d is the result of adding the deformation of wafer in Fig. 6c with the deformation extent that mimics a set of processing steps having tendency for radial symmetry in the distribution of the parameter of interest. Figs. 6e, f, and g show how the distribution of the parameter shown in Fig. 6d may be modiﬁed by subsequent lithography steps having periodicity corresponding to  reticle or die size. Fig. 6h shows the cumulative effect of the entire process as a wafer map. This ﬁnal summation determines the behavior of the fabricated circuit. It must be stressed here that this map represents only one hypothetical wafer and that it illustrates one speciﬁc realization of a stochastic process. This implies that the information which is necessary for fault probability estimation must include complete statistical characterization of this process which should include wafer maps of mean value and standard deviation (shown in Figs. 6i and j) as well as appropriate autocorrelation functions.


To assess the utility of the proposed model for boundless deformations, one should study at least two of its aspects: methodology of its application in fault probability calculation and feasibility of identiﬁcation of parameters of modeled stochastic


processes. However, a presentation of such a study is beyond the scope of this paper. We can only provide here some initial view, illustrated in Fig. 7. The wafer maps in Figs. 7a, b, c and d summarize the key elements of the envisioned yield estimation methodology. The most difﬁcult yet key step of this methodology is the transition of a wafer deformation map (Fig. 7a)into the map of "unacceptable deformations" (marked in black on wafer map in Fig. 7b). Next, a wafer map with unacceptable regions may be matched with a "die map" (Fig 7c).  Each die that contains within its boundary an unacceptable region can be marked as faulty (marked in Fig. 7c with a red cross). Of course, to obtain the desired yield map (Fig. 7d.) one has to repeat the above sequence of steps for many wafer maps generated by all relevant stochastic processes.


Second important use is the identiﬁcation of parameters controlling stochastic processes of interest. In this case, as of today, the main problem is deformation observability. The crux of this problem is illustrated with Figs. 7a, e, f, and g. It is caused by the frequency of "spatial sampling" of the deformation of interest. Simply, deformation maps such as shown in Fig. 7a are not available for wafers with real products. What may be available are maps such as maps shown in Figs. 7e, f and g, i.e., low-resolution maps obtained from sparsely distributed test structures. As is indicated by Figs. 7e, f and g, such maps do not provide a good enough resolution.


Finally, it is useful to notice that the above difﬁculty is derived from the features of the proposed modeling methodology. It is simply a direct consequence of the fact that higher spatial-frequency deformations become relevant as far as fault probability is concerned


Bounded Deformations


As was mentioned before, we are assuming for bounded deformations that the extent of deformation is "fatal" so that the only important characteristic of such a deformation is the geometry of its boundary. However, a complete description of the boundary would be very costly if not unmanageable.  Therefore, the taxonomy proposed below attempts to capture all essential characteristics of the geometry of the boundary and, at the same time, to minimize the amount of data that needs to be stored and processed when interaction between layout and the deformation is assessed.


The ﬁrst set of features that our approach focuses on are graphically described in Fig. 8. The characteristics of interest are:Composition of a deformation (nature of the deformation’s fragmentation), which includes number of deformation segments and distribution of the components' centers. An attempt is also made to distinguish between characteristics of boundaries of majority of deformations’ components (mostly-concave or mostly-convex). Hence, an attempt is made to project multiple attributes into the 2-dimensional drawing plane.  To accomplish this, a diverse set of deformations is arranged in a circle and we use the "time-of-day" as the coordinates. This"deformation clock" allows a compact description of diverse attributes, such as the distribution of deformation centers, the components' shapes, the deformation components-to-outline area ratios, and the number of components.  We use the ﬁrst 12 hours, "a.m.", for additive interaction (left column in Fig. 9)and the second 12 hours, "p.m.", for subtractive interaction(right column in Fig. 9).


For example, "5:30 pm" represents a defect with extra material that has a low number of components whose centers are randomly distributed and whose areas add up to little less than the area of the minimum enclosing circle. At 6 o'clock is the tradi224


tional "perfect" spot defect, circular in shape (6 a.m represents extra material while 6 p.m represents missing material).  Diametrically opposed, 12 noon or 12 midnight represents the absence of a defect. In between these two extremes lie the many variations with increasing number and increasing complexity of shapes of components.


One can see, however, that the taxonomy proposed in Figs. 8 and 9 may be sometimes not sufﬁcient or complete. It was presented here mainly as a device to communicate, in a possibly imperfect but simple way, deformation characteristics (and maybe also as a uniﬁcation and simpliﬁcation of the FA language).


The deformation can be composed of one or many components of various shapes and sizes (see Figs. 3-5).  Fig. 10 illustrates a progression of changing number of components (nc) and number of boundaries (nb).  In the top-left corner is a traditional spot defect and in the bottom-right is an example of a cluster of deformation components.  The ratio between the perimeter and the area of the deformation increases with the number of components.


Fig. 11 presents two alternatives to capture the complex shapes and outlines of deformations. The top row uses minimum enclosing circles (MEC), while the middle row uses minimum enclosing rectangles (MER).  The bottom row compares these two possibilities.  One attribute is the ratio between the deformation area and the area of the enclosing circle (or rectangle).


As another attribute, the ratio of the area of the minimum enclosing circle to the area of the minimum enclosing rectangle characterizes the difference, e.g., between a spot defect (ratio smaller than 1) and a scratch-like defect (ratio larger than 1).


Fig. 13 presents the deformation characterization ﬂow that is the core of our proposed taxonomy.  The various attributes mentioned in the previous paragraphs are listed here and provide a systematic way of describing deformations of IC structures. For the outline of a deformation composed of one or multiple components, Fig. 13a contains the attributes to describe geometrical and spatial properties.  Fig. 13b then zooms into the individual components of the deformation region.


Common to boundless and bounded deformations is the question about the affected layer or layers. In the case of a boundless, continuous spatial distribution of the deformation, the methodology of describing the deformation magnitude as a sum of periodic functions as previously discussed applies from here on.  For bounded deformations, a number of questions must be answered related to the outline of the deformation (or deformation components). We require the distribution of the centers of the deformation outline, the distribution of the ratio of the deformation area to the outline area, the shape distribution, the orientation distribution, and the distribution of the outline size. Some of these properties lead directly to a dependence on the layout and wafer coordinates since the interplay between layout and deformation determines the actual electrical consequence and possible yield loss. Some simpliﬁcations are possible since, for example, a circular deformation requires no description of its orientation.


Our taxonomy allows for a hierarchical description of deformations with multiple components.  As Fig. 13b shows, the distributions of the individual components are also relevant.  In the case of a deformation with many components, our taxonomy includes the distribution of the centers of the components.


The next steps are similar to Fig. 13a, but instead of the outline,


the distributions of the shapes, orientations and sizes of the components are collected.


In this paper,  we proposed a taxonomy of process-induced deformations of IC structures. This proposal should be seen as a ﬁrst step towards a rapidly emerging need for a “compact”description of geometrical attributes of deformations of modern IC structures.


The authors would like to thank the GSRC for ﬁnancial support.


1. W. Maly et. al., Deformations of IC Structure in Test


and Yield Learning, IEEE International Test


Conference, (2003).


2. W. Maly, 18-764 Lecture Notes, ECE Dept. Carnegie


Mellon University, Fall 2002.


3. T. Zanon et. al., Analysis of IC Manufacturing Process


Deformations: An Automated Approach Using SRAM


Bit Fail Maps, International Symposium for Testing and


Failure Analysis, (2003).


Deformed region: Incompletely exposed photoresist


Aluminum Lines Contamination Deformed region: Metal Bridge


Aluminum lines


Deformed region


Active regions


LOCOS Deformed region: Unwanted active


Active region LOCOS


Deformed region: Unwanted active


Active lines


Deformed region: Unetched spacer oxide


Unetched aluminum


Contamination


Cause: Too narrow gap between layout features EC: Undetermined


Layer(s) involved: Photoresist


Kind of image:


Source:


Philips


Description:


Due to high


ratio of the


photoresist


height to the


distance


between


adjacent layout features portion of photoresist


has been


under exposed.


Cause: Imperfect cleaning after litho


EC: Two-node bridge


Layer(s) involved: Photoresist and aluminum


Particle of


has obstructed etching of


metal.


Cause: Unknown particle obstructing exposure of photoresist


EC: Bridge of many adjacent lines in bus


Author's arch.


Shade of a


flake of some kind engraved in aluminum layer.


Cause: A particle obstructing nitride etching


EC: Complex network of active and passive devices Layer(s) involved: LOCOS process nitride active mask


Kind of image:Optical


A flake of


unknown


material


prevented


removal of


nitride layer during nitride dry etching -picture taken after field


oxidation.


Optical


nitride layer


during nitride dry etching -picture taken after poly and contacts litho.


Cause: A particle obstructing spacer oxide etching EC: Affected transistors quality/functionality


Layer(s) involved: Spacer oxide


spacer oxide.


Cause: Too short metal etching time EC: Two "two-line resistive bridges"Layer(s) involved: Aluminum


Thin film of


aluminum


remains on the oxide surface and forms


current path


adjacent metal regions.


Cause: Tungsten particle


EC: "Four-line bridge"


Tungsten particle


deposited on Al layer before


photoresist spin.


a.


b.


c.


d.


e.


f.


g.


h.


Figure 3. Collection of bounded deformations: Part 1.


Aluminum Contamination


Poly bit bit-bar lines Contamination


Edge of deformed poly region


Metal "N-1" - Aluminum


Metal "N" - Aluminum


Aluminum stringer


Cause: Tungsten contamination deposited on aluminum EC: "Seven-line bridge"


Flake of


tungsten has


accumulated


thick layer of


which could


not be fully


exposed and


then developed.


Cause: Large particle


EC: "Multiple line bridge"


material has


been deposited on Al layer


before


photoresist spin causing increase in photoresist


thickness.


Cause: Flake of Tungsten


EC: Complex parasitic transistors with shorted inputs (four)Layer(s) involved: Active, poly and photoresist


Tilted SEM


Tungsten


particle


deposited on top of poly


before poly litho -


shown after poly etch.


Cause: Mis-processed Spin On Glass (SOG) layer


EC: "Multi node bridges" in metal "N"


Layer(s) involved: Metal "N-1" , TEOS, SOG and Metal "N"


For specific


geometry in


metal "N-1"


surface of


deposition of


metal "N" has


deep grooves in which


unremoved


metal "N" forms stringers.


Cause: Electromigration


EC: "Partial Open" and "Increased Resistance"Layer(s) involved: Aluminum


Due to grains in aluminum and high


density of


from the side grain was


"blown away"by electrons.


Cause: Unknown


EC: One line open and increased resistance in other Layer(s) involved: Photoresist and aluminum


Undetermined contamination caused


overetching


of aluminum


in its


neighborhood.


EC: "Open" in 2 lines


Photoresist developed in deformed


despite


ignoring


"exposed"


pattern.


Figure 4. Collection of bounded deformations: Part 2.


Gate oxide Pinhole Edges of removed poly Removed field oxide


Aluminum bus


Deformed passivation region


Cause: Stress in gate oxide


EC: Leaky capacitor , deformed transistor characteristics Layer(s) involved: Gate oxide


Mechanical


stress caused weak point


(conductive


path) in gate


oxide which


then resulted in high density current that


eventually


malted away


gate oxide.


Cause: Contaminated photoresist


EC: "7 lines open" and "Increased Resistance" in 3 lines Layer(s) involved: Photoresist and aluminum


Interaction


contamination and photoresist caused


development


of unexposed photoresist.


Cause: Wafer handling


EC: Complex network of opens and shorts Layer(s) involved: Aluminum


Scratch in


that happened after


etching.


EC: Complex network of opens and shorts Layer(s) involved: Photoresist and aluminum


that happened after resist


development and before


Cause: Tungsten contamination deposited on aluminum EC: Complex network of opens and shorts


tungsten has accumulated thick layer of photoresist


which could not be fully


exposed and then


developed.


Cause: Not investigated


EC: Undetected


Layer(s) involved: Passivation


Large size


deformation caused


probably by a liquid agent during wafer handing.


Cause: Uncertain


Unharmful cosmetic or maybe reliability problem.


Cause: Deposited from the air in the processing chamber EC: Undetected


Not harmful cosmetic


problem.


Figure 5. Collection of bounded deformations: Part 3.


5%10%15%20%


-25%-30%


-20%-15%-10%-5%


Design


Maximum


Nominal


Minimum


i.


0 5%10%15%20%


j.


Figure 6.


Reality


Design assumption


60%


70%80%90%100%


10%


0%


20%30%40%50%


Yield


Un


acceptable


-25%


Figure 7.


Concave


Convex


Distribution of components centers


Gaussian


Uniform


Components shapes


XII


VI


IV


I


VII XI


II


VIII X


IX


III


5:30 PM


MEC


MER


MEC MER


Ad14/Ao14 =.01pr2/pr2 = .01


Ad13/Ao13 =.15pr2/pr2 = .15


Ad12/Ao12 =.5pr2/pr2 = .5


Ad11/Ao11 =pr2/pr2 = 1


Ad24/Ao24 =.01pr2/r2 = .0314


Ad23/Ao23 =


.15pr2/.5r2 = .942


Ad22/Ao22 =


.5pr2/2.4r2 = .654


Ad21/Ao21 =


pr2/4r2 = .785


Ao11/Ao21= .785


Ao12/Ao22 = 1.308


Ao13/Ao23 = 6.28


Ao14/Ao24 = 3.14


12:00


1:00


2:00


3:00


4:00


5:00


6:00


11:00


10:00


9:00


8:00


PM


Cr11 = Pd/Ad = 2/r


Cr12 > Cr11


Cr13 > Cr12 > Cr11


Cr14 >> Cr13


nc = 1


nc =1


nb = 1


nb =1


Cr21 > Cr11


Cr22 > Cr12 > Cr21


Cr23 > Cr13 > Cr22


nc = 2


nc = 3


nb =4


nb = 6


nb = 8


Cr31 > Cr21 > Cr11


Cr32 > Cr31


Cr33 > Cr32 > Cr31


Cr14 < Cr24


nc =5


nc = 7


nc = 26


nb = 3


nb =6


nb = 7


nb = 26


Cr24 >> Cr23


Distribution of Deformation Magnitude


Affected Layer(s)


Nature of Deformation


Spatial Distribution of the Deformation


Distribution of Centers of Deformations Outlines


Shape Distribution


Shapes of Deformations Outline


Deformations Outline Size Distribution


Deformation "Outline Area" to "Deformation's Area" Ratio Distribution


Orientation Distribution


Orientation of Deformations Outline


BINARY


CONTINUOUS


BOUNDED


WAFER DEPENDENT


UNIFORM


CO-ORDINATES DEPENDENT


CO-ORDINATES INDEPENDENT


LAYOUT DEPENDENT


LAYOUT INDEPENDENT


BOUNDLESS


MULTI-LAYER


SINGLE-LAYER


VARIABLE


"6 O'CLOCK"


RELEVANT


IRRELEVANT


MORE THAN ONE


ONE


MANY


IDENTICAL


Number of Deformation Components


Distribution of Components Centers


Shapes of Deformation Components


Size Distribution


Orientations of Deformation Components


Size of Deformation Components


Figure 8.


Figure 9.


Figure 12.


Figure 10.


Figure 11.


Figure 13.


[x0,y0]


a0


Rb


A9


A10


nc= 11


Ra


231


p 232-241


DOI: 10.1361/cp2003istfa232


## Analysis of IC Manufacturing Process Deformations: An Automated Approach Using SRAM Bit Fail Maps


Analysis of IC Manufacturing Process Deformations: An Automated Approach Using SRAM Bit Fail Maps


T. Zanon, M. Ferdman, K. Komeyli*, and W. Maly  Carnegie Mellon University, Pittsburgh, PA, USA


* Intel Corporation, Santa Clara, CA, USA


SRAM bit fail maps (BFM) are routinely collected during


earlier phases of yield ramping, providing a rich source of  information for IC failure and deformation learning. In this


paper, we present an automated approach to analyzing BFM  data efficiently. We also demonstrate the usability of our  analysis framework using real BFM test data from a large, modern SRAM test vehicle.


To facilitate the discussion, we first present important terms  used extensively throughout this paper.


Terminology


• A deformation is a difference between the IC structure of the


fabricated device and the desired structure of the nominal


device.


• A deforming event is the deviation from nominal


manufacturing conditions resulting in an IC deformation.


• A failure is the manifestation or impact of a deformation on


the behavior of a fabricated IC, detectable at test.


• A bit fail map (BFM) is a matrix of 0s and 1s describing


passing and failing SRAM cells at test (see Figure 1).


• A colored bit fail map is a bit fail map with additional


information about the way a SRAM cell failed during test. Bit


fail map cells are colored based on this information.


• A failure pattern instance (FPI) is a group of failing SRAM


cells attributed to the same deforming event.


• A failure pattern type (FPT) represents a set of similar failure


pattern instances (e.g., there is only one single-bit FPT, but


many single-bit FPIs in a test data set).


• A Euclidean minimum spanning tree (EMST) is the minimum


length acyclic graph G connecting all vertices of a set V (see


Figure 3b) [1,2].


• An artificial neural network (ANN) is a mathematical model


that emulates some of the observed properties of biological


nervous systems and draws on the analogies of adaptive


biological learning. Thus, neural networks are very suitable for


learning interrelations in complex data (e.g., complex FPIs) [3].


Application of SRAM bit fail maps in new technologies


SRAM bit fail maps have been successfully used in addressing a  number of major tasks in semiconductor manufacturing such as  process control monitoring, defect monitoring, and many others  in the yield improvement domain [4,5,6,7]. There are, however, three important issues that are becoming stumbling blocks to  using SRAM bit fail maps for analysis of the newest IC  technologies. First, the volume of bit fail maps harvested during  manufacturing of moderns ICs is overwhelming, especially in  the starting phase of yield ramping. Second, a significant  percentage of large modern memory devices are affected by  multiple independent deformations on the same die (multiplicity  of deforming events). This is especially true for earlier stages of  the product cycle, where the assumption of having a single spot  defect [6] per die does not hold at all. Third, many failure  patterns in modern SRAMs are geometrically very complex and  expected to become even more complex in future due to more  sophisticated manufacturing processes (IC failure-layout  interaction).


Consequently, new techniques that could effectively assist yield  improvement tasks are likely to become indispensable for any  modern IC manufacturing operation.


~ 4600 SRAM Cells


Figure 1: SRAM bit fail map showing a large deformation. Black dots represent SRAM cells that failed at test.


Objective of the paper


This paper describes one possible approach to address the above  stated goal of research oriented towards yield improvement. The  approach presented in this paper focuses on an automated  analysis of SRAM bit fail maps to enable fast yield learning  from a large volume of potentially highly complex BFMs found  in modern SRAM devices.


The paper is organized as follows: First, a software framework  that enables automated analysis of bit fail maps is introduced. Then, fundamental assumptions used in the development of the  framework are assessed using bit fail map data from a large, modern SRAM test vehicle. Finally, potential failure analysis  applications (e.g., Pareto chart analysis and deformation  analysis) that benefit from the use of the presented automated  BFM analysis approach are discussed.


SRAM bit fail map analysis approach


To address the need for SRAM bit fail map analysis defined in  the introduction, a set of software utilities for processing BFM  data has been developed. In this section, an overview of the  algorithms embedded in this software as well as the framework  organizing interactions between various BFM analysis software  components is provided. The flow diagram of this framework is  shown in Figure 2. Key functions performed by the major  components of the software framework are:


1. Segmentation of bit fail maps into failure pattern instances (FPI). Multiple IC structure deforming events that may be  present on a single die are separated into individual FPIs.


2. Extraction of basic characteristics of failure pattern  instances. Complexity of the description of failure patterns  instances (FPI representation) is reduced.


3. Clustering of failure patterns instances with similar  characteristics into failure pattern types (FPT). FPIs are grouped  into FPTs based on the similarity of FPI characteristics.


Details of the implementation of each of these three key  functions are described below.


Bit fail map data pre-processing


In general, bit fail maps consist of matrices of 0s and 1s  describing the pass/fail state of each tested SRAM cell. The  amount of data that has to be stored for SRAM devices with  large number of failing cells is significant. Further, any  processing of BFM data in their raw format is computationally  very inefficient and impractical. Therefore, all raw bit fail maps  are initially compressed using a data reduction algorithm that  combines neighboring failing cells into rectangular fail regions. These fail regions are then stored in a database (here: PostgreSQL [8]) for further analysis.


Segmentation of bit fail maps


Experience shows that in modern manufacturing processes a  significant number of bit fail maps are likely to be affected by  more than one deforming event. This is especially pronounced  during yield ramping. Furthermore, it is possible that some bit  fail maps consist of many individual fail regions, which are


actually caused by the same deforming event. An example is  illustrated in Figure 1. A large number of single and double-bit  failures in this die were evidenty caused by the same deforming  event. The ultimate objective of segmentation is to identify sets  of SRAM fail regions that are likely caused by a single  deforming event. This means, for example, that all single-bit  and double-bit failures of the large area deformation in Figure 1  are grouped into a single failure pattern instance.


A divisive clustering technique [9] to separate fail regions into  failure pattern instances is used. In order to perform  segmentation, the algorithm examines the relationships between  fail regions and uses four empirically determined parameters to  decide whether a set of fail regions should belong to the same  FPI. In a divisive clustering approach, all fail regions are first  considered to belong to one FPI. This failure pattern instance is  then iteratively split into smaller ones, as long as the overall  quality of the segmentation improves. The procedure terminates  when no further improvement can be achieved by splitting any  of the resulting FPIs.


The algorithm begins from a bit fail map of fail regions (Figure  3a). First, a Euclidean minimum spanning tree (EMST) connecting all fail regions (EMST vertices) on a die is created. The distance between the closest points of the fail regions  determines the edges of the EMST (Figure 3b). The EMST  edges are then traversed, starting from the longest edge. Based  on four clustering parameters, each edge is determined to either  span fail regions belonging to the same or two different FPIs. If  the edge is determined to span two FPIs, the edge is cut (a  detailed description of the edge cutting procedure is given  below) and the procedure continues with the next largest edge. If the edge is determined to connect two fail regions within a  single FPI, all fail regions still connected to these two are  considered to belong to the same FPI, and no cuts are made to


Bit  Fail  Maps


Bit Fail Map  Database


Segmentation of Bit Fail Maps


into Failure Pattern Instances


Failure Pattern Instance Clustering  into Failure Pattern Types


Extraction of Basic Failure  Pattern Instance Characteristics


Visual Inspection of


Failure Pattern Types


Applications


Figure 2: Flow diagram of bit fail map analysis framework.


separate them. When no more EMST edges that do not connect


fail regions within a previously determined FPI remain, the


procedure terminates (Figure 3c).


Figure 3d through Figure 3f graphically illustrate how the four  parameters (ν, δ, β and λ), are used to determine whether an  EMST edge connects fail regions in different FPIs. The  parameter ν dictates the smallest number of fail regions that are  necessary for a density metric (number of defective cells divided


by area of a convex hull enclosing these failing cells) to be


valid. If there is a sufficient number of fail regions present on at


least one side of the edge, the densities of the FPIs before and


after cutting are computed (see Dpart1, Dpart2 and Dtotal in Figure  3d). If (1-Dtotal/Dpart1)>δ or (1-Dtotal/Dpart2)>δ, cutting this edge  would “ improve”  (increase) the density of at least one resulting


FPI, and the edge in question is removed from the EMST. If  there are fewer than ν fail regions on at least one side of the  edge with length Ledge considered for cutting, the average  lengths Lavg or Lavg2 of edges spanning from the side of this edge  are computed (average length metric). If (1-Lavg1/Ledge)>β or  (1-Lavg2/Ledge)>β, the edge is cut because this cut would separate  an FPI with significantly shorter edges from a larger FPI (Figure


3e). If only one fail region is present on at least one side of the


edge in question, neither density nor average edge lengths can  be computed for this side of the edge. In this case, the fourth and  last parameter λ is used (distance metric). λ is compared to the  length Ledge of the EMST edge in question, and if the edge is  longer than λ, it is cut (Figure 3f).


Extraction of basic failure pattern characteristics


In order to make failure pattern instances accessible to failure


pattern type instance clustering (the last step of the proposed  analysis approach), their geometric complexity has to be  reduced. Consequently, the main objective of this step is to  extract basic geometric characteristics that represent suitable  building blocks for a simplified description of failure pattern  instances.


The FPI characterization approach adopted in this research is  related to previous work on bit fail map analysis reported in [10] and on defect shape analysis for computer vision applications


[11]. The key idea is to describe any geometric pattern by very  intuitive and simplified characteristics (note the fundamental  difference to approaches based on more complex and less  intuitive characteristics using, e.g., statistical moments [12] or  Fourier coefficients) In this research, these ideas were modified  and extended to accommodate for the intricate failure patterns  encountered in the available SRAM test vehicle. A detailed  discussion of the basic FPI characteristics that are considered  very promising candidates for adequate simplified  characterization of FPIs follows in the remainder of this section.


Inspection of failure pattern instances showed that many failure  pattern instances do not adequately represent the shape of the  underlying deformation. In these cases, the observed failure  pattern instance is a response to both the deformation and the  layout of the SRAM test vehicle (in general, the word-line and  bit-line structure of a memory). As can be seen in the example  in Figure 4, consideration of the entire failure pattern instance  strongly misrepresents the actual deformation. Consequently, the decision was made to identify and differentiate these layoutinduced failure components from the remaining failure  components of an FPI. These layout-induced components are  referred to as gray-colored failure components (see Figure 4). The remaining black-colored components now serve as a much  better representation of the actual area of deformation. Nevertheless, the gray-colored failure components should not be  regarded as useless. The strong relationship of the gray-colored  components to the SRAM layout points to specific metal layers  and makes the gray-colored components a valuable means for  pinpointing a potentially defective manufacturing step. Graycolored failure components are used as basic characteristics of  an FPI. In particular, the following three Boolean characteristics


c


f


δ - Density Metric ν≥5


β - Avg. Length


Metric


λ - Distance  Metric


EMST Edges  Fail  Regions


FPIs after  Segmentation


Convex  Hulls


EMST


Dpart2


Dtotal


Lavg1


Lavg2


Ledge


Figure 3: EMST-based bit fail map segmentation into FPIs. The  original multi-deformation bit fail map is depicted in a), the  resulting segmentation is shown in c). Details of the  segmentation procedure are illustrated in d) through f).


Actual Region of


Deformation


Layout-Induced “ A rti f icial


Deformations”


(Bit-L ines &  Word-L ines) Fai lure Pattern


Instance (FPI)


Figure 4: Examples of SRAM failure pattern instance where the  inclusion of layout-induced (gray) failure components strongly  misrepresents the underlying deformed memory region.


are used: 1) gray-vertical, 2) gray-horizontal, and 3) gray-block, indicating an FPI with at least one vertical, horizontal, or entire  SRAM block layout-induced failure component.


Appropriate FPI characteristics are needed to convey the notion  of area of a deformed SRAM region. The area of a convex hull  appears to be a suitable indicator of the deformed area. Thus, convex hull areas of failure pattern instances before and after “removal”  of layout-induced gray-colored failure components (see original and removed convex hulls in Figure 5) are  computed and used as basic FPI characteristics.


Although the knowledge of gray-colored failure components  and the area of deformed regions provide considerable  information for failure and deformation analysis, it was found  experimentally that additional characteristics are required for  proper description of many failure pattern instances. Important  FPI characteristics are (this list is by no means exhaustive): extent, aspect ratio, principal direction, defective cell density  within the deformed region and closeness of the shape of a  deformed region to a perfect circle. Some of these  characteristics can be derived from more fundamental ones (e.g., the aspect ratio of a deformed region can be described by the  ratio of length to width of the deformed region). For the purpose  of the research presented in this paper, it was found that the  extraction of only three additional, relatively simple geometric  features is sufficient to characterize the majority of encountered  failure pattern instances according to the above-mentioned list  of important characteristics. These geometric features are: 1) the  minimum enclosing circle (MEC), 2) the minimum enclosing  rectangle (MER), and 3) the total number of failing SRAM cells


of the deformed SRAM region. These geometric features  including convex hulls are illustrated in Figure 5. The FPIs in  this figure also demonstrate the focus of the proposed  characterization approach on the underlying deformation of a  failure pattern instance. If a failure pattern instance has any  black-colored failure components, only these components are  considered for the MEC and MER computation (see Figure 5a  and b). On the other hand, if the entire FPI consists of graycolored failure components only (see Figure 5c), computation of  geometric features is based on the gray failure components to  improve the clustering quality of such failure pattern instances.


A summary of how the basic characteristics can be utilized is  given in Table 1. Of course, we do not claim that this list of  basic geometric characteristics covers every single aspect of  failure pattern instance description, but the selected set works  extremely well with our data sets.


Clustering of failure pattern instances


Once all bit fail maps have been successfully segmented into  failure pattern instances and described using a suitable set of  simple FPI characteristics, interesting observations can be made  based on this representation of failure pattern instances (see  experiment and application sections). However, many useful bit  fail map analysis applications (e.g., generation of failure pattern  type Pareto charts) require failure pattern instances to be  clustered into unique groups. These groups of failure pattern  instances are called failure pattern types (FPT). The large  number of failure pattern instances hinders manual clustering or  at the very least makes manual clustering a time-consuming and  error-prone task. Consequently, the main objective of the final  step of the proposed analysis approach is to automatically  cluster FPIs into appropriate FPTs.


Random inspection of failure pattern instances from available  SRAM test data sets has shown that a significant portion of the  FPTs would not have been anticipated. Hence, any knowledgebased [14,15] clustering approach would have generated a very  large bin of unknown failure pattern instances (FPIs not  assigned to any particular FPT). A large bin of “unknowns”


Table 1: Extracted basic FPI characteristics.


Extracted basic


FPI characteristic


Potential use


Gray-horizontal  Gray-vertical  Gray-block


Diagnosis of defective manufacturing  step; emphasis on deformation


Area of original and  removed hulls


Area of the deformed region; Defective cell density


MEC radius  MEC center


Extent of deformed region; location of  deformed region on die; closeness to  circle (e.g., traditional circular spot  defect)


MER length  MER width  MER tilt


Alignment and approximate size of  deformed region; aspect ratio (e.g., straight scratch detection)


Defective cell count Defective cell density; texture of


deformed region


Removed Convex Hull


Original Convex Hull


Min Enclosing  Rectangle (MER) Tilt


Min Enclosing  Circle (MEC)


a)


b)


c)


Figure 5: Geometric features used for simplified description of  failure pattern instances and deformations. Examples show  failure pattern instances with a) black-colored only, b) black  and gray-colored, and c) gray-colored only failure components. The geometric features are computed using the Computational  Geometry Algorithms Library CGAL [13] .


corresponds to a tedious inspection process of each failure  pattern instance in this bin. Consequently, a clustering approach  was needed that does not require any a-priori knowledge of  potential clusters in the input data space (here: the space of  characterized FPIs). One clustering technique that meets this  requirement is based on growing hierarchical self-organizing  maps (GHSOM) [16,17,18], a particular type of unsupervised  artificial neural networks. GHSOM-based clustering is a  completely input data-driven procedure. Hence, clusters in the  space of failure pattern instances are extracted without any  specific structural knowledge of this space and without any  external interaction throughout the entire exploration (clustering) phase. The resolution of clustering, in essence the  desired “crispness”  of extracted failure pattern types, can be  controlled via two parameters τm (breadth growth parameter) and τu (depth growth parameter). Exact definition and use of  these parameters as well as a detailed description of the  operation of the GHSOM clustering procedure is outside the  scope of this paper [17,18]. Here only a brief outline of how  self-organizing maps facilitate failure pattern instance clustering  and how they tie into the presented automated bit fail map  analysis approach is given.


A simplified illustration of the FPI clustering procedure using (GH)SOM networks is depicted in Figure 6. First, all failure  pattern instances to be clustered are described by an appropriate  set of basic and derived characteristics (obtained from the FPI  characterization analysis step). The specific characterization of  each FPI is stored in a SOM input feature vector. Subsequently, the complete sequence of input feature vectors is fed to the  SOM learning algorithm (usually several times). An SOM  neural network consists of neurons organized on a regular, usually rectangular, two-dimensional grid. The core of each  neuron is a prototype vector, which is of the same dimension as  the input feature vector. During learning, the prototype vectors  of neurons are affected not only by the stream of input feature  vectors but also by changes of the prototype vectors of  neighboring neurons in the map. At the end of the training, the  prototype vectors of all neurons in the SOM have organized  themselves such that prototype vectors close in the input feature  space (here: vector of FPI characteristics) are spatially close in


the SOM network, which explains the name “self-organizing” . At this stage, each failure pattern instance can be assigned to  exactly one neuron (the neuron having a prototype feature  vector closest to the vector of the FPI) and each neuron  represents a failure pattern type. Consequently, we have  obtained a clustering of failure pattern instances into failure  pattern types. The key characteristics of the failure pattern type  are reflected in the respective prototype vector of its  corresponding neuron.


Experimental verification of framework operation


To assess the correctness of principles guiding the development  of the presented three-step SRAM BFM analysis framework, extensive experiments on a large set of real BFM test data from  large, modern SRAM products were conducted. Key results of  this experiment are reported in the following subsections.


SRAM test vehicle and test data statistics


The test vehicle used for this research is a relatively large static  memory device (256K x 72) manufactured in a six-metal


0.13µm Leff process technology. Memory devices of this size  consist in general of two or more hierarchy levels of sense  amplifier and word access control. For this research, word or  bit-lines in the first level of hierarchy are called local and those  in all higher levels of hierarchy are referred to as global. This  SRAM property was extensively used for failure pattern  characterization (gray-colored failure component). Test data was  collected from wafers with two different SRAM cell layouts (manufactured in alternating wafer columns) as well as from  two slightly different processes (test data set A and B). To  demonstrate the usefulness of the proposed framework without  making the procedure overly complicated, BFM analysis in this  experiment was based on test data from functional fail testing  only. Functional fail testing of the SRAM is carried out at  minimum acceptable power supply voltage and nominal clock  frequency using an appropriate test algorithm. All failure  information was obtained in the previously described format of  fail region. Table 2 summarizes the basic test data statistics.


As previously mentioned, many large SRAM devices fabricated  in modern process technologies may be affected by multiple  deforming events. After inspection of over 1000 randomly  selected SRAM bit fail maps from both test data sets, it was  concluded that the proposed failure pattern instance  segmentation step is imperative for proper analysis of bit fail  maps.


SOM-based Failure Pattern Clustering


Neurons = FPTs  Characterization of


Failure Pattern Instances: Input Feature Vectors


Failure Pattern Instances


Figure 6: Illustration of FPI clustering using SOM networks.


Table 2: Statistics of the collected test data. The gray boxes  highlight the number of SRAMs analyzed in this experiment.


Data set A Data set B


Wafers


453


439


Dies


46,280


46,156


Total


Fail regions


6,385,984 3,737,521


22,966


19,036


Functional fail  test only


5,508,208 2,922,258


Segmentation of bit fail maps is controlled by a set of four  parameters ν, δ, β and λ as described in detail in the previous  section. In the current stage of research, a suitable set of  parameters has to be determined by application of a number of  different parameter sets to a reasonably large and representative  number of SRAM bit fail maps with subsequent visual  inspection of the quality of the segmentation results. Extensive  segmentation experiments were conducted on over 1000 SRAM  bit maps randomly selected for visual inspection. Finally, the  parameter set leading to the highest quality segmentation results  was chosen as the parameter set for subsequent segmentation  experiments on all available dies (from functional fail test). The  values of the parameters selected are listed in Table 3.


Subsequently, segmentation experiments were conducted on  both test data sets. The number of failure pattern instances  extracted was 38,368 and 28,879, respectively. Inspection of  several hundred segmented bit fail maps again confirmed the  appropriateness of the chosen segmentation parameter set. The  number of extracted failure patterns instances clearly indicates  that large, modern SRAM devices are affected on average by  more than one deforming event per die. Comparing the number  of total extracted FPIs to the number of dies processed results in  an average of 1.58 FPI/die and 1.51 FPI/die for test data set A  and B, respectively. These results clearly demonstrate the  necessity of a BFM segmentation step for large modern memory  devices. According to the histogram shown in Figure 7, the bit  fail maps of 60-65% of the analyzed die can be explained by a  single failure pattern instance (potential occurrence of a single  deforming event). A significant portion of more than 30% of the  bit fail maps have multiple failure pattern instances and  therefore cannot be represented by any model based on the  assumption of single defect occurrence (e.g., traditional spot  defect model). This is a key observation that must be considered  for many tasks in IC fabrication (e.g., test generation or  redundancy design for yield improvement).


Once the SRAM bit fail maps from the collected test data sets


were segmented into failure pattern instances and simple and  intuitive primary geometric features were computed for each  FPI, the proposed GHSOM-based FPI clustering approach could  be carried out to obtain failure pattern types. Clustering of FPIs  in the presented experiments focused predominantly on the size  of deformations. Thus, an appropriate set of characteristics that  meets this requirement was selected (focus on, e.g., shape  requires a different set to work satisfactorily). The complete set  of selected characteristics for the presented experiments is listed  in Table 4.


The GHSOM neural network clustering experiments were  conducted with both available test data sets using the parameters  given in Table 3. These parameters were chosen empirically. However, this selection was not difficult to establish for high  quality clustering Figure 8 shows the hierarchical selforganizing map obtained after learning failure pattern clusters in  test data set A. Each rectangle of this map represents a neuron. A numbered neuron represents a designated failure pattern type (here: 70). The three unnumbered neurons are empty and are not  used as failure pattern types.


Table 3: Parameters used for the experiments described in this  section.


Parameters for segmentation of bit fail maps ν Min. number of fail region for density metric


δ Density metric threshold


0.94


β Average length metric threshold


λ Distance metric threshold


Parameters for failure pattern instance clustering τm GHSOM breadth growth parameter


0.5 τu GHSOM hierarchy depth growth parameter 0.5e-3


0 10 20 30 40 50 60 70


FPIs per Die


Figure 7: Percentage of dies from test data set A (black) and B (gray) versus number of FPIs found per die.


Table 4: FPI characteristics used as components of the input  feature vector for the demonstrated clustering experiment.


Input feature vector  component


Gray-vertical


Gray-horizontal


Gray-block


Boolean; separation of FPI with  various gray failure components


MER tilt


Three-valued parameter; distinction  between word-line, bit-line or no


layout alignment of an FPI


MER length  MER width


Approximate size and shape of FPI


Original & removed  Convex hull areas


Area of deformed region; improved  clustering quality of gray-only FPIs


Defective cell  density


“Texture”  of deformed region


Number of defective  cells


Empirically found to be beneficial for  FPI clustering.


Figure 8: Sample failure pattern type clustering for test data set A. Shown are multiple failure pattern instances for some  FPTs. Simple failure patterns (e.g., Single-Bit [G5] ) as well as more complex deformations (e.g., Small Solid [G6] , Partial  Bit-line [G63] , Full- Die [G12]  and [G47] ) have been successfully identified.


[G4] - 10.3 %


Double-Bit Horizontal


[G6] - 10.3 % Small Solid


[G1] - 1.1 % Block(s)


[G42] - 2.5 % Word-Line


[G10] - 0.4 %


Scratch / Splash-Like


[G5] - 28.5 % Single-Bit


[G63] - 0.27 % Partial Bit-Line


[G12] - 1.3 %


Full-Die


[G16] - 7.7 % Local Bit-Line


[G25] - 0.21 % Cross


[G26] - 0.22 % Cross-Like


[G30] - 0.54 % Global Bit-Line


[G66] - 0.47% Large Complex


[G47] - 0.44%


Full-Die & Gray-Horiz.


Different shades of gray of the boxes indicate different levels (here: four) of hierarchy in the map (with lighter shades  representing deeper levels) and thus different levels in the  failure pattern instance space. Also shown are several  representative failure pattern types that were selected to  highlight the benefits of GHSOM-based clustering for  investigative BFM analysis.


• All major “ crisp”  (identical) and highly frequent FPIs are  reliably assigned to unique FPTs (e.g., single-bit [G5], doublebit horizontal [G4] or local bit-line [G16] failures). Although  similar results for these expected failure pattern instances can be  obtained using a knowledge-based clustering approach, it is still  important to note that a neural network deals with them  appropriately without any additional effort.


• Clustering less frequent similar failure pattern instances  into the same failure pattern type (e.g., global bit-line [G30], partial bit-line [G63], small dense clusters [G6] or word-line [G42] failures) also works extremely well. The failure pattern  instances in these groups, although not identical, appear to share  their “strongest”  characteristic(s) (e.g., gray-vertical in the case  of group [G30]). The clustering behavior of the GHSOM (the  desired level of similarity in the FPIs that fall into a single FPT) can be controlled via the parameters τm and τu.


• Completely unexpected failure pattern instanced (e.g., large  complex failures [G66], which were observed in test data set A, but not in test data set B) are identified and clustered into  meaningful FPTs. Thus, the GHSOM deals with these FPIs  easily without any prior knowledge of their existence. Any  knowledge-based clustering approach would have assigned this  and many other unexpected failure patterns instances to the “unknown”  bin, requiring tedious inspection of many FPIs in  this bin before this FPT is discovered.


• Some initially quite similar looking FPIs with fine  differences are clustered into separate failure pattern type bins. This behavior of the GHSOM potentially increases the  diagnostic capability of BFM analysis. E.g., the full-die failures [G12] and [G47] look very similar at first glance, but upon  closer inspection are separated because of one or more graycolored horizontal failure components in failure pattern  instances of FPT [G47]. Thus, FPT [G47] allows a more  detailed diagnosis of the underlying manufacturing problems.


BFM analysis run-time


The experiments have been conducted on a Sun Sparc Fire 280R  with a 900 MHz CPU and 4 GBytes of RAM. Typical run-times  for each of the three main analysis steps of the framework are  listed in Table 5. Analysis execution times were found to be  reasonably fast, even without code optimization. Especially the


first step of the analysis framework can be expected to become  significantly faster with an optimized implementation of the  EMST algorithm.


Verification experiment - Conclusions


The presented experiment has decisively shown that the  proposed BFM analysis approach can be utilized for efficient  investigations of large sets of complex bit fail maps with  multiple deformation events per die. This is achieved by quickly  and automatically processing bit fail map information and  condensing it to a small number of “ intelligently”  clustered  failure pattern types for further failure analyses and diagnosis. It  was also found that clustering results of excellent quality can be  obtained using simplified characterization of FPIs in  combination with a GHSOM neural network. Finally, the runtime of the software at the current stage of development was  found to be fast enough to perform SRAM BFM analysis of  several hundred of wafers in reasonable time.


We investigated potential failure analysis and diagnosis  applications for IC manufacturing that can benefit from the  proposed SRAM BFM analysis framework. Three example  applications, including preliminary results, are briefly illustrated  in this section.


Building a deformation size portfolio


The extracted FPI characteristics can be directly used to learn  about specific deformation properties using standard statistical  means (e.g., using histograms). An example is shown in Figure  9a. The bubble chart bins the deformed regions from test data  set A according to their length (horizontal axis) and width (vertical axis) (using length and width of the MER). The area of  a bubble represents the number of FPIs in a given bin. The  bubble’s color differentiates FPIs with black-colored failure  components only (black bubbles) and FPIs with at least one  gray-colored failure component (gray bubbles). Two very  distinct observations can be made. First, an obviously large  number of small failure pattern instances exist (black bubbles in  the lower-left corner of graph, representing, e.g., single and  double-bit failures) as well as a quite considerable number of  full-die failures. Second, the impact of the layout-induced  failure components (gray-colored failure components) is  evident. This once again underlines the importance of handling  gray-colored components in a special manner.


Size analysis of deformed regions can be further improved by  taking failure pattern types (FPT) into account. Failure pattern  types were generated according to a variety of FPI  characteristics and potentially represent different deforming  events. Thus, based on FPT information, one can now more  reliably study the approximate size of specific deforming events. Examples are illustrated in Figure 9b. The failure pattern  instances of two FPTs from test data set A were binned  according to their length and width of the deformed region. The  black bubbles represent small solid FPIs ([G6] in Figure 8) as a  likely result of spot defects. The gray bubbles are for slightly  elongated “splash-like”  FPIs with lower defect cell density


Table 5: Analysis run- times for the three main analysis steps.


Step 1:


BFM Segmentation


75 minutes for 10,000 BFM (100  wafers) → 0.45 seconds / BFM


Step 2:


FPI characterization


7 minutes for 10,000 failure pattern  instances → 0.042 seconds / FPI


Step 3:


FPI clustering


< 2 minutes for clustering approx. 30,000 failure pattern instances


[G10] caused by some directional deforming event (e.g., wafer  handling issue).


Generation of failure type Pareto chart


The number of failure pattern types obtained from the presented  analysis framework is reasonably small, therefore enabling  manual inspection and processing of BFM data. Visual  inspection and labeling of failure pattern types has become, although still a human task, relatively simple and manageable. E.g., the generation of a FPT Pareto chart, which is a very  popular failure analysis means, can be achieved in minutes (see  Figure 10). This chart can then be used to support learning of  key yield detractors and to identify particular failure pattern  types for further, more detailed failure analysis (e.g., feeding a  dictionary-based inductive fault analysis with failure patterns  instances that are suitable for such a framework or identifying  large area failures for spatial frequency analysis to learn about  deformation-layout interactions).


Failure pattern type-based process monitoring


A more advanced application that benefits from the proposed


539


10936


2 4 8


64 128 256 512 1024 2048 4096


Length of MER [Cells]


4096 2048 1024 512 256 128


64


678


Figure 9: Bubble charts showing (approximate) sizes and  shapes of deformations (FPI) using the MER information from  the second analysis step. a) FPIs with black-colored failure  components only (black) and FPIs with at least one graycolored failure component (gray); b) Small solid FPIs [G6]  (black) and scratch/splash-like FPIs [G10]  (white).


0 20 40 60 80 100 120


Figure 10: Pareto chart of major failure pattern types (FPT) found in SRAM test data set A.


0 5 10 15 20 25 30 35 40


Wafer Sequence


Figure 11: Plot showing the number of failure pattern instance  of specific failure pattern types per wafer versus the wafer  sequence. FPT dependent excursions can be clearly identified, potentially indicating different root causes of the observed


excursions.


BFM analysis framework is failure pattern type-based process  monitoring for excursion identification or trend analyses. Established means already exist, of course, to catch excursions (e.g., yield monitoring based on e-test and in-line test data). Nevertheless, knowing the predominant failure patterns type(s) during an excursion period could greatly benefit root cause  analysis. Thus, process monitoring based on failure pattern  types extracted by the presented analysis framework can  enhance existing excursion identification practices. An  illustration is given in Figure 11. These plots show the number  of occurrences of selected failure pattern types per wafer with  the wafers arranged in the order of manufacturing. The two  types are: a) low-defective cell density, full-die failures [G12] in  Figure 8 and b) eight-column-wide, long-bit-line fails [G16] of  test data set B. The plots aid in monitoring the respective failure  pattern types over time. Various excursion periods can be easily  spotted and linked to potential root causes. The failure pattern  type in Figure 11a indicates a parametric front-end-issue spread  over the entire wafer (note the different impact of the deforming  event on the two products on the wafer). The failure pattern type  in Figure 11b can most likely be traced back to a sense amplifier  issue, since the eight-column-wide bit-line fails are aligned with  the locations of these circuits in the layout.


In this paper, we presented an automated three-step approach for  the analysis of bit fail maps from modern static memories. Experiments based on real SRAM bit fail map data demonstrate  that the proposed approach can be very beneficial for failure and  deformation learning in any semiconductor manufacturing  operation.


Key observations are:


• A significant portion of modern large SRAMs (and likely  other products) is affected by more than one deforming event.


• A large number of failure pattern types encountered in bit  fail maps of modern static memories exhibit a very complex  nature. This is especially true in the yield ramping phase where  SRAM bit fail map data plays a major role in failure analysis. We found that a neural network approach for SRAM BFM  analysis is extremely beneficial for successful data exploration.


• More comprehensive bit fail map data very likely improves  the diagnostic capabilities and resolution of the SRAM bit fail  map analysis framework. More complete knowledge of failures  and deformations could be established by applying the presented  analysis approach to colored bit fail maps that are colored  according to: a) the failed test, b) the actual steps within a  functional test that failed a cell or c) current measurements of  failing SRAM cells. Investigation of these opportunities, of  course, requires significant support from semiconductor  manufacturers by testing and providing necessary test data.


The authors would like to thank Intel Corporation for providing  valuable data from their SRAM test vehicle for this research as  well as financial assistance. The authors would further like to


thank Alisa Yurovsky for countless hours of software  development, the CMU/CSSI test group for discussions and  Thomas Vogels for his very constructive proofreading.


1. R.L. Graham and P. Hell, On the History of the  Minimum Spanning Tree Problem, Annals of the History  of Computing, 7, 43-57 (1985).


2. J.B. Kruskal, On the Shortest Spanning Tree of a Graph  and the Traveling Salesman Problem, Proc. of the  American Mathematical Society, 7, 48-50 (1956).


3. L. Fausett, Fundamentals of Neural Networks, PrenticeHall, Upper Saddle River, New Jersey (1994).


4. C. H. Stapper, On Yield, Fault Distributions, and  Clustering of Particles, IBM Journal of Research and  Development, 30(3), 326-338 (1986).


5. S. Lopez and D. Bakker, Correlating Defects to Bit Map


Failures Using Automated Patterned Wafer Inspection  Systems, presented at the UltraClean Manufacturing  Symposium, (1992).


6. J. Khare, et.al., Yield-Oriented Computer-Aided Defect  Diagnosis, IEEE Transactions on Semiconductor  Manufacturing, 8(2), 195-206 (1995).


7. J. Khare and W. Maly, Contamination Diagnosis Using  Contamination-Defect_Fault (CDF) Simulation, Proc.


of International Symposium for Testing and Failure  Analysis, 109-114 (1996)


8. PostgreSQL User’s Guide, http://www.postgresql.org.


9. R.O. Duda and P.E. Hart, Pattern Classification and  Scene Analysis, Wiley-Interscience, New York (1973).


10. R.S. Collica, et.al., SRAM bitmap Shape Recognition  and Sorting Using Neural Networks, IEEE Transactions  on Semiconductor Manufacturing, 8(3), 326-334 (1995).


11. M. Peura and J.Iivarinen, Efficiency of Simple Shape  Descriptors, 3rd International Workshop on Aspects in  Visual Forms, 443-51, (1997).


12. S.S. Gleason, et.al., Rapid Yield Learning through  Optical Defect and Electrical Test Analysis, SPIE’s


International Symposium on Metrology, Inspection, and  Process Control for Microlithography, (1998)


13. CGAL User’s Guide, http://www.cgal.org.


14. B.B. Sindahl, Interactive Graphical Analysis of Bit Fail  Map Data Using Interactive Pattern Recognitions, Proc. of International Test Conference, 687-695 (1987).


15. C.A.Gloor, Embedded Memory Analysis for Standard  Cell ASIC Yield Enhancement, Proc. of International  Symposium for Testing and Failure Analysis, 69-75 (2000).


16. T. Kohonen, Self-Organization and Associative  Memory, Springer Verlag, New York (1988).


17. The Growing Hierarchical Self-Organzing Map   Project, http://www.ifs.tuwien.ac.at/~andi/ghsom.


18. M. Dittenbach, D. Merkl, and A. Rauber, The Growing  Hierarchical Self-Organizing Map, Proc. of the  International Join Conference on Neural Networks, 6, 15-19 (2000).


p 242-247


DOI: 10.1361/cp2003istfa242


## Electrical Failure Analysis and Characterization of Leakage Paths Leading to Single Cell Failures in 128Mbit SDRAMs


Electrical Failure Analysis and Characterization of Leakage Paths Leading to  Single Cell Failures in 128Mbit SDRAMs


M. Versen and A. Schramm


Infineon Technologies AG, MP PDT PT1 PRE1


Balanstr. 73, D-81541 München, Germany


+49 89 234 20302, FAX: +49 89 234 23339


A common failure signature in dynamic random  access memories (DRAMs) is the single cell failure. The charge is lost and thereby the information stored  in trench capacitors can be destroyed by high  resistive leakage paths. The nature of the leakage  path determines the properties of the failure such as  temperature-, voltage- and timing-dependencies and  its stability. In this study, high resistive leakage paths  were investigated and delimited from classical shorts  by estimating the order of magnitude of the leakage  current and by comparison to a simple resistive  leakage path. Such an investigation is the basis for a  defect-based test approach that leads to multiparameter tests [1].  An introduction to the problem is  given in the first section, while the second section  deals with the characterization of the defects in two  case studies. A short summary is given in the end.


Opens and shorts occur in DRAM cell arrays as well  as in logic circuits. An open in the path between cell  capacitor C1 and bitline connected to VBL1, e.g., an  open bitline contact, is shown in the left part of Fig.


1. The right part of the figure represents a short  between the capacitor C1 and the wordline VWL1. These opens and shorts in the schematics shown in  Fig. 1 are in principle easy to detect and also easy to  localize. The open prevents any WRITE and READ  operation to and from the cell, and therefore a write  and read test pattern will detect such an open easily. If the open is exchanged against a resistor in Fig. 1(a), the detection of the failure will depend on the  WRITE and READ timings as well as on  temperature. Both polarities of information might fail  in this configuration.


The short from the capacitor to the wordline in Fig. 1(b) will lead to a low voltage level while the  wordline is closed (VWL1=0) and to a high level while  it is open (VWL1=3.0V). Any information written to  the cell will be overwritten by this leakage path. During a READ the wordline is open of course and in  any case a high level will be detected, although a low  level is possibly expected. In this case only the  physical zero information (“0”) is failing. In practice, both failures - the open and the short - are relatively


easy to detect and also easy to localize because all  cells have a unique address. The failure signature will  lead to an assumption on the leakage path or open  and to a successful physical failure analysis.


Fig. 1: Examples of an open (left schematic) and a  short (right) in a DRAM array.


Characterization of the Defects  – Case Study 1


The schematic in Fig. 2 shows a parasitic device  representing a totally different kind of defect. A cell  capacity normally accessed by its wordline VWL1 and  bitline VBL1 is connected to a second adjacent but  unused capacitor C2. This unused capacitor is just a  normal cell capacitor. It lies on the border of the  array for symmetry reasons, but this cell does not  have a bitline contact. The parasitic device is created  by a passing wordline that is running above a trench  capacitor. This is an intrinsic design property of the  memory chip. An attribute of this configuration is  that all circuits are working as they should. During  standard WRITE and READ operations the circuits  are functional, and they do not even have parametric  abnormalities. Only special sequences lead to failing  conditions. Such a special condition is also depicted  in Fig. 2.


The capacitor C1 must be charged with a high level in  a first step. Opening the parasitic device with the  passing wordline VpassingWL leads to an equalization of  the levels and to a transfer of charge to C2. Multiple  refreshes of C1 and activations of VpassingWL  will lead  to a high level in C2 that is nearly the high level VBLH  written into C1 via the bitline. When the preparation  of C2 is finished, a low level is written to C1. This  open


VWL1


VBL1


C1


short


situation is shown in Fig. 2 by the “0” next to C1 and  the “1” next to C2. Opening of the parasitic device  VparasiticWL will now lead to an equalization of the “0” with the “1” in C2. This leads to an intermediate level  between 0 V and the high level VBLH=1.8 V. This  intermediate signal level is not sufficient to be


evaluated correctly by the sense-amplifier.


Eventually a READ of the “0” will fail in this


configuration under tight READ timing conditions.


Fig. 2: Schematic of gated leakage paths in a DRAM


array: the schematic shows a configuration of two


capacitors. C1 is an active, C2 is an unused one. Both  are connected by a parasitic device.


If we assume that the intermediate level is achieved  by equalizing the charge between C1 and C2 during  an activation of VparasiticWL, then the effective  resistance of the parasitic device with open VparasiticWL  can be estimated in terms of a two terminal device by  the RC time constant of the configuration. The  effective resistance is given by Reff = t/C in this  approximation. The capacity is approximately 40 fF  and the passing wordline must be opened with a row  active time tRAS of 100 ns to induce the fail. So the  effective leakage current is an equivalent current  through a simple effective resistance with a value of  approximately Reff =2.5 MΩ.


Characterization of the Defects   – Case Study 2


The configuration shown in Fig. 3 is similar to Fig. 2, but there are two active capacitors C1 and C2, normally accessible by their wordlines VWL1 and VWL2  and bitline contacts VBL1 and VBL2. They are  connected again by a parasitic device such as shown  in Fig. 2. The parasitic device is gated by a passing  wordline that is running above one of the capacitors. This parasitic device is again an intrinsic property of  the memory chip. The fail configuration in Fig. 3 is  somewhat similar to the previously discussed one, but there are important differences.


Fig. 3: Schematics of gated leakage paths in a DRAM  array: the schematic shows two active capacitors C1  and C2 connected by a parasitic device.


The parasitic device is opened several times instead  of once in Case 1. C2 is refreshed by an activation of  wordline WL2 between two activations of the passing  wordline in order to have a well established low  voltage level at C2, which is the drain of the parasitic  device. In this case, the effective resistance is mainly  characterized by the number of activations. The  number of activations n of the passing wordline with  the row active time tRAS determines the total transfer  time or total open time ttotal of the charge by ttotal = n × tRAS. Since the parasitic device is effectively open  during this time, it is therefore a measure for the  effective resistance of the leakage path via


C t


RAS


eff


tRAS is the row active time and amounts to 152 ns, the  capacity shall be again 40 fF. Experimental data  collected with different tests are shown in Fig. 4. The  tests were executed on an Advantest T5581 test  system. The temperature was set to 85°C by a  temperature controlled thermostream using a  heated/cooled air stream. The operating DRAM  frequency is 105 MHz. A number of activations n of  Eq. (1) were needed to induce the failures on an  affected component, and it therefore varied from test  to test. After execution of a test with a fixed number  of activations n, the failcount data were taken from  one I/O pin of the DRAM device by using the fail  bitmap tool of the Advantest test system. The number  of activations n and the effective resistance R from  the effective resistance approximation formula (1) is  plotted versus the failcount for this component. The  lowest failcount value in the graph of Fig. 4  corresponds to the first fail induced by 13 activations  corresponding to an effective resistance of 49 MΩ. The failcount curve saturates in the range between  16,000 and 24,000 activations with approximately  1,200 to 1,400 fails. The additional failures in this


‘1‘


VpassingWL


‘0‘


parasitic


device


C2


VWL2


VBL2


range have highly resistive leakage paths with  effective resistance values between 40 GΩ and 60  GΩ. They are highly dependent on temperature. The  internal heating of the device, the previous test


executions, and unintended pauses between the two


test executions lead to some deviations from a


smooth curve (Fig. 4). The effective resistances range  from 49 MΩ to 60 GΩ and therefore exceed the value  from Case 1 by one to four orders of magnitude at


these test conditions.


Fig. 4: The number of activation of the parasitic  device n and the calculated effective resistance Reff  plotted versus the failcount of a single component, respectively.


Temperature dependency


The temperature dependency was analyzed for the  first fail of the previously discussed device. The first  fail appears with 13 activations at T=85°C  corresponding to a certain effective resistance.  The  device was cooled down in steps of 5°C by the  temperature setpoint of the thermostream. The tests  were executed with a starting activation number n=13  that is increased until the first fail appears. The  minimum required number of activations n(T) is  afterwards used as new starting activation number  n(T-5°C) for the next temperature step. The fail


address of the first fail was verified for each step  using the fail bitmap tool of the Advantest test  system. The required number of activations n for  inducing the first fail is plotted in Fig. 5. The error  bars represent different test results for repeated test  executions. In the range of the error bars the test  results are instable, because the test is either PASS or  FAIL. Activation numbers above the higher error bar  border give always FAIL test results, and below the  lower error bar always PASS test results.


Fig. 5: Required number of activations n to induce  the first failure for different temperatures T. The inset  shows the logarithm of the effective resistance plotted  versus the inverse temperature.


In general, the number of activations must be  increased in order to induce the failure at lower  temperatures. This activation increase corresponds to  a higher effective resistance R of the leakage path at  lower temperatures. The effective resistance increases  one order of magnitude, from 49 MΩ to  approximately 450 MΩ since an exponential behavior  is suspected for the response to temperature.


exp(


k


eff =


The logarithm of the effective resistance is plotted  versus the inverse temperature to determine the slope  and thereby the exponent E (shown in the inset of


4000 8000 12000 16000 20000 24000


-200


0 200 400 600 800 1000 1200 1400 1600


number of activations n


0 5 10 15 20 25 30 35 40 45 50 55 60


effective resistance (GΩ)


-5 5 15 25 35 45 55 65 75 85


temperature (°C)


0 50 100 150 200 250 300 350 400 450


103/T [1/K]


2,8 3,0 3,2 3,4 3,6 3,8


4,0 4,5 5,0 5,5 6,0


Fig. 5). This exponent E is a kind of activation


energy and was determined to be 0.19 eV.


This is an intrinsic property of each leakage path. The  schematic in Fig. 3 shows that there is a voltage drop


of VSD = VBL1 – VBL2 across the parasitic device. This  initial voltage difference is VSD = VBLH – 0 V = 1.8 V. This lowers since the levels between the trenches


equalize during the activation of the parasitic device,


the VBL1 level at capacitor C1 decreases, and the low  level at C2 increases during the activation. The  simplest approximation for VSD is a constant voltage  drop for each activation. Since the effective


resistance of the parasitic device is indirectly  proportional to the current through the device ID ~ R-1  and  as the voltage drop is assumed to be constant,


Eq. (2) can be written for the current:


In this context, the current can be understood as a  sub-VTH source drain current of the parasitic device. The physical meaning of the exponent E can be


derived by comparison to a proper sub-VTH source  drain current formula [2]:





′


TH


GS


exp


In Eq. (4) 0I ′  is identified as the current I0 from Eq.


(3) including the geometry of the device. The  difference between gate source voltage VGS during  activation and threshold voltage VTH of the parasitic  device equals the previously determined exponent –E. The sign is negative because VTH > VGS.  Since VGS  is known as the wordline voltage VWL = 3.0 V, then  the threshold voltage of the device should be VTH = VWL + E/e = 3.19 V. Such a comparably high  threshold voltage is known from thick gate oxide  transistors.


Threshold Voltage and Oxide Thickness  Calculation


In order to estimate the oxide thickness, the threshold  voltage VTH  was calculated by


SB


F


FB


φ


γ


The source bulk voltage is VSB = 0, because the  substrate and the source contact are at 0 V (see  schematic in Fig. 3). The flat band voltage was set to  VFB = – 0.8 V for this approximation. The surface to  bulk potential 2φF and the body-effect parameter γ are  given by


i A


n N


e T


kln


2φ


OX OX


eN


These parameters are dependent on the substrate  doping concentration NA and the oxide thickness tOX, while the other parameters are constant. The  threshold voltage according to Eq. (5) was calculated  for an oxide thickness between 40 nm and 140 nm  and a doping concentration between 1016 cm-3 and  1017 cm-3. The resulting VTH curves are plotted in Fig.


6.


The cross points with the experimentally determined  threshold voltage of 3.19 V (dashed line in Fig. 6) shows that the oxide thickness of the parasitic device  must be on the order of 140 nm to 50 nm for a doping  concentration in the 1016 cm-3 range. These results are  not totally unrealistic, because the process parameters  for the doping concentration and for the isolating  oxide of a passing wordline to the substrate are in this  order of magnitude.


Physical Failure Analysis


The root cause of these high resistive paths for the  defect Cases 1 and 2 was a light exposure problem at  the edge of the array. A SEM image of such a failure  was taken after a lift-off was performed on one  device (Fig. 7). The SEM image shows the edge of a  DRAM array. The dark circles are the locations  where isolating oxide were removed around the  trenches. The bright regions connecting two trenches  are active areas of highly doped poly-silicon. The  bitline contacts are sitting on top of these active  areas. The wordline would run perpendicular to the  active areas. The wordlines WL1, WL2, and two  passing WLs are indicated by the dashed lines in Fig.


7. They represent in this image the wordlines from  the schematics in Fig. 3. The trenches C1 and C2 are  fully functional and they are accessed by WL1 and  WL2, respectively.


Fig. 6: The threshold voltage VTH vs. the doping  concentration NA with the oxide thickness tOX as  parameter. The dashed line is the 3.19 V line.


A defective active area at the border of the array  connects the active areas of the trenches C1 and C2. A  leakage path was formed by a defective active area in  a special way: the active area was still at the assumed  location. It was thinner compared to the other active  areas, and it is bent at its ends towards the active  areas of the capacitors C1 and C2. The left and right  arrows in the bottom of Fig. 7 are pointing to these  locations. This leakage path is highly resistive and it  is gated by the passing wordlines at some place (middle arrow). As the semiconductor is p–doped  below the wordlines, the parasitic thick gate oxide  transistor is formed in this region. The oxide  thickness towards the passing wordline and the  doping concentration for this area fits to the order of  magnitude given by the DRAM process.


Fig. 7: SEM image of the leakage path: a defective  active area form a connection gated by a passing  wordline between two trenches C1 and C2 referring to  the schematic in Fig. 3.


Case Study 1 would be represented in the SEM image  by only one leakage path from the capacitor C1 to the  defective active area and from the defective active  area to a dummy trench. There should be no second  connection to the active area of C2 – the connection  pointed at by the right arrow should be missing. This  configuration is also shown in the top part of Fig. 8  for simplicity.


The failure of Case Study 2 was formed by the  already described connection from the active area to  the defective active area with a passing wordline as  parasitic device.  The connection from the other side  of the parasitic device to the second must be a direct  connection with some kind of point defect in the  trench oxide. Such a defect was found in the SEM  image at the two trenches, where the isolating trench  oxide was covered by a bright and therefore  conducting material (Fig. 7 and Fig. 8 middle).


The shown SEM image leads to a third class of  failures that was formed in the case where the  leakage path was gated by two passing wordlines  instead of one. This situation is shown as Case 3 in  Fig. 8.


9 10


2,0 2,5 3,0 3,5 4,0


tOX=  40nm


tOX=  50nm


tOX=  60nm


tOX=  70nm


tOX=  80nm


tOX=  90nm


tOX= 100nm


tOX= 110nm


tOX= 120nm


tOX= 130nm


tOX= 140nm


NA (1016cm-3)


WL1


WL2


passing WL


defective active  area and region  of the parasitic  device


connection to C1


connection to C2


Case 1


Case 2


Case 3


Fig. 8: The possible failure configurations: the  trenches and the active areas are shown in the same  arrangement like in Fig. 7. The wordlines are  running perpendicular to the active areas (dashed  lines). The leakage paths are shown as curved lines  with arrows.


Single cell failures in 128Mbit SDRAMs were  electrically analyzed. The root cause was identified  as a resistive leakage path either between two cell  capacitors or between cell and parasitic capacitor. The connection was formed by a parasitic device, the  passing wordline, which is design inherent. The  leakage currents through these parasitic devices were  comparable to currents through simple two terminal  resistors with effective values in a range between 2.5  M and 60 G. The root cause was identified to be a  light exposure problem at the array border. The  estimated values were very high values for shorts. Normally such high defect resistances are found in  opens, e.g., in via resistances [3]. The shorts are  caught by a multi-parameter test; the critical  parameters are high temperature, the activation  sequence, and timing conditions.


The authors would like to thank their colleagues in  the physical failure analysis department FA1,


especially Alexander Duch, for their help for the root  cause analysis.


1. J. Segura, A. Keshavarzi, J. Soden, C. Hawkins, ITC 02, pp. 90 – 99 (2002).


2. K. Hoffmann, VLSI Entwurf, Oldenbourg  Verlag, München (1996).


3. K. Baker, G. Gronthoud, M. Lousberg, I. Schanstra, C. Hawkins, ITC 99, pp. 467 – 476 (1999).


Session 10: Poster


# Session 10: Poster - Case Studies


Sandra Delgado. Accurel Systems. Sunnyvale, CA


p 249-255


DOI: 10.1361/cp2003istfa249


## A Study on Fluorine-Induced Corrosion on Microchip Aluminum Bondpads


A Study on Fluorine-Induced Corrosion on   Microchip Aluminum Bondpads


Y. N. Hua, S. Redkar*, Ron Dickinson* and S. L. Peh, Shirley


Chartered Semiconductor Mfg Ltd


No. 2 Science Park Drive


Singapore Science Park, Singapore 118222


*60 Woodland Industrial Park D, Street 2, Singapore 738406


In the authors' previous paper, we studied the  defects from Fluorine-Induced Corrosion on


microchip Al bondpads using SEM, EDX, TEM,


AES, IC, XPS and TOF-SIMS techniques. An


unknown F-Al compound was found and identified  as [AlF6]3-. In this paper, we will further study the  chemical mechanisms of Fluorine-Induced


Corrosion on microchip Al bondpads and propose a


theoretical electrochemical model to reveal the  secrets of Fluorine-Induced Corrosion on Al


bondpads. To support this new theoretical model,


we will provide substantiating data from TOFSIMS analysis and other failure analysis


techniques. According to the theoretical model of


Fluorine-induced Corrosion proposed, fluorine


contamination on Al bondpads will cause two types


of corrosions. First, fluorine reacts with Al and  forms a complex compound [AlF6]3- on the affected  area, which we will refer to as Fluorine Corrosion. Once the compound of [AlF6]3- forms on Al  bondpads, it will form an Anode and cause further


electrochemical reactions from O2, N2 and H2O (moisture) at the Cathode. The new products of  further electrochemical  reactions will be [OH]- and [NH4]+ ions. The new product of [OH]- ions will  react with Al and cause further Al corrosion on  bondpads and form corrosive product consisting of  Al(OH)3, which we will refer to as [OH]- Corrosion. The new product of [NH4]+ ions will  combine with [AlF6]3- and form  a  corrosive   complex compound (NH4)3(AlF6). This proposed  corrosion mechanism results in non-stick bondpad


Aluminum bondpads on semiconductor microchips  play an important role in chips functionality and  reliability. However, two types of corrosion issues (Galvanic Corrosion and Fluorine-Induced  Corrosion) will always affect quality of bondpads. To improve quality of microchip Al bondpads, in


our previous papers, we had made detailed failure  analysis studies of Galvanic Corrosion and  elimination solutions [1-2] and Fluorine-Induced  Corrosion defects [3] in wafer fabrication.


In the authors' previous paper [3], we had studied  Fluorine-Induced Corrosion defects on microchip  Al bondpads (Fig 1 and Fig 2). SEM, EDX, TEM, AES and IC techniques were employed to identify  the root cause of the failure and XPS and TOFSIMS advanced tools were used to study the failure  mechanism of fluorine-induced corrosion defects. As a interesting and significant result, we found an  un-known F-Al compound at the binding energy  position of 78.7 eV using high resolution XPS  fitting technique and identified it as [AlF6]3- (Fig.3) using electrochemical theories and TOF-SIMS  techniques as its fragment ion peaks, such as [AlF4]- were detected [3]. This finding is very  important and significant as it will help us to  develop a theoretical electrochemical model and  well understand the mechanism of FluorineInduced Corrosion on Al bondpads.


In this paper, we will present the results of our  further study of the mechanisms of FluorineInduced Corrosion on microchip Al bondpads and  propose a theoretical electrochemical model. To  support this theoretical model, we will provide  substantiating data from TOF-SIMS analysis  & other failure analysis techniques, which  reveal the  secrets of Fluorine-Induced Corrosion on  microchip Al bondpads. This new corrosion model  will definitely help us to understand failure  mechanisms of fluorine-induced corrosion and  identify solutions to reduce or eliminate fluorineinduced corrosion on Al bondpads in wafer  Fabrication.


Fluorine-Induced Corrosion Defects   on Microchip Al Bondpads


In wafer fabrication, some wafers were reported to  have the fluorine contamination problem on


microchip Al bondpads. Failure analysis results on  the affected bondpads revealed discoloration (Fig  1) and  SEM close-up inspection revealed some "flower-like" defects on the affected bondpads (Fig  2), EDX analysis detected a high fluorine peak on  the "flower-like" defects. TEM results showed that  only 20-30 A of the native oxide was seen on a  good bondpad, however the native oxide was  abnormally thicker than 500 A on the "flower-like" defects. After performing further investigation, we  had concluded that the fluorine contamination was  not due to the wafer fabrication process, but was  due to the wafer packaging foam material [3].


Figure 1. Optical photo showed discoloration and  with black dots on the affected bondpads.


Characterization of Al-F


Compound [AlF6]3-


XPS fitting results of Al 2P electron peak  revealed


Figure 2. SEM micrograph showed that the "flower-like" defects were formed on the fluorine  contamination bondpads and the defects had a  planarhexagonal structure.


revealed an unknown peak at the binding energy  position of 78.7 eV besides Al element peak at 72.8


eV, Al2O3 peak at 74.5 eV and AlF3 peak at 76.3  eV. After careful searching, so far there is no


record in XPS reference materials and books for


this un-known compound at the binding energy


position of 78.7 eV. As such, in authors' previous  paper we have identified it as a complex  compound, [AlF6]3- using the electrochemical  theories and TOF-SIMS technique as its fragment  ion peaks such as [AlF4]- were detected [3]


Figure 3. XPS high resolution scan (Al 2P electron  peak) revealed the chemical states of Al and  compounds, which were Al (72.8 eV), Al oxide (Al2O3) (74.5 eV), AlF3 (76.3 eV) and a un-known  Al compound at the position of 78.7 eV, which has  been identified as [AlF6] 3- [3].


A Theoretical Electrochemical Model of  Fluorine-Induced Corrosion


The finding of Al-F complex compound [AlF6]3- on  Al bondpad is very important and significant as it  can help us to develop a theoretical electrochemical  model and well understand the mechanism of  Fluorine-Induced Corrosion on microchip Al  bondpads.


O2 and H2O (moisture) Chemical Reaction


It is a well-known fact that certain levels of O2 and  moisture (H2O) on Al bondpads will result in Al  corrosion:


O2  +  2 H2O +  4e-        ⇔  4OH-


Eo (+0.40 V)


The Eo stands for the Standard Electrode and  Redox Potentials  at 25o C (298 K). In general, if  the Eo value of an electrochemical equation is  relative large or positive, the equilibrium tends to  shift to the right. However, if the Eo value is


relative small or negative, the equilibrium tends to  shift to the left. In Eqn. (1), the Eo is +0.40 V, then


the equilibrium tends to shift to the right and the


[AlF6]3-


new product will be [OH]-, which will react with  Al and cause bondpad corrosion.


N2 and H2O (moisture) Chemical Reaction


The Eo of Eqn. (2) is negative (-1.05 V), thus in  normal conditions, N2 in the air is chemical stable  and it is difficult to react  with moisture (H2O) from left to right in Eqn (2). However, N2 can also  react with moisture (H2O) and results in corrosion  of Al bondpads when [AlF6]3- presents on Al  bondpads as the Eo in Eqn (3) is more negative (Eo = -2.07 V) and is much lower than that (Eo = -1.05  V) in Eqn (2). In other words, there is an energy  difference between Eqn (2) and Eqn (3):


N2  + 8H2O + 6e-   ⇔ 2 NH4OH + 6 OH-         (2) (Eo = -1.05 V)


[AlF6] 3- + 3e-        ⇔  Al + 6F-


(Eo = -2.07 V)


Because of


NH4OH                 ⇔  [NH4]+   + OH-


Thus Eqn (2) can be re-written into:


N2  +  8H2O +  6e-     ⇔  2[NH4]+   + 8OH-            (5) (Eo = -1.05 V)


Therefore, if  [AlF6]3- presents on bondpad, similar  to O2, N2 will also react with H2O (moisture) and  form the new products of [NH4]+ and [OH]- ions, which will further react with Al and cause bondpad  further corrosion.


A Theoretical Model of Fluorine-Induced  Corrosion


From the above discussion, we understand that if  there is fluorine contamination on a Al bondpad, the chemical reaction from Eqn (3) will occur and  form [AlF6]3-. At the same time, chemical reactions  from Eqn (1) and Eqn (5) will also occur and cause  further corrosion on Al bondpads. This indicates  that [AlF6]3- has become an Anode while N2, O2  and moisture (H2O) become a Cathode  electrochemically:


Anode:


Cathode:


O2  +  2H2O +  4e-   ⇔  4OH-


(Eo = +0.40V)


N2  +  8H2O +  6e- ⇔  8OH- +2[NH4]+                  (8)  (Eo = -1.05 V)


4Al  ⇔ 3 Al (OH) 3          (9) [AlF6] 3- + 3[NH4]+    ⇔  (NH4)3(AlF6)


(10)


From an electrochemical view, on a normal Al


bondpad, Eqn (7) and (8) are difficult to react from


left to right as there is no chemical reaction from


the Anode of Eqn (6). However, if fluorine  contamination is present on Al bondpads, Eqn (6) will react from right to left and form [AlF6]3- as an  Anode. Then at the Cathode, Eqn. (7) and (8) will  react from left to right and form [OH]-, which will


react with Al and cause further corrosion on


bondpads by Eqn. (9).


Based on the above corrosion model, one can fully  and clearly understand that fluorine contamination


on Al bondpads will result in fluorine corrosion.


Fluorine reacts with Al and forms a complex  compound [AlF6]3- on the affected bondpads by  Eqn (6). We have proved the presence of  [AlF6]3- ion on the affected bondpads using TOF-SIMS  technique [3]. The   presence of  [AlF6]3- on Al  bondpads will form  an Anode and cause further


electrochemical reactions from O2, N2 and H2O (moisture) by Eqn. (7) and (8) at the Cathode. The


new products of the corrosion reactions will be [OH]- and (NH4)+ ions. The product of OH- ions  from Eqn. (7) and Eqn. (8) will react with Al and


cause further Al corrosion on Al bondpads by Eqn


(9) and form the corrosive product of Al(OH)3. While the new product of (NH4)+ ions will combine  with [AlF6]3- and form  a  corrosive  complex  compound (NH4)3(AlF6) by Eqn. (10).


Support Data from  TOF-SIMS  Analysis


In the authors' previous paper, we have proved the  presence of  [AlF6]3- ion on the fluorine  contamination bondpads using XPS and TOFSIMS techniques [3], which indicates the  occurrence of the chemical reaction from Eqn. (6). In this study, we will prove the presence of [NH4]+ ions on the affected bondpads, which indicates the  occurrence of the chemical reaction from Eqn. (8). TOF-SIMS technique was again employed to  determine [NH4]+ ions and it fragment ions such as  NH3,  [NH2]-  and [NH]2- on the affected bondpads.


TOF-SIMS analysis was carried out on an IONTOF SIMS IV system. A 25 keV Ga gun was  operated in both imaging and high mass resolution  mode to identify the chemical species and obtain  the distribution at the same time. Both positive and  negative ion images were obtained for higher  secondary ion yield.


TOF-SIMS mapping results showed the  distribution of F, O, [NH4]+ and Al on the affected  bondpad (Fig 4). From TOF-SIMS ion imaging  results (Fig. 4), one can see that the presence of [NH4]+ ions on the affected bondpad. This has  proved the occurrence of the chemical reaction  from Eqn. (8) as the new product of [NH4]+ was  detected on the affected bondpad. The results also  indicated the chemical reaction from Eqn. (8) only  occurred at the Fluorine-Induced Corrosion defect  areas as the distribution of [NH4]+ ions was the  same as distributions of F & Al ions, which was  only at the “flower-like” defect areas (Fig. 4).


TOF-SIMS analysis was also performed on a  normal bondpad and an affected bondpad.


Figure 4. TOF-SIMS ion imaging results showed  that the presence of [NH4]+ ions on the affected  bondpad and the distribution of [NH4]+ ions was  only at the “flower-like” defect areas, which was  the same as distributions of F & Al ions.


The analysis area was about 27 um x 27 um, the  collecting time was 100 secs. The peak calibrations  were performed by using F and Ga peaks for the  positive spectra and by using F and Al for the  negative spectra. The intensities detected from the  positive and negative ions are summarized in Table


1.


From Table 1, one can see that the amount of [NH4]+  ions and its fragment ions like NH3,  [NH2]- and [NH]2- detected on the fluorine contaminated


bondpad (F-Pad) are much higher than these


detected on the normal bondpad (N-Pad). This is a  very strong proof of the presence of [NH4]+ ion on  the F-Pad (fluorine contamination bondpad) and


supports the theoretical model of Fluorine-Induced  Corrosion proposed in this paper.


Table 1. Intensities from the Positive and Negative  Ions Detected on the Fluorine Contaminated  Bondpad (F-Pad) and the Normal Bondpad (NPad)


Positive


Negative


Ion      F-Pad    N-Pad    F-Pad    N-Pad


N        208    -


-      -


[NH]2-   808    5


1522      88 [NH2]-   13845    57      217      2  NH3      87355    147      48      22 [NH4]+  135817    794       -       -


Figure 3 shows the schematic of the HBM ESD circuit and the pin combination (I/O to Vss) testing of the  DUT.  Rc is the charging resistor, Rd is the discharging resistor,  Cc is the  charging/discharging capacitor, PUT is the pin under test, DUT, the device under test and Re is the resistance to earth ground.


The failing devices were analyzed using conventional  electrical , photon emission, chemical and electrochemical  techniques, followed by high magnification SEM  examination to distinguish the morphological and physical  damages and verify their physical location [ 1, 2, 19 ].  Photon emission is particularly useful because it allowed us


to identify the location before the chemical destructive  delayering.  The Input/Output I-V leakage characteristics  and Icc failures showed distinct differences between the  various failure signatures, enabling easy identification of  the pin combination stress mode initiating the failure.


Rc


Re


Rd


DUT


PUT


Experimental Results


The table below is a summary of the electrical characteristics and physical morphological failure signatures associated  with the different pin combination stress modes.


Pin Combination Electrical  signature Location  Chip structure


Failure signature


1.   I/O-to-Vss   2uA – 10 uA


Protection Pull-down


Contact spiking


2.   I/O-to-Vss   Icc >>  Icc max


Arc- over


3.   I/O-to-Vcc


500 nA –10 uA


Protection  Pull – up


4.   I/O-to-Vcc


Icc  >> Icc max


Arc-over


5.   I/O-to-I/O


1.0 – 100 uA


Protection Pull-up or   Pull-down;


6.   I/O-to-I/O


Core


Source-to-Drain or   Drain-to-Source


7.  Vss-to-Vdd    or   Vdd-to-Vss


Icc/Functional


Source-to-Drain   or Drain-to-Source


Pin Combination: I/O to Vss


Referring to the table above, two distinct electrical failure  signatures (Leakage-line 1 and Icc- line 2) were observed  for the same pin combination stress of I/O-to-Vss.  See  figure 4 for example of the leakage failure (low breakdown) and a good pin (flat line.).  This same pin combination  resulted in two distinct failure morphology, one being  contact spiking (figure  5) and the other, an arc-over type  failure (figure  6),  but both occurring in the same physical


location, the pull down NMOS transistor of the selfprotecting output circuit [ figure 7 – location A ].    For the  positive stress using  I/O-to-Vss,  the different directions of  the current flow from the pad into the whole device will  depend on the technology.  For this device technology, there are at least three possibilities: 1: the vertical NPN  through the substrate.  2: the lateral NPN between the drain  and the source and 3: the lateral substrate diode which is in  the reverse biased mode for this pin combination.   For the  negative stress using the same I/O to Vss, most of the  current now goes through the same substrate diode (which


is now forward biased ).  This negative polarity is what may  have caused the Icc type failure observed (line 2), as  opposed to the leakage current which is due to the positive  polarity stress.   This type failure is easy to distinguish for  this pin combination because both the electrical and  physical failures are quite different.  However, the


qualification standards do not place any strict requirement  on testing all positive, then all negative or alternating   between positive and negative pulses, then distinguishing  between results due to positive or negative stress can be  challenging.


Figure 4   I-V characteristic curve showing leakage at


the I/O protect structure for both pull up and pull down   pin combinations


Fig.5 HBM.  Contact damage at the poly level in the nchannel.  This is I/O to Vss Stress with leakage failure.   Similar  morphology for the MM stress.


Fig.6.  Arc over in pull down transistor


corresponding to I/O to Vss  leakage failure.


Figure 6


Figure 5


Figure 7 showing the failure location A in the Drain of the pull-down NMOS transistor for the I/O to Vss pin  combination stress.


Pin Combination I/O-vs-Vdd (Vcc)


Referring to the same table above, two additional distinct  electrical failure signatures (leakage- line 3 and  Icc/functional- line 4) were observed for the same pin  combination stress of I/O-to-Vcc.  This pin combination  also resulted in two distinct failure morphology: one being  contact spiking (line 3) in the drain due to the leakage  between the drain and the grounded substrate.  The other is  an arc-over type failure (line 4) between the Vdd and Vss  contacts and which represents the Vdd shorted to ground.  Note that both failures occurred in the same physical  location, the pull-up PMOS output transistor.  For the ESD


stress using  I/O to Vdd,  there are also three distinct  current paths similar to the I/O to Vss stress discussed  above, but here we have a parasitic vertical PNP transistor, a parasitic lateral PNP transistor and a substrate diode  which is forward biased to Vdd.   For the positive stress  most of the current will go through the forward biased  diode, which results in the leakage failure (table- line 3).    For the negative stress using the same I/O to Vcc pin  combination, the diode is now reverse biased so most of the  current goes through the Vdd-Vss protection device .  This  negative polarity is what may cause the Icc type failure  observed (line 4), as opposed to the leakage current which  is due to the positive polarity stress .   This type failure is  easy to distinguish for this pin combination because both  the electrical and physical failures are quite different.


Location A


I/O  pad


Inverter


Vss


I/O vs Vss compared to I/O vs Vcc


A closer look at the table reveals that line 1 (I/O to Vss) has  the same leakage type failure as line 3 (I/O to Vdd) and  also the same morphological failure (contact spiking)    What differentiates them is the different location of the  failure which should be as expected for the pull-down and  pull-up transistors respectively.  Similarly, the same Icc  failure found on line 2 for I/O to Vss and line 4 for I/O to  Vdd produces the same morphological failure type (arcover between contacts).   Again, what differentiates them is  the fact that   the failure occurs in two different locations  which are as expected for the pull-down and pull-up  transistors respectively.  What is to be noted here is that the  failure actually occurred between the  Vdd and the Vss  contacts.    The similarities can be seen for these two pin  combination types in that both types exhibited both leakage  and Icc type electrical failures and both exhibited contact  spiking and arc-over morphological type failures.  However, for proper distinction and conclusion, failure  analysis must be performed so that the morphology and  location can be determined.


Pin Combination I/O vs I/O


The I/O to I/O leakage failures produced physical damage  both at the internal core circuitry and in the contacts for  either the pull-up or pull-down transistors probably  depending on whether the stress was positive or negative, but most of the damage occurred in the nMOS transistors.


Since the standards require that both pulse polarities be  delivered to each pin during qualification, then  distinguishing between the failure caused by either the  positive pulse or the negative pulse effect can be  particularly difficult.  This is because, as mentioned above, the procedures in the different standards are not specific  about whether to alternate positive and negative on the  same pin or to perform all negative, then all positive or to  change devices for polarity stressing.  This polarity  separation/difference is important for designing purposes  because there are several travel paths for the ESD current


through the whole device and different ESD elements are  affected depending on polarity of the pulse.


Consider the following: for a positive pulse from I/O1 to  I/O2, the current will take the easiest path (see figure 8 ) from the several available paths..  The current path 1 will  go through the forward biased diode, D1, at the pull-up  transistor for the I/O1  pin, then travel through the internal (core) circuitry,  and then through the forward biased diode, D4, at the pull-down transistor for the I/O2  pin.  Both  leakage and Icc failures were obtained.  The path 2  could/will go through the reverse biased diode, D3, at the  pull-down transistor for I/O1  pin,  and then through the  forward biased diode, D4, at the pull-down transistor for  the I/O2  pin.  It seems that the pull-up Transistors for I/O1   and pull-down transistor for I/O2  will be the most  vulnerable in both situations where I/O2 is always grounded  while the Vdd and Vss pins are floating during this test.


For the leakage failures (line 5), the physical failures were  contact spiking in the drain contacts of the protection  structures and for the Icc failures (line 6), the physical  failures were arc-over between the source and drain  contacts at an internal location.   Since I/O to I/O failures  were so few and far between, no particular attention was  paid to the level of leakage current required to fail and  therefore distinguish between the pull up and pull down  failures for this stress mode, but most of the failures did  occur at the pull-down transistors.


Pin Combination Vdd to Vss   and Vss to Vdd


The pin combination Vss to Vcc (Vdd) stress  predominantly caused failures in the core logic of the  device in the form of Icc and/or functional failures which  showed arc-over damage from source to drain at an internal  location (figure 9) far from the ESD protection structure  which is located at the pad.  The dominant failure site was  a core internal parasitic lateral NPN formed between the  source of a pMOS device connected to Vdd bus and the  source of an nMOS device connected to Vss bus.  For this  programmable logic device, the Vss to Vdd and Vdd to Vss  failures occurred in the same core location.


D2


FIGURE 8  showing the 2 possible paths for the ESD current flow during the I/O to I/O pin combination stress.


Fig. 9.  Arc-over between S and D at internal


location for Vss to Vcc stress corresponding to


ICC failure.


The above data clearly shows the signature difference  between pin leakage failures and functional/Icc failures.  By  assessing the cause of failures, and making appropriate


corrections, the failure threshold of this device was raised  from a marginal 2000 volts  to over 3000 volts for  HBM  and from  200 volts up to 600 volts for MM. The lessons  learned were applied to all later product, resulting in a  3-fold reduction in field returns.


Conclusions:


The aim of the work was to use a case study to show the  basic ESD signature difference between devices which fail  for the pin combination I/O versus I/O leakage tests and  those which fail for ICC leakage during ESD  characterization or qualification Testing.  The principal  applies to ALL the pin combinations for the HBM and MM  ESD Testing.   The case study shows a technique for  combining the several individual methods and failure  results used by the failure analysis community to confirm  the failure from the specific stress mode for that pin  combination.  The methods include the use of the stress  mode, the electrical signature, the morphology and the


Figure 9


I/O2


nMOS  pMOS


CORE


I/O1


D4 D3


failure location to distinguish between the failures as a  result of the different pin combinations.    The results are  important because most reports have dealt only with the  individual electrical signature and then reported that a  failure site was located; but in too many cases, on closer  scrutiny, the two were not related, and the conclusions were  incorrect.   Using the above technique, there is no  ambiguity in  the results and the resulting conclusions.  It is


true to say that these results apply specifically to the  programmable logic devises reported here, but the author  has shown the same to be true for some communication  devices (not reported here), and believe it to be true for  most devices which have basic input and output protection  CMOS devices with pull-up and pull-down type transistors  for protection structures.


1. Leo G. Henry, I.H. Morgan, T.Raymond, M.Mahanpour,  “EOS and ESD Laboratory Simulations and Signature  Analysis of a CMOS PLD.”  Proc. of the 20th  International  Symposium. for Testing & Failure  Analysis (ISTFA), p117, Nov. 1994, Los Angeles, CA.


2   M. A. Kelly, G.Servas, T.Diep, D. Lin, S. Twerefour, G. Shah, .  “A Comparison of ESD Models and Failure  Signatures for CMOS Integrated Circuit Devices.” EOS/ESD Symposium  Proceedings.   EOS-17, p175, 1995, Phoenix, AZ.


3.  Ajith Amerasekera and C. Duvvury . “ESD in Silicon  Integrated circuits”,  John Wiley Publ., NY , 1995.


4.  Leo G. Henry, J. Barth, J. Richner, K.Verhaege,  26th  Annual ISTFA2000. “ Transmission Line Pulse  Testing of the Protection Structures in ICs- A Failure  Analysis Perspective”.  p203-214, 2000, Bellevue, WA.


5.  S. Dabral and T.J. Maloney, 1998  “Basic ESD and I/O  Design”. John Wiley & Sons, NY.


6.  G. Krieger, “ The Dynamics of ESD prior to Bipolar  action Related to Snap-back”, p  1989 EOS/ESD  Symposium, EOS-11, p136, 1989, New Orleans, Louisiana..


7.  Y. Smooha and Dong Lin, “ A Comparison of ESD  Thresholds of CMOS I/O buffers Using Real Human  Body and Human Body Simulators”, EOS/ESD  Symposium, EOS-12, p114, 1990, La Buena Vista,  Florida.


8.  M.S. Straus  and M. H. White, “Protecting N-Channel  Output Transistors from ESD Damage”, EOS/ESD  Symposium, EOS-13, p110, 1991, Las Vegas, NV.


9.  X.  Guggenmos and R. Holzner , “A New ESD  Protection concept for VLSI CMOS Circuits- Avoiding  Circuit Stress” EOS/ESD  Symposium, EOS-13, p74, 1991, Las Vegas, NV.


10.  C. Cook and S. Daniel  “Characterization and Failure  Analysis of Advanced CMOS sub-micron ESD  Protection Structures”  EOS/ESD Symposium, EOS14, p149, 1992, Dallas, TX.


11. N. Maene, J.Vanderbroeck, L. Van den Bempt , F. Antwerpen,   “On-chip ESD Protection for Inputs, Outputs and Supplies of CMOS Circuits”,  EOS/ESD  Symposium, EOS-14, p228, 1992, Dallas, TX.


12.  C. Johnson,  Tim J. Maloney and S. Qawami,  “An  Unusual HBM ESD Failure Mechanisms on a mature  CMOS Process”, .EOS/ESD Symposium, EOS-15, p225, 1993, La Buena Vista, Fl.


13.  M. Chaine, S.Smith and A. Bui,  “ Unique ESD  Failure Mechanisms during negative to Vcc HBM  tests”  EOS/ESD Symposium, EOs-19, p346, 1997, Santa Clara, CA.


14.  J.C. Smith,  “ A Substrate Triggered lateral Bipolar  Circuit for High Voltage Tolerant ESD Protection  Applications”, EOS/ESD Symposium, EOS-20, p63, 1998, Reno, NV.


15.  F. Krosropour , Leo G. Henry,  I. Morgan and C. Hatchard,  “Comparison of Failures for HBM ESD  Testers meeting the ANSI/ESD S-5.1 or the new  ESDA standard Test Method and JEDEC Standard” 24th Annual ISTFA 1998, p377, 1998, Dallas, TX.


16. M. Fliesler and I. Morgan, Evaluation of  On-chip   ESD Supply Clamp Robustness by In-situ Floating  Power Bus Monitoring.”  26th Annual ISTFA2000, p195-202, Nov. 2000, Bellevue, WA.


17. ESD Std. STM- 5.1-1999: Human Body Model (HBM) ESD Sensitivity Testing, ESDA, Rome, NY.


18.  ESD Std. STM- 5.2-1999:  Machine Model (MM) ESD  Sensitivity Testing,  ESDA, Rome, NY.


19  C. Cook, S. Daniel, and M.P. Vo .  “Root cause  Analysis of 1.0  Compiled  RAM Stress Failures for  Process Reliability Improvement”.   ISTFA ‘93., pg239, Nov. 1993, Los Angeles, CA


p 272-277


DOI: 10.1361/cp2003istfa272


## ESD: Correlation between Electrical Signature and Failure Modes


ESD: Correlation between Electrical Signature and Failure Modes


V.  Korchnoy *, Dr. B. Lisenker, and I. Posimeinik


Intel Israel (74) Ltd., Haifa, Israel


The correlation between electrical characteristics and failure


modes in some common cases of ESD protection circuitry is


described.  The investigation is based on experimental results  obtained during the qualification of highly integrated CPUs  and chipsets manufactured by 0.18 µm CMOS technology. The implementation of these data during qualification of 0.13 µm CMOS products allowed the decrease of qualification  throughput time (TPT), and, in some cases, reduction of FA


efforts. Some process related and designs related ESD


concerns are discussed herein.


The implementation of effective on-chip ESD (Electrostatic  Discharge) protection is a challenging task that requires  several design iterations, since the ESD performance of an A0  product step is usually not totally effective. Despite the  progress in ESD modeling programs in recent years, electrical  characteristics and failure mechanisms of devices under ESD  stress are still determined experimentally using test structures, process and product splits. Consequently, the product  qualification process demands much failure analysis (FA) effort. The correlation between products electrical  characterization and failure modes enables the main failure  modes to be quickly determined. This can essentially decrease  the throughput time of the product qualification process, and  in some cases, reduce the FA process to signature analysis  based on electrical characterization data. It has been shown  that in long channel silicided technology the electrical  characteristics of the input/output pins after Human Body  Model (HBM) ESD stress can be classified into five categories  in accordance with leakage current increase [1]. In conjunction  with physical failure analysis, these categories have been  related to typical failure modes. Recently, Charge Device  Model (CDM) ESD experimental results for 0.18 µm  integrated CPU’s together with correlations between electrical  characteristics and failure modes were described [2].  From  our point of view this correlation is demonstrable also for deep  sub-micron products. In these devices the transistor work  frequency is close to the Fourier frequency of a CDM ESD  impulse. Therefore, one can anticipate that the alternative  current path during a CDM ESD event would run through


similar transistor configurations in various products, namely  through the configurations which react faster than the ESD  protection scheme. For example, the higher current gain of an  n-p-n parasitic transistor inherent to a n-MOS transistor  ensures that it is first to trigger under CDM ESD conditions. Therefore, the ESD damage location is expected in  NMOSFET connected in parallel with ESD protection cells.


This study was initiated to address the common ESD-caused  failure modes in deep sub-micron technologies through  electrical characterization data, and relate them to specific  process or design issues in future processes products.  In the  first part of this investigation the methodologies of EDS stress  application and failure analysis are described. In the second  part, the main results on correlation between the electrical  signatures and failure modes after ESD CDM stress for 0.18 µm products are presented and discussed. It is shown that the  implementation of these data during qualification of 0.13 µm  CMOS products allowed essentially decreasing the time to  market. The final part presents conclusions and  recommendations.


Methodology


The investigation is based on experimental results that have  been obtained during the qualification of highly integrated  CPU and chipsets manufactured by a fully silicided 0.18 µm  CMOS technology with 5 metallization layers. These data then  have been successfully implemented during 0.13µm processed  integrated CPU and chipsets with 6 metal layers qualification. All signal pins, as well as all unique power supply (PS) pins  were protected from ESD damage by special structures using a  Standard Cell ESD Protection Methodology [3]. This  methodology is based on ESD and I/O libraries containing  proven standard timed PMOS clamps, pad cells (input only, CMOS I/O, GTL) and high-voltage-tolerant versions of these. Stacked-PMOS clamps that allow protection of PS pins up to  three times the nominal VCC voltage have been used as well.


ESD stress model and failure criteria


The main ESD problem in the CMOS device fabrication


process is static charge generation. Charging also takes place  during device transport along conveyor belts during assembly


and in a final test area. The Charged Device Model (CDM) test methodology has been implemented to model the effect of  charge collected during the manufacturing, assembly, test, and  installation phase to CMOS circuitry integrity. We used  Socket CDM testing [4, 5] to evaluate product ESD reliability. The ESD damage threshold criterion was non-functionality, defined as not meeting a data sheet limit or not performing a  device function.


A standard approach to I/O characterization, namely curve  tracing of each pin with respect to ground, power supplies, and  adjacent pins, has been used in this work. Final Test (FT) data  analysis together with direct current (DC) I-V characteristics  of each pin measured before and after CDM ESD stress, allow  localizing the failures to a few analog and core PS pins. All  failures occurred during negative zaps [2].


FA methodology


Generally, two kinds of ESD-related failures are observed [6]. The first is a “classical“ ESD failure, where only silicon  substrate and diffusion layers are affected during the ESD  event. The second is electrical over-stress (EOS) failure, which affects the overlying metallization layers and inter-layer  dielectrics (ILD). This event results in crack development in  the ILD and melting of the affected metal lines caused by the  high current flow.


The FA process of ESD-related failures includes infrared  emission microscopy (IREM) for fault isolation, followed by  several common failure analysis steps: die decapsulation, die  de-processing down to diffusion layers into the silicon  substrate, optical/SEM inspection at the region of interest (ROI). The ROI for FA is defined together with designers  based on the failing pin electrical characteristics.


As most current CPU and chipset products are assembled by  flip chip technology, the decapsulation step includes  mechanical grinding of a package substrate, or de-lidding by  heating of a package to a temperature higher than bump  melting point, and vacuum pulling of the die out of the  package. After the die is removed from the package, wet  etching of bump and under fill epoxy material is performed. Next, the decapped die is to be inspected at ROI using optical  microscopy. This inspection is geared towards detecting EOS  signs. Die deprocessing usually starts by dry/wet etching of  passivation layers. Next, two different ways of deprocessing to  the silicon diffusion layers may be implemented. The first way  includes parallel layer by layer polishing of the die, or  dimpling at the ROI with optical or SEM inspection, followed  by the wet etching of the last ILD film and poly lines to  expose the silicon.  The second way to expose ESD defects is  to perform quick stripback to substrate procedure by wet  chemistry. This procedure skips the laborious process of  polishing and the intermediate layers inspection, and allows  going directly to the silicon diffusion layers. Finally, optical/SEM inspection at the ROI is addressed to document  findings and FA results. To prove the failure root cause found  by FA, FIB circuit edit can be used.


ESD experimental results and discussion


The results below were obtained during qualification of


0.18µm CMOS CPU products. For effective on-chip  protection, the circuit must provide immunity to minimum  stress levels of 800V caused by CDM ESD stress. The CDM  ESD performance of the A0 step of the product under study  was much less effective [2]. The worst-case intrinsic ESD  failure voltage was 400V. Final Test (FT) data analysis  together with each pin DC I-V characteristic taken before and  after ESD stress localized the failure to a few analog and core  PS pins.


(a)                                           (b)


Figure1. I-V characteristics for PS pin before (green) and  after (red) –500V CDM ESD stress (a), SEM micrograph of a  typical ESD damage in functionally failed units (b).


All failures occurred during negative zaps. The whole  aggregate of electrical characteristics obtained after the CDM  ESD stress at the affected PS pins on 0.18 µm products were  classified into four categories (see Fig. 1a, 2a, 3a, 4):


a) A short that results in basic functionality failures (Fig. 1a); b) An increase in a leakage current that results in FT  parametric failures (Fig. 2a) due to pin leakage increase;


c) A core power supply shift due to shorts between isolated PS  pins. It was found that in this case the CDM ESD stress  applied to a few of the analog PS pins resulted in a core PS  shift (Fig. 3a). The I-V characteristics between the analog PS  pin and the core PS pin have been degraded or shorted. The  degradation is correlated with a dramatic increase in the  periphery standby current Isb and is determined in the FT as a  parametric failure [2].


(a)                                        (b)


Figure 2. I-V characteristics of a PS pin before (green) and  after (red) –500V CDM ESD stress for a leaky analog PS (a); SEM micrograph of a typical ESD damage in leakage failed  units (b).


Figure 3. I-V characteristics for core PS shift after the stress  to analog PS (a);SEM micrograph of a typical ESD damage  found in units with core PS shift after stress to analog PS (b).


d) Recoverable failures. The first CDM ESD zap causes shorts (see Fig. 4a), while after the second or third ESD zap the  forward biased I-V curve returns to the initial shape.


(a)                                    (b)


Figure 4.  I-V characteristics for PS pin before (green) and  after (red) –800V CDM ESD stress first zap (a) and after  second zap (b).


Units showing the above mentioned electrical signatures  underwent physical FA. After de-processing down to the  diffusion layer and visual (optical and SEM) inspection, four  types of defects were identified. These four categories of  electrical behavior are related to the four failure modes  described below. The application of the obtained data to the  new, 0.13 µm process, integrated CPUs’ and chipsets’ qualification is shown.


Functional failures


In the 0.18µm products, PS short with respect to ground was  associated with fulmination, resulting in damage between the  two adjacent diffusions in a small NMOSFET connected in  parallel to the failing PS. The device damage is located under  the gate of an NMOS transistor beyond the protection cell. A  SEM micrograph (Fig. 1b) shows a melted gate with a fused  Source-to-Drain junction on the NMOS part of the inverter. The material under the NMOS gate gets totally damaged


causing a possible short Gate-to-Source and Drain-to-Source. The melted filament between source and drain is evidence of a  sudden and sharp rise in local temperature along the filament. The damage usually occurs only on a single finger of the  device. The NMOS transistors affected during CDM ESD  stress showed strong evidence of local overheat in a specific  location where the diffusion and spacer cross. The local  temperature must be high enough to cause such runaway. There is a clearly understood and correctly modeled [8] high  current phenomenon in a bipolar transistor (second  breakdown) that results in current constriction, and causes a “hot” spot. In “hot” spots the temperature reaches the melting  point of silicon. This forms a filament and destroys the device. Every MOSFET transistor has an inherent parasitic bipolar  transistor. It is known that a clad silicide process modifies the  device’s second breakdown characteristics and reduces  NMOSFET ESD immunity to less than 35% of the level with  a non-silicide junction process [2]. In our case (fully silicided


0.18 process), a second breakdown in a parasitic bipolar  transistor inherent to an NMOSFET results in a high current  event development during -500V CDM ESD stress. The SEM  micrograph of such a failure is shown in Fig. 1b.


Figure 5a. Optical micrograph of an EOS-kind damage at M4  layer in functional failed unit after 500V CDM ESD stress.


Figure 5b. SEM micrograph of a typical GNAC damage in  functional and leakage failed units after 500V CDM ESD  stress.


The above correlation between electrical characteristics and  CDM ESD caused failure mode was successfully used during  CDM ESD qualification of 0.13µm products. Presented below  are experimental results that were obtained on a highly  integrated engineering CPU manufactured by a fully silicided


0.13 µm CMOS logic process with 6 metal layers. The studied


Figure 5. TOF-SIMS spectra showed that [NH4]+ and its fragment ions like NH3,  [NH2]- and [NH]2- were detected on the fluorine contamination  bondpad. This documents  the occurrence of the  chemical reaction from Eqn. (8).


The spectra of the [NH4]+ and its fragment ions like  NH3,  [NH2]- and [NH]2- detected on F-Pad are  shown in Figures 5.


NH4                                   Al


mass


18.00


18.05


[NH4] +


17.00


17.05


0 10


N 3


16.00


16.05


[N 2] -


15.05


[NH]2-


One can also see that besides the ions of [NH4]+ , the ions of [NH]2-, NH3 and [NH2]-  were also  detected. We speculate that they were  from  [NH4]+ ions, which occur from the chemical  reaction of N2 and H2O (moisture) in the air by Eqn (8). This is because fluorine contamination on Al  bondpads has formed complex compound of [AlF6]3-. Once the complex compound of [AlF6]3- forms on bondpad, it will become an  electrochemical Anode and cause further  electrochemical corrosion reactions from O2, N2  and H2O (moisture) at the Cathode


Support Data from Failure Analysis


Once again, fluorine reacts with Al and forms [AlF6]3- which we refer to as Fluorine Corrosion:


Al  +  6F-                [AlF6] 3-


(11)


The SEM micrograph shows the fluorine-induced  corrosion defects (refer to Fig. 2). As already  stated, the chemical reactions from Eqn. (7) & Eqn.


(8) also occur and form the new products of [NH4]+ and [OH]-. [OH]- ions will further react with Al  and form Al(OH)3, which we refer to as [OH]- Corrosion:


3 OH-  + Al        (Al (OH)3


(12)


Based on the above theoretical model, we also  predicted that after the [OH]- Corrosion, the "flower-like" defects (refer to Fig. 2) formed  during the Fluorine Corrosion would be partly  damaged or fully dropped away from bondpad  surface due to further [OH]- Corrosion. In the other  word, the [OH]- Corrosion would seriously damage  the surface of Al bondpads and would cause a nonstick bondpad problem at the assembly. Our failure  analysis results have confirmed the above  prediction.


For example, after a few months when we found  fluorine contamination and the "flower-like" defects on bondpads, it was reported that some  wafers were to have non-stick bondpad problem. Failure analysis results conformed that it was a  similar fluorine contamination case due to the  wafer packaging foam material [3] and SEM  inspection found some interesting results as the  "flower-like" defects  (Fig 2) formed during the  Fluorine Corrosion had been damaged and changed  into the "ring-like" defects (Fig. 6). EDX analysis  results showed that no fluorine was detected at the  center of the "ring-like" defect (Fig. 7), but fluorine


Figure 6. Surface SEM micrograph showed the "flower-like" defects (refer to Fig. 2) formed  during the Fluorine Corrosion had been further  damaged and changed into the "ring-like" defects


after further OH- corrosion.


Figure 7. EDX result showed that no fluorine was  detected at the center of the "ring-like" defect. This  means that the [OH]- Corrosion had made further  damaged.


peak was still detected  at  the edge of  the "ringlike" defect (Fig. 8). This means that the [OH]- Corrosion was only occurred at the defect area and  had made further damage on the surface of Al  bondpads


After a few months, we have also found two  similar fluorine contamination cases. It was found  that the "ring-like" defects and surface of bondpads  had been further damaged. Figure 9 showed that  the "flower-like" defects had been fully damaged   and dropped away and only a footprint was found  at the defect area. EDX analysis results further  confirmed our observation as fluorine was detected  at  the "ling-like" defect area, but  no  fluorine  was


Figure 8. EDX result showed that a fluorine peak  was still detected at the edge of the "ring-like" defect.


Figure 9. Surface SEM micrograph showed the "flower-like" defects (refer to Fig. 2) formed  during the Fluorine Corrosion had been further  damaged and fully dropped and only a footprint  was found at the defect areas after further OHCorrosion.


detected on the footprint area (Fig. 10). These  results indicate that after the [OH]- Corrosion, the  Fluorine-Induced Corrosion defects and surface of  bondpads had been further damaged.


The failure analysis results from another fluorine  contamination case also showed that after a longer  period of corrosion, the surface of Al bondpads  were seriously damaged (Fig. 11), which resulted  in a non-stick bondpad problem.


Figure 10.  EDX result showed that no fluorine  peak was detected on the footprint area of the  defect. This indicates that the "ling-like"  defects   had   been   fully   damaged and dropped away  after the [OH]- Corrosion.


After overview the results from Figure 2, Figure 6, Figure 9 and Figure 11, one can easily understand  the whole process of the Fluorine-Induced  Corrosion. All data has strongly supported the  theoretical model proposed in this study.


Summary and Conclusion


In this study, we have studied electrochemical  mechanism of Fluorine-Induced Corrosion on  microchip Al bondpads and proposed a theoretical  electrochemical model on Fluorine-Induced  Corrosion. According to the theoretical model of  Fluorine-induced Corrosion proposed, fluorine  contamination on Al bondpads will cause two types  of corrosions: Fluorine Corrosion and [OH]- Corrosion.


The mechanism of Fluorine-Induced Corrosion on  Al bondpad are: firstly, fluorine reacts with Al and  forms compound [AlF6]3- on the affected area, which will form an Anode and cause further  electrochemical reactions from O2, N2 and H2O (moisture) at the Cathode. The new products of  further electrochemical reactions will be [OH]- and [NH4]+ ions. Secondly, the [OH]- ions will react  with Al and cause further Al corrosion on  bondpads and form corrosive product of Al(OH)3. While the new product of [NH4]+ ions will combine  with [AlF6]3-  ions  and  form  a  corrosive  complex


Footprints


Figure 11. Surface SEM micrograph showed after  Fluorine-Induced Corrosion, the surface of the Al  bondpad had been seriously damaged.


compound (NH4)3(AlF6). These corrosive products  will cause serious damages on the surface of  bondpads, result in bondpad discoloration and nonstick bondpad problem.


To support the new theoretical model, we have  provided the support data from TOF-SIMS analysis  and failure analysis. TOF-SIMS analysis results  showed that [NH4]+ and its fragment ions like NH3,  [NH2]- and [NH]2- were detected on the fluorine  contamination bondpads. We also showed the  whole process of the Fluorine-Induced Corrosion. All data has strongly support the theoretical model  proposed in this paper.


The authors would like to thank Mr. Mo Zhiqiang  from PSB Corporation, Singapore, Chartered Fab1


Failure Analysis Group and Bondpad Taskforce  Team for their contributions to this technical paper. Special thanks to Perry Martin from Materials  Technology Laboratories, Inc. (Mentor for this  paper from the Technical Committee of  ISTFA2003 Conference) for providing technical & professional advice.


1. Hua Y. N., “A Study on Discolored Bondpads  and Galvanic Corrosion”. The proceedings  from the 24th International Symposium for  Testing and Failure Analysis (ISTFA’1998), 15-19 Nov, Hyatt Regency, DFW-East Tower, Dallas, Texas, USA, 269-272  (1998).


2. Hua Y. N., Low E. C., An L. H. and Redkar  S., "Failure Analysis and Elimination of  Galvanic Corrosion on Bondpads during  Wafer Sawing". The proceedings from the 26th  International Symposium for Testing and  Failure Analysis (ISTFA’2000), Nov 12-16  2000, Meydenbauer Convention Center, Bellevue (Seattle), Washington, USA, 369-372 (2000).


3. Hua Y. N., Redkar S., Lau C. K. and Mo Z. Q. (from PSB Corp., Singapore), "A Study on  Non-Stick Aluminum Bondpads due to  Fluorine Contamination using SEM, EDX, TEM, IC, Auger, XPS & TOF-SIMS  Techniques". The proceedings from the 28th  International Symposium for Testing & Failure Analysis (ISTFA’2002), 3-7 Nov, Phoenix Civic Plaza, Phoenix, Arizona, USA, 495-504 (2002).


p 256-258


DOI: 10.1361/cp2003istfa256


## Advanced Process Defect Detection by Using Dynamic Bias Condition and MCT Camera


Advanced Process Defect Detection by Using Dynamic Bias Condition and MCT  Camera


Ching-Wei Wu and Jeng-Han Lee


Taiwan Semiconductor Manufacturing Company, Ltd., Taiwan


In this paper, a failure analysis case, which uses a dynamic  operation technique and MgCdTe (MCT) camera to isolate  single scan-chain failed cell is demonstrated. Improved results  obtained using the MgCdTe (MCT) camera is compared with  traditional Si CCD camera. Scan-chain cell schematic and  failure mechanism is also presented to explain why static bias  conditions are insufficient to detect this failure.


Defect isolation is the most critical step of IC failure analysis. The bias conditions to trigger the chip and sensitivity of the  emission detector are critical for fault isolation. A complete  triggering procedure for a scan chain failure is used in  conjunction with a sensitive MgCdTe(MCT) emission detector  for abnormal emission detection.


Case History


The device is fabricated by 0.13 um, 7-level metal (Cu) process technology. The device is a mask defect and always  failed at a fixed scan-chain. Further analysis in tester showed  that scan-out data was always stuck at low after a specific  clock cycle. A Metal1 mask issue was suspected since this  failure mode appeared after a new Metal1 mask was  implemented in the factory. Emission microscope analysis (both CCD and MCT camera) under static bias did not detect  any leakage path. A combination of dynamic operation  technique with emission microscope is then considered. In  order to enter scan-shift test mode, some control signals had to  be kept at proper DC level according to test mode control  table. Scan-shift clock was forced by a square wave with  correct voltage level. To simplify the setup environment, the  device is re-bonded on to a universal board. Control signals  are bonded to hold VDDQ or GND level with respect to their  control table. Scan-shift clock is bonded separately and forced  to 3.3 v, 100k Hz square wave signal by a function generator. The status of the scan-shift mode is verified by monitoring  scan-out result. This approach works well since scan-out data


follow scan-in data after specific clock cycle. Failure mode of  stuck at low is also verified (Fig.1).


Figure 1: The oscilloscope waveform plot of the scan-out data  stuck at low even though scan-in data toggles.


In order to create a leakage path, scan-in data is kept at VDDQ  and scan-shift clock is toggled to shift the scan-in data to the  failing DFF cell. At first, a Si CCD camera was used to locate  the failure site. Unfortunately, no abnormal emission could be  detected even with long acquisition time of 600 seconds. Low  sensitivity and noisy background of the CCD camera also  impaired failure site localization. (Fig.2). The MCT camera  was used to acquire emission under similar condition. Abnormal emission is distinguished clearly from background  noise (Fig. 3).


Figure 2: Backside emission image of 0.8X CCD camera  under dynamic bias condition.


Figure 3: Backside emission image of 0.8X MCT camera  under dynamic bias condition.  Abnormal hot spot is easily  identified.


Because it is field relative failure, abnormal hot spot should  always appear at the same site. This experiment was repeated  on other failing dice and hot spot was reproduced at the same  site. To further localize the defect, emission images using  higher magnification are then acquired. Emission images  acquired, with 30s acquisition time, using MCT camera and, with 600s acquisition time, using CCD camera are shown in  Figures 4 and 5 respectively. At 50X, it is impossible to  identify abnormal hot spot in the Si CCD camera image (Fig.4) without referring to emission image from the MCT  camera (Fig. 5). It is well known that the quantum efficiency  of CCD camera is poor when wavelength is longer than 1.1um , whereas the MCT camera is excellent in IR region.. A hot  spot from a metal short will be more easily visible when using


a MCT camera than CCD camera. In this case the failure  appeared after Metal1 mask change, a metallic short defect, which will induce thermal radiation is suspected. Failing units  were further deprocessed and a metal1 short issue is found at  emission site (Fig. 6).


Figure 4: Backside emission image of 50X MCT camera under  dynamic bias condition.


Figure 5: Backside emission image of 50X CCD camera under  dynamic bias condition. The abnormal hot spot is hard to  identify.


Figure 6: SEM image of emission located metal short.


Figure 7: Schematic of the emission located failure site. Metal1 short defect is represented by red dash line.


Schematic of emission located failure site is presented in  figure7. Circuit analysis shows metal1 short defect will not  induce leakage path under static bias condition. A transfer gate  on the leakage path and will block the leakage. Leakage path  will be ‘on’ and emission is observed only when Scan_Enable  signal activates this transfer gate.


In this work, the superiority emission sensitivity of the MCT  camera to the traditional Si CCD camera is demonstrated. The  root cause of the scan chain failure was isolated using the  MCT camera emission spot and identified by deprocessing.


p 259-261


DOI: 10.1361/cp2003istfa259


## Via Chain Failure Analysis Using a Combination of E-Beam and Optical Beam Techniques


Via Chain Failure Analysis Using a Combination of E-Beam and Optical  Beam Techniques


Srikanth Perungulam and Albert Gleason


Texas Instruments Inc., Stafford, TX


This paper outlines some of the optical and e-beam based  techniques that can be used to isolate via chain failures. The  Scanning electron microscope based techniques discussed are  Passive Voltage Contrast (PVC) and Substrate Current  Imaging (SCI). The optical beam technique discussed is  Thermally Induced Voltage Alteration (TIVA) on the Laser  Scanning Microscope. A combination of these techniques can  be used to effectively analyze all types of via chain failures.


Wafer fab yield improvement is often driven by failure  analysis performed on test structures or structures that are  specifically designed to help identify certain process issues. A  simple via chain structure is one of the commonly used  designs in wafer yield enhancement studies. The failure  analysis performed on the via chain failures helps direct  process improvements that can impact yields dramatically. This makes failure isolation on via chain failures extremely  critical.


Via chain structures are typically serpentine spanning two  metal levels interconnect runs connected by vias. The common  failure mechanisms are opens and high resistance in the chain.  Historically, the failure analysis community has used passive  voltage contrast for isolating these failures. However, this  technique is effective only when the chain has a very high  resistance. In this paper, we discuss the use of complementary  optical and Scanning electron microscope (SEM) techniques  that can help isolate the full range of interconnect failures.


Description of the test structure


The via chains that were analyzed for the examples discussed  in this paper were simple two level metal structures. The chain  consisted of 30 rows of 87 vias each. The vias were 0.6um in  diameter. The typical resistance for the chain was around  3KΩ. The Pass/Fail resistance limit for testing was set at 6KΩ. The range of chain resistances analyzed was from 6.7KΩ to


2MΩ. For the SEM based analyses, the passivation layer  above the top metal was removed. No sample preparation was  needed for the laser based analyses.


SEM based techniques


The simplest form of analysis on the SEM for via chain  failures involves using Passive Voltage Contrast (PVC). This  technique is very effective when there is a very high resistance  defect in the via chain. The contrast in image on the SEM is  obtained from the differences in secondary electron (SE) yield. The secondary yield is largely controlled by the sample bias. In the case of PVC, one end of the via chain is grounded. In  this case, the pad at one end of the chain was shorted to an  adjacent GND line using carbon paint.  The defect essentially  divides the structure into a grounded region and a floating  region. This difference in potential generates a different SE  yield from each of these regions and enables the failure  analyst to identify the location of the defect at the boundary  between the two regions. While this is most suitable for opens  or defects with extremely high resistance, varying the  accelerating voltage and the scan speed can, to some extent, help in the isolation of defects with lower resistances. Tilting  the sample improves the PVC as topography has a significant  impact on SE yield. The advantages of PVC are that it is very  quick and works well at low accelerating voltages (0.5kV2kV).


Figure 1: Low magnification SEM image showing PVC on a  via chain with two bad vias.


Figure 2: Higher magnification of location A on Fig. 1


The other SEM based technique that has proved to be effective  in via chain analyses is Substrate current imaging (SCI).  In  this case we use a single probe on one end of the via chain. The probe is connected to a current amplifier with an  amplification range of 1011. The structure acts as a current  divider as the electron beam is scanned across the sample. The  net current (beam current- SE- other losses) which is in the  pA-nA range is then amplified and fed to an auxiliary port on  the SEM to form the substrate current image (SCI). This  image is then superposed on the SE image. Since the defect  acts as a current divider, there is a distinct difference in the  SCI signal from one side of the defect to the other. Typically  the current is amplified to about 109 times. The downside to  amplifying the signal higher is the increased noise.


Figure 3: Schematic showing the Substrate Current Imaging  setup.


This technique can be used to analyze a larger resistance range  when compared to passive voltage contrast. However, there is  a need for higher voltages and larger apertures to  accommodate the need for higher beam currents. The example  in Fig. 4  shows the SCI image for a via chain with resistance ~ 7.5K. In the absence of a probe, the chain can be grounded  to the substrate and the substrate current is monitored.  The  method in which this technique was applied makes it a variant  of the Resistive Contrast Imaging (RCI) technique [1].


Figure 4: Combined SCI/SE image identifying the location of  the failure.


Laser based isolation


Laser based failsite isolation techniques [2,3] are becoming  increasing popular in the failure analysis industry. The  example discussed here utilized a Laser Scanning Microscope (LSM) equipped with a 1320nm heating laser. The schematic  for the LSM setup is shown in Fig. 5. As the laser scans over  the sample, there is a heating effect that locally changes the


resistance in the scanned region. The change in the resistance  is monitored. If the current source is held constant and the  voltage monitored, the technique is called Thermally Induced  Voltage Alteration (TIVA). The analogous current monitoring  method is called Optical Beam Induced Resistance Change (OBIRCH).  In this case, the structure was sourced using a  probe setup. The supply was held at a constant current and the  voltage was monitored. As the laser heats the defect, there is  an incremental change in the resistance which leads to a  change in the voltage with the constant current supply. This ∆V is then amplified and fed to an auxiliary input to the LSM. An AC coupled amplifier with low and high pass filters works  well for noise reduction. The optical image of the via chain is  superposed with the auxiliary image to obtain the coordinates  of the failure. Figures 6 and 7 show the results of TIVA  analysis on a via chain with resistance ~6.9kΩ. This technique  has proven to be very effective for defects over a wide range  of resistance. When the fail mode is an open, the physics  behind the localization of the defect changes. Opens failures  are usually detected as a result of Seebeck effect (Thermal  gradients resulting in voltage gradients) and hence the name  Seebeck Effect Imaging (SEI) [3].


Figure 5: Schematic showing the LSM with the 1320nm laser [1].


Figure 6: Low magnification TIVA image identifying the


failsite.


Figure 7: Higher magnification image showing the failsite.


The examples discussed above detail the use of SEM and laser  based isolation techniques for isolation of defects in simple via  chain structures. The SEM based techniques have excellent  spatial resolution and with the use of SCI, defects in the  medium to high resistance range can be isolated.  PVC is  quick and effective for defects with high resistance. While  PVC can be used at low SEM beam currents (and hence low  voltages), generally for SCI there is a need for higher beam  currents (larger apertures/higher accelerating voltages). The  failure analyst needs to be aware of the effects of higher beam  currents on the devices, especially for units with low K  dielectrics. SCI also requires the chain to be grounded to the  substrate or the use of a probe on one end of the chain. The  laser based techniques have the best resistance range but  relatively poor spatial resolution. Additionally, the 1320nm  laser can be used for failure isolation through the backside of  the device.  In conclusion, this suite of techniques ensures  effective failure analysis on almost any type of metal  interconnect test structure failure.


1: Cole Jr., Ed., Microelectronic Failure Analysis, 4th Edition (1999), pp133-167.


2: Nikawa K. and Inoue S., Proceedings of Sixth Asian Test  Symposium (1997) p219.


3: Bernhard-H K. et al, Microelectronic Failure Analysis, 4th  Edition (1999), pp487-503.


Constant I  supply


Image  Process


AC coupled  Amplifier


Display


1320nm


TV


Y


p 262-271


DOI: 10.1361/cp2003istfa262


## ESD Failure Signature Differences in the Devices Core Logic and Protection Structures -- A Case Study


ESD Failure Signature Differences in the Devices Core Logic and  Protection Structures -- A Case Study


Leo G. Henry, Ph.D


ESD-TLP Engineering Consultants


P.O. Box 1665 , Fremont, CA, 94538,  USA   (510).657.5252        FAX  510.657.9661


e-mail: leogesd@ieee.org


www.leogesd.com


For certain programmable logic type devices, the electrical, morphological and failure location differences in the ESD  signatures between ICC failures and I/O leakage failures  have been identified.  Based on these electrical, morphological and physical failure signature locations, this  case study confirms that distinctions can be made between  the signatures associated with the likely stress modes for  pin combinations like I/O-to-Vss,  I/O-to-Vcc, I/O-to-I/O, Vss-to-Vcc and Vcc-to-Vss.  This separation also facilitated  the correct identification of core failures which are mostly  due to the supply-to-supply pin combination stress, but in  some cases are due to the pin-to-supply tests.


Background


In the 1994 paper on ESD and EOS failure signatures [ 1 ] the authors were able to show not only the distinction  between the failures ascribed to Electrical Overstress (EOS) and the failures ascribed to Electro-Static Discharge (ESD), but also able to show the subtle differences (signature) between physical damage and location due to the various  ESD models.  These models are: the Human Body Model (HBM), the Machine Model (MM) and the Charged Device  Model (CDM).  In 1995 [ 2 ], other authors also reported  on the investigation of the signature differences between


these three ESD models in addition to their failure  threshold differences.   The 1994 (1] work was extended to  cover differentiating both the electrical and physical  morphological failures due to the various ESD pin  combination stress modes ( I/O-to-Vss,  I/O-to-Vcc, I/O-toI/O, Vss-to-Vcc and Vcc-to-Vss) for both the HBM and  MM ESD events.  In several publications [ 3-14 ] where  some pin combination ESD testing are described,  the  authors provide insight into the mechanisms associated  with various current flow directions (both positive and  negative pulses) through the whole chip.   In this paper, a  case study is presented on how to combine some of the  several individual methods used by the testing and failure  analysis community to differentiate between the failures  associated with the different pin combinations initiating the  failures.


The data obtained from this ESD laboratory simulation  were used to successfully improve the ESD immunity of the  programmable product.  The procedure was also  successfully applied to other products (different  technologies) from the factory for engineering and  qualification, and also to product returning  from the field  for analysis [ 15, 16 ].


The devices used in this study are a different revision of the  programmable logic device used in the previous study [1].  This CMOS product uses stacked NMOS and PMOS  transistors in the I/O circuit where the PMOS is the pull-up  PNP p-channel transistor and the NMOS is the pull-down  NPN n-channel transistor (figure 1 ).   It is well established  that most if not all internal/core operating structures of  most ICs must be protected from the very fast nanosecond  to picosecond type pulses which results from the many ESD  events.   Since “All Devices Are Not Created Equal”, it  follows then that there are many different types of ESD


protection structures in existence and their specific use  depend on the device technology.  However, it has been  shown [ 3 ] that ESD protection structures are so layout  intensive that in most cases they are not exactly portable  from one design to another.  In this figure 1, we see the  simplistic schematic of the output buffers where the 2  diodes (D1 and D2) are being used as protective elements, the forward biased D1 running parallel to the pull-up  circuitry and the reverse biased D2 running parallel to the  pull-down circuitry.  D is the drain and S is the source for  each transistor.


S                  D1


PMOS


To core                          D


NMOS      D2


Figure 1.  This CMOS output buffer shows the 2 protection diodes one in the pull-up (p-channel) PMOS and the other in  the pull-down (n-channel) NMOS transistors connected to both supply rails (Vdd and Vss).  Here, S and D are the  Source and Drains of the transistors.


The figure 2 below represents the well-established crosssectional process view of figure 1 showing the lateral PNP  and NPN transistors in the pull-up and pull-down circuitry  respectively.  These are parasitic elements that turn on  when ESD events “attack” the I/O pin.  The Drain “becomes” the Collector, the Source “becomes” the Emitter  and the substrate is the Base as the structure takes on a  bipolar device operation.  The Gs are the gates and the Rs  are the substrate resistances, where Rpu represents the  resistance associated with the pull-up transistor and Rpd  represents the resistance  associated with the pull-down  transistors respectively.


Vdd                                   I/O                                          Vss


G                                                    G


S                  D                               D                   S


p                 p                           n                    n


pnp                                                                                  npn


nwell              Rpu                    p-epi                 Rpd


p-substrate


Figure 2 is a cross sectional process view of •the same output buffers where the contacts to the Drain are connected to  the I/O pad. This cross section of the full CMOS device shows the lateral parasitic transistors (PNP and NPN) associated  with the PMOS and the NMOS devices.


Experimental – ESD Stressing


HBM and  MM ESD stress testing were carried out using  the ESDA Standards STM-5.1 [  17 ] and STM-5.2 [  18 ] respectively.  All units were data logged both before and  after the stress testing such that any leakage current equal  or greater than 500 nano amps (0.5 uA) was flagged.   ESD  stress was applied to the devices (figure 3)  using +/- 3 zaps  with 1.00 second delay between pulses. This was used for


the 7 voltage levels starting at 125V and ending at 4KV.  The pin combination procedure followed that described in  the ESDA HBM and MM standards.  The Five distinctive  pin combinations of I/O-to-Vss, I/O-to-Vcc, I/O-to-I/O, Vss-to-Vcc and Vcc-to-Vss were used.  This procedure  allows for the separation of failures for I/O-to-power supply (Vss and Vcc)  from those failures that may occur  between  the actual power pins (Vss-to-Vcc and Vcc-to-Vss).


CPU has four different analog PS’s (VCCA (0-3)) pins. CDM  ESD margin characterization was performed by stressing each  VCCA pin separately. The applied stress started from 300V  and reached 800V with 100V steps. All pins except VCCA (0-3) passed 800V CDM ESD stress without failures and passed  qualification requirements. VCCA pins showed shorts after  ESD CDM stresses of different voltage levels. The VCCA  pins have three high voltage tolerant PMOS clamps for ESD  protection [9]. PMOS clamps are 3 huge (~50x70 microns) transistors [8], which are dedicated to providing a current path, and have to withstand the ESD event. Layout analysis shows  that in parallel to each VCCA PS there is a set of  NMOSFET’s with gates tied to ground. These node area  control diodes with grounded gates (so-called GNACs) are  used as process charge protection devices [9]. Similar GNAC  transistors are used as ESD protection devices as well [10]. In  our case, GNAC transistors consist of ten parallel antenna  diodes, which are connected to the huge M5-M6 antenna. They are not functional during regular chip operation, and are  used at the chip production step as a discharge path for  antenna charging. GNAC design layout and positioning are  driven primarily by reliability requirements to prevent process  charge degradation. These structures can be inherently weak in  terms of ESD and EOS. During both process charge and ESD  events the device operates as a parasitic bipolar transistor. From a comparison between the different combinations of  antennas and process charge protection devices [13] it is  obvious that the holding current It2 is a design and process  charge dependent parameter. It has also been found that It2  decreases with decreasing of transistors channel length, Leff  and threshold voltage, Vth. The It2 is lower for NMOSFET’s  with longer metal lines connected to the gate or/and to the  drain. In the failed devices, EOS/ESD damage has been found  at M4 level (see Fig. 5a) and below, down to silicon (see Fig. 5b). 800V stress causes EOS damage on the GNAC-transistors  and a one of three p-clamp transistors. 500V and 600V  stresses cause EOS damage on GNAC-transistors, although pclamps are not damaged. The assumption was made that  GNAC transistors react to ESD zaps faster than p-clamps  which are placed in parallel with GNACs. To prove this  assumption, GNACs were disconnected from the PS’s using  focused ion beam (FIB) circuit microsurgery. The FIB-ed  units passed the spec CDM ESD requirements (800V) with a  slight shift on some PS’s and I/O pins. This change was then


implemented to the chip design for the A1 product step.


Parametric failures


This kind of failure in 0.18µm products is found to be  associated with  gate oxide (GOX) breakdown in a capacitor  connected in parallel to the failing PS. The example of GOX  breakdown observed in MOS decoupling capacitors is shown  in Fig. 2b.


Figure 6. A schematic cross-section of the affected decoupling  capacitor during an ESD event


During a high current CDM ESD event the doped poly-silicon


gate material is injected into the substrate through the weak


point in the broken gate oxide. As a result, a local defective pn junction formes. This kind of defect is shown schematically


in Fig. 6.


During 0.13µm products ESD qualification, a degradation of


PS’s, which results in PS leakage increase caused by CDM


ESD stress, has been observed. The I-V characteristics before


(green) and after (red) 400V ESD CDM stress are presented in


Fig 7.  To find CDM ESD margins the stress was applied only


to one of the four VCCA analog PS pins. Table 1 represents


the failing stress voltage scattering for VCCA pins. The


majority of the units passed the ESD criterion (-800V) and


were not sensitive to the CDM ESD event. However, a


number of units failed at lower stress level. Thus, it was


necessary to know what determines the level of sensitivity to


CDM ESD stress for the given protection circuit design.     After the preliminary layout investigation, the initial


conclusion was reached that this is a GOX related failure.


Process charging at the back-end process stage caused the


GOX weakening. The large charging current flows through the


GOX to the gate, which is grounded to the source tied to VSS


[11]. During subsequent ESD stress these weak GOX points


got damaged and failed.  Thus, the root cause of the failure is


the high charging current coming from the drain terminal of


the GNAC's due to a large area of metal lines run in M6, M5


and M4 layers (antennas) connected to the  GNAC’s drain


node (see Table 1).  VCCA(3), which has the larger M4-M6


antenna, failed at lower ESD stress levels. The variations from


unit to unit in initial (prior to the stress) I-V characteristics of


VCCA PS pins were observed (Fig.8). This variation could be


attributed to a different initial trap level created by process


charging.


Figure 7. VCCA PS I-V curves before (green) and after -400V  CDM ESD stress (red).


Table 1: Results of VCCA PS’s ESD margin study


PS Pin M4,          sq.micron M5 and M6, sq. micron CDM worst,   V CDM best, V  VCCA(0) 10,419


131,000


300


>2000


VCCA(1) 8,075


55,500


VCCA(2) 6,361


38,900


VCCA(3) 44,616 1,480,000


600


Figure 8. I-V characteristics for one of VCCA PS’s measured  on three different units prior to the CDM ESD stress (green) and after the stress (red)


Shorts between isolated analog PS and VCC core PS


This kind of failure is associated with a breakdown in NMOS  capacitor or NMOSFET accidentally connected between the  failing PS’s.  Fig. 3b represents this case for a 0.18µm  product. It is essential to note, that both core and analog PS’s  were protected by PMOS clamps, which weren’t properly  operating during the EDS event. As a rule, these special  protection structures effectively shield sensitive circuits by  diverting current away   through the well-established robust  paths. Therefore, the last failures can be identified as “freak” failures. “Freak” failures by definition [10] are the failures  which are not observed for standard processing and design  parameters, but are the result of some deviation in the  manufacturing process or error in the design itself. In the  considered example the ESD stress applied to VCCHA or to  VCCGA pins resulted in shorts between VCC core and analog  PS’s. However, the direct zap to core PS’s pins and core I/O


pins didn’t cause the failure up to the 800V stress level. It was  found that for both 0.18µm and 0.13µm products, the analog  PS failures were caused by a breakdown in an NMOS  capacitor or NMOSFET between the failing PS’s and VCC  core PS.  When the failing capacitor or NMOSFET was  disconnected from the PS’s by FIB microsurgery, the units  passed the spec CDM ESD requirements (800V).


Recoverable failures


This kind of failure is found to be associated with consecutive  development of ESD damage during several ESD zaps and  extension of the damage to the upper metallization above the  failing structure. The first zap causes an ESD short with  respect to ground. The next zaps lead to EOS-like damage  development, melting of contacts and metallization along the  high current path, and finally, to total disconnection of the  failing structure. I-V characteristics will return to the normal  shapes (recovered) if the failing structure is not operating  during normal chip operation (as GNAC for example). Fig.9  represents this kind of failure in a 0.18µm product. Recovery  in this case can be attributed to charge-discharge processes, which leads to the creation of opens between PMOS clamps  and GNAC. Additional ESD stress on the recovered pins  doesn’t degrade I-V characteristics.


Figure 9. Voids in the damaged contacts caused by CDM ESD  stress (700V, 3 zaps, 0.3 seconds between zaps).


A detailed analysis of various electrical signatures occurring  after ESD CDM stress and their associated failure modes are  presented and discussed. The above results were obtained  during a study of 0.18µm devices and were successfully used  in 0.13µm products qualification. The conformities we found  helped us to elicit charge related problems and their influence  on ESD performance, and to reveal interaction between ESD  protection circuits and charging-protection device (GNAC) failures. In conjunction with physical FA data one can  conclude the following correlations between electrical  characteristics and CDM ESD caused failure modes:


1. A short between PS and ground is associated with  fulmination, resulting in damage between two adjacent  diffusions in a small NMOSFET connected in parallel to the


PS.


2. PS pin shift is associated with GOX breakdown in a  capacitor connected in parallel to the PS.


3. A short between isolated PS’s is associated with breakdown  in NMOS capacitor or an NMOSFET connected between  these PS’s.


4. A disconnection of a scheme that determined an alternative  current pass from the PS bus results in FT failures with no  changes in I-V characteristics of the corresponding pins.


The authors gratefully acknowledge their Intel coworkers: Ana  Faingold for ESD tests executions, Gila Yampolski and Roni  Schneider for help in FA work. The authors also acknowledge  fruitful discussions and valuable suggestions by Dr. Tim  Maloney.


1.    A. Amerasekera, W.van den Abeelen, L. van Roozendaal, M. Hanneman, P. Shofield, “ESD failure modes: Characteristics, mechanisms and process influences”, IEEE Trans. Electron Devices, 39, 430-436 (1992)


2.  B. Lisenker, “Process influence on product CDM ESD  performance”, Microelectronics Reliability, 43, 1029-1037(2003)


3.    Sanjay Dabral, Timothy J. Maloney, “Basic ESD and I/O


Design”, John Wiley & Sons, Inc. 1998.


4. Koen Vernaege, “Component Level ESD testing”,


Microelectron. Reliab., 38, 115-128 (1998)


5.   Andrew H. Olney, “Using Charge Device Model Testing


to eliminate Real-World ESD Failures”, Microelectron.


Reliab. , 38, 129-143 (1998)


6.  Leo G. Henry, “Differentiation between EOS and ESD


Failures for ICs”, Microelectronic Failure Analysis Desk


Reference Fourth Edition, p.421-436, ASM International


(1999)


7.  Schafft H.A. “Second-Breakdown – A Comprehensive


Review”, Proc. IEEE, 55, 1272 (1967)


8.  T.J. Maloney, “Designing power supply clamps for


electrostatic discharge protection of integrated circuits”,


Microelectronics Reliability, 38, 1691-1703 (1998)


9.  Kin P. Cheung, “Plasma Charging Damage”, IRPS 97


Tutorial Notes, Topic 4


10. Charvaka Duvvury and Ajith Amerasekera, “ESD: A


Pervasive Reliability Concern for IC Technologies”,


Special Issues on VLSI Reliability, IEEE Proceedings,


690-702, May 1993


11. Y. H. Lee. K. Wu, G. Sery, N. Mielky, and W. Lin,


“Reliability Characterization of Process Charging Impact


on Thin Gate Oxide”, International symposium on Plasma


Process-Induces Damage, 98, (1998)


p 278-281


DOI: 10.1361/cp2003istfa278


SEMI-AUTOMATED CROSS-SECTION PREPARATION PROCESS FOR COMPLEX MULTI-FACE  PERIMETER SAMPLES


Todd McDonald


Intel Corporation, Hillsboro, Oregon, USA


The fixed position sample mover plates currently offered to  the industry only facilitate two sided grinding and polishing. 3  and 4-sided requests cannot be accommodated with these  fixed position mover plates.  Ultimately this means performing  some or all of the work manually. Described here is a fixture  and process solution that makes semi-automation possible  through the entire process.


The latest grinding/polishing equipment utilizes pneumatic  pistons that extend to make contact with the top of the sample  forcing it against the grind/polish media.  These machines use  fixed holes in mover plates in which samples are placed.  The  challenge is that when grinding more that two sides, a sample  will be shrinking in dimension while the sample holes in the  mover plate stay exactly the same dimension thereby allowing  excessive sample movement. The results of this are often  dramatic, leaving intact solder balls at one end of a sample  while at the other end, the solder balls may be completely  gone.


Here is a solution using a spring plunger design that  continually compensates for the material removed from the  sample by maintaining firm pressure via spring/plunger action  to hold the sample in place. The information presented in this  paper is organized as follows:


1. An equipment and materials list of items needed to build  this solution and process samples with it.


2. A general guide explaining how to create the adjusting  mover plate, including the mechanical challenges and  limitations to consider when building this fixture.


3. A description of the 5 basic process steps required to  achieve good results using this fixture design.


4. Examples of typical results provided.


Equipment & Materials List


•  (Qty = 1) Struers Rotopol 31 Grinder/polisher base unit      with Roto-force 4 head [1]


•  (1)  Round 150 mm Diameter mover plate [2]


•  (1)  Mover plate shaft and mounting screws [1]


•  (3)  Piston catch caps [2]


•  (6)  Piston catch cap Allen screws


or spring plungers [2]


•  (6)   Spring/plunger bodies [2]


•  (12) Spring/plunger body screws [2]


•  (6)   Light gauge springs [3]


•  (3)   Molds cut from square/rectangle steel tubing  [2]


Building the adjustable sample mover plate


Fabricate a 150mm diameter round sample mover plate.  In the  center of the sample mover plate 3 mounting holes are  required for fastening the vendor-supplied shaft that inserts  into the grinders mover head. It may be necessary to modify  the shaft length to work effectively with the sample height and  piston lengths on the grinder’s mover head.  It is critical that  the shaft be short enough that the pistons make contact with  the sample tops and continue providing adequate pressure  during processing.


Next determine the maximum size, both length and width, of  the samples that will be processed in this fixture. Then  machine 3 cut out spaces in the mover plate, 0.81mm larger  than the samples to be processed in the fixture. Before  marking and cutting the sample spaces, insert the mover plate  into the machine head and activate the pistons from the head  to see where they will contact the samples. The sample needs  to be centered beneath the pistons for even grinding. Use this  information to locate and cut out the sample spaces in the  mover plate.  3 sample holes fit on one mover plate.


Have 6 spring and plunger body units machined out of  aluminum stock. Each plunger body needs two mounting holes  and a journal to accommodate the spring and plunger. See  Figure 1. Place a small light gauge coil spring and an


aluminum plunger inside the channel of each spring/plunger  housing body. Each aluminum plunger will need material  machined from the center of the tip to avoid contact and  damage to the delicate microstructures on the samples they  will be contacting. See Figure 1. Mount two of these  spring/plunger bodies on opposite ends of each sample hole in  the mover plate.


Figure 1. Photograph of mounted spring/plunger body.  Note  the notch in the end of the plunger.


Next, fabricate 3 aluminum piston catch caps that will  facilitate full contact from the pistons in the grinder head.  See  Figure 2. This is necessary because most 4-sided samples are  not long enough for the grinder pistons to make full contact. The catch caps are also designed to support the sample only at  the edges, while the remainder of the sample avoids contact  with the cap so that the cap does not scratch the delicate  sample surfaces. These aluminum caps use adjustable Allen  screws with soft plastic plunger tips or spring-loaded plungers  to hold the samples in place via pressure from the sides.  With  these elements constructed, the fixture is ready to process  samples.


Processing multiple face samples


Pot multi face components in square or short rectangle molds  See Figure 3. The critical detail here is to avoid a lot of excess  epoxy which equates to greater grind distance.  Ensure there is  equal space and material on all four sides of the component.


Place the samples into the spring loaded fixture by placing one  edge against a spring and plunger and compressing it, then  dropping the other corner into place. See Figure 4. If this is  too difficult, the spring is too strong or it is necessary to  shorten the plunger length. Load all 3 samples into the fixture. See Figure 5.


Figure 2. Photograph of a Piston catch cap with Allen screws


and spring loaded plastic plunger tips.


Figure 3. Photograph of steel mold and potted sample


.    Figure 4. Photograph of sample being loaded into fixture.


Figure 5. Photograph of a mover plate loaded with three  different sample sizes.


Figure 6. Photograph of piston catch caps with loaded  samples.


Attach the catch caps to the tops of each sample. See Figure 6. Attach the sample fixture to your grinding machine by


inserting the shaft end into the receptacle in the mover head.  See Figures 7a and 7b


1) Grind using 220 grit media until just before exposing the


beginning of the solder balls.  If the grinding is progressing  unevenly at this step, manually correct or rotate until even  results are achieved. The idea is that sometimes a pneumatic  piston may be out of calibration and applying slightly more  force to one side of the sample or due to material differences  along the length of a component or other variables the  component may wear at a quicker rate on one side causing it  to be uneven.  This is usually minor and if corrected early  before making contact with the solder balls, it will stay


Figure 7a. Photograph of mover plate and shaft inserting into  mover head on the grinder.


Figure 7b Photograph of fully assembled fixture, loaded with  samples, inserted into the Mover head


relatively even through the remainder of the processing.  Rotate the entire sample and process the next face using 220  grit media.  Continue to repeat this process rotating until all  intended faces have been processed with 220 grit paper.


2) Change to 500 grit media and grind about ¼ of the way into  the balls checking along the way to make sure they are  grinding evenly.  Correct if necessary.  Rotate and process  each face using 500 grit paper. Rinse samples and fixture well.


3) Change to 1200 grit paper and grind each face to the center  of the balls. It would be a rare occasion to need any correcting  on this step. Rotate and process each additional face with 1200  grit paper.   Rinse samples and fixture well.


4) Process all samples on all faces using 6-micron diamond  suspension fluid followed by 1-micron diamond suspension


fluid then followed by either OP-S or Colloidal Alumina final  polish solution. Rinse samples and fixture between micron and  final polish steps.


Typical results


Figure 8. Photograph showing 2 polished


faces of a 4-sided sample.


Figure 9. Photograph shows a magnified view of typical ball  from figure 6.


Using this fixture and the outlined process will deliver quality  results for multiple face cross sections within a single sample. The challenges this solution has addressed are sample quality  and the processing limitations that multi-side requests present. A well optimized fixture will be capable of grinding and  polishing to a depth of 5 or more perimeter rows on four faces


before running out of pneumatic piston and plunger travel to  maintain pressure.  These essentials provide a functional  model from which to modify and tune for individual specific  needs.


The Author would like to thank Gary Shade and Bill  Cunningham of Intel Corporation for their Mentorship in  preparing this manuscript. Also acknowledge the valued input  from session chair Sandra Delgado.


[1] Struers Logitech Inc.  Westlake, Ohio USA.


[2] DMI International Machining. Cornelius, Oregon USA.


[3] Ace Hardware. Aloha, Oregon USA.


p 282-287


DOI: 10.1361/cp2003istfa282


FIB Micro-pillar sampling of Si devices and its 3D observation


T. Yaguchi, T.Kamino


Hitachi Science Systems, Ltd., 11-1 Ishikawa, Hitachinaka, Ibaraki 312-0057 Japan


T. Ohnishi, T.Hashimoto


Hitachi High-Technologies Corp., 882 Ichige, Hitachinaka, Ibaraki, 312-8504 Japan


K. Umemura


Central Research Laboratory Hitachi Ltd., Kokubunji,185-8601 Japan


K.Asayama


Renesas Technology Corp., 20-1 Josuihon-cho 5, Kodaira, Tokyo 187-8588 Japan


A novel technique for three-dimensional structural and  elemental analyses using a dedicated focused ion beam (FIB) and scanning transmission electron microscope (STEM) has  been developed. The system employs an FIB-STEM  compatible sample holder with sample stage rotation  mechanism. A piece of sample (micro sample) is extracted  from the area to be characterized by the micro-sampling  technique [1-3]. The micro sample is then transferred onto the  tip of the stage (needle stage) and bonded by FIB assisted  metal deposition. STEM observation of the micro sample is  carried out after trimming the sample into a micro-pillar 2-5  micron squared in cross-section and 10 -15 micron in length (micro-pillar sample). High angle annular dark field (HAADF) STEM, bright field STEM and secondary electron microscopy (SEM) images are obtained at 200kV resulting in threedimensional and cross sectional representations of the microsample. The geometry of the sample and the needle stage  allows observation of the sample from all directions. The  specific site can be located for further FIB milling whenever it  is required. Since the operator can choose materials for the  needle stage, the geometry of the original specimen is not a  limiting factor for quantitative energy dispersive X-ray (EDX) analysis.


New materials such as electronic and semiconductor devices  have been moving toward higher integration and density and  their sizes are expected to continue shrinking. In  characterization or failure analysis of these materials and  devices, requirements for analytical TEMs are rapidly  increasing. FIB technique is becoming more prevalent for  sample preparation of specific areas of interest for TEM  investigation [4]. The FIB technique has advantages in every  step of the sample preparation procedure, including specifying  the milling area, monitoring the milling procedure, and  confirming the finally thinned area. Each step is carried out


with the help of scanning ion microscopy (SIM) image  observation.


An FIB-based sample preparation technique has the unique  ability to make site-specific TEM specimens available directly  from bulky samples [1-2]. In addition, the technique allows  cross-sectional and plan view TEM sample preparation from  the same initial material. Usually a sample should be thinned  to a thickness of 0.1 micron or less for TEM observation. However, structural information obtained from such a thin  film is two-dimensional, and it is difficult to characterize  complicated structures in electronic devices.


This paper describes a novel technique for preparation of a  piece of pillar shaped sample (micro-pillar sample) and its  three-dimensional characterization using the FIB-STEM  compatible 3D-observation sample holder.


Materials and method


Instruments used in the study are the Hitachi FB-2100 FIB  system and the HD-2300 200kV STEM. The FIB system is  attached with a mechanical probe made out of W, which is  used to extract the micro sample. An FIB-STEM compatible  3D-observation holder has been newly developed for this  study. An external view of the FIB-STEM compatible 3Dobservation holder is shown in Figure 1. The holder can be  used for both sample milling in the FIB system, and image  observations in the STEM. The holder has a stage rotation  mechanism that permits insertion of a needle shaped sample  stage on the rotation center. The needle stage has a flat tip  with a diameter of about 30 microns for mounting micro-pillar  samples (Fig. 2).  Since the operator can choose the material  used to construct the needle stage on which a micro-pillar  sample is mounted, background peaks from the stage will not  interfere in quantitative elemental analysis using energy  dispersive X-ray (EDX) systems. A schematic of the micropillar sample mounted on a needle stage, which is inserted on  the rotation mechanism, and its position and orientation  relative to the electron beam and the FIB are illustrated in  Figure 3. Since the sample is located at the center of rotation


and tilting axes, the sample does not shift during rotating or  tilting operations.


Figure 1: External View of the FIB-STEM compatible 3D


analysis specimen holder.


Figure 2: Tip of the needle stage.


Figure 3: Micro-pillar sample on the FIB-STEM compatible  3D analysis holder.


Figure 4 shows a schematic flow for the FIB micro-pillar  sample preparation technique.  A micro- sample is extracted  from a bulk material (a). The micro sample is then transferred  onto the tip of the needle stage and bonded by FIB assisted  metal deposition (b). The sample is then trimmed in the form  of a pillar-shaped sample (micro-pillar sample) of 2-5 micron  square and 10 -15 micron long (c). All of these operations are  accomplished inside the FIB system. In the case of a Si-device, it takes less than 30 minutes to prepare. A secondary electron (SE) image of a micro-pillar sample of a Si device mounted on  the needle stage is shown in Figure 5.


Figure 4: Schematic flow for the FIB micro-pillar sampling  technique.


Figure 5: SE image of a micro-pillar sample of a Si-device.


The method described above was applied to characterize  DRAM device. The micro-pillar sample was about 2.5 micron  square in base area. Figure 6 shows a series of SIM images  showing the procedure for the FIB micro-pillar sample  preparation. Firstly, the surface area to be characterized is  coated with an FIB assisted W deposition (a). A groove  surrounding the area to be examined is milled leaving a microbridge (b). Next, the sample is tilted and the bottom is milled


FIB STEM


changeover knob(safety lock)


DC motor


} P @ u O ˇ ˚ ^


@30um @


Rotation  mechanism


e -


Needle stage Micro-pillar


sample


¿


(a) Lifting out


Metal probe


2 5̀um


(b) Mounting


(c) FIB trimming


W-deposition


Needle stage


Micro pillar sample


by FIB (c). The sample is tilted back, and the W-probe of the  micro-sample unit is bonded on the surface of the sample by  W-deposition (d). The micro-bridge is then cut off for lift out


(e) and the micro-sample is transferred onto the tip of the  needle stage by manipulating the W-probe. The micro-sample  is bonded onto the tip of the needle stage by W-deposition (f). After bonding, the W-probe is cut off by FIB milling (g). The  micro-sample is then trimmed for making a micro-pillar  sample suitable for 3D observation. (h).


Figure 7 shows a dark field (DF) STEM (a) and SE (b) images


of a 2 micron-square micro-pillar sample of a DRAM structure  observed from the same direction. Though the sample is 2  microns thick, DF-STEM image provides fine structures of  capacitors as well as the metal lines inside the sample (a). SE  image (b) offers cross-sectional structures of components near  the cross-sectional surface clearly.


Figure 8 shows a piece of hemi-spherical grain (HSG) capacitor by SE (a, d, g), DF-STEM (b, e, h) and BF-STEM(c, f, i) viewed from three different directions. The shape and fine  structures of a capacitor are obtained three dimensionally.


Figure 6: Series of SIM images showing the procedure for the FIB micro-pillar sampling.


500nm


Figure 7: DF-STEM(a) and SE(b) images of  a 2 micron-square micro-pillar.


b) Trench milling


c) Bottom cutting


d) Probe bonding


e) Extracting


f)  Mounting


g) Probe cutting


h) Trimming


10um


W deposition


5um


W-probe


a) W-deposition

