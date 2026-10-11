---
title: "ISTFA-2002 - Part1.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_4fb7461f82ff6347c81fb068e0751b5d7295230462135641
file_size: 72930686
---

ISTFA2002


Proceedings ofthe


28th International Symposium for


Testing and Failure Analysis


3-7 November 2002


Phoenix Civic Center


Phoenix, Arizona


Sponsored by


EDEAS Electromic Devica Fallore Amalyals Society As Amiate Society of ASM Intermational


"= 1SIt;4/2002~


Published by


ASM International


Materials Park, Ohio 44073-0002


Copyright © 2002


by


ASM International@


All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any means, electronic, mechanical, photocopying, recording, or otherwise, without the written permission of the copyright owner.


First printing, October 2002


Great care is taken in the compilation and production of this book, but it should be made clear that NO WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN CONNECTION WITH THIS PUBLICATION. Although this information is believed to be accurate by ASM, ASM cannot guarantee that favorable results will be obtained from the use of this publication alone. This publication is intended for use by persons having technical skill, at their sole discretion and risk. Since the conditions of product or material use are outside of ASM's control, ASM assumes no liability or obligation in connection with any use of this information. No claim of any kind, whether as to products or information in this publication, and whether or not based on negligence, shall be greater in amount than the purchase price of this product or publication in respect of which damages are claimed. THE REMEDY HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND SOLE REMEDY OF BUYER, AND IN NO EVENT SHALL EITHER PARTY BE LIABLE FOR SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES WHETHER OR NOT CAUSED BY OR RESULTING FROM THE NEGLIGENCE OF SUCH PARTY. As with any material, evaluation ofthe material under end-use conditions prior to specification is essential. Therefore, specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or reproduction, in connection with any method, process, apparatus, product, composition, or system, whether or not covered by letters patent, copyright, or trademark, and nothing contained in this book shall be construed as a defense against any alleged infringement of letters patent, copyright, or trademark, or as a defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN: 0-87170-771-3


SAN: 204-7586


Materials Park, OH 44073-0002


www.asminternational.org


Printed in the United States of America


Multiple copy reprints of individual articles are available from Technical Department, ASM International.


ISTFA 2002 Organizing Committee


Christian Boit


General Chair


University of Technology Berlin Berlin, Germany


Thomas M. Moore


Vice General Chair


Omniprobe, Inc.


Dallas, TX


Richard J. Ross


Past General Chair


IBM Microelectronics Essex Junction, VT


Matt Thayer


Symposium Technical Program Chair


Advanced Micro Devices Austin, TX


Cheryl Hartfield


Audio / Visual Chair Texas Instruments Dallas, TX


Lee Knauss


Publicity Chair


Neocera


Beltsville, MD


Anu Barman


Exposition Chair


Foveon, Inc.


Santa Clara, CA


Ingrid DeWolf


Panel Discussion & User Group Chair IMECvzw


Leuven, Belgium


Jerry M. Soden


Seminar Chair


Sandia National Laboratories


Albuquerque, NM


iii


EDFAS 2002 - 2003 Board of Directors


|Richard J. Ross |Christian Boit |
|---|---|

|EDFAS President |Director-At-Large |

|IBM Microelectronics Division |University of Technology Berlin |

|Essex Junction, VT |Berlin, Germany |

|Edward I. Cole, Jr. |Sandra Delgado |

|EDFAS Immediate Past President |Director-At-Large |

|Sandia National Laboratories |Accurel Systems International |

|Albuquerque, NM |Sunny vale, CA |

|Gary F. Shade |Jim Erickson |

|EDFAS Vice President |Director-At-Large |

|Intel Colorado Springs Design Center |Boeing Satellite Systems |

|Colorado Springs, CO |Los Angeles, CA |

|Daniel L. Barton |Charles F. Hawkins |

|EDFAS Secretary |Director-At-Large |

|Sandia National Laboratories |University of New Mexico |

|Albuquerque, NM |Albuquerque, NM |

|Glen P. Gilfeather |Jacob C. H. Phang |

|EDFAS Financial Officer |Director-At-Large |

|Advanced Micro Devices |National University of Singapore |

|Austin, TX |Singapore |

EDFAS 2002 - 2003 Committee Chairs


|ASM Board of Trustees Liaison |EDFAS Website Committee |
|---|---|

|Reza Abbaschian |Jerry Soden, Chair |

|University of Florida |Sandia National Laboratories |

|Gainsville, FL |Albuquerque, NM |

|EDFAS Membership Committee |EDFAS Events Committee |

|Seshu Pabbisetty, Chair |Christian Boit, Chair |

|Texas Instruments |University of Technology Berlin |

|Stafford, TX |Berlin, Germany |

|EDFAS Nominations Committee |EDFAS Education Committee |

|Edward I. Cole, Jr., Chair |Gary Shade, Acting Chair |

|Sandia National Laboratories |Intel Colorado Springs Design Cente |

|Albuquerque, NM |Colorado Springs, CO |

|EDFAS Publications Committee |EDFA Magazine Committee |

|Terence Kane, Chair |Chuck Hawkins, Chair |

|IBM Microelectronics Division |University of New Mexico |

|Hopewell Junction, NY |Albuquerque, NM |

|AV Committee ||

|Cheryl Hartfield, Chair |Texas Instruments, Dallas, TX |

|Ed Keyes, Co-Chair |Semiconductor Insights, Ottawa, Ontario, Canada |

|Mikel Miller |Intel Corporation, Chandler, AZ |

|Zhiyong Wang |Intel Corporation, Chandler, AZ |

|Todd McMullin |Texas Instruments, Dallas, TX |

|Jim Colvin |Jim Colvin ConSUlting Services, Newark, CA |

|Tom Moore |Omniprobe, Inc., Dallas, TX |

|Panel Discussion Committee ||

|Ingrid DeWolf, Chair |IMECvzw, Leuven, Belgium |

|Steve Ferrier |Metatech Corporation, Corvallis, OR |

|Joseph Bernstein |University of Maryland, College Park, MD |

|Chuck Hawkins |University of New Mexico, Albuquerque, NM |

|Gay Samuelson |Intel Corporation, Chandler, AZ |

|Christian Boit |University of Technology Berlin, Berlin, Germany |

|Seminar Committee ||

|Jerry M. Soden, Chair |Sandia National Laboratories, Albuquerque, NM |

|Kendall Scott Wills, Co-Chair |Texas Instruments, Stafford, TX |

|Susan Li |Advanced Micro Devices, Sunnyvale, CA |

|Catherine Marcey |Intel Corporation, Folsom, CA |

|Brent Wahl |Agilent Technologies, San Jose, CA |

|Jeremy A. Walraven |Sandia National Laboratories, Albuquerque, NM |

|Brad Waterson |Analog Devices, Cambridge, MA |

|William E. Vanderlinde |Laboratory for Physical Sciences, College Park, M |

|User Group Committee ||

|Paiboon Tangyunyong |Sandia National Laboratories, Albuquerque, NM |

|Alan Street |Integrated Reliability, San Diego, CA |

|Tom Paquette |Insight Analytical Labs, Inc., Colorado Springs, CO |

|Kartik Ramanujchar |Texas Instruments, Stafford, TX |

|Seshu Pabbisetty |Texas Instruments, Stafford, TX |

|K.N (Bobby) Hooghan |Agere Systems, Allentown, PA |

|William Vanderlinde |Laboratory for Physical Sciences, College Park, M |

|Jim Colvin |Jim Colvin Consulting Services, Newark, CA |

|Andy Erickson |Multiprobe Inc., Santa Barbara, CA |

|Advanced Techniques |Committee |

|Lee Knauss, Chair |Neocera, Inc., Beltsville, MD |

|Kendall Scott Wills, Vice Chair |Texas Instruments, Stafford, TX |

|Ted Levin |IBM, Essex Junction, VT |

|Tony Peterson |Intel Corporation, Hillsboro, OR |

|Jan Gaudestad |Neocera, Inc., Beltsville, MD |

|Edward I. Cole, Jr. |Sandia National Laboratories, Albuquerque, NM |

|Charles Zhang |Advanced Micro Devices, Austin, TX |

|Die Level Fault Isolation ||

|Dave Vallett, Chair |IBM Microelectronics Division, Essex Junction, VT |

|Ted Hasegawa, Co-Chair |National Semiconductor, Santa Clara, CA |

|Jim Cargo |Agere, Allentown, PA |

|Moyra McManus |IBM, Yorktown Heights, NY |

|Travis Eiles |Intel Corporation, Santa Clara, CA |

|Aaron Falk |Optometrix, Inc., Renton, WA |

|Jerry Soden |Sandia National Laboratories, Albuquerque, NM |

|Tam Le |ST Microelectronics Inc., Carrollton, TX |

|Siva Kolachina |Texas Instruments, Stafford, TX |

|Rama Goruganthu |Advanced Micro Devices, Austin, TX |

|Discretes, Passive ||

|Jim Erickson, Chair |Boeing Satellite Systems, Inc, Los Angeles, CA |

|Stan Silvus |Southwest Research Institute, San Antonio, TX |

|Gary Molle |Kaiser Electronics, San Jose, CA |

|Mike Cozzolino |Boeing Satellite Systems, Los Angeles, CA |

|Gary Ewell |The Aerospace Corporation, Los Angeles, CA |

|Massimo Vanzi |Universita' di Cagliari, Cagliari, Italy |

|Failure Analysis Process ||

|Christopher Henderson, Chair |Sandia National Laboratories, Albuquerque, NM |

|Steve Ferrier, Co-Chair |Metatech Corporation, Corvallis, OR |

|Tom Libbey |National Semiconductor, Arlington, TX |

|Hei-Ruey Harry Jen |MIA-COM Tyco Electronics, Lowell, MA |

|George Gaut |Conexant Systems, Inc., Newport Beach, CA |

|Edward Keyes |Semiconductor Insights, Inc., Ottawa, Ontario, Canada |

|MEMS ||

|Jeremy Walraven, Chair |Sandia National Laboratories, Albuquerque, NM |

|Roland Muller-Fiedler |Robert Bosche GmbH, Stuttgart, Germany |

|Susanne Arney |Bell Labs, Lucent Technologies, Murray Hill, NJ |

|Ingrid De Wolf |IMECvzw, Leuven, Belgium |

|Francis Pressecq |CNES, Toulouse, France |

|Ted Lundquist |Schlumberger Probe Systems, San Jose, CA |

|Metrology & Materials Analysis ||

|Alain Diebold, Chair |International SEMATECH, Austin, TX |

|Syd Wilson |Motorola Semiconductor Products Sector, Tempe, AZ |

|Bryan Tracy |Advanced Micro Devices, Sunnyvale, CA |

|Dale Sheu |International SEMATECH, Austin, TX |

|William Vanderlinde |DoD Laboratory for Physical Sciences, College Park, MD |

|Military ||

|Dave Dylis, Chair |liT Research Institute, Reliability Analysis Center, Rome, NY |

|Joe Buben |Defense Supply Center Columbus, Columbus, OH |

|George Slenski |US Air Force, Wright Patterson AFB, OH |

|Jack Henderson |Naval Surface Warfare Center, Crane, IN |

|Perry Martin |Martin Testing Labs, McClennan, CA |

|Optical Probing ||

|Dan Bodoh, Chair |Motorola, Austin, TX |

|Ken WiIsher, Co-Chair |Schlumberger TT, San Jose, CA |

|Loon Ming |Micron Semiconductor Asia, Singapore |

|Brennan Davis |Advanced Micro Devices, Austin, TX |

|Package Level Analysis ||

|Rajen Dias, Chair |Intel Corporation, Chandler, AZ |

|Rama Goruganthu, Co-Chair |Advanced Micro Devices, Austin, TX |

|Cheryl Hartfield |Texas Instruments, Dallas, TX |

|Thomas Moore |Omniprobe, Inc., Dallas, TX |

|Deepak Goyal |Intel Corporation, Chandler, AZ |

|Poster ||

|Sandra Delgado, Chair |Accurel Systems International, Sunnyvale, CA |

|David Su |TSMC, Hsinchu City, Taiwan |

|Perry Martin |Martin Testing Labs, McClellan, CA |

|Dave Dylis |liT Research Institute, Reliability Analysis Center, Rome, N |

|Sample Preparation ||

|Kei-Wean Yang, Chair |Tektronix Inc., Beaverton, OR |

|Mark Kimball, Co-Chair |Maxim Integrated Products, Beaverton, OR |

|Michael Ruprecht |Infineon Technologies, Williston, VT |

|Victoria Bruce |Advanced Micro Devices, Austin, TX |

|SPM Techniques ||

|Jim Colvin, Chair |Jim Colvin Consulting Services, Newark, CA |

|Peter Harris |Digital Instruments, Santa Barbara, CA |

|Michael Bruce |Advanced Micro Devices, Austin, TX |

|Jeffery McMurray |IBM Microelectronics, Hopewell Jct., NY |

|Bernd Ebersberger |Infineon Technologies AG, Munich, Germany |

|System Level Analysis ||

|Jie Xue, Chair |Cisco Systems, Inc., Salem, NH |

|Jeff Birdsley, Co-Chair |Dell Computer Corporation, Round Rock, TX |

|Ernest Sirois |Motorola, Personal Communication Sector, Libertyville, IL |

|Sridhar Canumalla |Nokia, Irving, TX |

|Charlie Zhia |Advanced Micro Devices, Sunnyvale, CA |

|Robert Knoell |Visteon Corporation, Dearborn, MI |

|Test ||

|Jerry Soden, Chair |Sandia National Laboratories, Albuquerque, NM |

|Rob Aitken |Agilent Technologies, Santa Clara, CA |

|Anne Gattiker |IBM Corporation, Austin, TX |

|Anjali Kinra |Texas Instruments, Inc., Stafford, TX |

|PKOng |Advanced Micro Devices, Austin, TX |

iv


r


ISTFA 2002 COMMITTEE MEMBERS


D


v


vi


Y


Vll


Yield Enhancement


Tom Taylor, Chair Cary Gloor


Sam Subramanian Alfredo Herrera


Infineon Technologies, Sandston, VA LSI Logic Corporation, Ft. Collins, CO Motorola, SPS, Austin, TX


Advanced Micro Devices, Austin, TX


viii


2001 BEST PAPER AWARD


Resistive Interconnection Localization E. I. Cole, Jr., P. Tangyunyong


Sandia National Laboratories Albuquerque, New Mexico


C. Hawkins


University ofNew Mexico


Albuquerque, New Mexico


M. Bruce, V. Bruce, R. Ring, W-L Chong Advanced Micro Devices, Inc.


Austin, Texas


Future ISTFA Dates


29thInternational Symposium for Testing and Failure Analysis 2 - 6 November 2003


Santa Clara Convention Center


Santa Clara, California


30thInternational Symposium for Testing and Failure Analysis 14 - 18 November 2004


Worcester's Centrum Centre


Worcester, Massachusetts


Be sure to put these dates on your calendar!


ix


ISTFA 2003 • Call for Papers


29th International Symposium for Testing and Failure Analysis


2-6 November 2003 • Santa Clara Convention Center • Santa Clara, California USA


Sponsored by: ASM Electronic Device Failure Analysis Society (EDFAS)


|This is your opportunity to participate in "THE PREM/ERE EVENT" for the microelectronics failure analysis |This is your opportunity to participate in "THE PREM/ERE EVENT" for the microelectronics failure analysis |
|---|---|

|community. We encourage you to submit an abstract for potential inclusion in the ISTFA 2003 Symposium. |community. We encourage you to submit an abstract for potential inclusion in the ISTFA 2003 Symposium. |

|ISTFA solicits original, previously unpublished papers on a wide range of Testing and Failure Analysis topic of practical value to anyone working to detect, understand and eliminate electronic device and system failures. Non-commercial papers from equipment vendors dealing with new or unique tools and methodologies, applications and results are welcome. Papers will be selected for inclusion in the technical program on the basis of appropriateness and quality of data, technical importance, novelty/originality, and interpretation of results. Paper acceptance is based entirely on the information included in the abstract. |ISTFA solicits original, previously unpublished papers on a wide range of Testing and Failure Analysis topic of practical value to anyone working to detect, understand and eliminate electronic device and system failures. Non-commercial papers from equipment vendors dealing with new or unique tools and methodologies, applications and results are welcome. Papers will be selected for inclusion in the technical program on the basis of appropriateness and quality of data, technical importance, novelty/originality, and interpretation of results. Paper acceptance is based entirely on the information included in the abstract. |

|We are currently seeking abstracts on (but not limited to) the following relevant topics* |We are currently seeking abstracts on (but not limited to) the following relevant topics* |

|• Advanced Techniques • Failure Analysis Process |• MEMS |

|• Sample Preparation • System Level Analysis |• Test |

|• Die Level Fault Isolation • Package Level Analysis |• Discretes and Passives |

|• SPM Techniques • Yield Enhancement |• Military |

|• Metrology & Materials Analysis • Optical Probing and |Emission • Optoelectronic Devices |

|• FIB for Fault Isolation and Design/Edit ||

|*For session topic descriptions and pertinent information regarding abstract submission, please visit the ISTFA website at www.edfas.org/istfa. |*For session topic descriptions and pertinent information regarding abstract submission, please visit the ISTFA website at www.edfas.org/istfa. |

s


CALL FOR PAPERS DEADLINE • 3 March 2003


Abstract Submission:


ISTFA 2003 will consider abstracts in English only (two-page minimum) including representative images, figures and references. It is highly advisable to include sufficient detail to allow for fair evaluation of the work discussed.


Also, include the following information for all authors, presenting author listed first: complete name, title, affiliation with complete mailing address, telephone and fax numbers, and email address. This information must be


included with the abstract or it will not be considered for evaluation. Please go to www.edfas.org/istfa to


submit your abstract. The deadline for final submission is 3 March 2003.


Manuscript Submission:


All authors accepted into the ISTFA 2003 Symposium are required to submit a full manuscript for review by


14 July 2003. A final manuscript for publication will be required in electronic format by 18 August 2003.


Pre-approval to present your work at ISTFA 2003 is recommended. All costs associated with your attendance will be at your expense (travel, housing, registration).


For inquiries or information on 1STFA 2003, you may contact:


D ISTFA Conference Administrator, ASM International, Materials Park, Ohio 44073-0002 440.338.5151


D www.edfas.org/istfa


Xl


Preface


The ISTFA conference proceedings are an integral part of technical libraries, failure analysis (FA) laboratories and related industries. In this 28th edition, you will find a comprehensive reference of the state-of-theart research, development, tools and techniques presented at ISTFA 2002.


ISTFA is widely recognized within the worldwide FA community as a pacesetter,each year setting a new standard of excellence in furthering the science and technology of electronic device failure analysis. Once again this year, ISTFA proudly raises the level of knowledge and education on the newest FA innovations, including such topics as metrology and materials, optical probing, system level analysis, and FA process including high-speed analog and optoelectronics.


The predominant character of this year seems to be unpredictability - of economics, of politics, even of the next generation electronic mass products. Failure analysts are familiar with this situation: Unpredictability has always been one of the most challenging aspects of the FA business.


As the microelectronics industry continues to focus on economic recovery and revitalization,the FA community will have to be ready to


xiii


work on a large variety of products. More than ever, the key to successful failure analysis will be the wise selection and combination of an enormous range of techniques and tools. The Electronic Device Failure Analysis Society(EDFAS), through its ISTFA conference series and other educational offerings will continue taking an active role in leading this charge.


I would like to take this opportunity to thank everyone who contributed to ISTFA 2002 and encourage each of you to continue sharing your experiences and results in the development, manufacturing and assembly processes that are core to the ISTFA conferences and to the FA community worldwide.


"There is no success like failure", I once heard Bob Dylan sing (and we would all join in). "And a failure is no success at all", he continued. As failure analysts, we will succeed as long as we can find the failures... and we'll be around for a while.


Prof. Dr. Christian Boit


University of Technology Berlin


General Chair, ISTFA 2002


Christian. Boit@TU-Berlin.DE


Table of Contents


IPFA Best Paper Award Winner


SEM I SThM-Hybrid-System: A New Tool for Advanced Thermal Analysis of Electronic Devices


3


A. Altes, R. Heiderhoff, L.J. Balk, Lehrstuhl fUr Elektronik, Bergische Universitat Wuppertal,Wuppertal, Germany; I. Joachimsthaler, Triple-O Microscopy GmbH, Potsdam, Germany;G. Zimmermann, Infineon Technologies, Munich, Germany


Session 1: Advanced Techniques 1


From Microns to Molecules - Can FA Remain Viable Through the Next Decade?


11


D. P. Vallett, IBM Microelectronics Division, Vermont, USA


Soft Defect Localization (SOL) on ICs


21


M. R. Bruce, V. J. Bruce, D. H. Eppes, J. Wilcox, Advanced Micro Devices, Inc., Austin, Texas;E. I. Cole, Jr., P. Tangyunyong, Sandia National Laboratories, Albuquerque, New Mexico;


C. F. Hawkins, University of New Mexico, Albuquerque, New Mexico


Fault Localization and Functional Testing of ICs by Lock-in Thermography


29


O. Breitenstein, J.P. Rakotoniaina, F. Altmann, Fraunhofer Institute for Mechanics of Materials,Halle, Germany; J. Schulz, G. Linse, Melexis GmbH, Erfurt, Germany


Session 2: Advanced Techniques 2


Visualisation of Electrically Active Areas Using Electron Holography


39


U. Muehle, Infineon Technologies Dresden GmbH & Co OHG, Physical Failure Analysis, Germany;A. Lenk, M. Lehmann, H. Lichte, Dresden University, Institute of Applied Physics, Germany


A Study of Photoelectron Emission Microscopy Contrast Mechanisms Relevant to Microelectronics


47


V. Ballarotto, K. Siegrist, E. Williams, W. Vanderlinde, Laboratory for Physical Sciences and the University of Maryland, College Park, Maryland


Application of Acoustic Fourier Domain Imaging for the Evaluation of Advanced Micro Electronic Packages


55


J. E. Semmens, L. W. Kessler, Sonoscan, Inc., Elk Grove Village, Illinois


Orientation Imaging Microscopy Applications in Cu- Interconnects and Cu-Cu Wire Bonding


61


P. Ratchev, L. Carbonell, H. M. Ho, H. Bender, I. DeWolf, IMECvzw, Leuven, Belgium;B. Verlinden, Katholieke Universiteit Leuven, Leuven, Belgium


Session 3: Metrology & Materials Analysis


~. Materials Analysis and Process Monitoring in MegaFabs


69


B. Tracy, Advanced Micro Devices, Sunnyvale, California


xv


.一


STEM (Scanning Transmission Electron Microscopy) in a SEM (Scanning Electron Microscope) for Failure Analysis and Metrology


77


W. E. Vanderlinde, Laboratory for Physical Sciences, College Park, Maryland


Microcalorimeter Energy Dispersive X-Ray Spectroscopy in Routine Semiconductor Failure Analysis


87


B. Simmnacher, R. Weiland, Infineon Technologies AG, MOnchen, Germany; E. Langer, Advanced Micro Devices, MOnchen, Germany; M. BOhler, J. HOhne, Vericold Technologies GmbH, MOnchen,Germany; C. Hollerith, Technische Unversitat MOnchen, Germany


A Working Method for adapting the (SEM) Scanning Electron Microscope to Produce (STEM)Scanning Transmission Electron Microscope Images


93


E. Coyne, Product Analysis, Analog Devices, Limerick, Ireland


Applications of EELS to Semiconductor Devices Failure Analysis by Using a 300 keY TEM


101


J. Bow, W. Chang, Y. Tsou, H. Chou, C. Chiou, United Microelectronics Cooperation, Hsin-Chu,Taiwan


Session 4: Package Level Analysis 1


Laser Milling Methods for Package Failure Analysis


109


R. Dias, L. Skoglund, Z. Wang, Assembly Technology Development Quality and Reliability, Intel Corporation, Chandler, Arizona, USA


Laser Decapsulation of Transfer Molded Plastic Packages for Failure Analysis


117


G. Carter, Reliability Engineer, Advanced Analog Products, Texas Instruments - Tucson


Investigation of Microstructure Change on Ni-based UBM Systems in Lead Free Solder


127


T. T. Chun, T. C. Hang, C. T. Chong, Institute of Microelectronics, Singapore


Failure Analysis Strategy for 2 Stacked Die CSP


133


S. Mohamed, C. Francis, R. Saad, R. Jaffar, Advanced Micro Devices, Penang Malaysia Evaluation of Package Defects by Thermal Imaging Techniques


139


Y. Liu, R. Dias, Assembly Technology Development, Quality and Reliability, Intel Corporation,Chandler, Arizona


Session 5: Poster


Backside Hot Spot Detection


147


F. Beaudoin, P. Perdu, R. Desplats, CNES-THALES Laboratory, Toulouse, France;


L. D. de Morais, EPSILON Ingemierie, Labege, France; O. Crepel, C. Goupil, LAMIP - Philips


Semiconductors, Caen, France; G. Haller, ST Microelectronics, Rousset, France; T. Beauchene,D. Lewis, IXL, Universite Bordeaux, Talence, France


Optimizing Backside Image Quality


:


155


R. A. Falk, OptoMetrix, Inc., Renton, Washington


xvi


Infrared Microthermography for Integrated Circuit Fault Location; Sensitivity and Limitations


163


S. Kiefer, M. Nair, P. Sanders, J. Steele, M. Sutton, R. Thoma, S. Wilson, Motorola Digital DNA Laboratories, Tempe, Arizona; G. Albright, C. Li, J. McDonald, Quantum Focus Inc., Vista,


California


Failure Analysis of Tungsten Contact Failure in a 0.13 ~m CMOS Process


169


S. Bagchi, S. Subramanian, R. Ross, J. Beck, T. Chrastecky, V. Soorholtz, E. Widener, Motorola Inc., Austin, Texas


Backside Photoemission and Infrared Microthermography for Rapid Debug of Compound


Semiconductor Devices ........•...............•......•.......................................................................................................173


S. Mitra, S. Kiefer, M. Nair, P. Sanders, J. Steele, M. Sutton, S. Wilson, H. Henry, D. Hill,M. Sadaka, Motorola Semiconductor Products Sector, Tempe, Arizona


Laser-Voltage-Prober Measurements on Bipolar Devices


177


A. Stuffer, P. Egger, H. Pohl, Infineon Technologies, Munich, Germany; A. Moffat, NPTest Inc.,Ismaning, Germany


Application of Focused Ion Beam in Debug and Characterization of 0.13 ~m Copper Interconnect Technology


183


C. Yuan, M. Mahanpour, H. Lin, G. Hill, Advanced Micro Devices, Inc., Sunnyvale, California


Thin-Die Flip Chip Physical-FA Process Flow


189


A. J. Komrowski, N. S. Somcio, D. J. D. Sullivan, C. R. Silvis, L. Curiel, J. P. Baca, S. Scott,M. Sandoval, LSI Logic Corp., Fremont, California, USA


Failure Mechanism and Rootcause Analysis of UBGA Solder Ball Contamination


195


V. G. Martinez, A. Almero, Quality and Reliability Department, Intel Technology Phils. Inc.;G. Gador, Process and Equipment Engineering Department, Intel Technology Phils. Inc.


Passivation Damage and Residue-Induced Package Failure Analysis for a 16 Lead SOIC GaAs RF/IF


Package .....................................•...........................................................................................................................205


D. Cavasin, Motorola External Final Manufacturing, Austin, Texas


Study on a Single NFET Degradation After Circuit Modification With FIB


215


W. Lehner, Infineon Technologies, Munich, Germany


New Techniques to Improve the Efficiency of TEM Sample Preparation


221


J. Lue, J. Lee, J. Luo, ProMOS Technologies Inc., Hsinchu, Taiwan


A Transmission X-ray Microscope (TXM) for Non-destructive 3D Imaging of ICs at Sub-100 nm


Resolution .......................•.....................................................................................................................................227


S. Wang, F. Duewer, S. Kamath, C. Kelly, A. Lyon, K. Nill, D. Scott, D. Trapp, W. Yun, Xradia, Inc.,


Concord, California; S. Neogi, M. Kuhn, C. Bennet, Intel Corporation, Hillsboro, Oregon; P. Coon,


S. Yan, Intel Corporation, Santa Clara, California


A Broadband Model for Ultrasonic Pulses in the Presence of Thin Layers in Microelectronics


235


S. Canumalla, Nokia Mobile Phones


Beam-Based Localization Techniques for 0.18um IC Failure Analysis After Reliability Test


245


R. Chiu, H. Zhang, W. Chung, M. Cherng, X. Liu, WaferTech LTD, Camas, Washington, USA


xvii


Methodologies for Isolating Faults in Multi Chip Fiber Optic Transceivers That Use GHz Mixed


Signal ICs ...............••.............................................................................................................................................251


K. Seo, B. Wahl, M. Mayonte, Y. G. Kim, Agilent Technologies, San Jose, California, USA


Application of Various Fault Localization Techniques to Different Types of 6T-SRAM Column


Failures ...••..............................................................•....•.......................................•.......•.........................................259


C. Lin, C. Ting, C. Tang, C. Wu, C. Kuo, Y. Huang


Missing Metal Pillar Failure Analysis-A Plug Technology Issue


267


D. Nguyen, Texas Instruments, Dallas, Device Analysis Operation, Dallas, Texas, USA;T. Campbell; S. Whitlock; A Velaga, Agere systems, Microelectronics Orlando, Florida, USA


Session 6: MEMS


Reliability and Failure Analysis of RF MEMS Switches


275


I. DeWolf, A Jourdain, A Witvrouw, P. Fiorini, H. AC. Tilmans, IMECvzw, Leuven, Belgium;W. M. van Spengen, R. Modlinski, IMECvzw, Leuven, Belgium and E.E. Dept. of K.U.Leuven,Belgium


Failure Analysis of Polysilicon Micromirror Arrays


283


J. A Walraven, E. I. Cole, Jr., D. M. Tanner, S. S. Mani, E. J. Garcia, M. A Polosky, Sandia National Laboratories, Albuquerque, New Mexico


Failure Analysis of the Digital Micromirror Device


291


C. Davis, W. Mahin, B. Holdford, Texas Instruments, Inc., Dallas, Texas USA


Wavefront Coded(R) Imaging Systems for MEMS Analysis


295


D. L. Barton, J. A Walraven, *Sandia National Laboratories, Albuquerque, New Mexico; E. R.


Dowski, Jr., CDM Optics, Inc., Boulder, Colorado; R. Danz, A Faulstich, B. Faltermeier, Carl Zeiss,Gottingen, Germany


Session 7: Sample Preparation 1


Sample Preparation for Vertical Transistors in DRAM


307


M. W. Ruprecht, Infineon Technologies, Williston, Vermont; S. Wen, R. Vollertsen, Infineon Technologies c/o IBM Microelectronics, Essex Junction, Vermont


A Methodology to Reduce Ion Beam Induced Damage in TEM Specimens Prepared by FIB


313


C. K. Liu, C. Jen.Chen, J. Yan.Chiou, D. Su, Taiwan Semiconductor Manufacture Co. Ltd.,Hsin-Chu, Taiwan


CMOS Backside Deprocessing With TMAH /IPA as a Sample Preparation Procedure for Failure Analysis


317


S. Prejean, V. Bruce, J. Burke, Advanced Micro Devices, Austin, Texas


Investigation of Choline Hydroxide for Selective Silicon Etch from a Gate Oxide Failure Analysis Standpoint


325


V. Korchnoy, Intel Israel (74) Ltd., Haifa, Israel


XVlll


In situ Decapsulation of Plastic Encapsulated Devices Mounted to a Printed Circuit Board


333


R. R. Hylton, Maxim Integrated Products, Beaverton, Oregon


Session 8: Failure Analysis Process 1


A Standardized Scientific Method Formulation for Failure Analysis Application


341


S. Ferrier, Metatech Corporation, Corvallis, Oregon


Probeless FA Approach: A Breakthrough Simulation Based Failure Analysis Method


349


C. Lock, Y. Wong, K. Siek, Intel Technology Sdn Bhd, Penang, Malaysia


Electrical Faults Captured by In-line E-beam Inspection and Failure Analysis


355


Z.G. Song, G.B. Ang, H.Y. Li. V. Sane, J. Indahwan, S. Ansari, S.F. Tee, W. Richter, C.K. Oh,S. Redkar, Failure Analysis Group, QRA, Chartered Semiconductor Manufacturing Limited,


Singapore


Session 9: System Level Analysis 1


Effect of Corner Underfill Voids on Chip Scale Package (CSP) Performance Under Mechanical Loading


361


S. Canumalla, S. Shetty, N. Hannan, Nokia Mobile Phones, Irving, Texas


Leakage Isolation of Mixed-Signal Devices at Operating Modes


371


W. Xia, Qualcomm Inc., San Diego, California, USA


Method for Measuring Package to Board Interconnection Shear Strength for Area Array, Fine Pitch Packages


377


S. Canumalla, H. D. Yang, P. Viswanadham, Nokia Mobile Phones


Session 10: Die Level Fault Isolation 1


Picosecond Imaging Circuit Analysis of Leakage Currents in CMOS Circuits...................•..........................387


S. Polonsky, A. Weger, M. McManus, IBM, T.J. Watson Research Center, Yorktown Heights,


New York, USA


Scanning SQUID Microscopy for Die Level Fault Isolation


391


D. P. Vallett, IBM Microelectronics Division, Essex Junction, Vermont, USA


A Successful Failure Localization Approach for Defect Identification on High Resistance Interconnects


397


Y. Lin, Y.S. Huang, C.S. Lee, C.M. Cheng, W. Hsu, Taiwan Semiconductor Manufacturing Company, Ltd, Product Failure Analysis Dept.


; Backside FIB Device Modifications Through the BOX Layer of an SOl Device


Micro Devices, Inc., Austin, Texas


403


t ~i~H~~~i~~~·, i~c~ht~;t~;':~x'::'~ Johnson, M. Santana, Jr, T Y Chu, M Gonzalez, Advanced


xix


Coaxial, Photon-Ion Technology Enables Direct Navigation to Buried Nodes on Planarized Surfaces,


Including Silicon .....................................................•.....................................................................................•.......409


MA Thompson, E. LeRoy, T. Lundquist, W.B. Thompson, NPTest, Inc., San Jose, California;


C. Richardson, LSI Logic, Fort Collins, Colorado


Session 11: Discretes, Passive


Tin Whiskers on Discrete Components: The Problem


421


J. P. Siplon, G. J. Ewell, E. Frasco, T. Gibson, The Aerospace Corporation, Los Angeles,


California; J. A Brusse, ass Group, Incorporated, NASA Goddard Space Flight Center, Greenbelt,Maryland


Electron Beam Induced Luminescence....................................................................................................•.........435


N.C. Miller, K.P. Rispoli, Raytheon Co, Lexington, Massachusetts, USA


High Power Testing of Optical Connectors


439


P. Furcas, R. Pastorelli, G. Salmini, Cisco Photonics Italy; M. Vanzi, University of Cagliari - DIEE INFM


Failure Analysis of LCD Drivers: A Case Study


445


AC.C. Telles, L.R. Felix, M.H. Comerlato, AP. Mammana, D.S. Rozario, S. E. Filho, Centro de Pesquisas Renato Archer - CenPRA, Campinas - Brasil


Plastic BGA Module FA Process Flow Development


449


Z. Wang, L. Wagner, C. Cheah, Failure Analysis Lab & iPower Design Group, International Rectifier Corp., EI Segundo, California


Session 12: SPM Techniques


What Can a Failure Analyst Do With an AFM?


455


A N. Erickson, Multiprobe, Inc. Santa Barbara, California


Microprobing on Sub-Micron Features on ICs Using an AFM Based Technique


461


R. R. Goruganthu, S. McBride, M. Santana, Jr., Advanced Micro Devices, Austin, Texas;M. Mahanpour, Advanced Micro Devices, Sunnyvale, California


Site Specific 2-D Implant Profiling Using FIB Assisted SCM


467


K. Jarausch, J. F. Richards, L. Denney, Intel Corporation; A Guichard, P. E Russell, North Carolina State University


Conducting Atomic-Force Microscopy Investigations on Thin Silicon Gate Oxides: Influence of Tip Shape and Humidity


473


S. Kremmer, S. Peissl, C. Teichert, F. Kuchar, Department of Physics, University of Leoben,


Leoben, Austria


Enhancements of Non-contact Measurements of Electrical Waveforms on the Proximity of a Signal Surface Using Groups of Pulses


483


F. Du, SUSS MicroTec Inc., Santa Clara, California; G. Bridges, D.J. Thomson, Department of Electrical and Computer Engineering, University of Manitoba, Winnipeg, Canada;


R. R. Goruganthu, S. McBride, M. Santana, Jr., Advanced Micro Devices, Austin, Texas


xx


Session 13: Package Level Analysis 2


A Study on Non-Stick Aluminium Bondpads Due to Fluorine Contamination Using SEM, EDX, TEM,IC, AUGER, XPS and TOF-8IMS Techniques


495


Y. N. Hua, S. Redkar, C. K. Lau, Chartered Semiconductor Mfg Ltd, Singapore; Z.O. Mo,PSB Corporation, Singapore


Microstructure Studies of Under Bump Metallization Systems Using Transmission Electron


Microscopy ................................................•...........................................................................................................505


C. Tung, P. Teo, M. C.Y. Lo, Institue of Microelectronics, Singapore; G. 1.1. Sheng, Macronix


International Co., Ltd., Hsinchu, Taiwan


Hot Disk: A Transient Plane Source Technique for Rapid Thermal Conductivity Measurement


513


Y. He, Intel Corporation, Chandler, Arizona; G. S. Ng, Department of Materials Science and


Engineering, Massachusetts Institute of Technology, Cambridge, Massachusetts, and Intel


Corporation, Santa Clara, California


Comparison of Differential Scanning Calorimetry and Energy Dispersive X-ray Microanalysis for Measuring Low Gold Concentrations in Sn/Pb Solder Bumps


523


J. Mohr, E. Sullivan, P. Deal, M. Seddon, ON Semiconductor, Phoenix, Arizona, USA


Session 14: Die Level Fault Isolation 2


Infrared Emission-based Static Logic State Imaging on Advanced Silicon Technologies


531


D. R. Bockelman, S. Chen, B. Obradovic, Intel Corporation, Hillsboro, Oregon, USA


Pseudo-Dynamic Fault Isolation Technique Using Backside Emission Microscopy - Case Study,Where All Other Methods Fail


539


Y. Weizman, E. Baruch, Motorola Semiconductor Israel - Product Analysis & Characterization;M. Zimin, Wireless Infrastructures


Laser Beam Based ESD Defect Localization in ICs


543


F. Beaudoin, P. Perdu, R. Desplats, CNES-THALES Laboratory, Toulouse, France; E. Doche,


A. Wislez, LCIE, Toulouse, France; 1. Beauchene, D. Lewis, IXL, Universite Bordeaux, Talence,


France; D. Carisetti, THALES Research and Technology, Orsay, France; D. Tremouilles, Marise


Bafleur, LAAS, Toulouse, France


Advanced sub O.13~mCu Devices - Failure Analysis and Circuit Edit With Improved FIB Chemical Processes and Beam Characteristics


553


J. D. Casey, Jr., 1. J. Gannon, A. Krechmer, D. Monforte, N. Antoniou, N. Bassom, C. Huynh,


B. Silva, R. Hill, G. Gu, V. Ray, A. Saxonis, FEI Company, Peabody, Massachusetts; C. Chandler,M. Megorden, P. Carleson, FEI Company, Hillsboro, Oregon; M. Phaneuf, J. Li, Fibics Inc., Ottawa,


Ontario, Canada


Microwave Frequency Signal Propagation in Backside Focused Ion Beam (FIB) Fabricated


Interconnects


559


J. A. Rowlette, M. DiBattista, S. Fortuna, R. H. Livengood, Intel Corporation, Santa Clara, California


xxi


Session 15: Yield Enhancement


Targeted Defect Analysis for Yield Improvement .............................•.•......................................•..•...................571


L. Andrade, T. Bynum, R. Doyle, B. Flaherty, D. Grammer, C. Jacobs, M. Luzar, E. McDaniel,


D. Ricks, R. Stanley, T. Taylor, Infineon Technologies Richmond, Virginia, USA


Driving Baseline Yields on ASICs Using Logic Mapping


579


B. R. Benware, LSI Logic Corporation, Fort Collins, Colorado, USA


Methodology to Correlate Defect Reduction Systems to Electrical Test Data via Artificially


Manufactured Defects .........................................................................•....................•..•................••...........•..........587


M. Santana, Jr., A. V. Herrera, Advanced Micro Devices, Austin, Texas


Real Time Fault Site Isolation of Front-End Defects in ULSI-ESRAM Utilizing In-Line Passive Voltage


Contrast Inspection ........................................•..................................•.......................................•..........................591


O. D. Patterson, J. L. Drown, B. D. Crevasse, A. Salah, K. K. Harris, Agere Systems, Orlando,


Florida


N-Channel Sub-Threshold Leakage "Pipes" Generated From Micro-Twinning Near Shallow Trench


Isolation Interface


599


E. M. Spory, Atmel Corporation, Colorado Springs, Colorado, USA


Session 16: System Level Analysis 2


Making Failure Analysis a Value Add Proposition in Today's High Speed Low Cost PC Environment .....609 M. Lane, Intel Corporation, Oregon, USA; R. Bjork, J. Birdsley, Dell, Texas, USA


Boundary-Sean's Next Plateau: Testing and In-System Configuration at the System Level..


617


P. Collins, R. Dellecker, JTAG Technologies


Functional Failure Analysis by Induced Stimulus ..•.........................................................................................623


J. Colvin, Consultant, Newark, California


Case Studies of IR Based Rapid PC Motherboard Failure Analysis ..............................••....•..........................631


J. Swart, J. Woo, R. Zumwalt, J. Birdsley, Y. Taffese, Dell, Texas, USA


Session 17: Optical Probing 1


Prospects of Time-Resolved Photon Emission as a Debug TooL


645


J. Vickers, N. Pakdaman, S. Kasapi, Optonics, Inc., Mountain View, California


Defect Localization Using Time-Resolved Photon Emission on SOl Devices that Fail Scan Tests


655


D. Bodoh, E. Black, K. Dickson, R. Wang, T. Cheng, Motorola, Austin, Texas; N. Pakdaman,J. Vickers, D. Cotton, B. Lee, Optonics, Inc., Mountain View, California .


Timing Characterization of MUltiple Timing Domains


663


A. J. Weger, M. McManus, P. Song, IBM T.J. Watson Research Center, Yorktown Heights, New York, USA; A. Muszynski, IBM eServer Group, Poughkeepsie, New York, USA


xxii


Circuit Voltage Probe Based on Time-Integrated Measurements of Optical Emission From Leakage


Current .........................•.......................................................................................................................•...•.............667


F. Stellari, P. Song, J. C. Tsang, M. McManus, M. B. Ketchen, IBM, T.J. Watson Research Center,Yorktown Heights, USA


Session 18: Sample Preparation 2


Characterization of Reactive Ion Etching of Silicon Substrate for Backside Failure Mode Analysis


675


H. Wu, J. Cargo, Agere Systems, IC Quality Organization, Product Analysis Lab, Allentown,Pennsylvania


The Use of Precision Selective Area Milling for Failure Analysis of Flip-Chip Packages


683


G. F. Gaut, Skyworks Systems, Inc.


Methodology for TEM Analysis of Barrier Profiles


689


T. Lee, J. Huang, L. Chen, R. Hwang, D. Su, Taiwan Semiconductor Manufacturing Company, Ltd.,Hsinchu, Taiwan


Studies on Chemical Methods to Expose GatelTunnel Oxide and Identification of GatelTunnel Oxide Defects in Wafer Fabrication


695


Y. N. Hua, G. B. Ang, S. Redkar, Yogaspari, W. Richter, Chartered Semiconductor Mfg. LTD,Singapore


Session 19: Test


Parametric Variation or Defects?: Statistical Post-Processing Analysis of Wafer-Sor t Data


703


W. R. Daasch, IC Design and Test Laboratory, Electrical and Computer Engineering, Portland State University, Portland, Oregon


Diagnosis Using Quiescent Signal Analysis on a Commercial Power Grid


713


C. Patel, E. Staroswiecki, S. Pawar, D. Acharyya, J. Plusquellic, Department of CSEE, University of Maryland, Baltimore County


A New Technique for Scan Chain Failure Diagnosis


723


R. Guo, S. Venkataraman, Intel Corporation, Hillsboro, Oregon


SEM in-situ Study of Electromigaration Induced Degradation Processes in Embedded Copper Interconnects


733


E. Langer, M. A. Meyer, E. Zschech, AMD Saxony Manufacturing GmbH Dresden, Germany;M. Hermann, Technical University Dresden, Institute of Materials Science, Germany


Session 20: Optical Probing 2


Single Element Time Resolved Emission Probing for Practical Microprocessor Diagnostic


~.•...'...•...•...•.ApPlic:ti:n~~;;;~~:·c:·y~~·~~:··H:·M:(p;~ii·N~:·s:·P:·M~;;~~:T:·;;;:·E;i~~:·i~;;;ic~~~~;;;ti~~·,·s;~t;·C·I~;;;·:············741f California; B. Lee. Optonics. Inc.. Mountain View, California'f~


;~~


xxiii


The Influence of Optical Beams on Semiconductor Devices During Failure Analysis


747


C. Zhang, M. Thayer, L. Herlinger, G. Dabney, M. Gonzalez, Advanced Micro Devices, Inc.


Next-Generation Optical Probing Tools for Design Debug of High Speed Integrated Circuits


753


W. Lo, K. Wilsher, R. Malinsky, N. Boiadjieva, C. Tsao, M. Leibowitz, H. Deslandes, NPTest, Inc.,A Subsidiary of Schlumberger Technologies, San Jose, California, USA


Session 21: Failure Analysis Process 2


TEM Direct Observation of Gate Oxide Defects


765


N. Wang, S. Daniel, Cypress Semiconductor


Localization Techniques on a O.15um CMOS Device: Charge Pump Failure Analysis ••...........••..........•.•.....771


H. Pan, 1. Gibson, Actel Corp., Sunnyvale, California, USA


Debug and Fault Isolation of an RF/IF Circuit for 3G Cellular Applications With High Leakage: A


Case Study


777


S. Wilson, M. Nair, M. Vicker, R. B. Meador, G. Smoot, P. Sanders, S. Kiefer, J. Steele, M. Sutton,


Motorola Semiconductor Products Sector, Tempe, Arizona


Author Index.....••................••.......................•...•........................•..•................•............•.................•...........•.............785


xxiv


IPFA 2002 Best Paper Award Winner


© 2002 IEEE. Reprinted, with permission, from


Proceedings of the gth IPFA 2002, Singapore


SEM / SThM-Hybrid-System: A New Tool for Advanced  Thermal Analysis of Electronic Devices


A. Altes1, I. Joachimsthaler2, G. Zimmermann3, R. Heiderhoff1, L.J. Balk1 1Lehrstuhl für Elektronik, Bergische Universität Wuppertal,


Fuhlrottstr. 10, D-42097 Wuppertal, Germany


Phone: +49-0202-4393929   Fax: +49-0202-4393804   E-mail: altes@uni-wuppertal.de 2Triple-O Microscopy GmbH, Behlertstr. 26, D-14469 Potsdam, Germany  3Infineon Technologies AG, CFE PT FA 2, Balanstr. 73, D-81541 Munich, Germany


1.   Abstract


A resistive probe based Scanning Thermal Microscope (SThM) was implemented in an analysis chamber of a  Scanning Electron Microscope (SEM). By means of this  hybrid-system thermal device, specific characteristics are  detectable. Variable punctual heat sources can be simulated  and the influence of ambient parameters can be investigated.


2.   Introduction


The Scanning Thermal Microscope (SThM) is an established


technique in failure analysis of electronic devices. By using


a resistive thermal probe, the detection of temperature


distribution, with an accuracy of 5mK in the temperature


range and local resolution of about 50nm, was demonstrated PE beamPhoto-Topography data[1,2]. In addition, using the resistive probe as heater and


区


Piezo


Laserdiodes


detector simultaneously, contrast imaging of different local  thermal conductivity and measurement of quantitative  thermal conductivity with an error of ±2% is achievable [2].


Electronic


A significant disadvantage of the conventional SThM


control unit


performing failure analysis of electronic devices, is the


Sample


Resistive


obligation to prepare complex cross section samples of 1L


feedback


probe


Thermal


afterwards active operating integrated circuits. Although the Piezo scanherambient parameter of the tip can be very significant for


Wheatstone.S


effective operation of SThM, those kind of parameters are


X-Y scanning


bridge4jout


often neglected. Especially if we think about the fact that


SignalrefLock-inI


there is only a small part of the platinum wire in contact with


Beam blanking


generator


the specimen while there is a large surface of the filament  interacting with the ambient air, we can imagine that it might  be difficult to filter out the information of the sample. Thermal measurements are also affected by a liquid layer on  the sample surface, leading to additional unwanted heat  transfer between probe and the device being tested.


Moreover, the theoretical simulation of integrated circuits  becomes more and more difficult because of the complex  microscopic structures and some uncertainties during  manufacturing processes. To overcome all these problems, the SThM was integrated in the analysis chamber of a  Scanning Electron Microscope (SEM). By this means, simulations of variable punctual thermal hot spots are  possible at any interesting location by means of electron  beam irradiation and simultaneous detection of induced  temperature distribution by SThM probe at a defined  distance.


3.   Experimental Details


The SThM used in these SEM / SThM-Hybrid-System


experiments is based on an AFM with laser deflection  method (Fig. 1). A resistive probe (wollastone wire with  platinum core) is integrated into this AFM and is connected  to a Wheatstone Bridge. The output signal of the Wheatstone  Bridge is amplified by a Lock-In-Amplifier (LIA) and  recorded by an Electronic Control Unit (ECU) and PC. By  using the SEM beam blanker, the induction of a local  periodic punctual heat source at frequencies up to the MHz  range is practical. Hereby the simultaneous phase sensitive  detection of the thermal signal is obtained by connecting the  signal generator of the beam blanker to the reference input  of the LIA.


Fig. 1: Schematic set-up of the realised SEM / SThMHybrid-System


The scanning process is provided by xy-piezos which are  connected to the sample holder. Therefore two different  scanning-operation modes are feasible. In the first mode it is  possible to assure a constant distance between heat source  and thermal probe, while the sample surface moves in xydirection below the tip. This ‘constant distance mode’ allows  us to position a variable local punctual heat source at defined  distances. In the case of small distances and low power  supply of the down streamed Wheatstone Bridge, the selfheating of the resistive thermal tip is negligible, thus this  mode of operation enables us to detect the electron-beam  induced temperature in dependence of the local thermal  conductivity. The second operation mode is specified by the  fixed local position of the thermal probe on the sample, while the electron-beam is scanning the surface. In contrast  to the first mode, the distance between heat source and


 2002 IEEE.  Reprinted, with permission, from Proceedings of the 9th IPFA 2002, Singapore


Proceedings from the 28h International Symposium for Testing and Failure Analysis, 3-7 November, 2002, Phoenix, Arizona


Copyright© 2002 ASM International®


thermal probe varies depending on the current electron-beam


position. This ‘fixed probe mode’ is useful for measuring


and imaging of the electron beam induced temperature


distribution in dependence of the local, sample specific,


thermal characteristic and the currently adjusted power of


the electron-beam. While in [3] the beam induced substrate


heating is described mathematically by superimposition of


elementary analytic solutions, the here described SEM /


SThM-Hybrid-System allows the instrumentational


determination of the temperature distribution. Beyond this


two operations mode the conventional SThM with its


facilities for measuring local temperature and thermal


conductivity is, of course, also applicable without electronbeam but within a vacuum condition. To characterise the


developed measurement system, the ‘fixed probe operation


mode’ is centred in the sequencing presentation.


4.   Results and Discussion


Due to the electron beam and the perpetuation mechanism of


the necessary vacuum condition, adsorbent layers are


expected on the specimen. Since the thickness of this


additional surface layer is in the range of a few atomic layer,


a relevant influence on the implemented SThM (resolution ≥


30nm) can be excluded. In comparison to the conventional air


vacuum


SThM, there are primarily two different properties to be  mentioned, which affect the thermal measurement. First, there is the electron beam, whose conversion into thermal  energy within the device being tested, should simulate a  punctual heat source of the defect active device.


60


-5


vacuum:amplitude


amplitude [mV]台古台


air:amplitude


2μm


distance [nm]


force [uN]


a)


20


-4000-3000-2000


wacum.0-1000 pheas5-35


2


-22


air:phase


amplitude [mV]命台on


26


yacuum:amplitude vacuum:phase


-30phase [deg]


x[μm]0246


10


o


normalized thermal signal


vacuum air


8 0鼎


b)


-distance [nm]force [nN]


Fig. 2: SThM output signal in dependence of probesample distance and force load respectively, at different  ambient conditions


Beside the fact that this temperature distribution can be  measured and imaged by the thermal probe, this punctual  heat source and its resulting two dimensional temperature  field is assumed to allow conclusions about the investigated  material. Secondly, there is the missing ambient air and the  missing liquid surface layer, that are supposed to affect the  accessible thermal results such as thermal conductivity and  temperature distribution. For this reason, and to characterise  the SThM component of the hybrid system, the influence of  these ambient parameters were investigated first, by  performing force distance curves with simultaneous  detection of the thermal signal (Fig.2). The distance and  force dependencies were obtained at two extremely different  ambient conditions. While in air, the amplitude as well as  the phase even vary at probe sample distances in the range of  5µm (Fig.2a), in a vacuum condition, the thermal signals are  not influenced by the sample surface until the distance  becomes smaller than a few nanometers (Fig. 2b). This result  corresponds to the general statement of earlier publications  and to the conclusion of [4] which observed a strong  decrease of the heat transfer with increasing tip sample  distance on a length of about 10nm.


a


*phase [deg]


air: amplitude


42


-50-250125250--34


Fig. 3: Comparison of thermal conductivity images,


obtained by 3ω-method [6], in air and vacuum condition


However, although there is a significant difference between  air and vacuum conditions in distance and force load  depending thermal signals, we found no fundamental


discrepancy in measuring two dimensional thermal  conductivity of the cross section preparation of a glass / silicon composition in air and in a vacuum condition (Fig.3a). The fact that there are minor parallel heat flow  paths in vacuum, merely results in an slightly improved  spatial resolution, which is especially indicated by the line  measurements of the two dimensional thermal conductivity. In Fig. 3b, more small features and higher local gradients  can be observed at line measurements obtained in a vacuum  condition, than in line measurement obtained in ambient air. Nevertheless, it is clearly visible, that there are no grave  differences between thermal conductivity images performed  in air and vacuum. This result is very well explainable by the  use of a balanced Wheatstone Bridge, which equalizes the  additional heat flow from the measurement tip to the  surrounding air.


r[μm]


Fig. 4:Line-measured temperature distribution in


dependence of the scan direction without elimination of  the influence of backscattered electrons, and calculated  theoretical distribution


From Fig.2 we can gather, that there is no significant signal  change at a force load of about 2µN. In all measurements in


‘fixed probe mode’ presented in this paper, there was a force  adjusted in the range of 2-3µN. Thus we can assume that  there is no significant influence of the bearing-strength on  the thermal signal. The disadvantage of the permutation of  heat source and detector concerning the scan procedure, is  given by the fact that there is no exact static temperature  distribution on the sample surface anymore. This  circumstance results in an asymmetrical region with higher  temperature around the contact area. Fig.4 shows this  asymmetric temperature distribution and the operation mode  conditional scan direction dependence of the line measured  thermal signal. Hereby the investigated line on the sample  surface was set as close as possible to the tip contact area. By this means we wanted to make sure, that it is possible to  measure the temperature peak in the centre of the 2D  distribution below the tip. However, if this influence of the  non static distribution is known at given scan speed of the  electron beam, this influence can be eliminated in order to  achieve the real static surface temperature distribution. To  evaluate the influence we can exploit the theoretical  gradient. The spherical static temperature distribution T(r) in  theory is given by Fourier`s Law:


|gradT j ⋅ − = λ |(1) |
|---|---|

|2 4 r j Q π ⋅ = D |(2) |

where j is the heat flow density, QD  is the heat flow and λ is  the thermal conductivity. Considering the method of  resolution by [5] for calculating the electron beam induced  temperature distribution within the sample, these  fundamental thermal laws result in the following equations:


dr


dT


R


Q


)2


/


(


Ω-


π


λ−


=


;


0 <  r  < 2R (3)


0.8


right to left


dr dT


2πλ−


1


left to rightQ=-λ2m.2dT


0  <  r  < ∞   (4)


T(r) calle,


where R is the penetration depth of the electrons. In Fig.4  the theoretical distribution out of (3,4) and the measured  thermal signal are opposed. By several measurements with  the tip in contact and at defined distances (1µm, 2µm, 3µm)


distribution0.40.6


respectively, we found beside the asymmetrical gradient of  the thermal signal, that there is a relevant influence of the


0.2


backscattered electrons if the electron beam is in the contact


normalized temperatur


area (non contact area, respectively) of the thermal probe.


0


Since, at the non-contact measurement, the amplitude of the -50-2502550thermal signal is strongly dependent of the z-piezo voltage  adjusted distance, we can suppose that the backscattered  electrons partly hit the resistive probe. Because of their high  energy, which is transformed to heat within the tip, they  effect a resistance variation. This output signal of the  Wheatstone Bridge should obviously be distance dependent, due to the varying probability of electrons hitting the  detector. Since the thermal signal is still asymmetric, with  the thermal tip not in contact with the specimen, we can


presume that the thermal resistive platinum wire is not able  to follow rapidly the downward temperature jump when the  electron beam strides away from the thermal detector. Here  we have to take into account, that the only heat sink is given  by the supply line of the resistive filament (75µm wollastone  wire with 5µm platinum core and 70µm silver cladding). The poor heat dissipation of the entire thermal probe is also  indicated by the low temperature gradient along the  wollastone supply line, which was measured to ∆T / ∆x = 71mK / 330µm, and the low temperature difference between  the different parts of the tip (wollastone wire vs. glue-point: ∆T = 130mK; wollastone wire vs. mirror: ∆T = 123mK). The ‘fixed probe mode’ is combinable with two different SThM  operation modes. First, the Wheatstone Bridge with the  implemented thermal resistive probe can be supplied with a  slight AC voltage at high frequency (≈100kHz)). Because of  the inertia of the resistive probe, there is no resistance  modulation at this frequency range anymore. Moreover, the  self heating of the tip is negligible. Thus this dynamic mode  is applicable to sensitively read out the resistance change, according to the local temperature.


Fig. 5: Temperature distribution obtained in ‘fixed probe


mode’ and AC operation mode of Wheatstone Bridge


The second mode of the thermal bridge is characterised by a  slight DC voltage supply. Again, the self heating of the tip  should be negligible. But here the simultaneously at low  frequency chopped, scanning electron beam enables to  detect the amplitude and phase of the resulting thermal wave  in dependence of the current electron beam position and tipelectron beam distance, respectively. While in AC mode of  the thermal bridge, the static temperature distribution on the  sample surface and on the thermal probe itself (see above  mentioned temperature gradient) is available, in DC mode  the frequency and sample property depending propagation of  the thermal wave can be obtained. Fig.5a shows the static  temperature measured by AC mode, with the tip in contact  with the stabilizing glass of a cross section prepared  electronic device, and adjusted primary electron beam  current of Ibeam=50nA. The image is calibrated by using the  determined sensitivity of the Wheatstone Bridge (s=1.15mV/K). Fig. 5b distinguishes the temperature drift of  the entire sample, which is explainable by the low heat  dissipation only given by the tip in contact and the sample  holder. The determined temperature drift of ∆Tm≈4K was  confirmed by evaluating the resistance change of a PT100  element (∆TPT100 ≈5K), which has been brought in good


thermal contact to the sample, by using thermal conducting  glue. Furthermore, Fig.5a indicates a tip temperature of  Tm≈350K. This measured temperature ranges in the same  dimensions as the roughly calculated theoretical temperature  by Fourier`s Law: Ttheory≈376K (parameter: QD =0,5mW, length of platinum wire lpw=200µm, diameter of platinum  wire dpw=5µm, thermal conductivity of platinum λPt=71.6W/mK). A detailed theoretical description for the  calculation of the temperature distribution along a metal  filament heated in vacuum is given by [7].


If the Wheatstone Bridge is operated in DC mode and the  electron beam is chopped at low frequency (fchopp<2kHz), the  output signal of the bridge is proportional to the temperature  difference ∆TAC between the electron beam switched on  phase and the electron beam switched off phase. Thus, this  signal corresponds to the amplitude of the induced thermal  wave. By scanning the chopped electron beam in the contact  area of the tip, the gained probe-beam distance depending  signal could allow conclusions referring to the frequency  depending thermal penetration depth. But in this analysis, the frequency dependence of the attenuation of the resistive  platinum filament must be considered. In Fig.6 the  frequency dependence of the attainable thermal signal in AC  mode is illustrated by comparing the resulting signals at two  different electron beam chopping frequencies. Beside the  smaller surface area with detectable amplitude of the thermal  wave, the attenuation of the tip is visible in the equally  calibrated 2D images. To evaluate the amplitude of the static  temperature distribution peak, the equations (3) and (4) can  be used. If we assume that 100% of the electron beam power  is absorbed in the sample, the maximum heat flow QD  can be  determined by the SEM parameter (in the case of Fig.6: Uacc=20kV; Ibeam=50nA; pulse width ratio rpw=1:1). The  radius rps of the local heat source can be determined by the  simulation of dissipation volume in the Monte Carlo  Simulation.


Fig. 6: Temperature distribution of electron-beam


induced heat sources at different chopping frequencies (measured in DC mode of thermal bridge)


However, out of Fig.4 and the before described  measurements at very small distances (1-3µm) between tip  and sample, we can conclude, that there is a not to be  ignored influence of the backscattered electrons on the  thermal output signal of the SThM, if the electron beam is


close to the contact area of the thermal probe. To obtain the  influence of the thermal characteristic of the sample anyway, two measurements were performed in AC mode of the  thermal bridge. The first measurement, with the tip in  contact with the material, in order to get the thermal  information of the device being tested, and the second  measurement with an adjusted tip-sample distance of 1µm, to obtain the influence of the backscattered electrons. By  subtracting the non-contact temperature distribution, it is  possible to extract the 2D temperature distribution on the  sample surface due to a local punctual heat source with  given radius rps=2.5µm (result of Monte Carlo Simulation  with tilt angle of α =60˚, Uacc=20kV on glass) and power  Pbeam=0.5mW (chopped at frequency fchopp=489Hz and  Ibeam=50nA). In Fig.7, the calculated temperature distribution  by (3) and (4), using these parameters, is compared to the  measured temperature distribution (quasi static, because of  low fchopp), obtained by subtracting the contact and noncontact thermal signal. Compared to Fig.4, an significant  improvement regarding the consistency of measured and  calculated local gradients of the temperature distribution is  obvious. Of course a deviation on the right side relative to  the maximum of the peak is visible, but as shown before, this measurement artefact can almost completely be  eliminated, by considering the scan direction of the electron  beam.


Fig. 7: Corrected temperature distribution without  influence of backscattered electrons and calculated


distribution (material: glass; SEM: Uacc=20kV, Ibeam=50nA)


Thus we can state, that by means of the here described SEM / SThM-Hybrid-System, it is possible to simulate a local  punctual heat source on a given electronic device. Since the  static theoretical temperature distribution is given by well  known algebraic equations, the measured temperature  distribution of the simulated heat source can be used to  determine, in principle, local thermal characteristics of  integrated circuits, without the necessity of an active state of  the electronic device. In this context it has to be mentioned, that the existing inertness of the used thermal resistive probe  raises difficulties due to its large geometrical dimensions. In  addition, the existing inertness of the used tip could provoke  a conflict, since the required frequency variations ∆f for  significant distribution changes could be higher than the  cutting frequency fc of the tip. However, by using differently


conceived thermal probes it should be possible to overcome  these potential problems.


5.   Conclusion


A SEM / SThM-Hybrid-System was designed to simulate a  variable, local and punctual heat source on a sample  preparation of a non active electronic device. The system  was characterized concerning the two most important  differences compared to the conventional SThM. We found  out that the vacuum condition leads only to a slight  improvement of the achievable resolution, without  modifying the basic information about the 2D thermal  conductivity of the device under test. Beside the  measurement of the expected temperature drift, the influence  of the scan direction of the electron beam and the  elimination of this measurement artefact was demonstrated. Moreover, the remarkableness of the influence of the  backscattered electrons and the possibility of suppressing  this systematic error was shown. Considering these  falsifications, leads to a measured 2D temperature  distribution on the sample surface, which is in good  agreement with the calculated temperature distribution, by  the simple application of Fourier`s Law. Thus, the  performed measurements demonstrate the principle facility  of the simulation of a local, punctual and periodical heat  source at any location of a cross section prepared integrated  circuit and its simultaneous measurement. By possibly  replacing the used thermal resistive probe with an improved, miniaturized probe, further applications of the developed  hybrid system can be imagined.


References


[1] G.B.M. Fiege, V. Feige, J.C.H. Phang, M. Maywald, S. Görlich and L.J. Balk, „Failure Analysis of Integrated  Devices by Scanning Thermal Microscopy (SThM)”, Microelectron. Reliab. 38 (6-8) (1998), 957-961


[2] T.H. Lee, G.B.M. Fiege, A. Altes, G. Zimmermann, V. Ng, R. Heiderhoff, J.C.H. Phang, and L.J. Balk, "Characterization of MOS devices by the use of  Scanning Thermal Microscopy", Proceedings of the  27th International Symposium for Testing and Failure  Analysis (ISTFA 2001), 191-197


[3] T.R. Groves: “Theory of beam-induced substrate  heating”, J. Vac. Sci. Technol. B, 14(6), pp.3839-3844,(1966)


[4] W. Müller-Hirsch, A. Kraft, M.T. Hirsch, J. Parisi, A. Kittel, „Heat transfer in ultrahigh vacuum scanning  thermal microscopy“, J. Vac. Sci. Technol. A, 17(4), pp.1205-1210 (1999)


[5] L. Reimer, Scanning Electron Microscopy, Berlin, Springer (1985)


[6] G.B.M. Fiege, A. Altes, R. Heiderhoff, L.J. Balk, „Quantitative thermal conductivity measurements with  nanometre resolution”, J. Phys. D.: Appl. Phys. Vol. 32


(1999) L13-L17


[7] S. Halas, T. Durakiewicz, “Temperature distribution  along a metal filament heated in vacuum by DC  current”, Vacuum, 49(4), pp.331-336 (1998)


From Microns to Molecules – Can FA Remain Viable   Through the Next Decade?


David P. Vallett


IBM Microelectronics Division, Essex Junction, Vermont, USA


Abstract


hybrid CMOS chips and eventually emerge as the This paper examines the challenges facing IC failurenanoelectronic ICs. The requisite electrical and analysis through the projected end of the CMOSphysical scale of such devices is especially daunting roadmapand into the establishment of nextfrom an analytical perspective.


FA tools and techniques have fixed resolution and FA categories. The growing importance of faultaccuracy limits, and at some point become highly isolation is highlighted, especially for nanoelectronic


unproductive and eventually altogether prohibitive. It ICs where deviations on the order of one atom oris critical therefore to compare instrumental limits electron will find current instruments two orders ofwith future IC technology trends to identify major magnitude removed in capability. The potentialcapability gaps and proactively drive improvement impacts of self-assembled chips and fault-tolerantand innovation.


A number of publications have analyzed failure


Introduction


some proposing alternative business models entirely analysis prospects from a broad perspective with


the topic focusing more heavily on instrumental[1]-[5]. This paper will provide an updated look at nanoelectronic ICs. The first section brieflylimitations and introduce challenges posed by concept has already been demonstrated on structuressummarizes pertinent CMOS technology trends. The nanoelectronic devices, assembly methods, andarchitectures. The final section examines the outlookfor individual FA process steps and tools.


base technology fora newclassof fully


generation ‘nanoelectronic’ devices. It will review


technology forecasts and assess their effects on major


architectures are also discussed.


CMOS technology continues its relentlessmarch


towards ten-nanometer gates. And sometime before


this an entirely new class of quantum and molecular


devices is expected to phase into production. Proof of


nextsectionsurveyscurrentresearchin


expected to be almost one hundred times smaller than


state-of-the-art CMOS transistors. Radical changes in


fabrication, layout, and circuit architecture are also


forecast. One or more of these dramatically new


assemblies will likely be incorporated into future


||2001|2002|2003|2004|2005|2006|2007|2010|2013|2016|
|---|---|---|---|---|---|---|---|---|---|---|

|MPUASIC Half-pitch (nm)|130|115|100|90|80|70|65|45|32|22|

|Dimensional Scaling|||||||||||

|MPU Physical Gate Length (rm)|65|53|45|37|32|28|25|18|13|9|

|Critical defect size (nm)|65|58|50|45|40|35|33|23|16|11|

|Min. Equiv. Gate Ox Thickness (nm)|1.3|1.2|1.1|09|0.8|07|0.6|0.5|0.4|0.4|

|Intermediate Wiring Pitch (nm)|450|380|320|265|240|215|195|135|95|65|

|Electrical Performance|||||||||||

|On-chip Clock (MHz)|1684|2317|3088|3990|5173|5631|6739|11511|19348|28751|

|Vpo (high-performance) (V)|1.1|1|1|1|0.9|09|0.7|0.6|05|04|

|Sub-threshold Leakage (uA/um)|001|0.03|0.07|01|0.3|07|1.0|3.0|7.0|10.0|

|Static Power (nW per device)|56|67|10|11|26|53|53|97|140|110|

|Overall Complexity|||||||||||

|ASIC Transistor Count (millions)|714|799|810|1020|1286|1620|2041|4081|8163|16326|

|Wring Levels|B|8|8|9|10|10|10|10|11|11|

|Total Pads (high performance ASIC)|1700|1870|2057|2263|2489|2738|3012|4009|5335|7100|

|Total Interconnect Area (mmf)|1967|2078|2157|2318|2461|2571|2851|3360|4068|4762|

|MPU Transistor Area (mm2)|28.7|282|277|27.2|26.8|26.8|26.8|26.8|26.8|26.8|

Table 1:  Selected data from the International Technology Roadmap for Semiconductors most relevant to FA [6].


Throughout the paper the term microelectronics andmicroelectronicsComplexity is the third category, derived from CMOSareused interchangeablytodenoteCMOSfundamental ITRS data. A simple model examines the relationship between the area occupied by a


potential defect versus the total area of conductors on


Nanoelectronicsnanodevices


a chip (i.e., interconnect wiring plus transistor gates and diffusions). The total conductor area represents


‘opportunities’ for defects, and increases as transistor count and wiring length grow. Correspondingly,minimum critical defect area decreases as spacing between conductors shrinks (e.g., wiring pitch,systems or MEMS.


channel length, and gate dielectric thickness). The


CMOS Roadmap Summary


first-order indicator of FA complexity (i.e., smaller TheInternational TechnologyRoadmapfor2001 and plotted in Figures 3a and 3b, where a rapid Semiconductors (ITRS) [6] forecasts CMOS needs


non-linear increase over time is obvious.


in Table 1, where a number of trends are apparent.Qualitative changes are also expected in process Physical gate length, intermediate wiring pitch, gatematerials, packaging, and device structure. Since dielectric thickness, and minimum critical defect size1980 major changes in IC base materials, for are the primary indicators of dimensional scaling.


example, occurred about once every five years. But it They are normalized to 2001 and plotted in Figure 1,took only two years for low-k inter-level dielectrics showing a continuous decline through the end of theto emerge once copper metallurgy was established in roadmap. Changes in electrical performance are1997 [7], possibly signaling a more frequent similarly plotted in Figure 2 and show aggressiveturnover. Strained silicon and low-k dielectrics are increases in clock frequency and static power, andemerging and high-k gate dielectrics are still in especially in sub-threshold leakage, while operatingresearch


voltage decreases slightly.


0.5


0.0


2000


Figure 1: Change in ITRS physical scalingparameters (normalized to 2001).


25.0


20.0


15.0


5.0


Change in ITRS electrical scaling parameters (normalized to 2001).


contemporary bulk effect complementary-metal-


oxide-silicon technology and its derivatives (SOI,


SiGe, etc.). Nanoelectronics or nanodevices will refer


to emerging quantum effect and molecular devices.


The discussion is aimed primarily at logic ICs like


microprocessors and ASICs (as opposed to memory).


It also excludes the fields of chemical and material


analysis, inline metrology, and micro-mechanical


relative rate of change of these parameters then is a‘needles’ in larger ‘haystacks’). It is normalized to


through 2016. Selected data relevant to FA are shown


2.50


2.00


1.50


1.00


0.50


0.00


Figure 3a: Changes in IC conductor area vs.


minimum defect area (normalized to 2001).


100.0


80.0


60.0


Resulting trend in FA complexity derived from data in Fig. 3a.


0.3


1.0


2000 2002 2004 2006 2008 2010 2012 2014 2016


MPU physical gate length Critical defect size


Intermediate Wiring Pitch Gate dielectric


Figure 1:


10.0


On-chip Clock


VDD (high-perf.) Static Power


Sub-threshold


lkg.


Figure 2:


Total Conductor Area


(wiring + transistors)


Minimum Critical  Defect Area


Figure 3a:


40.0


Overall FA Complexity = Total Conductor Area / Defect Area


Figure 3b:


A particularly revolutionary possibility is that ofSET developed by the Electrotechnical Laboratory MITI in Japan [13]. It is electrically similar to a increases channel-to-body coupling to control shortCMOS FET with three terminals akin to a gate,


source, and drain, and operates qualitatively in like fashion whereby two-terminal current is gated by a third terminal. The major differences are in the self-aligned format required to minimize overlap


construction and electrical operation.


transistor by about 2007.


scanning probe microscope.


threatening CMOS.


Nanoelectronics Survey


categories:


• Solid-state quantum effect devices


• Molecular electronic devices


A. Solid-state quantum effect devices


Insulating barriers at either end of the ‘channel' form


Solid-state quantum effect (QE) devices includeoxides have been used, metal oxides like titanium are quantum dots (QDs), resonant tunneling diodesmanufacturable to much smaller dimensions - as(RTDs), resonant tunneling transistors (RTTs), and


little as 10 nanometers (critical for room temperature


single-electron transistors (SETs). Figure 4 shows a


operation). A metal gate electrode controls the energy


double-gated (DG) transistors. A second gate


channel effects without sacrificing drive current.


When placed at the back or bottom of a conventional


horizontal FET, a second gate is difficult to build in


capacitance. A promising alternative is the fin-FET


[8] where the transistor is rotated ninety degrees onto


TiOx Barrier


Source


its side so that both gates are manufacturable and


accessible from the top and therefore able to be


aligned. The ITRS predicts some form of DG


An especially acute problem for failure analysis is an


anticipated increase in so-called ‘non-visual’ defects.


Drain


Parasitic resistance or capacitance causes slow timing


paths or inadequate voltage levels that in turn cause


IC faults. As devices scale physically and electrically


Tunnel Junction Area


there is less margin for such deviations and therefore


greater sensitivity to smaller excursions (as opposed


to the more classical ‘hard’ opens and shorts). These


mechanismsmay be manifestedaschemical


contaminants or films that are not visible, in the


Island


traditional sense, to an electron beam or even


TiOx


Despite the impressive advancements and challenges


15-25nm35-50nm15-25 nm


projected by the ITRS, CMOS technology faces


100 nm SiO2


fundamental limits: quantum-mechanical tunneling of


carriers (through gate dielectric, channels, and from


N Si substrate


drain to body), control of dopant placement and


Gate Electrode


concentration, and process variation at near atomic-


scale dimensions. Widespread research is underway


3309


to overcome these with nanoelectronic devices that


SingleElectron Transistor


130a


leverage the same quantum-mechanical effects now


100号


-4100T300K ON-2V


出复r410


3188


110日ctanceConda


P


Common requirements for computing devices are


repeatable well-defined switching with a high on-off


⑤)


4100


ratio; low off-state leakage; electrical isolation of


output from input; and sufficient gain to drive desired


树


fan-out. A number of technologies are currently in


research [9]-[12] with the primary goal of optimizing


150mY15418mYS4范


these properties. They fall broadly into two


Drain Voltue VD(V)


电1中8-0.34s0.17


● Solid-state quantum effect devices, or


● Molecular electronic devices.


Figure 4: Single-electron transistor. Top - AFM


Athird category describes major changesin


image; Center - schematic; Bottom - electrical


fabrication methods and system architecture.


characteristics [13].  (©19971EEE)


an island isolating source from drain. While siliconFigure 4:


(© 1997 IEEE)


: 30-50 nm


states of the island, with respect to the source andThese conducting and insulating molecular building blocks can be used to create selective electrical pathways (i.e., Boolean logic). One such example is the molecular RTD shown in Figure 5. Two insulator molecules interrupt a conductive chain to form the


island. Current occurs when the kinetic energy of the


incoming electrons corresponds to, or is in resonance


with, one of the energy levels on the island (hence the


term resonant tunneling diode). Fig. 5 also illustrates


very high gain device.


how a complete molecular full-adder could be built


Vmaterials, silicon is


B. Molecular electronic devices


covalentlybondedmolecules.


polyphenylene chains


carbon nanotubes


wire when an appropriate bias is present. When anCarbon nanotube (CNT) devices are made from aliphatic group molecule is used, only singular orgraphite sheets rolled into elongatedhollow sigma bonds form, and the only channel exists alongcylinders. The tubes possess rare qualities unlike the positively charged nuclei of the molecules wherethose of classical metals or semiconductors and are known instead as semimetals. Their most striking


characteristic is that the unique twist and diameter of


drain, to a very high degree of sensitivity. When the


gate voltage exceeds a parameter known as the


Coulomb gap voltage, electrons repeatedly tunnel


through the barriers thus creating current. The


resulting source-drain characteristic is quantized, as


seen in Fig. 4, owing to a phenomenon known as the


Coulomb blockade, and is thereby sensitive to single


electron changes in gate charge. As such the SET is a


resonantfrom such molecular diodes.


Despite successful demonstration of a number of QE devices, many obstacles remain. On-off current ratios


"Island"


are not optimized, making logic states potentially


All


Au


indistinguishable. Greater sensitivity (as with SETs)


SCHCHz


makes voltage and current fluctuations more critical


than in CMOS. Room temperature operation is


limited, with most structures requiring cryogenic


roocasplend


operation. While many devices are now based on IIIEnergyMCsUnvcoupinde


Molecular Crbitala


preferred though its


Dccupled


Tramamied


workability at such dimensions is questionable.


Iecroma


Electrical isolation is especially critical, as damaging


Distanouan


background charge accumulation has already been


noted. Finally, such ultra-sensitive devices demand


Molecalar Oriaitalia Docupled


precision in material uniformity and dimensional


control presently unheard of in solids.


Moleculardevices exploit electrontransport


properties through individual (as opposed to bulk)


5


Theyoperate


somewhat like their solid-state QE counterparts in


that electron flow through an island is controlled by


an external electric field. Particularly attractive is the


fact that molecules form naturally in identically


shaped and sized units at the nanometer scale and


thus might prove to be ideal gate-level structures for


ICs, overcoming process uniformity issues that


plague CMOS and more-so QE devices, as noted


above. Two classes of molecular devices are


C,


currently being investigated - polyphenylene chains


and carbon nanotubes (CNTs).


GN


Cour


Phenyl group polyphenylene chains [14] are


comprised of benzene rings that selectively pass or


impede current. Conductivityarisesfrom the


conjugation or overlap of pi-orbitals (electron


Figure 5: Top - molecular resonant tunneling


‘clouds’) of individual molecules. A single large


diode; Center - energy level diagram and electron


orbital forms when the rings are in a chain


transmission; Bottom - full adder design [14].


configuration, and becomes what is known as a


(With permission: The MITRE Corp., McLean, VA)


molecular wire. Mobile electrons flow through the


electron flow is impeded. This arrangement serves as


a molecular insulator or resistor.


each tube govern its allowable electron states and Figure 5:


FETs and logic circuits where the CNTs form aWhile nanoelectronic ICs are far frommass channel between two electrodes as small as 1.5production, approaches at early fabrication are nanometers in diameter, shown in Figure 6. Workingfollowing one of two basic paths. The first is a‘bottom up' method, much like present day chips,a silicon or metal back-gate controls conduction inwhere materials are deposited, etched, and doped on the nanotubes, which can also be doped N or P-type.


a base substrate to create conductors and insulators.


scanning probes [18]. Like direct-write e-beam


technology, scanning probes serially transfer patterns consumption, greater heat dissipation, and quiteonto surfaces at dimensions


nanometers.They have alsobeenused in A/cm2 projected). While the tunable shape and size ofnanomanipulation of individual atoms and for very CNTs is an attractive characteristic, it does look tolocalized oxidation. Clearly such manual techniques make repeatablemanufacturing anightmare.are not tractable for mass production of millions of Attaching metal electrodes to the tubes is also atdevices, however arrays of scanning probes are in present a tedious and manual process.


Comparing the conventional SThM with the SEM/SThMHybrid-System there is, in addition to the unequal ambient  parameter, the influence of the electron beam, which has to  be mentioned as a substantial difference. The electron beam  causes an additional punctual heat source, the properties of  which can be varied by changing the well known SEM  parameters such as acceleration voltage (Uacc) and emission  current (Ie-beam). The basic idea of the constructed hybrid  system is to measure this induced power dependent heat  source and its resulting temperature distribution on the  sample surface. Two practical options are noted for imaging  two dimensional distributions of punctual sources: (a) scanning of the detector, while the source is fixed at one  position; (b) scanning of the source, while the detector is  fixed. Since our implemented SThM is based on a  positioning stage (scanning sample), we used the second  method to gain the local-position-depending thermal signal. This detection method with the stationary thermal probe has  the advantage that there is no signal due to a permanent  change of the thermal contact between the resistive probe  and the sample surface.


development that might provide a more parallel


100nm


A second, more intriguing approach is a ‘'top down’method known as self-assembly [19]-[20]. It


siO2


harnesses the nature of materials to form naturally properties. Lattice mismatch is one example whereby


nanotube


atoms in a deposited layer, say germanium, selfregister with the lattice of the underlying material,silicon for instance, and a 10-nanometer germanium island forms [20] (a similar process by which strained silicon is made today). Langmuir-Blodgett deposition is an alternative approach where one or more


Vad


nanotube C非


Va


precision at the molecular level, across a large area,manufacturing like repeatable and controllable from a liquid. If perfected for mass production, selfmolecular monolayers are created on a solid surface


AuA SiO2


at considerably lower cost than with lithography.


Another major departure from microelectronics is the


concept of large-scale defect tolerance [21]. In


B


-1.5V


5present-day ICs a pre-defined logic function is


非


interconnects to perform the desired Boolean


8


feut


functions. A defect-tolerant system is constructed in the reverse order, where an array of intersecting conducting pathways is fabricated first, and logic


Vour M


function is programmed in afterwards. The prospect


-1.0


of unprecedented levels of integration with millions


"In: 1,11,0 0,10,0


of identical self-assembled devices could enable


"Out:0I0


01B


massively parallel architecture at low cost. One such


15s1


implementation is known as Teramac architecture


-1.5


出


Time


massively parallel machine with 864 identical FPGA


NOR gate electrical characteristics [16].


therefore its conductive properties. Several groups


C. Nanofabrication and Architecture


[15]-[17] have made working room-temperature


logic gates and ring oscillators have been built where


One area rapidly growing in importance is the use of


What sets CNT FETs apart from CMOS transistors,


besides the much narrower channel, is lower power


as smallas 20


higher current density (107 A/cm2 observed with 1013


alternative.


Aubased on their inherent atomic or molecularassemblyoffersattractive benefitsfor IC


NOR


implemented on silicon by building transistors and


6☑


[22], originally built by Hewlett-Packardas a


Figure 6:Figure 6: Top - Carbon nanotube transistor SEM


chips. The key element in such defect-tolerant


image; Center - Layout schematic; Bottom -


approaches is the inherent redundancy that comes


from having parallel logic pathways that can be


(With permission: Dr. C. Dekker, DELFT University


externally configured to bypass defective circuits


of Technology, The Netherlands.)


discovered after assembly and test.


Failure Analysis Outlook


nanoelectronic deviceswill be muchmore The short-term impacts of ITRS trends and long-termTEM, and SEM,at least in non-destructive outlook for fully integrated nanoelectronics are


applications.


inspectiondeprocessingprocess steps of inspection, deprocessing,andThe SPM and its derivatives are anobvious physical electrical fault isolationphysical and electrical fault isolation.


alternative, already in prevalent use on nanodevices


[18] [26]-[27] but it necessitates surface exposure of


A. Inspection


defects. As discussed, non-visible defects are a


The raw resolving power of current high-resolution


electron and atomic scale nanoelectronic defects will microscopes is more than adequate for minimumbe equally if not more subtle. While some SPM techniques are capable of imaging vestiges of such of the technology feature size) through the end of theanomalies they require surface scanning directly current roadmap, and even down to expected atomicabove the affected area. The sizable challenge then scale nanoelectronic defects, as shown in Figure 7.


becomes precisely isolating and exposing an invisible


1.5-04


1JE-05100X Minimum CMOS Defect Visible, UVFull-chip or global deprocessing FA techniques have


宣


0****1E-07X-rayof wet and dry chemistry and chemical-mechanicalhistorically come from IC manufacturing in the form。


，


Figure 7 Spatial resolution of inspection instrumentsand minimum defect sizes versus time.


But high magnification trades off field-of-view andthat both methods will suffer. Compounding the depth-of-field, placing severe limits on the area andproblem is the need to expose defects not only volume of a chip that can be inspected in aphysically intact, but also electrically unaltered to reasonable amount of time. For such instruments toenable subsequent SPM-based localization. As be effective the probable defect location must bediscussed in the following section such local fault predetermined to both a tractable area and verticalisolation (FI) methods will become critical as global wiring level, placing a greater demand on the priorFI techniquesseereducedeffectiveness. For steps of fault isolation and deprocessing.


nanoelectronic devices where defects the size of


deprocessing may be limited to material removal and manipulation with an SPM [28], already becoming commonplace in nanotechnology.


more precise deprocessing and imaging with FIB,


Physical fault isolation (PFI) (i.e., the use of photon,SEM, TEM, or SPM. This gives XRT the potential tothermal, electric, or magnetic field imaging like fill the critical void between quasi-three dimensionalPEM, PICA, XIVA, SQUID, etc.) has three key visible-light microscopy and the higher magnificationrequirements:


Anotherconcern is the potentially


Localization precision.


Access is primarily dependent on packaging. Chip-


on-chip packaging, chip-scale-packaging, and plastic


ball-grid arrays, for example, can make it impossible Low-chargequantumandtothin die in-packagewhile maintaining


susceptible and may well preclude the use of FIB,


discussed below, in reverse order, for the major FA


growing problem on microelectronic ICs, and single-


critical defect sizes (defined by the ITRS as one-half


defect in three dimensions, without destroying it during deprocessing.


B. Deprocessing


1.E-08Minimum CMOs Defect SEMpolishing (CMP). In principle this model guarantees


1.E-09


1.6-10TEM SPM, STIMfor ‘bottom-up’ nanoelectronic assemblies as well.


Noncelectronic Defectssome FA deprocessing techniques and should holdthe availability of at least the base technology for


2000 2002 2004 20062008 2010 2012 2014 2016 20182020milling are unique to FA. Selectivity and depthLocal deprocessing methods like ion and lasersingle atoms or molecules will cause failure, local X-ray tomography (XRT) [23]-[24]offers a


promising alternative where it is possible to create


three-dimensional images of conductors buried in


insulator and search for defects with resolution to


below 100 nanometers. Such capability enables nonC. Physical Fault Isolation


destructive pre-localization of buried defects for


surface-only techniques, as Fig. 7 shows.


• Unobstructed access to the functioning die,


• Adequate sensitivity and signal / noise ratio, and


damaging


• Localization precision.


electrical effects of high-energy incident radiation.


Deleterious ion and electron beam effects on


relatively robust CMOS FETs are well known [25].


single-electron


Figure 7:control are already becoming inadequate for manyminimum sized defects, and with scaling it is likely


functionality with test stimulus to hundreds of pins.detectors, with the added potential of much wider A partial solution, limited to peripheral IO chips, isspectral response.


increases.


becomes apparent.


1000.0


1PstandayStandby Power


The most pervasive challenge to physical fault


Pdeflect


are localized to specific points on the die. But


10+


20002002200420062008


to depackage and rewire the loose die and perform


PFI from the frontside. However dense back-end-ofline wiring and fill patterns severely limit most PFI techniques, especially as the number of metal levels


PFI signal to noise ratio and sensitivityare particularly at risk for CMOS ICs. For instance,methods like PEM, SQUID, and thermal imaging rely on the ability to image defect-induced signals above background noise of a similar nature. Despite decreasing supply voltage, power density for minimum critical defects (calculated from ITRS data)actually increases ten-fold with time, as seen in


electron distribution (arb units)


。Vds=1.SV


1日口Vds=1.0VMCT日Vds=0.125Vemission:


00 Detectablesage 99日


1E4 E3


opaque


0OH


Silicon


CCD emission:


日


Detectable


Figure 8. But the very rapid rise in sub-threshold


0.00.20.40.60.81.01.2141.6


transistor leakage (Fig. 2) will cause chip standby


Eloctron Kinetic Energy (oV)


power density to increase three orders of magnitude


over the same period, eclipsing the more modest


Figure 9: FET hot electron distribution as a


increase in defect energy. The need to incorporate


function of supply voltage, compared with CCD


extensive cooling capability into PFI tools also


and MCT spectral response [29].


Density


isolation is that of fixed near-infrared (NIR) image resolution. The ultimate success and precision of PFI approaches lies in the accuracy with which signalssilicon's 900-nanometer absorption edge diffractionlimits spatial resolution to just under one micron,


*


already more than ten times greater than minimum


Defect Power


features. So as defects shrink, the ratio of PFI ‘search


volume' (a nominal one micron diameter cylinder times total stack height) to ‘defect volume’ increases,201020122014 2016as seen in Figure 10.


Figure 9:


(With permission: Dr. J. Tsang, IBM T.J. Watson Research Center, Yorktown Heights, NY.)


Relative changes in defect power


internode short circuits (normalized to 2001).density versus chip standby power density for Figure 8:


3元+06


A compounding issue with photon-emission imaging2E+06 is a drop in hot electron energy versus the fixed


response of common detectors. Figure 9 shows the


results of Monte-Carlo simulations performed at


IBM's T. J. Watson Research Center [29] where1E+06 decreased VDD causes FET hot-electron distributions


Volume divided Minimum PFI


to shift towards lower kinetic energy levels. The


by Minimum


impact is an approximately two-fold drop in the


Defect Volume number of electrons emitting at around one micron in20002002 2004 2006 2008 20102012 2014 2016DE+00wavelength, as supply voltage scales from 1.5V to


some emission, albeit trading off spatial resolution.Unless alternatives or enhancements are developed,For time-dependent emission (i.e., PICA) more exoticexisting global PFI applications will need to be approaches are being explored, like the promisingaugmented with local isolation where possible like results [30] reported using niobium nitride (NbN)scanning thermal [31] or magnetic force microscopy


1.0V. Therefore fewer electrons are within the visible


Figure 10: Increase in ratio of minimum backside


spectrum of CCD detectors now in prevalent use. For


PFI search volume (limited by NIR imaging) to


time-averaged emission the use of mercury cadmium


minimum defect volume.


telluride (MCT) detectors, for example, ‘buys back’


Figure 10:


[32]. However parts must be scanned at very closethe 10% to 10-12 ampere range, with requisite spatial proximity to the surface while remaining electricallyresolution on the single nanometer scale. The lack of a nanoelectronics timing probe is also critical and must be overcome to understand mechanisms that


will undoubtedly limit high gigahertz and terahertz operation.


high sensitivity.


Design for test (DFT) methods like scan chain


isolation that is ideally scalable since it is largely independent of process technology. Resolution is


limited in the best case to one logical node or circuit block (more typically to less than ten). While the search volume is much reduced from that of an entire tedious and poses the added risk of electrically


chip, it is still quite large. A single faulty node of average-length on a modern ASIC (about 260 microns) has a sizable ratio of search volume


(approximately equal to the square of twice the


minimum-sized defect volume of about 8x107-to-1


(for comparison, it's about 2x1014-to-1 for an entire isolation. With the exception of near-field local10 mm-square chip).


transistor-level probeslikescanningtunneling


microscopy (STM) and conducting tip AFM (CTIt is clear then that diagnostic routines alone are limited and must get ‘smarter’. One approach uses electricalandlayout information to minimize search area by identifying only those segments where immediately adjacent nets are at opposite logic levels (as in the case of a short circuit defect). Another is the superposition of DFT diagnostic output with PFI shown for comparison.


and/or inline defect data that restricts search area to


18+00


Schlieren,


FIRFMTSTIM


零 mear field


sitivity (A)Current Sen1E-09PEMICC SEM


AFH-Microprobe (2)CSTM, CT-AFM


low cost of nanoelectronic ICs, coupled with entirely circuitry. Finally, the promised device densities and


CBIRCH/TIVA


1E-06


designers must be even more strongly convinced that


SQUIDMFM>


tenth-micron CMOS and nanoelectronic ICs. Chip


Liqxtalmay be the only global fault isolation option for sub15-03


16-12


Figure 11: Matrix of current sensitivity and


withminimum defectsizesfor variousspatial resolution of PFI techniques, comparedtechnology nodes. (Areas A, B, and C are typical


defects,values for 100X CMOS defects, minimum CMOS


measurements, respectively.)


Fault isolation and deprocessing must combine to complement existing powerful microscopy capability by providing unprecedented localization precision,


functional. This places great demand on deprocessing


and sample preparation to expose affected circuitry


while leaving it electrically functional. Charge-


contrast SEM methods like absorbed current and


electron beam induced current (EBIC) are local PFI


alternatives finding renewed interest because of their


D. Electrical Fault Isolation


high spatial resolution, subsurface capability, and


diagnostics, for instance, provide critical global fault


Microprobing continues to be important as a quasi-


physical FI method. Its applicability is rapidly


diminishing however as optical microscope-based


probers lack resolution for minimum dimension


conductors, and augmentation with FIB probe pads is


altering devices. AFM, FIB, and SEM probers


promise some relief but long-term prospects appear


limited by probe tip size and durability.


minimum wiring pitch, times the net's length) to


Nanoelectronic ICs create what is arguably the


greatest long-term FA challenge in physical fault


AFM) [33], current PFI instruments severely lack


physicalresolutionat the


nanoelectronic scale, shown by Figure 11, a matrix of


approximate current sensitivity versus lateral spatial


resolution, based on published data, for a number of


PFI methods. Minimum critical defect dimensions are


Technology Nades 中CMOSCHOSHolecular


inline defects or where there is thermal, photon,


130mm 22mmImm


net segments where there is either an indication of


Far field


electric, or magnetic field activity.


As PFI capability lessens, designed-in diagnosability


- Defects


debug and FA capability on complex logic chips is becoming critically dependent on DFT and diagnosticnewarchitectures,willprovidetremendous 10-041E-05 1E-06 1E-07 1E-06 1E-09 1E-10 1E-11opportunities to integrate defect tolerancewith Lateral Reselution (m)


diagnosability, provided that the industrytakes


Conclusions


deprocessing and fault isolation, as Figure 12 shows.


Innovation and development of wide-area imaging or


perturbation of quantum device properties might


provide sensors and detection schemes for signals in


Figure 11:


advantage of the long lead time now available.


A review of future CMOS technology trends and a


and earlynanoelectronic device


long-term outlook for nanoelectronic ICs finds


adequate inspection capability but widening gaps in


especially in the vertical plane. Limitations imposed by NIR imaging and single-net diagnostic resolution make development of local FI methods, nondestructive deprocessing, and XRT critical.


||Glossary |
|---|---|

|CC SEM |Charge contrast SEM|

|CMP |Chemical mechanical polishing|

|CNT |Carbon nanotubes|

|CT AFM |Conductive tip AFM|

|DFT |Design for test|

|DG|Double gated (transistors)|

|EBIC |Electron beam induced current|

|FI |Fault isolation|

|ITRS |International technology roadmap|

||for semiconductors|

|LCE |Laser chemical etch|

|MCT |Mercury cadmium telluride|

|NbN |Niobium nitride|

|PEM |Photon emission microscopy|

|PFI |Physical fault isolation|

|PICA |Picosecond imaging circuit analysis|

|QD |Quantum dots|

|QE |Quantum effect (devices)|

|RIE |Reactive ion etch|

|RTD |Resonant tunneling diode|

|RTT |Resonant tunneling transistor|

|SET |Single electron transistor|

|SPM |Scanning probe microscope|

|SQUID |Superconducting quantum|

||interference device|

|STM |Scanning tunneling microscopy|

|XIVA |Induced voltage alteration|

||techniques (e.g., LIVA, TIVA)|

|XRT |X-ray tomography|

||References |

Technology Nodes子CMO5CMO5


Maleeular


130mm32mm


I mm


Viaible light, UV


汽


microocaps


Lg IaXRT


理


beckside 18


Techniquan学特别


SPMISTH


THM


军


SQULD


甲


Hicreprobes+学Defects*C2)APHDC BEM


、


LCI Z-reaolution CMP /mm removal rate


FIB spet


Almmic


I 16-051E-061E-071E-061E-0916-10


Resolution (m)


Figure 12:ApproximateresolutionofFA techniques compared with minimum sized defects for various technology nodes.


Whilethe timeframe for emergence of fully integrated nanoelectronic ICs is unknown, they will no doubt arrive in force. It is clear that with the exception of high-resolution surface imaging, the current FA toolset is woefully inadequate for single atom defects in single nanometer devices (Fig. 12).


The long lead-time before such fully integrated chips emerge must be used to work with researchers to design and implement built-in diagnostic capability,


C. Boit, The New Millennium: Challenges and


So the answer to the question of long-term FA


Analysis Desk Ref. 4h Ed., ASM International,


viability is of course: "It depends." It depends on


Materials Park, OH, p. 581, (1999).


D. Vallett, FA Future Requirements, in Failure


create advanced analytical instruments. And it


Techniques, edited by L.C. Wagner, Kluwer


depends on strong collaboration between industry,


Academic Publishers, Boston, MA, pp. 241-


concepts into solutions.


IC Technology Development, Proc. of the 7th


Acknowledgements


Analysis of Integrated Circuits, IPFA, p. 9,International Symp. on the Phys. & Failure


T.W. Joseph, R.E. Anderson, G. Gilfeather, C.


LeClaire, Semiconductor product analysis


challenges based on the 1999 ITRS, D. Yim,


Characterization and Metrology for ULSI


Technology2000InternationalConf.,


Gaithersburg,MD, USA, pp. 26-29 June (2000).


interest in nanotechnology.


of the 2001 8th International Symp. on the Phys.


and Failure Analysis of Integrated Circuits,


especially as self-assembly may erase the present advantages of a-priori layout knowledge.


1.The New Millennium: Challenges and  Opportunities,MicroelectronicsFailureOpportunities


harnessing existing technology to develop new FA2.FA Future RequirementsFailure Analysis of Integrated Circuits: Tools and tools. It depends on discovery of ‘new science’ toTechniques250,(1999).


academia, and tool suppliers to proactively turn


C. Boit, Can Failure Analysis Keep Pace with


3.Can Failure Analysis Keep Pace with  IC Technology Development(1999).


The author acknowledges Dr. Chuck Hawkins (Univ.4.


of New Mexico), Dr. Lee Knauss (Neocera, Inc.),


Semiconductor product analysis


Mr. Richard Ross (IBM Microelectronics), and Mr.


challenges based on the 1999 ITRS


Jerry Soden (Sandia National Laboratories) for


review and input; and Paul Vallett (Bellows Free


Academy High School) for piquing his father's


5.L.C. Wagner, Failure analysis challenges, Proc.Failure analysis challenges


IPFA,p.36-41,(2001).


Figure 12:


CMOS, IEEE Circuits and Devices MagazineCMOS


|6.|6.|International Technology Roadmap Semiconductors 2001 Edition, Semiconductor Industry Association, 4300 Stevens Suite Boulevard, Suite 271, San Jose, CA 95129.|International Technology Roadmap Semiconductors 2001 Edition, Semiconductor Industry Association, 4300 Stevens Suite Boulevard, Suite 271, San Jose, CA 95129.|International Technology Roadmap Semiconductors 2001 Edition, Semiconductor Industry Association, 4300 Stevens Suite Boulevard, Suite 271, San Jose, CA 95129.|
|---|---|---|---|---|

|7.|7.|E.J. Nowak, Maintaining the Benefits of CMOS Scaling when Scaling Bogs Down, IBM Journal of Res. and Dev., vol. 46 no. 2/3, (2002).|E.J. Nowak, Maintaining the Benefits of CMOS Scaling when Scaling Bogs Down, IBM Journal of Res. and Dev., vol. 46 no. 2/3, (2002).|E.J. Nowak, Maintaining the Benefits of CMOS Scaling when Scaling Bogs Down, IBM Journal of Res. and Dev., vol. 46 no. 2/3, (2002).|

|8. 9.|8. 9.|H-S. P. Wong, Beyond the Conventional Transistor, IBM Journal of Res. and Dev., vol. 46 no.2/3,(2002). R. Compano, L. Molenkamp, and D. J. Paul,|H-S. P. Wong, Beyond the Conventional Transistor, IBM Journal of Res. and Dev., vol. 46 no.2/3,(2002). R. Compano, L. Molenkamp, and D. J. Paul,|H-S. P. Wong, Beyond the Conventional Transistor, IBM Journal of Res. and Dev., vol. 46 no.2/3,(2002). R. Compano, L. Molenkamp, and D. J. Paul,|

|||Technology Roadmap for Nanoelectronics, Microelectronics Advanced Research Initiative -|Technology Roadmap for Nanoelectronics, Microelectronics Advanced Research Initiative -|Technology Roadmap for Nanoelectronics, Microelectronics Advanced Research Initiative -|

||MELARI NANO (1999). 10. edition, Academic Press (2001).|MELARI NANO (1999). 10. edition, Academic Press (2001).||D.J. Paul, Nanoelectronics, Encyclopedia of Physical Science and Technology, Third 25.|

|||||Aspects of Nanoelectronics, Proc. of the 24h|

||Hague, Netherlands, 22-24 Sept. (1998). 12. the IEEE, Vol. 85, No. 4 (1997).|Hague, Netherlands, 22-24 Sept. (1998). 12. the IEEE, Vol. 85, No. 4 (1997).||D. Goldhaber-Gordon, M.S. Montemerlo, J.C. 26. Love, G.J. Opiteck, and J.C. Ellenbogen, Overview of Nanoelectronic Devices, Proc. of|

||13. K. Matsumoto, Process to|13. K. Matsumoto, Process to|STM/AFM Room-Temperature-Operated Transistor and |STM/AFM Nano-Oxidation Room-Temperature-Operated 27. Single-Electron Transistor and Other Devices,|

||Proc. of the IEEE, Vol. 85, No. 4 (1997). 14. J .C. Ellenbo gen ,  and   Architectures for|Proc. of the IEEE, Vol. 85, No. 4 (1997). 14. J .C. Ellenbo gen ,  and   Architectures for|molecular|J. Christopher Love, electronic 28.|

||computers: 1. Logic built from molecular |computers: 1. Logic built from molecular |structures electronic | structures and an adder|

||built from molecular Corp., McLean, VA (1999).|built from molecular Corp., McLean, VA (1999).||iodes, Mitre 29.|

||15. trans Automation Conf. Proc., pp.94-98,(2002).|15. trans Automation Conf. Proc., pp.94-98,(2002).||R. Martel, V. Derycke, J. Appenzeiler, S. Wind, and P. Avouris, Carbon nanotube field-effect istors and logic circuits, 39th Design 30.|

SDL Imaging System


A schematic of the system is shown in Fig. 2. The SDL imaging system is similar to that described in Ref. 8.  A 1.3 µm near infrared laser, which produces the localized heating, is raster scanned by a scanning optical microscope (SOM).  The pass/fail state is monitored from a tester while the laser scans around the device. When the pass/fail state changes, a contrast variation will be produced in the SDL image.


Optimum sensitivity is achieved by selecting operating conditions that produce a non-zero probability of either a passing or failing condition occurring during each cycle of the vector set.  While this will produce a noisy image signal, extremely subtle changes in the pass/fail probabilities can still be detected.  The scan times can be similar to those used in Ref. 8; however, additional signal averaging is sometimes required to detect more subtle defects.


Voltage Amplifier


DUT


Tester


Computer control &image display


Optical


Scanning Microscope


Pass/Fail Status


Fig. 2. SDL imaging system.


SDL Imaging Examples


Three examples using SDL are shown as a demonstration.  The first example is from the front side on an ASIC, the second and third examples are from the backside on an advanced microprocessor.


In the examples, it should be noted that the SDL approach is similar to other global failure analysis tools in that a large area can be examined first and then higher magnification can be used in the SDL image contrast regions for site identification.


SDL on an ASIC


An ASIC was used for the front side example. No sample preparation was required. SDL localized a region on the ASIC where the logical output changes from a failing to passing condition with heating from the laser. The low magnification SDL contrast image and front side reflected light image is shown in Fig. 3.  A higher magnification view is shown in Fig. 4 that superimposes the SDL contrast image onto the front side reflected light image.


The site was identified as a parallel path in a race condition.  When heated, the switching transistor identified with SDL was slowed enough to allow the slower, parallel path to "catch up" and produce a functional passing condition.  Modifications were implemented that eliminated the race condition identified by SDL. We emphasize that no physical defect could be observed at the soft failure site.


Fig. 4. Higher magnification superimposed SDL(white grainy contrast as indicated by arrow) and reflected light image of the suspect site from Fig. 3.


SDL on an Advanced Microprocessor


In the second and third examples, SDL was performed on an advanced microprocessor from the backside. For sample preparation, the units were back-thinned and polished with an anti-reflective coating applied to the backside of the die14.


In the second example, the unit was intermittently failing in the control circuitry for the instruction cache. Results from SDL analysis are shown in Figs. 5 and 6. Fig. 5 is a low magnification SDL and reflected light image. Fig. 6 is a higher magnification SDL and reflected light image.  The identified site is the weak link in a serial conduction path that when slowed, produced a functional failure under the test conditions. Improvements to the process made the memory control circuit at the site less susceptible to process variations.


In the final example on an advanced microprocessor,a unit was failing the minimum voltage input high(VIH) or maximum voltage input low (VIL) electrical test at the input/output (I/O) pins. This is the minimum high or maximum low voltage allowable at a signal pin for that pin to register a high input as‘high’ or low input as ‘low’.  The device was fully functional otherwise. The failures were randomly distributed across the die; that is, no single I/O pin exhibited a higher degree of failure than any other I/O pin.  The pins that failed the VIH/VIL test did not fail for leakage, opens, or shorts.  However, it was observed that a small temperature increase exacerbated the problem.


Fig. 3.  Front side SDL (top) and reflected light(bottom) images of an area that increases the functional passing probability when heated. The site (indicated by the circle) was identified as a parallel path in a race condition.


Fig. 5. Backside SDL (top) and reflected light


(bottom) images of an area that decreased the


functional passing probability when heated. The


site was identified as the weak link in a serial


path.


The SDL technique was performed on the unit during a VIH/VIL electrical test. SDL analysis revealed several sites where the heat caused the I/O signal to either mostly pass or mostly fail the VIH/VIL test.


Fig. 7 shows the SDL results. The “fail-to-pass” sites are denoted in white while the “pass-to-fail” sites are denoted in black.  “Fail-to-pass” refers to when laser heating makes the device change from primarily failing to primarily passing, and vice versa for “passto-fail”.


Of particular interest is the thermally sensitive “failto-pass” site located on one of two filter capacitors between the input signal and the VCC power supply.


Heat applied to this particular spot on the filter capacitor caused the device to pass the VIH/VIL test.


Heat applied to any other filter capacitor to VCC (or any other portion of the suspect capacitor) failed to have any effect on the pass/fail status of the VIH/VIL test.


Fig. 6. Higher magnification SDL (top) and


reflected light (bottom) images of the suspect site


from Fig. 5.


Capacitor oxide damage was suspected; however,physical analysis failed to reveal any damage. The lack of damage suggested the capacitor was merely“leaky” at the SDL site but not a hard short.


Subsequent simulations showed that the small amount of leakage observed could cause a VIH or VIL failure. Improvements to the oxide fabrication completely solved the problem. This example shows


the ability of SDL to detect oxides with soft breakdowns.


Filter Caps to VSS


Filter  Caps to VCC


Fig. 7. VIH/VIL Fail: Overlay image of SDL sites and backside reflected image.  SDL “fail-topass” sites are denoted in white while the SDL“pass-to-fail” sites are denoted in black. The“fail-to-pass” site on the indicated VCC filter capacitor was observed to be leaky at the site.


The SDL methodology described here provides a new method for soft defect localization that is effective for both front side and backside failure analysis.  For the first time, using SDL, there is now a fast and convenient method to localize these types of defects that have historically been the most difficult type to localize due to their elusive nature. Like light emission microscopy2, SDL is global and is just as fast and easy to use. It is a powerful new addition to the set of failure analysis tools.


We would like to thank Glen Gilfeather, Robert Powell, Matt Thayer, Lee Rusk, Jeff Walton, Mark Miller, Bill Boothby of AMD and Rich Anderson of Sandia National Laboratories for their support during development. We would also like to thank the microprocessor product development group and Austin device analysis for their support. Sandia is a multi-program laboratory operated by Sandia Corporation, a Lockheed Martin Company, for the United States Department of Energy under contract number DE-AC04-94AL85000.


1. T.W. Joseph and B. Bossman, “Infrared laser microscopy of structures on heavily doped silicon,” International Symposium for Testing &Failure Analysis (ISTFA), pp. 1-7, Nov. 1992.


2. D.L. Barton, P. Tangyunyong, J.M. Soden, A.Y.


Liang, F.J. Low, A.N. Zaplatin, K. Shivanandan,and G. Donohoe, “Infrared Light Emission From Semiconductor


Devices,”


International Symposium for Testing & Failure Analysis(ISTFA), pp. 9-17, Nov. 1996.


3. M. Paniccia, T. Eiles, V.R.M. Rao, and W.M.


Yee, “Novel Optical Probing Technique for Flip Chip Packaged Microprocessors,” International Test Conference (ITC), pp. 740-747, Oct. 1998.


4. J.A. Kash, J.C. Tsang, D.R. Knebel, and D.P.


Vallet, "Non-Invasive Backside Failure Analysis of ICs by Time-Dependent Light Emission:PICA," International Symposium for Testing &Failure Analysis (ISTFA), pp. 482-488, Nov.


1998.


5. E.I. Cole Jr., J.M. Soden, J.L. Rife, D.L. Barton,and C.L. Henderson, "Novel Failure Analysis Techniques Using Photon Probing in a Scanning Optical Microscope," International Reliability Physics Symposium (IRPS), pp. 388-398, April


1994.


6. K. Nikawa and S. Inoue, “New Capabilities of OBIRCH Method for Fault Localization and Defect Detection,” Proc. of Sixth Asian Test Symposium, pp. 219-219, July 1997.


7. E.I. Cole Jr., P. Tangyunyong, D.A. Benson, and D.L. Barton, “TIVA and SEI Developments for Enhanced Front and Backside Interconnection Failure Analysis,” European Symp. On Reliability of Electron Devices  (ESREF), pp.


991-996, Oct. 1999.


8. E.I. Cole Jr., P. Tangyunyong, C.F. Hawkins,M.R. Bruce, V.J. Bruce, R.M. Ring, and W.L.


Chong, “Resistive Interconnection Localization,”International Symposium for Testing & Failure Analysis (ISTFA), pp. 43-50, Nov. 2001.


9. J. Segura and C. Hawkins, CMOS Electronics:How it works, How it Fails, to be published


2003.


10. R. Degraeve, B. Kaczer, A. De Keersgieter, and Gl. Groeseneken, “Relation between breakdown mode and breakdown location in short channel NMOSFETs,” International Reliability Physics Symposium (IRPS), pp. 360-366, 2001.


11. B.E. Weir, P.J. Silverman, D. Monroe, K.S.


Krisch, M.A. Alam, G.B. Alers, T.W. Sorsch,G.L. Timp, F. Baumann, C.T. Liu, Y. Ma, D.


Hwang, “Ultra-thin Gate Dielectrics: They Break Down, But Do They Fail?,” International Electron Device Mtg. (IEDM), pp. 73-76, 1997.


12. B. Kaczer, R. Degraeve, M. Rasras, K. Van de Mieroop, P.J. Roussel, and G. Groeseneken,“Impact of MOSFET Gate Oxide Breakdown on Digital Operation and Reliability,” IEEE Trans.


on Electron Devices, Vol. 49, pp. 500-506, Mar.


2002.


13. S. Kolachina, B. Taylor, K.S. Wills,“Application of TIVA in Design Debug,”International Symposium for Testing & Failure Analysis (ISTFA), pp. 497-501, Nov. 2000.


14. B. Davis and W. Chi, “Antireflection Coatings for Semiconductor Failure Analysis,”International Symposium for Testing & Failure Analysis (ISTFA), pp. 155-160, Nov. 2000.


Fault Localization and Functional Testing of ICs by Lock-in  Thermography


O. Breitenstein, J.P. Rakotoniaina, F. Altmann*, J. Schulz**, G. Linse**


Max Planck Institute of Microstructure Physics, Weinberg 2, D-06120 Halle, Germany  E-Mail: breiten@mpi-halle.de


*Fraunhofer Institute for Mechanics of Materials, Heideallee 19, D-06120 Halle, Germany **Melexis GmbH, Haarbergstraße 67, D-99097 Erfurt, Germany


In this paper new thermographic techniques with  significant improved temperature and/or spatial  resolution are presented and compared with existing  techniques. In infrared (IR) lock-in thermography  heat sources in an electronic device are periodically  activated electrically, and the surface is imaged by a  free-running IR camera. By computer processing and  averaging the images over a certain acquisition time, a surface temperature modulation below 100 µK can  be resolved. Moreover, the effective spatial  resolution is considerably improved compared to  stead-state thermal imaging techniques, since the  lateral heat diffusion is suppressed in this a.c. technique. However, a serious limitation is that the  spatial resolution is limited to about 5 microns due to  the IR wavelength range of  3 -5 µm used by the IR  camera. Nevertheless, we demonstrate that lock-in  thermography reliably allows the detection of defects  in ICs if their power exceeds some 10 µW. The  imaging can be performed also through the silicon  substrate from the backside of the chip. Also the  well-known fluorescent microthermal imaging (FMI) technique can be be used in lock-in mode, leading to  a temperature resolution in the mK range, but a  spatial resolution below 1 micron.


||16. A Dekker , Logic published online, October 4 (2001).|16. A Dekker , Logic published online, October 4 (2001).||. Bachtold, P. Hadley, T. Nakanishi, and C.  Circuits with Carbon Nanotube Transistors, Science, 294: pp. 1317-1320,|

|17.|P.G. Collins,H. Bando, and A. Zettl, Nanoscale electronic devices on carbon nanotubes, Nanotechnology 9,pp.153-157,(1998).|P.G. Collins,H. Bando, and A. Zettl, Nanoscale electronic devices on carbon nanotubes, Nanotechnology 9,pp.153-157,(1998).||31.|

||18. Review and 683-688,(2000).|18. Review and 683-688,(2000).|Letters, World|T.C. Shen, Role of Scanning Probes in Nanoelectronics: A Critical Review, Surface Scientific Publishing Company, Vol. 7, Nos. 5 & 6, pp. 32.|

||19. Self-Assembly and Nanoelectronics,|19. Self-Assembly and Nanoelectronics,||V.V. Zhirnov and D.J.C. Herr, New Frontiers: IEEE Computer Soc., Computer (USA) Vol.34, No.1,|

||Jan., pp.34-43 (2001). 20. 6, June (2001).|Jan., pp.34-43 (2001). 20. 6, June (2001).||T.I. Kamins and R.S. Williams, Trends in Nanotechnology: Self-Assembly and Defect 33. Tolerance, MST News (Germany), no.3, pp. 34-|

||21.|21.||J.A. Hutchby, G.I. Bourianoff, V.V. Zhirnov, and J.E. Brewer, Extending the Road Beyond|

D. Clark, Teramac: pointing the way to realTeramac: pointing the way to real  world nanotechnology, IEEE Computationalworld nanotechnology Science & Engineering (USA), Vol.5, No.3,July Sept., pp. 88-90 (1998)


Z.H. Levine and S. Grantham,X-Ray  aphy of Integrated Circuit  Interconnects: Past and Future, Proc. of the 27thnnects: Past and Future,International Symp. for Testing and Failure


W. Yun, D. Scott, and K.W. Nill, X-RayX-Ray  Nanotomography (XRMT) Tool for Nondestructive High-Resolution Imaging of ICs,tive High-Resolution Imaging of ICs Proc. of the 27" International Symp. for Testing and Failure Analysis (2001).


Campbell,K.A.Peterson,D.M.


Fleetwood, and J.M. Soden, Effects of focusedEffects of focused  ion beam irradiation on MOStransistors, Proc.on beam irradiation on MOS transistors Annual IEEE International Reliability Physics Symp., pp. 72-81 (1997).


P.A. Arutyunov and A.L. Tolstikhina, ScanningScanning (Tunneling and Force) Microscopy in  Metrological Problems of Nanoelectronics,gical Problems of Nanoelectronics Russian Microelectronics, Vol. 26, No. 6, pp.


T.W.Kelley, E.L. Granstrom, and C.D. Frisbie,ting Probe Atomic Force Microscopy: A  terization Tool for Molecular  Electronics,Advanced Materials,11, No.3,pp.lectronics


M. Sitti, Survey of Nanomanipulation Systems,Survey of Nanomanipulation Systems Proc. of the 2001 1st IEEE Conference on Nanotechnology,pp.75-80 (2001).


J.C. Tsang, and M.V. Fischetti, Why HotWhy Hot  Carrier Emission Based Timing Probes Will  Work For 50nm, 1V CMOS Technologies,For 50nm, 1V CMOS Technologies Microelectronics Reliability, 41, pp.1465-1470


W. Lo,K. Wilsher,R. Malinsky, N. Boiadjieva,C-C. Tsao, M. Leibowitz, and H. Deslandes,eneration Optical Probing Tools foe  Design Debug of High Speed Integrated   Proc. of the 28th International Symp.


for Testing and Failure Analysis (2002).


L. Shi, O. Kwon, G. Wu, and A. Majumdar,


Quantitative thermal probing of devices at sub100 nm resolution, Proc. of the 38th Annual resolution IEEE International Reliability Physics Symp., p.


W. Mertin, R. Weber, F. Seifert, and E.


Kubalek, Contactless Failure Analysis ofContactless Failure Analysis of  ted Circuits Via Current Contrast  Imaging with Magnetic Force Microscopy, with Magnetic Force Microscopy Proc. of the 27th International Symp. for Testing and Failure Analysis (2001).


M. Freitag, M. Radosavljevic, W. Clauss, andć A.T. Johnson, Local electronic properties ofLocal electronic properties of  all nanotubes circuits measured by  conducting-tip AFM, Physical Review B, vol.ting-tip AFM 62, no.4,R2307-R2310,15 July (2000).


Soft Defect Localization (SDL) on ICs


Michael R. Bruce, Victoria J. Bruce, David H. Eppes, Jacob Wilcox


Advanced Micro Devices, Inc., Austin, TX


Edward I. Cole Jr. , Paiboon Tangyunyong


Sandia National Laboratories, Albuquerque, NM


Charles F. Hawkins


University of New Mexico, Albuquerque, NM


We have developed a new scanning laser microscopy methodology, Soft Defect Localization (SDL), that directly locates soft defects from the front side and backside of an IC.  The method combines localized laser heating with the pass/fail state of a device to successfully localize soft defects.  Subtle, thermally sensitive soft defects can be localized by careful selection of the IC voltage, temperature, and operating frequency.  Several examples are shown.


Soft defects in integrated circuits (ICs) are responsible for functional failures when the IC is operated at certain conditions that may be within or outside of the normal limits for the part. These conditions include temperature, voltage, and frequency. Historically, soft defects have been the most difficult type of IC defect to localize, requiring a great deal of analysis and repetitive probing to identify the failing site. Additionally, the multiple levels of metal interconnection that obscure lower conductor levels and flip-chip packaging make IC front side examination techniques either difficult or impossible to apply.  This led to development of several backside IC analysis techniques such as infrared optical microscopy1, infrared light emission microscopy2, Laser Voltage Probing (LVP)3,Picosecond Imaging Circuit Analysis (PICA)4, LightInduced Voltage Alteration (LIVA)5, Optical Beam Induced Resistance Change (OBIRCH)6, and Thermally-Induced Voltage Alteration/Seebeck Effect Imaging (TIVA/SEI)7.  Unfortunately, these techniques are either ineffective or extremely time consuming in localizing soft defects.


To address soft defects, a new laser scanning methodology termed Soft Defect Localization (SDL)was developed that targets soft defect locations. The method combines two different concepts to successfully localize soft defects: 1) localized heating and 2) detection of changes in the pass/fail probability of a vector set.  The use of localized heating to change the pass/fail status of a cycled vector was originally reported with the Resistive Interconnect Localization (RIL) technique8.


Resistive Interconnects are one type of soft defects.


We found that by careful selection of the supplied IC voltage, temperature, and operating frequency, and by using signal averaging, other types of soft defects with far more subtle thermally sensitive characteristics can be localized.  After discussing the failure mechanisms that can produce soft defects, the SDL imaging system will be described followed by the presentation of several examples.


Soft Defects


Soft defects represent one of the most difficult classes of defects to isolate. They are generally characterized by elusive properties that allow the device to operate under specific conditions, but not under all environmental conditions9.  A device with a soft defect may fail intermittently or only in narrow pass/fail windows, and it can often be very sensitive to environmental parameters such as voltage and temperature.


Although by no means exhaustive, some of the more common causes of soft defects are:


•  Metallization or interconnect defects


o Via push up or voids


o Electromigration


o Stress voids


o Metal “mouse bites”


o Granularity


•  Oxide Defects


o Soft gate oxide shorts


o Hot carrier injection


•  Inter-level Dielectric (ILD)


o Voids


o Metal “slivers”


o Contamination


•  Process variations


o Transistor effects:


Vt shifts


Leff shift


Weff shift


NMOS to PMOS length ratio


Diffusion resistance


o Interconnect


Metal thickness variations  Spacing or pitch variations o Gate Oxide and ILD


Thickness variation


•  Operating or environmental conditions


o Frequency


o Voltage


o Temperature


Although many of the above listed defects can cause hard failures as well, keep in mind that we are referring to situations when these defects do not cause a hard functional failure in a device, but instead when they cause a soft defect; that is, the device will have some passing regions of operation or will operate intermittently. A discussion of some of these soft defects follows.


Metallization defects were thoroughly discussed in a previous paper on Resistive Interconnect Localization(RIL)8. This is one class of soft defects. Most metallization defects lead to a higher resistance interconnection, which in turn leads to propagation delays in a signal. This in turn may cause a failure flag in the test if it is too slow.  In some instances,involving voids or via-push-up, the resistance can actually decrease with temperature as shown in the previous work on RIL8.


Gate oxide defects have been a major concern since MOSFETs were first manufactured.  Defects in the older, thicker oxides usually manifested themselves as hard shorts after the breakdown of the insulating oxide, which led to hard functional fails.  For ultrathin oxides (<30 Å), instead of a hard short, defects are more likely to exhibit a soft breakdown which does not cause a hard functional failure9–12.  The soft breakdowns, which are irreversible, can lead to an increase in the noise of the gate voltage and/or elevated leakage in the oxide. After a soft breakdown a device will continue to operate within specifications in most cases; however, there will be cases where the


device will not operate under all specified parameters.  Soft gate oxide defects have been unusually difficult to detect; however, an example of a success using SDL will be shown in this paper.


Other defects can involve the ILD. Defects in the ILD can be due to voids, contaminants, thickness variations, or metal “slivers”.  This can lead to leakage currents or changes in the capacitance that may affect device performance.


Process variations are due to the uncontrollable nature of process parameters. These are not defects per se, but generally involve process parameters outside of the desired control window and may cause a device to fail within its normal operating parameters. These failures can be very difficult to resolve, as there are an enormous number of process parameters that can affect device performance.


Process variations can cause differences in metal or oxide thickness. These variations can lead to resistance and/or capacitance changes, cross talk, or increased inductance, to name a few. Some of the most important changes from process variations can occur in the transistor. Channel length or width variations, NMOS to PMOS length ratio variations,diffusion resistance changes, doping profiles, etc. can all have profound effects on the device performance.


These variations can translate into variations in the transconductance, drain drive current and threshold voltage (Vt) which in turn can cause soft defect errors in the test vector.  Transistor variations can also“wreak havoc” on sub-threshold leakage currents leading to increased power dissipation levels.


In order to ascertain the class or category of a soft defect, the operating or environmental conditions supplied to the IC are very important.  Some soft defects will fail under normal conditions, others will fail at extremes in operating frequency, voltage, and temperature.  Once the weak links causing the failure are identified by a technique like SDL, improvements can be made to the quality of the process and IC.


As described, soft defects are a diverse set and can represent very subtle failures.  While SDL represents a substantial breakthrough in localizing many types of these soft defects, particularly those with temperature sensitivities, it is not expected to detect everything.  Finally, it should be stressed that many of these defects leave no physical signature. For instance, with ultra-thin oxides, a physical defect is rarely observable after a soft breakdown. Instead, it will manifest itself only in the electrical properties.


Of course, this is one reason that soft defects are often difficult to detect. With SDL, detection has now become much easier for a wide class of soft defects.


Physics of SDL


At the heart of SDL is localized heat stimulation. In particular, it uses a 1.3 µm near infrared laser to locally heat a device. At this wavelength, unwanted photocurrents are not generated in the silicon. In addition, silicon is relatively transparent at 1.3 µm permitting analysis from either the front side or backside of the die1.


Because of the diversity of soft defects, their response to thermal stimulation will differ.


Fortunately, many defects are expected to have some sensitivity to heat. For instance, higher temperatures are known to slow device performance as metal resistance increases and transistor mobility decreases.


We, as well as others13, have observed that laser heating will slow down the switching speed of a ring oscillator. An example of this is shown in Fig. 1.  The frequency response of a ring oscillator is shown versus VDD. Also plotted is the decrease in frequency versus VDD under illumination from a 1.3 µm laser.


Ring Oscillator Frequency vs VDD


0 20


Decrease in Frequency (MHz)


<


40 (MHz)Frequency60 80


100


120 140 160 180 200


2.2


2.1


2.0


1.9


1.8


1.7


1.6


1.5


1.4


1.3


1.2


1.1


→


VDD (V)


0.4


个


Fig. 1. Frequency response vs. VDD of a ring


oscillator under 1.3 µm laser illumination. The


frequency of the oscillator is shown on the left


side (curve with the left arrow) and the decrease


of the oscillator frequency under 1.3 µm laser


illumination is shown on the right side (curve


with the right arrow).


As can be seen in Fig. 1, laser heating slows down the switching speed of the oscillator. This frequency reduction is believed to be due to decreases in mobility coupled with local power supply drops from longer times in saturation during switching transients and local metal interconnect resistance increases.


Additionally, leakage currents such as junction or oxide interface leakage, typically increase with


temperature. For temperature effects in metallization(interconnect), see Ref. 8.


Fault localisation in integrated circuits is the essential  starting point for an aimed structural and  morphological failure analysis with FIB-, SEM or  TEM. Liquid crystal investigations (LC, [1]) and  fluorescent microthermal imaging (FMI, [2]) are  standard thermal fault localization techniques, which  can be used to detect defects connected with local  heat generation in ICs such as oxide breakdown, latch-up, or metallization shorting. Steady-state  infrared (IR) thermography is also sometimes used  for this purpose, but it has two main disadvantages: Its spatial resolution is limited to about 5 µm owing  to the wavelength range used by the technique, and it  shows a strong IR-emissivity contrast (ε-contrast), which makes metallized areas appear dark and


obscures the thermal contrast. In principle the εcontrast may be compensated by capturing and  processing additional images at elevated  temperatures [3], but this is a time-consuming and  complicated procedure and often meets with limited  success. On the other hand, contrary to LC and FMI  imaging, IR investigations can be easily performed  from the backside of the chip, which is the only way  to investigate ICs in flip-chip mounting. It shares this  advantage with light emission microscopy (LEM,


[3]), which, however, does not image resistive heat  sources like metallization shorts. The detection limit  of all previously discussed thermal methods is  limited to 20 - 100 mK. Hence, they only allow to  image the mentioned pronounced heat sources, but as  a rule not regions of the normal operation of an IC. Decreasing operation voltages, multiple metallization  layers, and new package technologies complicate the  use of standard fault localisatation techniques, like  light emission microscopy and liquid crystal  thermography.


It will be shown that the IR lock-in thermography  technique considerably lowers the thermal detection  limit to below 0.1 mK [4] and eliminates the εcontrast with a single measurement by displaying the  phase image. The thermal diffusion length depends  on the lock-in frequency and is between 3 and 1 mm  for the lock-in frequencies of 3 - 30 Hz used here. However, this is no limit for the effective spatial  resolution, which also depends on the geometry and  the location of the heat sources. Point-like heat  sources at the surface can be located to an accuracy  of one pixel, and also the extension of the halo, which exists esp. around extended heat sources, is  usually smaller than the thermal diffusion length, but  considerably depends on the lock-in frequency, as  Fig. 3 will show. IR lock-in thermography is very  easy to apply and is also commercially available now


[5]. In addition, sub-micron spatial resolution can be  obtained by performing FMI in lock-in (a.c.) mode, which is currently under development. We are  introducing here first results of Lock-in FMI with 0.5 µm spatial resolution.


Proceedings from the 28th International Symposium for Testing and Failure Analysis, 3-7 November, 2002, Phoenix, Arizona


Experimental


The technique of IR lock-in thermography has been  used mostly for non-destructive testing and thermoelastic investigations [6], as well as for the  investigation of shunts in solar cells [7]. Periodic  heat pulses are generated in the sample by pulsing  the power supply to the IC. The surface is imaged by  a free-running thermocamera, and all pixel  information is digitally processed on-line to perform  a two-phase lock-in correlation, phase-referred to the  periodic heating. Hence, the primary results of lockin thermography are the in-phase (0°-) image and the  quadrature (90°-) image. They may be converted into  the amplitude image, displaying the local temperature  modulation amplitude, and the phase image, which  essentially describes the time delay of the local  temperature modulation referred to the periodic  power supply pulse. While the amplitude signal still  contains the ε-contrast, the phase image is principally  independent on the local value of the emissivity. By  averaging over many lock-in periods the signal-tonoise ratio (SNR) of a lock-in measurement drops  significantly below the SNR of the primary signal.


pulsed bias


CMT-FPA 384x288□detector


PC


frame grabber board


lock-in


reference


pulsed power


supply


PC-RAM


RS 232


DMA


object under investigation


hardware counter


Fig. 1: Scheme of the TDL 384 M 'Lock-in' thermography system


The lock-in thermography system used to take the  data included in this paper was the TDL 384 M  Lock-in from Thermosensorik GmbH, Erlangen  Germany [5] shown in Figure 1. It is based on a  highly sensitive 384x288 pixel sized Stirling-cooled  HgCdTe (MCT) focal plane array (FPA) IR detector  head made by AIM, Heilbronn (Germany) [8], which  detects at 3 -5 µm wavelength at a full frame rate of  up to 140 Hz. The digital image information (14 Bit) is captured by a frame grabber board and transmitted  on-line by DMA to the RAM of a 2x800 MHz Dual  Pentium III PC. The PC performs the lock-in  correlation and controls the hardware for generating  the lock-in reference signal, which triggers the pulsed  power supply. The detector head may be equipped  with a 28 mm standard IR objective, providing a  pixel resolution down to 30 µm, or by different  special microscope objectives, providing a pixel  resolution down to 5 µm. The temperature noise  level of this system decreases with the square root of  the acquisition time and reaches a level of about 70 µK after 1000 s (17 min). The digital lock-in  correlation procedure used in this system is  explained in Fig. 2 [4].


Additionally, we have modified a digital fluorescent  microthermal imaging (FMI) system to work in lockin mode. Here we exploit the natural 100 Hz  flickering of the UV lamp of the FMI optical  microscope. The supply voltage of the sample is  pulsed at 100 Hz, phase-synchronously to the mains  frequency, and the fluorescence signal is averaged  over many lock-in periods by a cooled slow-scan  CCD camera. Using special hardware, the phase  between the UV light pulses and the supply voltage  pulses is changed by 90° for successively captured  images, so that 4 subsequent fluorescence images


Fig. 2: Principle of the lock-in  correlation procedure [4]: The  pixel information of each  incoming frame is multiplied in  two channels by different sets  of


weighting


factors, approximating in channel 1 a  sin and in channel 2 a -cos  function. After summing up the  results in two frame storages  over many periods, storage 1  contains the in-phase (0°) image and storage 2 the  quadrature


(-90°) image, which may be  converted into the amplitudeand the phase image.


Heating power P


t


Multiplication by weighting factors


Result


Single incoming frames


(incl. topography


and noise)


∑1


∑2


F(t)


-1 1


sin(t)


-1


∆t=1/f frame


-cos(t)


sin(t)*F(t))


-cos(t)*F(t)


0°


-90°


correspond to a phase difference between light- and  bias pulses of  0°, 90°, 180°, and 270°. From these  four images the temperature modulation amplitude  signal A and the phase signal Φ are calculated for  every pixel position by:


) (


270


90


180


I


-


A


°


−


+


(1)


)


) 





−−


Φ


arctan


(2)


In principle this is a heterodyne technique, since  the  fluorescence signal is the product of the UV  intensity and the (temperature dependent) quantum  efficiency of the dye. Therefore the total amount of  light, averaged over many periods, contains some  amplitude and phase information about the periodic  temperature modulation at 100 Hz. By performing  the pairwise differences in the brackets of (1) and (2), the part of the fluorescence signal, which is not  affected by temperature modulation, completely  cancels out. Also here, by averaging over many  images the noise level may be considerably reduced.


For the comparison with other techniques Light  Emission Microscopy (LEM) has been performed  using an astronomical Peltier-cooled CCD-camera  AlphaMaxi from OES GmbH Egloffstein (Germany) with Kodak-chip KAF1600 in combination with a  Mitutoyo FS-70 microscope. The photo integration  times are indicated in the images. Liquid crystal  investigations have been performed using nematic  liquid crystals with a clearing point of 29°C under  the Mitutoyo FS-70 in cross-polarization modus. The sample temperature was regulated manually by  a hairdryer.


Results


IR Lock-in thermography


For lock-in thermography on ICs until now only  amplitude images have been published [4]. Fig. 3  shows an IR topography image (which is a single IR  image, always measured before a lock-in  measurement), and amplitude- and phase images of  an intact integrated circuit in static operation with the  supply voltage of 16 V / 2.4 mA pulsed at 3 and 20  Hz. Though also the topography image was measured  with supply voltage applied, the emissivity contrast  dominates this image and does obscure the weak heat  sources. In the amplitude images the stationary  topography contrast is compensated and the  dominant heat sources can be located. However, this  image is still modulated by the ε-contrast, and it is  hard to decide whether some bright features are weak


local heat sources or regions of high IR emissivity. The phase image, on the other hand, is totally free of  emissivity contrast and clearly shows single heat  sources. The influence of the lock-in frequency on  the extension of the inevitable halos around heat  sources is clearly visible both in the amplitude and in  the phase images. Moreover, it is visible that in the  phase image heat sources of different power appear  with a similar brightness.


Fig. 3: Topography, amplitude-, and phase images of  an IC in pulsed static operation for two lock-in  frequencies


topography


500 µm


amplitude, 3 Hz


phase, 3 Hz


amplitude, 20 Hz


phase, 20 Hz


Fig. 4: Topography and phase images of 3 positions  in an 8 bit microprocessor clocked at 12 MHz, supply voltage pulsed at 20 Hz, imaged "through the  chip" from the opened backside. The defect in  position c) is responsible for the increased supply  current.


Topography and phase images from the investigation  of 3 positions in an 8 Bit microprocessor IC are  shown in Fig 4. This IC was working in dynamic  operation with the internal clock generator of 12  MHz running, but no ROM was connected. The  supply voltage of 5 V was pulsed at 20 Hz. We have  investigated an intact IC consuming a current of  about 8 mA, and a defective one taking about 50 mA  at 5 V. The investigations have been performed from  the opened backside of the chip, as it has to be done  if chips are mounted in "flip chip" configuration. The  heat sources in the upper images a) and b) of Fig. 4


with a maximum amplitude of about 10 and  <1 mK, respectively, belong to the normal operation of this  IC. They are found both in an intact IC consuming 8  mA supply current and in the defective one. The  dominant heat source in Fig. 4 c), however, showing  an amplitude of about 1 K, is the fault location. In an  intact sample no measurable heat is produced in this  position. While the acquisition times for Fig. 4 a) and  b) were 2 and 20 min, respectively, Fig. 4 c) has been  recorded within some seconds


The final example shown in Fig. 5 demonstrates the  high sensitivity of the lock-in thermography  technique. This was a CMOS device damaged by  ESD pulses, which showed a leakage current of about  24 µA at an applied bias of 5.5 V, leading to a  dissipated power of 132 µW. The device was  measured under these conditions with a lock-in  frequency of 3 Hz for an acquisition time of tac = 7  min. The maximum measured T-modulation signal  amplitude in defect position was about 500 µK, and  the signal-to-noise ratio (SNR) was about 4, hence  the noise level of this measurement was in the order  of 125 µK. Since the noise level decreases with


ac


[4], after 1 hr acquisition time a heat source


of the same geometry with a power of 45 µW could  be detected with the same SNR. Note that this heat  source seems to have a certain spatial extension. For  a real point source at the surface the detection limit  would be even lower.


Fig. 5: Topography and amplitude image of a defect  in an IC dissipating 132 µW, measured at 3 Hz with  an acquisition time of 7 minutes


Meanwhile we have performed about 40 fault  localizations in different IC types by IR lock-in  thermography, hitherto all of them being successful. In some cases the fault origin was verified using FIB  cross section preparation of the fault region followed  by TEM failure analysis. Whenever a fault results in  a current increase of at least some ten microamps, it  usually can be localized by this technique to a spatial  accuracy of 5 ... 10 µm.


c)


Lock-in FMI


Fig. 6 shows one of our first results of Lock-in FMI. Here an NMOS test structure with an oxide  breakdown was investigated, leading to a leakage  current of 6.5 mA at 5 V. Also here the "topography  image" (a single fluorescence image) was captured  with a bias applied to the structure, showing a weak  quenching of the fluorescence in fault position. After <10 minutes acquisition time of Lock-in FMI, the  amplitude image clearly shows the point-like fault  position as well as a resistively heated line. The pixel  resolution in these images is 0.5 µm. Indeed, the  bright local signal maximum in fault position is  significant and defined by this spatial resolution.


Fig. 6: Fluorescence image (topography, top) and  lock-in FMI amplitude image (bottom) of a MOS test  structure containing an oxide breakdown (arrows) and a resistively heated line.


Comparison with other techniques


The IC investigated in this section (in some images  called device #3) was the same IC which was also  used for Fig. 3. It was a High-Voltage-CMOS motor  controller, which was damaged by ESD pulses. The  undamaged IC shows a quiescent current of about 40 µA and no light emission. Due to the damage the


quiescent current has increased to about 1 mA at Vcc = 10V and about 2.8 mA at Vcc = 16 V.


device#316√2.8mA


5x-object!e/600sintegratiotime


Fig. 7: Comparison between light emission image (top: green = topography, red = light emission) and  lock-in thermography (phase image, bottom, see Fig. 3) of an ESD pulse damaged High-Voltage-CMOS  motor controller


Fig. 7 shows a survey light emission image of the  defective sample at Vcc = 16 V and the amplitude  image and the phase image of the IR lock-in  thermography investigation of the same circuit under  the same conditions. The LEM results are displayed  as a superposition of the topography image (in green  color) and the light emission image in red color. Different positions are indicated as #1 through #5. Note that in the amplitude image (see Fig. 3) the  signal amplitude is proportional to the dissipated  power, and metallized regions appear darker due to  their low IR emissivity (emissivity contrast). The  phase image, on the other hand, is a measure of the  time delay of the local T-modulation with respect to  the modulated applied bias. So this image does not  contain the emissivity contrast, and heat sources of  different power may appear with a comparable  brightness. Note that the defect in position #4 shows  a T-modulation amplitude above the brightness  scaling limit, therefore this defect appears artificially  blurred in the amplitude image. The comparison  shows that some local heat sources detected by IR


amplitude


100 µm


lock-in FMI


开#1


#4


#5


#1


#2


#3


phase


lock-in thermography in positions #2 and #3 and also  the lower part in position #1 are not visible in light  emission. On the other hand, one light emission site (position #5) is only weakly visible in thermography (only in the phase image). Obviously the sites visible  only in thermography are purely resistive heat  sources, whereas the light source in position #5  seems to be connected with a very weak heat  dissipation. Generally, the spatial resolution of light  microscopy is clearly superior to that of IR lock-in  thermography.


device #3/position #1


LOT-picture/ 20x-objective


device #3/position #2


LCT-picture/ 50x-objective


tonbelure202582device #3/position #3


mu8/z0x-9Q|001N6


Fig. 8: Liquid crystal images of positions #1... #4 of  Fig. 7 in higher magnification


The next comparison is that between IR lock-in  thermography and liquid crystal thermography (LCT). Fig. 8 shows LCT images of positions #1, #2  and #3, and #4. In position #5 nothing was observed


in LCT. The LCT results generally confirm all IR  thermography results, but they also show the  limitations of LCT. It is complicated to obtain a  homogeneous LC thickness, especially at the die  edges there are always some dark positions, which  are not wetted. The real spatial resolution of IR  thermography is clearly better than that of LCT, though the nominal pixel resolution of LCT is  superior. This is due to the non-linear (step-like) contrast behaviour of LCT and to the lateral heat  spreading, which disturbs LCT but is suppressed in  lock-in thermography. So the IR thermography  amplitude images reveal that both in position #3 and #4 there are actually two heat sources, a strong and a  weak one. In both cases LCT allowed the detection  of either the stronger one, or both merged together, depending on sample temperature.


The final comparison is between IR lock-in  thermography and lock-in FMI (fluorescent  microthermal imaging). Our experimental lock-in  FMI system is not optimized yet to reach highest  possible detection sensitivity. Moreover, the applied  bias was limited to 10 V here for technical reasons. A  problem is also the degradation of the dye limiting  the measuring time to about 20 min. Therefore only  the heat source in position #4, which was the  strongest one, could be investigated by lock-in FMI. Moreover, another device of the same type than that  used for the previous investigation was used for this  comparison. This device showed the same ESDinduced fault as the previous one, but the primary  defect was in a slightly different position. Fig. 9  shows a comparison of the IR lock-in thermography  amplitude and its topography image, and the lock-in  FMI amplitude image together with its topography  image, all measured at Vcc = 10 V. The region  imaged in FMI is framed in the IR thermograms.  These images are rotated by 180° with respect to  Figs. 3, 7, and 8. In this IR amplitude thermogram  the brightness scaling was optimized for the  dominant defect in position #4, in contrast to the  image in Fig. 7. The comparison in Fig. 9 shows that  the detection sensitivity of our present experimental  lock-in FMI system is still far below that of IR lockin thermography. However, the spatial resolution of  lock-in FMI is clearly superior to that of IR  thermography and comparable to that of light  emission microscopy. There are some other fault  detection techniques like TIVA (Thermal Induced  Voltage Alteration) [9] or OBIRCH (Optical Beam  Induced Resistance Change) [10], which could not be  compared to lock-in thermography yet, since the  authors had no access to these techniques. These  techniques rely on changes of the quiescent current


50 µm


34


on the action of a focused Laser beam. Lock-in  thermography could have an advantage to these  techniques, since it also allows the detection of weak  leakage sites in ICs having a large quiescent current (see Fig. 3).


Conclusions and Outlook


IR lock-in thermography shows a considerably better  thermal resolution than previous thermal imaging  techniques. This technique has the potential to  become a new standard technique for fault  localization up to an accuracy of 5 µm. Lock-in  thermography may also be used in flip-chip  configuration. Other advantages include its ease of  operation, since it needs no foreign layer at the  surface, no room darkening, the results are  straightforward to interpret, and there is no  degradation as for FMI.


The comparison between different thermal fault  detection techniques has shown that lock-in  thermography is able to detect practically all defects, which are visible also in light emission microscopy. We have estimated a detection limit of this thermal  technique of below 0.1 mK corresponding to about 3 µW for point heat sources [4] and some 10 µW for  slightly extended sources, which is well below the  detection limit of liquid crystal thermography. A  number of heat sources visible in IR lock-in  thermography don't show any light emission, since  lock-in thermography detects a different physical  mechanism than does LEM. Therefore in some cases, lock-in therography may be more useful, and in other  cases LEM may be more useful. Unfortunately, the  spatial resolution of IR lock-in thermography is  limited to 5 µm because of the IR wavelength of 3 - 5 µm used. Here lock-in FMI may become an  interesting alternative in future by detecting local  heat sources with sub-micron spatial resolution. The  presupposition is, however, that the hitherto  unsatisfactory detection sensitivity of lock-in FMI  can be considerably improved. Corresponding work  is underway.


In future the frequency range of IR lock-in  thermography will be extended up to 1 kHz, leading  to a further improvement of the effective spatial  resolution. Moreover, IR lock-in thermography or  lock-in FMI may become integrated into an  intelligent IC testing station, which activates and  deactivates certain functional groups in the pace of  the lock-in correlation. In this way the correct


operation of well-defined functional groups in ICs  can be tested thermally.


Zoirw


20μm


Fig. 9: Lock-in thermography amplitude and  topography images (top) and Lock-in FMI amplitude  and topography image (bottom) of defect #4 in Fig. 7


This work was supported by the BMBF projects No. 0329743B (DIXSI) and KA 0015101AJS0 (FASµm).


||References |
|---|---|

|1. |N. Hirayama, K. Nikawa, M. Nakagiri, Proc. ISTFA 1986, pp. 139-144 |

|2. |P. Kolodner, J.A. Tyson, Appl. Phys. Lett. 40, 782 (1982) |

|3. |www.quantumfocus.com |

|4. |O. Breitenstein, M. Langenkamp, F. Altmann, D. Katzer, A. Lindner, H. Eggers, Rev. Sci. Instr. 71, 4155 (2000) |

|5. |www.thermosensorik.com |

|6. |X.P.V. Maldague: Theory and Practice of Infrared Technology for Nondestructive Testing, Wiley (New York) 2001 |

|7. |O. Breitenstein, M. Langenkamp, O. Lang, A. Schirrmacher, Solar Energy Materials  Solar Cells 65, 55 (2001) |

|8. |www.aim-ir.de |

|9. |www.optomet.com |

|10. |usa.hamamatsu.com |

U. Muehle1, A. Lenk2, M. Lehmann2, H. Lichte2


1 Infineon Technologies Dresden GmbH & Co OHG, Physical Failure Analysis, Germany  2 Dresden University, Institute of Applied Physics, Germany


1. Introduction


In accordance with the predictions of the  International Semiconductor Association [1] we  expect a further decrease in the structural widths of  semiconductor devices. For an in depth  characterization of actual structural details, the  Transmission Electron Microscopy (TEM)-technique  is becoming more and more significant [2]. An urgent  requirement is in the visualization of dimensions of  the doped regions and estimation of p-n-junctions  profile with a high level spatial resolution. Former  techniques addressing this challenge like wet etching  for SEM-imaging [3], etching of TEM-lamellas [4], or  scanning capacitance observations [5] are not  sufficient to reach this goal with adequate reliability  and reproducibility. However, off-axis electron  holography, a special TEM-technique is able to  visualize electrically active areas in semiconductors


[6]. For the application of this technique in an  industrial environment a target preparation, based on  Focused Ion Beam (FIB) -techniques [7] is necessary. Samples for holography have to fulfill some special  requirements. The present paper describes a way to  achieve sample preparation for TEM-holography from  actual memory products and also provides an idea of  the potential of this technique for semiconductors  failure analysis.


2. Physical basics


The interaction between the electron waves and the  solid state sample in the TEM influences both the  amplitude and phase of the incident wave. Differences  in intensities between sample locations are directly  visible on screen or image. Intensity at each location  is proportional to the square of amplitude at that  location.  Their origin is the summary of individual  scattering processes of electron waves during  transmission, dynamic effects of interaction between  electron wave and sample as well as wave aberration  of the objective lens.


The phase shift ϕ is determined by the mean inner


potential V0 of the solid state by


( 1 )


where t is the foil thickness and σ is an interaction


constant [8]. The mean inner potential of silicon is  about 12V [6]. The space charge region, developed at  a junction between different doped regions changes  the local depletion region inner potential V∆pn about +/- 0.7V. This leads to local differences in phase shift ∆ϕ, according to


( 2 )


where the active foil thickness has to be reduced by  the so called dead layer t0{[9], see fig. 1. Since only  the intensity can be recorded in a conventional TEMimage, a method for recording the complete wave is  necessary.


Figure 1: Behavior of an electron wave during  transmission through a semiconductor sample (surrounded by solid line): The phase shift between  object wave and vacuum wave is different between nand p-doped regions. This difference constites about  10% of the total phase shift of the sample compared  to vacuum wave. The dead layers (d) do not  contribute to ∆ϕ.


Off-axis electron holography solves this problem by  generating interference between the object wave and  an unmodulated vacuum wave and recording the  resulting pattern. Using Fourier analysis, it is possible  to separate the contributions of phase and amplitude  to the hologram and exploit them separately.


V0


σ


ϕ =


2t


V


n


p −


∆


ϕ


f 0


f 0 f n f p


? f


d


p


3. Technical Solutions


For practical accomplishment of electron holography  an electron beam with high coherence is necessary, which can only be achieved by FEG-emitter [10]. After  passing through the specimen the object wave  contains the phase information. The object wave can  be compared with a vacuum wave with un-modulated  phase (fig. 2), which travell very close to the sample.


Figure 2: Principle of electron holography: Object  wave and un-modulated wave are brought together to  form an interference pattern using the biprism. The  interference pattern is a hologram, from which, by  means of Fourier analysis a phase image revealing the  phase differences is reconstructed. The interference  pattern of the hologram also contains the  conventional image information.


The interference of both parts is accomplished by a  so-called “Moellenstedt Biprism” [11]. This consists  of a positively charged wire, tilting the wave fronts  against each other. It is situated in the plane of the  selected area aperture and can be rotated to the  optimum position with respect to the sample. The


19 1/mm


resulting hologram, (fig. 3), is recorded by a high  resolution CCD-camera. The deformation of the  interference fringes at the location, where the borders  of the doped region intersect, provides some idea  about the kind of information that can be obtained. A  Fourier analysis of the image (fig. 4), yields a  reconstruction of phase and amplitude images [12]. For reconstruction “Holoworks”-software, improved


by several scripts from the Triebenberg laboratory, is  used as a plug-in for GATAN’s Digital Micrograph.


Figure 3: Example of a recorded hologram: fringes  nearly parallel to substrates surface dominate the  image. Some details, well known from the bright field  image, like (a) the Gate Contact are slightly visible. (b) At the location, where the p-n-transition is expected, the fringes seem to be bowed out.


For holographic investigations of semiconductor  structures the normal objective lens of a TEM is not  suitable. They are designed for high magnifications  and include only a small field of view, not enough for  imaging a sufficient area of the structure and the  vacuum beam as well. The application of a Lorentzlens is able to overcome this limitation, but results in a  much larger spherical aberration, leading to more  stringent demands on alignment and handling of the  tool.


Figure 4: Fourier analysis of hologram: The image  shows the Fourier transform of a Silicon substrate. After separating the sideband (circle) only and


wnm


N


wwinwnunwnPlane waveSi-sample号Phase shift depending ondopants concentration Bipris


Hologram, aquired by GATAN-CCD-camera


Fourieranalysis


Phase and amplitude image


retransformation a phase image is obtained. Note that  the Fourier transformation of a complicated structure  is not so clear.


Figure 5: TEM-cross section of a typical test  structure: On the Si-substrate with the device three  layers of metal (a, b and c) are situated, connecting  source and drain areas.


Taking into account all the physical and technical  aspects, some particular requirements for TEMholography specimens can be formulated:


(a) The thickness of the sample has to be much  larger than the usual TEM-specimen. As can be  seen in eq. 2 the signal is proportional to the foil  thickness. To distinguish the signal clearly from  the background noise a large foil thickness is  recommended. On the other hand, the  transmitted coherent intensity decreases with  increasing foil thickness. The optimum  relationship between these two aspects was  found at a foil thickness between 200 and 300 nm


[13]. As a consequence of this not all  semiconductor structures are suitable for  holographic investigations. In a cross section of  a MOS-transistor the gate width becomes the zdimension of the TEM-sample. For a convenient  preparation it has to be large as well, whereas  the x-direction (gate length) is not restricted.


(b) The edge of the sample has to be situated as  close as possible to the doped regions in order  to keep the distance to the reference wave short. Hence all additional layers above the silicon (fig. 5), especially the metalization, should be  removed without remaining topography.


(c) Because the depletion region potential V∆pn is  about one order of magnitude lower than the


mean inner potential, local changes of foil  thickness have to be kept very low. To obtain  useful phase images with a sensitivity of 10% in  phase shift, the requirement for thickness  variation is less than 1%.


4. Sample Preparation


In order to fulfill condition 3a, transistors designed for  electrical tests were chosen for TEM-holography. The  electrical requirements on geometry of this transistors  are very similar to a sample for TEM-holography (fig. 6). These structures are present in the test structure  between the chips of every memory product. The test  structure represents the real manufacturing  technology for p-FET’s as well as for n-FET’s. They  yield transistor parametric data. A gate width of about  10 µm is large enough to prepare a comparably thick  TEM-foil homogeneous in z-direction. Because our  test structures have a parallel layout to each other, it  is possible to prepare a few TEM-lamellas in one


sample.


Figure 6: Design of the test structures, chosen for  electron holography: The part above the white line  shows a row of pads with transistors between (arrows). The lower part shows one transistor at the  plane of the first metalization (see layer “a” in fig. 5). Below location “a” is the gate contact, “b” indicates  the connections of source and drain.


Source and drain contacts of the MOS-transistors are  connected over adjacent pads using second  metalization layer, as seen in cross-section (fig. 5). To  fulfill the 3b condition it was necessary to remove all  metalization layers above the gate contact. In practise, mechanical polishing was the most feasible method to  achieve this without creating surface topography.


An FIB system does not generate an ideal rectangular  edge due to the Gausian shape of the beam. [14]. When an FIB is used the resulting edge becomes  beveled, deviating from ideal vertical direction. This  bevel depends on the sputtering resistance of the  material above the silicon and leads to the so-called   curtaining effect and to considerable variations in foil  thickness (figure 7).


Figure 7: Curtaining effect of FIB-preparation: Different materials above the Silicon substrate lead to  variations in foil thickness, visible as alternating  contrast fringes.


To avoid this only homogeneous materials should  cover the sample to guarantee no ion beam curtaining. The dense tungsten metallisation, (contacts, upper  part of gate contact) must be removed because of its  ability to create a curtaining problem in the sample. The removal of the tungsten can be accomplished by  a single step chemical etching.


Another problem with sample generation is the  deposition of the platinum bar, which acts as a  protecting layer for the lamella. The deposition  process causes an amorphisation of the silicon  substrate up to a depth of 50 nm (fig. 8). To combat  the amorphisation an amorphous silicon layer of  thickness of approximately 50 nm is deposited prior to  the platinum bar.


Pt


C


50 μm


Figure 8: Amorphisation of Si-substrate (a) during  Platinum deposition: The thickness of the amorphous  range (b) is about 50 µm.


In general, the preparation of a cross-section sample  for final FIB-work from the piece of the wafer as well  as FIB-preparation itself was done like any FIBpreparation at Infineon DD PFA [15]. Some special  features have to be taken into account:


(a)  The protective platinum bar at the location of the  later lamella should not exceed a thickness of  about 100 nm in order to keep the distance  between object beam and vacuum beam short, (see 3b). Note that such a thin layer can be  consumed relatively fast during scanning. Image  acquisition during FIB-work should be reduced  to a minimum.


(b)  As mentioned above, a small bevel at the edge  of the sample arises by perfectly vertical  sputtering. To obtain a lamella as flat as possible  it is recommended tilting the sample slightly  against the beam during the last polishing steps.


(c)  The desired final thickness of the lamella can be  observed very well. For a better comparison of  different samples, a standard thickness between  200 and 300 nm is recommended.


5. Results


The samples were investigated at the “Triebenberg  laboratory” of the Institute of Applied Physics at the  Dresden University [16]. The laboratory is optimized  for high-end TEM-work by reducing electric and  magnetic fields, as well as seismic influences and all  kinds of background. For the holographic  investigations a Philips CM200FEG ST/Lorentz  electron microscope equipped with a rotatable biprism  was used.


Figure 9: Phase image of a p-channel FET: The dark  bar indicates the location of the former gate contact. Bright lines from A to B and A to C show the location  of the line plots (Fig. 10).


Figure 9 shows the phase image of a p-channel FET. The electrically active areas below the source and  drain contacts are visible as dark clouds in the Sisingle crystal. The former location of the gate contact  is only slightly visible only in the phase image. This is  a result of thorough delayering and the completely  different contrast behavior of the phase image. The  base of the corresponding bright field image indicated  the location of the gate contact. So a complete  characterization of the observed transistor is feasible.


3.0


2.5


中2.0


50100150


hmB


3.5


3.0-


中2.5-


b 1


Figure 10: Line plot of the phase shift vs. location in  figure 9 from A to B (upper part) using an integration  width of 50 pixel and from A to C with 20 pixel.


The gray scale image can give only an optical  impression of active areas. For a better understanding  of the dopants behavior, diffusion length’ etc. a  quantitative evaluation is desired. In order to make a  quantitative determination the gray levels in the image  are converted to real values of phase shift between 0  and 2π. A plot of these values vs. location including  some characteristic points can be used to distinguish  different transistors. From the generated images a  comparison of different transistors, (figure 10), can  also be obtained. Integrating over the width of the  present homogeneous range can improve the ratio  between signal and noise. For noise reduction  integration of adjacent pixels in both the horizontal  and vertical directions is required. In the example  shown the integration for the line A – C is limited to  20 pixels due to the rapid variation of dopant  concentration perpendicular to A – C.  Along line A – B the integration width can be expanded to 50 pixels  due to the flatness of the diffusion bottom. The


resultant plots achieve better spatial resolution than  single line measurements and some information about  the real differences in mean inner potential is obtained  as well.


1.5-A


nmC 100200300400500


Figure 11: Phase images of p-channel-FET (a) and nchannel-FET (b): The line plot along the white line of  p-FET shows a much stronger difference in phase  shift (ϕ = 2.0 vs. 0.8) than in case of n-FET.


The visualization of doped regions works for pchannel FET’s as well as for n-channel FET’s (figure  11). When comparing the phase difference between nchannel- and p-channel-FET’s, about twice as much  phase shift is seen in the case of p-channel FET [17]. This is caused by different values of dopant  concentrations and leads to a decreased ratio  between signal and noise for n-channel FET’s.


0 1 2 3 4 5


200


300


一p-FET


n-FET


≈  0.9


≈  2.0


c


A structure designed for the development and testing  of prospective memory products provides another  example of the electron holography. The structure  consists of straight lines, doped with 1020 cm-3 As in  1017 cm-3 B-doped substrate. After ion implantation  the wafer was annealed with different process  parameters, leading to different distributions of  dopants. Using the holographic method it is possible  to characterize the diffusion depth and the electrical  activation of Arsenic, (fig. 12). In order to obtain  quantitative results phase shift vs. location should be  displayed, starting at a defined point, (fig. 13).


200nm


4.5


4.0


3.5-


b


nm


250nm


重


1.0-


0100200300400500


0.5+


0100200300400500 A


Figure 12: Electrically active area resulting from As-C


Implantation and following anneal: A line plot (see fig. 13) from A to B, where the white rectangle  demonstrates the integration width, allows an  estimation of the diffusion profile.


Figure 13: Line plot in fig. 13: Using the center  between upper and lower level of mean inner potential  we find about 120 nm diffusion depth.


For a more complete understanding of the dopants  behavior and for the determination of the exact


location of p-n-transition, it is necessary to simulate  their influence on the mean inner potential [18] and  compare the result with figure 13. Work in this area is  still ongoing. The distance between the decrease of  potential determines the electrical behavior of the later  product. Figure 14 compares this distance for the  different diffusion profiless as observed in fig. 12 and


13.


|A|B|
|---|---|

|a||

Figure 14: Two neighboring diffusion areas like the  ones shown in fig. 12 (a): Different parameters of the  anneal lead to different distances (b and c) of  electrically active areas, important for the electrical  behavior of the structure.


Performing this type of analysis directly after a


1.4-


questionable annealing process can yield valuable


information about the actual outcome of the anneal


太


before the wafer is completely processed.  Early


1.0-120nm


knowledge of the dopant profile can accelerate


0.8-A


development cycles. Electron holography can also be


050100150200


used for process monitoring.


hm


6. Summary


Electron holography enables us to visualize the  doped regions of semiconductor structure with a  spatial resolution in the dimension of the Debye44


length. To perform Electron holography on a structure  of interest FIB sample preparation is mandatory due  to the more stringent sample requirements as  compared to conventional TEM samples.


In this paper we showed that different types and sizes  of FET’s and testing structures could be visualized. The results obtained from electron holography can  act as an input for quantitative investigations and/or  verify these investigations.


7. Acknowledgements


The work for this paper was supported by the EFRE  fund of the European Community and by funding of  the State Saxony of the Federal Republic of Germany (project number 6327). The authors are responsible for  the contents of the paper.


5. T. Trenkler, P. De Wolf, J. Snauwaert, W. Vandervorst, L. Hellemans, J. Vac. Sci. Technol., B16, 355 (1996)


6. W. D. Rau, P. Schwander, F. H. Baumann, W. Höppner, A. Ourmazd, Phys. Rev. Lett. , 82, 2614-2617 (1999)


7. J.F. Walker, European FIB Users Group Meeting  at ESREF, 1998


8. A. Tonomura, L. F. Allard, G. Pozzi, D. C. Joy, Y. A. Ono (Editors), Electron Holography, Elsevier  Science B. V. (1995) 69-79


9. A. C. Twichett, R. E. Dunin-Borkowski, P.A. Midgley, Phys. Rev. Lett., 88, (2002)


10. H. Bethge, J. Heydenreich (Editors), Electron  Microscopy in Solid State Physics, Elsevier  Amsterdam, 1987


11. G. Moellenstedt, H. Dueker, Zeitschr. f. Physik , 26, 377-397 (1956)


12. W.D. Rau, H. Lichte, E. Voelkl, U. Weierstall, Jour. Comp.-Aid. Microscopy, 3, 51-63 (2001)


13. A. Lenk, Diploma Thesis, TU Dresden, 2001


14. G. Auvert, European FIB Users Group Meeting  at ESREF, 1998


|1. |Y. El Mansey, VLSI-Symposium and Silicon Technology Honolulu, 2000 |
|---|---|

|2. |C. Boit, 8th International Symposium on the Physical and Failure Analysis of Integrated Circuits IPFA, Singapore, 7-12, 1999 |

|3. |C. Spinella, V. Raineri, M. Saggio, V. Privitera, S. U. Campasino, Nucl. Instr. a. Meth. i. Phys. Res., B96, 139-143 (1995) |

|4. |H. Cerva, J. Vac. Sci. Technol.; B10, 491-495 (1992) |

15. B. Schwalbe, Diploma Thesis, TU Dresden, 1997


16. www.triebenberg.de


17. A. Lenk, H. Lichte, U. Muehle, 3 Countries  Conference on Electron Microscopy Innsbruck , 2001


18. Z. Wang, K. Sasaki, N. Kato, K. Urata, T. Hirayama, H. Saka, Jour. Electron Microsc., 50, 479-484 (2001)


A Study of Photoelectron Emission Microscopy Contrast  Mechanisms Relevant to Microelectronics


Vincent Ballarotto, Karen Siegrist, Ellen Williams and William Vanderlinde


Laboratory for Physical Sciences and the University of Maryland  8050 Greenmead Dr, College Park, MD  20740


We report on a quantitative investigation of  doping-induced contrast and topography-induced  contrast in photoelectron emission microscopy (PEEM).  Calibration samples were fabricated  using standard photolithography and focused ion  beam writing to test both types of contrast.  Using a near-threshold light source, we find that  the doping-induced contrast increases  monotonically with B concentration over the  measured range of 1017 – 2x1020 cm-3.  The  variation in doping-induced contrast as incident  photon energy is varied was also investigated.  Optimal doping-induced contrast and PEEM  sensitivity is achieved by imaging with photon  energy slightly above the highest nominal  photothreshold of interest.  The photoemission  model, based on near-threshold emission, used to  describe doping-induce contrast gives good  agreement with the measured intensities. Thus, measuring the relative intensity ratio provides a  robust technique for determining doping levels.  Topography-induced contrast was investigated  by imaging Ti samples of various step heights (75, 150, 290, and 550 nm).  Image data suggests  that edge contrast increases with step height.  Numerical simulations show that non-uniform  electrostatic fields at step edge are responsible  for this contrast.  Experimentally, we  systematically vary the lateral field strength and  show that edge contrast can be controlled.  This  technique could be useful in failure analysis by  identifying breaks in metal lines.


The photoelectron emission microscope (PEEM) is a novel microscope that has several features  that may be useful for failure analysis, as well as  being a processing diagnostic of Si.  Furthermore, this technique offers high spatial  resolution and good temporal resolution  necessary for practical inspection of large areas  of devices.  In particular, PEEM has a nominal  spatial resolution of 80 nm, in addition to a large  field of view (200 µm) that allows video rate  analysis.  Thus, real-time imaging of doped areas


in silicon which may be difficult to image by  other methods can be done.  Perhaps more  importantly, PEEM has unique contrast  mechanisms that are relevant to device  characterization.  As an example, we show a  PEEM image from a CMOS logic array in Figure


1.  It is immediately obvious that the image is  quite complex.  The contrast in this image is a  combination of several mechanisms, including  doping level contrast, surface topography and  material contrast.  To quantify the available  information, the individual contrast mechanisms  that are present need to be identified and  characterized.  To achieve this goal, it is more  productive to analyze simple model devices so  that the information available in a PEEM image  can be extracted.


We have been doing both theoretical and  experimental studies on simple device models in  order to understand how contrast mechanisms, individually and in combination, produce a  PEEM image.  For example, theoretical studies, which include models based on standard surface  science ideas1 along with numerical simulations  of the microscope, are being used to establish a


Figure 1: A PEEM image of a CMOS logic array. Several different sources are present, including


doping-induced and topography-induced contrast.


The field of view is ~150 µm.


Proceedings from the 28b International Symposium for Testing and Failure Analysis, 3-7 November, 2002, Phoenix, Arizona


quantitative basis for PEEM image  interpretation.  Consequently, several types of  contrast that occur in PEEM imaging have been  identified as relevant to device characterization.  In particular, spatial variations in photothreshold  and sample topography are two sources of  contrast that are applicable to image analysis of  integrated circuits.  We present here a detailed  investigation of doping-induced contrast and  topography-induced contrast that occurs in  PEEM of simple devices.


In PEEM the imaging electrons are  photoelectrons generated by absorption of  ultraviolet light in the specimen.  A grounded  sample serves as the cathode while the anode, a  flat metal electrode with a centered aperture  allowing for passage of the photoelectrons, is  held at approximately 10 kV.  The resulting  electric field (~ 106 V/m) is used to accelerate  the photoelectrons toward the imaging column of  the microscope that is usually several millimeters  away.  Typically, the electrons will then pass  through a series of electrostatic lenses that are  used to magnify the image.  Finally, the  photoelectrons are projected onto a detector that  converts the electron image into a visible one.  This is the image that is recorded for image  analysis.  A detailed description of image  formation in PEEM is given by Rempfer and  Griffith.2


A commercial PEEM (Staib PEEM-350) mounted in a UHV stainless steel chamber was  used to image the devices.  All imaging was  done in a vacuum of approximately 10-9 Torr.  The samples were mounted approximately 4 mm  from the aperture of the objective lens.  The light  source was a 100 W mercury short-arc lamp  which produces a continuous spectrum up to  roughly 5.15 eV.  In addition, imaging was done  with spontaneous coherent radiation from the  Duke University UV free electron laser (FEL).  Data at the FEL was obtained using photon  energies ranging from 4.5 to 5.2 eV with a  focused intensity of 10 W/cm2.  A chevron-type  multi-channel plate is used to intensify the  images approximately a million times.  Typically, the images are recorded using a 12-bit  CCD camera which produces a 1280x1024  bitmap.  Quantitative assessment of the resulting  PEEM image contrast was done by averaging  sets of parallel line scans to produce an intensity


profile with a rms fluctuation that is less than 1% of the average intensity from the n-type  substrate.


A number of devices have been designed and  fabricated to investigate the individual contrast  mechanisms.  To investigate doping-induced  contrast, a lateral array of pn junctions was  formed by broad-beam implantation of boron  ions (1018 cm-3, 190 keV) through a mask into an  n-type Si(001) substrate (P, 1014 cm-3).  The  structures were then modified using focused ion  beam (FIB) writing to allow systematic variation  of the doping levels.  The nominal doping levels  of the additional FIB lines ranged from 1018 to  6x1020 B+ cm-3.  Subsequent to implantation, the  samples were annealed at 1100 ºC for 60 s to  activate the dopants.  We have found that no  chemical etching is necessary prior to loading the  samples into the PEEM chamber, thus a native  oxide is present on the degreased Si substrates.


To experimentally investigate topographyinduced contrast, 0.5 µm of Ti was evaporated  onto a Si substrate using an electron beam  evaporator.  A positive photolithographic pattern  was then used as a etch mask.  Topography was  systematically generated (see Figure 2) by  optimizing an rf plasma etch of SF6 to produce  the desired profile.


Well-defined steps from 5 to 500 nm in height


can be produced.  After the desired topography  was achieved, the etch mask was chemically


removed with 1-methyl 2-pyrrolidinone (NMP).  A second structure was fabricated that allows the  application of voltage between two layers of Ti.


Figure 2:  Scanning electron micrograph of  a topography sample.  The step height was  generated by etching about 160 nm of the  Ti layer.  The field of view is roughly 1.2 µm.


After depositing 0.5 µm of Ti, a layer of SiO2


whose thickness depended on the total height


desired was grown using an electron beam


evaporator.  Subsequently, a second layer of 100  nm of Ti was deposited on top of the dielectric


layer.  The topography was then generated using  the procedure outlined above.  Once the exposed  area of the upper Ti layer was completely etched, the oxide layer was etched using an rf plasma of  trifluoromethane and oxygen.  Obviously, we


refer to this sample as Ti/SiO2/Ti.  Sample height  and profile were verified using profilometry and  scanning electron microscopy.  Prior to PEEM


imaging, the samples were Ar-sputter cleaned.


Theoretical


In order to model doping-induced contrast, it is  necessary to understand the variation in  photoyield as a function of doping concentration.  Thus, we considered near-threshold  photoemission from the valence band for indirect  optical transitions.3  The photoyield Y from the  valence band can be expressed as


where hν is the incident photon energy and  ET(x,n) is the photothreshold as a function of  depth x and doping concentration n.  The  constant CN depends on the incident photon flux  and the excitation cross section.  The reduced  electron escape depth l (18 Å) is given by 1/l =


1/lα + 1/le, where lα (~ 60 Å) is the absorption  length and le (~ 25 Å) is the electron escape  depth.


To determine the depth dependence of the  photothreshold, we solved Poisson’s equation in  the space charge region to find the valence band  profile ∆E(x).  The valence band profile is  implicitly dependent on the doping  concentration, and the density and distribution of  surface states.  For a lightly doped  semiconductor the bands are flat, whereas the  band curvature increases as the doping level  increases.  Therefore, the photothreshold  decreases with bulk depth.


Another effect of increased doping concentration  is the broadening of the impurity states near the  band edge.  For sufficiently high concentrations, the states merge with the continuous band  resulting in a reduction of the band gap.  Since  we have imaged devices consisting of heavily


doped silicon, it is necessary to use the reduced  band gap in determining ET as a function of  doping concentration.  From Wagner’s published  data,4 the band gap for boron-doped silicon is  reduced by approximately 50 and 160 meV for  1018 and 1020 cm-3, respectively.


To make a quantitative comparison of the  observed photoyield with that expected for  electron excitation from the valence band, the  photoyield Y was calculated for a given photon  energy, doping level and surface state  concentration.  Comparing the photoyield for  each doping concentration of interest allowed us  to quantify the resulting contrast.


Numerical Modeling


If topography is present on a sample, the local  accelerating field can be perturbed enough so  that PEEM imaging conditions are modified.  In  the simplest case, the perturbations are small  enough that the effects are negligible.  However, if the lateral component of the perturbed  accelerating field is large enough, electrons  originating from a single point on the surface  will not re-unite to a single point in the imaging  plane.  As a consequence, image contrast will  arise.


To characterize this type of contrast, we have  constructed numerical models of several types of  topography.  The numerical modeling is done  with commercial software (CPO-3D).5  The  program uses the surface charge method6 to find  electrostatic potentials and fields.  In this  approach, a system of linear equations is used to  solve for the local electric field strength rather  than a system of partial differential equations.  Also, the surface of the test electrodes is divided  into segments.  To properly model topography, it  is important that the density of segments near the  step edge is greater than the density of segments  far from the step edge.  Typically, a segment is  10 nm in length near the edge whereas a segment  is 50 nm far from the edge.  Thus, a step that is  20 µm wide consists of 740 segments.  This  allowed us to accurately determine the local  lateral field strength in the vicinity of a step  edge, and thus characterize topography-induced  contrast in PEEM.


,


)]


[


dx


e


x


E


h


l


T


∫


ν


We first consider contrast that arises from  doping.  In Figure 3, we show a PEEM image of


150 Photoyield (a.u.)50


4.BeV n5.2eV


a lateral array of pn junctions illustrating dopinginduced contrast.  The bright horizontal lines are  nominally p-type 1020 cm-3 FIB lines, while the  dimmer vertical p-type lines (produced with  broad beam implantation) are nominally 1018 cm3.  Using a near-threshold light source, we find  that the photoyield from the p-stripes increases  monotonically as the amount of doping is  increased.  The average ratio of the peak  intensity profile for the 120 keV FIB implants is


6.3:2.5:1.0 for nominal 1020:1019:1018 p-type  doping, respectively.  The results for the six  different FIB doping levels are summarized in  Table 1 (see ref. 7 for details).


Table 1: Nominal implant value, corresponding  value of doping at surface (calculated with  SUPREM-IV8), intensities normalized to lowest


|Nominal Doping |||
|---|---|---|

||Doping at Surface|I|

|1x1020|2x1020|/Imin|

|6x1019|3x1019|12|

|1x1019|7x1018|6.3|

|||18 |

|6x10 |6x10 |8x1017 |

|1x1018|1x1018|1x1017 |

doping level.


To further characterize the contrast seen in  Figure 3, we also acquired images of the  different doping concentrations with a variable  photon energy source (FEL).  As mentioned


previously, the photon energies were varied from


The Ti/SiO2/Ti structure was modeled  numerically using two electrodes separated by a  distance that corresponds to the thickness of the  SiO2 layer.  This simplification is necessary  because the surface charge method is not  applicable to dielectric material.  A 20 µm wide  step was segmented 580 times in order to model  the upper Ti line.  The thickness of the step (100  nm) was taken into account by using 20  segments with a total length of 100 nm.  The  bottom Ti layer of the device was represented by  1000 segments that have a total length of 2.5  mm.  Again, we note that the density of line  segments was increased near an edge.  As  expected, the model predicts that the lateral field  strength increases linearly as the bias voltage  between the Ti layers increases.  In addition, the  simulated device predicts that the bias voltage  necessary to minimize the edge effect is a  function of height.  Simulations show that the  radial field strength is balanced at 0.5 V for 200  nm, 1.0 V for 400 nm, and 1.5 V for 600 nm.


Therefore, the bias voltage necessary to  minimize the edge contrast increases roughly 2.5  mV per nanometer in step height.


Discussion


The contrast observed between different  concentrations of boron-implanted regions in our  pn junction array comes about because the  photothreshold is dependent on the amount of  doping.  In agreement with earlier work,9 we find  that the photothreshold decreases as the doping  level increases.  Thus, doping-induce contrast is  generated because the intensity from heavy  doped Si (>1017 cm-3) is greater than from lightly  doped Si.  By making PEEM intensity  measurements relative to a known reference  sample, the ratio of intensities should provide a  robust measure of the dopant concentration at  high levels.  Although we have only presented  data from p-type doping, doping-induced  contrast will also occur in heavily doped n-type  Si.


However, when the energy of the incident light is  varied, we observe intensity from the heavily  doped regions at energies below the nominal  photothreshold of Si (5.15 eV).  When imaging  heavily doped Si, the effects of impurity band  tailing must be included. At degenerate doping  levels, the impurity states near the band edge  merge with the continuous band and this results  in reduction of the band gap.  The reduction in  band gap, and therefore the photothreshold, helps  to explain our observation of sub-threshold  intensity from our B-doped lines.  Yet, the  intensity from the implanted regions decreases as  the energy of the incident light is lowered toward  a particular photothreshold. Consequently, optimum doping-induced contrast and thus  PEEM sensitivity is achieved by imaging with a  photon energy slightly above the highest  threshold of interest.  This will produce a  sufficient signal to noise ratio for imaging the  lowest doping level of interest.  Conversely, the  visibility of boron implanted regions can be  removed by imaging with a photon energy less  than its effective photothreshold.


Doping-induced contrast is well described with a  photoemission model that takes into account the  density and distribution of surface states.  Ideally, this allows us to take into account the  condition of the surface of the device when  imaging.  We refer the reader to an earlier paper


Figure 6:  PEEM image of a pair of 32 µm wide structures illustrating edge- and  volage-induced contrast.  A)  When no  bias voltage is applied only edge contrast  is present.  B)  When 10 V is applied  between the line pair, the edge contrast is  dramatically effected.  The field of view  is ~100 µm for both images.


A)


B)


where the effect of various surface state  distributions on doping-induced contrast was  studied.1  If the device surface is modeled with  either a continuous or discrete distribution of  states, we find that approximately 5x1013 cm-2  surface states are necessary for the calculated  PEEM intensities to increase monotonically with  doping concentration, in agreement with  experiment.  Consequently, this tells us that the  imaging technique is quite robust.  Thus, only  minimal sample preparation such as standard  degreasing procedures is necessary for the  sample to produce doping-induced contrast.   We  mention in passing that the photoemission model  used here is general enough to model and predict  doping-induced contrast in PEEM of other  semiconductors.


When imaging real devices with PEEM, topography-induced contrast is invariably  present.  However, it is not always possible to  distinguish this particular contrast mechanism  from others during image analysis.  By imaging  well-defined topography on simple structures, topography contrast can be characterized.  Not  surprisingly, our initial results indicate that the  lateral electrostatic field is equal in magnitude to  the perpendicular accelerating field strength.  Therefore, the perturbation of the local electric  field strength at a step edge is sufficient to  prevent Gaussian imaging conditions from  occurring.


Yet, the observation that systematically varying  the lateral field strength directly affects edge  contrast is interesting.  By applying a voltage to  the step, the topography-induced perturbation to  the local field strength can be varied, and thus  controlled.  This result could be useful in solving  several practical problems.  For example, the  height of the structure could be determined by  finding the bias voltage necessary to minimize  the edge effect.  However, a more  technologically interesting example would be to  use this contrast mechanism to identify breaks in  metal lines.  Implementation of this technique  would require identifying metal lines where no  changes in edge contrast occurs as the probe  voltage is varied.  Thus, this technique is  analogous to the voltage contrast (VC) technique  used in SEM of micro-circuits.  Here, only the  contrast at the edge of the biased structure is  modified whereas the whole structure in the VC  technique is affected when a bias voltage is  applied.  To utilize this result more work needs


to be done, however.  Further studies include  characterizing the lateral extent of the edge effect  between adjacent line pairs as a function of bias  voltage, and determining if the effect can be  observed when the metal line is buried under an  oxide.


Conclusion and Summary


In summary, the results from both experimental  and theoretical studies have been used together  to investigate how information may be extracted  from PEEM images of device samples.  Consequently, several types of contrast that  occur in PEEM have been identified as relevant  to device characterization.  In particular, dopinginduced contrast and topography-induced  contrast are two types of contrast that are  applicable to analysis of integrated circuits.


We find that PEEM intensity increases at a rate  of approximately a factor of 2 per decade  increase in B doping concentration from 1017 to  2x1020 cm-3.  Thus, contrast between different  doping levels is generated.  This type of contrast  is optimized by imaging with photon energy  slightly above the highest photothreshold of  interest.  Doping-induced contrast can be well  described with a simple photoemission model  that includes the effects of impurity band tailing  and surface state associated band bending.  This  model also suggests that doping-induced contrast  is robust if the density of surface states is  sufficient (>5x1013 cm-2).


The presence of sample topography leads to  perturbations in the local electric field that  generate PEEM contrast.  Numerical simulations  show that a lateral electric field that is  approximately equal in magnitude to the  perpendicular electric field is the source of edge  contrast.  Imaging well-defined structures reveals  that topography contrast can be characterized.  By intentionally varying the lateral field near a  step edge, we find that topography contrast can  be generated and controlled.


Thus, doping-induced contrast and topographyinduced contrast give PEEM unique properties  that can be applicable to analysis of  microelectronics.  For example, the large field of  view characteristic of PEEM could be used to  rapidly distinguish between doping  concentrations of the diffusion layer.  Since the  image is formed without an external source of


electrons, there are no concerns about beam  radiation damage inherent to other electron  microscopies.  Furthermore, the essentially nondestructive character of PEEM suggests that it  would be a reasonable tool for in-line inspection  during IC processing.  The capability of imaging  intentional changes in the edge contrast of metal  lines could also make PEEM useful in failure  analysis of integrated circuits.  Thus, PEEM  could serve as a complementary tool to SEM, as  well as be a stand alone tool, for device  characterization.


The authors would like to thank Stacy Mogren at  the Microelectronics Lab in Columbia, Maryland, Professor Robert J. Nemanich at  North Carolina State University, Mihaela Breban  and John Barry at the University of Maryland, and Toby Olver at the Laboratory for Physical  Sciences.


1)  V.W. Ballarotto, K. Siegrist, R.J. Phaneuf, and E.D. Williams, J. Appl. Phys., 91, 469-475 (2002).


2)  G.F. Rempfer and O.H. Griffith, Ultramicro., 47, 35-54 (1992).


3)  E.O. Kane, Phys. Rev., 127, 131 (1962).


4)  J. Wagner, Phys. Rev. B, 29, 2002 (1984).


5)  CPO-3D is a simulation package from RBC, Ltd., Dept. of Physics. and Astronomy, University of Manchester, UK.


6)  E. Harting and F. Read, Electrostatic Lenses, Elsevier, 1976.


7)  V.W. Ballarotto, K. Siegrist, R.J. Phaneuf, E.D. Williams, and S. Mogren, Surface Science, 461, L570 (2000).


8) Computer code SUPREM-IV, Stanford  University, Palo Alto, CA.  Calculates 1- and 2-D implant profiles with pre- and post-annealing  simulations.


9)  F.G. Allen and G.W. Gobeli, Phys. Rev., 127, 150 (1962).


Application of Acoustic Fourier Domain Imaging for the Evaluation of  Advanced Micro Electronic Packages


Janet E. Semmens and Lawrence W. Kessler


Sonoscan, Inc.


2149 E. Pratt Boulevard


Elk Grove Village, IL   60007   USA  Phone: (847) 437-6400


Fax: (847) 437-1550


E-mail: Jsemmens@sonoscan.com


Acoustic Micro Imaging (AMI) has been used for  years to evaluate microelectronic packages for the  presence of internal defects. The drive in micro  electronic packaging is to reduce the size of the  components as much as possible to keep pace with  the shrinking size of the end products. This leads to  smaller/thinner packages with internal features and  possibly defects that are approaching the resolution  limits for conventional AMI. Recently AMI has been  combined with Fourier transforms of the acoustic  signal to produce frequency domain images. Previously features that were at or below the  accepted resolution limits for a given frequency were  not detected in the time domain images, however  these features are revealed in the frequency domain  images.


Acoustic Micro Imaging (AMI) has long been  established as a method of evaluating materials and  bonding for various micro electronic applications [1, 2]. Acoustic micro imaging uses high frequency  ultrasound (5 to 300 MHz) to image the internal  features of samples. Ultrasound is sensitive to  variations in the elastic properties of materials and is  particularly sensitive to locating air gaps (delaminations and voids). The method of imaging  most commonly used at present involves time gating  of a selected echo or echoes on an A-scan, which is a  single point depth profile through the sample, to  select a specific depth in the sample for  display/analysis. This is known as time domain  imaging. There is a direct relationship between  frequency and resolution in AMI. The higher the  frequency the shorter the wavelength and  the higher  the resolution potential. With the evolution of  microelectronic devices to smaller sizes and/or higher  I/O counts the sizes of the features have become  increasingly smaller and layer thicknesses  increasingly thinner. This has pushed the  development of higher frequency imaging in AMI to  increase the available resolution in both the spatial (x-y) and axial (z) dimensions. However, there is a


point at which further methods are needed to extract  additional information beyond what can be done by  standard time domain (C-Scan) acoustic imaging.


In the past, studies have been done in AMI using  Fourier analysis of echo waveform distortions to  measure minute thickness variations in materials [3]. More recently imaging in the frequency domain has  been used to enhance features and bring out  information previously unavailable when using time  domain AMI. In the work done for this study the  method involves mathematically converting the  captured waveforms within a time gate to the  frequency domain. Specific frequencies are selected  from the Fast Fourier Transform (FFT) spectra and  an image is then reconstructed from the frequency  information.


Our recent study shows that FFT frequency domain  imaging has been used to reveal features down to  only Angstroms in thickness, which is substantially  below the accepted wavelength limit of the  resolution, in applications such as wafer bonding and  flip chips.


A brief discussion of Acoustic Micro Imaging (AMI) techniques and the Fourier imaging method with  example applications follow.


Acoustic Micro Imaging


A-Scan


In reflection mode Acoustic Micro Imaging the  fundamental information is contained in what is  called the A-Scan.  The A-Scan displays the echo  depth information in the sample at each x, y  coordinate. Echoes displayed in the A-Scan  correspond to different interfaces in the device being  examined. There is a time - distance relationship  between the echoes related to their depth in the  device and the ultrasonic velocity in the materials.  The amplitude and phase (polarity) information of the  echoes is used to characterize the condition at the  interface and is dependant on the acoustic impedance  value of the materials involved. The equation that


describes the pulse reflection at an interface between  materials is as follows:


Z2 - Z1


R  =  I  --------


Z2 + Z1


Where R is the amplitude of the reflected pulse, I is  the amplitude of the incident pulse, Z1 is the intrinsic  acoustic impedance of the material through which the  pulse is traveling and Z2 is that of the next material  which is encountered by the pulse.


Interface Scan - C-Scan


The “interface scan” is the most common imaging  method used to evaluate devices for voids and  delaminations between layers.  This method involves  gating the A-Scan signal for the appropriate echo  from the interface to be investigated. The gate  corresponds to a time window that that is selected  and applied to each x-y position for the scan. The  geometric focus of the acoustic beam is optimized for  the interface as well. At each x-y position only the  peak intensity value and the polarity of the echo  within the gate are displayed.


The conventional C-scan output is only twodimensional consisting of an x-y plot of one specific  plane in the z dimension. Features existing in the  device but not included in the electronic gate or  features with lesser signal strength at a given position  will not be displayed for analysis in the image. The  A-scans for each point on the sample are not typically  saved with the images due to file size considerations


ns


when documenting a significant number of samples. Since the A-scans are not saved, the data cannot be  re-gated, nor can the echoes be reprocessed to create  different image information. But the conventional CScan is very useful and has been the standard since  acoustic micro imaging was developed.


A-scan Storage


More recently a method is used that stores the A-scan  information for each x-y point in a scan. From the  stored information images of depths within the device  not included in the original gate for the image can be  recreated and/or waveforms (echoes) can be viewed  for analysis without rescanning the sample. In  addition to this the echoes can be digitally processed, frequency filtered, etc., to extract further information  about the condition of the sample, or extract  information at or slightly beyond the limits of  conventional AMI.


Frequency Domain imaging


Frequency Domain imaging is one method that can  extract further information by using the frequency  content of the signal.


The transducers used in AMI range in center  frequency from 5 MHz to 300 MHz and above. In  conventional acoustic imaging, the choice of  transducer determines the spatial resolution, penetration, and other parameters. These transducers  typically have highly damped waveforms in order to  achieve better resolution, both spatial and axial, using  time domain imaging. Figure 1 displays an A-scan  with typical echoes (pulses) as seen in the time  domain. However these highly damped waveforms  contain broad-spectrum frequency information which  can be displayed in the Fourier (frequency) domain. When using time domain imaging at a center  frequency of 50 MHz, one can not manipulate the  image data to produce a 10 MHz image or a 100  MHz image, because in the time domain the acoustic  pulses themselves do not have sufficiently wide  frequency content. However, the data file including  the stored A-scans makes this kind of manipulation  possible, within limits. Data collected at a center  frequency of 50 MHz can be used to create images  showing the sample at frequencies from 30 MHz to  70 MHz, and data collected at 300 MHz can be used  to create images showing the sample at frequencies  from 225 MHz to 375 MHz using frequency domain  imaging. But much larger excursions in frequency – for example, using a data file collected at 10 MHz to  create 300 MHz C-Mode images – are not possible. The sample can of course be physically scanned with  a variety of transducers.


||0|0|100|100|
|---|---|---|---|---|

Figure 1: A-scan displaying typical waveforms (pulses) in the time domain.


Because the A-scans for each point in the image are  collected with the image  changes in frequency that  may occur during reflection can be analyzed. For  example, a pulse of 15 MHz ultrasound launched  toward a material interface (such as molding  compound to die) may be reflected with a different  frequency content than originally pulsed, and this  change – not otherwise detectable – may be  indicative of the interface condition. The gated  echo(es) from the stored A-scans can be filtered by  means of a Fast Fourier Transform (FFT), also called  a Frequency Domain algorithm, to isolate a given  frequency. The Fourier transform decomposes the  selected waveform(s) into sinusoids of different  frequencies. An illustration of a broadband pulse with


corresponding component frequency sinusoids is  shown in figure 2.


Figure 2: sinusoids of single frequencies combine  constructively/destructively to form a single  broadband waveform.


The FFT identifies the different frequency sinusoids  and their respective amplitudes. Figure 3 shows the  frequency content distribution of the gated echo  shown in Figure 1 in the frequency domain. Images  can then be reconstructed from components of the  frequency information. Specific features may yield  more information at one frequency than another; therefore, FFT filtering of the echo can bring out  image detail that may not be visible with  conventional time domain imaging.


Figure 3: Broadband pulse content in the frequency


domain for the echo shown within the gate on the Ascan in Figure 1.


The following examples demonstrate instances where  the frequency domain imaging has been able to bring  out features that were either not clear or not  detectable in the time domain images.


Applications


Plastic Encapsulated Packages


In the following example a TQFP plastic  encapsulated package is shown using time domain  imaging and frequency domain imaging. Using time  domain imaging the most significant echo over the  duration of the gate is displayed for any given point. The various levels in the package can be seen such as  the die surface, die pad surrounding the die and the  lead frame. A delamination at the die pad can be seen  as a red region (dark grey in the black and white print  of the color image), the red color indicating the area  of inverted polarity. Information below the die (die  attach) is not evident in this image as the die surface  and die attach echo compete within the gate at the  same x-y position for display to the image. The die  surface echo in this case shows the stronger signal  and is the one displayed. The frequency domain  image (Figure 4b) of the same gated area however  brings out the detail not present in the time domain  image. A delamination at the die attach interface now  can be seen which is continuous with the die pad  delamination and the dimple pattern of the die pad  becomes visible.


From this example it can be seen that the detection of  features such as delaminations of the internal  interfaces is easier from the time domain image as the  polarity inversion is clearly displayed using color  mapping. It should also be noted that the die attach  delamination can be readily imaged in the time  domain by changing the gate for the image. And, using A-scan storage the new image can be generated  instantaneously without rescanning the part. But this  example demonstrates how additional features can be  brought out using frequency domain imaging to  insure that no details of the condition of the device  are overlooked


Figure 4a: TQFP time domain image


Figure 4b: TQFP frequency domain image


Figure 5a: Time domain image of silicon wafer


Figure 5b: FFT single frequency image of silicon  wafer.


Silicon Wafers


Figures 5a and 5b reveal an issue of detecting polysilicon dioxide layers on a silicon wafer. The wafer


shown here was the remaining part of a  silicon/silicon bonded wafer where the other wafer  had been removed. The purpose was to detect the  presence/absence of the poly-silicon dioxide layers  remaining at the bond interface and to determine if  this had any relationship to the presence of voids in  the bond. The appearance of the wafer in the time  domain image (5a) shows very faint evidence of the  presence of the poly-SiO2 layers in the lower left  quadrant of the image. The frequency domain (FFT) image enhances the appearance of the poly-SiO2  layers. The reported thickness of these layers is only  2 to 150 Angstroms.


Flip Chip


Advancements have been made in recent years with  respect to higher resolution in the acoustic images by  increasing the frequency/design of the transducers


[4]. However there is a point where the thickness and  type of material in the packaging will limit the use of  even higher frequency ultrasound even though  package features are becoming increasingly smaller  and internal layers increasingly thinner. Frequency  domain (FFT) analysis of the waveforms has been  used in the past to measure bondline thickness and  has shown the capacity of measuring to thickness  well beyond the axial resolution limit of a given  frequency. Frequency domain imaging can be used to  improve detection/resolution in the lateral dimensions  by removing the low frequency component from the  image.  Figure 6a shows the time domain image of a  flip chip at the chip/bump interface. The bump bonds  can be seen as well as associated laminar cracks next  to some of the bumps. The evidence of the  metallization on the chip is very faintly visible in  some areas. The frequency domain image using the  higher frequency portion of the signal (Figure 6b) shows the metallization clearly.


4.5 to 5.2 eV in steps of 0.1 eV.  Figure 4 shows  an example of our results, consisting of intensity  scans across PEEM images of a pair of broadbeam implanted lines.  Once again, the intensity  increases monotonically as the photon energy  increases.  The variation in image intensity  observed for three different implantation  concentrations is summarized in Figure 5.  The  data were normalized to the calculated  photoyield for a dopant concentration Na = 1x1017 cm-3 and a photon energy of 5.2 eV. Both  the intensity and the contrast between the n and p  regions drop with decreasing photon energy.   However, contrast between p-type lines and ntype substrate is observed for photon energies  well below the nominal photothreshold of 5.1  eV, suggested by Allen and Gobeli.9  In  particular, the contrast between the p-stripes and  the n-doped substrate is observable down to 4.9  eV for the 1017 cm-3 stripe, 4.7 eV for the 1018  cm-3 stripe, and 4.5 eV for the 3x1019 cm-3 stripe.  We note that channel plate saturation may have  reduced the measured intensities for 1018 and  3x1019 cm-3 at 5.2 eV.


These results, in which we tune the photon  energy, demonstrate that the effect of impurity  band tails as well as band bending must be  considered to correctly describe doping-induced  contrast.  The lines plotted with the data points in  Figure 5 show the calculated photoyield  expected from the p-type regions as a function  hν.  Here, the total calculated photoyield was  obtained by integrating Y(hν) over a distribution


Doping at Surface I/Imin


6x1020


2x1020


12


1x1020


3x1019


6.3


6x1019


7x1018


1x1019


1x10


18


1x1018


Figure 3:  PEEM image of lateral array of


pn junctions illustrating doping-induced  contrast.  The field of view is ~40 µm.


010020C90040C500600700


Figure 4:  PEEM intensity line scans of


photolithography lines measured at different  values of incident photon energy.  Inset:  The  vertical lines are p-type (3x1019 cm-3) FIB  lines.  The horizontal lines are p-type (1018 cm-3) photolithography lines.


function of photon energies that characterized  the FEL light source.  This weighting function  was a Gaussian distribution of photon energies  centered about the desired photon energy with a  full width at half maximum of 0.13 eV.  In this  case, a continuous (parabolic) areal surface state  density of 5x1013 cm-2 was used to describe a  native oxide-covered Si surface.  The best  agreement of the calculated intensity variation  with the data in Figure 5 was obtained for a  surface photothreshold, ET(x>0), greater than  predicted by Wagner.4  Using a nominal surface  photothreshold of 4.9 eV, we find that band gap  reduction of 25 meV and 40 meV produce good  agreement with our 1018 and 3x1019 cm-3 data, respectively.  We did not implement gap  reduction for the 1017 cm-3 case since none is  expected.


To calculate the intensities, we considered both  continuous and discrete surface state  distributions to describe the condition of the  sample surface.  In general, both types of surface  state distributions give consistent results for  doping-induced contrast as long as a sufficient  number of surface states are present.  In  particular, if the density of surface states is  greater than approximately 5x1013 cm-2, then  varying the position, uniformity and density of  the surface states does not affect doping-induced  contrast.  However, if the number of surface  states is too small, the calculated intensities will  not increase monotonically as the doping level is  increased.  Thus, the model puts a lower bound  on the density of surface states necessary to


describe the measured doping-induced contrast  observed in Si(001).


The effect of topography on PEEM contrast is  now considered.  Several Ti structures with steps  of 75, 150, 290, and 550 nm were imaged and  then line scans across the steps were acquired.  Analysis of the image data indicates that the  minimum intensity associated with the step edge  decreases linearly as the step size increases.  Consequently, the edge contrast increases as the  Ti step height increases.  However, image  analysis reveals that the width of the edge  contrast does not increase consistently as the step  height increases.


To model edge contrast, step heights of 70, 150  and 300 nm were evaluated numerically.  In all  cases, a 20 µm wide step was represented by 740  grounded segments and the anode lens (2.5 mm  wide) was represented by 1000 segments held at  3 kV one millimeter away.  This segmentation  produces a lateral field strength of 3 kV/mm in  the vicinity of the step edge which is equal in  magnitude to the perpendicular accelerating field  strength.  As the step height increases, the  calculated magnitude of the lateral field strength  stays the same but the lateral extent of the  perturbation increases.  This suggests that PEEM  edge contrast should increase in magnitude and  in lateral extent as the sample step height  increases.


Since the lateral field strength affects imaging, we also investigated the effect of systematically  varying the lateral field strength.  In Figure 6, we  show PEEM images of the Ti/SiO2/Si sample  where the bias voltage can be applied between  two adjacent Ti lines.  The pair of 32 µm wide Ti  lines is separated by 2 µm.  The line on the left is  grounded.  In Figure 6A, the bias voltage  between the line pair is zero.  The only contrast  present is strictly due to the edge effect of each  line.  However, in Figure 6B, the bias voltage is  10 V.  The edge contrast on the right line has  been dramatically increased.  The same effect is  also seen if the polarity of the bias voltage is  reversed.  Furthermore, the lateral width of the  edge-contrast increases linearly as the bias  voltage is increased from 0 to ±10 V.  Qualitatively, we observe that the bias voltage  necessary to minimize the edge effect increases  as the height of the structure increases.  This  effect provides a method for determining the


Figure 5:  Photoyield intensity as a function  of photon energy.  The symbols are  measured values of PEEM intensity  normalized to obtain agreement between  measurement and calculation at 5.2 eV and  1017 cm-3.  The curves show calculated


intensity (x10) from the valence band of Si.


thickness of the dielectric layer between the two  metal layers.


Figure 6a: Time domain image of flip chip. The  arrows point out examples of the laminar cracks  associated with the bump sites.


Figure 6b: frequency domain image of flip chip. The  arrows point out examples of the laminar cracks  associated with the bump sites.


Small Void Detection


Voids in underfill can reduce the field life of the  device particularly when the voids are in close  association to the interconnect bumps. Halo voids  that surround the bump totally or partially at the  chip/bump level typically result from flux residue or  other contamination on the chip surface.


Figure 7a displays a time domain image of a flip chip  that shows halo voids associated with two of the  bump bond sites. Figure 7b shows the corresponding  frequency domain image. The image was made again  using the higher frequency content of the pulse. In  the FFT enhanced image many other halo voids  become apparent.


Figure 7a: Time domain image of flip chip with halo  voids in the underfill.


Figure 7b: Frequency domain image of flip chip. Now many more bumps show associated halo voids.


SUMMARY


The examples presented here demonstrate only some  of the instances where imaging in the frequency  domain has been useful. The drive to manufacture  smaller and thinner microelectronic devices and  features in the devices is pushing the limits of the  inspection technologies to resolve/detect these  features. Frequency domain imaging is one tool that  can be used with AMI to evaluate advanced  microelectronic packages.


REFERENCES


[1] L.W. Kessler, “Acoustic Microscopy” in Metals  Handbook, Ninth Edition, Vol. 17 - Nondestructive  Evaluation and Quality Control  - ASM International, Materials Park, OH, 1989, pp. 465-482.


[2] J. E. Semmens, and L.W. Kessler, “Application  Of Acoustic Micro Imaging For The Evaluation Of  Advanced Microelectronic Packaging:  An Overview  Of Experiences From 1973 – 1996”, Proceedings of  ISEPT ’96 conference, Shanghai, China 1996.


[3] Sridhar Canumalla and Bryan P. Schackmuth, “Metrology of Thin Layers in IC Packages using an  Acoustic Microprobe: Bondline Thickness”, Proceedings of the 49th Electronic Components and  Technology Conference (ECTC), San Diego, CA, June 1-4, 1999.


[4] J.E. Semmens, “Flip Chips and Acoustic Micro  Imaging: An Overview of Past Applications, Present  Status, And Roadmap for the Future”, Proceedings of  ESREF conference, Dresden, Germany, Oct. 2000.


Petar Ratchev, Laureen Carbonell, Hong Meng Ho, Hugo Bender and Ingrid De Wolf


IMECvzw, Leuven, Belgium


Bert Verlinden


Katholieke Universiteit Leuven, Belgium


In this paper we described a technique which is not commonly used for failure analysis: Orientation Imaging Microscopy (OIM). We demonstrated that it offers unique opportunity for failure analysis of Cu bonding and interconnects. Additionally to its main application: texture analysis, it can also reveal early stages of oxidation of Cu bond pads and interconnects. A link has been made between oxidation and bondability. OIM can also show areas of the wire bond where the deformation concentrates due to the bonding process.


The need to increase the integrated circuit performance and reduce electromigration effects has led to the implementation of Cu in place of Al as the interconnect material. Unfortunately, Cu readily oxidizes in air or in a humid ambient, which is a serious technological challenge,not only for interconnects but also for the bonding to Cu.


Data Acquisttlon


Faxtonsomple


OIM is a powerful method for microstructure and texture


&. Processing


characterization [1]. It has recently been employed with success in studies of Cu interconnects [2]. The reliability of


CEmbe


Cu interconnects is a function of many factors such as alloy


D00=Low LghtCamela


。


chemistry (which depends on the electroplating bath), film thickness, barrier layer etc. Among them grain size distribution and crystallographic texture are very important.


RcngCxmara ContoPhosphor Screen


These were studied mainly by OIM [2].


The aim of this work is to show that OIM offers unique opportunity for failure analysis of Cu interconnects and of Cu to Cu wire bonds. Additionally to classical microstructure and texture studies, it is used here to reveal early stages of oxidation of Cu bond pads and to observe and characterize cross sections of Cu-Cu wire bonds.


OIM


A scheme, illustrating the principle of the OIM measurement, is given in Figure 1. OIM is actually a fully automated Electron Back-Scattered Diffraction (EBSD)technique. During the measurement, an electron beam scans the sample in a standard Scanning Electron Microscope(SEM). At each point, a unique back-scattered Kikuchi pattern is produced and collected by a low-light camera towards which the sample is tilted. This pattern, after being indexed, determines the crystallographic orientation at each point. The beam motion and image processing is fully computer-controlled. The collected data processed with specifically designed software packages, can be presented in different ways, for instance as microstructure and texture maps, histograms, pole figures, Orientation Distribution Functions etc.


Figure 1: Principle of OIM measurement


The OIM measurements were performed on a Philips XL-30 SEM equipped with the standard TSL (Tex-Scan Ltd.)hardware and software package. Usually scans of 50x50 µm


Proceedings from the 28t International Symposium for Testing and Failure Analysis, 3-7 November,2002, Phoenix, Arizona


CopyrightC 2002 ASM International®


were performed with a step of 0.2 µm, which gave a spatial resolution of about 0.5 µm. The measured textures are presented in volume fractions of the major directions,


<111>, <100> and <110>, parallel to the surface normal(the so called “fibre” textures). A tolerance angle of 15º around the surface normal was used. Thin lines were drawn on OIM maps to indicate high-angle grain boundaries(>15º). The following color code is used in OIM maps:


<111> texture in blue, <100> in red and <110> in green.


EBSD patterns are very sensitive to surface oxidation,contamination or high plastic deformations. Such regions simply give very poor patterns, which are wrongly indexed.


These patterns can be filtered out based on the so-called confidence index (CI), which is a measure of the certainty in the pattern indexing. Work at TSL, Inc. [3] has shown that patterns with CI > 0.1 are generally correctly indexed, while the uncertainty drastically increases for lower CI. Therefore,if OIM maps are cleared for points with CI < 0.1; the black areas which appear indicate possibly oxidized regions. This technique was used to detect early oxidation on Cu bond pads and interconnects. EBSD patterns are also very sensitive to local plastic deformations. A locally increased dislocation density results in a pattern loss, such as grain boundaries or highly deformed regions. The latter was used to locate areas of high deformation on a cross-section of a Cu to Cu wire bond.


Samples


Single damascene trenches were used in this study. The processing first involved patterning of 650 nm deep trenches in the dielectric stack (600 nm SiO2 / 50 nm SiC). After patterning, a 25 nm Ta(N) metallic barrier layer and a 150 nm Cu seed layer were deposited using Ionized Physical Vapor Deposition (I-PVD). Gap-filling was achieved by electroplating a 1000 nm thick copper layer, followed by an anneal in a pure N2 ambient at 200°C for 30s. Finally, the excess of copper and barrier was removed by a two-step CMP process. The dry oxidation of copper was investigated by annealing wafers in a RTP system at 420°C for 20min in N2 ambient with oxygen concentrations ranging from 0 to 250 ppm.


The wire bonding process was performed using the ASM AB339 wire bonder. The whole assemble module (single die attached to leadframe) was placed under a heating stage at a temperature of 145°C. The Cu wire bonding process starts off with the free air ball formed at the end of the wire,which is protruding outside the capillary. The Electronic Flame-Off (EFO) system melted the tail of the wire to form the Cu ball within a pocket of inert gas (5%H2+95%N2) to prevent oxidation of the Cu ball surface. The capillary then presses the Cu free air ball against the Cu bond pad on the die so that the shape of a ball bond is formed. A ball bond with metal-to-metal weld in-between the Cu wire and Cu bond pad was formed under the combination of transducer’s


ultrasonic energy, force pressure, scrubbing action of the capillary tip and hold down time.


Results and Discussion


Sample preparation for OIM


Sample preparation for OIM is not always trivial. The main requirement is that the sample should be able to produce diffraction patterns that can be acquired and processed by the software. Therefore the surface must be free from oxide layers and contamination. All deformed layers (due to polishing for instance) should be thoroughly removed. The Cu bond pads and interconnect lines do not need a special preparation. The standard deposition techniques and clean room storage conditions suffice. On the contrary, getting a diffraction pattern of decent quality from a wire bond crosssection is not an easy task. Very precise grinding and polishing (including a final step with colloidal silica) is necessary but not sufficient. The problem is the high reactivity of the Cu surface. At the end of the polishing job an oxide layer has been formed, which hinders the diffraction pattern. The electropolishing method, which gives nice results on bulk samples, cannot be applied here due to conductivity difficulties. In order to solve this problem, a Focussed Ion Beam (FIB) instrument, FEI-200,was used for a final cleaning of the polished surface. A conductive Au layer was sputtered on the polished sample,which consists of the wire bond embedded in an epoxy matrix. In this way, conductive contact was assured during the ion milling so that charging could be fully avoided. The cleaning is done with the polished face parallel with the incident beam and performing a line-by-line cleaning as usually applied for the cleaning of FIB milled structures for cross-sectional imaging. A relative high beam current (1000 pA) is used to be able to clean the large polished surface in an acceptable time. The surface quality of the sample is controlled in the FIB by means of the quality of the ion channeling image when tilting the sample over 45º. We have proved that if a channeling pattern of good quality is obtained, the surface quality is sufficient for a successful OIM scan. The developed preparation technique is nonconventional and offers the unique possibility to study cross sections of Cu-Cu wire bonds with OIM.


OIM study of Cu oxidation and bondability


In-house bond strength experiments on Cu wires bonded to Cu bond pads showed that the bond was good for one sample, while it was very weak for a second sample of the same lot. In order to study the cause of this difference, OIM was applied to the bond pads. Figure 2 shows the results of an OIM analysis on two Cu bond pads, one (Figure 2a)showed a good bonding during bond tests and one where the bonding failed (Figure 2b). According to the OIM map, the surface from the good sample (Figure 2a) is almost not


oxidized. On the other hand, the OIM image of the failed sample shows weak oxidation, as small as 15-20%, seen as black areas in Figure 2b. Both images are representative for 3 measurements taken in the middle of a bonding pad on similar locations of test chips. We are confident that this is oxidation and not contamination because, during the oxidation experiment, explained further, a microstructure was developed, which at later stages was identified as oxidations by means of SEM [4]. With even small level of oxidation, it could lead to a sharp deterioration of the Cu bondability. This makes bonding to a Cu die a very difficult task, for which bond pad cleanliness and minimum oxidation during wire bonding is crucial. A possible solution, which we recently reported, is applying an organic protective layer [5]. In this work was shown that if the Cu bond pad is coated with a Self-Assembled Monolayer film,the surface is well protected from oxidation.


boundary levels:15.0c


To study this oxidation further, experiments were performed on samples annealed 20 minutes at 420°C in N2/H2(10%)+125 and 250 ppm O2. They showed that OIM allows us to observe the early stages of oxidation. An oxidation as small as 5-10% is already detectable. As examples in Figures 3 and 4 the OIM maps are given of a bond pad and 5 µm lines oxidized in 125 ppm O2. Oxidation appears first on triple points and grain boundaries (see arrows). For interconnect lines, it begins often also at the sides of the lines. It was found that further oxidation is orientation dependent, i.e.


grains with <111> orientation oxidize faster than the ones with <100> orientation, as we have already reported [4]. In this work was suggested that impurities of the plated Cu migrate to the surface during annealing. One of them, S,segregates preferentially on <100> oriented grains,providing an oxidation protection and slowing down their oxidation rate compared to <111> oriented grains. A tendency also exists of increasing oxidability with decreasing the line width. This can be noticed comparing the OIM maps of the bond pad and of the 5 µm line (Figures 3 and 4). This will be an additional issue when decreasing the width of Cu interconnect lines. Summarizing, it was shown that the OIM technique gives the unique possibility of linking microstructure/texture with oxidability and bondability of Cu-surfaces.


a7.00μm-35 stepsTiled [001] IPF Map


b6.25 μm-25 steps Tiled [001] IPF Mapboundary levels:15.0


Figure 2: Early stages of oxidation of bonding pads,affecting the Cu-wire bondability; color code: <111> in blue, <100> in red and <110> in green. The black areas indicate the oxidized regions. a/ OIM map of a bondable surface (less than 5% oxidation); b/ OIM map of a nonbondable surface (15-20% oxidation: black areas).


Figure 3: OIM map of a Cu bond pad oxidized in 125 ppm


0.45


<111>


O2 . Color code: <111> in blue, <100> in red and <110> in


■<100>


green


S


u


00.35


。0.3


n0.25 0


A0.28 n


x0.15


0.1


0.05 0


Reference


Annealed


□<110>


Figure 4: OIM map of 5 µm Cu lines oxidized in 125 ppm


◆


0.250


0.3S


鹿皇


0.15


0.1A


Texture of Cu bond pad and interconnects


bonding


The main application of OIM is the study of texture. We


pad


Line width, micrometers


studied the Cu texture both on bond pads and on interconnects. It was observed that the texture of bonding pads after self-annealing (“reference” sample) is predominantly <111>, see Figure 5. A similar result was found for wide interconnects. It is recalled that this <111>texture, if predominant in interconnects, is beneficial for the electromigration performance [6]. Unfortunately, our measurements show that the texture in lines shows a randomization tendency, increasing with a decreasing line width, as is shown in Figure 6. Two of the texture components, <111> and <100>, decrease significantly their


contribution to the overall texture. This means that electromigration might not only be an issue in narrow lines due to the dimensions (higher current density) but also due to the difference in texture.


In addition, when this sample is annealed for 20 minutes at 420°C in a N2/H2 atmosphere, which simulates a treatment needed later during the processing, the <100>-fibre increases at the expense of the <111>-fibre (Figure 5). This is observed both on the bond pads and in interconnects. This process is governed by a grain growth mechanism, driven by strain energy minimization [7]. The anisotropy of the elastic constants of Cu makes the <100> grain orientation the most favorable from strain energy point of view. So, not only decreasing the width, but also a high temperature anneal will result in a decrease of the <111> texture, and might increase the susceptibility to electromigration.


boundary levels:15.0°


10.50 μm=50 steps Tiled [001] IPF Map


Figure 5: Effect of annealing on texture of Cu bonding pads.


◆<111>fibre


11.25 μm=45 stepsTiled [001] IPF Map


■<100>fibre


▲<110>fibre


0.35


Figure 6: Influence of the interconnect line width on the texture of Cu, as measured by OIM.


OIM of a wire bond cross-section


In Figure 7, an OIM scan is shown of a cross-section of a Cu to Cu wire bond for the first time. Although some preparation artifacts still exist (parallel lines due to steps


induced on the FIB cleaned face by the variable Cu height on the edges compared to the center of the wire bond,compare with Figure 8), some interesting tendencies were noticed. Two types of grain morphologies were observed:smaller, equiaxed grains in the wire and larger, elongated grains in the wire ball area. This type of grain morphology was observed also in Cu balls before bonding and it depends on the ball formation conditions. In Figure 9, an etched cross-section of such a “free air ball” is shown, formed at the same solidification conditions as the bonded ball in Figure 7. In Figure 7, it can be noticed that at the interface with the bond pad, there is an area (see the dashed lines triangle), where the EBSD signal deteriorates strongly and is partially filtered out according the CI >0.1 criterium.


High-angle boundary


Low-angle


boundary


Figure 7: OIM of a wire bond cross-section. A deformation concentration can be noticed (dashed line triangle). Thick lines are used for high angle grain boundaries (>15º) and thin lines- for low angle boundaries (<15º). The arrows point on the contamination visible in Figure 8. Color code:


<111> in blue, <100> in red and <110> in green


20 µm


Figure 8: FIB of the wire bond from Figure 7. The image is tilted at 45º about a horizontal axis. The arrows show surface contamination, which is probably generated during the ion milling.


boundary levels:3.0° 15.0°


13.50 μm=45 steps Tiled [100] IPF Map


20µm


Figure 9: Grain structure of a Cu free air ball before bonding(optical microscopy of etched cross-section).


This effect is caused neither by contamination, nor by oxidation, because they should be visible on the FIB image(Figure 8). Actually some contamination, visible in another area of the FIB image could be traced back on the OIM map(shown on both images with arrows). On the other hand, if oxidation were present, this would cause loss of the channeling contrast in this area of the FIB pattern, which is certainly not the case. Therefore the only possible reason left is a very high dislocation density, which leads to a loss of EBSD pattern. The increasing grain misorientation in this region, which is noticed in the OIM image, clearly points in this direction. For more clarity, two types of grain boundaries were used on this OIM map: high angle (>15º),


with a thick line, and low angle (<15º), with a thin line.


High angle boundaries typically separate recrystallized grains. Low angle boundaries are associated to small misorientation inside the grains, i.e they are typical for deformed grains. The increased density of low angle boundaries in and around the marked region in Figure 8,which at the end leads to a loss of EBSD patterns (black areas), can be related only to strong deformations. In addition, the FIB image of this area indicates “smashed”grains. The existence of this strongly deformed region can have important consequences. The “stored energy”accumulated during this deformation provides a strong driving force for recrystallization [8]. According to this, a subsequent recrystallization in this area should be expected upon annealing (for instance during high temperature storage experiments) which will probably affect the reliability of the wire bond. In order to investigate this effect we are presently performing an annealing experiment. This result shows also that the deformation during bonding localizes mainly around the center of the wire bond. It leads also to stress concentration in the die locally below this point, which increases the chances for failure during bonding.


Summary and Conclusions


Summarizing, this work shows the benefits of OIM for testing Cu bond pads and Cu interconnects, as follows:


• The traditional application of OIM reveals the texture and microstructure of Cu bond pads and interconnects.


The <111> texture seen in bond pads and interconnects randomizes for narrow lines and upon annealing.


• A non-traditional application of the method can be used also to trace the early stages of oxidation. Especially the latter finding is a new and original application of this technique. We showed, using OIM, that Cu bonding is very sensitive to oxidation of the bond pads.


• The study of a cross-section of a wire bond by OIM became possible due to a non-conventional preparation technique. A strongly deformed zone at the interface between wire bond and bond pad was found. It can be expected that this region, due to its high recrystallization potential, might affect the reliability of the wire bond during a thermal aging. The high localization of this deformed zone around the center also suggests a stress concentration in the die during the bonding process.


The work reported here is based upon the IMEC’s “Waferlevel packaging on Cu/low-k” Industrial Affiliation Program. The continous assistance of the project menager Pedro Banda is kindly acknowledged. The authors would


like to thank also Dr. Charles J. Vath III from ASM Technology Singapore Pte Ltd for his and his company support and fruitfull discussions. The authors thank Mrs. C.


Drijbooms for the FIB work.


1. A. J. Schwartz, M. Kumar and B. Adams, “Electron Back-Scatter Diffraction in Materials Science”, ed.


Kluwer, New-York (2000).


2. D. P. Field and M. Novel, Proc. of 4-th Int. Conf. on Recrystallization and Related Phenomena, Eds. T.


Sakai and H.G. Suzuki, The Jap. Inst. of Metals (1999).


3. TSL, Inc. OIM Software Version 2.0 User Manual,Draper, UT (1996).


4. L. Carbonell, P. Ratchev, R. Caluwaerts, M. Van Hove,B. Verlinden and K. Maex, accepted for publication in"Microelectronics Engineering".


5. H. M. Ho, W. Lam, S. Stoukatch, P. Ratchev, Ch. J.


Vath III, E. Beyne, Proc. of Eur. Microelectronics Packaging and Interconnection Symposium , Cracow,Poland (2002).


6. C. Ryu, A. L. S. Loke and S. Simon Wong, 35th IEEE Int. Reliability Phys. Symp. Proc., 201-205 (1997).


7. E. M. Zielinski, R. P. Vinci and J. C. Bravman, J. Appl.


Phys. 76 (8), 4516-4523 (1994).


8. F. J. Humphreys and M. Hatherly, “Recrystallization and Related Annealing Phenomena”, Elsevier Science Ltd., Oxford (1995).


Materials Analysis and Process Monitoring in MegaFabs


Bryan Tracy


Advanced Micro Devices, Sunnyvale, Ca


The essential role of the material analysis laboratory in modern IC production is confirmed by the scale of the investment made in such facilities. The laboratories are part of the initial design of the fab and are well staffed and superbly well equipped.


There are many factors which drive this investment,but perhaps the most compelling is the realization that the materials analysis lab is required to support early fab start-up, support production needs, and to pursue process development. During this talk,examples of each of these functions will be presented. The metrology of IC production is highly varied, and the implementation of this metrology varies widely company-to-company and even within any given company. The balance of in-fab vs out-offab measurements is of considerable importance and will be discussed in detail during this talk. Pertinent examples of contamination analysis and defect review will be presented.


Looking ahead to 100 and 70nm nodes, the imaging requirements are daunting and will require scanning electron microscopes with astoundingly high resolution. Remembering that the physical gate length in a modern microprocessor is approximately one half the technology node size, it is clear that imaging 35nm transistors at 500KX will be required.


Examples of state-of-the-art SEM, TEM and STEM will be presented as a "look-ahead" into the imaging requirements of the sub 100nm technology generations. The introduction of exotic materials such as high and low K oxides and ultra-thin barriers present special challenges and will spur a lively debate as to which measurements are needed, which measurements can/should be taken in the fab, and, of course, the turnaround time and cost? The rush to early process transfer and early production has given rise to the concept of "concurrent process development and transfer", where the new process flow is transferred to the megafab, almost in its infancy. In this case, the role of the materials analysis lab is expanded to directly aid "next generation" process development. As can be seen from the discussion above, the importance and linkage between Materials Analysis and IC process control has never been greater.


The new materials and structures in the sub 130nm nodes promise to introduce at least as much change into semiconductor manufacturing as have the last several technology generations combined. These new materials have selected properties, which make them attractive from a specific performance point of view. However, they typically have large "negative properties" which must be contained, designed around and monitored. Furthermore, these selected materials properties are not a given, and specific measures must be taken to insure that these beneficial properties continue to be delivered into the final product.


For example, contrast titanium metal and low K dielectrics. In the mid 80's titanium was added to the back-end metallization stack because it solved a number of problems which had been increasingly disruptive to IC manufacturing. With the addition of a single PVD sputtering step, three major problems were eliminated: Si junction spiking, high contact resistance, and poor electromigration lifetime. This titanium deposition step added some cost and time to the process and necessitated the development of new etch recipes, but with the possible exception of triaxial tensile stress voiding, this Ti dep was both beneficial and benign to the IC process flow. The introduction of low K materials in contrast has been anything but fast and easy. Low K's are required in order to reduce RC propagation delays. However,these low K materials have decidedly inferior mechanical and chemical stability properties. In order to ease the integration challenges, initial low K dielectrics have chemical compositions close to SiO2; for example SiO2[F] and SiO2[C]. But even these modest composition changes have necessitated re-engineering of the dielectric etch processes, and the fluorine-containing materials are fraught with delamination problems as a result of fluorine's intense reactivity with materials such as titanium.


Going forward, the integration of low K dielectrics poses even greater problems. For example, it will likely be necessary to monitor the "engineered porosity" with advanced metrology tools such as Ellipsometric Porosimetry1 (EP) or X-Ray Specular Scattering2. An example of a bimodal pore size distribution obtained by EP is shown in Figure 1.


Pore Radius, nm


Figure 1: Ellipsometric Porosimetry plot of a low K material show a bimodal pore size distribution.


Alternatively, the X-Ray reflectivity method can be used to make similar pore size distribution measurements in low K materials. Please see Figure 2 below.


C007350-20 9.0kV x150k SE


300nm


0.7p


Figure 2: Small angle x-ray scattering plot of a porous low K material


An advantage of the X-ray technique is that the same tool can also make x-ray reflectivity measurements which give very accurate and precise film thickness and density values. This combined functionality makes the x-ray techniques very attractive from an in-fab perspective.


25


-6- Desoption


SOI Monitoring


The likely widespread use of SOI in volume production, see Figure 3, will bring new metrology


15


and monitoring protocols. At this point, it is not clear which parameters need to be monitored. Some


dV/dR


possibilities include, Crystal Originated Pits (COPS),


古


stacking faults, oxygen level, stress, body thickness,Buried Oxide (BOX) thickness and perhaps the


00A2345


roughness of the top surface of the body.


Figure 3: SEM image of an SOI transistor.


06


Pore size distribution


Nitrogen in the Gate Oxide


#31;Do=1.4nm#32;Do=1.5nm---#33;Do=1.8nm


In order to allow the continued scaling of SiO2-like materials, nitrogen is added into the gate oxide.


y/nm-1bilitPbaro


Dielectric constant


ESCA is emerging as a possible process monitor. An example of ultra-high resolution ESCA depth


#31:k=2.54


profiling of a nitrided gate oxide is shown in Figure 4


#32:k=2.43#33:k=2.28


below. However, for process monitoring, it is likely that the ESCA measurements will be confined to nitrogen dose and film thickness.


Figure 4: ESCA depth profile of 2nm gate oxide.


0 2 4 6


24


。810


8 10 12


4


6


Angstro


O


Pore Diameter D/nm


S*SiO


Contamination Control


The analytical technique of choice for these operations appears to be in-fab Total Reflection XRay Fluorescence (TXRF). This technique has many advantages including surface sensitivity, speed, low detection limit, good standards and ease of use.


Most current megafabs have at least one TXRF.


With Cu and high K materials, the risk of cross contamination is higher and a "front end" and "back end" TXRF is a likely fab configuration. The TXRF EDS spectrum, Figure 5, shows the excellent sensitivity of this technique to low concentrations of transition metal contamination.


Figure 5: TXRF-EDS spectrum.


Poly Profiles


Aggressive device scaling is most excruciating at the poly gate layer where the physical dimension is less than 1/2 of the design rule. Indeed, it is likely that we will see 50nm transistors in production by yearend 2002!! The lithography and etch requirements needed to produce such structures are daunting and require imaging at enormous magnifications. An example of a "poly profile monitor wafer" is shown below in Figure 6 at 500KX.


Figure 6: Polished SEM XC of a 70nm transistor.


Recently, there has been an effort to automate this poly profile measurement using the Dualbeam Focused Ion Beam (FIB). Unattended operation of this tool would allow sampling of many more sites per wafer and could be completed as an in-fab operation. This in-line metrology is already well established in the hard disk industry. An example of first results3 is shown below in Figure 7.


Figure 7: Automated Dualbeam FIB poly profile cross-section.


A new and exciting possibility for poly gate profile imaging is the use of "low voltage" scanning transmission electron microscopy (LV STEM).


Conventionally done at 200kV, the recent work of Nakagawa and Dunne4,9 shows the exceptional promise of this technique. Superb layer contrast is obtained from these low Z materials, even at moderate thickness (100nm) and 30kV. STEM samples can be prepared by FIB in two hours. The


thin sample geometry overcomes the three main problems associated with conventional SEM cross sections by providing improved layer contrast and eliminating both chemical staining and metal coating.


Please refer to Figures 8 and 9.


Figure 8: 30kV STEM image of a poly gate transistor


4 mm HfO2


106 105


-- simulated profile oexperimental data


Poly-Si


Si3N4


克克京点 Intensity (counts s1)


SO2


036007200108001440


Si Sub


Co Si2


Angle (arcseconds)


(f)


S-5200 30.0kVx500k TE


|||4 nm HfO2|4 nm HfO2|4 nm HfO2|4 nm HfO2|4 nm HfO2|
|---|---|---|---|---|---|---|

|Layer|Layer|t(A)|t(A)||σ(A)|σ(A)|

||||||+49|+49|

|Si substrate|Si substrate||||1.1 -12|1.1 -12|

|||||+2.7|+0.5|+0.5|

|SiO1|49|49|-2.0|-2.0|1.0|-10|

||||+0.3|+0.3||+0.5|

|HfSii-O2|HfSii-O2|2.6|2.6|-02|-02|+0.5|

|||33.6|33.6|+0.3|+0.3|2.8|

|HfO2|HfO2|||-02|-02||

|||||+1.7|+1.7||

|HfO2|HfO2|6.7|6.7|-17|-17|9.0|

Figure 9: 30KV STEM image of gate corner/spacer.


High K Gate Oxide


It is hard to know which analytical methods will be most useful for the production monitoring of this completely new class of materials, but it is probable


-0.03


that a subset of the analytical techniques most useful during early process development will be used to monitor high K gate oxides in production. ESCA's sensitivity to chemical bonding, whole film sampling without sputtering, precise thickness measurement capability (see Figure 10), and non-destructive nature, make it the leading analytical technique.


Additionally, the non-destructive nature and high


intrinsic accuracy of X-Ray Reflectivity (XRR) are compelling attributes. Please see Figure 11.


Figure 10: ESCA depth profile of an HfO2 film.


Figure 11: XRR spectrum of a Hafnium silicate film.


Note sub-angstrom accuracy of this technique.


SI:N


10 20


30 40 50 60


SiO2


W


70 80 90 100


CoSu


150nm


50


Depth (Å)


C1s


N1s O1s小Si2p.1 Si2p.2 Hf4f.1 Hf4f.2


Backend Processing


The materials analysis and process monitoring needs


for copper metallization are extensive at all nodes.恚th1aD焦UDualbeam FIB technology, shown schematically inFigure 12 is a "must have" tool for both SEM andTEM analysis.


Figure 12 - Dualbeam schematic, courtesy FEI Corp.


Copper Voiding8N58600m50 MAL-2080-0062F7 BE16:2EE Bean Bood MagmWD


Copper voiding is major headache in the megafab production of IC's. Copper can form as many as four different types of voids6,10 (see Figure 13)necessitating constant vigilance and tight process control.


1) via interface voids


2) via sidewall voids


3) bulk voids


4) cap layer voids


Figure 13: Typical Void defects in Cu.


FIB sectioning of void test structures is a destructive but effective method to monitor process induced voids. See Figures (14-16) below:


Dual-column tools for failure analysis


Fig 14: SEM of a M2/M1 via void test structure.


SEM


>Schottky emtter


Us0.5-30 kov>Resolution3 mm


FIB


60°


5mm


IonMicroscope (FIB)>Gafon source5-30 kev 1-20.000A>Resolution 7 m


ElectronMicroscope


Figure 15: Bulk and via sidewall voids.


EBeam Spot MagmDat WD


500:mm


50000mTLD ED MAL-00785-00 72E7 moh BE11 2-3


Figure 16: Cap interface voids.


Sub surface Cu voiding is particularly hard to detect because it neither visible to "top view" KLA-like inspections and rarely results in a full electrical opens. Thus slower and destructive techniques are required to monitor the process. Passive FIB voltage contrast is especially helpful with well-designed test structures. Please see Figure 17 below. Figure 18a shows the location of the failing via using top-down


voltage contrast. Figure 18b, reveals the viainterface void.


Figure 17: FIB passive voltage contrast schematic.


Figures 18a and 18b: FIB voltage contrast image and via test structure showing via interface voids.


Barrier Metal Step Coverage


It has been our experience that step coverage monitoring of the barrier layer using transmission electron microscopy is a full-time proposition requiring daily FIB sample prep and subsequent TEM analysis. A nice example of such step coverage measurements is shown in Figure 19. In this case, the image was formed using a relatively new technique called Z-contrast. Z-contrast images


are taken in the high resolution scanning TEM(STEM) mode. Only electrons which are scattered to high angles (large atomic number) are used to form the image resulting in strong contrast between the barrier metal and the copper.


Figure 19: Barrier Metal via step coverage.


The plated copper thickness will have to be monitored, but the greater challenge is monitoring the step coverage of the tantalum-containing barrier.


The via and trench etches must be almost perfectly controlled such that a thin, conformal barrier can be deposited. Once again, the process window for barrier metal deposition is tiny, but critical, because the subsequent sputtering of the copper seed and plating of the bulk copper crucially depend on proper tantalum deposition. Should any of these steps go awry, voiding of the copper trench is the likely result.


Free surfaces such as voids are fast diffusion paths for electromigration resulting in significantly degraded reliability.


As much as we may desire to move away from TEM because of its time and resource consuming nature,the honest truth is that no other analytical technique has the resolution and contrast to make such critical measurements of atomically thin layers on topography. Indeed several papers have already been published in which TEM tomography techniques, see Figure 20 below, have been used to better understand the three dimensional characteristics of barrier metal step coverage5,6.


Figure 20: 3D TEM reconstruction of barrier metal.


The preceding analytical examples are by no means an exhaustive list of the enormous variety of metrology measurements made in a modern megafab.


Indeed such a compilation would consume an entire volume. Other related metrology areas include Contamination Free Manufacturing (CFM), wafer electrical test, 4-point probe and various types of profiliometery and scatterometry.


Looking ahead, it is likely that additional "engineered materials" will be introduced into the IC process flow. Any time such "specific function" materials are used, it is likely that the materials parameters which measure this desirable property will have to be monitored in order to insure that the final product will be fully functional. The best example is the implementation of low k dielectrics. Great engineering efforts have been made to produce and integrate low K's into the process flow. It would be very unfortunate, after all of this effort, if the low K properties were degraded by some small shift in the process parameters. Indeed such materials are highly sensitive to the exact etch and resist strip processes7.


During the past twenty years, the material analysis laboratory associated with IC production has expanded enormously in both staffing and instrumental sophistication. In the early eighties, it was called the "SEM Lab" and contained a few optical microscopes and an SEM. In the 100nm generation, the "Materials Characterization Facility"is a $25M investment, staffed with 25 people including numerous PhD level scientists and engineers. This trend can only continue as all


foreseeable implementations of the ITRS Roadmap8 mandate the increased use of exotic materials and non-conventional devices. IC processes are unlikely to get simpler and most assuredly devices will get smaller. The net result is it is a good time to be a failure analyst/materials scientist.


The author would like to sincerely thank all those individuals who freely shared their experience and micrographs with the author. These individuals include: Eckhard Langer, Ehrenfried Zschech, Mine Nakagawa, Alain Diebold, Joffre Bernard, Hans Juergen Engelmann, Heiko Stegmann, Cynthia Gonsalves, Steven Robie, Alline Myers. John McIntosh.


1.


Figure 1 courtesy of Alain Diebold,SEMATECH.


2.


Figure 2 courtesy of Rigaku Corporation.


3.


Unpublished research, Bryan Tracy and John McIntosh, FEI Corporation, 2002.


4.


M. Nakagawa and R Dunne, J of the Japanese Society for Electron Microscopy,51(1), 53-57 (2002).


5.


J. Mardinly: Microscopy and Microanalysis Meeting, Long Beach, Ca, USA, 2001.


6.


H. Stegmann, H. J. Engelmann, E. Zschech:Microelectron. Eng (2002) in press.


7.


T. Poon, J. Ma, M. Naik, B. Tang, M. Yu,C. Lang, I. Lou, D. Sugiarto, P. Lee, W.


Yau, D. Cheung, VMIC proceedings, Sept 7-9, page 190-192, 1999.


8.


International Technology Roadmap for Semiconductors, Semiconductor Industry Association, 2001.


9.


Figures 8 and 9 courtesy Hitachi HighTechnologies, Technical Data, SEM 100.


10.


E. Zschech, E. Langer, H. J. Engelmann, K.


Dittmar, EMAS, Strasbourg, Sym O, 2002


STEM (scanning transmission electron microscopy) in a SEM


(scanning electron microscope) for Failure Analysis and Metrology


William E. Vanderlinde


Laboratory for Physical Sciences, College Park, MD, USA


Recent developments in transmission electron  microscopy (TEM) sample preparation have greatly  reduced the time and cost for preparing thin samples. In this paper, a method is demonstrated for viewing  thin samples in transmission in an unmodified  scanning electron microscope (SEM) using an easily  constructed sample holder. Although not a substitute  for true TEM analysis, this method allows for spatial  resolution that is superior to typical SEM imaging  and provides image contrast from material structure  that is typical of TEM images. Furthermore, the  method can produce extremely high resolution x-ray  maps that are typically produced only by scanning  transmission electron microscope (STEM) systems.


Recent literature has demonstrated greatly improved  methods for preparing thin samples (<100 nm thick) for TEM analysis by automated cleaving, polishing, and focused ion beam methods.1 In particular, Tsung  et al.2 showed a method for preparing 10 TEM


samples in about 6 hours using a combination of  focused ion beam (FIB) deposition and reactive ion  etching. Tsung developed this method to enable  routine metrology of sub-0.2 micron poly lines since  cross-sectional SEM images lack sufficient  resolution. These advances have brought TEM  sample preparation into reach of the typical failure  analysis laboratory. However, dedicated TEM  systems remain expensive to purchase and maintain, and they require highly trained personnel to operate. Therefore it is highly desirable to be able to view a  thin sample in transmission in ordinary SEMs that are  widely available.


Modern field emission SEMs have a nominal spot  size of 1 nm or less, but it is rare to see resolution of  1 nm on any sample other than a special resolution  standard such as gold islands on a carbon substrate. However, viewing a thin sample in transmission can  produce an image with resolution approaching the  actual beam diameter. Although it is possible to  mount a secondary electron detector underneath the  sample stage for detecting the electrons transmitted  through the thin sample,3 it is far more convenient to


create a special “STEM-in-SEM” holder and simply


introduce that holder into the SEM when STEM  imaging is desired.


The lateral spatial resolution of energy dispersive xray spectroscopy (EDS) elemental maps is generally  limited to a few hundred nm in bulk samples due to  lateral scattering of the electron beam in the sample.  However, X-rays created by an electron beam in a  thin sample will be localized to a small region in the  sample allowing very high spatial resolution energy  dispersive x-ray maps with the STEM-in-SEM  method. Note that in a typical TEM the beam is not  scanned and the “spot mode” is generally limited to  about 1 micron beam diameter, thus limiting x-ray  spatial resolution. Very high spatial resolution x-ray  maps can also be achieved in thin samples using the  much more expensive STEM instruments.


The STEM-in-SEM concept is well documented in  the literature,3 including the use of a high atomic


number reflector below the sample to generate  secondary electrons.4 This method is sometimes used


to obtain high resolution images of particles mounted  on a carbon thin film. In the present work an  integrated sample holder and detector was designed  using a graphite collimator and a high-efficiency twostage gold reflector which enabled high resolution  STEM-in-SEM images of thin films cross sections of  semiconductor devices.


Experiments were conducted in a LEO 1550VP field  emission scanning electron microscope with nominal  beam diameter of 1 nm at 30 keV. This SEM was not  modified in any way other than the introduction of a  modified sample holder. The “STEM-in-SEM” holder is shown in Fig. 1. The body of the holder was  machined from 1 cm stock aluminum. The thin  sample is mounted in a recessed slot near the top of a  graphite block. After passing through the thin film  sample, the electron beam travels down a narrow hole  drilled in the graphite block. The graphite acts to  collimate the beam by absorbing the highly scattered  electrons. Thus, it improves the image resolution. After passing through the collimator, the electrons  strike a pair of gold reflectors.


The first gold reflector is at very low tilt angle (~10o) to the beam as this will create the maximum number


of secondary electrons. This first reflector also directs  the high energy forward scattered electrons into the  second gold reflector where even more secondary  electrons are created. These secondary electrons are  then collected by an ordinary secondary electron  detector (SED) in the SEM chamber. The two-stage  reflector produces about 3 times as many secondary  electrons as a simple 45 degree reflector. Although  some secondary electrons will be created at the top of  the thin sample, the quantity of these electrons will  be negligible compared to the large number of  electrons produced by the gold reflectors.


The LEO 1550 VP has both an in-chamber SED in  the normal position, and also an in-lens detector  above the final lens which collects secondary  electrons that go back up the column. Since the inlens detector can only collect the secondary electrons  emitted from the surface of the thin sample, this  detector produces an ordinary SEM image rather than  a STEM image. The ability to switch quickly  between the in-lens detector and the in-chamber  detector was a convenient feature for this experiment  since it was easy to compare reflected and  transmitted images.


Figure 1: Design for a “STEM-in-SEM” sample  holder. The overall height is 2.5 cm.


Figure 2: Optical photo of the STEM-in-SEM sample  holder mounted to the SEM stage. The pole piece of  the final lens is visible above the sample holder.


For this experiment, thin samples were prepared by  traditional TEM preparation methods including  polishing and ion milling and were then mounted to a  standard 3 mm diameter TEM grid. The TEM grid  was then placed in a shallow 3 mm diameter  cylindrical hole in the top of the STEM-in-SEM  holder and held in place by a retaining ring. However, the STEM-in-SEM holder can be easily  modified for a variety of sample shapes and lengths. When thin samples are prepared by FIB, the 3 mm  limitation on sample size imposed by standard TEMs  can significantly increase the difficulty of the  preparation2 but with STEM-in-SEM the sample can


be of virtually any length. It is, however, crucial that  the sample be mounted in a clean and mechanically  rigid fashion. Metallic tape is often used to mount  SEM samples, but at the very high magnification  available with STEM-in-SEM the tape will allows  unacceptable sample drift. Likewise, carbon paint is  often used to mount SEM samples, but with STEMin-SEM the paint was found to transfer carbon  contamination to the thin section. Therefore a  mechanical mounting method such as spring clips or  retaining rings is recommended.


Electron Beam-Sample Interactions


Transmission electron microscopes typically operate  at 200 kV or higher, so it may be somewhat  surprising that an electron beam voltage of 30 kV or  less can be used to view a sample in transmission. While it is often said that TEM samples must be  thinned until they are “electron transparent” this is a  misleading statement. The electron range of a 30 keV  electron in aluminum can be calculated by the  Kanaya-Okayama formula as more than 8 microns.5


TEM samples are typically thinned to less than 100  nm thick so that most of the electrons undergo no  more than one scattering event, since TEM imaging  is typically done with electrons that have not  undergone any scattering events (bright field) or  those that have been scattered exactly once by the  lattice (dark field). At 200 keV the mean free path for  elastic scattering is large (~350 nm) compared to the  thickness of a 100 nm thin film, but at 30 keV the  elastic mean free path in aluminum is 17 nm for a  scattering angle of 2 degrees or greater.6 Therefore at


30 keV an electron will typically be scattered several  times when passing through a 100 nm thin sample, resulting in degraded lateral spatial resolution.


A Monte Carlo simulation of electron trajectories was  conducted using the commercially available “Electron Flight Simulator” program,7 see Fig. 3. The


Monte Carlo simulation shows that 30 keV electrons  will be scattered into a cone of half-angle 8.5  degrees, resulting in a beam diameter of about 30 nm  as the beam exits a 100 nm thin film. In order for a


raster beam system to produce a sharp image, electrons should collect information only from the  area very close to where the beam enters the sample. If the beam scatters 30 nm laterally within the  sample, then contrast will be collected from materials  that are far from the electron beam position, which  will seriously degrade the image resolution. Thus a  graphite collimator was designed into the STEM-inSEM holder below the sample to absorb the most  highly scattered electrons. The design of the  collimator necessitates a trade-off between the need  for a large transmitted signal and ease of aligning the  sample to the hole, versus the desire for eliminating  the most highly scattered electrons that will degrade  image resolution. Prototype holders were constructed  with a 5.2 degree half-angle of acceptance (using a 1  mm diameter hole in a 5.5 mm long collimator) and a


3.5 degree half-angle of acceptance (using a 0.6 mm  diameter hole in a 5 mm long collimator). In both  cases it was possible to achieve both easy alignment  and adequate secondary electron signal.


Figure 3: Monte-Carlo simulation of the trajectories  of 30 keV electrons passing through a 100 nm  aluminum thin film.


For an electron deflected through angle θ passing  through a film of thickness t, the total lateral  deflection x is given by:


x = 2t tan θ


Given a 3.5 degree collimator, the lateral scattering in  a 100 nm film is about 11 nm. Since the observed  resolution in the STEM-in-SEM images was as small  as 2 nm, it is apparent that the film must have been  much thinner than 100 nm in the sites where the  highest resolution images were taken.


Figure 4: Diagram illustrating the derivation of  Equation 1.


Figure 5 is a low magnification image acquired by  using the SEM’s in-chamber secondary electron  detector (SED) to collect secondary electrons from  the gold reflectors that were produced by electrons  that passed through the sample. The image shows the  TEM sample, which consists of a thinned strip of  silicon attached to a 3 mm copper grid with an oval  hole. The bright circle in the center of the picture  corresponds to the hole in the graphite collimator  which allows electrons to penetrate to the gold  reflectors. When necessary, the holder was tilted to  bring the area of interest to the center of the bright  circle, and the entire holder was then rotated to  maximize the collection of secondary electrons from  the gold reflectors to the secondary electron detector. Once the holder was aligned, high resolution STEMin-SEM images were acquired by selecting a thin  area of the sample and simply increasing the  magnification and then focusing and stigmating in the  usual fashion.


1 mm


Mag = 74x


Figure 5: Low magnification STEM-in-SEM image  showing the TEM sample.


Due to the high resistance of tungsten to ion milling, tungsten is difficult to ion mill to transparency  without destroying a thin sample. Since these thin


samples were prepared by polishing and ion milling  methods, the tungsten plugs shown in this experiment  are opaque in both conventional TEM and the  STEM-in-SEM images. Ion milled films tend to vary  in thickness and may be as thin as 20 to 30 nm in  places, which would allow higher resolution than that  calculated by the Monte Carlo simulation.


Electron Imaging Results


Figures 6, 7, 9, and 11 are STEM-in-SEM images of  typical CMOS structures such as aluminum lines,


100mm


TMag=215.95KXWD=2mmEHT=20.00AVSignNA=MP3EDato :27IXar 2002


tungsten plugs, and poly lines with sidewall spacers. These images were taken at 20 kV or 30 kV beam  voltage and 2 mm working distance. For comparison, Figures 8, 10, and 12 are images of similar structures  taken using a traditional bright-field TEM at 120 kV  beam voltage. The traditional TEM images are  clearly higher resolution, but the STEM-in-SEM  images have a similar appearance and contrast to the  TEM images, showing internal grain structure on the  poly-silicon, the aluminum, and the barrier metals. Close examination of the STEM-in-SEM images  demonstrates a resolution of approximately 2 nm  which is far superior to that achieved by traditional  SEM images of these structures. The STEM-in-SEM  image contrast is based on differences in atomic  number, density, and crystallographic orientation  which scatter different numbers of electrons away  from the detector.8


100Hm


Aag=100.00kxWD=2mmFle Name=B8s.tfTime:18:22:05EHT=30.00kVSignalA=MPSEDale:14 Jun 2002


200 nm


Mag = 100,000x


Figure 6: STEM-in-SEM image of an aluminum line  connected to a tungsten plug contact. The barrier  layer and the plug liner are visible.


Fle Nare=C8120KMicf Time:14:42:55


Mag = 216,000x


Figure 7: Higher magnification STEM-in-SEM image  resolving a titanium plug liner and barrier layer.


Um


100 nm


Mag = 240,000x


Figure 8: Conventional TEM image of structure  similar to Figure 6.


100rm


EHT=20.00AVSignalA-MPSEDale:18Ma|2002 MoG-250.00KXWD-6mmProte No.=144Time:19:01:41 200 nm


Mag = 250,000x


Figure 9: STEM-in-SEM image of a tungsten plug  contacting silicon.


Al Line


W Plug  Ti Barrier


Ti Barrier


and Plug Liner


Ti Plug  Liner


Ti Barrier  Layer


Figure 10: Conventional TEM image of structure  similar to Figure 9.


200km


EHT=20.00AVSignal A=InLersDa%o:18Ma:2002


Mag=100.12KX


WD=6mmPhoto No.=140Time:18:34:51


Figure 11: STEM-in-SEM of broad poly-silicon line  with sidewall spacer.


50 nm


Mag = 500,000x


Figure 12: Conventional TEM of narrow poly-silicon  line with sidewall spacer.


For comparison, Figure 13 is an image of a thin film  mounted to the STEM-in-SEM holder, but with the “in-lens” detector being used to generate a normal  SEM image. Resolution is good, but not significantly  better than an ordinary cross-sectional SEM.


Figure 13: Conventional SEM image of a thin film  acquired with an “in-lens” detector.


Figure 14 shows a STEM-in-SEM image taken  without the graphite collimator. Lateral scattering  serious degrades the resolution, proving that the  graphite collimator is needed to achieve high  resolution.


EHT =20.00 kVSignal A=MPSE


Mag=250.00KX


WD=3mmPhoto No.=138


Figure 14: STEM-in-SEM image taken without using  the graphite collimator.


||1091|EHT=30.00AV|SignalA=MPGE|Dake:16Ma:2002|
|---|---|---|---|---|

|mag=200.00Kx||WD=6mm|Photo No.=131|Time:19:13:08|

|100 nm |||Mag |= 200,000x |

As an experiment, the STEM-in-SEM holder was  tilted so that the imaged area was outside the bright  circle that corresponds to the entrance of the  collimator, see Figure 15. Under these conditions, only the scattered electrons are able to pass through


50mm


the collimator and reach the gold reflectors, in effect  creating a “dark field” image. Note that the tungsten  which is dark in the other images now shows some  bright areas. The overall image has degraded  resolution, but the contrast on the material just below  the tungsten-silicon interface is enhanced. It may be


Sidewall spacer


Poly-silicon


that this type of dark field imaging could be used to  enhance the contrast from highly scattering material  such as inter-metallic grains at material interfaces.


Bulk sample


Mag=100.00KxWD=1mmEHT=30.00AVSignlA=MP3ERleName=C7k.JagTime :16:24:39Cato:23May 2002


Figure 15: “Dark Field” STEM-in-SEM image.


X-ray Elemental Imaging in Thin Films


There are many advantages to performing energy  dispersive x-ray spectroscopy on thin films rather  than bulk samples. First, the x-rays are localized to a  smaller region allowing better lateral spatial  resolution. Second, it is possible to create the x-rays  using a very high energy electron beam that generates  a greater variety of characteristic peaks and can  eliminate peak overlap problems. Furthermore, the  high energy electron beam will create more  characteristic x-rays and also reduce the amount of  Bremsstrahlung background x-rays relative to the  characteristic peaks, which improves trace element  sensitivity and reduces noise in x-ray maps. Each of  these points is discussed in further detail below.


High energy electron bombardment of solids  produces x-rays by two distinct mechanisms:  (1) electron shell transitions result in x-ray peaks with  energies that are characteristic of the element that  produced them, and (2) the Bremsstrahlung or “braking radiation” effect produces a broad  background in the x-ray spectrum that is generally  considered a nuisance since it interferes with  detecting the characteristic x-rays.


When an electron beam enters a bulk sample, x-rays  are created in a fairly large region called the “excitation volume” as show in Figure 16.  Although  the shape of the excitation volume varies with the  beam energy and material composition, in general the  lateral size of the volume is on the order of the same  distance as the electron penetration depth. As can be  seen in Table 1, this distance is more than one micron  at 10 KeV and almost 10 microns at 30 KeV. Therefore x-ray elemental imaging has very poor


lateral spatial resolution in bulk materials when the  electron beam energy is high.  However, if the  sample is a thin film then the x-rays will be localized  to a small region in the sample allowing much better  lateral spatial resolution.


e-beam


Thin film


X-rays


..*


Figure 16: Illustration of x-ray emission from a bulk  sample and from a thin film sample.


X-ray elemental mapping on bulk samples is often  conducted at 5 KeV electron beam energy or below  in order to decrease the amount of lateral electron  scattering and improve the x-ray lateral resolution as  well as the surface sensitivity, as shown in Table 1. However, the low beam energy limits the number of  x-ray peaks that are available for analysis. Of  particular concern is the fact that the silicon K-α peak  at 1.74 KeV overlaps the tungsten M-α peak at 1.78  KeV. Only when the beam energy is high enough to  excite the tungsten L-α peak at 8.40 KeV is it  possible to map tungsten against a silicon  background.


|Electron beam energy (KeV) |Electron penetration depth in silicon (microns) |
|---|---|

|5 |0.47 |

|10 |1.49 |

|15 |2.93 |

|20 |4.73 |

|25 |6.87 |

|30 |9.31 |

Table 1: Electron penetration depth in silicon as a  function of electron beam energy, calculated from  the Kanaya-Okayama formula.5


As the energy of the electron beam increases both the  number of characteristic x-rays and the number of  Bremsstrahlung x-rays increases rapidly, see Table 2.


300-


However, the characteristic x-ray production


700


increases more rapidly with beam energy than the


600-


Bremsstrahlung background, so the peak to  background ratio improves with higher beam energy.


500-


400


Since thin samples allow 30 KeV beam energy to be


used without compromising lateral spatial resolution, 200 these conditions will also provide x-ray spectra with


a good selection of characteristic peaks, high x-ray 100 intensity, and relatively low levels of Bremsstrahlung


background x-rays. The low background level means


that peaks for trace elements can be identified with


good sensitivity, see Figures 17 and 18. Furthermore,


low background levels reduce the noise in x-ray maps


which is caused by background rather than


characteristic x-rays.


Figure 17: EDS spectrum of silicon thin sample


showing a very high peak to background ratio. The


electron beam energy was 30 KeV.


Figure 18: EDS spectrum showing good sensitivity to  trace elements in a thin sample with Si, W, Al, Ti, O, and F. The electron beam energy was 30 KeV.


X-ray Imaging Results


|Electron Beam Energy (KeV) |Peak |Background |Peak to Background ratio ||
|---|---|---|---|---|

|Electron Beam Energy (KeV) |x-ray |counts at |Peak to Background ratio ||

|Electron Beam Energy (KeV) |counts |2.0 KeV |Peak to Background ratio ||

|Electron Beam Energy (KeV) |Si K-α ||Peak to Background ratio ||

|5 |734 |7.9 |93 ||

|10 |4489 |22.7 |198 ||

|15 |10652 |44.2 |241 ||

|20 |19583 |59.7 |328 ||

|25 |22402 |66.4 |337 ||

|30 |31744 |88.1 |360 ||

|Table 2: Characteristic x-ray peak |Table 2: Characteristic x-ray peak |Table 2: Characteristic x-ray peak |Table 2: Characteristic x-ray peak |counts |

|measured for the silicon K-α peak at 1.74 Bremsstrahlung background at 2.0 KeV |measured for the silicon K-α peak at 1.74 Bremsstrahlung background at 2.0 KeV |measured for the silicon K-α peak at 1.74 Bremsstrahlung background at 2.0 KeV |measured for the silicon K-α peak at 1.74 Bremsstrahlung background at 2.0 KeV |KeV and for a bulk |

|sample. Counts were measured for 10 energy bins. |sample. Counts were measured for 10 energy bins. |sample. Counts were measured for 10 energy bins. |sample. Counts were measured for 10 energy bins. |eV wide |

X-ray data was acquired using a NORAN Ultra-dry II  energy dispersive x-ray detector. For x-ray imaging, the STEM-in-SEM holder was rotated 180 degrees so  that x-rays from the gold reflectors would not have a  line-of-sight to the x-ray detector, which is located  near the secondary electron detector. Working  distance was also increased from the 2 mm used for  STEM-in-SEM images to about 20 mm needed for  the x-ray detector. During x-ray analysis, the electron  imaging was acquired by traditional means, i.e. secondary electrons emitted from the top surface of  the sample were directly collected by the secondary  electron detector.  Once a suitable area was located  for analysis, the electron beam control was  transferred to the x-ray computer and x-ray data was  collected at every point on a 128 by 128 raster array. X-ray windows for aluminum K-alpha (1.49 keV), titanium K-alpha (4.51 keV), and tungsten L-alpha (8.40 keV) were selected.


Figures 19, 20 and 21 are the resulting elemental  maps for titanium, aluminum, and tungsten. Fig. 22 is


3000-


a secondary electron image of the same area. The  appearance of some aluminum and titanium signal in


2500


the tungsten plug area is due to Bremsstrahlung x2000-


rays from the tungsten, a known artifact that occurs  in bulk x-ray mapping as well as these thin-film


1500-


maps.


1000-


Note that the magnification of these x-ray images is


much greater than typical for EDS elemental maps. The absence of lateral scattering in the thin sample  allows very high resolution x-ray mapping. However, resolution is clearly much lower than the 2 nm  achieved for STEM-in-SEM imaging due to the poor  signal-to-noise ratio of x-ray imaging. Another factor  reducing x-ray map resolution is the fluorescence  effect, i.e. x-rays produced by the electron beam


5.0 KeV


cause additional x-rays in the surrounding material. It  is difficult to quantify the x-ray map resolution, but  the upper titanium layer which is 35 nm thick does  clearly look thinner than the lower titanium layer  which is 55 nm thick. In the titanium elemental map  one can see both the very shallow depression in the  upper layer above the plug, as well as the much larger  depression in the lower layer, demonstrating an x-ray  resolution of perhaps 10 nm.


400 nm


Mag = 75,000x


Figure 19: Titanium elemental x-ray map.


Figure 20: Aluminum elemental x-ray map.


Figure 21: Tungsten elemental x-ray map.


Figure 22: SEM image of approximately the same  area as the elemental x-ray maps in Figures 19-21.


A method has been demonstrated for achieving  scanning transmission electron images in an ordinary  SEM with superior resolution of about 2 nm. Since  the method requires no modification to the electron  microscope it can be easily adopted by the typical  user. The method also allows for x-ray elemental  maps with resolution of about 10 nm to be acquired  on thin samples.


I would like to thank Mr. Harry Kawayoshi of  AMER, Inc. for preparing the TEM thin samples and  taking the conventional high-voltage TEM photos. I  would also like to thank Mr. Leslie Lorenz who  machined the STEM-in-SEM holder, Mr. Adarsh  Kumer who providing gold films used as reflectors, and Ms. Constance Schuster for arranging the sample  preparation.


1. S. Morris, S. Tatti, E. Black, N. Dickson, H. Mendez, B. Pyle, B. Schwisesow, and R. Pyle., Proceedings of ISTFA 1991, p. 417-427 (1991).


2. L. Tsung, A. Anciso, R. Turner, T. Dixon, and N. Holloway, Proceedings of ISTFA 2001, p. 299-302 (2001).


3. D. Susnitzky, ISTFA 2000 tutorial notes.


4. Joseph I. Goldstein, Dale E. Newbury, Patrick  Echlin, David C. Joy, A. D. Romig, Jr., Charles E. Lyman, Charles Fiori, and Eric Lifshin, Scanning  Electron Microscopy and X-ray Microanalysis, A  Textbook for Biologists, Materials Scientists, and  Geologists, 2nd  Edition, Plenum, New York, 1992, p.


267.


5. Goldstein, p. 89.


6. Goldstein, p. 74.


7. Available from Small World LLC, 2226  Chestertown Drive, Vienna, VA 22182.


8. Goldstein, p. 269.


Microcalorimeter Energy Dispersive X-Ray Spectroscopy   in Routine Semiconductor Failure Analysis


B. Simmnacher, R. Weiland


Infineon Technologies AG, München, Germany  E. Langer


Advanced Micro Devices, Dresden, Germany


M. Bühler, J. Höhne


Vericold Technologies GmbH, München, Germany  C. Hollerith


Technische Unversität München, Germany


Microcalorimeter based energy dispersive X-ray  analysis (EDS) combines in a revolutionary way  resolution of wavelength dispersive spectroscopy (WDS) with the ease of use of conventional EDS. The necessary operating temperatures (~100mK) for  the superconducting sensor are supplied by a  mechanical, maintenance free and fully automated  cooling system, allowing the integration of the  system not only in a traditional F/A environment, but  also as an inline (cleanroom) installation. Typical  examples of material analysis in everyday F/A work  show that the detector exhibits an energy resolution  of about 10 eV. With this performance, the solution  of well known overlap problems existing for element  combinations commonly used in semiconductor  technology (peak separation of Ti/N, Ta/Si, W/Si) is  possible. Structures of small volume can be  investigated successfully, since the tool is optimized  for work in the low energy range. The case of a  failing TiN-layer showed that µ-calorimeter EDS  allows also thin film analysis: oxide layers with a  thickness difference of a few nm can be  distinguished; subsequent depth-profiling with Auger  electron spectroscopy confirmed the results.


According to the semiconductor roadmap1) feature  sizes of below 40 nm will be reached in 2005.  Therefore semiconductor production and failure


analysis have to face new challenges and it has to be  ensured that future semiconductor components can  still be analyzed.


Because of shrinking dimensions, the use of common  material compositions as well as new materials (copper, tantalum and ferroelectric compounds) used  in semiconductor production, X-ray microanalysis  with conventional detectors of silicon or germanium  reaches its limit. Since standard energy-dispersive Xray spectroscopy (EDS) uses the primary beam of a  scanning electron microscope (SEM) for generation  of X-ray radiation, the spatial resolution is  determined by the energy of the primary beam and  the related excited volume. Furthermore, to excite  characteristic X-ray lines, the primary electron beam  energy has to be at least 2 times higher than the  energy of spectral line of interest. To minimize the  excitation volume and to avoid X-ray radiation from  non-relevant structures (lateral) or layers (vertical), the energy of the primary beam has to be reduced, so  that the elements of interest have to be identified  only due to their X-ray transitions in the low energy  range. Unfortunately, in this range the K-lines of  light elements tend to overlap with the characteristic  radiation from higher shells. With an energy  resolution of approximately 130 eV, conventional  semiconductor detectors are not able to separate  these peaks of characteristic radiation. Wavelengthdispersive X-ray spectroscopy (WDS) offers an  energy resolution of 5eV, because it is based on the  principle of X-ray diffraction. To cover  a wide  energy range several diffraction crystals have to be  used; the analysis is therefore extremely time  consuming, because the different energy bands have


to be measured sequentially with the corresponding  diffractors. Additionally, a large probe current due to  absorption loss is necessary, which can induce  damage or time dependent changes to the specimen.  The existing gap in material analysis, between fast  analysis with high-energy resolution, is filled by a  new microcalorimeter X-ray detection system.2), 3).


Detection principle


The microcalorimeter consists of a superconducting  Ir/Au phase transition thermometer detecting the  energy of the hitting X-ray quants by means of  temperature rise. The phase transition between  conducting and superconducting phase is shown in  Fig. 1. A small variation in temperature T results in a  large change in resistance RT that is measured by the  current change of a superconducting quantum  interference device (SQUID).


Since the transition curve is considerably steep, energy resolutions of 15eV and better are possible  with this detector type. Recently it was shown that  even energy resolutions of 2eV could be reached4). Energy calibration is realized by measuring the  detector response to artificial heat pulses. To  linearize the total energy range, pulse trains of  different energies are sent to the detector during the  accumulation of the spectrum.


Resistance [a.u.]50


∆T


∆R


Temperature [mK]


Figure 1: Transition curve of an Ir/Au phase


transition thermometer. The insert shows the read  out circuit.


Necessary temperatures of <100mK are reached by a  mechanical cooler, consisting of a pulse tube cooler  and a single stage adiabatic demagnetization  refrigerator (ADR) cooler5). This aspect is of major  importance especially for inline applications if


integrated in defect review tools or inline dual beam  SEM/FIB systems, because no liquid gases have to  be handled inside the cleanroom.


Integration in routine failure analysis


A beta-tool of this system has been installed in a  failure analysis lab, where industrial applications and  the benefits for semiconductor industry and every  day failure analysis are currently investigated5) 6). Like conventional EDS-systems, the instrument  consisting of the detector on top of a snout and the  cooler, is mounted onto a scanning electron  microscope with a Schottky field emission electron  source, allowing high resolution of 1.5nm@5keV. The tool is optimized for SEM imaging up to  magnifications of 200.000x where the electron  column becomes very sensitive to external  disturbance as caused e.g. by vibrations. As required  for a lab environment, the system works completely  automated in a way that analysis results can be  obtained on operator level. This includes complete  automation of the cooler, spectra acquisition and  peak identification via standard EDS software. With  typical operational times of 8 hours after which the  ADR has to be recharged for about 20min, the  handling of the cooler does not affect the daily  workflow in the F/A lab.


A drawback of the actual setup is the low count rate  resulting from the small active detector area of the  microcalorimeter compared to a standard Si(Li) detector. Consequently, spectra acquisition time is


150


relatively high (approximately 5 times longer) so that  the count rate will be the limiting factor for complex


analysis. As demonstrated4), integration of a  polycapillary lens system will heavily improve the  usability.


08590


95100


Analysis results


To test the capabilities of the microcalorimeter  system in routine failure analysis work, the focus is  set on


(a) commonly used material combinations with  overlapping X-ray peaks in the low energy range like  TiN and WSi2


(b) new materials which are related to copper  technology like Ta and TaN


(c) analysis of multilayer systems


(d) analysis of structures of small volume (e.g. particles)


There are several element combinations which are  commonly used in semiconductor fabrication,


characteristic X-ray lines of which can not be


350


sike


separated with conventional energy-dispersive X-ray


WMa


detectors. The basic energy resolution of the system,


S250


compared to that of a standard EDS detector, can be


山


n20011,9eVsike


seen in the X-ray spectrum of TiN, which is used as


3150


WmS


barrier layer or antireflective coating (Fig. 2). An


identification of Ti by its Kα  line (4.508 keV), as


50 usually necessary with a conventional Si(Li) detector, 0+is not successful for analysis of thin coatings or


1500160017001800 1900200021002200


layers, as X-rays are emitted by the whole excited


energy /eV


volume. Since the N-Kα line (392 eV) and the Ti-Lα  line (452 eV) in the low-energy range are separated  by only 60 eV analysis with a standard tool is not  possible, whereas the microcalorimeter detection  shows a clear separation of the two peaks. From the  spectrum in Fig. 2, the typical energy resolution is  determined to be 10 eV@1keV. Although the count  rate of the detector is low, an identification of the


present elements is possible after an acquisition time


TaMC


of several minutes due to the low background level.


140


160


s120Oke U


n100


TaMz


080


140 120


40-


9


u100


11.5eV


n 0 0


C160.


TiLx


50075010001250150017502000


80-


0T 20 60


Figure 2: X-ray spectrum of TiN. Comparison of  measurement with conventional Si(Li) detector (red,


counts x 50) and µ-calorimeter (blue) at 5keV.


The situation is even more complicated for the


analysis of WSi2 (Fig. 3), since Si-Kα (1.739 keV) and W-Mα (1.774 keV) are separated by only 35eV.


Thin films of Ta/TaN are used in copper technology  as barrier layers. Fig. 4 shows a microcalorimeter  analysis of two different layer stacks, sample A with  40nm Ta and sample B with 25nm Ta/TaN on TEOS. The spectra were acquired at 4 keV within 10 min. It  can be seen that the excitation volume reaches the  TEOS layer in case of sample B, because Si- and OKα lines are present. This application underlines the  need for high energy resolution because this material


combination could not be separated with standard  EDS equipment.


Figure 3: X-ray spectrum of WSi2.


Comparison of measurements with conventional   Si(Li) - detector (red, counts x10) and µ-calorimeter (blue) at 10keV.


energy/eV


40-20-


OKO


may 0+


Figure 4: X-ray spectra of Ta/TaN films on SiO2 at


100200300400500600


4keV. Sample A: 40 nm Ta (red), Sample B: 25 nm


energy / eV


Ta/TaN (blue, offset: 60 counts).


Besides the problem of chemical identification  geometrical aspects may limit the use of  conventional EDS detectors. Regarding systems of  multilayers, the energy of the primary beam can not  be increased to a certain extent, because the detected  radiation will contain not only the information of the  layer of interest but also of the layers below. Fig. 5  shows the X-ray spectra of a SrBi2Ta2O9 (SBT) / Pt / TiO2 / SiO2 / Si - material stack which is typically  used in ferro-electric devices. At 5keV (a), X-rays  are only emitted from the SBT layer, whereas at 10  keV (b) additionally Pt-peaks appear. All peaks  relevant for identification of  the different elements  occur below 2.6 keV. With a conventional detector


Sr and Ta have to be distinguished by Ta-Lα (8.145  keV) and Sr-Kα (14.14 keV); for this energy of the  primary beam X-ray radiation will also be emitted


from the Pt-layer below and it is not possible to  identify the two separate layers.


250


Tama


200-


100 nm Pt


S150-


Tamp


BinoxSi-substrale 180 mm si9kT2205


election beam


10 0


sra


BikMa


100-


50-


SYLP


150017502000225025002750300000


Figure 5a: X-ray spectra of a multilayer material


stack for ferroelectric devices at 5 keV. The


penetration depth of the primary electron beam is


shown in the inserts (blue: microcalorimeter; red:


conventional Si(Li)-detector, counts x 5).


n30-


0 5


TilaOKa


Figure 5b: X-ray spectra of a multilayer material


20-


stack for ferroelectric devices at 10 keV. The


10-


shown in the inserts. (blue: microcalorimeter; red: 00 conventional Si(Li)-detector, counts x 5).


200300400500600


The investigation of a TiN top layer which seems to  exhibit a wrinkled surface in an optical microscope (Fig 6a) demonstrated that also problems typically  analyzed by Auger electron spectroscopy (AES) can  be solved by the use of the microcalorimeter. By  AFM-analysis it was shown that the observed effect  is not topography related. The surface of the  suspicious sample is as flat as a good one showing no  wrinkles at optical inspection.


Fig 6a: Optical suspicious “wrinkled” TiN surface


The excitation energy was chosen in that way, that  the beam is fully absorbed in the TiN layer and does  not reach the underlying silicon nitride of the  passivation , proven by the absence of the Si-Kα line.


180TaMiC


180 nmSr8i:Ts20


The spectra (Fig. 6b) taken at identical conditions (excitation energy, working distance, take-off angle,


BiMa


625nm S102 10am no 100nm形


etc.) exhibit, as expected, the well separated peaks of


S120


PtMc


Si-substrate


the present elements (Ti, N, O, C).


n100TaMB0


080NPEMB


Biwβ


sruce14,6eV


STLβ


20 ofmatht


十good


1500175020002250250027503000


40 50-


NKa


--bad


Figure 6b: X-ray spectra of TiN


surface layers at 4keV.


Good surface (green, circles), bad surface (red).


Compared to equal heights of the Ti-Lα peak, the


oxygen peak at the “bad” surface is higher than at a “good” reference. This increase of the oxygen


content inside the excited volume may indicate a


thicker oxidized layer on top. This suggestion was  confirmed by additional depth profiles obtained by  AES (Fig. 6c) giving an oxide thickness of ~6nm for  the “bad” and ~3nm for the “good” sample.


Sputter Time /min


Figure 6c: depth profiles of TiN surface layers


(cf Figure 6b) measured with AES.


A well-known example in failure analysis is  illustrated in Fig. 7. An electrical short was measured  in the SRAM block of a 0.25 µm device. The  following preparation by FIB cross-sectioning  brought out a bridge between neighboring metal lines (Fig. 7a).


Figure 7a: FIB cross section of metal short.


A subsequent X-ray analysis of the bridge and a


X105


reference point showed that the defect consists of


3,5


aluminum (Fig 7b).


3,0


TiN


2,5


Ti


人2,0bad s


1,5 u1,0


0,5


Si


u n150


0,0


0 2 4 6 8 10 12 14 16 18


CKX


x105


0+产


02505007501000 1250 1500 1750 2000 50-


0门 S


AlKa


OKX


3,0TiN


人1!2,0goodTi


Figure 7b: X-ray spectra of the defect shown in fig.7a (blue; offset: 100 counts) and a reference point (red)


aO


1,5


at 5keV.


u1,0 0,5


Summary, Conclusion and Outlook


0 2 4 6 8 10 1214 16 18


The implementation of a microcalorimeter for X-ray  spectroscopy in an F/A lab is a revolution in material  analysis. Fast energy dispersive analysis with an  energy resolution comparable to wavelength  dispersive X-ray spectrometers meet all requirements  of failure analysis concerning work flow and quality  of the analytical results. Regarding the count rate of  the detector further improvements are expected by  the implementation of X-ray optics.


Compared to surface analysis methods like AES, the  system does not require UHV conditions, can easily  be installed at a SEM and uses its high spatial  resolution. An additional combination with STEM  option would also allow excellent lateral resolution  of 2-dimensional X-ray mappings. The closed loop  mechanical cooling system requires no handling of  liquid gases and therefore the µ-calorimeter is the  premier choice to improve inline defect  characterization.


H没


Part of this work was funded by the European  Commission in the SEA project MESA (IST-1999-20010). The authors thank Dr. Boit for enabling this


work and R. Schaller for measuring the AES-spectra. The essential contributions of D. Wernicke and K. Phelan in detector and software development are  gratefully acknowledged. Special thanks are given to  EDAX Inc. and D. Redfern for their continuous  engagement throughout the project, their valuable  contributions to a vibrational damped mounting of  the µ-calorimeter to the SEM and especially for  integrating cooler automation routines and data and  refinement procedures into their standard analysis  software GENESIS which makes daily routine work  with this tool now possible.


1. The International Technology Roadmap for


Semiconductors, Semiconductor Industry


Association 2001


2. High Resolution X-Ray Spectroscopy using


Iridium/Gold Phase Transition


Thermometers


J. Höhne, M. Altmann, G. Angloher, P. Hettl,


J. Jochum, T. Nüßle, S. Pfnür, J. Schnagl,


M.L. Sarsa, S. Wänninger, F. v. Feilitzsch,


Proceedings of the European Conference on


Energy Dispersive X-ray Spectrometry 1998


EDXRS-98, edited by J. E. Fernandez and


A. Tartari, ISBN 88-7794-195-2, pp. 77-80


3. High-resolution, energy-dispersive microcalorimeter spectrometer for x-ray microanalysis


D.A. Wollman, K.D. Irwin, G.C. Hilton,  L.L. Dulcie, D.A. Newbury, J.M. Martinis,  J. Microscopy, 188, 196-223 (1997).


4. Microcalorimeter Energy Dispersive X-ray  Spectrometer for Low Voltage Microanalysis  D.A. Wollman, J.M. Martinis, S.W. Nam,  G.C. Hilton, K.D. Irwin, D.A. Rudman,  N.F. Bergren, S. Deiker, M.E. Huber,  D.E. Newbury, Elec. Dev. Fail. Anal. News,  Vol. 2(4), pp.1 (2000)


5. Cryogenic Detector Systems for Materials  Analysis


J. Höhne, U. Hess, M. Bühler, F. v. Feilitzsch,  J. Jochum, R. v. Hentig, T. Hertrich, C. Hollerith, M. Huber, J. Nicolosi, K. Phelan, D. Redfern,


B. Simmnacher, R. Weiland, D. Wernicke


Ninth International Workshop on Low  Temperature Detectors (LTD9): Edited by   F. Scott Porter, Dan McCammon, Massimiliano  Galeazzi and Caroline K. Stahle, AIP  Conference Proceedings, 605, pp. 353 (2002)


6. The Microcalorimeter for Industrial  Applications


D. Redfern, J. Nicolosi, J. Höhne, R. Weiland,  B. Simmnacher and C. Hollerith, NIST-MAS  Workshop (to be published).


A Working Method for adapting the (SEM) Scanning Electron  Microscope to Produce


(STEM) Scanning Transmission Electron Microscope Images


Edward Coyne


Product Analysis, Analog Devices, Limerick, Ireland


This paper describes the problems  encountered and solutions found to the practical  objective of developing an imaging technique that  would produce a more detailed analysis of IC  material structures then a scanning electron  microscope.


To find a solution to this objective the  theoretical idea of converting a standard SEM to  produce a STEM image was developed. This solution  would enable high magnification, material  contrasting, detailed cross sectional analysis of  integrated circuits with an ordinary SEM. This would  provide a practical and cost effective alternative to  Transmission Electron Microscopy (TEM), where  the higher TEM accelerating voltages would  ultimately yield a more detailed cross sectional  image.


An additional advantage, developed  subsequent to STEM imaging was the use of EDX  analysis to perform high-resolution element  identification of IC cross sections. High-resolution  element identification when used in conjunction with  high-resolution STEM images provides an analysis  technique that exceeds the capabilities of  conventional SEM imaging.


The two primary difficulties encountered in  achieving this objective were,


Summary


Salient features of the laser milling tool have been  described. By adjusting the laser parameters, package  milling can be made material specific and with little


material redeposition. Applications of the laser  milling technique described include plastic package  delayering, silicon milling, package x-sectioning and  package decapsulation. The laser milling technique  was found to be able to address many of the  limitations or issues identified with using traditional  DPA methods on current package technologies such  as multiple stacked die packages and  chip scale  packages. As packages become more complex the  laser milling tool is expected to be an integral part of  the failure analysis tool suite.


Acknowledgments


The authors would like to thank Brandon M. Frazier  from Potomac Photonics for providing the feasibility  evaluations on the different package applications  described in this paper.


1. A. Dubotzky , “Evaluation of Alternate  Preparation Methods for Failure Analysis at  Modern Chip and Package Technologies, Conference Proceedings of the 27th ISTFA, 2001,  pp 83-86


2. F. Beaudoin , “ New Laser Ablation Method for  Non Destructive Backside Sample Preparation” Conference Proceedings of ISTFA, 2000 , pp  553-558


3. Institute for Micromanufacturing, “Principles of  UV Laser Ablation Microforming Ststems”,  http://www.latech.edu/tech/engr/ifm/principl.ht


ml


4. G.P. Behrmann and M.T. Duignan, “Excimer  Laser Micromachining for Rapid Fabrication of  Diffractive Optical Elements”, Applied Optics, 36(20), 10 July 1997


5. M. Frazier , “ Laser Based Sample Preparation  for Electronic Package Failure Analysis”, Proceedings of SPIE Vol# 4637: Photon  Processing in Microelectronic and Photonics,  Jan 2002


6. R.Shukla, Flip chip CPU package technology at  Intel: A technology and manufacturing  Overview, 49th Electronic components and  Technology Conference, 1999, pp 945 – 949


Laser Decapsulation of Transfer Molded Plastic Packages for Failure  Analysis


George Carter


Reliability Engineer


Advanced Analog Products  Texas Instruments - Tucson


Decapsulation of plastic packaged components is  frequently necessary for failure analysis or product  development.  Conventional techniques utilize an  acid etch process, which is not compatible with  copper and other acid-sensitive materials.  There is  limited ability to alter etch geometry or selectively  decapsulate individual circuit elements.  Laser  ablation using a raster scanned Nd:YAG laser was  used for selective decapsulation of temperature  sensitive passive components in a PDIP packaged  DC-DC converter.  Copper welds, nylon insulated  ferrite, and polyesterimide insulated magnet wire  were decapsulated without damage, allowing failure  analysis of a miniature transformer and its associated  welded leads.


Device failure analysis frequently requires the  decapsulation of plastic packaged devices for visual  inspection or SEM analysis of components, or for  electrical probing of circuit nodes.  Conventional  techniques utilize hot fuming nitric acid, sulfuric  acid, or a mixture of the two.  A sealed reaction  chamber is created by using an O-ring to isolate the  decapsulation area from the rest of the package.  A  measured volume of acid is applied and recirculated  onto the device for a programmed period of time.  This sequence is repeated until the desired area has  been exposed.  The process cannot be directly  observed, and the end-point must be determined by  trial and error.  Microprocessor controlled equipment  has greatly improved the capability and safety of the  procedure, but ultimate accuracy and repeatability  are limited.  Internal components susceptible to acid  attack are severely damaged or destroyed.  The  geometry of the exposed area is determined by the  size of O-ring used, and cannot be precisely defined.  It is not possible to open areas of irregular shape, or  precisely target individual circuit elements.  For very  small package outlines, special repotting techniques  are required as part of the sample preparation.


Laser ablation has been utilized in various  applications in medicine, engineering, and  instrumental analysis.  Pulsed and continuous wave  lasers have been used in a wide variety of  semiconductor processes for several years.  Various  authors have recently reported on the application of  laser ablation to package decapsulation and device  failure analysis1, 2, 3.


The application of laser ablation to package  decapsulation is straightforward in principle, but  more difficult in practice. The ablation mechanism  itself is highly complex, and is affected dramatically  by material properties as well as multiple process  variables.  The optimal process settings for bulk  ablation of the package may be significantly different  from those required at the device surface.  The mold  compound filler material can create significant  complications due to both optical and physical  effects.   The variation in optical properties between  the various circuit elements can be either a detriment  or an advantage depending on the application; but  with suitable selection of laser wavelength, proper  adjustment of process parameters, and consideration  of material properties laser ablation can be utilized as  an effective and practical decapsulation technique.   Devices can be quickly exposed with no significant  temperature rise in the bulk package.   Acid sensitive  circuit elements such as copper can be exposed with  no visible damage.  Thermally sensitive materials  such as nylon and polyesterimide insulation can be  exposed with minimal evidence of heat stress.  By  the use of optical filters or video equipment, realtime visual monitoring of the ablation process is  feasible.  With suitable ablation chamber design, controlled-atmosphere ablation is possible.  Isolated  circuit elements can be decapsulated by means of  metal masks in the case of single-shot lasers with  areal optics, or by direct-write procedures if the  equipment has  galvanometer driven scan mirrors.


Laser systems with direct write capability offer  significant advantages over single-shot lasers when  sample heating is a critical concern.  In an areal  optics system the entire sample area is exposed to the  laser energy in a single shot.  Consequently the entire


area must simultaneously dissipate any excess heat.  With the energy levels required for rapid package  ablation, sample overheating can become a  significant problem.  With a direct-write laser system  additional adjustment of the timing and spacing of  individual laser pulses and line scans is possible, resulting in better control of package heating during  the ablation process.  The decapsulation reported in  this paper was performed with a 1064 nanometer  marking laser, using an interlaced raster-scanned  ablation pattern. Discussion of the process  optimization requires some preliminary discussion of  the ablation mechanism.


The Ablation Mechanism


There has been considerable discussion in the  literature regarding the operative mechanism or  mechanisms during ablation, due to the high  complexity of the various possible interactions of the  sample with laser light.  Multiple mechanisms can be  detected including simple thermal heating, evaporation, pyrolysis, and photolysis.  However, the  defining mechanism in ablation is the inception of  vigorous mechanical spalling of the sample at the  ablation threshold, accompanied by the physical  ejection of the ablated material.  The decapsulation  technique discussed in this paper is based upon  optimization of the photo-mechanical aspect of the  ablation process4.


The ablation threshold is typically defined as the  threshold fluence (J/cm2) where ablation begins, or  where the ablation rate increases dramatically.  The  observation of a significant change in the visible  ablation plume and an audible report at the ablation  threshold are frequently noted.  The empirical results  reported demonstrate a major change in reaction rate  and/or mechanism at the ablation threshold.  These  observations are a common denominator in the  literature, although there has been considerable  discussion regarding the actual ablation mechanism.


Domankevitz, and Nishioka used a high speed  framing camera to determine the ablation threshold  for fresh tissue samples5.  The onset of ablation was  based on the first visible evidence of an ablation  ejection plume. The photographic sequences  obtained confirmed that the ablation event is  explosive in nature, and not due to simple  vaporization of sample constituents.  These findings  are particularly significant since the samples in  question were elastic biological tissue, and did not  have brittle fracture properties.  The authors also  observed a finite time delay between the start of the


laser pulse and the appearance of the ejection plume.  This delay is commonly reported in the literature, and is due to the finite time required for the sample  to absorb and respond to the transient laser pulse.  A  key factor in optimizing the ablation process is the  ability to input energy into the sample with a  transient pulse which is shorter than the physical  response time of the sample matrix.


A sharp increase in acoustic output at the ablation  threshold is commonly reported in the literature.  This is not a transient phenomenon, but a continuous  one.  At fluences above the ablation threshold, audible sound is produced.  The amplitude and  frequency of the sound are strongly affected by the  pulse width and frequency, as well as the fluence.  Changes in the sound intensity correlate with  changes in the ablation rate.  The explosive ejection  of material from the substrate is an integral part of  the ablation process, and is a defining criteria for the  start of ablation.


Kolomenskii and Hess used a probe-beam-deflection  method to study the surface acoustic waves  generated above and below the ablation threshold6.  They monitored the amplitude and waveforms  generated by 355 nanometer Nd/YAG laser pulses in  undoped polished (111) silicon.  The ablation  threshold was determined to be at a fluence of 1.5  J/cm2.  A linear increase in amplitude was observed  from 0.05-0.2 J/cm2, and the first and second  oscillation of the acoustic pulse had approximately  equal amplitude.  At a little above 0.2 J/cm2 the rate  of increase in the amplitude diminished.  At this  point the amplitude of the first acoustic pulse was  observed to become significantly greater than that of  the second pulse.  When fluence was increased to the


1.5 J/cm2 ablation threshold the acoustic pulse  amplitude increased dramatically, and continued  to  increase with increasing fluence.  Below the ablation  threshold the acoustic signal remained relatively  constant when multiple laser pulses were applied to  the same physical location on the wafer.  But at  fluences above the ablation threshold the acoustic  signal changed significantly with successive laser  pulses.  The authors concluded that there is a  transition from a thermoelastic excitation mechanism  to an ablative excitation mechanism at the ablation  threshold. Profilometer measurements confirmed a  dramatic increase in the depth of surface damage at  the ablation threshold.


The abrupt change in sonic energy at the ablation  threshold indicates a change in mechanical vibration  in the substrate.  As pointed out by Kolomenskii and


Hess, thermoelastic behavior is in effect below the  ablation threshold6.  The laser energy can be  absorbed and dissipated fast enough to avoid  mechanical bond rupture; and the phonons generated  by the cyclic laser pulsing can be detected as sound  waves leaving the substrate surface.  The appearance  of shock waves at the ablation threshold is analogous  to the changes observed when taking a macroscopic  sample beyond the yield limit to the point of brittle  fracture.


Figure 3: Optical image of a mechanically prepared  STEM sample. The visible circuitry on the surface is  about 10-20um wide with the defect site in the  middle.


The primary advantage of this method is that by  using glass slides as the supporting frame, there was  no direct physical handling of the die and hence the  risk of accidental damage was greatly reduced.


Initially the samples were ground  perpendicular to the die surface, however these  samples were structurally unstable with a minimum  thickness of about 50um.  Since only the top 3-5um  of a sample is of interest, it meant that samples could  be ground at an angle relative to the horizontal plane.


An angle of 30 degrees dramatically increased the  sample strength and hence reduced the minimum  thickness achievable.


Unstable


3401V65D010    2001971*0810"


Stable


Figure 4: SEM image comparing a perpendicularly  ground sample to a sample ground at an angle.


FIB (Focused Ion Beam) Preparation


Once the sample was mechanically  prepared, the FIB was used for the final stage to thin  the sample down to electron transparency of  approximately 100nm.


This was achieved by getting the  mechanically prepared sample, which is still  supported by the glass slide and depositing a  Platinum track on top of the defect site in order to  protect it.


Pt Track


Figure 5: Image showing the Platinum track  deposited on the defect site.


Next a trench was cut either side of the Platinum  track leaving a thin wall structure remaining.


Figure 6: Image showing the two trenches cut on


either side of the defect site.


Circuitry: Target area


Finally the wall was cleaned down to electron  transparency. This is best achieved by tilting the  sample at an angle of 2 - 3 degrees relative to the  axis of the beam. This was in order to accommodate  the conical shape of the ion beam and prevent it from  etching the upper surface of the STEM sample.


Lower Detector


Figure 7: Image of an electron transparent STEM


Glass Support


Initial Imaging Procedure


The imaging setup for the Hitachi S-4700  field emission scanning electron microscope consists  of two electrically biased secondary electron  detectors. The upper detector that is located  vertically above the sample and the lower detector  that is located to the side of the sample.


Figure 8: Diagram showing the relative positions of  the upper and lower secondary electron detectors.


Detector sensitivity is a function of sample  working distance. At small working distances, when  the sample is close to the upper detector, it is more  efficient. While at larger working distances the lower  detector is more efficient.


The initial theory for converting the SEM to  produce STEM images was to use the upper detector  at small working distances to focus the electron beam  upon the STEM sample. Then switch to the lower  detector and image the attenuated transmitted  electrons with the lower detector.


e-bcamaxis


STEMSample


e-beam axis


~100nm


20mm


e's


STEM sample


Figure 9: Diagram of the initial theory for producing


STEM images.


This technique was based upon the assumption that


the electrical bias at the lower detector was sufficient


to deflect the attenuated transmitted electrons.


Imaging Results


Producing STEM images with the electrical  bias of the lower detector yielded low intensity  images with limited resolution.


S-4700 30.0kV 7.1mm x25.0k SE(L)


2.00um


Figure 10: STEM image produced with the electrical  bias of the lower detector.


With this image a number of practical observations  can be made which yield information on the physical  processes behind the first STEM imaging technique. Primarily, there is a larger signal from denser


Upper   Detector


Lower   Detector


Working   Distance


materials, while there is limited material resolution  and contrast, and the voids in the material are dark.  Based on these observations it is possible to  conclude that the lower detector was only imaging  the low energy secondary electrons, while a large  amount of energetic transmitted primary electrons  were not being imaged. Therefore the electrical bias  at the lower detector is not sufficient to attract the  transmitted energetic primary electrons


Problem


S-4700 20.0kV 5.2mm x15.0k SE(L)


9.00um


These conclusions were derived from the  image by taking into account of the following  analysis.


When the 30KeV primary electrons are  focused upon the upper surface of the STEM sample, they produce secondary electrons from a small focal  area. When these secondary electrons are imaged  with the upper detector they produce a well-focused  image.


Figure 11: SEM image of a STEM sample taken with  the upper detector. Note that the image has got high  resolution.


However as the primary electrons travel  through the STEM sample, they begin to diverge and  scatter. Therefore, when they emerge from the far  side of the STEM sample, they produce secondary  electrons from a larger focal area.


These secondary electrons are then attracted  to the electrical bias of the lower detector, which  produces images of limited resolution and material  contrast.


S-4700 5.0kV 17.7mm x2.00k SE(L)


20Dum


At this stage it is important to note that the  energetic transmitted primary electrons that contain  the best information are not being imaged and escape  down the SEM chamber undeflected. If a method  could be developed to image these primary electrons, then it would dramatically increase the quality of the  transmission images.


Figure 12: Secondary electron image of a STEM  sample produced with the electrical bias of the lower  detector.


Theoretical Solution


The solution to this problem was found by  placing a 45O metal deflector horizontally across  from the lower detector in the path of the energetic  primary electrons, along the axis of the SEM column. When the primary electrons hit the metal target, they  would produce a quantity of secondary electrons  directly proportional to the magnitude of the incident  beam. Therefore when the primary beam strikes the  STEM sample, it would become attenuated according  to the density distribution of the material across the  sample area. This transmitted attenuated beam then  contains all the information on the material density at  that point. The metal plate then translates this  information into secondary electrons, which can


S-470020kV 53mm x18.Ok SE(u)


3.00um


easily be collected with the lower detector.


Figure 13: Initial attempt to implement the  theoretical solution of converting the transmitted  primary electrons to low energy secondary electrons


This solution is based upon the assumption  that the quantity of secondary electrons is linearly


Secondary electrons


Primary Electrons


proportional to the transmitted primary beam across  the full area of the metal target plane.


With the 45O target at the back of the STEM  sample, two significant problems were encountered. First, it was noticed that the target topography was  superimposed on the STEM image and also, that the  lower detector was not efficient for the small  working distances. However by increasing the  separation between the STEM sample and the metal  target it was possible to solve these two problems.


Figure 15: Diagram showing the relative position of  the metal target to the STEM sample.


This solution worked because the incident  primary electron beam which was focused upon the  upper surface of the STEM sample was out of focus  by the time the attenuated transmitted beam reach  the metal target. Therefore no detail of the metal  target could be superimposed on the STEM image. Also, this larger separation meant that the metal  target was at a more suitable working distance for the  lower detector to image the secondary electrons.


Using this setup higher intensity images  with greater material contrast were observed. In  addition to this the voids in the material were  brighter and there was a relatively weaker signal  from the denser material. This indicated that the  primary electrons were being converted to lower  energy secondary electrons and imaged with the  lower detector. However the images still had limited  resolution.


Figure 16: Image of a STEM sample, where a metal  target was used to convert the primary electrons to  low energy secondary electrons.


Final Problem


The limited resolution that was observed  with this imaging setup was because the lowresolution secondary electrons from the STEM  sample were swamping the secondary electrons from  the metal target. The solution to this problem was to  shield the secondary electrons at the STEM sample  from the lower detector.


Secondary Electrons


Metal


Shield


Figure 16: Diagram showing the position of the  metal shield around the STEM sample. The metal  shield blocked the secondary electrons from the  STEM sample.


This final technique then produces an indirect  scanning transmitted electron image of the sample.


Final Results


Titanium


Aluminium


Tungsten


Figure 17: High resolution STEM images with good  material contrast of a bipolar transistor and contact.


High Resolution EDX Analysis


An additional advantage to STEM cross  sectional imaging is the use of EDX analysis to  perform high-resolution element identification of the  different materials seen across a STEM sample. Conventional EDX analysis is limited in resolution  by the mobile nature of energetic electrons. As  electrons enter a sample they diverge and scatter to  produce x-rays from a larger volume then the actual  spot size of the incident electron beam


X-R ay G eneratio n  V olu m e


Figure 18: Simulation of the x-ray generation volume  for a normal sample at 20KeV.


With a STEM cross-section, the short range of the  sample thickness limits the electron scattering. Therefore, the x-rays produced enable far higher  EDX resolution and material analysis.


Figure 19: EDX elemental analysis of the different  metallic structures seen across a STEM cross section  of a bipolar transistor.


Conclusion


With this project a step by step procedure  for producing and imaging STEM samples with a  standard SEM was developed. The STEM technique  offers an imaging capability that bridges the gap  between the conventional FIB/SEM images and the  detail seen with TEM images. Although the TEM  imaging capability with higher accelerating voltages  ultimately yields more detailed images, STEM  images are very cheap and easily reproduced with a  wide variety of samples.


This imaging technique, when used in  conjunction with high-resolution EDX element  identification, provides an analysis technique that  ultimately exceeds the capabilities of conventional  SEM imaging and in doing so achieves the original  objective of this project.


[1] S. Morris, S. Tatti, E. Black, N. Cickson, H. Mendez, B. Schwiesow, and Ron Pyle, “A  Technique for Preparing TEM Cross Sections to  a Specific Area Using the FIB, 1TSFA, 1991.


[2] D. B. Williams and C. B. Carter, “Transmission Electron Microscopy”, Plenum  Press,


N.Y.


(1996)


Applications of EELS to Semiconductor Devices Failure Analysis by  Using a 300 keV TEM


Jong-Shing Bow*, Wen-Tung Chang, Yun-Ming. Tsou, Hsing-Shuang Chou, and Christ Chiou


United Microelectronics Cooperation, Hsin-Chu, Taiwan, ROC


A 300 keV TEM equipped with an EELS and energy  selected imaging (ESI) system has proven to be a  necessary and powerful analytical tool for R&D and  failure analysis support.  The advantages and the  efficacy of this advanced elemental mapping technique  can be optimized when the TEM is operated correctly.  Variants of ESI, elemental mapping, jump-ratio  mapping, and pre-edge imaging have been adapted to  explore root causes of different type of failures in  semiconductor manufacturing.


The reduction of scale in the semiconductor devices has  made the work of R&D and failure analysis (FA) face  stricter challenges.  Demands on powerful TEM to  reveal fine and complicated structures are becoming  urgent.  Position resolved EELS and elemental mapping  in a TEM with an imaging filter, which was developed  for materials science in 1991,[1, 2] has become an  important routine analysis tool in semiconductor FA  laboratories since 1997.[3]


Conventional TEM images themselves are, from time to  time, unable to identify the failing features definitely.  The combination of conventional TEM and  compositional analysis, have made failing features, both  constitutes and their distribution, more clear. TEM-EELS has been shown to be able to perform  compositional and chemical bonding state analyses of  nano-meter scale,[4, 5] and to be much more sensitive to  light elements, such as C, N, and O, when compared to  TEM-EDS.  These advantages have made EELS a  standard analytical tool for deep sub-micro  semiconductor devices.[5]  The characteristics of EELS  spectra are quite different from those of EDS spectra.  Ionized edges, rather than peaks, of specific elements  are superimposed on a high intensity, decaying  background due to various energy-loss processes.[6]  Thus, the three-window method should be used to  extract the real elemental maps rather than the  one-window method used in EDS.  This technique, which is called energy selected imaging (ESI), can  acquire elemental mappings in TEM mode rather than  traditional STEM mode.  The advantage of elemental  mapping in TEM mode is that data from large numbers  of pixels are collected simultaneously increasing the  data collection efficiency and reducing specimen drift.


As reported by Jacob et al.[7], for EELS analysis, the


specimen thickness of FIB, lift-out prepared TEM  samples has to be about 50 nm, while for conventional  BF imaging is about 100 nm.[7, 8]  The reduction in  specimen thickness has been very operator intensive.  This restriction can be relaxed somehow, if not  completely eliminated, by using a 300 keV TEM instead  of a 200 keV one, widely used in most TEM laboratories, considering the penetration of high energy electrons.  This work takes the advantage of the 300 keV TEM.


Most developments of the ESI technique have focused  on how to accurately subtraction of the background  underneath the ionization edges.[9]  Relatively, very few  people have paid attention to study the effect of TEM  focus conditions on the quality of mapping “images”.  For TEM users, under-focus conditions are used in  bright field (BF) images to underline the boundaries of  phases, and used in high resolution TEM (HREM) images to compensate the spherical aberration of the  objective lenses.  These focus conditions, however,


can’t be adapted for ESI.  The effects of TEM focus  conditions on the quality of elemental maps will be  studied in this work.


The charm of the ESI technique is not restricted to the  three-window method mapping only.  The two-window  method mapping, also called jump-ratio mapping,[10, 11] and pre-edge images alone have shown their own unique  merit in imaging different types of failures in  semiconductor devices.  Applications of these  compositional imaging techniques to solve problems in  the work of R&D and FA in the semiconductor industry  will be explored in this paper.  Artifacts due to specimen  thickness and elemental effect will also be discussed.


TEM samples were prepared by either mechanical  grinding & polishing or focus ion beam (FIB) cutting  and lift-out technique.  TEM observation and analyses  were performed in a Philips TEM, Tecnai 30, operated at  300 keV.  Data of composition analyses of position  resolved and 2D mappings were collected and processed  using a Gatan GIF system, a post-column EELS and  imaging equipment, attached to TEM.[2]


Effect of Focus Condition


It has been generally accepted that an elemental  mapping can be acquired only when the position of the  energy window is correctly set.[9]  But most people have  forgotten to emphasize that a sharp elemental map, especially for tiny phase and phases of trace elements, can be acquired only when correct focus condition is set.  For conventional BF images, the optimum focus  condition is a little under focus so that Fresnel fringes  make boundaries of features clearly visible.  However, this focus condition can not be applied to EELS  mappings.  That means we can’t go directly to acquire  three energy-selected images when we get a clear BF  image.  Because of its low intensity, it is impossible to  focus energy selected images directly.  A focus  condition in the BF image should be related to the best  focus condition the mapping.  Being formed by all  electrons passing through the objective lens aperture, the BF image is high intensity and its intensity change  continuously.  Fresnel fringes are then required to  highlight boundaries of various phases.  A mapping, on  the contrary, has abrupt change in intensity.  Ideally, only the phase contains that specified element has dose  of electrons in the map, and nothing outside the phase.  So, there is no longer requirement for Fresnel fringes to  highlight boundaries.  Under this situation, the in-focus  condition in BF image should be the best focus  condition for the corresponding mapping.   Under or  over focus only makes the elemental map blurred and  should not be used to acquire those energy-selected  images.


Experimental results in our laboratory have proven this  hypothesis.  Figure 1 shows one set of these results.  Figure 1a and 1c are under-focus and in-focus BF  images respectively, Figure 1b and 1d are corresponding  Co-mappings.  The fine structures of barrier layers and  cobalt silicide are visible in Figure 1a but not in Figure  1c.  However, the tip of Co-silicide is blurred in Figure  1b, but visible in Figure 1d.  By using this unique focus  condition, we succeed to map tiny and trace phases, such as a very thin oxide layer at the interface of  tungsten contact and Ti-silicide, reported by  McDonald.[3]


Si-Mapping


The L2,3 edge of elemental silicon is at 99 eV, and shifts  to 106 eV for SiO2.  As it is about 50 eV behind low loss  region, it is a very suitable element for ESI when the  intensity and the pre-edge background are considered.  Because of the high intensity of Si signal, the width of  the energy slit used to select specified energy range to  form elemental maps can be as small as 6 eV.  The shift


of the thresh-hold energy of silicon from elemental state (Si) to oxidized state (Si4+) is about 7 eVs.  As a  consequence, we can distinguish the distribution of Si of  crystallite and amorphous (a-Si) from SiO2 by carefully  setting the position of the energy windows.  A typical  case is shown in Figure 2.  Figure 2 shows a set data of  typical EELS analysis for a defect in a deep trench.  An  abnormal layer between poly 1 and poly 2 was observed  in the BF image (Figure 2a), but the BF image can not  tell exactly what it is.  Position resolved EELS analysis (Figure 2f) indicates that this abnormal layer was a  carbon-rich phase.  Figure 2b clearly displays the  distribution of this carbon-rich phase, between poly 2  and oxide liner as well as poly 2 and poly 1.  Mappings  of elemental Si (Figure 2d) and oxidized Si (Figure 2e) confirm that the distribution of silicon of different  chemical state in semiconductor devices can be  distinguished by the ESI technique.  However, this does  not work for all cases.  Specimen thickness is one of the  key factors.  The TEM specimen used in Figure 2 was  prepared by mechanical grinding and polishing, and had  thinner regions than those prepared by FIB.


Figure 1: Effect of TEM focus conditions on elemental  mappings.  (a) and  (b) are under-focused BF image and  Co-mapping; (c) and (d) are in-focused BF image and  Co-mapping.


Effect of Ti on Si-L Edge Mapping


As mentioned before, the plural scattering is significant  for most FIB prepared TEM specimens.  This effect


causes another puzzle for Si L2,3-edge mappings when  titanium-contained phases are involved.  For deep


sub-micron semiconductor devices, Ti/TiN layers are  widely used as diffusion barrier layers for tungsten  plugs.  Figure 3 shows the results of elemental mappings  for a diffusion contact.  From the Si L2,3-edge mapping (Figure 3b), it was not clear whether there was Si in the  barrier layer or not.  Analyses of position resolved data  and Si K-edge mapping (Figure 3d) indicated that the Si  signal at barrier layer in Figure 3b was an artifact.  Where did these “Si” signals come from?  How did these  Ti-contained phases display as Si-contained phases?


Figure 2:. (a)BF image, (b)C-mapping, (c)O-mapping, (d)Si mapping, (e)Si4+-mapping, (f)EELS spectrum of  circled point in (a).  This sample was prepared by  mechanically grinding and polishing.


In an EELS spectrum, the most commonly used  characteristic edge for Ti is L2,3 edge located at 456 eV.  This edge is 300 eV beyond the Si L2,3 edge.  It is thus  impossible to affect the Si L2,3 edge.  Titanium has outer  cells – M cells.  The characteristic edge of Ti-M2,3 is 30  eV, and M1 is at 60 eV.  These M-edges become  prominent when specimen thickness increases.  The  delay maximum of M1-edge is around 70 eV, the tail of  the M1-edge then makes the slope of the curve of 70 to  99 eV steeper and results in the artifacts in Si-mappings.  To confirm the barrier layers are free of silicon, Si  K-edge mappings, which are not affected by titanium,


characteristic edges were acquired.  The result, shown in  Figure 3d, indicates that there is absolutely no Si in the  barrier layers.  Si K-edge elemental maps were reported  to be less susceptible to the change in chemical bonding  state of silicon.[12]  The intensity change of a Si K-edge  mapping is thus able to correlated to the concentration  variation in the material system analyzed.  The  integrated line profile from A to B labeled in Figure 3d  is displayed in Figure 3e.  The result is as expected.  Si-substrate has the highest concentration, while SiO2  has the lowest concentration among these three  Si-contained phases.


Figure 3: Effect of Ti on Si-L2,3 edge mapping. (a)BF  image, (b) Si-L2,3 mapping, (c ) Ti-L2,3 mapping, (d)Si-K  mapping, (e)intensity profile of Si across SiO2/TiSi2/Si


Pre-Edge Imaging


The contrast of copper is usually very dark in TEM BF  images, making it difficult to outline the profiles of the  barrier layers of Cu-vias and to measure their thickness.  Many TEM workers have tried to use other TEM  imaging techniques to definitely outline the boundaries  of Cu and its barrier layers.  In addition to elemental  distribution, we have found that ESI is also a very  effective technique to draw out the boundaries between


C-K


O-K


Energy Loss


f


TiSi2


Si-sub2


different phases, both compositional and structural. As  shown in Figure 4, the profiles of the barriers are clearly  distinguishable from the Cu vias and trenches.  Moreover, boundaries of SiC, SiN, and layers of low K  materials, which are not visible in the BF image, can all  be clearly observed.  The mechanism of this type image  forming is still under study.  In current work, we only  demonstrate it to be a very simple and effective TEM  imaging technique to outline the barrier layers of Cu  vias.


Figure 4: An oxygen pre-edge image (b) has better  contrast for phases than a traditional BF image (a).


Jump-Ratio Imaging


Electrons are scattered into high angles when they travel  through phases formed by heavy elements.  A typical  heavy element used in semiconductor devices is W (z = 74).  The high angle scattered electrons are blocked and  unable to contribute to the final TEM image.  This effect  results in dark contrast in W plugs in BF images, and in  difficulty with checking filling condition of W plugs by  TEM.  Using the technique of jump-ratio image, we can  very clearly observe the filling of W-plugs.  This  technique was originally designed to enhance the  contrast of elemental mapping and to eliminate the  effect of thickness variation by setting a pre-edge  window and post-edge window,[10, 11] of 20 to 30 eV, usually to acquire two energy-selected images.  The  post-edge image is then divided by the pre-edge image.  For a specified element, the post-edge image contains  this element, but the pre-edge image does not.  Therefore the jump-ratio image shows high contrast for  this specific element.


In this experiment, we have modified some operating  parameters.  First, the energy window was set to be only  6 eV.  Secondly, the window was set at zero-loss peak  and plasmon peak rather than before and behind a  characteristic edge of a specified element.  By dividing  the plasmon image into the zero loss image, we obtain a  ratio image as shown in Figure 5.  For regions in a phase, such as inside the W-plug, the change in intensity stands  for the variation in thickness.  The intensity of the  plasmon increases with specimen thickness.  The darker


regions then stand for the thinner regions where  plasmon intensity are low.  For regions of different  phases, this simple relationship no longer holds due to  the different electron scattering power of different kinds  of atoms.


Figure 5: Ratio image displays the void in the W-contact  clearly.


As the size of microelectronic devices continuously  shrinks, the work of failure analysis (FA) faces more  challenges.  TEM cannot definitely identify abnormal  phases by using BF images only.  New TEM techniques  have been developed to overcome this problem.  TEM  work in our laboratory has proven that energy selected  imaging and its variants are very effective modern TEM  techniques to solve most problems encountered in deep  sub-micro semiconductor devices.  We predict that these  techniques should work well for nano-scale  semiconductor devices too, because the resolution of


Void


Via


TEM is close to atomic scale.


This work was performed in 2001 ~ 2002 at United  Microelectronics Cooperation (UMC), Hsin-Chu, Taiwan, ROC.  The authors would like to thank the  company for permission to publish these data and the  financial support.


1. R.D. Leapman and J.A. Hunt,  Proc. Annual  Meeting of EMSA, 49, 8-9 (1991)


2. O.L. Krivanek, A.J. Gubbens, N. Dellby, and C.E. Meyer, Proc. Annual Meeting of EMSA, 50, 1192-1193 (1992)


3. R.C. McDonald, A. J. Mardinly, D.W. Susnitzky, Proc. Annual Meeting of MSA, 55, 449-450 (1997)


4. D. A. Muller, T. Sorsch, S. Moccio, F.H. Baumann, K. Evans-Lutterodt, and G. Timp, Let. of Nature, 758-761 (1999)


5. Y. Mitsui, F. Yano, Y. Nakamura, K. Kimoto, T. Hasegawa, S. Kimura, and K. Asayama, IEDM  Technical Digest, 329-332 (1998)


6. R.F. Egerton, Electron Energy-Loss Spectroscopy  in the Electron Microscope, p 194, Plenum Press, New York (1996)


7. P. Jacob, A. Schertel, L. Peto, and G. Sundaram, Proc. of 7th IPFA, 69-72, (1999)


8. T.T. Sheng, G.P.Goh, C.H.Tung, John L.F. Wang, and J.K. Cheng, Proc. of 6th IPFA, 92-96, (1997)


9. R.F. Egerton, Electron Energy-Loss Spectroscopy  in the Electron Microscope, p 113, Plenum Press, New York (1996)


10. J. Bentley and E.A. Kenik, Proc. Annual Meeting of  MSA, 52, 1000-1001 (1994)


11. J. Bentley, N.D. Evans and E.A. Kenik, Proc. Annual Meeting of MSA, 55, 975-976 (1997)


12. D.W. McComb, R.S. Payne, P.L. Hansen, and R. Brydson, Annual Meeting of EMSA, 50, 1258-1259 (1992)


(a)


To develop a quick and simple  method for sample preparation.


(b) To adapt the SEM which was  designed for the purpose of  producing a scanning electron  image to receive the electrons from  a transmitted signal and convert  them into a meaningful image.


Sample Preparation


The transmission capability of a material  sample is dependent on the incident energy of the  electrons, the thickness of the sample and density of


the material. The maximum accelerating voltage of  the SEM is 30KV and in order to achieve electron  transparency, it was necessary to thin the sample to  the order of ~100nm. Although there is a wellestablished method for sample preparation with TEM  analysis, an alternative method had to be developed  for STEM analysis because the support mechanism, loading method and detector setup were all unique  for the different machines. The method for achieving  this sample thickness had to be quick, simple and  easily reproduced with a wide variety of samples  while minimising the risk of damage during  preparation. Also, the setup for supporting the  sample had to enable the transmitted electrons to  escape and reach a detector with minimal difficulty. To solve these problems it was necessary to  start with the standard two-step process of first  mechanically grinding the sample to about 10-20um  and then using the FIB to thin the sample down to  electron transparency of around 100nm. However, in  addition to this, other techniques were developed in  order to minimise structural weakness, physical  handling, cost and time.


Mechanical Preparation


The initial method used for mechanical  preparation involved attaching a die where the defect  site had been identified to a glass slide with a twopart mixture of super epoxy resin. A glass slide was  chosen as the supporting mechanism because its  transparency enabled accurate positioning and  grinding, while the rigid support it offered could also  be cut and ground at the same rate as the Silicon die.


Figure 1: Image of a die attached to a glass slide with  a two-part mixture of super epoxy resin


Next the excess parts of the glass were removed and  the sample was ground from one direction to within  10um of the defect site.


Figure 2: Optical image of the sample attached with  superglue to the grinding stub. This adhesive can  simply be dissolved in acetone.


The sample was then placed on a second glass slide, and similarly ground down from the other direction  until it was within 10um of the defect site. Finally the  remaining section of the sample was approximately  10-20um in thickness with the defect site located in  the middle.


Current methods used for package level destructive  physical analysis (DPA) such as chemical and  mechanical decapsulation methods, reactive ion  etching (RIE) and diamond saw x-section methods   could potentially result in artifacts such as die  cracking, delamination or corrosion when used on   complex packaging technologies such as multiple  thin die stacked packages with combination of flip  chip and wire bond interconnections. Many of the  shortcoming of these ubiquitous DPA tools are being  addressed by a laser milling approach to DPA. The  system described in this paper consists of a   ultraviolet (UV) laser used for local micromachining  or milling to access package internal features and a  near infrared(IR) laser used for precise soldering of  fine wires to enable testing and fault isolation.  Applications of the laser milling tool described in the  paper are 1) Delayering of multilayer printed circuit  board (PCB) substrates to expose internal metal  traces  so that they can be tested to fault isolate the  failure without loosing electrical functionality of the  product. 2)  Silicon milling to expose flip chip  interconnections. 3) Package cross sectioning and 4) Plastic package decapsulation.


Current methods used for package level destructive  physical analysis (DPA) often have severe limitations  when used on complex packaging technologies such  as chip scale and wafer level packaging, stacked  packages, multiple thin die stacked packages with  combination of flip chip and wire bond  interconnections, flex tape packages etc. DPA  methods such as diamond saws for x-sectioning , reactive ion etching (RIE) and chemical  decapsulation for exposure of package internal  features and mechanical techniques for disassembly  could potentially result in artifacts such as  die/package cracking, delamination or cracking of  internal layers or interconnections, overetching /corrosion effects, etc. Moreover, some of these  techniques, destroy electrical functionality of the  device and prevent any further fault isolation. Many  of the shortcoming of these ubiquitous DPA tools are  being addressed by a laser milling approach to DPA  and described in this paper.


Feasibility of laser based methods such as Ultraviolet (UV) laser ablation for package decapsulation [1] and backside sample preparation [2] for failure  analysis have been published where lasers are  optimized for only one application. In this paper, a  state of the art laser micro-milling system is  described that has the ability to selectively and  locally remove a variety of materials to enable access  to internal package and device features such as metal  traces, via, flip chip/wire bonds and die thin films.


Principle of UV laser ablation


The ultra violet range of 100 to 400 nm wavelength  is a small portion of the electromagnetic spectrum. Common UV lasers are Excimer lasers, argon ion  lasers , Nd:YAG lasers etc. The laser ablation  phenomenon is still not completely understood  as it  occurs within 10 to 100 nanoseconds [3].  The  process of laser ablation involves removal of material  from sample surface and has an important parameter  called  threshold fluence. Fluence is the laser pulse  energy per unit area. When the laser fluence is below   a threshold value, no noticeable ablation occurs. When the laser fluence is gradually increased, an  acoustic signal is generated  when the ablation  threshold is reached and signals the start of the  ablation process. The laser ablation creates numerous  fragmented molecular products from the surface of  the sample. The threshold fluence for a sample  depends mainly on the  material structure and  absorption coefficient of the sample. At laser  fluences just above the threshold, the ablation rate  increases logarithmically with laser fluence(F) as  shown in the equation (1). below where (d) is the  ablation rate and (Fth) is the threshold fluence for the  sample material being ablated.








≈


Fth F


ln


Equation 1. Ablation rate as a function of laser  fluence above the threshold.


With increase in laser fluence, the ablation rate  changes from a logarithmic to a linear rate above a  characteristics fluence (Fo) as shown in equation 2.


Rajen Dias, Lars Skoglund, Zhiyong Wang


Assembly Technology Development  Quality and Reliability  Intel Corporation, Chandler , Arizona, USA


F


Equation 2. Ablation rate as a function of laser  fluence above the characteristic fluence (Fo).


The absorption of laser radiation into the sample  leads to a temperature rise in the sample. At fluences  below the threshold fluence, the temperature rise is  directly proportional to the fluence , but at fluences  above the threshold fluence, the temperature rise is  considerably slower [3].


Since laser milling needs high laser fluence energy, usually only Excimer lasers are used especially for  hard materials. For softer materials such as polymers, argon ion lasers can also be used.  Commercial  Excimer lasers are a family of pulsed lasers operating   in the wavelengths of  193, 248, 308 and 351 nm. The source of the laser emission is a fast electrical  discharge in a high pressure mixture of a rare gas (krypton, argon or xenon) and a halogen gas (fluorine  or hydrogen chloride).  The particular combination of  rare gas and halogen gas determine the Excimer laser  wavelength. The UV laser ablation process is  dependant on the laser variables used and the   material properties of the sample being ablated. Important laser system parameters are laser  wavelength, laser spot size, laser pulse energy, laser  pulse duration and frequency. Material properties  that have a major influence are material bonding  energies, conductivity, and the laser absorption  coefficient of the material.


Laser Milling System


The laser milling system used  to develop methods  for package failure analysis was a  commercially  available Laser Micromachining system  made by  Potomac Photonics[4]. The system is comprised of a   Ultraviolet (UV) range laser used for local  micromachining or milling of PCB and cerami  packages to access package internal features. The  system can also be adapted to include another laser  in the near infrared (IR) range for precise soldering  of fine wires to package features to enable  testing  and fault isolation [5]. The system also contains   beam delivery optics, a scanning head to raster the  laser beam over a selected area on the package, computer controlled stages, and application-specific  software. The system accepts computer aided designs (CAD) inputs, so delayering can be confined to the  region immediately around a fault, as opposed to  Reactive Ion Etching (RIE) where, unless complex  masks are used, the delayering becomes global. It


also contains coaxial optics which allow in-situ  vision feedback during the milling process. The UV  laser beam spot size, laser fluence and beam  repetition rate can be varied in-situ to control the  milling rate. Small spot size with low laser fluence is  used for fine milling or delayering when  micron  level resolution is needed and large spot size with  high laser fluence is used when coarse milling or  cutting of package for cross section analysis is  required.


Since each material in the package has a unique laser  fluence threshold for ablation,  in-situ adjustment of  the laser fluence can be used to make the delayering  process either material selective or non-selective, allowing preservation of metal traces within a  package or penetration through metal to access  deeper buried features. The ablated material is  removed by an air or nitrogen gas flow and  redeposition of the ablated material is minimal.


Laser Milling Applications in Package  Failure Analysis


Laser milling procedures were developed for several  different applications in package failure analysis and  the results compare with traditional DPA techniques  used.  The applications evaluated and described in  detail in this section were delayering of a multilayer  PCB substrate, Silicon milling, Package cross  sectioning and plastic package decapsulation.


Plastic Package Delayering


The primary purpose of delayering a multilayer PCB  substrate is to expose internal  metal traces  so that  they can be tested to fault isolate the failure without  loosing electrical functionality of the  product. The  traditional DPA method is using Reactive ion etching (RIE) to remove PCB materials above and below the  metal traces.  RIE has two major limitations. Firstly, RIE is a global process, forcing the operator to  remove a complete package layer unless unique  masks are used. Secondly,  commercial RIE systems  are not usually capable of penetrating planar metal  layers without the addition of hazardous gases such  as chlorine. This makes investigation under metal  layers very difficult by the RIE technique. Package  planar grindback is the other commonly used method  of delayering but it results in loss of electrical  functionality of the product and is not very effective  when the packages are warped.


A laser milling method was developed to expose  copper traces in a multi layer PCB land grid array


package [6]. The laser fluence thresholds to remove  only the solder mask and PCB dielectric material was  first determined. With a laser spot size of 30  microns, the solder mask and PCB dielectric layer  removal rate of 1-2 micron per laser pass was  achieved. Removal rates of 5 to 12 microns have also  been demonstrated with larger  laser spot sizes.  Figure 1 shows laser milling done on an PCB  package surface to remove the solder resist material  and expose the top metallization layer. With proper  choice of the laser fluence, copper traces at multiple  layers are not affected when the dielectric layers are  removed. Figure 2 shows laser milling done to  various layers in the PCB package substrate. In cases  where it is desirable to remove a metal layer such as  a power or ground plane to expose metal traces  below the plane, the laser fluence is increased so that  the copper plane can be ablated. Once the copper  plane is ablated, the laser fluence is reduced to  remove the dielectric layer below the plane and  expose the underlying copper traces. Material  removal occurs only in areas where the laser scans  the sample and hence local areas in the package can  be exposed without the need to do global delayering  which may alter the residual stress in the package  and result in package artifacts such as cracking or  delamination.


Figure 1. Surface of the PCB substrate with laser  milled areas where the solder resist material has been  removed to expose the copper trace lines.


With the added capability of package CAD inputs, in-situ optical vision and Z depth focus control of the  laser, the analyst can precisely control the delayering  process to expose any buried feature or defect. With  the ability to selectivity remove only certain  materials it is possible to expose defects such as  metal migration and corrosion by-products for  further material analysis by  scanning  electron  microscopy ( SEM) or surface analysis techniques


Figure 2  Surface of the PCB substrate showing areas  where the laser delayering was done to different  depths into the substrate to expose interconnections  at the various layers.


Silicon Milling


Laser milling of die is possible by adjusting the laser  fluence to ablate Si. Pockets as small as 100 microns  square have been made on the die backside of flip  chip packages and the Si milled through the whole  die thickness of 750 microns without resulting in any  die cracking or chipping. Figure 3 shows laser  pockets milled on die backside surface of a flip chip  package. The laser energy was varied for each pocket  to understand the effect of fluence on the surface  roughness of the silicon. This technique can be used  to expose flip chip interconnections from the  backside of the die when there is a need to confirm  package level failures. Figure 4 shows a flip chip die  surface where the silicon has been milled away  completely at a die corner to expose the flip chip  interconnections.


The depth of milling can be controlled by removing a  specific amount of Si, monitoring the axial (Z) focus  of the laser or by in-situ visual feedback. Typically  the laser fluence is adjusted to rapidly remove 15-25  microns per laser pass through 90% of the die  thickness and then to reduce the laser fluence for fine  milling at 1-3 microns per pass to improve the  surface finish.  Figure 5 shows the flip chip package  with a laser pocket cut through the silicon and into  the package substrate. With the advent of low  dielectric constant (K) and ultra low K dielectrics in  Si, this silicon milling technique will have additional  applications.


Figure 3.  Surface of a flip chip package showing  square pockets made in the silicon with different  laser fluences.


Figure 4. Silicon on die backside of a flip chip unit  was milled away to expose the flip chip bump  interconnections made to the package substrate.


Figure 5. Silicon backside of a flip chip package  showing a laser milled pocket through the silicon  thickness and into the package substrate.


Package Cross Sectioning


Complete package cross-section analysis is typically  used in failure analysis to access buried defects such  as delamination, cracks and interconnect failures to  fully understand the root cause of a failure. Diamond  impregnated saws are  traditional used to cut the  package.  Mechanical drilling using milling bits and  grinding methods can also be used.


Package sectioning is also possible with the laser  milling system and results have shown that the cut  kerf widths and quality of cut can be much better  than traditional diamond saw cutting. In the x-section  mode, the laser parameters are typically set to a large  spot size and high laser fluence to cut through the  silicon die and the glass fiber reinforcement in the  substrate. For a typical PCB package with a 1mm  thick fiber reinforced substrate, the cut kerf widths  were approximately 50µm. Figure 6 shows a flip chip  package cut in half with no evidence of any die  chipping. Cuts can be made within 5µm (in X and Y  axes) of the defect region if desired. Removal rates  in the cross-section mode were as high as 100µm per  laser pass and the total cutting time for a package  was less than 10 minutes. Figure 7 shows the xsection interface of the laser cut flip chip unit. There  is no evidence of any die chipping or cracking and  features in the plastic substrate can be seen.


Figure 6 . Flip chip package x-section using laser  milling.


Figure 7  Laser mill x-section image of  a flip chip  unit.


After the x-sectioning, the two halves can be rotated  by 90 degrees to expose the x-section interfaces for  further laser milling using the delayering laser  conditions to polish the surface to a micron finish. The x-section surfaces can also delayered or  micromachined at 1-2µm per pass to expose the  defect or feature being investigated. Figure 8 shows a  x-section of an PCB pinned package where the  through hole was cut in half and part of the through  hole metallization was removed to simulate a high  resistance connection. Laser milling of the x-section  surface was done to improve the surface finish.


Figure 8. Laser x-section through a  through hole.


One major advantage of the laser process is that it  can be used to cut the package in any pattern and not  just a straight cut as in the diamond saw process. This capability allows the analyst to cut along a  feature such as a package trace, even if the trace  bends, in order to view multiple via connections  associated with the trace. In addition, package  delayering can be combined with sectioning for a  variety of application in stacked packages or, multi  die stacked package where local cutting and  delayering may be needed to minimize change in  package residual stressed or to preserve electrical  functionality of some of the components. Another  advantage of the laser cutting process is that it is a  dry process and not involve any lubricants as needed  in the saw process. Hence , minimum sample  preparation is needed to image the cross sections  units in SEM.


Plastic Package Decapsulation


Package decapsulation is usually done on plastic  molded packages to remove the molding material  over the die and wire bond interconnections so that  device and interconnect FA can be done. The  traditional decapsulation methods use wet etching  techniques. The wet etching techniques normally  require use of gaskets to define the area to be etched. While the wet etch technique is well established for  single die molded packages, over etching problems  can be encountered when decapsulating multiple  stacked die packages. Moreover, the global removal  of the molding compound can alter the package  residual stresses and lead to package artifacts such as  delamination and cracking.


Package decapsulation by the laser milling process   provides a dry method of removing the molding  compound. The laser parameters can be adjusted so  that the milling process can selectively remove only  the molding compound and not affect the wirebond  interconnections, the die surface or the package  substrate leads. Figure 9 shows a decapsulated  wirebonded plastic package where the laser milling  process was stopped once the wirebonds were  exposed.  The laser parameters are then adjusted for  fine milling till the die surface is exposed as shown  in figure 10.  Molding material under the wirebonds  are shadowed by the wirebonds but can be removed  by tilting the unit are rescanning the laser beam.


The use of laser milling as a method to decapsulate  the package has many advantages over standard wet  etch methods especially when it  comes to  decapsulation of multi-die stacked packages


Figure 9.  Laser decapsulation of a molded package  to expose the gold wirebonds.


Figure 10. Laser decapsulation of a molded package  to expose the wirebonds and the die surface.


In comparison to wet etch methods, the laser milling  process has more control in the amount of material  removed, and since no aqueous chemicals are used, overetching and corrosion can be prevented. Moreover, by patterning any shape for the laser  raster scan, the milling can be made to expose  multiple levels of wirebonds either locally on any die  location or globally to expose the die or dice. A stair  case type of milling can also be done to expose all  wire bond connections in multiple stacked die  packages. In multiple stacked die packages, the  milling can  also be used to expose any die surface or  region of a die surface by locally milling off all  material above that the specific die. Figure 11 shows  local decapsulation on one edge of the die to expose  the wirebonds. The procedure takes less than a


minute to do and can be  used to inspect a suspect  bonding defect without decapsulating the whole unit.


Figure 11. Local Laser decapsulation of the molding  material to expose gold wire bonds on one edge of  the die.


The laser decapsulation method overcomes several  limitations of the traditional planar grindback  technique used to remove top die in order to expose  the bottom die. For example, grindback becomes  extremely difficult if there is appreciable warpage in  the package or when there is die tilt. These problems  in grindback become more prominent when the   number of die increase or when the die thickness  decreases.


Future Developments


Laser milling tool applications described above use  an UV laser. The tool can also be adapted with a  separate IR laser that can be used for precise  soldering of fine wires to package features or to  easily cut metal lines[5]. This added capability will  allow the failure analyst to fault isolate a defect  within the package without completely destroying the  functionality of the device. Potential application also  include edit and rework capability during product  development.


Rimini discusses the extreme mechanical stress  which can be generated by pulsed laser operation7.  Enormous power densities can be generated by a  sufficiently short-pulsed laser.  Power can be further  concentrated by reducing the laser spot size.  With  the pulse width and spot size used for decapsulation, each 0.1 mJ pulse is delivered at an ultimate power  density of over one megawatt/cm2.  Tremendous  transient thermal gradients are created in the  immediate vicinity of the laser pulse. The substrate  lattice begins to expand, but is “inertially confined” in the plane of the substrate.  It can expand more  freely in the immediate vicinity of the surface, perpendicular to the plane of the surface. This  generates severe anisotropic strain in the lattice.  During each pulse, high compressive forces are  generated as heating occurs.  Between the pulses, cooling occurs and tensile forces are generated.  As  laser fluence is increased at a constant pulse width, a  transient power level is ultimately reached sufficient  to initiate ablation.  At this point the substrate matrix  is no longer able to dissipate the energy fast enough  to avoid mechanical bond rupture.  Brittle fracture  abruptly begins to occur, and the sonic output  transitions from sound waves to shock waves.


It can be seen that the ablation process is  characterized by a significant mechanical component  in the ablation mechanism.  This has been referred to  as a photo-mechanical mechanism4.  The effect of  this mechanism is dramatically visible in samples  with brittle fracture bulk properties, such as transfer  molded microelectronic packages.  At the ablation  threshold a powdery residue abruptly begins to  appear on the sample.  The quantity increases in  proportion to the ablation rate.  Upon microscopic  inspection this powder is found to consist of minute  particles which have spalled from the substrate  surface.  The particle surfaces exhibit typical brittle  fracture appearance.  The inception of rapid


mechanical ablation at the ablation threshold cannot  be adequately explained by direct photo-chemical or  photo-thermal bond degradation alone4.  On the other  hand, photonic and thermal bond degradation are  obvious contributing factors to the photo-mechanical  ablation mechanism.


The optimization of the ablation process for package  decapsulation is based on maximizing the photomechanical aspects of the ablation mechanism, while  minimizing reactions involving epoxy photolysis or  pyrolysis.  This was accomplished by adjustment of  the laser fluence in conjunction with the temporal  and spatial  properties of a raster scanned ablation  pattern.


Experimental Results


The particular application discussed in this paper is  the decapsulation of a transfer molded PDIP device.  Passive components in this device include a  miniature ferrite transformer with welded leads.  The  copper transformer wire is insulated with a  temperature resistant polyesterimide.  The nylon  insulation on the ferrite core has a melting point of  approximately 180 oC.  Initial failure analysis  confirmed open windings, but the defect location  could not be identified by x-ray.  Conventional acid  etch decapsulation could not be used due to the  copper windings and lead frame.  Laser ablation was  used to expose the transformer windings and weld  sites in order to determine root cause of the open  circuit.  The nylon and polyesterimide insulation, and


the welded 40 gage wires were exposed without  damage, as shown in Figure 1.


Figure 1: PDIP device opened by laser decapsulation.


The open circuit defect in this particular device was  located in the coil windings, as shown by the SEM  photo in Figure 2.


Figure 2: coil defects exposed by laser decapsulation.


The surfaces exposed at the copper wire breaks were  not visibly altered during the laser decapsulation.  In  contrast, conventional acid etch decapsulation totally  destroyed the transformer windings.


Equipment Used


The equipment used was a TSI 4005 laser marking  system, which uses a Lee Laser Series 800 lamppumped Q-switched Nd:YAG laser operating at 1064  nanometers.  This laser can be operated at 1 k Hz to  50 k Hz frequencies at a maximum average power of  25 watts.  The pulse width at the 20 k Hz Q-switch  frequency used is approximately 220 n sec, with a  rated pulse energy of 0.96 mJ.  The peak pulse power  under these conditions is rated at 6 kW at 100% output.  The ablation experiments were performed at  various power settings below the maximum rated  power.  Although all experiments were performed  with the system calibrated at 25 watts average power  output, the actual output at reduced program settings  is not precisely known.  Programmed power is set as  a percentage of the calibrated average power.  Good  bulk package ablation results were obtained over a  wide range of power settings.  The power required  was affected by the pulse and line spacing used in the  ablation pattern.  Some of the best results were  achieved with pulse and line spacing that allowed an  11% power setting.  The pulse energy is estimated to  be on the order of 0.1 mJ at this setting.  The fluence  is estimated to be on the order of 0.4 J/cm2.


Being designed as a laser marking system, the  equipment uses galvanometer driven mirrors to scan  the beam in the desired pattern.  Autocad was used to  create a simple raster scan over the desired ablation  area.  This consisted of a series of uniformly spaced  lines in a rectangular pattern.  The center-to-center


line spacing was adjusted by means of the Autocad  drawing.  The overlap of sequential pulses was  adjusted by the means of the marking program.  In  this way both the spatial and temporal  aspects of the  raster scan, as well as the actual laser power settings  could be adjusted.  This was a key factor in achieving  the results.


Process Optimization


Avoiding excessive temperature rise was a primary  consideration during process optimization.  With a  melting point of approximately 180 oC, the nylon  core insulation is easily damaged. Even microscopic  exposure of the ferrite core resulted in severe  package overheating due to the high absorption  coefficient of the ferrite at the 1064 nanometer laser  wavelength.  Although more temperature resistant, the polyesterimide wire insulation is also easily  damaged by the laser settings typically used for  device marking.  Initial ablation experiments resulted  in severe package overheating, and catastrophic  damage to both the nylon and polyesterimide  insulation.


Bulk package heating could be reduced somewhat by  simply lowering the laser energy, but could not be  eliminated while maintaining consistent ablation  quality at an acceptable decapsulation rate.  Package  temperature was observed to rise at an increasingly  rapid rate as multiple ablation scans were performed.  However, thermal damage to the nylon insulation  could be virtually eliminated by allowing the sample  to return to room temperature between subsequent  scans.  This was not a practical alternative, but did  indicate that dissipation of collateral heating was a  major factor.


A rectangular raster scanned ablation pattern was  created, consisting of an array of equally spaced line  scans. Each line was made up of overlapping laser  pulses.  With coordinated adjustment of both pulse  and line overlap, the ablation rate as well as the  temperature rise of the device could be adjusted over  a significant range, even though laser settings were  held constant.  By optimizing pulse and line overlap  in conjunction with laser parameters, a process  window was identified which yielded high ablation  rates with minimum package heating.  The best  results were obtained with an interlaced raster scan, which maximized the time for cooling between  successive passes.  The uniformity of the ablation  was also affected by these adjustments.  The ultimate  laser settings and ablation pattern produced rapid  uniform planar ablation with minimal package


temperature rise.  A 14 lead PDIP device could be  decapsulated to the level of the leadframe in  approximately ninety seconds.  The package was  only slightly warm to the touch immediately after  decapsulation.


Figure 3 is a close up view of a decapsulated  transformer.  The nylon core insulation and the  polyesterimide wire insulation are undamaged.  The  particulates visible on the windings in the upper right  section of the photo are residue from the ablation  process.


Figure 3: nylon insulated ferrite core and


polyesterimide insulated 40 gage copper wire


decapsulated by laser ablation.


Figure 4 is a photo of a wirebonded diode from the  same device.  A noticeable coating of dusty residue  from the ablation process is visible on the surface of  the diode.  The 1.2 mil gold wire and the aluminum  diode metallization are undamaged.  Diode  metallization is relatively thick.  Decapsulation of  integrated circuits with more delicate features is  much more difficult due to complications created by  the molding compound filler material.


Process Complications


Although homogeneous on a macroscopic scale, the  microscopic composition of the molding compound  varies considerably.  The epoxy is highly loaded with  silica filler material.  Variations in filler shape, size, and optical properties cause variations in the ablation  process from point to point within the package.  This  causes minor complications during bulk  decapsulation, but can create serious problems when  trying to expose the surface of a delicate integrated  circuit.


Figure 4: diode decapsulated by laser ablation.


The molding compound in this particular study was a  novalac epoxy with silica filler.  Both angular flake  and spherical particles are used.  Some particles are  translucent while others are optically clear.  The  specified particle size spans a 9X range in diameter  from nominal to maximum.  But empirical  measurements confirmed an extended upper tail to  the particle size distribution.  The largest silica flake  had a diameter of over 15x that of the nominal  spherical particles.  The wide range in particle size  and shape created multiple complications during  decapsulation.


The process settings were adjusted to achieve  ablation of the interstitial epoxy with no evidence of  ablation of the filler particles.  Energy levels high  enough to ablate the silica filler will ablate the die  when it is exposed, and will also cause severe  overheating during bulk decapsulation.  Acceptable  results required adjustment of the process to achieve  vigorous ablation of the interstitial epoxy, with a  spall diameter sufficiently large to dislodge the  largest filler particles.  This was accomplished by  coordinated adjustment of the laser and scan  parameters as described above.  Marginal ablation  settings will leave residual filler particles, which can  cause problems due to either dispersion or focusing  of the laser energy.


When ablation is marginal, any dispersion of the  laser beam by the filler particles can result in conical  pillars or stalagmites of residual material.  Figure 5  illustrates this problem.


Figure 5: stalagmite caused by molding compound  filler particles and marginal ablation settings.


A vertically oriented silica flake can be seen  embedded in the top of the column of residual  molding compound.  The edge of the flake is visible  in the photo as a thin white line at the apex of the  column.  Only the outer edge of the flake is exposed.  This has dispersed the laser beam, reducing the  ablation energy in the vicinity of the flake.  The high  aspect ratio of the flake and the vertical orientation  prevented it from being dislodged during ablation.  Similar beam dispersion problems are encountered  when exposing the wirebonds, as shown in Figure 6.


In this photo the die has been tilted so that the  wirebond loops are in focus.  The ball bond is on the  left side.  Large filler particles are visible protruding  from  the residual molding compound under the wire  loops.  Particles of this size are present throughout  the bulk of the epoxy.  The process settings were  adequate for bulk ablation, but beam dispersion by  the bond wires prevented ablation below the wire  loops.


In addition to complications due to beam dispersion, the filler particles can cause problems with beam  focusing.  This is insignificant during bulk ablation, but becomes critical when the surface of the die is  reached.  Figure 7 shows a clear filler particle in  intimate contact with the die surface.  The large  particle at the upper right of the photo is acting like a  micro-lens.  The camera was focused at the plane of  the die, which can be seen through the middle of the  particle.  During ablation such particles can focus the  laser beam to a smaller spot size, resulting in


unexpected hot spots.  Most particles have a thin   film of molding compound separating them from the


Figure 6: residual molding compound under bond


wires due to dispersion effects.


die surface, and can be removed without damaging  the die.  But particles in intimate contact with the die  are a major complication when decapsulation of a  delicate IC is required.


Figure 7: a large clear silica filler particle in intimate  contact with the die surface, acting as a micro-lens.


As previously mentioned, photo-thermal and photochemical bond rupture also occur during ablation.  Volatile species are generated which can condense  on the sample.  The black coating which results can  significantly affect the ablation process, causing  increased problems with stalagmites and overheating.


Condensation can be minimized by optimizing the  rate of photo-mechanical ablation.  The laser power  may need to be either increased or decreased  depending on the position in the process window.  At  high fluence the ablation rate begins to decrease  because of increasing beam blockage by the ablation  plume; but the rate of photo-thermal bond rupture at  the molecular level continues to increase with  increasing power.  Condensation increases rapidly  with increasing fluence at the upper limit of the  process window, and a reduction in power is  necessary.  At the lower limit of the ablation window, a power increase is needed to increase the photomechanical ablation rate relative to molecular bond  rupture.  A decrease in pulse overlap may also be  required to eliminate condensation.


In Figure 8 a composite photo is shown illustrating  the effect of pulse overlap on condensation.  Three  sets of individual scan lines are shown, each having  an increasing amount of pulse overlap.  The laser  settings used were at the lower limit of the ablation  window, and required physical pulse overlap to  sustain consistent ablation.  The same laser settings  were used for all three groups.  In the upper group  the pulse overlap was just sufficient to produce mild  ablation.  There was minimal spalling action, and  ablation was limited to the interstitial epoxy.  The  ablated surface is very light in color, with no  evidence of excessive temperature.  In the middle  group the center-to-center pulse spacing was reduced  by 50%.  The pulse overlap was slightly excessive, causing a slight discoloration of the ablated area.  The width of the ablation line has increased; and  traces of black condensate can be seen.  In the lower  group the pulse spacing is reduced another 50% and  significant condensation is evident.


The condensation shown if Figure 8 has the  appearance of burn marks in the photograph, but  actually consists of ablation particulates coated with  condensate.  The black areas in the lower group are  built up significantly higher than the ablation surface.  The results shown are for a single pass of a single  line scan.  When condensation occurs during a  normal bulk ablation sequence, the progressive  accumulation of condensate can cause serious  problems with stalagmites, as shown in Figure 9.


The left side of Figure 9 shows an ablated area with  power set to produce vigorous ablation.  Pulse  overlap is marginally excessive, resulting in a narrow  band of black condensate at the edge of each scan  line.  The ablation pattern used was an interlaced  progressive raster scan.  The line to line spacing was


set to just achieve uniform planar ablation.  The  ablated area in the photograph is ten scans below the  package surface, which was a depth


Figure 8: condensation versus pulse overlap when  photo-mechanical ablation is minimized.


Figure 9: Tendency for stalagmites with excessive  pulse overlap and insufficient power.


of approximately 50 mils.   In the right side of the  photo all settings are identical except the laser  power, which was reduced by 50%.  The reduction in  power did not eliminate the visible condensation; but  it did reduce the amount of photo-mechanical  ablation, resulting in a significant increase in  stalagmites.  These appear as the dark features in the  right side of the photograph, and are a few tens of  mils high.  These results were typical.  When  condensation was observed at the lower side of the  process window, an increase in power and a decrease  in pulse overlap was usually required.


Figure 10 shows the same sequence of increasing  pulse overlap as shown in Figure 8.  The same  average laser power was used as in Figure 8, but with  a much shorter pulse width and a much higher peak  power.  The increase in peak power was  approximately 230:1.  The improvement in photo123


mechanical ablation is dramatic.  There is minimal  evidence of localized overheating, even with  excessive pulse overlap.  The ablated areas are highly  fractured as a result of the vigorous spalling.  In  comparison, the ablated areas in Figure 8 show  minimal evidence of macroscopic spalling.


Figure 10: Ablation rate versus pulse overlap when  pulse timing is optimized.


As can be seen by comparing figures eight through  ten, full optimization of the ablation process window  requires coordinated adjustment of scan properties as  well as laser pulse properties.  An iterative empirical  approach was necessary to maximize the consistency  and rate of ablation while minimizing thermal  damage to the device


Laser decapsulation offers significant advantages  over conventional acid-etch procedures in some  applications.  Acid sensitive circuit elements such as  copper can be exposed without damage.  The risk of  collateral thermal damage can be minimized by  proper optimization of the ablation process window.  Key factors include the laser fluence, wavelength, pulse width, and repetition rate; as well as the  adjustment of pulse and line overlap in the ablation  pattern.  With optimal adjustment an interlaced raster  scanned ablation pattern can decapsulate low melting  point materials such as nylon from a novalac epoxy  package without damage; but the mold compound  filler material creates serious complications when  attempting to expose delicate integrated circuits.  The filler particles can cause both dispersion and  focusing of the laser beam.  Filler particles in  intimate contact with the die can focus the laser  beam, creating unexpected hot spots.  Complications  due to the generation of condensable species can be  minimized by proper optimization of the ablation  process window.  The optimum decapsulation results


were not obtained at the process settings giving the  maximum ablation rate; but at those settings giving  adequate ablation rates with minimum bulk heating, minimum condensation, and minimum occurrence of  stalagmites.


By utilizing CAD drawings and programmable  scanning laser techniques, laser decapsulation can  expose individual circuit elements as needed.  The  ablation depth can be accurately controlled, allowing  decapsulation to a particular package plane.  Device  features can be exposed individually, sequentially, or  simultaneously as required.  Full process  optimization requires an empirical iterative approach  to identify the best balance of interdependent process  variables and competing mechanisms.


1. Dubotzky, B. Kruger, “Evaluation of Alternative  Preparation Methods for Failure Analysis at  Modern Chip and Package Technologies”; 27th  International Symposium for Testing and  Failure Analysis, Session 3: Packaging; Nov., 2001; 83-86, (2001)


2. M. Frazier, S. A. Mathews, M. T. Duignan, L. D. Skoglund, Z. Wang, R. C. Dias; “Laser-Based  Sample Preparation for Electronic Package  Failure Analysis”; Proceedings of SPIE Vol. #4637: Photon Processing in Microelectronics  and Photonics, Jan., 2002, 4637, 374-377 (2002)


3. M. H. Hong, Z. H. Mai, G. X. Chen, T. Thiam, W. D. Song, Y. F. Lu, C. E. Soh, T. C. Chong; “Pulsed Laser Ablation of IC Packages for  Device Failure Analysis”; Proceedings of SPIE  Vol. #4637: Photon Processing in  Microelectronics and Photonics, Jan., 2002; 4637, 44-452 (2002)


4. I. Itzkan, D. Albagli, M. Dark, L. T. Perelman, C. Von Rosenberg, and M. S. Feld; “Short Pulse  Laser Ablation is Photomechanical, not Thermal  or Chemical”; Conference Proceedings, IEEE  Laser and Electro-Optics Society, 1994 7th  annual Meeting; IEEE, New York, NY, USA; Vol. 2; 71-72 (1994)


5. Yacov Domankevitz, and Norman S. Nishioka; “Measurement of Laser Ablation Threshold with  a High Speed Framing Camera”;  IEEE Journal  of Quantum Electronics; Vol. 26, No. 12; 2276-2278 (1990)


6. A. A. Kolomenskii, and P. Hess; “UV Laser  Excitation of Broadband Surface Acoustic Wave


Pulses in Silicon Near the Ablation Threshold”;


1994 IEEE Ultrasonics Symposium  Proceedings, IEEE, New York, NY, USA; Vol. 2l, 651-654 (1994)


7. E. Rimini, “Energy Deposition and Heat Flow  for Pulsed Laser, Electron, and Ion Beam  Irradiation”; Surface Modification and Alloying  by Laser, Ion, and Electron Beams: Chapter 2; Edited by J. M. Poate, G. Foti, and D. C. Jacobson; Plenum Press, New York, 1983


Investigation of Microstructure Change on Ni-based UBM Systems   in Lead Free Solder


Tan Teck Chun, Tung Chih Hang, Chai Tai Chong


Institute of Microelectronics


11, Science Park Road, Science Park 2  Singapore 117685


The effect of interfacial reaction of Ti/Ni(V)/Au  under-bump metallisation (UBM) systems in Pb free  solder had been investigated. The objective was to  examine the microstructure change and intermetallic  formation of Ni-based UBM during isothermal  annealing in lead free solder as well as to understand  its impact on the UBM failure mechanism. Studies  revealed that after IR reflow, spalling of Ni-Sn  compound from the UBM took place. A layer of NiSn-V was found to have form in the UBM. The  formation of Ni-Sn-V layer was believed to have an  impact on the failure mechanism of the Pb free  solder. Studies also showed that doubling the Ni layer  thickness in this UBM system did not have  significant improvement to the overall integrity of the  solder joint. However, samples with electroless  Ni(P)/Au UBM in lead free solder showed relatively  good thermal properties. No major change in the  intermetallic composition was observed. More details  on the microstructure change during thermal aging of  the UBM systems were presented in this article.


One of the challenging issues in lead free flip chip  technology is the development of a low cost and  compatible under bump metallisation or UBM. Nickel has shown slower reaction with tin as  compared to copper in tin rich lead free solder [1-3]. Consequently, UBM schemes with Ni as the wettable  layer have been identified by the semiconductor  industry as the preferable replacements to Cu-based  UBMs.


The top-most Au layer in Ni/Au system serves two  purposes, mainly to promote solder wettability and to  protect the underlying layers from oxidation. Owing  to its high solubility in molten Sn rich solder, the Au  layer dissolves completely and forms AuSn4  intermetallic compound in the solder during the  reflow process [4]. Small amount of Au from the  Ni/Au UBM showed no detrimental effect in SnAg  and SnAgCu systems [5].


It has been reported that spalling of Ni3Sn4 compound  from the Ti/Ni thin film was observed during  isothermal annealing in conventional eutectic SnPb  solder on Ti/Ni thin films system. The growth of the  Ni3Sn4 compound has given rise to scallop-type  morphology. Although this spalling phenomenon is  similar to that of Cu6Sn5 from Cu/Cr thin films, the  former takes place at a slower rate. This eventually  lead to de-wetting of the solder from the Ti surface


[6].


In this study, the focus was on Ti/0.3µm Ni(V)/Au  UBM (Table 1) system with lead free solder  SnAgCu. The objective is to understand the behavior  of Ni-based UBM during isothermal annealing in  lead free solder. Attention was drawn to the  microstructure changes and intermetallics formation  with respect to aging time. This was compared to two  other UBM systems. One was a thicker Ni UBM to  see the effect of variation in thickness on the  microstructure change. The other was a much thicker  UBM, in the form of electroless Ni. Much has been  reported on electroless Ni UBM and hence current  work aims to add on to some of the previous reported  work [7, 8].


Table 1: Details of the three UBM systems in current investigation.


UBM  Systems


Ti/0.3µm Ni(V)/Au


Ti/0.6µm Ni(V)/Au


Electroless Ni(P)/ Au


Fabrication  Process


Sputtering


Plating


Bond Pad Aluminum


Aluminum


Structurelayer  thickness


Top layer – Au – 0.1 µm


Mid layer – Ni (V)– 0.3 µm  Bottom  layer – Ti –0.1µm


Mid layer – Ni (V)– 0.6 µm  Bottom  layer – Ti –0.1µm


Bottom  layer – Ni (P) – ~10µm


Solder


Sn2.6Ag0.8Cu


Experiment Procedure


Test vehicle used in this experiment was a 5 x 5mm  flip chip with 16 x 16 peripheral solder bumps. A  picture of the test vehicle is shown in Figure 1. The  Pb-free solder composition consists of 96.1%Sn 2.6% Ag 0.8% Cu and some Sb. UBM for the solder bump  was a Ti/Ni(V)/Au system on Al bond pad. Details of  the UBM system are listed in Table 1. All test chips  were subjected to 1x reflow (as-reflowed) and  additional 5x reflow to simulate the number of reflow  during flip chip assembly and surface mounting  process. Reflow of the samples was done in a Seho  infra red (IR) reflow oven. Reflow profile for the lead  free solder is shown in Figure 2, with peak  temperature of 260°C. After the test chips had been  reflowed, they were further subjected to thermal  aging up to 1000 hours. This was performed in an  ESPEC oven with temperature set constant at 150°C. Microstructure and intermetallics of Ti/0.3µm  Ni(V)/Au UBM were examined at the cross-section  using optical microscopes, scanning electron  microscope (SEM) with energy dispersive x-ray (EDX)  and transmission electron microscope (TEM) after each reflow stage and at regular intervals after  thermal aging.


Figure 1: Test vehicle – 5x5mm flip chip with Pbfree solder bumps on Ni-based UBMs.


Figure 2: Pb-free reflow profile for the flip chip  samples.


In addition, test chips with Ti/0.6µm Ni(V)/Au and  electroless Ni(P)/ Au UBM on SnAgCu solder were  selected to undergo the same reflow and thermal  aging condition as the Ti/0.3µm Ni(V)/Au UBM for


comparison purposes. The microstructure and  intermetallics of these UBMs were also examined at  the cross-section after 1x reflow, 5x reflow and after  thermal aging up to 1000 hours.


Ti/Ni(V)/Au UBM


Scanning electron microscope image and EDX  element map of the UBM in the SnAgCu solder after  1x reflow is shown in Figure 3. Au was dissolved  readily in the as-reflowed condition (1x reflow) and  Ni began to react with Sn from the solder. Microstructure revealed the formation of some Ni-Sn  compound in the solder above the UBM interface, suggesting that Sn in the solder had reacted with Ni  in the UBM to form the Ni-Sn compound. Studies  have shown that Ni dissolves naturally in Sn-rich  solder during thermal reflow experiment, and occurs  at a faster rate compared to eutectic SnPb solder [9]. TEM analysis showed that this reaction formed  Ni3Sn4. In addition, some sign of spalling of the  Ni3Sn4 compound from the Ti/Ni(V)/Au UBM in the  as-reflowed condition was also observed.


Figure 3: Ti/0.3µm Ni(V)/Au UBM sample in the asreflowed condition – EDX element mapping shows  Ni-Sn compound spalling from the interface.


In order to have better understanding of the  interfacial reactions at the UBM, the sample was  further examined by TEM at the UBM in the asreflowed condition. Figure 4 shows a TEM image, revealing a continuous layer of Ti on the Al bond  pad. Grains of Ni3Sn4 formed a layer of intermetallic  beneath the Sn-rich solder. Between the Ni3Sn4 layer  and the Ti layer, a layer of fine grain Ni:Sn:V = 76:12:12 region had formed. This layer was  originally the Ni(V) rich layer in the UBM, serving  as the wetting surface for the Sn-rich solder. The  presence of Sn in this region was believed to have  come from the solder. This suggested that Sn diffused  into the Ni(V) layer through the grain boundaries of  Ni3Sn4 layer to form the fine grain Ni-Sn-V region. Eventually, the whole Ni(V) layer reacted with Sn as  thermal aging progressed.


Al


Ni-Sn


Figure 4: Ti/0.3µm Ni/Au UBM sample in the asreflowed condition - TEM image at the interface of  the solder and UBM. Notice the formation of a fine  grain Ni-V-Sn layer.


Figure 5: Ti/0.3µm Ni/Au UBM sample after 96hours  thermal aging - TEM image at the interface of the  solder and UBM. Ti was attacked by Sn and appeared  roughened.


The interfacial reaction did not stop with depletion of  Ni layer.  As thermal aging continued, Ti layer in the  UBM was also susceptible to the attack by Sn  (Figure 5). The attack caused the Ti layer to become  roughened and discontinuous. Gradually, Ti reacted  with Sn and was subsequently depleted. TEM results  showed that after 1000 hours of thermal aging, Ti  was completely attacked, with EDX showing  Sn:Ti:Al:V:Ni = 74:11:13:1.5:0.5 (Figure 6). This  makes delamination between UBM and underneath  oxide/Al a near certainity.


The microstructure changes at the interface of the  Ti/0.3µm Ni/Au UBM in the lead free solder joint  revealed the weakness of this system. Lack of  interfacial strength was evident from the solder bump  shear test failure mode, which showed a fairly  consistent mixed mode failure i.e. failure through


bulk solder and UBM (figure 7), after reflow and  thermal aging. This again indicated a weakness in the  UBM. Such weakness would contribute to a  weakness in the solder joint and potentially a failure  site during reliability tests. From the above  mechanism, it suggested that thickness of the Ni layer  in the UBM might be an area of concern.


Figure 6: Ti/0.3µm Ni/Au UBM sample after 1000  hours thermal aging - TEM image at the interface of  the solder and UBM system. The UBM is completely  attacked.


Figure 7: Sheared surface of Ti/0.3µm Ni/Au UBM  sample after shear test, revealing mixed mode failure.


Effect of Variation of UBM Thickness


The thickness of the Ni layer in the Ti/Ni(V)/Au  UMB was doubled (from 0.3µm to 0.6µm) to  understand the effect of varying UBM thickness on


the interfacial reaction and microstructure changes. SEM image and EDX element map of the Ti/0.6µm  Ni(V)/Au UBM in the SnAgCu solder after 1x reflow


was shown in Figure 8. Au was dissolved readily in


the as-reflowed condition and Ni began to react with


Sn from the solder. Microstructure studies revealed  the formation of Ni-Sn compound in the solder above  UBM


Ni (V)


Ni-Sn-V


Ni3Sn4


Ni(V)


the UBM interface, showing that Sn had reacted with  Ni from the UBM to form the Ni-Sn compound. TEM/EDX analysis showed that this reaction formed  Ni3Sn4. Some sign of spalling of the Ni3Sn4  compound from the Ti/Ni(V)/Au UBM in the asreflowed condition was also observed. These  observations were consistent with that of the 0.3µm  UBM system right up to 1000 hours thermal aging. Solder bump shear test after thermal reflow and  aging, typically revealed mixed mode failure as  shown in Figure 9.


Figure 8: Ti/0.6µ Ni(V)/Au UBM sample in the as  reflowed condition – EDX element mapping shows  Ni-Sn spalling from the interface.


Figure 9: Sheared surface of Ti/0.6µm Ni(V)/Au  UBM sample after bump shear test, revealing mixed  mode failure.


From the above experiment, it was apparent that the  Ti/0.6µmNi(V)/Au UBM had undergone similar  microstructure change as the Ti/0.3µm Ni(V)/Au  UBM. The Ni(V) layer reacted with Sn and after  thermal aging, Ti layer in the UBM was also  susceptible to the attack by Sn. Gradually, Ti reacted  with Sn and was subsequently depleted. Hence, doubling the Ni layer thickness did not improve the  overall integrity of the solder joint.


Effect of using Electroless Ni UBM


Flip chip samples with electroless Ni(P)/Au UBM in  lead free solder exhibited relatively good thermal  aging properties. Au was dissolved readily in the  solder after 1x reflow. In the UBM, Ni had reacted  with P to form an intermetallic that has stochiometry  similar to that of Ni3P (Figure 10). It was reported  that upon reflow in a electroless Ni(P) UBM on SnPb bump, the electroless Ni(P) transformed to Ni3Sn4  and Ni3P. Crystallization of Ni(P) to Ni3P was  brought about by the depletion of Ni from electroless  Ni-P to form Ni3Sn4 [10]. However, Ni3Sn4 was not  detected in this case.


Figure 10: Electroless Ni UBM sample after 96 hours  thermal aging – EDX mapping showing the presence  of intermetallic at the Ni3P interface.


TEM/EDX analysis showed that two types of  intermetallics, Sn:Ni:Cu = 5:2:4 and Sn:Ni:Cu = 6:3:2, have formed at the Ni3P interface, instead of  Ni3Sn4. These were indicated in the TEM image as  shown in Figure 11. With the formation of these  intermetallics, no further major change in the  composition of intermetallics took place after thermal  aging. The intermetallics detected were similar to that  reported by Zeng et. al. who did not find the presence  of Ni3Sn4 in between Sn-rich Pb free solder and  Ni(P)/Au finish on PCB [11]. It was reported that  after reflow and annealing, a layer of (Cu,Ni)6Sn5  intermetallic was formed, serving as a barrier layer  for the reaction of Sn-rich solder with the Ni-based  UBM. Figure 12 shows the TEM image of the UBM  at the interface of the solder interface after 200hours  thermal aging. Findings revealed a slight growth in  the intermetallic thickness during this time. Solder  bump shear test reported failure occurring  consistently in the bulk solder up to 1000 hours of  annealing (Figure 13).


UBM  Solder


Ni3P


UBM


Intermetallic


From the observations, the intermetallics showed  fairly good thermal stability during the thermal aging  process. There was no depletion of the UBM as  compared to the Ti/Ni(V)/Au UBM systems. Other  authors have also shown that SnAgCu solder is  compatible with electroless Ni(P)/Au UBM [12]. Flip  chip samples need to be studied for actual flip chip  assembly and assess at the package level, in order to  determine the reliability of this UBM.


Figure 11: eNi UBM sample after 96hours thermal  aging – TEM image showing two types of  intermetallics at the Ni3P interface.


Figure 12: eNi UBM sample after 200hours thermal  aging TEM image showing two types of intermetallic  at the Ni3P interface, similar to Figure 11.


Summary and Conclusion


In conclusion, spalling of Ni3Sn4 compound from the  UBM interface occurred after 1x reflow, or as soon  as the bumping is completed in the Ti/Ni/Au system. During this time, Sn diffused into the Ni(V) layer  through the Ni3Sn4 grain boundaries and formed a  fine grain Ni-Sn-V region. After thermal aging, the  whole Ni(V) layer reacted with Sn. Eventually, Ti in  the UBM was also attacked by Sn and was  subsequently depleted. This suggested an  incompatibility of this UBM with Sn-rich lead


Figure 13: Sheared surface of eNi UBM sample after  bump shear test, revealing failure in the bulk solder.


free solder, giving rise to weakness in the UBM. It  was believed that such weakness would be a potential  contributing factor to failure at this location during  reliability tests.


The benefits of the above study revealed the  interfacial reaction of Ti/Ni/Au UBM and lead free  solder as well as its potential impact on failure  mechanism. Parametric study enhanced the  understanding of varying UBM thickness on the  thermal stability of Ni-based UBM in lead free  solder. Doubling the Ni layer thickness did not  improve the overall integrity of the solder joint. Flip  chip samples with electroless Ni(P)/Au UBM in lead  free solder showed relatively good thermal aging  properties. Two ternary intermetallics had been found  with this UBM and no major change in the  intermetallics’ composition was observed with  thermal aging time.


Acknowledgement


The authors would like to thank Mr. Gautham  Viswanadam and Mr. Marvin Lo for the test wafer  fabrication and Ms Pan Kun for preparing the test  sample for TEM analysis.


1. S. Bader, W. Gust and H. Heiber, Acta Metall.


Mater. 43 , 1995, pg 329


2. R.S. Rai, S. K. Kang and S. Purushothaman,


Proceeding of 45th ECTC, 1995, pg 1197.


3. M. Harada, R. Satoh, O. Yamada, Proceeding of


47th ECTC, 1997, pg 866.


4. A Prince, Jou of Less Common Met, 1967, vol 12,


p107.


5. K.Y. Lee and M. Li, “Formation of Intermetallic


Compounds in SnPbAg, SnAg, and SnAgCu


Solders on Ni/Au metallisation”, Metallurgical  Solder


Sn:Ni:Cu=57:26:17


Sn:Ni:Cu=50:15:35


Ni(P)


Ni3P Sn:Ni:Cu=55:28:17


Sn:Ni:Cu = 44:18:38


and Materials Transactions A. Oct 2001, Vol 32A,


pg 2666.


6. P.G. Kim, J.W. Jang, T.Y. Lee, K.N. Tu,


“Interfacial Reaction and Wetting Behavior in


Eutectic SnPb Solder on Ni/Ti Thin Films and Ni


Foils”, Journal of Applied Physics, vol. 86, no.12,


1999, p6746 - 6751.


7. C.K. Ong, T.C. Tan, V. Kripesh, T. C. Chai, “Thermal Aging Behavior of Pb-free Solders In  CSP Packages”, Semicon Singapore 2002, pA1 - A8.


8. T. Noudou, K. Hasegawa, A. Takahashi, A. Hakaso, “Solder Joint Reliability of Electroless  Ni-P/Pd/Au Finish’ ICEP Proceedings 2002, Japan, p498-503


9. T.M. Korhonen, P. Su, S. J. Hong, M. A. Korhonen, and C. Y. Li, “Under Bump  Metallisation for Lead Free Solder”, ECTC


2000.


10. J.W. Jang, P.G. Kim, K.N. Tu, D.R. Frear, “Crystallization of Electroless Ni-P UBM  Induced by Solder Reaction”, Int’l Sym on  Advanced Packaging Materials, 1999, p252 - 255.


11. K. Zeng, V, Vuorinen, J.K. Kivilahti, “Intermetallic Reactions between Pb-free  SnAnCu Solder and Ni(P)/Au surface Finish on  PWBs”, ECTC 2001.


12. Marvin Chen-Yang Lo, Poi-Siong Teo, Charles  Lee, “Thermal Stability Of Lead-Free Flip Chip  With Al/Ni(V)/Cu And eNi/Au UBM”, APACK  Conference on Advances in Packaging, Singapore, 2001.


Failure Analysis Strategy For 2 Stacked Die CSP


Shamsul Mohamed, Caroline Francis, Rodzaki Saad, Rosli Jaffar


Advanced Micro Devices, Penang Malaysia


Multi chip packages provide higher functionality in a  module using multiplicity of dice. One specific packaging  technology known as Stacked Chip-Scale Packaging  raises new challenges for the failure analysis community. A methodology to perform full electrical isolation and  failure analysis without damaging the electrical  connectivity on either package or any of the dies in a  stacked 2-die package is described. A second challenge is  to obtain analysis result in a limited time frame in order to  improve manufacturing yield and perform corrective  action effectively.


Example of successful failure analysis following this  methodology on units with failure in packaging unit and  units in failure in the die are presented.


Stacked -Chip Scale Package (S-CSP) is an emerging trend [1-4] to meet higher storage and faster speed requirements (Figure 1). The miniaturization and higher functionality is  accomplished in stacked die packages through the  optimization of die size and thickness, die attach stacking  and wire bonding process. All these tasks are important in  minimizing S-CSP substrate interconnect density.


This paper outlines the failure analysis technique for 2  Stacked Die Chip Scale Package (CSP) where the analysis   has been carried out without damaging the integrity of  package interconnects. The top die is 16Mb Flash device  and the bottom die is a 4Mb SRAM. The top die removal  technique used a combination of wet etch and  decapsulation processes and is described in detail. This  technique was specifically developed to analyze a device  failure that could be due to die fabrication, assembly, testing process or even a handling related issue.


Figure 1: A typical construction of 2-stacked Die CSP  package


Failure  Analysis Strategy


Based on our previous work, we reviewed the basics  needed to fully analyze the failing device or package. The  bottleneck for analyzing 2 stacked die CSP package was  to be able to access the bottom die when emission  microscopy or other fault isolation analysis was needed. On the other hand, other failures linked to either  package/substrate or top die would be easily tackled using  the normal analysis flow. The analysis flow for 2-Stacked  Die CSP is illustrated in Figure 2.


Figure 2: The flow chart above illustrates the failure  analysis matrix developed for 2 -stacked die CSP package.


Determination of Package/Dice Related  Failure


In the failure analysis, the understanding of  device/package construction and functionality played a  very important role. This would enable an analyst to  strategize the analysis flow, minimize the scope of the  investigation and at the same time shorten the analysis  turn-around time. Pre-decapsulation analysis such as  electrical diagnostic, simulation and isolation were proven  helpful during preliminary stages. In this paper however, we will only describe the electrical probing process that is  widely used for parametric failures such as open, short  and leakage. This process is performed to isolate whether  the failure is due to die or package.


In our analysis, normally the initial electrical probing  process start between solder ball and copper interconnect (located at the edge of package) of the failing pin. This  will give early information of the electrical integrity of the  copper interconnect between the solder ball and the  copper pad. The probe point is represent ed as B and C in  Figure 4. Secondly, the probing analysis is performed  between point s A and B to inspect the integrity of the  bond wire and to determine if the failure has  not  originated from the package/substrate.


Figure 3: Typical construction of Stacked-CSP package  with points A, B and C representing the probing locations.


Top Die Removal Process


Two  (2) killing factors were taken into consideration  when developing top die removal technique. First desire  was to maintain the same packaging quality and the  second one was to minimize alteration of any failure mode  so that further electrical fault isolation could be performed  on the bottom die. The top die removal process is  described in detail below:


Step 1: A small opening on top die was gained through a  decapsulation process. The size of the opening was  approximately 75%-85% of the actual size of the top die


Figure 4: The S-CSP package with top die exposed after  the  decapsulation process.


Step 2: The active circuitry of the exposed top die was  etched-off (Figure 5) by dipping the unit in hydrofluoric  acid The etching time could vary from 10-15 minutes  depending on device fabrication process. The purpose of  HF etch is to remove passivation, ILD and metal layers.


Figure 5: The active circuitry of top die was completely  etched-off by HF acid. This step will allow rapid removal  of silicon in the subsequent step.


Step 3: The top die was essentially etched-off (Figure 6) in this step by dipping the CSP package into hot sodium  hydroxide (KOH at 100C) solution. The concentration of  KOH used was 46%. The etching time could vary from 30  to 180 minutes depending on the thickness of the die.


Figure 6: The majority of top die was removed in step 3  with some of the residue remaining on the bottom die  surface.


Step 4: The top die is completely removed (Figure 7) in  this step by etching off any residual top die, die attach and  balance of the mold compound covering the bottom die. This was accomplished by performing a wet decapsulation  process.


Figure 7: Photos of S-CSP package after the bottom die  was fully exposed.


After step 5, electrical fault isolation can be performed on  the bottom die to determine the location and type of


failure. In some instances it is necessary to etch away the  bond wire as well, before electrical fault isolation on the


bottom die can begin as shorts between the bond wires can  occur. A summary of the top die removal process is


illustrated in figure 8.


Figure 8: Flow  chart showing the summary of top die  removal process.


Decapsulation process to


expose 75%-85% of top die


Nitride passivation of top die  is stripped using HF acid


Etch-off  the top die in hot  KOH.


Etch the remaining of top die, die attach and balance of mold  epoxy covering the bottom die


Bottom die


exposed


Remove the remaining bond


wires of the top die


Completed top die


removal


Analysis of a Package/Substrate Related  Failure


During qualification of a new S-CSP device, three units  were found failed open during reliability tests. Based on  the specification, all the units failed earlier than  anticipated. Quality and reliability engineering requested a  full investigation for root cause of this failure.


The electrical probing analysis by failure analysis group  showed the failure to have originated from  package/substrate. Subsequent package de-processing  process was performed to expose the copper interconnect  and the thru hole via. High optical and scanning electron  microscope (SEM) inspection revealed solder resist crack  that propagated across the copper interconnect and had  caused the reported failure.


Figure 9: SEM inspection revealed solder resist crack that  propagated across the copper interconnect.


Analysis of Die Related Failure


T wo units of 4M SRAM devices failed low leakage at  room and hot temperature with current reading more than  50uA. The failures were encountered by product  engineering during Initial Class Test (ICL). Electrical reverification and isolation by failure analysis group   confirmed the reported failure and proved the failure  originated from bottom die and not from package  substrate.


Based on initial results, accessing the bottom SRAM  became essential for determining the root cause for   failure. With successful top die removal process, full  electrical failure analysis was then performed to zoom in  on the defect/damage location. Photon emission analysis  revealed emission site at circuitry associated with high  voltage bus line (Figure 10). Sequential die delayering to  silicon level revealed mid gate pinhole (Figure 11) which  was caused by gate oxide breakdown.


Figure 10: The photon emission analysis detected  emission site on the failing SRAM unit.


Figure 11: Photo of gate oxide rupture at circuitry  associated with the emission site.


Comparison to Planar Polish Technique


Previously [5], an FA technique applicable for 2 stackeddie CSP has been reported.  This method deals with  mechanical polishing of the top die using a planar  polishing technique and then chemically etching  remaining mold compound, and die attach material to  expose the bottom die. The bottom die is extracted and  rebonded to a suitable package for analysis.  This method  relies critically on polishing so that the bottom die is  unaffected in the process.


The present method has advantages over the polishing  technique [5] as it does not require a re-bonding process  and secondly a sample preparation for planar polish. It can  be argued that a local polishing technique with good  control for material removal has advantages over globally  polishing the major surface of a package.  The relative  merits of these options are to be weighed in by the failure  analyst to choose the best approach that suits the nature of  the failure.


A major challenge during failure analysis of 2 stacked die  CSP package is to fully isolate and perform electrical  isolation on bottom die while maintaining the electrical  connectivity. This has been exemplified by successful  analysis of the failure in the bottom die of a stacked CSP. Any attempt to mechanically or chemically remove the  top die can cause stress to the bottom die. In this respect, parameter optimization (i.e temperature, etching time, concentration of acid/alkaline) and a deep understanding  of package properties and design play major role for   successful analysis. Furthermore, the experience gained  from this package was proven helpful in dealing with  future stacked die CSP.


The authors would like to sincerely acknowledge Dr. Rama R. Goruganthu of AMD Austin for  all the enormous  support, technical advice and consultation on writing the  manuscript. A special thanks to Glen Gilfeather and  Anthony Marquez of AMD’s Worldwide Device Analysis (WDA), MG-Product Engineering and Penang QE for  their encouragement and valuable insight in publishing  this paper.


1. Jean-Paul Clesh, "Flip-Chip and Chip -Scale Package  Reliability Modeling", ChipScale Review -November


2. Lee Smith and Ted Tessier (Amkor Technology Inc), "Stacked Chip -Scale Packages: They Are Not Just  For Cell Phones Anymore", ChipScale Review - July


2001.


3. M.Kada and L.Smith, "Advancement in Stacked  ChipScale Packaging (S-CSP) Provide Package  Functionality for wireless and Handheld  Applications", Proc. Pan Pacific Microelectronic  Symposium 2000.


4. Reza Ghaffarian, "Joint Integrity of Chip Scale  Packages Under Isothermal Aging", ChipScale  Review - July 1998


5. Christopher C. Flores, “Failure Analysis of StackedChip Scale Package”, ISTFA2002


Evaluation of Package Defects by Thermal Imaging Techniques


Yongmei Liu, Rajen Dias,


Assembly Technology Development, Quality and Reliability Intel Corporation


5000, W. Chandler Blvd.


Chandler, AZ 85226, USA


Study presented here has shown that Infrared thermography has the potential to be a nondestructive analysis tool for evaluating package sublayer defects. Thermal imaging is achieved by applying pulsed external heating to the package surface and monitoring the surface thermal response as a function of time with a high-speed IR camera.


Since the thermal response of the surface is affected by the defects such as voids and delamination below the package surface, the technique can be used to assist package defects detection and analysis.


Increased package complexity and shorter development time requires continuous development of advanced analytical capabilities. One of the key challenges is to develop nondestructive imaging capability to detect package defects such as cracking,delamination and voids. The results of a study presented here reveal that recent advancements in IR thermography have the potential for detecting certain package defects.


Infrared thermography is a nondestructive evaluation method that allows extraction of information on sublayer defect and abnormality based on thermal response of the inspected part after it is subjected to an instantaneous or a continuous heat source [1,2].


An infrared detector records the thermal response,that is the local infrared emission from the surface according to the Stefan-Boltzmann law. Information about the internal structure of the part such as thermal properties or presence of the defects can be obtained by analyzing the infrared information [3].


The principle of thermal imaging for defect detection is as follows: when heat is applied to an object, it diffuses from the source into the surrounding material. A flaw in the material, such as a void, alters the diffusion rate depending on the size and location of the defect. This in turn affects the local temperature in the vicinity of the flaw and eventually changes the temperature profile on the surface of the material. Thus, by monitoring the surface thermal response, one can detect the changes in the surrounding material caused by the presence of


defects in the path of the thermal conduction front


[4]. Determination of the actual surface temperature is often of limited interest in IR thermography, and the emphasis is placed on detecting the differences in temperatures at different points on the surface being monitored. Thermography may be thought of as the mapping of isotherms (contour of equal temperatures) [5].


It is easier to detect the flaws in a material that is not highly conductive. The temperature gradient around such a flaw is greater and lasts longer. In contrast,the surface temperature perturbations caused by a flaw in a highly conductive material are not strong because heat is dissipated more rapidly and more evenly on the surface of a highly conductive object


[4]. Therefore, pulsed infrared thermograpghy is often conducted, where a pulse of energy is injected to the part and this launches a thermal front that propagates under the surface by diffusion according to the Fourier diffusion equation. [3,6]. The change of sample surface thermal response in a very short duration after applying a single heating pulse is recorded. Infrared detector detects the change of surface radiation when a heat conduction wave front encounters the subsurface change in thermal conductivity. The effect of sublayer defects on surface temperature distribution is temporarily magnified during the early stage of the thermal transient state. As time passes, the effect of defects reduces in magnitude and becomes small as the steady state is approached due to lateral heat transfer[4, 7].


This technique has several attractive features: it is non-destructive, easy to set up, and it can provide inspection results quickly since it operates in a pulsed transient regime while a large area can be analyzed due to possible surface-wide pulsed heating


[3]. Thus, it is a popular tool for characterizing material defects [8]. It has now been extended to a broad range of applications in automotive, aerospace and energy industries [9].


A feasibility study has been conducted here to evaluate the capability of using IR thermography in for thermal interface material (TIM) defect detection in electronic packages. Inspection of TIM defects was conducted by applying an external heat pulse to


the package surface. The surface thermal response was monitored as a function of time with a highspeed IR camera. The uniqueness of this method lies in the capability of capturing surface temperature distribution in the transient mode at a speed of several hundred frames per second. The data is integrated to understand the change of the temperature pattern that can be correlated to possible defects underneath.


Preliminary results suggested that this metrology can provide useful information on these types of defects,and it is an important tool that can complement existing failure analysis techniques for packages. The potential of the method, the challenge, and approaches to improve the sensitivity are also discussed in this paper.


Materials and Methods


Specimens


Typical defects observed in electronic packages are delamination, cracking and voiding. Study on TIM defects is presented here. In this case, a thin layer of TIM is sandwiched between the Si die and lid, as illustrated in Fig. 1.


Four samples with different TIM defect were inspected by scanning acoustic microscope in reflective (CSAM) mode, as shown in Fig.2. These include a part without TIM defect (#1), TIM delam(#2), lack of TIM (#3), and no TIM (#4). CSAM image provides a baseline to compare with the result obtained by IR thermography. Note that delamination and voiding would show up in white color in CSAM.


Setup of Echotherm IR non-destructive tool is illustrated in Fig.3. The testing system contains the following major components: heating source, IR camera, data acquisition and imaging processing system.


320 × 240 focal plane array (FPA) IR camera with Indium Antimonide (InSb) detector was used to monitor the change of thermal response on the surface of the lid. The IR camera operates in the wavelength range of 3-5 µm, and has high-speed imaging capability. Bi-tube flash lamp assemblies with short pulse (few ms) width and a maximum power output of


Figure 2. CSAM images for samples #1 ~#4. Die edge was outlined for each sample.


~10 KJ was used. A removable absorptive coating was often applied to the package surface to improve its infrared emissivity and sometimes reduce its optical reflectivity. The flash lamp assemblies were carefully fixtured to heat the target uniformly. The sensitivity of the IR camera is rated to be at ~ 25 milli-Kelvin by the IR camera manufacturer.


The Infrared system receives the infrared radiation emitted from the testing samples and converts it to electrical signals. These signals are then processed and displayed on a screen as thermal gradients [5].


The image data can be represented by IR intensity or absolute temperature. To understand the actual temperature rise and decay, the IR camera can be calibrated externally using a black body source to allow measurement of absolute surface temperature changes.


Lid


TIM


Die


Figure 1: Schematic cross-sectional view of samples used in this study.


High speed


IR camera


Flash Lamps


Heat conduction IR radiation


defect


Image/data processing


Figure 3. Schematic setup of one-sided pulsed thermography.


Modeling


To understand defect impact on lid surface temperature distribution, modeling simulations were conducted using IR Thermographic Non-Destructive Testing (NDT) Software Packages [10]. IR Thermographic NDT Software Packages include numerical modeling for computing dynamic temperature distributions and for test optimization. It also has special image processing software that allows defect characterization [11]. Modeling configuration was similar to Fig.1. The following cases have been modeled: (1) various sizes of the TIM voiding to assess its impact on surface temperature distribution; (2) introduce delaminationlike thin defects at lid/TIM and TIM/die interfaces.


Surface Temperature Evolution


Upon pulsed heating, the entire lid was heated up. IR images were taken every 5 milliseconds and signal was then processed to obtain the image with improved resolution on substructure. Fig. 4(a) shows a single frame image of specimen #2 at t = 10ms after flash heating. At this time, the surface thermal response was fairly uniform. The same has been observed for other samples inspected. As time increases, the temperature profile containing a defect deviates from the one without defect during a particular period of time that occurs after heating.


Consequently, sub-layer structure of the TIM started to appear on the lid IR image, as shown in Fig. 4(b) ,where single frame image was taken at t = 20ms.


TIM shape became clearer at 40 ms, Fig. 4(c). The shape of the good region (bonded interface, lower temperature) shown in Fig. 4(b) and 4(C) is similar to that observed in CSAM (Fig. 2), thus demonstrating the possibility of using IR


thermography to detect the bonding/debonding in TIM.


Figure 4. Single frame IR image of the lid for sample#2 at (a) 10 ms, (b) 20 ms and (c) 40ms.


Detecting TIM Defects


Fig. 5 reveals the subsurface structure detected using the high-speed pulsed thermography for samples#1~#4. These were averaged composite images based on 4 consecutive frames, beginning at 20ms after the flash to 40ms, with the preflash lid image subtracted to reduce possible fixed pattern artifacts associated with heating or the camera focal plane. Differential temperature range ∆T between the good (bonded)and the bad (defect) region was found to be ~ 0.2 to


0.3°C. Cooler lid surface temperature indicates more efficient heat transfer through TIM; while hotter regions on the lid surface indicate defective TIM underneath. It has been noted that the different compositions of TIM also affects surface temperature decay.


(b)


(c)


Figure 5. Average lid IR image (20 ms to 40 ms)with preflash image subtracted for #1 ~ #4. Entire lid was captured.


Modeling Simulation


a). Effect of TIM voiding size


Modeling showed that the defect size plays a significant role on the lid temperature distribution as a function of time. By increasing the TIM voiding radius from 2 mm to 4 mm, the temperature difference on the lid surface between the void and the adjacent good region increased form 0.124°C to


0.240°C. The optimal observation time window to detect such temperature difference ranges from 30 to 50 milliseconds after the heat pulse is applied.


b). Resolution of TIM delam interface


Thermal modeling also indicated that the depth information of gross delamination could be distinguished by pulsed thermography coupled with advanced defect characterization algorithms. This was done by introducing delamination-like thin defect with dimensions of 8mm × 8mm × 0.01mm at lid/TIM (defect 1) and TIM/die interfaces (defect 2),respectively, as illustrated in Fig. 6(a). The simulated lid temperature distribution at 46 ms is shown in Fig.6 (b). Modeling showed that the maximum temperature contrast (or difference) over the defect was 0.24°C for defect 1 and 0.21°C for defect 2. The optimal observation time was 46ms and 54 ms for defect 1 and defect 2, respectively. This indicates at least for large delamination, that the TIM interface of delamination could be identified nondestructively by the thermal imaging techniques.


Evaluate TIM defect by IR Imaging


Although the number of testing samples was limited,preliminary results indicated that IR thermography could be an effective technique to detect TIM defects nondestructively.


Experimental results showed that the gross delamination such as those in sample #2 and #3 can be clearly revealed by lid IR image, where regions with TIM delamination (shown white color in CSAM) is hotter than adjacent regions. It is clear from Fig.5 that there is no cooler region due to no TIM for sample #4, while there is a well-defined cooler center for sample #1 due to good TIM coverage. Note that the actual surface thermal response may vary slightly from test to test, but our primary interest was to detect the differences in thermal response. ∆T between the bonded and defected region was observed to be ~0.2 to 0.3°C,which is 10 times the tool sensitivity and should be captured by IR camera. TIM profile revealed by IR imaging (Fig.5) is in general agreement with CSAM result (Fig.2).


Note that the CSAM can detect physical defects with much higher resolution. However, pulsed IR thermography has its advantages since it relates to the TIM thermal performance more directly. Besides,unlike CSAM, units do not need to be dropped in water and throughput time is also much shorter.


It should be pointed out that quantitative analysis is possible in pulsed thermograpgy. Information such as


Defect1


Defect2


Figure 6 : (a) Top views of two TIM defects located between lid/TIM (defect1) and TIM and TIM/Die(defect2); (b) Predicted lid temperature distribution at t = 46ms.


High speed IR camera


Heat conduction


IR radiation


Figure 7. Schematic setup of thru transmission pulsed thermography.


the onset of time where the temperature profile containing a defect deviates from the one without defect and the timing with maximum ∆T could be very useful for defect characterization. In pulsed thermography, a useful relationship between the thermal propagation time t to the depth z of a subsurface defect is [12]


α


~z


where α is the material thermal diffusivity (m2 s -1 ),α=K/ρC, ρ is the mass density, and C is the specific heat. Quantitative analysis can also be computed based on thermal contrast images which requires one to compute temperature difference in images with respect to a non-defected area in the image [13]. A well-used contrast definition is [14]


Ts


where index i refers to a suspected defective location and s to a sound area. C(t) is computed with respect to temperature difference at the defected region and normalized by the behavior of a sound area. Note that the definition for contrast C(t) is dimensionless and is a function of time. The maximum value of contrast is of interest.


As both theoretical and experimental studies have shown, the time to reach the maximum temperature contrast increases with defect (voiding) depth,whereas the magnitude of the contrast decreases rapidly with the depth [15]. As modeling predicted(Fig.6), it is feasible to determine the delamination location in the Z-direction when delamination is gross. Theoretical study has also shown that a defect close to the surface would cause a much more localized perturbation in the measured temperature distribution at the time of maximum contrast,compared to the extended perturbation caused by a defect of similar size situated further away from the surface [1]. Quantification of IR image data and defect characterization will be explored in a future study.


Defect Detection Sensitivity and Future Work


The minimum resolvable defect (with confidence in size and shape) was estimated to be about a few mm on current configuration in the present study. Small defect would be difficult to be detected by IR imaging due to strong lateral heat transfer of highly conductive Cu lid. This is because the IR image of subsurface defect would appear blurred at the surface


as a result of fast thermal diffusion as time elapses.


Therefore, it is critical to capture defect information at the very early stage using fast IR camera. The spatial resolution of defect detection appears to be mainly limited by thermal diffusion.


In addition to one-sided inspection, pulsed thermographic through transmission inspection may provide valuable information about thermal interface quality as well. As shown in Fig.7, where one side is rapidly heated and the thermal response of the other side is monitored.


Image average, subtraction, division and contrast methods, etc are used to improve signal to noise ratio and to reduce the effect of non-uniform heating and fixed pattern artifacts from the camera focal plane[3,9,11,16,17]. To improve resolution and the capability to detect small defects, advanced image processing should be investigated continuously.


Furthermore, direct die heating and monitoring lid surface temperature is expected to provide greater surface ∆T over external pulsed approach [18].


By combining experimental, modeling simulation and advanced image-processing algorithms,potentially, TIM integrity can be effectively assessed. Furthermore, this method could be used for other thin film delamination detection as well.


Present study demonstrated the strong potential of applying pulsed IR thermography for package TIM defect analysis. Packages with gross TIM delamination has been clearly detected, and the throughput time was very short. The impact of defect size on the lid temperature distribution was analyzed by modeling and result was shown to be sensitive of defect size. Characterizing small TIM defects


especially away from surface remains to be a major challenge due to limitations originated from thermal diffusion. Tool sensitivity would be improved with advanced imaging processing and direct die heating.


This technique could be an important complementary tool to existing failure analysis techniques.


The authors would like to thank ThermalWave Imaging for assistance in the pulsed thermography study.


1. Sayers, C. M., “Detectability of Defects by Thermal Non-destructive Testing”, British Journal of NDT 26, 28-33 (1984).


2. Maldague, X.P.V., “Instrumentation for the infrared”, Infrared Methodology and Technology,edited by X.P.V. Maldague, pp.53-101, Gordon and Breach Science Publishers (1994).


3. Maldague, X., and S. Marinetti, “Pulse Phase Infrared Thermography”, J. Appl. Phys. 79 (5),pp.2594-2698 (1996).


4. Burger, Christian and Raj, Babak, “Nondestructive Evaluation Through Transient Thermographic Imaging”, Proceedings of the 15th Symposium on Nondestructive Evaluation, pp.56 –67 (1985).


5. Burger, C. P. and Gryzagorides, J., “Transient Field Infra-red Video Thermography as Procedure for Non-destructive Testing,” Proc. Measurement Science Conference, Palo Alto, pp.201-208 (1983).


6. Carslaw , H. S., and J. G. Jaeger, Conduction of Heat in Solids, 2nd ed. Clarendon, Oxford (1959)


7. Daniels, Arnold, “Optimization of pulsed temporal stimulation for the thermal nondestructive testing,”Proc. SPIE Thermosense, V.3361, pp.254-265(1998).


8. Vavilov, V.P., “Infrared Techniques for materials Analysis and Nondestructive Testing”, in Infrared Methodology and Technology edited by X.P.V.


Maldague, pp.131-210, Gordon and Breach Science Publishers (1994).


9. Shepard S., “Advances in Transient Thermal NDT”, Prod. SPIE Thermosense XXIII, V.4360 pp.511-515 (2001).


10. Vavilov, V.P, personal communication (2000).


11. Vavilov, V.P, S. Marinetti, E. Grinzato and P.


Bison, “Thermal Tomography, characterization and pulse phase thermography of impact damage in CFRP, or why end-users are still reluctant about practical use of transient IR thermography”, Pro.


SPIE 3361, pp.275-281 (1998).


12. Cielo, P., X. Maldague, A.A. Deom, and R.Lewak, Material Eval. 45, 452 (1987)


13. E.Grinzato, V.Vavilov, P.G. Bison, S. Maruneti,and C. Bressann, Proc. SPIE, 2473, 167 (1995)


14. X. Maldague, Nondestructive Evaluation of Materials by Infrared Thermography, Springer,London (1993).


15. Burch, S. F., Burton, J. T. and Cocking, S. J.,“Detection of Defects by Transient Thermography: a Comparison of Predictions from Two Computer Codes with Experimental Results”, Br. J. NDT, vol 26, No.1, pp.36-39 (1984).


16. Lhota, J., S. M. Sherpard, B. A. Rubadeux and T.


Ahmed, “Enhanced Spatial and Depth Resolution of Pulsed Thermographic Images”, Review of Progress in QNDE, 20 (in press) (2000).


17. Maldague, X., Couturier, J.-P., Salerno, A. and Wu, D., “Phase Analysis in Pulsed Thermography”,CSNDT Journal 4, July/August, pp.5-10 (1997).


18. Abhay Watwe, private communication, Intel(2000).


Félix Beaudoin, Philippe Perdu, Romain Desplats


CNES-THALES Laboratory, 31401 Toulouse , France


Lionel Dantas de Morais


EPSILON Ingénierie, 31319 Labège, France


Olivier Crepel, Christophe Goupil


LAMIP - Philips Semiconductors, 14079 Caen, France


Gérald Haller


ST Microelectronics, 13106 Rousset, France


Thomas Beauchêne, Dean Lewis


IXL, Université Bordeaux 1, 33405 Talence, France


Defects localization from the IC’s backside using hot  spot detection techniques is discussed. Simulations  are used to validate the applicability of hot spot  detection from the silicon backside and to determine  the optimal experimental conditions. The effects of  the dissipated power, the substrate thickness and the  defect position relative to the chip area are studied. These simulations take into account the thermal  dependence of the silicon thermal conductivity. Transient simulations are also performed to evaluate  the effect of modulating the power on the backside  temperature difference. Backside Liquid Crystal  Microscopy as well as Infrared Thermography and  Thermal Laser Stimulation results on defective ICs  are presented.


Hot spot detection has been widely used in the past to  localize current leakage related failure. Its popularity  is closely linked to the ease of use, high success rate  and equipment low costs of Liquid Crystal  Microscopy (LCM)1. However, the need to perform  failure analysis from the backside of ICs, due the  widespread use of flip-chip and lead-on-chip  packaging, and due to the use of metal filling and  multiple metal layers, challenges the applicability of  hot spot detection techniques. Despite the recent  development of several techniques to tackle the  challenging task of fault localization through the IC’s  backside, such as backside emission microscopy and  thermal laser stimulation2, rapid and broad


localization of hot spots still has its usefulness in a  Failure Analysis laboratory.


A question then arises: to what extent hot spots can  be detected from the silicon backside? The objective  of this paper is to develop an answer through  simulations and experimental studies. Thermal  simulations are used to validate the applicability of  hot spot detection from the backside. The effect on  the backside temperature of the dissipated power, the  substrate thickness and the defect location relative to  the chip are studied in order to determine the optimal  experimental conditions. Temperature distribution  maps are presented and interpreted according to hot  spot detection techniques such as liquid crystal  microscopy. Moreover, transient simulations are  compared with steady state ones in order to evaluate  the effect of modulating the power on the backside  temperature difference.


Finally, front-side and backside hot spot detection  results on defective ICs presenting a Vdd-Vss short  are presented. The applicability of liquid crystal  microscopy and infrared thermography in a backside  failure analysis flow is evaluated. The results are  compared with the ones obtained using the Thermal  Laser Stimulation technique.


Thermal Simulation


Modeled Structure


The thermal behavior of the silicon substrate in the  presence of a hot spot was modeled with a Boundary  Element Method software, REBECA-3D, developed


by EPSILON Ingénierie. The modeled structure  consists of three 1µm x 1µm metallic lines connected  to the substrate through a 1µm3 via. These metallic  elements are embedded in silicon dioxide and  covered by a resin as shown in Figure 1. The die size  is fixed to 500µm x 500µm and several substrate  thicknesses are used in this study.


Figure 1: Modeled structure in REBECA-3D.


The heat-dissipating defect is represented here by  vias in contact with the substrate. Therefore a fixed  power is applied on the full volume of the vias. The  top surface of the resin, assumed to be in contact with  a thermal regulator, is kept at a fixed temperature of  25oC. The side surfaces and the silicon backside are  submitted to natural convection with air (h=5W/m2K, T=25oC). In addition, the aluminum lines are  assumed to be connected to wire bonds of 1cm length  kept at the ambient temperature. An equivalent  convection is imposed (h=22600W/m2K, T=25oC). It  takes into account the bounding heat sink effect. Finally, the non-linear evolution of the silicon  thermal conductivity coefficient is taken into account. As shown later, this non-linear evolution, which is  more representative of the reality, plays an important  role in the silicon substrate heat-spreading behavior. All other material properties used in this study, which


are given in Table 1, are considered temperature  independent. The structure mesh definition was  adapted for each considered case.


Table 1: Material Properties


K (W/mK) Cp (J/kgK) ρ (kg/m3)


Bounding


226


Resin


0.138


1506


1040


1.381


744.8


2200


225.9


920.5


2698


K(T)*


2330


*K(T)= 150⋅(T/300)-4/3


Steady State Thermal Simulations


Preliminary transient studies have shown that for a  constant dissipated power, the temperature difference (∆T), calculated by subtracting the die backside  highest temperature with the lowest one, is not time  dependent. The temperature distribution remains  unchanged after a few microseconds even though the  system time constant is approximately 0.34s. The  maximum temperature is reached within one second. Therefore, the effect of the parameters listed in Table  2 on the silicon backside temperature distribution is  studied under steady state condition only.


Table 2: Variable Parameters


Studied  parameter


Position Thickness Power


Study #1  Location


V1, V2, V3


30µm


6mW


Study #2  Thickness


V1


30µm, 50µm, 70µm


Study #3  Power


1 to  30mW


Effect of location


The effect of the hot spot position is simulated by  applying a 6mW power on either one of the vias  shown in Figure 1. The substrate thickness is 30µm. The temperature difference, given in table 3, was  found to be increasing when the hot spot location was  moved away from the die center.


Table 3: Temperature differences for the three hot  spot location:


Hot spot location ∆T


0.57 oC


V2


0.88 oC


V3


1.61 oC


Effect of thickness


The backside temperature is calculated for a hot spot  located at via V1 and for a power of 6mW for three  different substrate thicknesses. As shown in Figure 2, the temperature difference significantly increase with  decreasing silicon thickness. As expected, the silicon  substrate acts as a thermal spreader. The thicker it is, the better the thermal repartition.


0 0,1 0,2 0,3 0,4 0,5 0,6 0,7


30


40


70


80


Substrate thickness (µm)


Figure 2: Temperature difference as a function of the  substrate thickness.


Effect of power


This study was performed for a constant silicon  thickness of 30µm and for the following dissipated  powers at via V1: 1, 3, 6, 9, 12, 24 and 30 mW.


The temperature difference, as shown in Figure 3, is  strongly power dependent. The non-linearity  dependence is due to the silicon substrate thermal  properties. The silicon conductivity reduces with the  temperature, which therefore limits the thermal  spreading and increases the temperature difference.


0 0,5 1 1,5 2 2,5 3 3,5 4 4,5 5


35


Power (mW)


Figure 3: Temperature difference as a function of the  power.


Temperature Distribution Maps


The temperatures distribution maps are shown below  for three different cases. The temperature scale is  given as follows: [Tmax ; Tmax – 0.2°]. This scale is  used to visualize the spatial extension of the hot spot  on the silicon backside. A temperature difference of


0.2oC is well representative of the sensibility that can


be obtained with hot spot detection technique such as  with liquid crystals, which is at best 0.1oC1.


The first map shown in Figure 4 is obtained for a  silicon thickness of 70µm and for a power of 6mW  applied at via V1. The temperature difference on the  whole backside is less than 0.2oC. Liquid crystal


microscopy is therefore inapplicable to detect hot


spot from the IC’s backside for such Si thickness and


low power dissipation.


Figure 4: Temperature distribution for a substrate  thickness of 70µm and a dissipated power at via V1  of 6mW. The scale is [Tmax ; Tmax – 0.2°].


However, if the substrate is thinned to 30µm, the


0.2oC hot spot is significantly reduced in size (80µm  diameter), enabling its localization (Figure 5). A high


dissipated power for such silicon thickness also


improves the hot spot resolution. This is illustrated in  Figure 6, the 0.2oC hot spot for a dissipated power of  24mW has a spatial extension diameter of 20µm  only!


Figure 5: Temperature distribution for a substrate  thickness of 30µm and a dissipated power at via V1  of 6mW. The scale is [Tmax ; Tmax – 0.2°].


Figure 6: Temperature distribution for a substrate  thickness of 30µm and a dissipated power at via V1  of 24mW. The scale is [Tmax ; Tmax – 0.2°].


Transient Thermal Simulations


Transient studies were carried out to evaluate the  effect of modulating the power on the backside  temperature difference. A square power signal of  6mW with a short oscillation period of 0.6ms  compared to the system time constant is applied to  via V1. Four temperature probes where placed at  relatively equal distance from the silicon backside  center to one of the corners. The temperature at these  four nodes as a function of time is shown in Figure 7.


Figure 7: Temperature as a function of time at 4  nodes when a 6mW square power signal with an  oscillation period of 0.6ms is applied to via V1.


The temperature oscillations caused by the modulated  power are observable on the backside surface. However, the temperature difference does not  significantly increase with time, as we would have  hoped. In fact, the temperature difference after 0.4s is


0.49oC compared to 0.54oC when a constant power is  applied. At steady state the temperature difference is


0.57oC.


Due to the relatively high thermal diffusivity of  silicon (8.91x10-5m2/s) and due to the large  dimension involved, the silicon substrate acts as heat  spreader. At the vias, the heat is first absorbed by the


substrate and is then redistributed in the SiO2. This  effect is illustrated in Figure 8 in which the heat flux  at the silicon surface is shown. We can see that the  heat flux is directed toward the silicon only at the via  proximity. The remaining silicon redistributes the  heat flux essentially in the silicon dioxide. In fact  98% of the heat flux is going through the resin and  less than 1% gets out through the silicon backside. Only a small fraction of the flux is dissipated in the  aluminum lines even though an equivalent  convection, which takes into account the bounding  heat sink effect, is used.


Figure 8: Heat flux distribution on the silicon  substrate in the proximity of the dissipative via. Only  the heat flux directed toward the silicon is  represented.


Backside Hot Spot Detection Results


The thermal simulation results showed us that hot  spots are detectable from the IC’s backside if proper  care is taken. First the substrate thickness has to be  sufficiently thinned and second the dissipated power  has to be consequent. We therefore enthusiastically  attempted liquid crystal microscopy as well as  infrared thermography for backside hot spot  localization


Failed IC Characteristics and Front-Side Liquid  Crystal Microscopy Results


The experiments were performed on several failed  ICs presenting an ohmic current leakage behavior as  shown in Figure 9. These ICs came from a rejected  wafer lot that was characterized by metal-2 / metal-3  short-circuits.


Front-side liquid crystal microscopy was first  performed in order to confirm the dissipating nature  of the shorts. The result obtained on one of the failed  ICs is shown in Figure 10. A dark spot, corresponding to the dissipative area, is clearly  observable close to one of the I/Os of this IC.


Inward heat flux


Figure 9: I(V) curve of one of the failed ICs


Figure 10: LCM image obtained from the front side  of a failed IC using a 20x objective


Backside Preparation


The failed ICs were therefore prepared to allow  backside testing. As shown in Figure 11, a square  piece of wafer containing the defective chip is glued  upside down on a metallic plate. Note that an opening  was made in the plate in order to physically and  electrically isolate the defective chip. Only the Vdd  and Vss pads are connected to separate corners of the  metallic plate to allow its polarization. Finally, a  resin is used to protect the chip as well as the  connections.


Figure 11: Image of the full chip from the front side (left) and backside (right) after thinning


The initial substrate thickness of these back-lapped  ICs is 200µm. To perform liquid crystal microscopy, some of the failed devices were further thinned down  to approximately 50µm using a parallel polishing


wheel. A final polishing step using a 0.1 µm disk was  used to obtain an optical surface quality.


Liquid Crystal Microscopy


As mentioned previously, a few failed ICs were  thinned to approximately 50µm prior to backside hot  spot localization using liquid crystal microscopy. The  tests were performed on a commercial prober  equipped with a thermal chuck and a colored CCD  camera. The liquid crystals used in this study are the  K18 from Licristal which have a transition  temperature close to 35oC. The ICs were put in  contact with the thermal chuck through the metallic  plate.


The tests were performed at a maximum current of  50mA, which correspond approximately to a 20mW  dissipated power at the defect. Unfortunately no hot  spot could be detected from the IC’s backside using  liquid crystal microscopy due to the following  difficulties:


− Poor liquid crystal homogeneity


− Insufficient backside substrate quality after  thinning


− Poor thermal regulation


First, the liquid crystals could not spread on the  silicon backside due to its hydrophobic nature. To  overcome this problem, an oxidation step using  HNO3 or H2O2 was performed. Both significantly  improved the spreading of the liquid crystal film. However the obtained film quality is still highly  inhomogeneous compared to the application of  liquid crystal on the passivated front-side as shown  in Figure 12.


Figure 12: Optical image of the liquid crystal film on  the oxidized silicon surface


In order to validate the experimental setup, the  transitional temperature window of the liquid  crystals was evaluated by varying the temperature of  the thermal chuck. For comparison, the same liquid  crystals were deposited on the front side of a


reference IC which was also placed on the thermal  chuck. As expected, the transition temperature  window was found to be 0.1oC for the front-side  case. However, a transition window of 3oC was  measured for the liquid crystals deposited on the  IC’s backside. The rotation of the polarization plan  was also found to be inadequate. Instead of transiting  from the transparent to the opaque regime as in the  front-side case, the liquid crystal deposited on the  IC’s backside had a transition from light gray to dark  gray.


In addition to the poor film homogeneity, the low  temperature resolution and poor imaging is attributed  to the insufficient surface quality of the backside  after thinning and polishing. It most likely prohibited  a proper rotation of the polarization plan. Another  unfavorable factor is the poor thermal regulation  obtained trough the resin used to isolate the defective  chip from the metallic plate.


Improvement in the liquid crystal microscopy  technique must therefore be done in order to foresee  its integration in a backside FA flow. First a good  oxide quality should be obtained on the silicon  backside. For example, oxygen plasma-cleaning or  SiO2 CVD deposition could prove to be more  effective than the use of HN03 or H2O2 chemistries. Secondly, a better thermal regulation scheme must  be developed. This would allow the use of more  sensitive liquid crystals such as the ROCE 1510  which has a transition window of only 1x10-5 oC. Finally the experimental setup must be improved to  allow visualization through the silicon substrate. A  superposition of the liquid crystal microscopy image  on a IR reflected image would allow the localization  of the hot spot from the IC’s backside.


Infrared Thermography


Backside infrared thermography was attempted on  non-thinned failed ICs (200µm silicon thickness). The tests were performed on the THEMOS-100  system from Hamamatsu. This system is based on a  Platinum Silicide IR-CCD detector with 801x512  pixels. It has a spectral response from 3µm to 5µm, thus enabling backside analysis. The theoretical  temperature resolution is 0.08oC and the smallest  feature it can resolve is in the micrometer range.


Unfortunately no thermal emission could be  observed. The highly doped p-type silicon substrate (~1019cm-3) might partially explain this result. For  such doping, the infrared light with a wavelength in  the spectral response of the THEMOS-100 system is  significantly absorbed3. Thus the thermal emission at  the defect cannot be observed. However the silicon  surface radiation contribution should be observable.


Further investigation on different samples is currently  under consideration.


Thermal Laser Stimulation


The applicability of the Thermal Laser Stimulation (OBIRCH4, TIVA5) technique for locating hot spot  defect from the IC’s backside was also evaluated. This technique uses an infrared laser to thermally  stimulate the metallic elements of the device under  tests. Correlating the induced IC’s power  consumption variations, caused by the resistance  change at heated metals, with the laser spot position  provides a precise localization of resistive type  defects. This is possible since the heating and the  resistance change of smaller metallic elements are  favored compared to larger ones6.


The Thermal Laser Stimulation tests were performed  using the OBIRCH option on the PHEMOS-1000  system from Hamamatsu. This commercial  equipment uses a 1.3µm infrared laser of 100mW  laser power. The induced variations in the power  consumption are picked up by Hamamatsu’s  detection system. It consists of a current/voltage  amplifier equipped with a voltage/current source.


Thermal Laser Stimulation results, obtained on the  same device previously characterized by front-side  liquid crystal microscopy, are shown in Figure 13 and


14. The test was performed prior to thinning, i.e. through 200µm thick highly doped p-type silicon. The failed IC was biased under a voltage of 100mV, which correspond to a leakage current of  approximately 12mA. As can be seen in Figure 13, the resistive defect is localized near the same I/O pin  identified by the front-side liquid crystal microscopy  technique. A higher magnification image using a 50x  objective allows precise localization of the defective  area. Here the defect is not directly detected since  there is no direct access to the metal-2 / metal-3  layers where the defect is located. However, the  leakage current path induced by the short-circuit  defect can be visualized in Figure 14.


Hot spot detection techniques are widely used for  front side failure analysis. However, for a wide range  of circuits, i.e. Flip Chip, these approaches are no  longer applicable. Hot spot detection from the  backside of ICs is still considered a valuable method  for rapidly localizing the failure area. Using  simulations, the influence of several parameters such  as the silicon thickness and the power consumption  on the hot spot propagation on the substrate backside  could be interpreted.


A converging beam passing through a flat plate produces  spherical aberration8. This process is shown in Figure 4 for


converging illumination. An equivalent, reverse, process  occurs for imaging a point light source within the substrate. The aberration results from Snell's law of refraction for  light passing through a surface


( )( )


1 2


2 1


sin sin


n n


θθ


(10)


where θ is the angle off normal and n is the refractive index  in each material indicated by the subscripts. Rays at high  angles get deviated proportionality more than rays at low  angles. A beam that initially focuses to a single spot will be  spread out as shown in Figure 4


Silicon Substrate


Figure 4  Example ray trace of spherical aberration in a  silicon substrate at 1.064 micron wavelength and n = 3.5.


It can be shown, with some effort, that the amount of  spherical aberration that occurs is proportional to the  thickness of the plate and roughly to the third power of the  objective numerical aperture, NA. Surprisingly, the amount  of aberration is not linear with refractive index, but to first  order is given by


aberration


∝


(11)


where an air interface (n1 = 1) is assumed. The aberrations  peak at a value of 1.73 and fall off on either side.


Determining the resolution limitations which occur from the  spherical aberration of a flat plate in closed form would be  tedious at best. Instead, the author opted to use a  commercial optical CAD program (XEMAX) to model the  effect. A matrix of numerical apertures and thickness were  modeled. The program automatically produces diffraction


spot size and an RMS radius of the aberration spot. The  RMS radius assumes a Gaussian profile, where as the the  diffraction profile is a Bessel function. The diffraction spot  diameter is related to the image resolution by a factor of


2.44. The RMS Gaussian profile does not fall off as fast as  a Bessel function. An additional factor of 1.18, (position of  the RMS radius compared to the FWHM) was factored in to  compensate for this shape change.


Figures 5-9 show the derived diffraction and aberration  limited resolutions versus silicon thickness for a set of five  numerical aperture values at a wavelength of 1.064 micron  and n = 3.5. The diffraction resolution is constant for a  particular numerical aperture. The aberration resolution  limit is linearly proportional to thickness with slope  increasing with numerical aperture.


0 2 4 6 8 10 12


Silicon Thickness (microns)


Diffraction Limit Aberration Limit


Figure 5  Resolution limits for wavelength of 1.064 micron  and NA = 0.89.


0.5 1


1.5 2


2.5 3


3.5 4


4.5 5


Figure 6  Resolution limits for wavelength of 1.064 micron  and NA = 0.75


Figure 7  Resolution limits for wavelength of 1.064 micron  and NA = 0.60


Figure 8  Resolution limits for wavelength of 1.064 micron  and NA = 0.45


0.6


0.8 1


1.8 2


500


600


Figure 9  Resolution limits for wavelength of 1.064 micron  and NA = 0.30


0 1 2 3 4 5 6 7 8 9 10


Numerical Aperture


Diffraction Limit Aberration Limit Fit


Figure 10  Diffraction and aberration limited resolution for  200 micron thick silicon substrate. Fit line from Eq. 12.


Figure 11  50X image with NA of 0.45 through ~ 250  micron of silicon.


Figure 12  100X image with NA of 0.55 through ~ 250  micron of silicon.


Clearly aberrations severely limit imaging resolution at  large numerical apertures and thickness. Generally, backside samples are thinned to increase their  transparency6. A typical final thickness is ~ 200 micron. Figure 10 shows a plot of resolution limits versus numerical  aperture for this thickness. Aberration dominates for  numerical apertures above ~ 0.5 and limits to resolution to ~ 1 micron. Larger numerical apertures actually make the  image quality worse.


A fit to the data shown in Figure 10 is given by


( )


]3


arcsin NA


kt


res =


(12)


where t is the substrate thickness and k is a constant with  value 2.75x10-2 .


Figures 11 and 12 show images taken through ~ 250 micron  silicon substrate at 50X and 100X. The pixel size in each  image is matched at ~ 0.3 micron to avoid any  misinterpretation due to pixelation. The size scale, contrast  and brightness have also been matched. The lines seen in  each image range from 1 to 2 micron widths, just at the  resolution limit for the 50X objective with a numerical  aperture of 0.45. The 100X objective used has a numerical  aperture of 0.55. The magnification ratio might imply a  factor of two improvement in the line resolution. The  numerical aperture ratio indicates that only a 22% improvement should result. In fact, the lines are slightly less  distinct in the 100X image, as expected from the model  results above.


Aberration Correction


The spherical aberration introduced by the silicon substrate  can be compensated for by purposefully introducing  spherical aberration of the opposite sign in the objective. The two cancel each other out. A "corrected" objective  results. Objectives with fixed correction are available for  biological imaging to compensate for a standard cover slip. Unfortunately, the cover slip thickness, 1.1 millimeter, and  refractive index ~1.5 requires significantly more correction  than needed for 500 micron or less of silicon.


Even if a fixed correction objective were available, there  would still be an issue of polishing the silicon substrate to  the correct thickness. Figure 13 plots the thickness accuracy  required to correctly compensate when using a fixed  correction objective. The requirement at high numerical  aperture is beyond current polishing technique.


10 100 1000


0.7


0.9


Figure 13  Polishing thickness accuracy requirement for  fixed correction objective.


Variable correction lenses have been designed. They are  very expensive and are no longer commercially available. An example of the correction capability of this type of lens  is shown in Figure 14.


Figure 14  Images taken with 100X, 0.9 NA objective  through 220 micron silicon substrate. Image on left was  taken with spherical correction and image on right is  without. White dots on black rectangles have spacing of ~ 2  micron and almost disappear in uncorrected image. Some  pixelation is apparent in these images.


The model results and images show that spherical  aberration is a significant limit to backside imaging  resolution. Corrected objectives can compensate for this  limit, however, at this time no commercially available  solution exists.


The author thanks Dan Barton for supplying the example  images in Figure 14.


1. For a review and further references see: B.V. Davis, "A  Comparison of Backside Emission Microscopy  Systems", Proceedings ISTFA 2000, 173-6 (2000).


2. For a review and further references see: K. BernhardHofer, D.L. Barton, and E.I. Cole, Jr., "Flip-Chip and  Backside Techniques", Microelectronic Desk  Reference 4th Edition, 487-503 (1999).


3. R.A. Falk and E.W. Budiarto "Application of Near IR. Phase Contrast Imaging to Backside Failure Isolation  and Analysis", Proceedings ISTFA 2000, 567-73 (2000).


4. L.A. Knauss, B.M. Frazier, H.M. Christen, S.D. Silliman, K.S. Harshavardhan, E.F. Fleet, F.C. Wellstood, M. Mahanpour, and A. Ghaemmaghami, "Detecting Power Shorts from Front and Backside of  IC Packages Using Scanning SQUID Microscopy", Proceedings ISTAF 1999, 11-16 (1999).


5. J.A. Kash, J.C. Tsang, D.R. Knebel, and D.P. Vallett, "Non-Invasive Backside Failure Analysis of Integrated  Circuits by Time-Dependent Light Emission: Picosecond Imaging Circuit Analysis", Proceedings  ISTFA 1998, 483-489 (1998).


6. R.A. Falk, "Near IR Absorption in Heavily Doped  Silicon - An Empirical Approach", Proceedings ISTFA  2000, 121-7 (2000)


7. V. N. Mahajan, Optical Imaging and Aberrations , SPIE Optical Engineering Press, Bellingham, WA (1998).


8. V. N. Mahajan, Optical Imaging and Aberrations, 318-22, SPIE Optical Engineering Press, Bellingham, WA (1998).


S. Kiefer, M. Nair, P. Sanders, J. Steele, M. Sutton, R. Thoma, S. Wilson


Motorola Digital DNA Laboratories, 2100 E. Elliot Rd., Tempe, AZ 85284


G. Albright, C. Li, J. McDonald


Quantum Focus Inc., Vista, Ca. 92083


In order to understand spatial and temperature  resolution limits of an infrared microscope used for  fault location in semiconductor devices, numerical  models and bench methods are correlated and  discussed.  Results clearly show fault identification  capability in the sub-micron realm and “hot-spot” resolution of a few tenths of a degree K.


One frequently encountered problem in integrated  circuit debug and failure analysis is locating sites where  excess current is flowing due to some sort of fault or  defect.  The most commonly used technique for this  type of fault location is photon emission. [1,2] This  method works well when the current is associated with  a leaky reverse biased junction or a forward biased  junction where radiative electron hole recombination  occurs.  In this case, light emanates from the site where  the current is flowing.  This radiation is easily detected  with low light cameras, designed for astronomy  applications and adapted to semiconductor failure  analysis.  Correlation to the faulty device is made by  digitally superimposing a reflected light image upon the  photon emission image.


However, if the source of the leakage is a resistive short  where radiative recombination does not occur, the  photon emission technique is not effective for fault  location.  (This type of fault may be due to a conductive  short where the IV curve is linear or a depletion related  short where the leakage is low until the space between  two similarly doped regions is depleted and then current  increases approximately linearly.)  In these cases, often  the next step is to see if the dissipated power is large  enough and sufficiently localized to form a hot spot on  the integrated circuit.  The most commonly used  technique to detect this type of hot spot has been to  spread a thin layer of cholesteric liquid crystals over the  sample surface and look for transitions in the films  transparency as power is applied to the integrated  circuit [3].  Another method that has been reported but  is less commonly used is fluorescence  microthermography [4].  Both techniques require the  handling of special materials that is not always


convenient and both are limited when there is a need to  do back side studies.


Recently we have investigated the use of infrared  microthermography to detect hot spots.  The test set up  and methodology is very comparable to photon  emission with the only major differences being the  camera and lenses which are optimized for 3-5 micron  radiation rather than the visible to near infrared.  Because transmission of radiation in this wavelength  through pure or lightly doped Si and GaAs is typically  very good, this technique is readily applied to backside  analysis.


In the past, infrared microthermography has not been  heavily investigated as a fault detection technique  because of the limitations in sensitivity and concerns  about spatial resolution. Recent advances in infrared  camera and lens technology, due to their use in a variety  of fields, have led to many improvements.


Figure 1.  Composite optical and IR image of  circuit with low BVdss  pmos devices.


We have found IR microthermography valuable in  finding circuit shorts such as the pmos devices with low  BVdss shown in Fig. 1, as well as other non-photonemitting shorts [5]


We have also found that the resolution limitation is  much less than the diffraction limited resolution  initially anticipated.  Therefore, there is clearly a need  to determine the typical range of defects to which this  sort of tool can be successfully applied..


Instrument Description


The microscope used in this work (fig. 2) employs a  512x512 liquid-nitrogen cooled, InSb focal plane array  detector and a set of large aperture lenses.  These  lenses, designed for high throughput in the 2-5µ  wavelength, infra red region, have magnification factors  of 2x, 5x and 15x.  Although higher magnification  lenses could, in theory, be fabricated, diffraction limited  resolution considerations and the need to match lens  characteristics with camera parameters dictates a  narrower range of magnifications compared to visible  light optics.


The result is that each of the 24µ (square) detector  elements is exposed to the radiation from a 1.6µ, 4.8µ, or 12µ region of the sample depending on the lens.  For  fault identification, this is adequate resolution to  distinguish one gate from another in today’s CMOS  technology. .


Figure 2.  IR microscope mounted on an 8-inch  wafer probe station.  The DUT is a  disencapsulated IC.


Our microscope is mounted on an analytical probe  station that can accommodate up to an 8-inch  diameter wafer in either front or backside mode.  Also, the prober can be configured for evaluation  boards, RF test fixtures and packaged devices.  For  wafer level analysis several micropositioners can be  configured to apply bias to the device under test, or a  probe card can be used with computer automated test  equipment.


Tool Sensitivity:  Theoretical Limitations


The infrared detection system has been modeled  using NEDT (Noise Equivalent Delta Temperature) to determine the temperature differences that can be  detected for the three different lenses (2X, 5X, and  15X) and three different hot spot sizes (>25um, 25um  and 6um).  The parameters considered in the hot spot  NEDT modeling are shown in Table I.


The minimum resolvable temperature change in mK  is presented in table II.  For the smallest hot spot  modeled this indicated that the instrument should be  able to detect a 25µ diameter heat source if the delta  temperature is at least 161mK for the 2X lens, 161mK also for the 5X lens and 269mK for the 15X  lens.


Tool Sensitivity:  Practical Limitations


The microscope can be operated in either of two  modes, “temperature mapper” and “hot-spot  detector”.  The camera actually gages radiance  which, with appropriate calibration methods, can be  converted to temperature.


The “hot spot detector” mode compares the radiance  from the device when powered up to the reference  radiance when unpowered.  The image from the  unpowered device shows details based upon the  emissivity of the various features such as metal lines, polysilicon structures, etc.


The difference between the reference image and the  delta-radiance image can be displayed as a composite  color graphic of the “delta radiance” upon the grayscale unpowered image.  The “delta-radiance” color  thresholds can be adjusted for best resolution.


.


Backside liquid crystal microscopy was attempted on  several failed ICs. However, due to the poor liquid  crystal homogeneity, insufficient backside substrate  quality and poor thermal regulation, no hot spot could  be detected. Improvements must be made to apply  this technique in a backside failure analysis flow. Infrared thermography was also evaluated, but due to  the high doping nature of the p-type substrate, no  thermal emission could be observed.


Only the Thermal Laser Stimulation technique  allowed a rapid and precise localization of the hot  spot defect from the failed IC’s backside. This newly  developed technique could, in time, replace the  traditional hot spot detection techniques. However  improvements in the application of liquid crystals on  the IC backside might challenge this view.


1. S. Khandekar and K.S. Wills, Microelectronic  Failure Analysis Desk Reference (EDFAS  publication), 4th Edition, 171-174 (1999).


2. F. Beaudoin, R. Desplats, P. Perdu, D. Patrie, G. Haller, P. Poirier, P. Jacob, and D. Lewis, ISTFA, 227-235 (2001).


3. N.M. Wu, K. Weaver, and J.H. Lin, ISTFA, 393-399 (1996).


4. K. Nikawa and S. Tozaki, ISTFA, 303-310 (1993).


5. E.I. Cole Jr., P. Tangyunyong, and D.L. Barton, IRPS, 129-136 (1998).


6. F. Beaudoin, X. Chauffleur, J.P. Fradin, P. Perdu, R. Desplats, and D. Lewis, ESREF, 1477-1482 (2001).


This study was triggered by a question posed at  EUFANET (European Failure Analysis Network). We received good advice from several EUFANET  members as well as from Michael OBEIN from  DIGIT CONCEPT. Finally we would like to thank  M. George K. Laopodis from HAMAMATSU for  performing the Infrared Thermography and Thermal  Laser Stimulation tests.


Figure 13: Thermal Laser Stimulation image obtained  through the backside with a 5x objective


Figure 14: Thermal Laser Stimulation image obtained  through the backside with a 50x objective


R. Aaron Falk


OptoMetrix, Inc., Renton, WA


Backside imaging through a silicon substrate introduces  spherical aberration at high numerical apertures. For a  typical 200 micron substrate thickness, these aberrations  limit the resolution to less than 1 micron. A theoretical  analysis of the aberrations describes the limiting factors. Means for correcting for these aberrations are described.


Backside imaging has become an important part of  semiconductor-device failure analysis. Techniques include  photo-emission1, laser scanning probes2, Schlieren thermal  mapping3, magnetic imaging4 and PICA5. These techniques  are limited to the near infrared spectrum due to the  absorption of the silicon substrate6, which limits the  potential imaging resolution of these systems.


An additional limit to the imaging resolution is aberrations  introduced as the light passes through the silicon substrate. These aberrations occur because of refractive bending at  the substrate surface. At high angles, the bending is not  proportional to the angle of incidence, but is described by  Snell's law as a ratio of sines. This process introduces  spherical aberration, which limits imaging resolution at high  numerical apertures.


This paper first reviews the basic properties of an imaging  system, in order to clarify the optical terminology used  later. The spherical aberrations produced by the silicon  substrate are then described. Finally, examples and means  for mitigating the aberration limits are discussed.


Basic Optical Imaging System


Significant confusion often occurs in imaging systems  between parameters such as magnification, numerical  aperture and resolution. The properties of a basic optical  imaging system are reviewed here to clarify the terminology  used in the analysis presented later in this paper.


Backside imaging rarely involves placing ones eye to an  eyepiece. Active, laser-based instruments typically utilize  near infrared wavelengths, which cannot be seen. Passive, thermal or photo-emission, instruments also operate in the  near infrared for backside operation and often involve  extremely weak optical sources. Backside imaging systems  can be separated into two general categories, staring and  scanning. An electronic camera, typically a CCD, is used as  the detection means in a staring system. Scanning systems  utilize a single detector and a mechanical scanner to move  the detector image point on the target. In both cases, the  resultant image is displayed on a video monitor.


The components of a basic, staring imaging system are  shown in Figure 1. A real system will be more complex and  can include components such as beam splitters for  illumination. Nonetheless, the key features of the system  can be understood from this simple configuration.


The example uses an infinite conjugate objective and a  second “tube lens”. The use of finite conjugate objective is  typical of microscopes used for visual imaging, where an  additional lens, the eyepiece is used to form a virtual image. Instrumentation microscopes typically opt for an infinite  conjugate arrangement because of the ease of adding  addition optical components in the collimated beam path  between the objective and the tube lens. For imaging  purposes, the two arrangements are seen to be identical by  reducing the spacing between the objective and the tube  lens to zero.


Image


Objective


Tube Lens


Object


f2


h2


h1


Figure 1  Infinite conjugate objective form of staring  imaging system.


Magnification


Magnification, or “X” of an objective is often the first thing  considered in objective selection. Although, other  parameters such as numerical aperture, NA, are often more  important. The overall magnification of an electronic  imaging system includes the size and resolution of the  electronic display. The optical magnification of the system  describes the geometric optical imaging properties of the  system and is given by


f f


m =   ,


where f1 and f2 are the objective lens and the tube lens focal  lengths respectively. The magnification of an infinite  conjugate lens is only defined with respect to a particular  tube lens focal length, which is arbitrarily chosen by the  objective manufacturer.


The image height, h2, in the instrument is set by the size of  the CCD array. Thus, the optical magnification of the  system determines the observable object height, h1, or fieldof-view, FOV, of the instrument,


m h


FOV


1 =


≡


For an infinite conjugate objective with "magnification", X, knowledge of both the objective manufacturer’s standard  tube lens focal length, fs and actual tube lens focal length, f2, used in the instrument are required to evaluate the  resultant FOV. Specifically,


Xf f


(3)


For a scanning system with an internal scan angle of α, the  field of view can be shown to be


X f


(4)


Clearly, the magnification, X, of an infinite conjugate  objective is an ambiguous quantity, being only a scaling  factor in defining the field of view of the instrument.


Resolution Limits


The previous geometric description of the imaging system  only defines the instrument FOV. Resolution of the  instrument is limited by one of three components, diffraction, pixelation, and optical aberration.


Diffraction


Geometric optics would imply that a perfect lens can focus  to an infinitely small spot. Diffraction takes into account the  wave nature of light, which limits the minimum spot size. A  circular lens will focus light to a spot whose radial intensity  distribution is given by


v v


J


(5)


where


2NAr vλπ≡


(6)


and


( )φ


sin


NA ≡


(7)


where J1 is the first order Bessel function, r is the radial  coordinate in the focal plane, λ is the optical wavelength, n  is the refractive index of the media (1 for air), and φ is half  of the total acceptance angle of the lens. The numerical  aperture, NA, of the lens determines the size of its focus  spot and is the critical component in determining the  diffraction limit of the lens.


The ability to just resolve two such spots is given by the  Rayleigh criteria as


51


.0


NA


λ


(8)


which represents the best possible resolution for a staring  optical system. Scanning systems such as confocal  microscopes can improve on this resolution by 20-30%.


A diffraction-limited optical system is one in which all  other limits to the resolution are smaller that the diffraction  limit. The objective must be diffraction limited in order for  the system to be diffraction limited. Most modern  objectives are diffraction-limited at the center of their FOV. However, aberrations, e.g. coma and astigmatism, will  occur as the image spot moves away from the optical  center. The FOV derived from Eqs. 3 or 4 should be no  larger than the diffraction-limited FOV indicated by the  manufacturer.


Pixelation


A diffraction-limited objective does not guarantee  diffraction-limited performance for the system. Pixelation is  another limiting factor. Electronic images are not  continuous, but are broken down into small areas called  pixels as shown in Figure 2. The diffraction limit at the  objective can be propagated through to the CCD focal  plane, yielding


pixel


md


≥


(51


'


(9)


where dpixel is the size of an individual pixel element. In a  scanning system, dpixel is defined by how often the scanned  signal is sampled.


The product of the objective focal length, f1, and NA is not  constant for even a family of objectives from a specific  manufacturer. Table 1 lists the optical parameters for a  particular family of objectives, including values of this  product. The product is nearly constant until higher “X” values, where it changes dramatically. Also included in  Table 1 are sample calculations assuming a 10 mm square  CCD array and a wavelength of 1 micron. A 512 x 512  pixel CCD of this size would have a pixel size of 19.5  micron, a good match at the lower “X” values, however, the  image is being significantly over sampled at 100X. This  over sampling results in what is sometimes referred to as "empty magnification". Another way of looking at this same  effect, is that between the 20X and 100X objectives, the  magnification increased by a factor of 5, while the  resolution only increased by a factor of 1.4! The NA, not  the magnification controls the resolution of the objective.


Figure 2  256 x 256 pixel image (a) and blowup of 32 x 32  pixel portion showing pixelation due to individual detectors  in CCD


Magnification or "X"


Focal Length (mm)


0.06


0.25


0.65


(Focal Length) * (NA)


4.8


FOV (mm)


Diffraction Limit at Objective (micron)


8.5


3.4


Diffraction Limit at CCD (micron)


17


23


78


Table 1  Example results for a family of infinite conjugate objectives assuming a 10 mm detector array and a wavelength of 1  micron. Tube lens focal length for this family is 200 millimeter.


System Aberrations


Aberrations occur in all optical systems7. Figure 3 shows  some of the aberrations that occur for a simple lens with a  single spherical surface. Spherical aberration occurs along  the optical axis, which appears as different points of focus  for rays that pass through the outer edges of the lens than  for those that pass through the center. The focal plane of  the lens is defined by the focal point of those center (paraxial) rays. Spherical aberration moves the focus closer  to the lens and limits the minimum size of the focus spot. Off axis, other aberrations occur, e.g. coma and  astigmatism. These aberrations manifest them selves as  moving the best focus away from a flat plane and as  concentrating the rays off to one side.


Lens


Focal Plane


Best Focus


Figure 3  Example of aberrations that occur in a simple  lens with a spherical surface.


Aberrations internal to the optical system will not be  corrected by the objective. For the system shown in Figure  1, both the objective and the tube lens must be diffraction  limited for the entire system to be diffraction limited. Any  additional internal optics, e.g. relay lenses used in most  scanning systems must also be diffraction limited. Most  modern optical systems utilize multi-element lens designs to  achieve diffraction-limited performance.


Aberrations in Backside Imaging


A perfect, diffraction-limited optical imaging system may  still be unable to produce diffraction-limited images. The  object being imaged is part of the total optical system and  can also affect the imaging quality of the system. For  backside imaging, the curvature and roughness of the back  surface of the silicon can significantly degrade image  quality. However, even a perfectly polished sample can  introduce aberrations in the image at high numerical  apertures.


Figure 9. Evaluation of the average temperature  deviation <∆>, which is observed in systems of  different power dissipator area F with IR lenses of  magnification 2x, 5x, and 15x.


We have so far looked at a DOE, where the dissipated


power was held constant and the temperature profile


with its peak values resulted as an outcome. The


opposite situation can be constructed too, where the  peak temperature deviation ∆max is held constant and  the power dissipation P is changed accordingly with


equation (1).  Figure 9 shows results of such a


simulation set up for peak temperature deviations ∆max=0.32K and ∆max=5.12K. The plot clearly shows  how the average temperature deviation <∆> is  underestimated for the case of small area devices.  In


case of the 2x lense this effect is significant for device  areas below 500µm2. 5x and 15x lenses reduce this  limitation to roughly 50µm2 and 5µm2.


The calibration point of about 1 degree Kelvin for the  25 x 25µ transistor dissipating 5mW under the 5X lens  shows the numerical modeling to be reasonably close, at least within experimental error.


From the numerical model it is seen that the minimum  detectable temperatures corresponding to the minimum  detectable power dissipation (MDPD) values shown in  table 3 are roughly 0.4-0.8°K for the 25 x 25µ device  and about 10° K for the 0.4 x 0.5µ device depending on  the lens.


These are somewhat larger values of minimum  detectable temperature than the NEDT model predicts  but consideration must be given to the non-ideal (low) emissivity of the uncoated samples and a number of  other mitigating factors.


The data does clearly show that circuit defects, responsible for shorted device characteristics, can be  rapidly located using infra red thermography with  spatial resolution in the sub-micron range and “deltatemperature” resolution in tenths of a degree Kelvin.


We gratefully  acknowledge the support of Kabir ElSayed from Integrated Systems Engineering for  valuable discussions about the device simulation  software.


G. F. Shade, “Photoemission Microscopy—Basic


Theory/Application”  Microelectronics Failure Analysis (4th  edition) pp. 199-212, 1999.


C. Boit, “  Photonemission Microscopy—Advanced/Theory


of


Operation” Microelectronics Failure Analysis (4th  edition) pp. 213-229, 1999.


S. Khandekar, K. S. Wills,  “Liquid Crystal  Microscopy”  Microelectronics Failure  Analysis (4th edition) pp. 171-174, 1999.


D. L. Barton, P. Tangyunyong,  “Fluorescent Microthermal Imaging” Microelectronics Failure Analysis (4th  edition) pp. 175-194, 1999.


S. Wilson, P. Sanders, et. al.,  “ Infrared  Microthermography Applications In Fault  Identification In Advanced BiCMOS  Technology.  ISTFA, Nov. 2001.


ISE Dessis is an integrated device simulator  from Integrated Systems Engineering, release 7.0, Zurich Switzerland.


<∆> (K)


∆max=5.12K


∆max=0.32K  F=1µm2


F=32µm2


Failure Analysis of Tungsten Contact Failure in a 0.13 µm CMOS  Process


Sandeep Bagchi, Sam Subramanian, Ryan Ross, James Beck, Tony Chrastecky, Vince Soorholtz, and Ed Widener


Motorola Inc., Austin, TX


For its latest generation of high performance logic  applications, Motorola employs a 0.13 µm CMOS  technology with shallow trench isolation (STI). The  contact dimension and spacing requirements for the  dense areas of the circuitry, such as the cache, are  quite aggressive. We recently encountered single bit  and massive array failures, which were traced to an  electrical short between tungsten contacts. We report  here the failure analysis, which involved electrical  and physical testing techniques.


Random single bit and massive array failures were  observed in the cache at final probe. Investigation of  the inline test structure data indicated high  confidence in contact shorting.  Further electrical  analysis was performed on an SRAM test vehicle  designed to provide direct access to the bit line (BL) and bit line bar (BLB) nodes of bit cell in the array. A schematic of the six-transistor SRAM is shown in  Figure 1(a). A plot depicting a typical sweep  performing a write and read operation in the normal  cell is shown in Figure 1(b). In this sweep, BL is held  high, the word line is turned on, and BLB is swept  from low to high to write and read ‘1’ in the bit cell. An electrical sweep of the BL and BLB nodes of a  failing SRAM bit cell is shown in Figure 1(c). The  opposing currents in BL and BLB nodes during a  write-read operation indicated that the nodes were  shorted. The extent of the short varied among  various bits. The short disappeared when the word  lines were turned off. Above analysis suggested that  the electrical short was located inside the bit cell. The top down deprocessing and SEM inspection (Figure 2) of the failing dice did not show any visible  defects at the contacts. Additional failure analysis  was performed using transmission electron  microscopy (TEM). Details of the TEM analysis  follow.


Figure 1(a). A schematic of the six-transistor SRAM  bit cell.


Figure 1(b). Plot depicting a typical sweep  performing a write and read operation in the normal  cell.


Figure 1(c). Plot depicting the electrical sweep of the  shorted bit line (BL) and bit line bar (BLB) nodes of  a failing SRAM bit cell.


Figure 2. SEM image of a deprocessed  six-transistor  SRAM bit cell. No shorts were observed between the  contacts.


TEM Analysis


The physical analysis of the dense contacts consisted  of cross-sectional TEM (XTEM) imaging and  Energy Dispersive X-Ray Spectroscopy (EDXS) of  the contact area identified to be electrically shorted. The XTEM specimen was prepared by the lift-out  method [1,2], which allowed for locating the area of  interest precisely within the TEM foil. The TEM was  operated at 200 keV energy.


An overview XTEM image of the failed contact area  is shown in Figure 3. It shows a STI feature, flanked  by tungsten contacts. The shallow trench is filled  with SiO2, and capped by plasma enhanced nitride (PEN), which acts as an etch-stop layer during  contact etch process. Above the PEN is a thin (~5  nm) layer of amorphous undoped silicon, which has  the purpose of reducing process induced damage (PID) [3]. PID results from plasma-induced radiation  damage from subsequent HDP (High Density  Plasma) process. Using HDP process, phosphosilicate glass (PSG) was deposited above the  Si layer. During XTEM analysis, the silicon layer  appeared to be unexpectedly dark and crystalline, between the contacts, suggesting that it contained at  least one element heavier than silicon.


Figure 3. An overview XTEM image of the failed


contact area.


The silicon layer was determined amorphous and  bright elsewhere in the TEM section where the  contacts were absent, as shown in Figure 4. Figure 5  shows a high-resolution XTEM  (HRXTEM) image  at higher magnification, revealing the details of the  shorted dark Si layer from Figure 3. Lattice fringes in  that image were used to identify the crystalline  material comprising the layer. Fast Fourier  Transform (FFT) of the area enclosed in the dashed  box of Figure 5 yielded spots, shown in the inset. The process of performing FFT on the lattice fringes  of an HRXTEM image area is equivalent to obtaining  a diffraction pattern from it. Thus, the spots in FFT  can be used to identify the material, by comparing it  to the diffraction pattern of known substances. For  this purpose, we used JCPDS powder XRD data. The  lattice spacings and angles closely matched with the  CoSi2 phase (JCPDS# 38-1449). The EDXS data


from the same layer is presented in Figure 6. It shows  the presence of Co and Si, thus corroborating the  FFT analysis. Co was absent in the neighboring PEN  and PSG layers.


Figure 4. An XTEM image from an area where


contacts were absent.


Figure 5. An HRXTEM image, showing lattice  fringes at the thin Si layer. The FFT of the dashed  area is shown in the upper right inset. The lower  inset lists the measurements on spots in the FFT.


Figure 6. EDXS spectrum from the thin Si layer  between two failed contacts.


Based on the above data, it was concluded that the  amorphous Si layer had inadvertently come in  contact with Co and formed CoSi2 compound. The  origin of the Co was found to be the CoSi2 in the area  at the base of the contacts. The plasma cleaning  process for the contact hole had caused the  dissociation of CoSi2, and the sputter and  redeposition of Co on the contact sidewall. The Si in  the thin layer came in contact with the Co from the  contact sidewalls, causing its silicidation. The  contacts spacing inside the bit cell is less than half of  the spacing the BL contacts. This explained  disappearance of the shorts between BL and BLB  nodes in the bit cell when the word line is turned off. The close proximity of the contacts inside the bit cell  led to virtually the full length of the silicon to be  silicided. This formed a low resistance “bridge” between adjacent contacts.


1. L. Giannuzzi , J. L. Drown, S. R. Brown, R. B. Irwin, and  F. A. Stevie, Mat. Res. Soc. Symp. Proc. ,Vol. 480, (1997), 19.


2. R. Rai, S. Subramanian, J. Conner, S. Rose, P. Schani and J. Moss, 26th International


Symposium on Testing and Failure Analysis,


(2000), 415 .


3. S.-C. Song, S. Filipiak, A. Perera, M. Turner, F. Huang, S. G. H. Anderson, L. Kang, B. Min, D. Menke, S. Tukunang, and S. Venkatesan, 2002  Symposium on VLSI Technology- Digest of


Technical Papers, (2002), 72.


Backside Photoemission and Infrared Microthermography for Rapid Debug of Compound Semiconductor Devices


S. Mitra, S. Kiefer, M. Nair, P. Sanders, J. Steele, M. Sutton, S. Wilson, H. Henry, D. Hill, M. Sadaka


Motorola Semiconductor Products Sector, Tempe, AZ 85284


Visible to infra-red photon emissions can be readily observed in compound semiconductor devices through the semi-insullating substrate and are useful in fault identification when analyzing yield problems. The techniques described here have uncovered several yield-limiting mechanisms and have lead to rapid and effective corrective measures.


Compound semiconductors, especially InGaP HBT’s,are finding many applications in telecommunications equipment but increased competition, combined with the need for shorter development times, makes rapid debug and yield enhancement critical.


Photon emission has become a pervasive method in the analysis lab for fault identification in silicon based semiconductor technology (1, 2), and infra-red thermography has found similar application for nonphoton generating defects (3).


Here we show three case studies of these techniques applied to compound semiconductor devices using the transparency of the GaAs substrates to enable imaging from the backside.


Device Description


The device design and processing of our InGaP HBT(fig. 1) makes it difficult to find the location and physical cause of a failure using standard front side photoemission techniques since the active device area is covered by a thick, metal-2 “air-bridge”. This layer blocks almost all the photoemission emanating from the device.


Emitter r


M2 Air-Bridge


Collector


Base


Figure 1. Cross Section of InGaP HBT showing device structure.


The demand for fault identification along with the difficulty of front side photoemission analysis led to the need for backside photoemission and infrared microthermography techniques. The backside emission techniques require samples without a metal layer on the backside. To remove the backmetal, a simple, multistep wet chemical process was optimized to remove the back metal and leave a smooth GaAs back surface.


Special care was given to handling and probing samples due to the fragility of these thin GaAs devices. Once our techniques were perfected, we proceeded to address several different failure modes, to identify defect sites,and to determine the physical cause for each failure mode.


Backside Photon Emission Analysis


In one case study several devices, when probed in forward base-emitter bias, showed irregular photoemission on random emitter fingers during yield monitoring front side photoemission. Under this condition the devices should light up uniformly.


Finger 5 frontside PE


Figure 2. Frontside photon emission image where non-emitting finger is barely discernable.


Analysis began with a single faulty device, which had one emitter finger showing no front side emission (Fig.


2). After removing the back metal, the backside photoemission study (Fig. 3) agreed with the front side,revealing the same finger as faulty.


Finger 5 backside PE


Figure 3. Backside photon emission image where non-emitting finger is more apparent.


No physical anomaly was detected near the “faulty”emitter finger when the device was examined with the optical microscope.


Investigating further, FIB cuts were made to isolate the base resistor from the active device region. The FIB cuts were placed on three emitter fingers: normal,faulty and normal, to compare them (Fig. 4). For all three cuts when measuring the base ballast resistor, the I-V characteristics were very close to the design value.


While attempting to probe the transistor side of the FIB cut, the metal 2 tab lifted and became detached (fig. 5).


Figure 4. FIB plan on good, “faulty” and good fingers.


Probing directly on the M1 line to the base revealed good photoemission and IV characteristics for the emitter indicating the assignable cause of the failure was poor metal-2 adhesion.


Subsequent screening and process design experiments led to a significantly more robust airbridge process and the elimination of adhesion failures.


Figure 5. Missing metal 2 tabs at site of “faulty”emitter finger.


In another case study, a InGaP-on-GaAs HBT wafer was removed from processing to investigate some minor yield problems detected at a probed electrical screen.


A map of the wafer was produced and three devices were located representing “good, bad and marginal leakage conditions.


Backside photon emission through the full thickness of the GaAs substrate was used to characterize the leakage sites on all three devices. An example is shown in Figure 6.


Figure 6. Backside PE image of GaAs HBT Icbo leakage.


The backside PE image was then recitified, scaled and superimposed upon an image from a good metalurigical microscope of the front side of the device (figure 7)providing an accurate map for navigating the subsequent physical analysis.


Figure 7. Composite image of device with backside PE image for navigating the FIB cross section.


The mechanism for these faults which appear at the corners of the device mesa (figure 8), had been previously identified and corrective measures were already in place.


Figure 8. Corner cavity in collector mesa causing Icbo leakage was corrected with a mask change and improved etch process.


IR thermography


In another case study, a “frangible” short issue was analyzed. The challenge was that these shorts were fused open at a random low current and subsequently behaved normally. The faulty devices showed an ICEO leakage that “burned out” with a few mA of current.


Using backside IR thermography analysis through the GaAs substrate, the tool was set in “movie” mode


obtaining 10 images per second of the infra red light emission while the current through the shorted device was ramped up to the point where the frangible short fused open. The “movie” was then replayed and stopped at the frame that captured the image of the fusing defect (Figure 9) providing a map for subsequent physical analysis..


A detailed SEM study along with an EDS analysis were completed after deprocessing the “faulty” sites. SEM imaging revealed many whisker like formations emanating from the emitter finger and laying across the device creating a short to the collector.


Figure 10 shows one of many such whiskers that were observed. EDS analysis and a FIB cross-section of one of these regions confirmed that the assignable cause of the frangible shorts were gold. Subsequent experiments characterized this as an integration problem that was fully resolved by optimizing both the design rules and the plating process.


Figure 9. Backside IR thermograph showing hot spots that identify the fault sites.


Figure 10. High magnification SEM view of stringer.


Since surface metal patterns often hide the active regions and because the GaAs substrates used in the fabrication of compound semiconductors are typically transparent to infrared and near-infrared radiation,backside imaging has been become a valuable tool for the rapid debug and yield enhancement of these high performance devices.


Theory/Application”Microelectronics Failure Analysis (4th edition) pp. 199-212, 1999.


C/ Boit, “ Photonemission Microscopy—Advanced/Theory


Operation”Microelectronics Failure Analysis (4th edition) pp. 213-229, 1999.


S. Wilson, P. Sanders, et. al., “ Infrared Microthermography Applications In Fault Identification In Advanced BiCMOS Technology. ISTFA, Nov. 2001.


Anton Stuffer, Peter Egger, Helmut Pohl


Infineon Technologies, Failure Analysis Munich, Germany


Antje Moffat


NPTest Inc., Ismaning, Germany


Modern package technologies like flip-chip, require measurements of transient signals from the chip backside [1], [2]. This is because frontside access is not possible while running a test pattern.


This is an established method for CMOS devices and commercial equipment is available.


This paper demonstrates the usefulness of a LaserVoltage-Prober for transient signal measurements from the backside on bipolar-devices.


For design debug and failure analysis, the measurement of transient signals, even in high speed domain, is mandatory for bipolar devices. With the use of modern packages like H-BGA or Flip-Chip backside techniques for the measurement of the transient behavior is required.


On H-BGA packages, the balls and the chip surface are on the same side. For transient measurements,which needs stimuli and therefore fixturing of the DUT in a test socket, only a backside approach can be used (see Figure 1a).


Also, as Flip-Chip packages become more common for bipolar devices, access to the active area is possible only from the backside (Figure 1b).


Therefore, common solutions for measurement of transient signals, like microprobing with pico-probes or EBEAM measurements, cannot be used any more.


As a substitution to the above mentioned frontside methods for transient measurement, a backside technique is necessary.


The optical measurement of signals with a laser might be one of the solutions for this problem, but it has been developed and investigated only for CMOStechnologies.


With the Laser-Voltage-Prober (LVP) IDS2500 from NPTest, dynamic measurements through the backside of a chip, can be done even for high frequencies(GHz). Another advantage of  this backside method is


the access to all nodes independent on the overrouting in higher metal layers.


Figure 1a: H-BGA package


Figure 1b: Flip-Chip device


But which tool can we use to make a transient measurement from the backside on bipolar-devices ?No tool is commercially available on the market which is especially made for bipolar requirements.


But is it possible to use our Laser-Voltage-Prober ?


The answer for this question is discussed in this paper.


This presentation describes the measurement setup and sample preparation used in the Infineon FA labs in munich for backside measurement of transient signals on bipolar devices and shows two examples for this measurement methods. It is demonstrated, that this approach can be used for frequencies greater than 1GHz frequency.


Laser Voltage Probing - principles


The laser voltage probing technique uses the partial transparency of silicon to IR light for the wavelength near the band gap of silicon. A pulsed IR laser beam is focused to a diffusion of interest (Figure 2). Several opto-electronic interactions occur in a electrically stimulated pn-junction when the laser beam is focused onto the junction [3], [4], [5].


One of these mechanisms is the electro-absorption(known as Franz-Keldysh effect) . The electrical field applied on the concerned pn-junction causes a change in the band gaps which results in a local change of the absorption of the laser light in the junction region.


Other mechanisms are free carrier effects such as absorption and refractive index change. The increase of the width of the depletion region reduces the number of free carriers in this volume and vice versa.


This change of the free carrier density in the junction region changes the absorption of the light due to an optical interaction between the light and the free carriers, a quasi-plasma optical effect.


The reflected laser beam is modulated in its phase(detected with phase interference detection, PIDmode) and its amplitude (detected in standard mode)with the applied stimuli of the concerned pn-junction(transistor). From this modulated reflected laser beam a waveform will be constructed (ppm absorption)from either the phase or the amplitude modulations.


In order to lock the laser clock with the measured signal, a master clock synchronized with the test pattern is needed. As with other stroboscopic methods, an endless loop of the test pattern and a trigger signal for the laser voltage prober is required.


Figure 2: principles of laser voltage probing


For imaging and navigation on the chip and noise cancellation, a second (reference)  laser is used. The optical resolution is about 500nm for the laser scan image (LSM) and is limited by the used wavelength of 1064nm.


Low Frequency Measurement


Measurement Setup and Sevice Preparation


For the first experiments, a standard bipolar device was used. The chip was mounted in a H-BGA package with a large cooling plate on the top.


To meet the working distance requirement of the LVP, the copper cooling plate had to be thinned by surface parallel polishing. For laser voltage probing,the thickness of the silicon should be in the range of 50 – 100µm.


However, it is not possible to polish the whole chip,including the package, down to this thickness as it would cause the DUT to be unstable. Also, the device would be unmountable in a test socket. Therefore, a hole is etched into the cooper cooling plate using wet chemistry and the silicon is locally ground and polished with a CNC-drilling machine (see Figure 3).


With these methods, we can achieve a die thickness in the range of 50µm with sufficient even surfaces for LVP and meet the requirement of 1mm working distance.


Afterwards, it is also essential for laser voltage probing to cover the silicon with anti-reflection


coating (ARC). For this purpose we use a low temperature CVD nitride layer.


Figure 3: Backside view of 1st DUT after preparation for LVP


For these measurements only, a simple electrical setup was used. The power supply pins of the device were connected to their spec levels and a rectangular clock was provided as a stimuli to the P_CLKIN pin.


This clock is shifted through the chip and can be controlled by an external oscilloscope at the P_CLKOUT-pin.


For the stimuli, a rectangular 10MHz signal from a standard HF-Generator was used. This signal is synchronized to the master clock and the trigger signal for the LVP (LVP master clock: 10MHz,trigger: 100kHz).


The laser-voltage-prober set-up for bipolar devices(for e.g. focus, correction ring setting) is rather simple when compared to highly integrated CMOS devices..


The structure size and the probing area (pn-junction)of bipolar devices is larger compared with more or less minimum structure size in CMOS logic blocks.


Measurement


Figure 4 and 5 show the laser scanning image (LSM)of two measurement points used for this experiment.


The probing area is the base – emitter junction region.


For the 1st measurements only the standard mode of the LVP [6] was used. This mode provides fast measurements (quicker set-up) but is less sensitive(lower SNR). It was chosen to check several values for the LVP set-up (e. g. correction ring setting).


Figure 6 shows typical waveforms measured with this standard set-up. The quality of the measured


waveforms is comparable to the results of an EBEAM used for frontside measurements of transient signals.


In contrast to CMOS devices, the impact of the LVP set-up such as focus or correction ring is less sensitive on bipolar devices. Even not corrected set-up values result in reliable measurement signals. A reason for this might be the better modulation of the reflected laser signal with the signal applied to the pn-junction(discussed later in this paper).


Also, the possible probing area is larger compared to CMOS devices.


Figure 4:  LSM image measurement point CLKIN(probing point marked) field of view 20 x 20µm


Figure 5:  LSM image measurement point CLKOUT(probing point marked), field of view 40x40µm


chip backside


Figure 6:  waveforms measured on CLKIN and CLKOUT


High Frequency Measurement


Measurement Setup and Device Preparation


The second analyzed device is a HF power amplifier manufactured with silicon bipolar technology. This device is mounted as flip-chip directly on the customers circuitry. For this measurement, devices mounted as flip-chip on an ‘application board’ are used (Figure 7). All preparations of  the device have to be done on the board. The device was ground and polished to a thickness of 80µm and anti-reflection coating was used in the same way as described above.


The whole board is mounted into the laser-voltage prober with a special adapting plate. The condition of 1mm working distance for laser-voltage is achieved with this setup.


The device is connected to the power supply and the signal in and out via HF connectors and HF cables.


For electrical stimuli, a 1.9GHz sinusoidal signal from an HF generator is used.  Several attenuator values were used to generate different amplitudes for the signal to be measured (see Table 1).


The stimuli signal is synchronized to a 10MHz master clock signal and a 100kHz trigger signal for the laser voltage prober. A loop length of 10µs is used for these measurements.


Figure 8 shows a simplified schematic of the measured circuitry.


Figure 7: 2nd DUT on ‘application board’ after preparation for laser-voltage probing


Input/Output Voltage: Vin (dbm)  Vout (V)


–4dbm     1.42V


–7dbm     1.0V


–12dbm     0.72V


–18dbm     0.35V


Table 1: Input and output values of stimuli.


Figure8: Simplified circuit schematic.


CLKIN


CLKOUT


CLKOUT 2nd


Figure 9 shows the laser scanning image (LSM) and layout. Figure 10 shows a simplified cross section of the measured device. As mentioned above, the active region on a bipolar device is the base-emitter junction and is used for the measurements. This region has the highest free carrier density enabling free carrier effects such as absorption and refractive index change.


The phase modulation  of the reflected laser light can be explained by this mechanism. Also, the area of the base-emitter diode has the largest variation of  size of the space charge region. This triggers the electro absorption and causes amplitude modulation of the reflected laser light.


The approach to measure anywhere on the basecollector diode failed.


Figure 11 shows waveforms taken in PID (top) [4]and standard (bottom) mode for different input/output levels. Especially in PID mode, the waveform reproducibility was very high and the probe position was not very critical. Even small input/output amplitudes could be probed. The relative amplitudes in Scope Tool correspond to the output voltage levels(Vout) which were measured with an external oscilloscope.


Figure 9: LSM image, layout and simplified cross section on measured point.


Figure 10: Simplified cross section of the measured bipolar transistor.


Figure 11: Waveforms measured with different amplitudes and measurement modes.


A standard laser voltage prober can be used to measure transient signals from the chip backside of bipolar silicon devices.


For both, high and low frequency domain this measurement is applicable.


A high frequency signal  of 1.9GHz with amplitudes of less than 1V can be easily measured.


No additional effort for preparation of the devices is necessary.


Measurements


The authors would like to thank H. Millinger and T.


Linzner for backside preparation and A. Dübotzky for anti-reflection coating.


Thanks to the management of the FA lab in Munich especially F. Bruns and S. Görlich for the assistance to this work.


1. Laser Voltage Probe (LVP): A Novel Optical Probing Technology for Flip-Chip Packaged Microprocessors: Wai Mun Yee. et. al, Proc. of 26th ISTFA, 3-8, (2000)


2. Optical Probing of Flip-Chip-Packaged Microprocessors: Eiles T.M. et al, Proc. of the International Solid State Circuits Conference(ISSCC), p.200, (2000)


3. Optical Processing of Semiconductors: Dover Publication Inc., New York (1971 )


4. Optical Charge Modulation as an Internal Voltage Probe for CMOS IC’s: G. Koskowich,IEEE Journal of Quantum Electronics, Vol.24 p.181, (1988)


5. Electrooptical Effects in Silicon: E. Soref and B. Bennett, IEEE Journal of Quantum Electronics, Vol. 23, p.123, (1987)


6. Optical Probing of VLSI IC’s from the Silicon Backside: Eiles, T. et al, Proc. of 25th ISTFA,27-33, (1999)


7. Integrated Circuit Waveform Probing Using Optical Phase Shift Detection: Wilsher K. et.


al,  Proc. of 26th ISTFA,  479 – 486, (2000)


Application of Focused Ion Beam in Debug and Characterization of


0.13 µm Copper Interconnect Technology


Caiwen Yuan, Mehrdad Mahanpour, Hung-Jen Lin, Gene Hill


Advanced Micro Devices, Inc. One AMD place, Sunnyvale, CA 94088-3453


Focused Ion Beam (FIB) has been widely accepted in  circuit modification and debugging of new chips and  process technologies [1]. It has the advantages of rapid  confirmation of design fixes and reducing the cost  and time to build new masks. In this paper, we will  describe the latest application of FIB to debugging  Static Random Access Memory (SRAM) test chips  processed on a dense copper metallization  technology. Examples of finding leaky capacitors  will be given. Individual transistors in the cell array  have also been “fibbed” and characterization curves  were measured. We compare the measurement with  the SPICE simulation and discuss possible damage to  the underlying transistors during FIB pad creation. Resistors in the periphery circuit were fibbed and  measured with two and four point probes. Contact  resistance was characterized and compared to that of  Al interconnects. Example of finding problem vias  with the help of cross-section and voltage contrast is  given.


The equipment we used for debugging was a FIB  200TEM from the FEI Company. The machine is  equipped with three gas injection systems (GIS). Pt  was used for depositing FIB probing pads. I2 was  used for selective metal etching. XeF2 was used for  enhanced oxide etching or etching of other dielectric  materials. With a high voltage accelerator and the  electrostatic lens system, the ion beam can be  accelerated up to 30,000 volts and focused down to a  few nanometers. The ion beam scans the sample  surface in combination with different gases from the  GIS and either deposits material or etches the surface. A detector for secondary electron or ion collects the  signal and constructs the image. Cross-section of the  sample, local circuit modification, and probe pad  creation for node monitor are typical applications of  the FIB system. Copper interconnect technology has  been gradually introduced into mainstream  semiconductor processing because its higher  conductivity gives higher integrated circuit  performance. Copper reacts differently to the etching  gas used in conventional Al FIB systems, so it is  important for us to develop and understand the new


FIB application to be able to debug and characterize  new Cu interconnect processes.


Ion channeling properties of Cu are significantly  different from those of Al and result in an increase in  the differential etching rate (among Cu grains of  different orientation) of up to three times over large  area [2]. Copper is also prone to corrosion under the  etching gases such as Chlorine, Bromine, and Iodine [3,4]. The silicon nitride layer deposited around Cu to  prevent diffusion creates faulty end-point detection.  Also, the final surface finish of the Cu backend using  the CMP process yields no visible topographical  information regarding the metal layout, which is  completely different from the Al backend.


There are many different approaches for circuit  debug due to the different circuit performance, and  characteristics of the individual circuit. In this paper, we limit our scope to SRAM circuits. SRAM has  been widely used for new process technology  qualification. A general failure analysis flow for  SRAM has been discussed by Brillert et al. [5] The  most important information for circuit debug is the  sort yield as well as the wafer level test data. New  circuits in the design are also something we need to  pay attention to. In the next few paragraphs, we are  going to describe the application of FIB in our  SRAM circuit debug.


Localization of Leaky Parts


The new SRAM we debugged had a very high  leakage current from the power pins such as Vdd  periphery and Vdd core pins. Figure 1 shows the  schematics of the ESD clamp circuit. To isolate the  leakage current, we need to cut off the paths from  Vdd periphery and Vdd core pins.


Fig1. The schematics of clamp circuit.


Figure 2 shows the layout of the clamp circuit. Green  lines are for Metal 3 (M3). Purple lines are for Metal  2 (M2), and blue lines are for Metal 1 (M1). M2 is  running from the top to bottom for Vddcore, while  the M2 of Vddperi run from top to bottom and also  connect to the M3, which run horizontally. Due to the  complicated wiring of the Vddperiphery, we decided  to start from the Vddcore pins because it is relatively  isolated. After cutting off the Vddcore as shown in  figure 3, the leakage current remains the same. This  suggests that most of the leakage current is coming  from the clamp circuit.  In the clamp circuit, the  capacitor is the primary suspect. To cut off


Fig2. Layout of clamp circuit for both Vdd core and  Vddperi. The bonding pad is on the top. The clamp  circuit is located in the center. The capacitor is on the  right.


Fig3. Image shows the Vdd core is cut off to the core.


the capacitor, we need to get down to the M1 level  from the M3 level. Fortunately, over the M1  capacitor cut point, we do not have M2, and M3 lines  can be partially cut off without affecting the


functionality of the overall circuit. After cutting off  the capacitor, the leakage current was reduced over  two orders of magnitude proving that excessive  leakage in the capacitor was not allowing that node to  charge up to Vdd as required for proper operation. We performed the same operation on the Vdd  periphery. To isolate the Vdd periphery clamp circuit, we need to cut off


Fig4. Image shows the Vdd peri have been FIB cut  and is isolated to the periphery circuit.


three sides as in figure 4. The leakage current for the  Vddperi was reduced by about the same magnitude.


SRAM Core Cell Probing


To characterize the core cell functionality, the most  common method is to check the read and write  functions. To check the individual devices, we  performed core cell FIB to test the individual  transistors. As the technology advances, the core cell  is getting smaller and smaller. That creates a  challenge for us to probe into the core cell. In the  following paragraphs, we are going to describe the  fibbing on the 0.16µm 4Meg SRAM.


Figure 5 shows the typical SRAM single bit with six  transistors. It contains two PMOS and four NMOS  transistors. To measure the core cell transistors, we  de-process the die down to the M1 level. And then  we blanket deposit about 700nm of SiO2 by CVD. Due to the wet etch before the SiO2 deposition, the  M1 metal lines clearly show up after the oxide layer  deposition. Figure 6 shows the FIB opening of three


0.2 x 0.2µm2 holes. Holes are open with the condition  of 10pA beam current. Pt pads are also deposited  with 10 pA ion beam current to avoid local heating. A total of nine probe pads are


Fig5. The schematic of the SRAM bit cell.


Fig6. Contact holes are open with 10pA beam size  and material file iee_small.mtr. Nominal size of the  hole is 0.2x0.2 µm2.


created to measure all six transistors in the single bit  cell. Figure 7 shows the optical image of this pattern. The probe pads connecting to bit line, Vdd, and Vss  can be open far away from the cell and provide space  for other probe pads. With careful consideration of  the FIB pads, we are able to FIB connect all nine FIB  pads without creating serious local heating. Figure 8  shows the measurement of one NMOS pass


Figs7. Optical view of FIB pads on the sample.


-0.2


Vds


0.5 mea


0.5 spice


1.0 mea


1.0 spice


1.5 mea


1.5 spice


Fig8. SPICE model and the measurement data  comparison.


gate transistor compared to the SPICE simulation  data. In the graph as shown in figure 8, we do not see  the leakage current, which is typically present when  such a small transistor is fibbed. Damage to the  transistor due to the ion beam from the FIB operation  is negligible. Comparing the Ids from measurement  and the SPICE model, we suspect that the reduction  of Ids in the measurement may be due to the voltage  drop to the gate.


This is the optimized condition for fibbing the  transistors in the core cell. For other conditions, we  saw gate damage as well as leakage current when  high beam current is used to open holes or deposit the  Pt pads. The lower the ion beam exposure of the  underlying device, the less damage we will create. Sometimes, to reduce the FIB exposure time of some  areas, we deposit multiple pads in serial mode, and  then, bigger patterns are deposited over the smaller  pattern. This way, the cleaning is done only once. This will also reduce the damage due to cleaning.


Resistor Measurement


A new mask set was processed on the 0.13µm Cu  process; we have zero-yield for the lot. All the  outputs are tested as logical high. What is the  problem? From the very logical point of view, the  input and output circuit should be checked first, and  then the sense amplifiers, lastly the core cell. Since  all outputs are stuck at high, some systematic  problem in the circuit is suspected. In our SRAM  design, the En_bar enables or disables the output  buffers. See figure 9 for detail.


Fig9.  Simplified output circuit.


This circuit can be tested with a FIB point at  Data_out and a FIB point at En_bar, and monitor the  output circuit with various states of En_bar and  Data_out. To make sure that the FIB points are  connected to the designated area, it is helpful to  double the FIB points, so the second one can be used  as monitor pad. What we observe is that the output  pad is always at high for all combinations of Data out  and En_bar. This information suggests that this part  of the circuit has a problem. For a functional circuit, the Output pad should follow the Data_out with  En_bar at low. And the output pad is in tri-state (or  high impedance state) for En_bar at high. To isolate  the problem, we put a FIB point before and after the  resistor. We tested the circuit again at the FIB points  before and after the resistor, with the combination of  the Data_out and En_bar. Now we see the change for  the FIB point before the resistor and stuck at high for  the FIB point after the resistor with En_bar at low. The debugging process so far has confirmed that the  problem is in the resistor. To confirm the finding, we  need to measure the resistor and check if it is in the  same range as we designed it. To measure the  resistor, we need to de-process the chip down to M1. The die is first dipped into hot (about 80C) nitric acid  solution for about 30 mins to remove the die from the  package. And then the die is plasma etched for 5  mins to remove the Nitride top layer and oxide. After  that, we CMP the die to remove the metal and plasma  etch to remove the oxide again until reaching the M1  with contact and oxide on. Figure 10 is the optical  microscope picture of the resistor. In the image, the  bright lines are M1 lines. The resistor is under the M1  and is doped silicon. It appears as a dark strip  between two M1 lines. If we put the FIB points on


the spots as in figure 10, we can measure the  resistance with 2 and 4-point techniques.


Fig10. Optical image of the resistor circuit.


The four-point probe resistor measurement shows the  value is about 103 times higher than the nominal  value. This information lead to the finding of mask  error and corrective action was implemented in the  subsequent lots resulting in good yield.


Contact resistance of Cu and Al for  FIB probes


Aluminum has been used as backend metal for over  two decades. As we approach smaller and smaller  line width, copper has been largely adopted for its  better conductivity for the 0.18 µm generation and  below. It is interesting to compare the contact  resistance between the old and new backend metals. The contact resistance of the FIB probe may be a  concern for the designer when we modify the circuit  and the balance of the input and output resistance is  critical to the overall circuitry. To compare the  contact resistance between Cu and Al, we used fourpoint probe measurement. Pt is used as FIB probe  metal. In the contact resistance calculation, we ignore  the spreading resistance between the probe and the  metal line and the resistance between the current and  voltage probe in the metal line.


Table 1 shows the contact resistance for Pt/Al and  Pt/Cu for different contact sizes. The data show that  the contact resistance for Pt/Al goes up from a few  hundred to 10 kilo ohms as the contact size reduces  from 1x1 µm to 0.25x0.25 µm, while the contact  resistance for Pt/Cu remains about a few hundreds for  different contact sizes between 1x1 µm2 and


0.25x0.25 µm2.


Output  buffer


Table1. Contact resistance between Pt and Al, Cu  lines for different sizes.


Contact size (µm2) Al (Ω)


Cu (Ω)


0.25x0.25


10554


268


0.5x0.5


591


1x1


228


367


Problem Via


During the debug of the SRAM, we have observed a  failing signature typically associated with the senseamp. The function of sense-amp is to convert the data  information from the core cell to output circuit. We  first fibbed down to the sense-amp and found out that  the last part of the circuit was functional, but the first  part of the circuit was biased at the wrong voltage. Since that portion of the via and the contacts were  newly designed, we suspect that the new process  technology may have been marginal. To check the  vias, we performed a cross-section as shown in  Figure 11.


Fig11. Circuit layout and the cross-section direction.


The cross-section at position A as shown in figure 11  shows a connection problem in the sense-amps. The  dark metal lines shown in figure 12 are the  sense_amp_enable lines. Compared to the adjacent  sense-amp, they were not properly connected. The  sense amp enables were supposed to be connected to  the bulk silicon and they are bright in the SEM image  in figure 12. So, where is the weak connection? As  we cut through position A to B, we found the answer.


Fig12. Cross-section on M3 lines as shown in figure


10. It shows the M3 are floated as the arrows shown  compare to the other sense-amps next to them.


Figure 13 shows one bad connection result in the  malfunction of the sense-amp circuit. The bad  connection is between the metal one and metal two. A via problem!


Fig13, Cross-section on M3, M2, M1 and the vias  and contacts, as shown in Figure 10. It shows the via  problem between M2 and M1.


FIB provided fast turn around time in debugging new  process or new design. Local interconnect were  created by FIB and helped us localize design  anomalies. It reduces cycle time to debug possible  errors in new process development.  Using FIB, we  localized the leaky capacitor. We found bad contacts  by cross sectioning the problem area. We  characterized the core transistor by successful FIB  pad deposition. We measured resistors and found a  mask error. By comparing the contact resistances for  both Al and Cu to Pt, the FIB pad metal, we believe  the influence from the contact resistance between Pt


and Cu is not significant when we open holes in the  quarter micron range.


We would like to thank Dokham Phengthirath for  device de-processing. We would also like to thank  David Su of TSMC for his helpful comments about  this paper.


References:


1. K.N. Hooghan, K.S. Wills, P.A. Rodriguez, S. O'Connell, "Integrated Circuit Device Repair using  FIB system: Tip, Tricks and Strategies", ISTFA, 1999, pp247-254


2. R. A. Lee, P. Wolpert, A. Pednekar, "Various  Focused Ion Beam Microsurgery Techniques in  Dealing with Copper Metallization in ICs" ISTFA, 2001, pp285-288


3. S. B. Herschbein, L.S. Fischer, A. D. Shore, M.P. Tenney, T. L. Kane, "Challenges of Focus-Ion-Beam  Chip Repair and Debug Assistance in the 0.25um  Copper Interconnect Millennium" ISTFA, 1998,


4. M. T. Abramo, L. L. Hahn, “The application of  Advanced Techniques for Complex Focus Ion Beam  Device Modification”, Microelectron. Reliab. 36 (11/12), 1775 (1996)


5. Christof Brillert, Christian Burmer and Peter  Egger. “SRAM Failure Analysis Flow”, ISTFA, 2001, pp323-329


Andrew J. Komrowski, N. S. Somcio, Daniel J. D. Sullivan, Charles R. Silvis,Luis Curiel, Jeff P. Baca, Steven Scott, and Mary Sandoval


LSI Logic Corp., Fremont, California, USA


Table 1.  Parameters considered in hot spot NEDT modeling


Camera


Heat Source


Spectral Band


Size


Quantum Efficiency


Transmission


Emissivity


Well Size


Contrast (Delta Radiance)


Pixel Pitch and Fill Factor


Cold Shield Efficiency


Dark Current


F/#


Residual Noise (A/D, etc.)


Table 2.  Simulation results for different lenses, and hot spot diameters using NEDT method


Minimum  Resolvable  Temp.


Change


(°mK)


Lens   Mag


Lens Specifications


(M=magnification, NA=numerical aperature)


Large Hot Spot


35.64


2x


M=2.00, NA=0.40 Tran=0.88


5x


M=5.00, NA=0.55, Tran=0.752


75.67


15x


M=15.0, NA=0.6, Tran=0.88


25µ Hot Spot


161.19


160.9


269.4


6µ Hot Spot


793


194


327


The “temperature mapper” mode incorporates  additional calibration steps.  During one of these  steps a shutter is brought into place under the lens .and although it is possible to set up probe needles  under the 15x lens, the working distance is marginal  and introducing the shutter for temperature mapping  is less than practical.


In this experiment the camera is in “hot spot detector  mode and two process control devices (“Scribe Grid  PC’s) were measured.  The first was a “long-wide” MOSFET that measured 25 x 25µ (gate length by  gate width).  The second was a “short-narrow” device  measuring 0.4 x 0.5µ.  Both devices were on a silicon  wafer and were analyzed in the topside microscopy  mode without coating for emissivity enhancement.


Each of the two devices were characterized with each  of the three lenses (2x, 5x and 15x) at several power  dissipations.


An example of the images obtained is shown in  figure 3.  From these images, a minimum detectable


power dissipation (MDPD) was (more or less  subjectively) arrived at and tabulated in table III.


Table 3.  Minimum detectable power dissipation  for a 0.4 x 0.5m  MOSFET and a 25 x 25m


MOSFET


Lens 0.4 x 0.5 MDPD 25 x 25 MDPD


1.00mW


1.80mW


2.00mW


A second experiment was completed in which the  camera was operated in the “temperature mapper” mode and the 25 x 25µ device was temperature  mapped with 5mW of dissipation using the 5x lens.


The results of this measurement produced a single  calibration point of about one degree Kelvin hot spot  for the 25 X 25µ transistor dissipating 5mW.


Figure 3.  Composite image taken with 15X lens of  a powered (1mw) 0.4 x 0.5m scribe grid test  transistor demonstrates a practical minimum  detectable temperature rise on an uncoated small  geometry device.


Tool Sensitivity:  Discussion


We have applied TCAD simulations to develop a  physical understanding and calibration of our  experimental measurements.  DESSIS-ISE [6] is a  numerical device simulator for electro-thermal  simulation of semiconductor structures. It is well  suited for the application in this paper, because it  allows: (1)  electrical simulations of the device under  test for evaluating the 3D distribution of the intrinsic  heat dissipation, (2) thermal simulations for the  evaluation of the 3D temperature profile, and  (3) full  electro-thermal simulations for investigating the  validity of the assumptions made in a non selfconsistent approach consisting of (1) and (2).


It is the goal of this paper to develop a simple model  for the system consisting of the device under test and  the IR detector. A suitably sized region of the  semiconductor wafer was represented by a cylindrical  silicon region as shown in figure. 4.  A doping of  1015cm-3 was chosen for the substrate and its top  surface is covered with a 10µm thick oxide as a  representation of the backend.  Two thermal contacts  are defined: One covers the complete bottom of the  substrate defining a constant temperature of T0=300K  and acting as a heat sink. The other contact is located  in the center of the silicon top surface and acts as a  heat source by dissipating a constant amount of  power per unit area. Both contacts are assumed as  infinitesimally thin in the z-direction and do not have  any intrinsic heat conductivity.


A DOE is defined, in which the area F of the top  contact is varied between 1µm2 and 1.6×104µm2 with  a total power dissipation P between 0.1mW and


25.6mW.  The depth of the substrate and radius of the  cylindrical cross section is chosen to be 250µm or  larger in order to make sure, that the adiabatic


boundary conditions for the side walls of the


simulation system do not lead to artifacts in the  temperature distribution.


Figure 4. Cross section of the simulation region  with the position of one individual pixel of the IR  detector.


Figure 5.  Radial temperature distribution for the  cylindrical simulation region near the top surface  of the substrate. Different curves refer to the  profiles of different power levels applied  to a heat  source with an area of 512mm2.


Silicon  Oxide


Pixel


z


Figure 6. Extracted maximum temperature (∆max) found in the radial temperature profile for  specified power levels, P, and heat source areas, F.


Numerical device simulation results in a 3D  temperature profile, which can be parametrized as  T(r,z) because of the cylindrical symmetry.  Temperatures are found to be highest at the top  surface of the semiconductor and the global  maximum is located around the center axis at r=0. Figure 5 shows a 1D cutline model of this radial  temperature distribution T(r,z=0) at the top surface of  the sample right under the oxide layer.


A summary of maximum temperature deviations ∆max=Tmax -T0  is given in figure 6.  The double  logarithmic plot shows that the temperature deviation  scales linearly with the dissipated power P and  inverse proportional to the square root of the  dissipation area F.   The graph follows therefore over  a wide range of conditions the simple relationship:


F P


∆max


The constant α was empirically determined as 0.6835  Kcm/W.


A simple model for the IR detector was studied, in  which the camera is viewed as an array of  pixels  with the area a. The pixel resolution can be improved  through installation of an IR lense boosting the  resolution area to A=a/M2, where M stands for the IR  lens  magnification. The average radiation power <P> received by one individual detector pixel is then  defined as:


dxdy


∫∫


>=


σ is the Stefan Boltzmann constant of the  electromagnetic black body radiation and T denotes  the 2 dimensional surface temperature distribution. We assume that the peak temperature is projected  into the center of the pixel. The average temperature  deviation <∆> read by the IR detector out of the  average radiation power can now be defined with the  relationship:


>


P σ


Equation 3 guarantees that the peak deviation ∆max  and the average deviation <∆> are identical for the  case of a constant temperature distribution.  Figure 7  shows results for the averaged temperature deviation  for the same DOE as in Figure 6 with the resolution  area A=23µm2 (24µ edge length detector pixel and 5x  lens).  It saturates to a constant value for heat source  areas, F, smaller than the resolution area, A, and it is  equal to the maximum temperature deviation ∆max for  areas F larger than A. Comparison of figure 6 and 7  shows that the detection of a surface temperature  deviation with a 5x lens for devices or defects in the  1µm2 area range is a factor of 4 too small.


Both figures. 6 and 7 are combined in figure 8  through elimination of the parameter F (power  dissipator area). It shows that the maximum  temperature for a small heat source may be much  greater than the averaged temperature for F smaller  than A, an important concern when peak  temperatures are of interest. Numerical simulations as  performed here are therefore valuable for the  estimation of the real peak temperature. Information  about the dissipated power and the area of the power  dissipator is sufficient for the extraction of this  information from figure 8.


Figure 7.  Temperature deviation profile averaged  over the resolution area A=23µm2 of a 2x IR lens.  The averaged temperature deviation <∆> saturates for heat source areas (F) smaller than  the resolution area (A).


Figure 8.  Result of a combination of Fig. 6 and 7. This figure suggests that the maximum  temperature for a small heat source may be much  greater than the averaged temperature seen by the  detector for F smaller than A.


The use of flip chip technology inside component packaging, so called flip chip in package (FCIP), is an increasingly common package type in the semiconductor industry because of high pin-counts,performance and reliability. Sample preparation methods and flows which enable physical failure analysis (PFA) of FCIP are thus in demand to characterize defects in die with these package types.


As interconnect metallization schemes become more dense and complex, access to the backside silicon of a functional device also becomes important for fault isolation test purposes. To address these requirements, a detailed PFA flow is described which chronicles the sample preparation methods necessary to isolate a physical defect in the die of an organicsubstrate FCIP.


Performing both Electronic-FA (EFA) and PFA on flip chip die poses many challenges because the metallization and active regions of the die are obstructed by the substrate from routine inspection and de-processing. When a defect in the die is suspected, one must first isolate the defect location.


This requires that the die be thinned and polished to enable photon detection techniques from the backside(for example, see 1, 2). However, photon transmission through silicon decreases with increasing silicon thickness 3:


I(x) ∝ e-x


I(x) : transmitted photon intensity


x : silicon thickness


Balancing the obvious EFA motivation to thin the die as much as possible, is the hindrance posed by performing PFA on a thin, fragile die. Typically, the die is thinned to ≤ 100 µm which prohibits the use of a mechanical shearing action to remove the die from the substrate. An alternative is to perform PFA from the backside by removing all of the silicon bulk 3.


However, it is difficult to document defects or failure sites in the Si active regions by this approach. An alternate approach is to remove the die from the package and proceed via a traditional top-down approach. This paper describes a PFA de-processing flow for a thin-die flip chip that has been developed and implemented at LSI Logic’s Analytical Services Laboratory in Fremont, CA. Since organic-laminate FCIP are quickly becoming the industry standard due to their low cost, this paper will only discuss PFA of these package types.


Thinning and Polishing the Silicon


A schematic diagram of a generic FCIP is presented in Figure 1. In FA cases where a defect in the die is suspect, the first major task of the PFA work is to prepare the flip chip die for EFA test. As stated above, this requires that the die be thinned from the backside and polished to a mirror finish while maintaining electrical functionality of the part. First,the die thinning procedure requires removal of the package’s heat spreader and stiffener. A razor blade may be used to remove the heat spreader. The blade


is forced between the heat spreader and the stiffener to defeat the adhesive. To minimize the strain on the package, the razor blade is worked around the part to all four corners.


Figure 1: Schematic cross sectional view of a FCIP.


A prudent approach to remove the stiffener depends on the substrate buildup employed in the package. It is important not to flex the substrate, die interface, or die while removing the stiffener. Thick-core, buildup substrates use a center of bismalamide triazine(BT) with nominal thickness 800 microns. The core gives the substrate rigidity -- a razor blade may be used to detach the stiffener. However, non-build-up substrates do not contain an inflexible core, and must be mounted on a solid support before removing the stiffener. In this case, it may even become necessary to thin the stiffener with an end mill in order to dislodge the metal stiffener without inducing damage in the substrate.


The package should be mounted on a metal puck in preparation for die thinning. Important characteristics to note when choosing a mounting wax are the strength, melting point, and solubility. MWH135 mounting wax from South Bay Technology provides high strength while possessing a moderate melting point. After warming the puck and wax, the wax should be spread out on the surface of the puck over an area approximately as large as the substrate. The FCIP should be mounted to the puck so that all of the balls on the substrate are in contact with the wax. Of course, the substrate must lie flat on the puck so that the die and puck surfaces are parallel. The wax is soluble in acetone. After thinning, the part may be thoroughly cleaned before EFA.


The die is thinned by mechanical grinding on diamond film (roughness: 30 µm – 1 µm). An Allied TechPrep polishing machine enabled with a MultiPrep positioning device offers grinding and polishing in a semi-automated, measured approach.


Use of a digital dial indicator allows real-time measurement of the bulk material removal. Ideally,


one would verify the reported silicon removed with a direct measurement of the silicon thickness remaining by means of confocal microscopy,ellipsometry, or reflectance spectroscopy


Additionally, there are references that describe techniques to deal with die bowing at very thin die thicknesses 4. Nevertheless, in a typical example the starting die thickness is approximately 750 µm, so the first grinding step with 30 µm roughness diamond film may be set to remove 550 µm silicon.


Additionally, 6, 3, and 1 µm film are used to thin an additional 100 µm and remove coarseness on the die surface. The final polishing step employs 0.05 µm colloidal silica and a felt polishing wheel (Imperial polishing cloth from Allied High Tech Products,Inc.). After final polish the die should be rinsed with dH2O to remove residue from the colloidal silica.


Finally, the die surface is blown dry to avoid water stains developing on the surface. The die backside should be a mirror finish at this stage.


The steps to remove the die + substrate from the puck depend once again on the substrate buildup employed in the package. Build-up substrates may be removed from the puck by reheating to soften the wax. Nonbuild-up substrates require additional steps to avoid damaging the substrate, interface, or die. For these package types, glue a spare stiffener to the substrate with epoxy. This will prevent flexing of the substrate after it is removed from the puck while enabling EFA investigation of the die backside. With the stiffener in place, the thin-core chip package may be removed from the puck by reheating the wax.


An anti-reflective coating (ARC) applied to the polished backside of the die enhances the sensitivity of EFA techniques used to isolate the location of the failing circuitry. For a description of various ARC applications in FA, see reference 5.


The die is now ready for fault isolation test.


Photoemission microscopy, thermal spot detection,and laser voltage probing are some fault isolation techniques that require transmission of a signal through the silicon. As a brief review, it should be noted that these testing techniques have been promoted by the careful preparation methods described. Specifically: (1) Taking great care not to induce damage in the package, especially that of packages with non-build-up substrates. (2) Thinning the die in order to improve photon transmission through the silicon. (3) Polishing the backside surface of the die in order to minimize scattering from the surface. (4) ARC coating in order to increase the transmitted intensity. Once a target area is identified by EFA, the location becomes the focus of subsequent PFA work.


Heat spreader Stiffener


Substrate


Balls


Bumps


Underfill Die Thermal grease


Removing the Thinned Die from the Substrate


In the common case where the fault under investigation has been isolated to the die, the PFA deprocessing challenges on FCIP are eased by the fact that the substrate becomes dispensable 6. However,special procedures must be followed when removing the thinned die from the package because the die is easily broken, thereby compromising the integrity of the target. The first step is to attach a support (silicon or glass) to the backside of the flip chip die for added strength during and after the substrate removal process. The size of the support should be slightly larger than the die, but smaller than the inner cutout of the stiffener. The bonding agent to be used should be resistant to subsequent chemical etching steps throughout the de-processing. An acceptable choice for this purpose is Masterbond Supreme 10HT, a one part epoxy. Certain two part epoxies may also work well, but when using such small quantities it can be difficult to measure out precise amounts of the epoxy and the hardener. A critical aspect in preparing the support is to spread the bonding agent out in a thin layer over an area at least as large as your die, then press your die onto the surface. This is critical because any unbonded portions of the thinned die may chip away once the substrate has been removed.


A common technique to remove a flip chip die from the substrate is to use a mechanical shearing action.


A machine devoted to this task, and routinely used to remove non-thinned flip chip die, is a rework station.


However, this technique may appear as risky or crude since many engineering hours have by now been devoted to the FA. Even though the thinned die is reinforced by a support, the die may still chip or crack—compromising the integrity of the target. An alternative approach is to remove the substrate after encapsulating the part. Although more time is required, this method is more reliable in removing the thinned die intact.


The first step in the process is to form a barrier around the die and support. Various waxes form very good barriers or temporary structures for applications in PFA flows. In this case, ordinary candle wax may be used to coat the die and support (Figure 2). For further protection, the stiffener and heat spreader are reassembled on the package to protect the die—the soft wax acts as a modest bonding agent to hold the package together. If necessary, stack two or more stiffeners together so that the height of the stiffener(s)rises above the height of the die + support: when reassembling the package, significant cracks between the package layers must be avoided. Next, the reassembled package is encapsulated in epoxy to form a puck (Figure 3). High temperature curing epoxy is satisfactory, but where time permits low temperature curing epoxy is superior because it is unlikely to disturb and displace the wax layer. Buehler Epokwick (curing time 45 min.) and Buehler Epoxide(curing time 6- 8 hrs.) are exemplary epoxies.


Figure 2: Thinned die + substrate with the stiffener in place; die covered with wax.


The thinned die may be released from the substrate and package by grinding through the substrate with a mechanical polishing wheel. In order to avoid damage to the die, it may be desirable to cut the last bit of remaining substrate material around the edge of the die. If the die doesn’t immediately release from the wax, heat the puck in an oven to flow the wax and release the die. Since the thinned die is mounted to a support, the die may be handled with tweezers.


(A)


(B)


Figure 3: Encapsulated package with thinned die,substrate, stiffener, and heat spreader ((a) top view,


(b) bottom view)


The die surface may still have package assembly materials such as organic laminate, solder bumps, and underfill attached (Figure 4). Chemical etch steps may be used to remove all of these materials to reveal the IC metallization. This is accomplished without affecting the metal interconnects of the IC. First,fuming Nitric acid heated to 80° C is employed to dissolve the underfill and any small amount of organic laminate left on the die surface. An etch time of 30 minutes should adequately remove the material in this step. Second, 70% Nitric acid should be diluted 1 : 4 in dH2O to make a solution that will remove the solder bumps by attacking the Lead. This will leave a clean die.


Figure 4: Optical image of a thinned flip chip die released from the substrate and package. Underfill and solder bumps are still attached to the die.


Removing the Redistribution / Top-layer Metallization


As a final point, we shall discuss the removal of the top layer of metal on an IC with an aluminum /tungsten metallization scheme. The top layer of metal in an IC often contains thick, wide metal lines. On a flip chip, the top layer of metal is frequently a redistribution-layer that connects the metallization of the IC to the bumps. These large metal lines can obstruct the view of the target location during PFA.


In the course of planar de-processing, regions of dense metallization lap more slowly than less dense regions. This phenomenon leads to ‘hills and valleys’on the IC surface. Throughout the process of parallellapping, multiple metal layers are exposed simultaneously at nearby areas, complicating analysis. Therefore, after the top metal layer of the IC has been visually checked for defects, it is desirable to selectively remove it. Thus, the ultimate goal of this procedure is to discretely remove the top most layer of metallization without affecting the layers beneath.


In this process, the first step is to controllably expose the top most layer of the IC with a High Density Plasma Reactive Ion Etch (HDP-RIE) process. The tool used to accomplish this task is the Nextral 860 by Unaxis. A basic silicon nitride / silicon dioxide etch removes the top passivation. It is important to monitor the exposure of the top layer of metal and to stop the etching when metal (in this layer only) is exposed since any exposed metal will be etched in subsequent steps. After the dry etch step, two wet etch steps are needed to remove the aluminum and the barrier + via material, respectively. Phosphoric acid heated to 90° C selectively etches aluminum in a step that should last 15 minutes. Next, the Ti / TiN barrier layer and the Tungsten vias are etched with a solution of Ammonium Hydroxide: Hydrogen Peroxide: Water (1:1:1) at room temperature for 45 minutes. Figure 5 presents optical images of a flip chip die prior to (A) and after (B) removal of the redistribution metallization layer.


Figure 5: Optical images of a flip chip die prior to


(A) and after (B) removing the redistribution


metallization layer


An effective physical failure analysis de-processing flow on a thin-die flip chip has been described. The


steps in the flow are specifically tailored to (1)


deliver a functional device with backside silicon


thinned, and (2) extract the thinned die from the


package and prepare it for planar deprocessing fault identification.


S. Seidel, V. R. Rao, A. N. Zaplatin and F. J.


Low, Proceedings of 25th International


Symposium for Testing and Failure


Analysis, 471-476 (1999).


W. M. Yee, M. Paniccia, T. Eiles and V. R.


Rao, Proceedings of 26th International


Analysis, 3-8 (2000).


D. Davis, O. Diaz de Leon, L. Hughes, S. V.


Pabbisetty, R. Parker, P. Scott, C. Todd, J.


Widaski, G. Wilhite, K. S. Wills and J. Zhu,Proceedings of 24th International


Symposium for Testing and Failure Analysis(1998).


T. Lundquist, E. Delenia, J. Harroun, E.


LeRoy and C. C. Tsao, Microelectronics Reliability, 41, 1545-1549 (2001).


B. Davis and W. Chi, Proceedings of 26th International Symposium for Testing and Failure Analysis, 155-160 (2000).


S. Hsiung and V. Chan, Proceedings of 26th International Symposium for Testing and


Failure Analysis, 107-115 (2000).


FAILURE MECHANISM AND ROOTCAUSE ANALYSIS  OF UBGA SOLDER BALL CONTAMINATION


Vanessa Grace Martinez Alden Almero


Quality and Reliability Department


Intel Technology Phils. Inc.


Gerard Gador


Process and Equipment Engineering Department Intel Technology Phils. Inc.


ABSTRACT


A comparison of the electrical performance and effect of different types of flux to Micro Ball Grid Array (µBGATM) solder ball quality was conducted.


The units using no clean flux were found to exhibit opens failures during off-board testing and programming. Initial analysis conducted showed that the failures were due to contact problems between the solder balls and the test/programming sockets resulting from the presence of a transparent residue on the solder balls. In-depth failure analysis, in parallel with experiments conducted in the assembly line, was performed to determine the root cause of the solder ball contamination. Three failure analysis techniques were employed, namely: Scanning Electron Microscopy (SEM), Energy Dispersive Xray Analysis (EDX), and Fourier Transform Infrared(FTIR) Spectroscopy.


An initial experiment was conducted to isolate the cause of the contamination by examining the different modules in the µBGATM assembly.


Failure analysis and experimental data proved that the opens failures were due to the no clean flux residue that was deposited on the surface of the solder ball after the reflow process.


1. 0 INTRODUCTION


Experiments were conducted to compare the electrical performance and effect of different types of flux to µBGA solder ball quality. Two types of fluxes were evaluated: the no clean flux and the water-soluble flux. Electrical performance data showed that the units using no clean flux exhibited opens failures during off-board testing and programming. Preliminary analysis revealed that


there was residue present on the affected units,primarily of carbon composition. An initial cleaning experiment was done to see if isopropanol could remove the foreign material, but to no effect.


1.1 µBGATM Package Construction


A µBGATM package is a chip-scale package (CSP)mainly used for Flash memory devices. Figures 1 and 2 show the top view and the cross-sectional view of the package. A chip scale package typically has the package area less 120% of the die area. The µBGATM package utilizes a polyimide tab tape with eutectic solder balls (63% Sn and 37% Pb). A thermosonic lead bond is used for the interconnection between the die to polyimide tape. A protective silicone elastomer compound between the die and polyimide tape absorbs stresses due to the coefficient of thermal expansion (CTE) mismatch between the package and the substrate.1


Figure 1. The µBGATM package.


Figure 2. Cross-Section of a Flash µBGATM package.


1.2 The µBGA Ball Attach Process Flow2


A ball placer cycle consists of:


1.2.1 Solder Ball Absorption


After the substrate has been loaded to mounting position, the ball placer vacuum head will move over to the solder ball supply tank. The supply tank contains the solder balls that are to be placed onto the land pads. Once over the tank, the vacuum head will descend into the reservoir. The vacuum will be activated and the tank will move in circular motion under the vacuum head. The vacuum head pick-up tool will then lift the solder balls up. Figure 3 shows an illustration of the vacuum head pick-up tool lifting the solder balls.


Figure 3. Solder ball pick-up.


1.2.2 Flux Transfer


Flux is a viscous liquid that is used to enhance the melting, flowing, and attachment of the solder balls during the heating process at the reflow oven. It also assists the mounting process by temporarily attaching the solder balls to the solder pads. Without flux, the solder balls would simply roll off and/or scatter in the substrate during vacuum release and air blow.


The ball placer combines flux application and solder ball mounting by pin transfer technology. It uses a unique process of dipping the balls into the flux and then placing them onto the substrate. After proper pick up of the solder balls has been verified, the ball placer vacuum head moves to the flux stage. A squeegee assembly uniformly spreads a layer of flux onto the table surface and the balls are dipped into the flux. Figure 4 shows an illustration of the flux application process.


Figure 4. Flux application by dipping.


1.2.3 Solder Ball Mounting


Once the solder balls are ready to be placed, the vacuum head travels over the mounting unit wherein the substrate to be processed is precisely clamped.


The head descends, turns off the vacuum, and blows air to release the absorbed solder balls. The flux temporarily adheres the solder balls to the solder pads for the pre-re-flow visual inspection and downstream re-flow process. Figure 5 illustrates this process step.


Figure 5. Solder ball placement.


1.3 The Reflow Process3


After ball placement and visual inspection, strips are loaded in the reflow oven. The equipment used is a forced convection reflow oven. During reflow, solder– in the form of solder spheres – is heated along withµBGATM frames. Using solder balls composed of 63/37 Sn-Pb alloys, the solder becomes a liquid at 183°C. When the solder is in the liquid state, a solder joint forms between two surfaces – the solder balls and copper land pads. The use of inert gas – nitrogen(N2) – during reflow helps control any potential oxide build-up.


1.4 Scope of the Problem


To determine the extent of the problem, samples of different BGA packages that use no clean flux were subjected to SEM imaging. Result showed that all packages that use no clean flux had ball contamination in various degrees. However, all of the units assembled using the water- soluble flux were clean.


Units that use no clean flux were also noted to fail pre-SMT electrical testing or pre-SMT programming.


No failures were seen for no clean flux units that already underwent SMT prior testing/programming.


2.0 EXPERIMENTAL SECTION


2.1 Failure Analysis


The no clean flux residue was identified through three basic FA techniques, namely: Scanning Electron Microscopy (SEM), Electron Disperse Xray (EDX) analysis and Fourier Transform Infra-Red(FTIR) Spectroscopy.


2.1.1 Scanning Electron Microscopy (SEM)


The SEM creates magnified images by using electrons instead of light waves. The SEM shows very detailed 3-dimensional images at much higher magnifications than is possible with a light microscope. The images created without light waves are rendered black and white. The combination of higher magnification, larger depth of focus, greater resolution, and ease of sample observation makes the SEM one of the most heavily used instruments in failure analysis today.4 In this case, the failing units were submitted for SEM imaging to confirm the presence of contamination on the solder balls.


2.1.2 Energy Dispersive X-Ray (EDX) Analysis


This technique is used in conjunction with the SEM.


An electron beam strikes the surface of a conducting sample. The energy of the beam is typically in the range 10-20keV. This causes X-rays to be emitted from the material. The energy of the X-rays emitted depends on the material under examination. By collecting and analyzing the energy of these x-rays,the constituent elements of the specimen can be determined.5 However, this is a qualitative and not a quantitative technique, which means that the amount of each element cannot be determined. This method of analysis was used to identify the elemental composition of the contamination on the solder balls.


2.1.3 Fourier Transform Infra-Red (FTIR)


Spectroscopy


FTIR spectroscopy is a powerful non-destructive analytical tool for characterizing and identifying organic molecules. FTIR spectrometers record the interaction of IR radiation with experimental samples, measuring the frequencies at which the sample absorbs the radiation and the intensities of the absorptions. Determining these frequencies allows identification of functional groups that are known to absorb light at specific frequencies.6 In order to identify the compounds that made up the


contamination on the surface of the solder balls,FTIR analysis was conducted. The spectra of reflowed flux samples and the contamination samples that were scraped off from the solder ball surface were compared.


2.2 Metrology on the Degree of Contamination


The Failure Analysis team working on the project constructed a table of metrology in order to establish a baseline method for assessing the degree of solder ball contamination. Table 1 shows the metrology used.


Table 1. Table of Metrology


Level


Degree of Contamination(per ball)


Generally clean (0%)


1%-30%


31%-60%


61%-90%


91%-100%


The degree of contamination for a unit was based on the ball/s with the highest level of contamination.


This was the metrology used for all the succeeding experiments, rework evaluations, and shift monitors.


2.3 Assembly Experiments


In order to investigate the root cause of these failures, a series of experiments were conducted.


Results of the second experiment showed that the presence of flux dictates the occurrence of contamination, and that different solder ball suppliers have no effect on the level of contamination. A combination of different flux sources (all no clean fluxes) and different ball types were used in the succeeding experiment. Contamination was found to be present on the solder balls regardless of the flux source. It validated an earlier result showing the type of solder ball used has no effect on contamination.


The oven dependency of the contamination was also confirmed. The effect of the oven on the solder ball contamination was observed in one of the experiments (this is discussed in detail below and not included in the tabular summary). No signs of contamination were seen for the samples that were not reflowed. This, along with the results of experiment 1, showed that the reflow process is needed for the contamination to occur. From the results of the last experiment, it was seen that the units that were assembled using the water-soluble


flux were free from contamination. These experiments support the FA data that the residue on the solder balls is due to a thin film of re-flowed flux.


In order to determine what causes the flux to remain on the balls, additional experiments were conducted.


These are discussed in detail in the next section.


2.4 Materials


To determine what caused the no clean flux residue to remain in the surface of the solder ball after the reflow process, fully assembled strips of µBGATM units were ran in two different types of reflow ovens using different reflow temperatures and belt speeds.


Another experiment was also run using solder balls and copper strips to validate the earlier findings.


Table 2 shows the experiment details.


Table 2. Table of Materials


Expt#


Variables Equipment


Materials


Reflow


equipment


Infrared


oven


Convection oven


1 strip of Device


X


µBGATM


per equipment


Reflow temp Belt Speed


XµBGATM per leg


Soak Time Dwell Time


Solder ball


Substrates


Copper strips


2.5 Procedure


2.5.1 Experiment 1 – Reflow Oven Experiment


This experiment was conducted to verify whether the type of reflow oven would influence the degree of no clean flux residue contamination on the solder balls.


One strip of µBGATM units was reflowed using the standard manufacturing parameters in the infrared reflow oven and in the convection reflow oven at the manufacturing floor. Samples were analyzed using SEM imaging in order to determine the degree of contamination. Table 3 shows the reflow oven parameters.


Table 3. Reflow Oven Standard Operating


Parameters


Parameter


Temp Range


Value


Ramp Rate


1-5 °C/sec


Soak Time


150-180°C


60-180 sec


Dwell Time


> 183°C


15-75 sec


Peak temp


215 + 15 °C


Cooling Rate


183-40°C


1-8°C/sec


Belt Speed


35+/-5


in/min


2.5.2 Experiment 2 – Peak Temperature and Belt


Speed Experiment


This experiment was conducted to determine the impact of different peak temperatures and belt speeds (dwell time) in a convection oven. The different parameter settings and combinations are shown in Table 4. One strip of µBGATM units was run using 8 different peak temperatures and each leg was run at two different belt speeds.


Table 4. Experiment 2 Combination Summaries


Expt. Leg Peak Temp, C Belt Speed


25, 50


240


230


220


210


7


190


185


2.5.3 Experiment 3: Soak Time and Dwell Time Experiment8


This experiment was conducted to determine what causes the flux residue to remain on the solder balls.


Another goal of the experiment was to come up with a recommendation on how to minimize the residue on the solder balls. In order to control the experiment, copper strips were used instead of solder balls. The flux was applied to the strips by printing using an 8-mil thick stencil. Figures 6-8 show the copper strip set-up.


Figure 6. The copper strip image.


A clean curve copper coupon (1x5cm) was placed almost perpendicular to the copper strip on the board using tape to stabilize the strip.


Figure 7. Bird’s eye view of the experiment setup


Figure 8. Side view of the experiment setup


The sample was the loaded in the re-flow oven using different profiles. The profile parameters are shown in Table 5. Profile A is the standard profile used in the assembly reflow process. Profile B is similar to Profile A except that the reflow zone was reduced to soak zone temperature and no dwell temperature.


Profiles C up to E used a combination of different soak and dwell times. After reflow, the set-up was inspected for the degree of contamination.


Table 5. Profile Parameters for the Experiments at the Supplier Site


Profile


Soak Time(110-183°C)


Dwell Time(> 183°C)


137 sec.


63 sec.


0 sec.


140 sec.


90 sec.


131 sec.


51 sec.


104 sec.


3. 0 RESULTS AND DISCUSSION


3.1 Failure Analysis Results


3.1.1.Scanning Electron Microscopy (SEM)


Initial failure analysis showed that the failing units had gross white residue contamination on the tab tape or solder ball side of the units when inspected through a low power scope.


However, the same residue was not observed on the surface of the solder balls. From the optical image of a contaminated solder ball shown in Figure 9, no abnormality can be seen. The physical appearance is the same as that of an unaffected solder ball.


Figure 9. Optical image of a solder ball on a failing


unit at x 20 magnification.


9. 0 REFERENCES


1. Intel, Comprehensive User’s Guide for µBGA


Packages, 1998, p.7


2. G. Gador, uBGA BARD Module 32M


Characterization Report (Rev. 01), 1998, p. 1


3. G.R. Gador and A. H. Dajac, RATIONALIZING A


“NO CLEAN” FLUX FOR µBGA™ BALL ATTACH,1999, p.4


4. Welcome to the World of Scanning Electron


Microscopy, Iowa State University


www.mse.iastate.edu/microscopy/home.html


5. www.nlectc.org/nlectcwr/edx.html


6. Fourier Transform Infrared Spectroscopy at


Aberystwyth, The University of Wales, 1997


gepasi.dbs.aber.ac.uk/roy/ftir/ftirhome.htm


7. A. Long, FA Analysis on Flux Residue, June 27,


2000, p. 1-3


10. 0 ABOUT THE AUTHORS


Vanessa Grace Martinez is a BS Chemical Engineering graduate of De La Salle University. She is currently a Package Failure Analysis Engineer for Flash memory devices. She has been with Intel for 2 years.


Alden Almero is a BS Metallurgical Engineering graduate of the Mapua Institute of Technology. He worked for four years in Intel.


Gerard Gador is a BS Chemical Engineering graduate of Santo Tomas University. He works as a BARD Module Engineer. for µBGA™ assembly. He has worked for six years in Intel.


Passivation Damage and Residue-Induced Package Failure Analysis  For a 16 Lead SOIC GaAs RF/IF Package


Daniel Cavasin,


Motorola External Final Manufacturing,


3501 Ed Bluestein Blvd, MD J4, Austin, TX, 78721.


Phone: 512 933 5225; Email: RXXS40@email.sps.mot.com


Recently, Motorola was notified that certain of their  RFIC devices had failed electrically during


Accelerated Life Testing (ALT) at their customer’s


board-mounting facility.  These devices were


assembled in both 8 and 16 lead narrow-body SOIC  packages, and had been previously qualified ‘by


comparison’ as JEDEC Moisture Sensitivity Level


(MSL) 1, indicating that the packages could be


shipped without dry packing and left indefinitely at


factory-level temperature and humidity, without the  need for pre-baking before surface mount reflow. The  returned parts exhibited delamination of the mold


compound from the die surface, in some cases


resulting in wire bond lifting. Since the parts had


been shipped as MSL1 for several years in some


cases, it was not deemed necessary to investigate


whether the customers, Motorola N.S.S. in Fort


Worth, TX, and Swindon, U.K., had implemented


any changes in their handling procedures which may  have impacted the MSL performance of the


packages.


At the beginning of February, 2000, because of the


fact that the SOIC packages were assembled at an


external subcontract facility, the issue was brought to  the attention of the Motorola External Manufacturing  Quality (EMQ) and External Final Manufacturing


(eFM) organizations. A containment action was


immediately implemented at the assembly site, which  consisted of large-scale Scanning Acoustic


Microscope (SAM) inspection of the assembled


devices, to identify delamination after post mold cure (PMC). A separate series of more in-depth


engineering analyses were also initiated, centering on  three main areas: 1, Possible die surface


contamination; 2, Possible mold compound material  issues, and 3, Possible molding process variation.  All  such activities were conducted with the support and  assistance of the IC packaging subcontractor. Results  gathered from these activities are summarized below.


Analysis


Die surface condition


After being notified of the delamination issue and  receiving a request to implement containment  procedures, the packaging subcontractor submitted a  number of the RFIC devices to an external laboratory  in Taiwan (The Materials and Electro-Optics  Research Division, Chung Shan Institute of Science  and Technology) for surface analysis.  Areas which  appeared to have passivation staining or other defects  were identified using optical microscopy. Auger  analyses performed on those devices on two separate  occasions indicated the presence of C, Cl, K, Ni, and  O in the area of the defects, while the non-defective  areas showed only trace amounts of K, present on the  surface as well as within the SiN passivation layer [1,2].


In light of these results, additional die samples from  the wafer ‘carcasses’ of the reject wafer lotb were  retrieved from storage at the Motorola GaAs wafer  fab and submitted to the Motorola Process and  Materials Characterization Lab (PMCL) in Mesa, AZ, for duplicate Auger analysis.  The latter  activities did not reveal the presence of the elements  previously identified; however, the analyses were not  performed on optically-located defective areas of the  die surface, as had been done previously [3].


In a follow up experiment, several RFIF wafers were  obtained from the wafer fab, taken from different  points in the backend process: before backgrind, after  backgrind/backmetal, after dicing, after pick and  place, after final inspection, and after ‘bagging’ (placement of the picked and placed die on dicing


frames into individual wafer carriers and Ziploc-style plastic bags for shipping). Control wafers were  also obtained for comparison. The object of the  experiment was to determine whether surface  contamination was being introduced onto the wafers  during backend processing at the fab, or as a result of  shipment in the plastic bags.


The Motorola GaAs wafer fab back end process is  unique as compared to standard Si wafer fabs. In  order to better illustrate the activities described in  subsequent sections of this report, a brief description  of the Motorola GaAs wafer fab process follows. A  schematic representation of the process flow is shown  in Figure 1.


• Gel-filled protective tape is manually  applied to the 4” wafer active surface to  protect circuitry during thinning process.


• Wafers are mechanically background to a  thickness of 12-14 mils, depending on the  product.


• Wafers are stress-relieved using a wet  chemical process, which utilizes, in various  steps, HF, H3PO4, H2SO4, HNO3, and  Acetic acids, among others. This process  removes the last 30-50um of wafer material, relieving stress retained from the mechanical  grinding process.


• The wafers are rinsed in a ‘bleach/HCl’ process which utilizes NaOCL/H20 and  HCl, in preparation for backmetal  deposition. Wafers are processed in a  vertical position for this step.


• Backmetal (Ti/Ni/V/Au) is sputtered onto  the wafer backsides.


• Gel-filled protective tape is removed and  wafers are mounted to dicing tape and film  frames for dicing.


Figure 1. Process flow for backgrind and backmetal


deposition at the Motorola GaAs wafer fab wafer fab.


After the dicing operation, the sawn wafers are  processed through a pick and place station, where the  good die are located using an electronic wafer map (no inking), and transferred robotically to a new film  frame and tape ring.  In this fashion, only good die  are shipped to the assembly sites. This procedure  obviates the requirement of the assembly sites to  implement hazardous waste processing/disposal for  the toxic GaAs material.  After an outgoing  inspection for die and saw defects, the rings are  individually packaged in Fluoroware containers,


inserted into plastic Ziploc-style bags, and shipped  to the assembly site.


The wafer samples previously discussed were  submitted for Electron Spectroscopy for Chemical  Analysis (ESCA) examination at the Motorola FMTC


Failure Analysis laboratory in Austin, TX.  Results of  the ESCA analyses were at this time interpreted as  showing no significant introduction of contaminant  materials on the sampled wafers; however, the wafer  surface locations analyzed had been randomly  selected, one site per wafer, and the surfaces were not  optically inspected prior to analysis to locate areas of  possible defects [4].


Mold Compound Material


The molding compound, Nitto MP76H is a mature  product which has been used in the semiconductor  packaging industry for several years. Although this  mold compound is not generally considered to be a  likely choice for MSL1 package qualification, the  fact that certain other narrow-body SOIC packages  had been previously qualified at MSL1 in the  packaging subcontractor using this same compound  was the basis for the extension of the MSL1 rating to  the RFIF devices in question.  In hindsight, it became  apparent that this ‘qual by comparison’ was not  appropriate, as the previously qualified devices  incorporated Si die of much smaller dimensions than  the GaAs devices being compared. This factor is  important insofar as the documented effect that  increasing die size-to-package ratio has on degrading  package moisture performance.


As with all such materials, lot-to-lot variations in the  composition of the mold compound resin or filler can  have an impact on package performance.  Therefore, information regarding the material properties of  several lots of this compound which were utilized  during the period of time when the initial failed  devices were detected was requested from Nitto  Denko Quality Assurance.  These data, consisting of  standard mold compound characterization test results  such as spiral flow, gel time, viscosity, specific  gravity, filler content, adhesion, and shear force,  were all deemed to be within normal manufacturing  specification limits [5].  In addition, Nitto had not  received any indication of material problems from  other customers using this same compound during  that time frame.


Molding Process Characterization


Extensive work was performed at the packaging  subcontractor to characterize the narrow body SOIC  molding process.  This work consisted of several  designed experiments (DOEs) which were structured  to investigate a number of different mold process  variables, and their impact on the susceptibility of the  packages to delamination.  Among the factors  examined were mold temperature, in-mold cure time, in-mold cure temperature, transfer time, pre-heat  temperature/time, and transfer pressure. Although  these experiments revealed that the mold process


Gel tape


RFIC wafer


Backgrind


Wet etch


Bleach/HCL


Sputter


Tape applied to


wafer active surface


Stress relief uses HF, HCL, other  aggressive acids


Rinse


Backmetal Deposition


Tape Removal


could be varied enough to produce delamination and  voids, it was eventually concluded that the standard  mold process being used by the packaging  subcontractor was in fact the most stable. Of further  import were the results of one DOE which  incorporated wafer material (Si vs. GaAs), mold  compound (MP76H vs MP8000), and plasma  cleaning (clean vs no clean) as the main factors. This  experiment concluded that the only significant factor  was the wafer material, as the Si was not observed to  delaminate under any of the experimental conditions


[6]. After lengthy analysis of the packaging  subcontractor’s mold process and equipment, it was  determined that the mold process was not likely to be  the root cause of the delamination.


The above activities were carried out over a period of  approximately 3 months from the time the problem  was first communicated outside Motorola W.I.S.D. Toward the end of that period, is was determined that  the issue could be best resolved by having  representatives of eFM and EMQ conduct an on-site  investigation at the packaging subcontractor.  As a  result of this action, the root cause of the  delamination phenomenon was identified as die  surface contamination.  A description of the  investigation which led to this conclusion, along with  evidence to support it, are presented in the following  section.


Root Cause Determination


After conducting an extensive line tour of the narrow  body SOIC assembly area at the packaging  subcontractor, it was found that no incoming  inspection is performed on wafers received there for  assembly. This practice had been abolished several  years previously, as is the case in many modern  packaging facilities. In an effort to determine the  surface condition of incoming wafers destined for  assembly in the suspect SOIC packages, a 100% die  high power inspection was performed on a lot of  RF1219 wafers in queue at that time.  During this  inspection, over 40 devices were identified which  exhibited some level of noticeable passivation defect. Of the 40, approximately 8 showed significant  passivation staining or ‘hazing’.  Figures 2-5 show  representative optical microscope and SEM photos of  the defective die.


Figure 2. Optical micrograph of passivation defects.


Figure 3.  Optical micrograph of passivation defects.


Figure 4. Scanning electron micrograph of  passivation defects.


Figure 5. Scanning electron micrograph of  passivation damage.


The defective devices were segregated from the main  population of die and assembled on separate lead  frame strips.  These strips were processed through the  standard assembly line and subjected to SAM  inspection after PMC.  At that time, as part of the  containment action, the standard assembly flow  included an argon plasma cleaning before wire bond.  The segregated and processed strips did not show any  signs of delamination after PMC. This effect is likely  due to the effect of the plasma cleaning on any  surface residues which may have existed on the  segregated die prior to assembly.


The 100% visual inspection was repeated on the next  lot of RF1219 wafers received.  A total of 120 die  were segregated, die attached, and sent through  assembly without the plasma clean. Of these  segregated die, approximately 40% were confirmed  to have delaminated from the mold compound, as  indicated by SAM imaging. This figure compares to  the approximately 0.25 to 1% delamination fallout  typically observed in assembly lots which had not  been plasma cleaned.  Optical micrographs of  representative die surfaces are shown in Figures 6  and 7. The SAM images of representative die  surfaces are shown in Figure 8.  Delaminated areas  are indicated by the red color in the SAM images.


Figure 6. Optical micrograph of die surface residues  and defects on segregated die.


Figure 7. Optical micrograph of die surface residues  and passivation damage on segregated die.


Figure 8. Scanning Acoustic Microscope image of  delaminated die surface interfaces on suspect die.


After similar inspection, defective die segregation, assembly, and SAM imaging of a 2nd lot, it became  evident that a correlation may exist between the  observed passivation defects and the delamination  phenomena.  The visual inspection/segregation  process was repeated on a 3rd wafer lot, which  consisted of RF289 devices.  In order to remove any  experimental bias which may have impacted the  results from the first and second experiments, the  segregated strips were replaced into the general  population of the assembly lot for standard  processing, with no plasma clean being performed on  the entire lot.  As expected, the presence of the  passivation defect was found to result in a  significantly higher percentage of delaminated parts  than observed under normal circumstances. Figures 9  and 10 show representative optical micrographs of  the die surface defects observed on this wafer lot.


Figure 9. Optical micrograph of passivation  condition.


Figure 10. Optical micrograph of passivation damage  on die surface.


Once the correlation between passivation condition  and die surface delamination had been established, the focus of the investigation was directed toward  determining what the actual delamination mechanism  was, i.e., was it a result of surface contamination, or a  mechanical separation of the passivation from the die  surface?  Several samples were collected and  returned to the Austin FMTC failure analysis  laboratory for detailed surface analysis.  The 100% visual inspection of incoming wafer material was  maintained at the packaging subcontractor factory  while the investigation proceeded.


With the newly identified die surface defects now  being the focus of activity, wafers which had been  previously obtained from the Motorola GaAs wafer  fab and analyzed using ESCA (as described in the  Background section above) were re-examined  visually.  It was found that the many of those wafers  showed passivation staining and hazing, similar to  that observed on the devices segregated from  incoming wafer lots at the packaging subcontractor.  Although most of these wafers had been processed  through dicing, one of them had been retrieved from  the process before dicing, after backgrind and  backmetal.  This wafer retained the original gel-filled  protective tape on its surface.  Visual examination of  this wafer showed significant evidence of staining, as  well as the presence of apparent chemical residues in  the passivation streets between the die.  Upon  removal of the gel-filled protective tap coating from  the die surface, a very clear pattern of residue was  observed on certain portions of the adhesive surface  of the tape material.  This pattern was a mirror image  of the passivation streets and die surfaces on the  wafer, and in many locations even had distinct  imprints of the die circuitry.  Figures 11-14 show  optical micrographs of the wafer surface staining and  the patterns observed on the gel-filled protective tape  adhesive material.


Figure 11. Optical micrograph of wafer surface  staining patterns.


Figure 12. Optical micrograph of wafer surface  staining pattern.


Figure 13. Optical micrograph showing adhesive tape  surface. Pattern is mirror image of staining seen on  wafer surface.


Figure 14. Optical micrograph showing close-up of  adhesive tape staining pattern. Wafer saw street  pattern is clearly visible on tape.


A sample of the passivation-stained material was  subject to high-resolution SEM inspection [7].  The  sample surface was observed to contain a high level  of an apparent organic residue. This residue was  observed to be heaviest in the areas of darkest  passivation staining, and became lighter on areas  adjacent to the staining.  Figures 15 and 16 show  micrographs of the surface residue observed in the  stained and adjacent areas.


Figure 15. High-resolution SEM photo of die surface   residue.


Figure 16. High resolution SEM photo of die surface  staining  in die corner.


ESCA analysis performed on the areas of die surface  contamination revealed the presence of significant  amounts of C, O, and Si, as well as smaller levels of  Au, Ga, and As. Because the Si (as SiN passivation), O (as native oxide on the passivation), Au (as the  circuit metal), Ga and As (as GaAs) are all native to  the wafer surface, it is impossible to speculate which  components may have been deposited and which may  be native, based on these data alone. It is interesting  to note that the gel-filled protective tape material is a  polydimethylsiloxane, containing a ratio of 2C:O:Si, among other trace elements.  ESCA analyses of the  adjacent areas on the wafer surface showed varying  levels of all these elements, but again, because of the  background signals, no solid conclusions could be  drawn from these data alone.


Based upon these results, data from the original  ESCA analyses performed on the Motorola GaAs  wafer fab material were re-examined.  Upon further  scrutiny, it became apparent that a significant  increase in surface C occurred on all the sample  wafers taken from downstream of the tapeapplication stage. When compared in this fashion, before and after tape application, any background  signals from the native elements on the wafer  surfaces remain fairly constant, and the obvious  increase in surface C can be inferred as resulting  from the application and removal of the tape material.  In this manner, it was determined that the gel-filled  protective tape adhesive may be a possible source of  the surface residues detected.  Figures 17 and 18  show the ESCA spectra taken from sample wafers  before and after the tape attach (backgrind) stage. (from [4]).


Carbon peak before taping


Figure 17. ESCA spectrum taken from sample of  non-taped wafer surface.


Carbon peak after taping


Figure 18. ESCA spectrum obtained from sample of  wafer surface after tape adhesive removal.


At this point it was clear that two separate  phenomena were occurring with the RFIF wafers. The passivation (SiN) surfaces on the wafers were  clearly being attacked in some fashion, most likely  chemically.  Surface contamination of an organic  nature was being deposited as well, most heavily in  the areas of passivation staining, but also in areas  where no visible staining was observed.  Because  passivation is naturally chemical-resistant, there are  few chemicals which can cause the kind of damage  observed on some of the sample wafers. It was also  known that the only organic materials which  intimately contact the surface of the wafer after the  passivation has been deposited were those present in  the gel-filled protective tape adhesive.  A suitable  explanation for both these phenomena was thus  pursued.


Archived surface analysis reports were obtained from  the Motorola GaAs wafer fab, which detailed earlier  work done to investigate the viability of several  different backgrind tape materials.  Two key reports, issued by the Motorola MRST Materials  Characterization Laboratory in 1995, provided the  information necessary to explain the observed  condition of the gel-filled protective tape material  and the SiN passivation surface.  These reports, ‘Analysis of the Outgassing Properties of Wafer  Tape’, May 2, 1995 [8], and ‘FTIR and TGA  Analysis of Wafer Tapes’, October 13, 1995 [9], noted the following.


Scanning Electron Microscopy (SEM) imaging of the opens failures revealed a contamination that covered the surface of the solder balls in various degrees.


Figure 10 shows the SEM image of the failing solder balls. It was concluded that the contamination was transparent, which is the reason why no abnormality was seen during optical visual inspection. On the other hand, units using water soluble flux had clean solder ball surface as shown in Figure 11.


Figure 10. SEM image of affected ball on a unit failing for opens.


Copper Strip


Figure 11. SEM image of a solder ball on a unit that used water soluble flux.


3.1.2 Energy Dispersive X-Ray


EDX analysis revealed that the contamination was primarily made up of carbon and oxygen. The EDX results are shown in Figure 12. It is to be noted,however, that the spectrum just shows the presence of these elements and does not give the exact quantity of each element. The height of the peaks is not an indication of the relative amount of each element.


C Peak


O Peak


Figure 12. The EDX spectrum of the contamination found on the solder balls.


3.1.3 Fourier Transform Infra Red (FTIR)Spectroscopy


FTIR results are shown in Figure 13. Results revealed that the highest match for the contamination on the opens failures was reflowed flux (78-79%).


This confirmed that the residue on the balls is due to the no clean flux.


Figure 13. FTIR spectra comparison of the residue from the failing units and the re-flowed flux.


3.2 Root cause Experiments


3.2.1 Experiment 1 – Reflow Oven Experiment


The infrared reflow oven uses infrared radiation for heating. The forced convection oven uses air (inert N2 gas) as a medium for heating. SEM imaging showed that the degree of contamination for the units reflowed using the forced convection oven was significantly greater compared to the units reflowed in the infrared reflow oven as shown in Figure 14.


Convection Oven


Infrared Oven


Level 5


Level 2


Figure 14. Experiment 1 results showing the degree of contamination.


The difference in results is probably because there is a tendency for the flux residue to be circulated in the forced convection oven. Also, the level of contamination could also be dependent on the frequency the oven was used. It was noted that the IR oven was less often used compared to the convection oven that was employed for production.


Failing unit


Reflowed flux


Table 6 summarizes the results of Experiment 2. It was observed that the degree of contamination for most of the legs was ranging from level 3-4. As seen from most of the results, a lower level of contamination was seen for the experiment legs with a lower belt speed. However, the difference between the degrees of contamination among the different belt speeds becomes less significant as the peak temperature decreases. There was no significant trend seen for the level of contamination as the peak temperature increases.


Table 6. Experiment 2 Summary of Results


Peak Temp


Level of


Contaminatio n


Plotting the contamination level versus the peak temperature, it was seen that for most cases, shown in Figure 15, a higher belt speed would result in greater contamination.


Contamination Level vs Peak Temperature


170 180 190 200 210 220 230 240 250 260


Peak Temperature (oC)


Belt Speed = 50 Belt Speed = 25


Figure 15. Trend of contamination level against the peak temperature.


3.2.3 Experiment 3 – Temperature and Dwell Time Experiment8


From the results shown in Table 7, it was seen that shortening the time of flux exposure above 183°C reduced the movement of the flux up onto the copper coupon. It was also observed that the degree of contamination is directly proportional to the soak time. A shorter soak time would result in lesser amount of flux contamination on the copper coupon.


Table 7. Experiment 3 Summary of Results


Profile Soak Time(sec)


Dwell Time(sec)


137


63


Height of


contamination is 3.5 mm from the base of the coupon.


No flux observed on the coupon.


contamination is 4.0 mm from the base of the coupon.


131


contamination is 2.0 to 2.5 mm from the base of the coupon.


104


contamination is 2.0


mm from the base of


the coupon.


Plotting the height of contamination from the base of the coupon versus the dwell time, shown in Figure 16, it is seen that the relationship between the amount of contamination and the duration of the unit in the dwell zone is almost directly proportional.


Contamination vs Dwell Time


20 40


60 80 100


Dwell Time (sec)


Figure 16. Trend of the height of contamination against dwell time


3.2.2 Experiment 2 – Peak Temperature and Belt Speed Experiment


4.3 Failure Mechanism


From the failure analysis results and the experimental data gathered, it was identified that the opens failures seen for the no clean flux units was caused by solder ball contamination. The contamination was found to be due to a thin film of no-clean flux. The capillary action of the flux upward and onto the surface of the solder balls during reflow leaves a tough residue resulting in contact problems during off-line testing and programming.


5. 0 CONCLUSION


Comparison of the performance of no clean flux vs.


water-soluble flux on µBGATM units revealed that no clean flux yielded opens failures during pre-SMT testing/programming. Solder ball contamination was found to be the cause of these electrical failures. Indepth failure analysis using various techniques was conducted on the affected units. FA results revealed that the contamination was due to a thin transparent film of no clean flux residue on the solder balls. This was validated by the experiments conducted in assembly.


6. 0 RECOMMENDATIONS


Further experiments on reflow profile optimization and its effect on no clean flux contamination should be conducted. Reducing the flux exposure above 183oC should be one of the primary considerations.


Studies on the influences in the flow of flux and solder in a bias environment can also be performed.


This can be achieved by having the substrate temperature higher than the ball temperature. It may also be possible to have different temperatures in the top and bottom preheats zones of the re-flow oven.


By setting the bottom heaters at a slightly higher temperature than the top heaters, the flow of flux and solder will have a tendency to spread and wet more on the substrate rather than the ball.7


8. 0 ACKNOWLEDGMENT


The authors would like to extend sincerest gratitude to the following people:


Mirex del Fierro for his invaluable support and leadership skills that were critical for the success of this project, and for initiating the creation of the metrology used in the experiments.


Marilin Nery and Arthur Santos for providing the SEM support crucial in the failure analysis and analysis of the experimental results.


Christopher Basilio, for the FTIR support needed in the characterization of the ball contamination.


Audrey Long, for providing the FA analysis and recommendation for Experiment 3.


Estenele Barbaza, Aldy Macatangay, Sinforoso Santillan, Rodney Macabinta, Leandro Lavilla, Nina Buenaseda, Cai Qin Luo and the rest of the team for their valuable contribution leading to the completion of this project. Good teamwork was exemplified and active participation was seen from the various crossfunctional groups (Product and Process Engineers,Planners, CQE’s, Product and Package QRE’s,Product and Package FAE’s, Material’s Group, and FATE).


Celso Co, Rommel Esteban and Deepak Goyal for their inputs and recommendations that have greatly contributed to the improvement of this paper.


Lastly, the Lord Almighty, for His constant guidance and inspiration.


• “…the adhesive on the tape is severely


attacked by the acids used in the (wet) etch  solution.”


• “The results indicated that the phosphoric  acid in the etch  had reacted with the


adhesive and had broken up its molecular


structure into a large number of smaller


fragments. This hypothesis would explain


the large increase in the mass loss observed


for the adhesives which had been exposed to  the (wet) etch.”


• “As the majority of the volatile species are  siloxane based, possible backmetal adhesion  problems could occur. Only low levels of


these tenacious compounds would be


required to cause adhesion problems due to  their very low surface free energies.” (Italics  not in original report) (Author’s note: this


comment by the analyst referred to the


outgassing and re-deposition of the volatiles  during the pumpdown process used for


backmetal deposition. It also would apply to  the actual surface in contact to the tape


material, the wafer active surface).


• “The gel-filled protective tape, while


having a reasonable outgassing performance  below 120C, unfortunately exhibits the


highest residue levels. These residues are


polydimethylsiloxane based and the low


surface free energy of these compounds


could lead to wire-bonding problems.”


In consideration of the findings in these two reports, a clearer understanding of the observed passivation  staining and surface residues observed on the RFIF  devices was formed. Referring again to Figures 11-14, it is clear that an ingress path for some liquid  contaminant exists within the wafer passivation  streets. The severe staining in the passivation streets  can be seen to terminate around corner areas of the  die, in some cases reaching far into the interior of the  die surface region.  The severe chemical attack on the  passivation, as previously noted in Figures 2-5, can  only be caused by a small number of known  chemicals; those same chemicals exist in the etch and  bleach/HCl processes which the wafer undergoes  prior to removal of the tape material.  The fact that  the staining is never observed upstream from the  application of the tape material, and is always seen  after the tape is removed, indicates that it must occur  while the tape is adhered to the wafer surface. The  photos in Figures 13-14 also clearly show that the  tape adhesive layer has undergone chemical attack as  well, as mirror-image artifacts of the wafer surface  damage and residues are visible on certain tape  regions after removal from the wafer surface.  It was  thus inferred that the passivation damage must result  from incursion of the etch chemicals from the etch  and bleach/HCl process, underneath the protective  tape layer, and into the interior regions of the wafer  surface.
  The presence of such chemicals, which had  been demonstrated to severely attack the gel-filled  protective tape adhesive and to cause substantial  increase in the outgassing weight loss of the adhesive  from the tape carrier, caused both the chemical  damage to the passivation layer, as well as the  increased tendency for deposits of tape residue to  accumulate on the wafer surface, particularly in the


areas of the greatest chemical ingress (the stained  passivation areas).  In areas of the die edges where  the chemical attack had been most damaging, the  dicing process exacerbated the damage by causing  the already-corroded passivation material to be flaked  off of the die surface.  In some cases, this latter  process resulted in removal of the bond pad material  as well.  The presence of both the chemical etch and  organic adhesive residues directly promoted the disadhesion (delamination) of the mold compound  material from the die surfaces within the SOIC  packages. This fact is supported directly by both the  demonstrated correlation of increased delamination  on die selected from areas of visible passivation  staining, as well as the reduced occurrence of  delamination when stained die are plasma cleaned  before molding.


Further support for the above observations is  provided by the original Auger surface analyses  conducted at the Chung Shan Institute of Science and  Technology, in Taiwan.  As referenced previously, this report documented the presence of C, K, Cl, Ni, and O, on surface areas of GaAs RFIF devices which  had been optically observed to show passivation  defects and staining.  It is not coincidental that the  backgrind/etch/backmetal deposition processes  involve chemicals and materials which can act as  sources for all these elements. (The K is likely  sourced from a Potassium Iodide etch which is used  to remove Au-C veils after dry etch, before  passivation deposition. The detection of K thus  indicates that at least one portion of the examined  area had passivation damage substantial enough to  allow penetration of the electron beam to underlying  layers).


Upon discovery of the interaction of the tape material  with the etch chemicals, a search of the lot histories  for the majority of the wafer lots shipped to and  assembled at the packaging subcontractor between  February and May, 2000, was performed.  The  objective of this search was to determine the length  of time that each wafer lot had spent between the  initial gel-filled protective tape application, and its  removal after backmetal deposition.  Results are  documented in Table I.


Table I. Delamination results correlated to length of  time the wafer lots spent with the gel-filled protective   tape adhered to their surface while in process at the  fab.


Wafer Lot #


# Die  assembl ed (per  assembl y lot)


# parts


delaminated


with gelfilled


protectiv e tape  coating (days)


after  PMC


after  reflow


C27520


2254


9/480 5/20 23.41


C28832


6400


1/480 0/20 6.39


“  “


2/480 0/20 6.39


6/480 0/20 6.39


5174


0/480 0/20 6.39


C28833


3223


3/480 0/20 4.02


4/480 0/20 4.02


3200


0/480 0/20 4.02


4281


5/480 0/20 4.02


C28776


6394


0/480 0/20 3.62


3190


3909


1/480 0/20 3.62


C28775


3174


0/480 0/20 3.31


6396


1/480 0/20 3.31


5882


5261


3/480 0/20 3.31


C28191


5896


7/480 0/20 2.44


"  "


4246


25/480 0/20 2.44


C28777


5900


6/480 0/20 1.42


5901


25/480 0/20 1.42


2741


7/480 0/20 1.42


C28831


0/480 0/20 0.74


4362


C28190


6106


0/480 0/20 0.48


6065


6310


4782


C26333


5061


0/480 0/20 0.42


C28968


0/480 0/20 0.34


C29283


3878


0/480 0/20 0.25


C23634


5420


0/960 0/20 0.20


5399


2/960 0/20 0.20


2604


5/960 1/20 0.20


1545


As shown in the Table, without exception, every lot  of wafers which spent more than 0.74 days with the  gel-filled protective tape adhered showed evidence of  die surface/mold compound delamination after  assembly. With the exception of one wafer lot (C23634), every lot which spent less than that period  of time with gel-filled protective tape showed zero  delamination after assembly.  Hence, the presence of  delamination is once again strongly correlated to the  presence of the gel-filled protective tape.  During  processing at the wafer fab, the wafers are usually


transferred immediately from backgrind through etch  and bleach/HCl. Any time lag between tape  application and removal will occur after the  deposition of the backmetal. It therefore appears that  the longer the period of time that the wafers age with  tape on their surfaces, after having been exposed to  the aggressive etch chemicals, the higher the  likelihood that they will delaminate in assembly.  Also, the fact that the tape is manually applied with  the possible inconsistency of initial application force, may be responsible for the variation in regions of  staining (chemical ingress, as well as the fact that  some wafers do not exhibit the staining at all. If the  application force varies around the radius of the  wafer during taping, this could result in regions of  weaker adhesion. These regions would be more likely  to dis-adhere from the wafer surface, particularly  along the locations of the passivation streets, which  are lower than the surrounding passivated surfaces, allowing easier ingress of the damaging chemicals  during the etch/rinse processes.  The hypotheses  regarding the exact mechanism responsible for  allowing chemical ingress beneath the surface tape  could not be rigorously tested, due to the  unavailability of 4” diameter wafers and the  discontinuation of the wet etch and Gel-filled


protective tape tape application processes.


Summary of Findings/ Conclusions


Investigation of the root cause of mold compound-todie surface delamination of RFIF GaAs products  packaged in 8 and 16 lead narrow body SOIC  packages at an external IC packaging subcontractor  has revealed the following.


1. Delamination is strongly correlated to areas  of passivation defects on the wafer surfaces, as well as the length of time that the wafers  spend in the wafer fab back end with the  gel-filled protective tape adhered to their  active surfaces.


2. A noticeable increase in C is observed, using  ESCA surface analysis, on the wafer  surfaces after removal of the gel-filled  protective tape material used in the  backgrind/backmetal deposition process.


3. The aggressive chemicals used in the wet  etch and bleach/HCl processes are known to  chemically attack both the SiN passivation  and the gel-filled protective tape adhesive  materials. In the latter case, it has been  demonstrated that the presence of such  chemicals substantially increases the  outgassing behavior of the tape.


4. Such passivation defects, and organic  residues, are not observed on the wafer  surfaces prior to the application of the gelfilled protective tape.


5. Wafer lots which are processed through  assembly after plasma cleaning the die  surfaces do not exhibit the delamination  phenomena.


The die surface to mold compound delamination  phenomenon observed in 8 and 16 lead narrow body  SOIC packages assembled with Motorola RFIF  devices at the IC packaging assembly site is  attributable to the deposition of tape adhesive and  other residues on the die surfaces.  These residues, along with chemical damage to the SiN passivation  layer of these devices, result from the application of  the gel-filled surface-protective tape material used  during the wafer thinning and backmetal deposition  process, in conjunction with the presence of the  highly aggressive chemicals present in the  backgrind  stress-relief and bleach/HCl surface preparation  processes.


1. Materials Test Report 89-7-590, the  Materials and Electro-Optics Research  Division, Chung Shan Institute of Science  and Technology, Lung-Tan, Taoyuan, Taiwan, R.O.C.. March 29, 2000.


2. Addendum to Materials Test Report 89-7-590, ‘2nd Auger Analysis Summary’, the  Materials and Electro-Optics Research  Division, Chung Shan Institute of Science  and Technology, Lung-Tan, Taoyuan, Taiwan, R.O.C.. April 7, 2000.


3. Chen, Gordon, ‘SAM Analysis of Nitride  Passivation in J77F’, Motorola Digital DNA  Laboratories, Process and Materials  Characterization Lab, Report No. SAM0582, March 6, 2000.


4. Cavasin, Daniel, ‘Investigation of CS1 GaAs  Wafer Surfaces as Related to Delamination  Issue on RFIC Devices Packaged in 8 and  16 Lead SOIC at the packaging  subcontractor’, Motorola eFM internal  report, May 4, 2000.


5. Takenoshita, I., ‘MP-76H/Delamination  Issue’, report # 00-04-020, Nitto Denko  Corporation, Q Quality Assurance Section, April 22, 2000.


6. ASE Chung-Li Inc, Corrective Action  Report #M000203, Rev AA, May 3, 2000.


7. Miller, Chuck, ‘GaAs package delamination  and wafer contamination’, Motorola FMTC  FA internal report, 6/3/00.


8. Cave, Nigel, and Sullivan, Eileen, ‘Analysis  of the Outgassing Properties of the Vichem  Wafer Tape’, Motorola Materials  Characterization Laboratory, Report  CA2641, May 2, 1995.


9. Cave, Nigel, and Duda, Erika, ‘FTIR and  TGA Analysis of Wafer Tapes’, Motorola  Materials Characterization Laboratory, Report CA2754, October 13, 1995.


Study on a Single NFET Degradation After Circuit   Modification with FIB


Werner Lehner


Infineon Technologies, Balanstraße 73, 81541 Munich, Germany


The use of FIB in circuit modification can generate  huge influences on MOS transistor parameters. It is  necessary to investigate and understand the effects  that occur after Ga irradiation to evaluate the  influence on the behaviour of the modified  structures. In this paper we investigate influences  on the threshold voltage of an n-FET MOS  transistor in a standard, state of the art 0.17 µm  DRAM technology, after FIB irradiation.  In  particular, the effect of varying the distance (vertical and horizontal) between the location of the  FIB modification and the active area as well as the  possibility of recovering the induced Vth shift has  been characterized.


Focused Ion beam (FIB) is one of the most  important tools for failure analysis in circuit  modification. Beside all the advantages gained by  this method, side effects should not be neglected. A  few reports deal with the influences from Ga  irradiation on MOS transistors 1,2.


In this paper we investigate the influences caused  by FIB modifications like cutting metal lines and  depositing contact pads to isolate a transistor from  a circuit and the measurement of its characteristics. The aim of all measurements was, to define the  influences of modifications at various locations, i.e. different distances to the active area and at  different metal levels (M2 to M0). Also we  investigate the possibility of recovery the effects of  FIB by annealing. As a general aim we want to  give recommendations for a best practise for circuit  modification e.g. minimal influence on the  functionality of the modified product.


Experiments


The aim of the experiments was, to see what  happens with the threshold voltage if the gate, source and drain of a MOS transistor were  contacted by FIB pads at different locations (distance to active area and different levels: M2 to  M0). Due to the design of the test structure, it was


only possible to vary the distance between the FIB  modified area and the gate at the M0 level. In  addition source and drain modifications were  possible at different metal levels but only close to  the active area.


First the gate line was contacted (M0), at several  distances from 0µm to 130 µm from the active  area. The experiment is divided into two parts: the  geometric proximity of the source pad and the  passing gate line could influence the results. For  that reason, the source kerf pad was once  electrically isolated by cutting off the connections  to the transistor and once not (Fig. 2).


Second, the source/drain lines of the transistor were  contacted at different metal levels, to see the  influences of the vertical distance. FIB pads were  created at the M2, M1, M0 levels near the active  area.


Third, source drain and gate were contacted to have  a complete contacted transistor. The gate pads were  set at 130µm and 0 µm distance to the active area, and the metal line was cut directly behind the FIB  pad. The gate distances were set to 130µm and  0µm to prevent the aforementioned influence of the  source pad.


Finally, an annealing experiment took place to  reverse the influences induced by the  modifications. The modifications consisted of a cut  from the structure pad line (gate/source/drain) and  a deposition of a contact pad (PL). The FIB-pad  size was 2x4 µm and the thickness 0.4 µm. The  modifications were made with an aperture of 80 pA  and a time of 2.5 – 3.5 min. This means a charge  dose of 1 – 1.5 nC/µ2 (Fig. 2).


All experiments were made on an n-FET MOS  transistor in the kerf (test structure) (w: 34µ/ l:


0.39µ/ gate oxide: ~4nm, see Fig.1) on a 128M


0.17µm wafer. All modifications were made with  an FEI 800 FIB system (30 KeV).


The reference point for the comparison pre and  post FIB modification, was the threshold voltage (Vth) A simplified definition for Vth for an nFET  is: Ith = 40 nA * w/l  (w,l: width/length of the  transistor). The transistors were characterised  electrically by measuring drain current (Id) versus  gate voltage (Ug) and the consequent Vth. Ug was


swept from 0.2 V, Udrain was set to 3V and source /well was set to ground (Fig. 3). For each  modification a new device was used. About three  devices were modified for each measurement point.


Figure 1: Optical image showing the test


structure


Figure 2: Schematically overview of the  transistor layout and the experimental  modifications.


Figure 3: measurement set-up


Experimental results


Gate Line Contacting


The first experiment connects the gate line at  different distances to the active area. The Id vs. Ug  curves were collected for each distance. It showed


that the most significant influence (Vth shift) happens by gate modification depending on the  distance from the modification to the active area. The highest shift occurred at 130µm distance (Fig.4). Because of the geometrical proximity of  gate line and kerf-source pad and the resulting  influence, two experiments were made. One with  electrically isolated kerf-source pad (blue curve) the other with not isolated kerf-source pad (red  curve). The different trends of the curve indicate  the influence of the source pad of the transistor. Due to this design influence, we consider for the  interpretation of the results, either only the  measurement at pad 1 on the red curve or the whole  blue curve. In both cases we can see a shift to  higher values. This indicates that the gate line was  set to a negative potential due to the modification. At the distance where the modification is close to  the source-kerf pad, the same effect, which brings  the gate line to a negative potential take place for  the source. In short, as soon as gate and source  have the same loading, the shift will be  compensated because the transistor channel is  defined by the potential difference between Ug and  Us.


Figure 4: Vth shift in relation to the modification  distance to active area. The modifications were  made along the gate line (M0). The red curve  describes the experiment with kerf source pad  influence the blue one with electrically isolated  kerf source pad.


Source/Drain/Gate Modification at M2,M1 and  M0


The next modifications were made at the source, then source/drain and finally source/gate/drain, whereby FIB pads contacted all three lines. Gate  contacts were done at M0, source/drain at  M2/M1/M0 level. The gate FIB pads were made at  two distances 0µm and 130µm, to prevent the  source influence. The result was a slight Vth shift  after source and source/drain modification. A huge  shift (125 mV) occurred at the additional  modification of the gate at 130µm and less at 0 µm (Fig. 5,6,7).


2 0


4 0


6 0


8 0


1 0 0


1 2 0


0 ,00 0 ,02 0 ,04 0 ,06 0 ,08 0 ,10 0 ,12 0 ,14


P ad  5


P a d  4


P a d  3


P a d  2


13 0


P A D  1


D is ta n ce (F IB p a d/a c tive  a re a)  / [µ m ]


G


3V


p-well


U


electrically isolated


elec. not isolated


Figure 5: Vth shift after source, source /drain and  source/drain/gate modifications at M2 level. The  gate was modified at M0 level in two distances to  active area (130µm and 0µm).


Figure 6: Vth shift after source, source /drain and  source/drain/gate modifications at M1 level. The  gate was modified at M0 level in two distances to  active area (130µm and 0µm).


Figure 7: Vth shift after source, source /drain and  source/drain/gate modifications at M1 level. The  gate was modified at M0 level for two distances to  active area. (130µm and 0µm)


Due to the design of the test structure, the gate  metallization is only modifiable at the M0 level but  at different distances to the active area. Source and


drain can be modified at all metallization levels (M2, M1, M0) but only close to the active area. Figure 8 summarizes the measured Vth shifts for  the different modifications and shows the trend to  the lowest shift for the closest distance gatemodification to active area (0µm) and for a  modification of gate/source /drain at the same  metallization level (M0).


Figure 8: Summary of the Vth shifts in dependency  of metallization level and distance to active area


Annealing Experiment


After the modification, attempts were made to  recover the Vth shift by annealing. A sample with  modified gate source and drain was measured again  after annealing at 300°C for 60 minutes at  atmosphere (Fig. 9). The result was an almost  complete compensation of the Vth shift. Noticeable  is also a shiftback of the Vth after 4 weeks of  storage.


Figure 9: Vth shift recovery after 4 weeks storing  and after 1hour annealing at 300 °C (atmosphere)


We have seen that after FIB modification the  threshold voltage shifts to higher values. The  threshold voltage is defined by the potentialdifference of gate and source and is thus dependent


0,60


0,65


0,70


0,75


0,80


0,85


0,90


1E-6 1E-5


∆U=12mV


∆U=40mV


∆U=118mV


gate:0µm


gate:130µm


___  post FIB


___  FIB pad drain


___  FIB pad source/drain


___  FIB pad source/drain/gate<0µm>


___  FIB pad source/drtain/gate<130µm>


Idrain3,48µA


Ugate[V]


∆U:110mV∆U:30mV


∆U:10mV


Idrain=3,48µA


Ugate [V]


0 0,02 0,04 0,06 0,08 0,1 0,12 0,14


Layer M2


Layer M1


Layer M0


0 µm


130 µm


0,02 0,04 0,06 0,08 0,1 0,12 0,14


120


Distance/ [µm]


__ post FIB


__ after 4 weeks


__ after annealing


∆U: 47mV∆U:125mV


___  FIB pad source/drain/gate<0µm>___  FIB pad source/drain/gate<130µm>


on the symmetrical/unsymmetrical loading of  gate/source (higher shifts at unsymmetrical  loading). The cause of the shift could be induced  by Ga+ Ion implantation in the oxide during the  modification (Fig. 11). This positive electrical  charging of the oxide can induce a static negative  mirror charging in the deposited FIB-pad or  affected metal lines, to reconstitute the electrical  equilibrium (Fig.11). This signifies a lowering of  the electrical potential of the metal line (gate). This  again causes a Vth shift to higher voltages, as  verified in the experiment (Fig. 12).


Figure 10: Equivalent circuit diagram describes the  influence of the implanted Ga-ions and the  resulting negative charging of the gate due to the  build up of mirror charges


Figure 11: Schematic overview of implanted Ga  ions and resulting mirror charges


Figure 12: Schematic explanation of the Vth shift  induced by modification.


In order to verify this hypothesis, we vary the  deposited FIB pad thickness with respect to FIB  pad-size. Due to the very small penetration depth of  the Ga+ Ion (~ 30 nm), the Vth shift should


become higher with a larger pad size, and it has to  be constant for a thicker pad: for an approximately  30nm pad thickness, no more Ga ions can penetrate  into the oxide and increase the positive charging. Otherwise with a larger pad size more Ga ions can  be placed in the oxide, which will raise the  charging effect. Both experiments were made and  the results verify the theory (Fig.13, 14).


0.02


0.04


0.08


0.12


0.14


0.16


Distance / [µm]


FIB-Pad 4x4 µm groß, 0,4 µm dick


FIB-Pad 4x4 µm groß, 0,8 µm dick


Figure 13: Variation of the FIB pad thickness. Both  curves show the same trend. For the measured  structure the kerf source pad was not electrically  isolated.


Figure 14: Variation of the FIB pad size (8x8µm  and 4x4µm). The shift becomes higher with larger  FIB pad size. At the measured structure the kerf  source pad was electrically isolated


A degradation of the gate oxide due to tunnelling  can surely be part of the Vth shift but the main  reason for it should remain the build up of mirror  charges.


If only a degradation of the gate oxide would have  taken place, no difference in the Vth versus  distance to the gate should occur because the load  due to the irradiation was the same at all distances.


0 0,05 0,1 0,15 0,2 0,25 0,3


8x8 µm FIB-Pad


4x4 µm FIB-Pad


source pad el. isolated


Usource


Usource/manipulated


Ugate


Ugate/manipulated


Vth pre FIB


Vth post FIB (gate) without source


influence


∆ Ugate/source


Vth with


gate/source  influence


+ + + + + + + + + + + + +


-   +Ga


S           D


UGS


gate line


Fib pad


Ga


- - - - - - - - - - -


We described the effect of FIB modification on  threshold voltage. The modification parameters  were oriented at real settings like they occur in  daily work. All variations (dependent on the design  possibilities) of modifications in horizontal and  vertical directions were made.


We have shown that the Vth shift is dependent on  the symmetrical/unsymmetrical irradiation of gate  and source. The shift was higher for unsymmetrical  loading. The main issue for the shift could be  identified as Ga implantation and the resultant  build up of mirror charging in the deposited pad  and affected metal lines.  Furthermore, it was  shown that the Vth shift could be almost recovered  by annealing. All these results give some hints for


future neutral modifications, which should  minimize the effects of FIB irradiation on the  electrical functionality of the modified product.


[1] Ann N Campbell et. al. The 25 th Int. Symp. for  Testing and Failure  Analysis “Focused Ion Beam  Induced Effects on MOS Transistor Parameters” (1999)


[2] Ann N Campbell et. al.  “Effects of FIB  Irradiation on MOS Transistors” IRPS `97 (1997)


New Techniques to Improve the Efficiency of TEM Sample  Preparation


Jen-Lang Lue, Jack Lee and Jian-Shing Luo


ProMOS Technologies Inc., Hsinchu, Taiwan


Three techniques have been developed for TEM  sample preparation to improve efficiency in terms of  time reduction and success rate.  The first technique  is to closely control the thickness of a sample for a  specific area to less than 10µm by mechanical  polishing before undergoing FIB thinning.  The  second one is to repair cracks produced during  mechanical polishing before further milling in the ion  miller.  The last one is to provide an in-FIB remedy for  face-to-face cross-sectional samples, which peel from  each other during mechanical polishing.  These new  techniques will substantially enhance the success  rate and turnaround time for TEM sample preparation.


In the integrated circuit (IC) industry, a transmission  electron microscope (TEM) equipped with energy  dispersive spectroscope (EDS) is one of the most  useful analytical instruments in structure analysis and  materials characterization for process evaluation and  failure analysis.  However, sample preparation for  TEM observation by focused ion beam (FIB) and  mechanical polishing is always a critical process and a  challenge even for TEM experts.


Many authors reported methods for preparing TEM  samples of specific areas using mechanical polishing  and FIB [1-5].  One of the main purposes of these  publications is to improve the success rate and  shorten preparation time.


Preparation of a specific site cross-sectional sample to  electron transparency using a focused ion beam (FIB) is widely used in the semiconductor industry.  The  conventional method [1-5] involves mechanical  polishing of the sample to a certain thickness, and FIB  milling to electron transparency.  The thickness of a  mechanically thinned sample determines the FIB  milling time and limitation of the EDS analysis.  The  thicker the mechanically thinned sample, the greater


the amount of sidewall area surrounding the final FIBthinned TEM foil.  Because the sidewalls surrounding  the thin foil may prevent the X-ray signal emitted from  the thin foil from reaching the EDS detector, the EDS  analysis may be limited by weak X-ray signal.  Generally, the more bulk silicon material removed  during mechanical thinning, the shorter the amount of  time necessary to FIB thin and the greater the  likelihood that good EDS results will be obtained.  However, monitoring sample thickness during  mechanical polishing is difficult as excessive  polishing may result in loss of the specific target area  whereas insufficient polishing may increase FIB  milling time and limit EDS analysis.  Basically, the  sample is about 20µm-75µm thick when it is ready for  FIB.  Thus how to obtain and control a desired  thickness for FIB milling becomes an interesting topic  for TEM sample preparation.  In this paper, we mainly  introduce a method to carefully thin down the sample  to less than 10µm by using a tripod polisher under the  monitoring of an optical microscope (OM).  The ease  of use and the accurate control of thickness make this  method useful in TEM sample preparation and  increase the time availability of FIB usage for other  users.


In addition, the wedge method [6] by mechanical  polishing for TEM sample preparation has been  widely used in the semiconductor industry for  process evaluation for many years.  It is well known  that some problems such as cracks and peeling can be  encountered during mechanical polishing so that they  will affect the sample quality or result in failure in the  ion miller.  In this paper, two techniques will also be  introduced to overcome these problems increasing  the success rate for TEM sample preparation.


Procedure and result


The First Technique


The tripod polisher has been used for pre-thinning  specific-area TEM samples, as noted by other authors,


for many years [3,5].  Our approach in the first  technique is to carefully control the thickness of  cross sectional TEM samples of a specific area to less  than 10µm by using the tripod polisher with a scale  ruler to measure the thickness of the sample under an  OM.


A Si (100) 256M DRAM wafer was used for sample  preparation.  The specific area for TEM was marked in  the FIB system and then the sample to be mounted  onto the L-bracket of the tripod polisher was cut to an  appropriate size (4mm x 8mm) by a wire saw.  The  backside of the chip was mounted onto an L-bracket  of a tripod polisher by wax with the cross-sectioned  surface facing the grinding wheel as shown in figure 1.  The sample was then mechanically ground and  polished using diamond lapping films of different grits  until the polished plane was down to about 1µm from  the area of interest.  An OM equipped with a scale  ruler was used to monitor the thickness as seen in  figure 2.


Figure 1: A schematic diagram showing a front view  of the sample on the L-bracket of the tripod polisher.


Figure 2: A schematic diagram showing the tripod


polisher with L-bracket that was moved to an OM to  monitor the thickness to the target.


Later, the sample was removed by placing the Lbracket onto a hot plate, and then cleaned with  acetone and alcohol.  The sample was then cut  200µm  short of the area of interest from the other side parallel  to the previously polished plane.  The sample was  then mounted onto the edge of a rectangular glass  slide by wax with the polished plane against it and  two dummy Si wafers placed beside the sample for  polishing references as shown in figure 3.  The glass  slide was then mounted onto the bottom of the Lbracket of the tripod polisher with the edge of the  glass slide parallel to the edge of the L-bracket as  seen in figure 4.


Figure 3: A schematic diagram showing the setup of  sample on glass slide for the polishing of the second  side.


Figure 4: A schematic diagram showing a bottom view  of the glass slide on the L-bracket of the tripod  polisher.


The sample was then mechanically ground and  polished by using diamond lapping films of different


grits. Polishing was stopped when the polishing plane  was less than 10µm from the area of interest as  observed by in-situ monitoring using an OM (figure 5  and figure 6).  Finally the TEM one-half Cu grid was  affixed onto the sample with epoxy and taken away  from the glass slide by dissolving in acetone as seen  in figure 7.  It then was ready for FIB milling.  A  typical FIB image of a sample with less than 10µm  thickness before further FIB milling indicates that this  method is reliable for controlling thickness as shown  in figure 8.


Figure 5: A schematic diagram showing a front view  of the sample holder (glass slide) on the L-bracket of  the tripod polisher.


Figure 6: A schematic diagram showing (a) the tripod  polisher with L-bracket that was moved to an OM to  monitor the thickness to the target. (b) An  enlargement of the area of interest on the sample, prior to removal from the glass slide.


Figure 7: A schematic diagram showing (a) the bottom  view of a glass slide on an L-bracket after the desired  thickness to the specific area is obtained, and one half  of a Cu grid is applied  (b) a sample affixed with a


TEM one-half Cu grid ready for FIB after removal from  the glass slide.


Figure 8: A typical FIB image showing 5µm thick  sample containing the specific area before FIB milling.


The Second Technique


The objective of the second technique is to repair  cracks produced during mechanical polishing of  random cross-sectional samples.  If these cracks are  not repaired, the samples may break in the ion miller.


Figure 9: A schematic diagram showing (a) the cracks  produced on the wedge shaped sample (b) the  propagation of cracks stopped by glue (c) the  propagation of cracks stopped by a laser drilled hole.


A traditional wedge method [6] was used for crosssectional TEM sample preparation.  Two chips were “sandwiched” face-to-face with epoxy, sliced and  mounted to a glass slide using wax.  After grinding  and polishing the first side, a Cu grid was affixed to


the first side by epoxy. The sample was then  dissolved from the glass slide, flipped over and  mounted with the Cu grid onto the glass slide again.


Figure 10: The typical images of an OM showing (a) cracks produced after mechanical polishing and after  epoxy glue is applied (b) cracks produced after  mechanical polishing and stopped from further  propagation by laser created holes (c) a sample with  electron transparency obtained after ion milling.


The second side of the sample was ground and  polished until the desired thickness was achieved  before ion milling to obtain a large thin electron  transparent area.  However, cracks such as those  shown in figure 9(a) might be introduced during  mechanical polishing and will propagate to affect the  success rate and quality of the TEM samples during  ion milling.


Two approaches were introduced to stop the  propagation of cracks to improve the success rate and  quality.  The first was to apply a low temperature  curing epoxy on cracks while examining the sample  under an OM.  By using a sharp tooth pick, the epoxy  can be easily applied on the cracks, and the cracks  will be protected by the epoxy , as shown in figure 9(b), during further processing.  The second was to use a  laser beam to create a hole in front of the cracks, which were close to the device structure.  The laser  system (wavelength 532nm) was mounted on an OM, and an optimized intensity of laser beam was selected  from the intensity controller of the laser system.  This  laser beam created a tiny hole in front of the crack as  shown in figure 9(c), and effectively stopped the  propagation of cracks during ion milling in the ion  miller.  Figure 10 shows typical OM images with  cracks produced after mechanical polishing, and  repaired by glue and laser beam.  The repaired cracks  will not propagate into the interface and cause the  sample to fail during ion milling (figure 10(c)).  This  method improved the success rate for TEM sample  preparation.


The Third Technique


Our approach in this technique is to provide an in-FIB  remedy for random cross-sectional samples, which  can peel from each other during mechanical polishing.


The same wedge method [6] described before is also  used for cross-sectional TEM sample preparation. The front sides of two chips were sandwiched with  epoxy.  The procedure to obtain a thin area was the  same as described in the second technique.  However, peeling between the two front sides of the chips can  occur as shown in figure 11(a), during polishing or ion  milling.  Peeling will influence further milling quality  and make it difficult to obtain a thin area.


A method of in-FIB remedy was introduced to  increase the success rate.  The samples were  separately covered with two new one-half Cu grids  with a 1mm inner diameter, parallel to the peeling  surface at a certain distance.  The original Cu grid was  then cut very carefully into two pieces with a sharp  knife.  Two samples with one-half grids were then  ready for FIB milling as shown in figure 11.  The  typical optical micrographs are shown in figure 12 and  demonstrate the practicality of this technique once  the samples peel away from each other.


Figure 11:  Schematic diagram showing the procedure  of an in-FIB remedy for face-to-face cross-sectional  samples, which can peel from each other during  mechanical polishing


Figure 12:  The typical images of an OM showing (a) the in-FIB remedy sample is covered with two onehalf Cu grids.  (b) An enlargement of the sample as  tilted with an angle.


Three techniques have been developed for TEM


sample preparation to improve efficiency in terms of


time reduction and success rate.  The first technique


is to control carefully the thickness of the sample for a


specific area to less than 10µm by mechanical


polishing before undergoing FIB thinning.  The


second one is to repair cracks produced during


mechanical polishing before further milling in the ion


miller.  The last one is to provide an in-FIB remedy for


face-to-face cross-sectional samples, which peel from


each other during mechanical polishing.  These new


techniques will substantially enhance the success


rate and decrease the time needed for TEM                   sample preparation.


The authors would like to present our thanks to Mrs. Tina Lin in the TEM group for her sample preparation.


1. S. Morris, S. Tatti, E. Black, N. Dickson, H. Mendez, B. Schwiesow, and R. Pyle, Proc. 17th  ISTFA (1991) p417.


2. E. C. G Kirk, D. A. Williams and H. Ahmed, Inst. Phys. Conf. Ser. No. 100 (1989) p501.


3. R. Anderson and S. J. Kelpeis, Mater. Res. Soc. Symp. Proc. Vol. 480 (1997) P187.


4. R. J. Young, E. C. G. Kirk, D. A. Williams and H. Ahmed, Mater. Res. Soc. Symp. Proc. Vol. 199 (1990) P205.


5. A. J. Leslie, K. L. Pey, K. S. Sim, M. T. F. Beh and  G. P. Goh, Proc. 21st ISTFA (1995) p353.


6. E. Fuchs, H. Oppolzer, H. Rehme, Particle Beam  Microanalysis, p. 165, VCH, Weinheim (1990).


A Transmission X-ray Microscope (TXM) for


Non-destructive 3D Imaging of ICs at Sub-100 nm Resolution


Steve Wang*, Frederick Duewer, Shashidar Kamath, Christopher Kelly,  Alan Lyon, Kenneth Nill, David Scott, David Trapp, and Wenbing Yun* Xradia, Inc., 4075A Sprig Drive, Concord, CA 94520


Suneeta Neogi*, Markus Kuhn, and Casey Bennet


Intel Corporation, 2501 N. W. 229th Street, Hillsboro, OR 97124


Peter Coon and Souping Yan


Intel Corporation, 2200 Mission College Blvd., Santa Clara, CA 95052


*Correspondence should be sent to the following authors: Steve Wang at swang@xradia.com, Wenbing Yun at wyun@xradia.com, and Suneeta Neogi at suneeta.neogi@intel.com.


Abstract: Xradia has developed a laboratory table-top transmission x-ray microscope, TXM 54-80, that uses 5.4 keV x-ray radiation to nondestructively image buried submicron structures in integrated circuits with at better than 80 nm 2D resolution.  With an  integrated tomographic imaging system, a series of x-ray projections through a full IC  stack, which may include tens of micrometers of silicon substrate and several layers of  Cu interconnects, can be collected and reconstructed to produce a 3D image of the IC  structure at 100 nm resolution, thereby allowing the user to detect, localize, and characterize buried defects without having to conduct layer by layer deprocessing and inspection that are typical of conventional destructive failure analysis.  In addition to being a  powerful tool for both failure analysis and IC process development, the TXM may also  facilitate or supplant investigations using scanning electron microscopy (SEM), transmission electron microscopy (TEM), and focused ion beam (FIB) tools, which generally require destructive sample preparation and a vacuum environment.


Hard x rays are ideally suited for imaging the 3D


structure of semiconductor integrated circuits


(ICs) at high resolution using tomographic techniques (discussed in more detail in sections 3).


An attribute that TXM has in common with electron microscopes is the short wavelength − 2.3Å


for the microscope described in this paper.  This


value is much less than the spatial resolution of


the imaging optics, hence the objective lens can


have very low numerical aperture (NA) of 0.001


to 0.01.  This low NA leads to relatively large


working distance and depth of field, both critically important for tomographic imaging: the


long working distance allows the sample to be


rotated to large projection angles without interfering with the optics and the large depth of field  allows a large region of interest to be maintained  in focus when the sample is rotated.


X rays, however, have many advantages over  charged particles: (1) X-ray absorption is highly  material dependent, especially between low-Z  dielectric materials such as organic and Si-based  dielectric materials, and high-Z conducting materials such as copper and tantalum. Consequently, x-ray images often show high intrinsic  contrast between interconnect and dielectric materials.  (2) X rays are weakly absorbed by ambient air and the silicon substrate, so that an  electrically functional IC with its Si substrate


locally-thinned to about 10 micrometers can be  imaged in an ambient air environment, unlike  other high resolution imaging tools such as  SEM, TEM, and FIB. (3) There is practically no  charging effect with x-ray imaging.  (4) The  damage to the sample is about two to four orders  of magnitudes less when imaging with x rays  than with electrons.  These advantages make it  possible to develop powerful and convenient xray imaging tools for non-destructive imaging of  the internal structure of semiconductor ICs.


On the other hand, imaging systems using  charged particles have the advantage that, at  high energies, it is easier to focus charged particles than electromagnetic radiation.  TEM can  achieve atomic resolution while the highest resolution demonstrated in x-ray microscopy is  about 25 nm.


X-ray nanotomography with a 3D resolution of  about 100 nm was first demonstrated by Haddad  et. al. [1].  More recently, biological specimens


have been imaged with a 25-nm resolution in 2D


[2], and 80-100 nm resolution in 3D [3, 4].  The  application of these techniques to 3D imaging of  semiconductor ICs was demonstrated through  computer simulations that revealed a great potential for non-destructive visualization of internal structures [5].  Following demonstrations of  3D imaging of simple metal structures in silicon [6, 7], high-resolution x-ray imaging of microchips using x rays capable of penetrating a full  IC stack has been recently demonstrated [8-9].  These cited demonstrations have all employed  synchrotron radiation sources that are impractical for industrial applications.


Xradia has developed the first practical  laboratory-based x-ray microscope with fully  integrated tomographic imaging capability.  Its  optical train is similar to that of an electron  or  visible light microscope, consisting of an x-ray  source, condenser lens, objective lens, and detector system.  The tool has demonstrated 2D  imaging resolution of better than 80 nm and


1 10 100


4000


6000


8000


10000


Energy(keV)


Figure 1: X-ray interaction lengths in Si, Cu, and Ta (from top to bottom).  The attenuation  length refers to the thickness required to absorb 1/e or about 37% of incident x rays.  Absorption contrast is quite high between Si and Cu or Ta.  At 5.4 keV, an IC with a total Si thickness of up to tens of micrometers can be imaged.


maximum 3D resolution of 100 nm in the transverse direction and 200 nm in the longitudinal  direction.  The Xradia TXM microscope is designed to image unpackaged ICs without affecting their electrical functionality by locally thinning the silicon substrate to a few tens of micrometers near the region of interest (more details on sample preparation can be found in section 4).  A data set for 3D tomographic imaging  is acquired by taking a series of 2D projection  images of the IC at multiple tilt angles relative to  the x-ray beam.  These projection images are  then mathematically reconstructed to produce a  3D image of the IC stack. This process takes  between 1 to 10 hours, depending on the line  width and complexity of the IC structure.  ICs  with finer line structures require more time.  As  an example, tomographic imaging of an IC with  multiple copper lines of 120 nm width requires 6  to 10 hours.  An additional 3D imaging mode, the stereo mode, allows the user to acquire two  images with approximately 20º angular separation in about 20 minutes, and view them with a  stereo goggle.  This imaging mode allows the  user to qualitatively examine the 3D structure of  a chip, but does not provide quantitative 3D information.


2. X-ray Imaging Contrast Mechanism for  Important Materials in IC Fabrications


Absorption contrast has been used in nearly all  commercial x-ray imaging equipment, including  printed circuit board (PCB) inspection tools and  medical x-ray computed tomography (CT) scanners.  The attenuation length (the thickness  through which x-ray transmission is reduced by  1/e or about 37%) varies with atomic number, density, and x-ray energy, so that variations in  sample composition can lead to large differences  in x-ray absorption contrast [10].  As shown in  Fig. 1, the tabulated [11] x-ray linear attenuation  lengths of Cu and Ta are significantly smaller  than Si, providing an intrinsic absorption conProjection at angle θ acquired.


object


lens


detector


projection angle θ


θ


object plane


(a) Object imaged at various angles to obtain tomographic projections.


(b) Projections mathematically reconstructed


to form an image.


1 of 35 projection


reconstructed


5 of 35 projection


10 of 35 projection


25 of 35 projection


all 35 projection reconstructed


Figure 2. Illustration of the tomographic reconstruction process.  (a) Projections of an object, a phantom in this illustration, are acquired at different angles θ. (b) The collection of projections are mathematically reconstructed into a 3D image which represents the original object.


trast for imaging Cu and Ta features with Si  thickness of up to about 10 microns.


X rays in the 1.5-10 keV energy range offer a  combination of good image contrast between  many important materials in ICs and adequate  penetration power for non-destructive imaging  of either partial or full IC stack.  In particular, the interconnect metallic materials such as Cu, W, and Ta or Ta-containing compounds used in   Cu interconnect technology have strong contrast  with conventional or low-κ dielectric materials.  The TXM 54-80 uses 5.4 keV x rays.  This energy is chosen to optimize the absorption contrast between silicon and copper, the penetration  depth in silicon, and the x-ray imaging system  efficiency.


3. Tomographic Imaging of ICs


The tomographic imaging technique for ICs can  be described as a CT scan for chips.   As illustrated in Fig. 2, an object  is placed in the imaging field and imaged at many angles.  The set of  images thus acquired are called projections at  various projection angles.  The projections can  then be mathematically reconstructed into a 3D  image that represents the original object.  The  underlying principle of this technique is the Fourier Slice Theorem, which relates the Fourier  transform of the projections to the Fourier transform of the object [12].  In the TXM 54-80, projections with tilt angles between –70º to +70º  can be obtained.


4. Sample Preparation Steps for the TXM


The sample preparation requires localized thinning of the silicon substrate in the region of interest. It is relatively simple compared with  other high-resolution techniques such as SEM, TEM, or FIB.  The requirement for an IC to be  imaged is that the total copper and total silicon  thickness at the region of interest (ROI) should  be less than 5 um and 10 um, respectively.  If an  IC contains more than these amount of material, it is still possible to image the sample, but longer  imaging time will be necessary due to the increased absorption in the additional material.  Conversely, a thinner sample will result in


shorter exposure time.  A recommended sample  preparation flow is illustrated in Fig. 3.  In this  procedure, a flip chip packaged IC undergoes  global backside thinning of the silicon to a  thickness about 100 um. This is followed by localized trenching of the silicon in the region of


Packaging


Circuits


Step 3: Remove the packaging.


Step 1: Polish the Chip


to approximately 100


um globally.


100 um


Step 2: Locally thin the


silicon below the region of


interest to about 10 um.


Region of Interest


10 um


~500 um


Step 4 (Optional): Deprocess top layer. Mark ROI with


heavy metal (e.g. W or Pt).


Figure 3. Illustration of the sample preparation steps for flip chip packaged ICs.


interest to a thickness of less than 10 microns. The silicon trench dimensions are typically  about 400 um at the bottom of the trench.  Following this step, the silicon chip is removed  from the flip chip package and deprocessed to  the top of the interconnect stack. For non-flip  chip packaged ICs or in the case of previously  de-packaged bare thinned die, the localized silicon trenching procedures will require modification.  Extra care is required in handling the samples during and after sample preparation due to  the fragility of the thinned region. Heavy metal (e.g. W or Pt) markers are often deposited to  help locate and align the ROI within the field of  view of the TXM. The metal markers also help  in aligning the tomographic projections for 3D  reconstruction.


5. Sample Handling in the TXM 54-80


To easily align the ROI of a sample for imaging, the TXM 54-80 microscope includes a visible  light microscope with its field of view aligned to  that of the x-ray microscope.  Specially designed  sample holders mount onto both the x-ray and  visible light microscope via a kinematic mount, and holds samples securely by an integrated  clamping mechanism.  This prealignment system


will place the sample’s ROI correctly in both the  transverse and the longitudinal directions.


Before imaging a sample in the x-ray microscope, the operator mounts the sample holder on  the visible-light microscope and places the sample on the sample holder.  Then using an integrated micromanipulator, the operator can move  the sample’s ROI to a marked field of view, and  finally clamps the sample to the sample holder.  The sample is now ready for imaging in the xray microscope.  A robotic sample handling system loads the sample holder into the x-ray microscope.  Once the sample is in the x-ray microscope, the ROI will be aligned to the field of  view, and focusing is generally not necessary  since the depth of focus is much greater than the  alignment accuracy of the prealignment system.


6. Results from the TXM 54-80


The TXM 54-80 has been tested for resolution, contrast and throughput as well as usability and  reliability.  A Fresnel zone plate consisting of  gold lines of minimum 70 nm width was used as  a resolution test pattern.  Its image acquired with  the TXM is shown in Fig. 4.  The 70 nm lines  are clearly resolved.  The resolution as measured  by Rayleigh criterion is about 80 nm.


Figure 4.  Image of a Fresnel Zone plate acquired with the TXM 54-80.  Lines with 70 nm width are clearly resolved.  Some defects in the zone plates are also visible.


Figure 5. An electromigration test sample imaged with the TXM 54-80.  Voids in  lines number 1, 5, 7 and 9 (counting from  the left) can be identified.


The microscope was also used to image ICs with  copper structures.  Fig. 5 shows an electromigration test sample imaged with the TXM.  The  lines in this test sample are 160 nm wide and  200 nm thick.  They have about 1% intrinsic  contrast.  In this image, we can identify the heat  sinks made of tungsten (darkest circular structures), copper vias (grey circular structures) and  the copper lines and pads.  Voids near the ends  of some copper links can be identified.


A tomographic data set from this sample has  also been acquired and the 3D reconstruction has  been computed from this dataset.  From the 3D  image, one can digitally section the chip and  observe the structure of each chip layer.  Figure  6 shows three sections of the reconstruction  showing the chip layers containing the lines, pad  and the heat sinks.  Chips with more complex  structures have also been imaged with the TXM.  A tomographic dataset of a 5-layer  copper interconnect structure was acquired with the TXM.  Its 3D structure was reconstructed and shown in  Fig. 7. With this technique, it is possible to study  the 3D structure of an IC without physically  modifying the chip.  It is ideal for situations  where the chip structure needs to be studied  nondestructively.  The process of tomographic  data acquisition and reconstruction takes between a few to 10 hours.


The basic performance parameters of the TXM  54-80 are summarized in Table 1.


7. Discussion and Conclusions


The TXM 54-80   transmission x-ray microscope  shows great promise for use in IC failure analysis and process development, including the nondestructive imaging of defects and the evolution


Figure 6.  Layers extracted from the tomographic reconstruction of the electromigration sample, showing the three layers of the IC structure.


Figure 7.  A 5-layer IC imaged with the  TXM 54-80.


of failure mechanisms such as those induced by  electromigration.  The TXM has demonstrated  better than 80 nm resolution and high throughput  for imaging semiconductor chips with finest line  features currently produced in the IC industry  and for those expected in the near future.  Its  unique ability of the being able to image the 3D  structure of ICs at sub-100 nm resolution without having to physically modify the IC structure  will become a valuable addition to the IC failure  analysis and yield enhancement toolset.  Besides  providing new capabilities for non-destructive  imaging of defects, it may also become a powerful tool to guide the use of traditional destructive  imaging techniques such as the SEM and TEM.


We would like to thank Steve Kirch for initiating this project and overseeing its early phases  of development.


1. Haddad, W.S., et al., Ultra high resolution xray tomography. Science, 1994. 266: p.


1213--1215.


2. Schneider, G., Cryo x-ray microscopy with


high spatial resolution in amplitude and


phase contrast. Ultramicroscopy, 1998. 75:


p. 85-104.


3. Wang, Y., et al., Soft x-ray microscopy with


a cryo STXM: II. Tomography. Journal of


Microscopy, 2000. 197: p. 80-93.


4. Weiß, D., et al., Computed tomography of


cryogenic biological specimens based on xray microscopic images. Ultramicroscopy,


2000. 84: p. 185-197.


5. Haddad, W.S. and J.E. Trebes. Developments


in Limited Data Image Reconstruction Techniques for Ultrahigh-Resolution X-ray Tomographic Imaging of Microchips. in Developments in X-ray Tomography. 1997. San


Diego, CA: SPIE.


6. Levine, Z.H., et al., Tomographic reconstruction of an integrated circuit interconnect. Applied Physics Letters, 1999. 74(1): p.


150-152.


7. Levine, Z.H., et al., Tomography of an integrated circuit interconnect with an electromigration void. Journal of Applied Physics, 2000. 87(9): p. 4483-4488.


8. Yun, W., et al. Hard x-ray microscopy and


tomography at the ALS: experiments and


plans. in X-ray Microscopy: Proceedings of


the Sixth International Conference. 2000.


Berkeley, CA: American Institute of Physics.


9. Schneider, G., et al., In situ x-ray microscopic observation of the electromigration in


passivated Cu interconnects. Applied Physics


Letters, 2001. 78(13): p. 1936-1938.


10. Engström, A., Quantitative micro- and histochemical elementary analysis by Roentgen


absorption spectrography. Acta Radiologica


(Supplementum LXIII), 1946. 63: p. 1-106.


11. Henke, B.L., E.M. Gullikson, and J.C. Davis,


X-ray interactions: photoabsorption, scattering, transmission, and reflection at E=50--


30,000 eV, Z=1--92. Atomic Data and Nuclear Data Tables, 1993. 54: p. 181--342.


12. Rosenfeld, A. and Kak, A. C., Digital Picture


Processing, Academic Press, Inc., San


Diego, 1982.


Table 1. Performance of the TXM 54-80.


Rayleigh resolution 80 nm


21 µm


(single image) Field of view 200 um


(mosaic mode) Pixel size at sample 21 nm


2D image exposure


time (1% contrast) 10 min.


3D tomographic data


acquisition time 1-10 hours


(tranverse)


3D imaging resolution


(Center) 200 nm


(longitudinal)


A Broadband Model for Ultrasonic Pulses in the Presence of  Thin Layers in Microelectronics


Sridhar Canumalla


Nokia Mobile Phones


sridhar.canumalla@nokia.com


A broadband model is proposed to describe the nature  of ultrasonic pulses in multilayered systems with a  sub-wavelength thickness layer. This model, which is  targeted towards acoustic microscopy of  microelectronic devices, can incorporate measured  ultrasonic properties of electronic materials and  predict the complete ultrasonic pulse-train for all the  interfaces in an electronic device. The model is robust, and incorporates material and geometric variables  commonly encountered in microelectronics  applications. Results are presented to illustrate how  delaminations and cracks with foreign material or  moisture ingress can appear to be well-bonded and  why acoustic images of interfaces with thin layers can  sometimes give erroneous indications of the bond  state.


INTRODUCTION


Acoustic microscopes are widely employed in the  nondestructive inspection of microelectronic devices  for cracks, delaminations, porosity and package  integrity. Historically, acoustic microscopes have been  employed primarily for imaging applications [1-4] in  the microelectronics community. Recently, however, they have found increasing use for characterizing  properties of electronic materials [5], measuring  elastic properties [6] and metrology applications [7]. The nondestructive nature of the measurements and  the potential for accurate measurements make acoustic  microscopy an attractive alternative to timeconsuming destructive methods.


Acoustic microscopy image interpretation has been  standardized for consistent results across different  package and device types. For example, in acoustic  images of interfaces, it is commonly accepted that  regions exhibiting inverted polarity of the reflected


ultrasonic echo (commonly pseudo-colored in red or  yellow) are delaminated. Indeed, for applications  involving relatively simple package constructions, such simplistic guiding principles will suffice. However, for samples that contain thin layers or  delaminations filled with foreign matter, conventional  principles for interpretation of acoustic images can  lead to erroneous conclusions. A more rigorous  approach is required to help understand the  propagation of ultrasound pulses in devices and  predict the pulse shape.


Theoretical approaches that could be used for this  purpose can be broadly categorized according to  increasing levels of complexity as i) simple pulse  superposition schemes [8], ii) reflection coefficient  approaches that are still relatively straightforward  computationally (for example [9]), and iii) generalized  multi-layer approaches [10]. The three approaches  attempt to model the physical phenomenon with  different degrees of complexity, with the generalized  multi-layer approach being the most computationally  intensive.


From an acoustic microscopy perspective, most  microelectronic packages can be characterized as  having a single thin layer of sub-wavelength thickness  sandwiched between several thick layers having  disparate acoustic impedances and ultrasonic  velocities. Therefore, the goals for the proposed model


Glass


Molding Compound


Water


Spacer


Figure 1. Schematic of the test vehicle to simulate  delamination between epoxy molding compound and  Si with water ingress.


include a) ability to incorporate measured ultrasonic  properties, b) simplicity of computational scheme, c) robustness for use in the inverse approach, d) capacity  for automation, and e) ability to model the complete  layer stackup in the package simultaneously and  predict the complete time trace. Therefore, the  reflection coefficient approach, which affords a  balance between ease of implementation and detailed  description of the physical phenomena, is adopted  here for further improvement.The examples addressed  in this paper are i) pulse distortion at delaminations  with water ingress, ii) imaging of interfaces with thin  layers.


Pulse Distortion At Delaminations With Water  Ingress


The simple scheme of delamination as described  previously can yield erroneous results in several  instances and there has been continued interest in  understanding the apparent anomalies. Tilgner et al.


[11] have suggested that surface roughness can lead to  false indications of delaminations due to asperity  contact transmitting enough ultrasound. Ranade et al.


[12] suggest that “false healing” observed in their  study could be due to a) presence of moisture inside  the package or b) moisture ingress into the  delamination. The concept common to both studies is  the idea of a gap filled with water or other material  behaving as if the gap is not a delamination. Pulse  distortion at delaminations filled with water will be  explained using the model and a simple laboratory  experiment (Figure 1) in which the water gap is varied  in a controlled manner.


Thin Layers on Substrates


The presence of thin layers can potentially result in  erroneous indications of delamination, and is  illustrated for the case of a Parylene-N coating on  stainless steel [13, 14]. The effect of transducer  frequency on the extent of distortion will be discussed  using example images obtained with 30 MHz, 100  MHz and 230 MHz transducers.


THEORY


To study the nature of ultrasound at interfaces in  microelectronics devices it is useful to understand the  basis for discrimination of an interface ultrasonically. For the sake of simplicity and to emphasize the effect  of material properties and geometry on the  propagation of ultrasound in microelectronics  assemblies, we shall limit the discussion to the case of  plane longitudinal (compressive) waves propagating  along the x-axis in an isotropic material. The  generalized governing displacement equations are  given [16-18] by


&&ρ


µ


∇


⋅


∇∇


which can be reduced to


x u


∂∂


ρ


In other words,


2 3


0 1


2 ...


(n-1)


Interfaces - 1


(n-1)a+h


Figure 2. Schematic showing a) normal incidence of an ultrasonic pulse at a semi-infinite half-space boundary  and b) normal incidence of an ultrasonic pulse on a semi-infinite half-space coated with a thin layer, c) a n+1  layer stackup with n interfaces of interest, each with thickness hi, etc.


where u is the generalized displacement vector, u is  the displacement in the x direction and t is time. The  compressional velocity is related to the elastic  constants by the equation


ρµ


λ +


The more commonly used engineering moduli can be  expressed in terms of the Lamé constants by the  equations











++


λλ


Modulus


Shear


sRatio


Poisson'


Modulus s


Young'


G v


The solutions to the wave equation (3) are given by   for travel along the positive x-axis,  ( )


kx


i


= ω    for travel along the negative x-axis, ( )


= ω .


Let us now consider the case of a plane harmonic  wave impinging on semi-infinite material 2 from 1 in  Figure 2a.


Reflection and Transmission Coefficients at  interface of two semi-infinite half-spaces


The reflection of acoustic waves incident at the planar  interface between two isotropic, semi-infinite media  can be described in terms of their characteristic  acoustic impedance. Acoustic impedance is defined as  the negative ratio of stress to particle displacement  velocity. The characteristic acoustic impedance of a  material is also given as


Z ρ=


For normal incidence upon an interface, continuity in  stress and displacement must be maintained across the  interface. If the stress or pressure amplitude of an  incident wave is unity, and the stress amplitudes of the  reflected and transmitted waves are R and T, the  continuity of stress results in 1+ R = T and  displacement continuity results in the condition (1-R)/Z1 = T/Z2,. Then, the reflection and transmission  coefficient, R and T respectively, are given by





+−


Z


The reflection coefficient constitutes the primary basis  of detecting defects in acoustic microscopy. It is based  on the observation that defects such as inclusions, voids, and delaminations typically have different  acoustic impedances in comparison to the surrounding


“good” material. The reflection coefficient also plays  a critical role when the acoustic microscope is used as  a metrology tool. In pulse echo measurements, the  equation used to determine thickness or velocity, is  given by


h∆=


where ∆t is the time lag between the front and back  surface of the specimen and h is the thickness of the  layer.


The assumption implicit in such measurements is that  there is a substantial acoustic impedance mismatch at  the boundaries of the test specimen. For example, in  measuring the stand off height of a flip chip specimen, it is assumed that the acoustic impedance of the gap  filled with water is substantially different than that of  materials above (Si) and below (substrate). However, equation (9) fails when thin layers are present at the  boundaries of the test specimen. For example, the  presence of solder mask or passivation layer could  substantially alter the physics of the measurement. In  such cases, using the simplistic equation (9) will lead  to inaccurate measurements.


Reflection and Transmission Coefficients at a Thin  Layer Sandwiched Between 2 semi-infinite HalfSpaces


A steady state harmonic wave traveling in medium 1 (Figure 2b) along the positive x-direction can be  expressed by the equation


ik


inc e


(10) where the subscript refers to the medium of  propagation, ω refers to the circular frequency and the  factor


e ω is omitted from the right hand side of the  equation for simplicity (but will be introduced in a  later section). The waves that are reflected and  transmitted from the entire thin layer assembly in  Figure 2b, respectively, are given by


ref


Ae


trans


De


The motion inside the plate is described by a forward  traveling wave transmitted at the interface between 1  and 2 as


Be


(13) and a backward traveling wave reflected from  interface between 2 and 3 as


Ce


2 =


(14) To satisfy the continuity of displacements and stresses  at the two interfaces a and a+h,











∂∂


∂


inc


2 2


(15)


Following [9], it can be deduced that,


k


123


(16a)


(16b)


ik h


(16c)


(16d)


Here, ijR  and ijT  are the reflectance and transmission  coefficients as defined earlier for a simple interface  between two materials. The transmission coefficient ( 123T ) for the entire thin layer is given by equation for


D and the reflection coefficient ( 123R )for the thin  layer is given by the equation for A(f). Similarly for a  wave traveling in the negative x-direction, it can be  shown that


32


321


, and (17)


(18)


The attenuation in materials is easily incorporated into  these equations by replacing k with


( αik − , where α


is measured in dB/mm. The equations presented until  now have dealt with the propagation of ultrasonic  waves of any frequency. In most commercial acoustic  microscopes, the ultrasonic energy is excited as a  broadband pulse. The essential difference between a  wave and a pulse, as treated in this paper, is that a  pulse has a well-defined time trace and frequency  bandwidth while a wave can have any single  frequency. In other words, a pulse is a packet of  ultrasonic waves of several different frequencies  whose relative strength is characterized by the


frequency spectrum of the pulse. The model will now  be extended to pulse propagation.


Constructing the Pulse for a Broadband, Pulsed  Acoustic Microscope


The model development in this section follows the  approach published earlier [19]. It is convenient to  assume that the frequency response of a transducer  can be approximated as a Gaussian function of  frequency. Indeed, from an examination of several  dozen commercial transducers from different vendors  with frequencies ranging from 5 to 230 MHz, there  were few instances where a Gaussian function did not  adequately describe the frequency response. Therefore, the spectral output or frequency response ( Λ(f) ) of an ultrasonic transducer can be described as


exp


amp














 −


Λ


(19)


and the pulse emanating from a transducer can be  described by the equation


∑Λ=max min


initial


ω


δ


ψ


(20)


where the subscript 0 represents the propagation in  water. The use of the first two terms inside the  summation is a simple way to model a wide variety of  commercial transducers.


For the case of a pulse impinging from water onto  material 1 at interface 1 in Figure 2c, the reflected and  transmitted pulses, respectively, are given as


∑∑


01


max


min


ηξ


(21)


In equation (21), all terms preceeding the reflection or  transmission coefficient are identical because those  terms describe the incident pulse. At each interface the  reflection and transmission coefficients and the terms  accounting for the propagation distance need to be  included inside the summation. In pulse echo mode, only the reflected pulses are of interest. The  contribution of each interface can be modeled by an  effective transmission coefficient


ji


ijTT .


j








∏


∑


ξ


(22)


)1


)(


(23)


At each interface prior to the interface of interest, the  amplitude is first reduced by a factor equal to the  forward transmission coefficient and then again by the  bacward transmission coefficient because the pulse  has to travel back to the transducer for detection. In  generalized form, the pulse reflected from the nth  interface of interest in the n+1 layer system in Figure  2c can be written as in equation (22). If the (n-1)th  layer is a sub-wavelength thick layer, then equation


(23) may be used.


Once the individual pulse reflections are computed  using equations (22-23), the entire time trace can be  constructed using the equation


total


(24)


One key point to remember while constructing the  entire time trace is that the computation represents  only the compressional wave without any focusing  effects and mode conversion due to oblique incidence. The issue of multiple reflections, however, is  implicitly accounted for in the model. The material  properties used in the paper are tabulated in Table 1.


EXPERIMENTAL


All images and time data in this study were obtained  using a C-SAM scanning acoustic microscope. A  majority of transducers used in acoustic microscopy  use focusing lenses to ensure the best resolution  possible [19]. Unfocused transducers have a large spot  size and are unsuitable for microelectronics  applications. Therefore, when using focused  transducers that are normally used for imaging without  sacrificing accuracy, an aperture-limiting cap (with a 2  mm diameter central aperture), was placed over the  lens for data acquisition from internal interfaces.  The  cap limits the ultrasonic beam to paraxial rays, which  permits a comparison of the experimental data to the  predictions of the model.


Pulse Distortion at Delaminations with Water  Ingress


The phenomenon of pulse distortion is investigated for  the case of delamination at a molding compoundSilicon interface into which water has penetrated. This  was simulated in the laboratory by creating a waterwedge using a flat molding compound beam on a glass  plate as shown in Figure 1.  Since the thickness of the


spacer at the open (right) end is known, the gap  thickness at different points along the bar can be  calculated.  Time and frequency data were saved to  disk for further data analysis.


Interpreting Images of Interfaces with Thin Layers


Transducers with nominal center frequencies ranging  from 30 to 230 MHz were used for these experiments.  The stainless steel (SS) test vehicle had a thickness of  8 mils (approximately 200 microns).  The dielectric  material Parylene N was coated to a nominal thickness  of 1 mil (25 micron) to 1.5 mil (37.5 microns). The  average surface roughness was 0.3 microns and the  maximum contour height was 1.8 microns [13]. The  coating was removed in the top left corner of the sheet  to expose the base material.


RESULTS AND DISCUSSION


The first example discusses how a delamination filled  with water or other foreign material can distort the  pulse and cause erroneous interpretation of the extent  of delamination.


Pulse Distortions at Delaminations or Gaps


The acoustic image of the molding compound-water  interface is shown in Figure 3a.  First principles  suggest that the pulse reflected from this interface be  inverted with respect to the incident pulse.  By


convention, if the incident pulse was positive ( ), the  pulse reflected from a molding compound-water or  molding compound-air interface should be negative


( ) since the acoustic impedance of water (1.5  Table 1. Material properties used.


Medium


Compressional


Velocity


(mm/µs)


Impedance (MRayls)


1.485


5.6


13.2


Parylene N


Stainless Steel


5.9


45.7


8.0


Molding


Compound


3.8


7.9


Sylgaard 577


1.027


MRayl) is less than that of the molding compound (7.9  MRayl).  Similarly, the pulse reflected from a waterglass interface is expected to be positive because the  acoustic impedance of glass (13 MRayl) is greater  than that of water.


Since water fills the gap (delamination between the  molding compound and glass) at all locations except at  the left and right supports, the reflected pulse should  be negative throughout the length of the molding  compound-water interface.  Negative pulses are shown  in yellow and red shades, while positive pulses are  shown in grayscale.  Contrary to expectations of a  single shade of red along the complete length of the  specimen, it is seen that the color in the image of the  molding compound-water interface varies with gap  spacing. Conventional rules for interpreting acoustic  images fail to explain the anomaly.


At the far right of the molding compound specimen, where the gap spacing is maximum (indicated on the


image by 1), it is seen that the negative reflection from  the molding compound-water interface and the  positive pulse from the water-glass interface are  widely separated (Figure 3b). In the middle of the  sample, at the spot indicated by “2” in the image, the  two echoes are not as widely separated, but the pulse  in the gate is predominantly from the molding  compound-water interface.  Both these locations  exhibit a uniform yellow shade indicating a “delamination.” Examining the echoes at a point  where the gap is smaller than at location 2 (indicated  by “3” on the image), it is seen that the two echoes  have merged into one, enhancing the amplitude of the  pulse within the gate.  Although the echo amplitude  and pseudocolor have changed, the color-map still  indicates a “delamination,”  and image interpretation  is still straightforward inspite of the pulse distortion.


At the edge of the molding compound specimen  resting on the glass plate, the thickness of the gap  approaches zero.  In this region (indicated in the  image by “4”), the acoustic image indicates a positive  pulse (grayscale), which might give the incorrect  indication that this area is not delaminated.  The  apparent anomaly can be better understood in terms of  the broadband model as discussed below.


The experimental data in Figure 4a were acquired  from the molding compound-water-glass specimen at  a location where the gap was 192 µm thick.  Similar  data are shown in Figure 4b for the case when the gap


Figure 3. a) Acoustic image of the molding  compound-water interface in the test vehicle. b) Captured time-traces at different locations along the  length of the bar illustrating the phenomenon of pulse  distortion.


Figure 4. Comparison of the measured pulse shape to that  predicted by the model for the location where the  thickness of the delamination is a) 192 µm and b) 25 µm.


spacing is 25 µm.  The experimental data are plotted  as points while the theoretical predictions from the  model are depicted by a solid line.  It is seen that there  is very good agreement between the measured data  and the predictions of the model.  The pulse shown in  Figure 4b is similar to the distorted pulse shape shown  by “4” arrow in Figure 3a while the pulse shown in  Figure 4a is representative of regions where the  echoes are completely separated in time (1). The  results of simulation indicate that the region  represented by location 4 is actually delaminated even  though it does not appear red or yellow in color in the  acoustic image.


Thin layers on substrates


Special considerations for accurate interpretation of  acoustic micrographs of interfaces with thin layers are  discussed below with a Parylene coated stainless steel  sheet as an example.


In interpreting the acoustic image, it should be  remembered that the acoustic impedances of water, Parylene and SS are 1.5, 2.2 and 45 MRayl, respectively. In the sample examined here, the pulse  reflected from the water-Parylene interface is  expected to be a small amplitude positive pulse while  that reflected from the Parylene-SS or water-SS  interface should be a much larger positive pulse. The  images obtained with 30, 100 and 230 MHz  transducers are compared and analyzed for their  relative sensitivities to the presence of the Parylene  coating.


When a 30 MHz transducer was used to image the  coated sample (Figure 5a), little contrast could be  discerned between the coating and the exposed base  material indicating that at 30 MHz, the ultrasound is  relatively insensitive to the thin layer on top of the SS  sheet. At 100 MHz, however, the ultrasound is  extremely sensitive to the coating even though the  time trace did not reveal complete separation between  the pulses.  In the acoustic micrograph (Figure 5b), the  entire coated area appears to be disbonded and is  pseudo-colored in red. In the acoustic images obtained  with a 230 MHz transducer of the same sample (Figure 5c), on the other hand, there is only a slight


Figure 5.  Acoustic image of the Parylene N coated SS  sheet using a a) 30 MHz transducer, b) 100 MHz, and  c) 230 MHz transducer focused on the surface.


Figure 6.  Comparison between measured pulse and  theoretical model predictions for a 100 MHz  transducer for a) bare SS surface and b) pulse  reflected at the water-Parylene-SS inteface.


variation between the coated and un-coated areas and  the coated area appears to be well-bonded based on  the pseudocolor information.


Conventional rules for interpretation fail to explain the “anomalous” indication of delamination in only the  100 MHz image.


The first step is to verify that the model is capturing  the pulse response of the transducer. For this purpose, a comparison between the modeled pulse shape and  the experimental waveform capture (dots) over the  bare SS area is presented in Figure 6a. The good  agreement between model and experiment is  validation of the model’s adequacy in capturing the  response of the 100 MHz transducer (Figure 6a).


The ultrasonic pulse reflected from the coated areas  can now be examined. Figure 6b shows the  comparison between the predicted and experimental  waveforms over the coated area. In the modeling, a  thickness of 21 microns was used for the Parylene N  layer. The very good comparison between the  predicted and experimental pulse shape confirms that  the “red” area is actually well bonded and that the  apparent polarity reversal is actually caused by the  thin layer of Parylene. This kind of pulse distortion  should be properly accounted for when inspecting IC  packages, and not all “red” areas with negative  polarity are automatically delaminations.


While a 30 MHz transducer is relatively insensitive to  the 21 µm thick Parylene coating, the 230 MHz  transducer is able to fully separate the water-Parylene


and Parylene-SS interfaces. In both cases, pulse  distortion and concomitant anomalous indications of  delamination do not occur. At 100 MHz, however, the  pulse is especially sensitive to the presence of the  Parylene coating and gives a false indication of “delamination” even though the coating is well bonded  to the SS.


The dissimilar response obtained with different  frequency transducers can be explained in terms of the  reflection coefficent curve of the water-Parylene-SS  interface (Figure 7). A solid horizontal line at 0.936  indicates the reflection coefficient of the water-SS  interface without any coating. The reflection  coefficient over the coating shows successively more  pronounced maxima and minima with increasing  frequency. In addition, it is seen that the moving  average of the reflection coefficient is continuously  decreasing from the initial value of 0.936.


Low frequency pulses are not able to detect the thin  coating and suffer only a minor perturbation in the  reflected amplitude. Progressively higher frequency  pulses are affected more by the Parylene coating and  less by the substrate, and hence the reflected  amplitude continuously decreases. At frequencies  where the maxima in the reflection coefficient are  observed, constructive interference between the waterParylene and Parylene-SS interfaces can be expected. Conversely, at frequencies characterized by minima in  the reflection coefficient, destructive interference  between the reflected pulses from the two interfaces is  expected. In broadband pulsed inspection, some


Figure 7. The reflection coefficient at the water-Parylene-SS interface reveals several minima and maxima that  determine the extent of distortion at different frequencies.


frequencies in a pulse undergo constructive  interference while others undergo destructive  interferene, which gives rise to pulse distortion in the  time domain.


Scope of Model


The model discussed in this paper is a simple wave  propagation approach and takes into account  measured transducer characteristics and material  properties to yield surprisingly accurate results for the  simple geometries discussed. Further study is needed  to validate or modify the model for cases involving:


a) Highly focused transducers where refraction


effects dominate


b) More complex geometries involving multiple thin


layers smaller than the wavelength of ultrasound or


curved or very rough interfaces


c) Highly attenuative materials such as transducer


backing materials or other materials where


dispersion can be expected to contribute to errors


d) Materials in which guided modes of wave


propagation are operative


e) Materials with property gradients such as


underfills with filler settling


f) Inhomogeneous materials where the size of the


second phase is comparable to the wavelength of


ultrasound (in such cases, scattering becomes


dominant).


B. De-layering the ILD Layers


The Inter-Layer Dielectrics (ILD) of the IC are  de-layered with a Plasma Etcher (Fig. 12).


• Removal of Passivation  & ILD Layers:


Equipment:  Plasma Etcher


Gas/Volume: CF4: O2 / 9:1


Power:  75 Watt


• Etching time (Approx):


Passivation Layer: 10 Min


Each ILD layer: 5 Min


• During the plasma etching, the IC was not


detached from the module


Fig. 12 Plasma System for Passivation & ILD


Layer Removal


Fig .13 Band-gap reference circuits after ILD


de-layering


C.  IC is Setup under Normal Operating


Conditions


After de-layering the ILD Layers (Fig .13), the  IC was setup to run under normal operating  conditions (Fig. 14).  This means that the IC was  setup to run as a whole unit with the module.  This was an important element of the experiment  because it was found that results might differ if  the IC was tested independently from the  module.  If it were tested independently, the  absence of interference from other components  in the module might alter the results. Also, testing the IC while it is still mounted on the  module eliminates significant costs because a  special IC tester and training is not needed.


Fig.14 The Module was mounted on PCB


test board after removal of ILD layers


D.  RF Probe Station Setup


This probe station3 (Fig. 15) requires the  following:


• Vibration Table


• High Magnification Microscope


• Customized Testing Rack


• Motor Controlled Precision Manipulator


• Computer that is able to control the  Manipulator and the focusing of the  Microscope


• High-Input Impedance Active Single Probe2  Probe tip (0.1um, 0.5 um, 1um)


• High-Frequency Amplifier (GHz)


Characteristics of the High Impedance Active  Single Probe (Fig. 16):


Input Capacitance: 0.07 pF


Input Resistance: 10.0 MΩ


Frequency Response: DC to 3 GHz


Fig. 15 RF probe station


Fig. 16 High Impedance Active Single Probe


(These experiments are conducted with 3 GHz


probes.  New high-speed active single probes are  currently under evaluation and measurements of  up to 30 GHz signals are expected with the


introduction of these new instruments.)


E. Using the RF Probing Station to Test the


Circuit


The internal circuit signals are then measured  using the probe station.  These probes can be run  manually using a computer controlled precision  manipulator or automatically using a CAD  navigator4.  The probe is moved to the area of  interest and then is moved to make contact with  the bandgap circuit metal lines.  After that, a test  program is run in order to gather the results.  In  this case, twenty-one output voltages of the  bandgap circuits were read in order to gather  sufficient data (Fig. 17).


1 3 5 7 9 11 13 15 17 19 21


Sample number


Fig. 17 Band-gap Voltage Measurements from  Internal Circuits


Fig. 17 shows that most of the bandgap  reference output voltage readings that were  retrieved from the internal IC circuits were not  close to their spec of 1.2 volts.  In fact, only 7 of  the 21 measurements extracted from the IC  circuits were close to spec.  Since more than two  thirds of the measurements were not close to the  spec of 1.2V of bandgap reference voltage for all  four channels, there was strong evidence to  suggest that the incorrect offsetting of the bandgap reference circuits caused the problem of the  Rx output voltage swing. In this case, after the  test case data was collected and compared with  the design data, the fault was quickly isolated.  In retrospect, the fault was not discovered during  the simulation because only a series of random  checks were made in order to look for trends. With the new data, designers were then able to  redesign the bandgap reference circuits with the  information from this case.  The results from  Fig. 18 show that the outputs from the  redesigned circuits are now within specification.


New RX Differential Output


300 400 500 600 700 800 900


Channels


Fig. 18 Newly Designed IC Rx Differential  Output Voltages with 700mV target


This methodology has an advantage over the  conventional mechanical probe and general Ebeam probe that it can more accurately measure  analog signals from the internal circuit. Often, it  is difficult to extract high frequency GHz range  of electrical data in mixed signal ICs because of  the signal interference.  However, with this  methodology, fault locations can be quickly and  accurately identified because the analog signals  can be acquired simply with a simple direct  measurement.  Paramount accuracy can be  achieved because there is no local oscillation  and data calibration when using the high-input  impedance active probe.


This technology can improve the R&D  development cycles and can be implemented  without extensive additional training and with  equipment that is relatively inexpensive. For  example, a system that can debug ICs with a  minimum geometry of .35 microns of metal-line  width and up to five-metal layers can be  purchased for $200,000 or less.  Companies can  save substantial amounts of money because of  these new technological advances in failure  analysis.


The authors would like to thank Hui Xu, Binh  Tran and Forrest Dial for helping with sample  preparations and for adding to the technical  discussion.


1. Paul R. Gray & Robert G. Meyer


Analysis and Design of Analog Integrated


Circuits, 3rd Edition .1997


John Wiley & Sons, Inc.


2. GGB Industries, Inc.


Picoprobe Model 34A


Naples, FL: GGB Industries, Inc.


www.picoprobe.com


3. Cascade Microtech, Inc.


REL-1000 LCD/Large Area Probe Station


Beaverton, OR: Cascade Microtech, Inc.


1995


4. EGsoft, Division of Electroglas


Merlin’s Framework


San Jose, CA: EGsoft, Division of


Electroglas


Application of Various Fault Localization Techniques to Different  Types of 6T-SRAM column Failures


Cheng-Piao Lin, Cheng-Chun Ting, Chin-Hsin Tang, Cheng-Hsu Wu, Chih-Ming Kuo, Yung-Sheng Huang


In this paper, we demonstrate different techniques of  fault isolation from front-side of 6T-SRAM column  failures. We show how to choose proper and  suitable methods to solve column failures with a  variety of characteristics. The capabilities and  physical mechanisms of OBIRCH, photoemission  microscope and LCA are reviewed utilizing these  SRAM column failures.


Optical Beam Induced Resistance Change (OBIRCH)[1]/Temperature Induced Voltage  Alteration TIVA[2-3] or XIVA[4], Fluorescent  Microthermal Imaging (FMI)[5] and Liquid Crystal  Analysis (LCA)[6]...etc. are all good at detecting  metallic shorts, yet they are also complementary. The choice of technique is a function of the type of  problem we are trying to isolate. One of the  challenges faced by our failure analysis (FA) laboratory is failure site localization of parts having  multi-level (up to 7 levels) metallization and low or  normal IDD leakage. Furthermore, when dealing  with memories, such as SRAM arrays, the cell area  is repetitive and consequently difficult to mark the  fault site from front side of device although a “hot” spot can be found from backside analysis. A  navigation system should be available to help, although with added expense. Therefore, fault site  localized by front-side analysis is expected to be  adopted for SRAM.


SRAM failure analysis is a general tool to reveal  problems during new technology qualification and  yield enhancement process. Column failure is often  seen in SRAM failures and requires further fault site  localization. However, the electrical characteristics  for SRAM column failures are strongly dependent  on layout, process and type of defect. [7]. These  variations make the fault localization process more  complex. Therefore, methods for the overcoming  the difficulties in fault isolation process that are  contributed by different level of metal layers, different level of IDD leakage [8], different metal  composition, different technologies as well as  synchronous and asynchronous operation will be  demonstrated in this paper. The following  experiments focus on metallic shorts only, not open


columns.


Since TSMC is an IC foundry company.  When parts  are returned by customers, it is not always possible


to have a tester and detailed product related  information to help in the fault isolation process, especially for failures involving normal IDD  leakage. Therefore, an inexpensive but useful  simulated bias interface is built to achieve the same


objective.


The 6T-SRAM failures that we studied are based on  the well-known six-transistor cell design. Its  architecture is three metals and single port SRAM  design. Some SRAM products among them act as  test vehicle. Thus, up to 4 dense dummy metals are  placed beyond the metal-3 in order to simulate the  real condition of embedded-SRAM products.


Six different types of 6T-SRAM column failure  cases demonstrated are described below.


Case #1


The device is 0.15µm process technology, 3-level  metal design 8Mb synchronous SRAM with a single  column failure. It presents high IDD leakage of  800~900 µA under 1.2V constant voltage. The  device has a typical metallic short failure. Therefore, front-side OBIRCH or TIVA is recommended to  quickly localize the leakage source. As expectation,


the front-side OBIRCH works effectively (Fig. 1, 2).


Figure 1: OBIRCH image.


Figure 2: SEM image of OBIRCH located metal  residue between BL and VSS-line.


Case #2


The device is 0.18µm process technology, 6-level  metal (4-6 layers are dummy layers) design 2Mb  synchronous SRAM with a single column failure. The device presents high IDD leakage of 700~800 µA under 2.0V constant voltage (Fig. 3). The  resistance of metallic short could be calculated  approximately as R=V/∆I=2V/700µA=2.9x103Ω.


Experiment shows that OBIRCH cannot find the  fault site from front-side since dummy metal layers  block the laser from the metal layers below. Nikawa  Et al. reported in 1993 that the minimum  temperature could be detected by Hamamatsu  Photonics (emission system) was estimated to be  about 180°C [1]. It is considered to be thermal  radiation. Therefore, the temperature of metallic  short type of defect, which provided leak path, may  have the possibility to reach closely 180°C or higher. To gain the advantage of front-side analysis, Hamamatsu photo emission microscope (Phemos  200, a dedicated emission system) was tried to  localize fault site even though it is not expecting to  detect metallic short type of defect. [9-11]. Fortunately, the above metal layers are not dense  enough to block the emission. Eventually, the device  under appropriate acquisition time for front-side  photo emission microscope was applied


successfully to find the fault site and result (Fig.4, 5)


Figure 3: I-V (VDD-IDD) curve for good device and  fail device. The resistance of metallic short could be


calculated


approximately


as


R=V/∆I=2V/700µA=2.9x103Ω


Figure 4: Front-side photoemission image


Figure 5: SEM image of photoemission located  metal residue between BL node and VSS-line


Case #3


The device is 0.15µm process technology, 7-level  metal (4-7 layers are dummy layers) design 2Mb  synchronous SRAM with a single column failure. The device presents high IDD leakage of 700~900 µA under 1.5V constant voltage (Fig.6). The  resistance of metallic short could be calculated  approximately as R=V/∆I=1.2V/360µA=3.3x103Ω.


After several attempts, neither front-side OBIRCH  nor front-side photoemisison microscope could  isolated the fault site due to dense metal layers. As a  result, liquid crystal analysis (LCA)[6], which is a  very traditional technique, under specific range of  voltage bias was attempted to overcome this  difficulty (Fig 7, 8). The attached laser cutter also


provides an advantage to in-situ mark the fault site.


Figure 6: I-V (VDD-IDD) curve for good device  and fail device. The resistance of metallic short  could be calculated approximately as  R=V/∆I=1.2V/360µA=3.3x103Ω


Figure 7: Image of LCA hot spot and in-situ laser  mark.


Figure 8: SEM image of LCA located metal residue  between BL node and VSS-line


Case #4


This case shows that not all metallic short type of


defects induce high IDD leakage. The device is


0.25µm process technology, 3-level metal design  1Mb synchronous SRAM with a single column


failure. The device presents low IDD leakage of  40~50 µA under 2.5V constant voltage. The


resistance of metallic short could be calculated  approximately as R=V/∆I=2.5V/40µA=6.3x104Ω. The magnitude of this resistance is one order higher  than for case #2 and case #3. It could never be  localized by above techniques due to such low IDD  leakage defect.


For this case, we used a system where a photo  emission microscope was connected with a  engineering memory tester -Mosaid 3490 (Fig. 6). [12, 13] High repetition rates with active bias  condition can be more effective to locate the failure  site. The result is TiN-rich metal flake between BL  node and VSS-line (Fig. 10,11). The composition of  metal flake also can explain why its resistance is


higher than other cases


Figure 9: Photoemission microscope (Hamamatsu  Phemos-200) connecting with a memory tester (Mosaid 3490)


Figure 10: Photoemission image occurs by active  bias stress.


Figure 11: SEM image of photoemission located  TiN-rich metal flake between BL node and VSS-line


Case #5


In this case, the device that was returned from our  customer is 0.15µm process technology, 3-level  metal design 18-Mb synchronous SRAM with a  double column failure. The device presents normal  IDD leakage under 1.5V constant voltage. A short  between neighboring bitlines was suspected due to  its IDD level and layout.


Unfortunately, there is no leak path in standby mode. OBIRCH and photoemission microscope  consequently can not help to localize fault site when  parts under static bias. However, a leak path can be  created between neighboring bitlines through active  operation-both write (Fig. 12) and read operation. Thus, an easy and inexpensive testing interface then  has been introduced to achieve the objective. [13, 14]. Basically, all commands have to refer to the  rising edge of CLOCK for synchronous SRAM (Fig. 13). To simplify the bias condition of write  operation mode, the device is re-bonded on a  general board. Then, all pins are kept at their proper  DC level except oscillator (Fig. 14) forces the  CLOCK pin. It is quite successful in localizing these  types of defects (Fig. 15,16), which cannot be found  by other techniques that we have available


Figure 12: Voltage relation between BLs for standby  mode and write mode


Figure 13: Write timing for synchronous SRAM and  its simple bias condition


Figure 14: Oscillator used as CLOCK and general  board. The oscillator is the key role of active bias  condition. The general board just is an example used  in tsmc.


Figure 15: Photoemission image under simple write  operation mode.


Figure 16: SEM image of photoemission located  metal residue between neighboring BLs


Case #6


The device is 0.13µm process technology, 6-level  metal (Cu) design 4 Mb asynchronous SRAM with a   double column failure. The device presents normal  IDD leakage under 1.5V constant voltage. The  situation is very similar to case #5 except it is an  asynchronous SRAM. So, a bias condition similar to  case #5 was simulated. Because it is asynchronous  SRAM, there is no CLOCK pin as a reference. To  achieve the purpose of active bias condition, the  WEB pin forced by oscillator was attempted (Fig. 17). This approach works quite effectively (Fig. 18)


Figure 17: Write timing for asynchronous SRAM  and its simple bias condition


Figure 18: Front-side photoemission image under  active bias condition


The significant differences between these cases are  summarized in below table (Table 1). One point has  to be emphasized that we don’t painstakingly  compare specific instruments but to fully utilize  available recourses we have on hand. We believe  that other versions of these instruments or other  advanced techniques may have better performance.


Both IDD leakage level and metallization level are  summarized as the key considerations in choosing  of proper fault localization techniques, as indicated  from the results.


For parts with high IDD leakage, OBIRCH  consequently is the most timesaving tools among  listed techniques. But multi-level and dense  metallization may reduce its capability. Thus, photoemission microscope or liquid crystal analysis


will be the second choice.


On the other hand, if parts have normal IDD leakage, then static bias condition will never cause heat or  emission since there is no leaky path. In such a case, active bias condition, either engineering tester or  simulated test interface, can help to create leaky


path and increase the repetition rate on fault site.


The effectiveness of photoemission microscopy has  been proven over the years. It is efficient in  detecting a wide range of leakage defects like  junction leakage, contact spiking, latch-up, oxide  current leakage, substrate damage...etc, but no  metallic short. Therefore, there is a question need to  be answered - Why photo emission can detect  metallic shorts? And what kind of metallic short can  be detected by photoemission microscope? There is  a plausible mechanism. As previously mentioned in


case #2, literature [1] revealed that


Table 1: The significant differences between the six cases


the  minimum temperature could be detected by


Hamamatsu Phonics was estimated to be about


180°C. For this reason, the temperature of the


metallic short is suspected to be high enough, due to


joule heating, so as to be detected by photo emission


microscope. It is so pity we don’t have enough


resource to clarify if it is true or not. Furthermore,


most of the particles we demonstrate are not quiet


solid, and its resistance is very high as compared


with metal line. It may provide some clues, which


are porous and high resistance, to identify the


possibility of detection. It also consistant with our


available examples that the power short (solid short)


has never be detected by photoemission microscope.


Six failure analysis processes of 6T-SRAM column  failures with different characteristics are illustrated  in this paper. When dealing with fault isolation, some challenges include 1). difficult to recognize  fault site from backside image for repetitive  memory cell, 2). multi-level metallization could  block the emission or stimulation laser, and 3). normal IDD leakage, that is no leaky path at standby  mode, …etc are faced. However, by means of the  choosing of proper techniques with suitable bias  condition, the difficulties are overcome smoothly. This illustrated concept can also be implemented  into other modes of failures for other kinds of  products.


1.  K.Nikawa and S. Tozaki, Int. Symp. Test and  Failure Analysis (ISTFA), pp.303-310, 1993


2.  Edward I. Cole Jr., Paiboon Tangyunyong, and  Daniel L. Barton, Int. Reliab. Phys. Symp. (IRPS), pp.129-136, 1998


3.  F. Beaudoin, R. Desplats, P. Perdu, D.Patrie, G. Haller, P. Poirier, P. Jacob, and D. Lweis, Int. Symp. Test and Failure Analysis (ISTFA) , pp227-235, 2001


4.  R. Aaron Falk, Int. Symp. Test and Failure  Analysis (ISTFA) , pp59-65, 2001


5.  D. L. Barton and P. Tangyunyong, Int. Symp. Test  and Failure Analysis (ISTFA), pp.41-49, 1997


6.  Shekhar Khandekar and Kendall Scott Wills, Microelectronic Failure Analysis, Desk  Reference Fourth Edition, pp171-174


7.  C. Brillert, C. Burmer, P, Egger, Int. Symp. Test  and Failure Analysis (ISTFA) , pp323-329, 2001


8.  S. Nakajima, T. Ueki, S. Tazawa, K. Ochiai, S. Nakamura, Y. Komine, and T. Takeda, Int. Symp. Test and Failure Analysis (ISTFA), pp.249-255, 1993


9.  Cristian Boit, Microelectronic Failure Analysis, Desk Reference Fourth Edition, pp213-229


10. K.Naitoh, T.Ishii, and, J. I. Mitsuhashi, Int. Symp. Test and Failure Analysis (ISTFA), pp.145-151, 1997


11. Charles F. Hawkins, Jerry M. Soden, Edward I. Cole Jr., Eric S. Snyder, Int. Symp. Test and


Failure Analysis (ISTFA), pp.55-66, 1990


12. P. Perdu, R. Desplats, F. Beaudoin, and J.-Y. Bernard, Int. Symp. Test and Failure Analysis


(ISTFA), pp469-475, 2001


13. C. Boit, Microelectronic Failure Analysis, Desk  Reference Fourth Edition, pp223


Dat Nguyen


Texas Instruments, Dallas Device Analysis Operation   Dallas, Texas, USA


Tim Campbell, Steven Whitlock, and Ankineedu Velaga


AgereSystems, Microelectronics


Orlando, Florida, USA


Smaller technologies and increasing chip  functionality has resulted in tightly packed devices  and more stacked metal layers. For technologies  between 0.25µm and 0.14 µm, stacking packed  metal layers required the combination of Tungsten  plugs as interconnection and the utilization of  Chemical Mechanical Polishing (CMP).  “Pillar”, however, is a small metal line, which allows interlevel connections between Tungsten plugs.  The  size and shape of the pillar can be a yield limiting  issue.  The process of identification and resolution  of the missing metal pillar included yield analysis, electrical and physical failure analysis, root cause  analysis and the engineering coordination of photo  engineering, etch process engineering, CMP  engineering, integration engineering, and inline  inspection. Resolving the missing pillar issue has  proven to have significant contribution to yield.


In a device layout, meters of metal lines overlay  each other.  Separating metal layers and in-between  metal lines are dielectric (SiO2) layers.  Connection from the upper metal layers to lower  metal layers can be done with the utilization of  Tungsten plugs.  In the case of 5 metal layers, the  top metal layer, metal 5 (M5), can be directly  connected to bottom metal layer, metal 1 (M1), through the use of Tungsten plugs and metal  pillars, as shown in Figure 1.  Metal pillars can also  be viewed as landing pads for Tungsten plugs.


Metal pillars have the line width of the normal  metal runners.  In a densely packed metallization, metal runners became narrower as did the metal  pillar’s dimension.  For example in 0.25µm  technology, a metal line can have a width as small  as 0.50µm.  Smaller metal line width made it more  challenging for patterning, and the challenges  multiplied when it came to patterning metal pillars.  This issue is not easily seen, since metal runners  can be characterized through IV structures in the  wafer grid.  However, there is no IV structure  designed to characterize metal pillars.  Aggravating


the issue is the thickness uniformity across the  wafers due to chemical mechanical polishing (CMP).  Thickness variation across the wafer and  within die posed challenges for lithography in  terms of optimized focus/expose margin.


This paper will evaluate the yield impact of  missing metal pillars, to provide failure analysis  techniques to identify the issue, and the root cause  analysis, which leads to resolving of the missing  metal pillars.


Figure 1: Metal 5 (M5) connecting down to Metal  1 (M1) via Tungsten window 5 (W5) through window 1 (W1)


Yield Analysis and Yield Impact of Missing  Metal Pillars


In a high volume manufacturing environment, yield  improvement is a continuous effort.  Wafer yield    is closely watched and plotted against a yield  model.  Besides wafer yield, yield can also be  tracked by random yield loss (D-zero) and  systematic yield loss (Y-zero).  Low yield lots (25  wafers in a lot) or wafers are subjected to failure  analysis.  Some of the yield analysis tools include  wafer yield map recognition, IV signature (grid  structure testing), IV correlation (yield vs. IV  parameter), process log review; wafer position  analysis, common facility analysis, SPC, etc. Yield


analysis tools serve as a guide to physical failure  analysis (FA), which supports the isolation of the  failure mechanism.  The combination of yield  analysis and physical failure analysis often  pinpoints the exact problematic process facilities.


a) Identification of Yield Issues


The identification of yield issues related to missing  metal pillars began with the low yielding lots and  yield fluctuation of different product types.  Whitlock’s bad sites yield model [1] was used to  analyze the scope of the issue.  Figure 2 plotted the  average number of tested bad chips with respect to  total number of tested chip per wafer (cpw), with 1  site equal to 1 tested chip.  Note that each product  type has a different cpw.  The plot segregates fab  issues into several existing and known systematic  issues, such as repeating-defect, design, and normal  random yield loss. The lines on the graph are the  regression of the data points, which indicates that  the design issue is a slightly bigger problem than  that for the repeating-defects. Moreover, design  and repeating defect problems both added about 40  bad cpw.  Besides design and repeating-defect  issues, there are other product types, represented by  square on Figure 2.  These products have a higher  level of bad cpw, and their commonality is 5 metal  layers.  This suggests a unique systematic issue  with 5 metal layers and the above product types.  This issue can impact yield from 50cpw to as much  as 170 cpw.


0.25um Bad Site Failure Modes


0 100 200 300


1000


1500


Sites Tested


Normal


M5


repeating


design


Power (Normal)Power (repeating)Power (design)


Figure 2:  Bad site model plot


b) Positrak: Yield vs Wafer Cassette  Position


Positrak is a yield tool, which plots a wafer yield (in a lot of 25 wafers) verses its cassette position.  Wafers within a cassette were randomized at  various points in the fab. During randomization, wafer id, wafer cassette position, and time-date  stamp were recorded. If there were a correlation  between wafer yield to cassette position, then the  steps between the randomization would be  responsible for the yield degradation.  The higher


frequency of randomization results in the fewer  number of steps between the randomization points.


Regarding the issue with more than 4 metal layers  indicated by Whitlock’s bad site yield model  above, Positrak captured the yield issue between  depositing metal 4 to dielectric 5 etch.  Figures 3  and 4 show the Positrak of a lot with date-time  stamps and its corresponding process steps.


Figure 3: Positrak plot of a 5 metal layer product  lot.  The lot was randomized at 16:36 on Feb 19  and 5:59 on Feb 24.


Figure 4: Process steps between randomization  corresponding to Figure 3 above.


Date Time Process Steps


Fac


# #Wfr


2/24/2001 02:32:10,


1-MTR-D5 ETCH  POSTMEAS


8242 25,YD,


2/24/2001 02:15:56,


1-BLOCK MTR D5  ETCH


8085 25,YD,


2/24/2001 00:48:21, 0- 18-APPLY PR


7927 25,YD,


2/23/2001 23:05:53,


1-EXPOSE & DEVELOP PR


8134D 25,YD,


2/23/2001 21:36:17, 10-APPLY PR


7929 25,YD,


2/23/2001 21:05:46, 12-DEPOSIT D5_2


8130 25,YD,


2/23/2001 18:08:18, 2-DEPOSIT D5_1


9608 25,YD


2/23/2001 03:34:18,


2-MEASURE WAFER  FINAL


8192 25,YD,


2/23/2001 02:00:54, 7-PLASMA PR STRIP


8075 25,YD,


2/23/2001 00:53:07,


2-VISUAL


INSPECTION


8078 25,YD,


2/23/2001 00:44:31, 2-METAL 4 ETCH


10059 25,YD,


2/22/2001 20:55:46,


2-MEASURE LINE  WIDTH


8191 25,YD,


2/22/2001 20:03:19,


8355D 25,YD,


2/22/2001 16:21:48, 16-APPLY PR


7930 25,YD,


2/22/2001 15:56:05, 7-PLASMA PR STRIP


9406 25,YD,


2/22/2001 14:57:53,


10875 25,YD,


2/21/2001 10:23:04,


7781D 25,YD,


2/21/2001 03:52:35, 16-APPLY PR


2/21/2001 03:05:56, 1-DEPOSIT METAL 4


242288 25,YD,


2/19/2001 17:18:45,


24-POST CMP  MEASURE


9223 25,YD,


c) Wafer Yield Profile and common  facility analysis


Positrak and the bad site model provided a guide of  where the problems may be coming from.  The  wafer patterns indicated the problems tended to be  strongest on the outer edge.  Figure 5 showed the  wafer pattern [2] of 6 different products, and 2  different technologies.  White indicates a good  chip, while dark or colors indicate bad die from  different failure modes.  For 326cpw and 542cpw, the yield also appeared to be a repeating pattern (or  flashy) across the wafer (from lower to upper).


Figure 5: Product types with missing pillars issue


Moreover, common facility analysis was done.  Photo, etch, and deposition tools were examined.  Furthermore, when physical failure analysis  indicated missing metal pillars, common facility  analysis placed the focus on photo facilities. The  results pointed to multiple facilities.  This  complicated the task of implementing of corrective  actions.


CONCLUSIONS


A broadband pulse propagation model is presented  to accurately describe the nature of ultrasonic pulses  in microelectronic packages. The model is capable of  predicting the characteristics of ultrasonic pulses  based on measured material and transducer parameters  and can accommodate thin layers explicitly. In  addition, the model is capable of predicting an entire  pulse train that is visible on an oscilloscope. The  model can serve as a practical tool for the failure  analyst by providing a framework for understanding  the nature of ultrasonic propagation in the package.


ACKNOWLEDGEMENTS


The author is thankful for reviews by Puligandla  Viswanadham and Venkataramana Jagarlamudi, and  appreciates the support provided by David Corkum.


1. J. E. Semmens and S. Canumalla, “Application of


highly focused, high frequency transducers for


evaluation of near-surface flaws and thin packages:


Smart cards, Flip chip, Flex circuits and Thick


films, Interpack 99.


2. G. A. Gordon, Canumalla, S., and Tittmann, B. R.,


“Materials Characterization by Ultrasonics,”


Ultrasonics, 31 5, pp. 373-380, 1993.


3. T.M. Moore, S.J.Kelsall, and R.G. McKenna, “The


application of scanning acoustic microscopy to


control moisture/thermal induced package


defects,” Proceedings of International Symposium


for Testing and Failure Analysis (ISTFA), pp. 251-


258,1990.


4. R. S. Gilmore, “High frequency Ultrasonic Testing


of Bonds: Application to Silicon Power Devices,”


Materials Evaluation, pp.65-72, 1979.


5. S. Canumalla and L. W. Kessler, “Towards a


Nondestructive Procedure for Characterization of


Molding Compounds,” Proceedings of


International Reliability Physics Symposium, pp.


149-155, 1997.


6. S. Canumalla and M. G. Oravecz, “Nondestructive


Elastic Property Characterization of IC


Encapsulants,” ASME Symposium on Applications


of Fracture Mechanics in Electronic Packaging, pp.


151, 1997.


7. S.Canumalla, and Schackmuth, B. P., "Metrology


of Thin Layers in IC Packages using an Acoustic


Microprobe: Bondline Thickness," International


Journal of Microcircuits and Electronic Packaging,


23 (1), pp. 146-151, 2000.


8. S. Lees, “Ultrasonic Measurement of Thin


Layers,” IEEE Transactions on Sonics and


Ultrasonics, 18 (2), pp. 81, 1971.


9. V.K. Kinra and C. Zhu, “Ultrasonic


Nondestructive Evaluation of Thin (subwavelength) Coatings,” Journal of the Acoustical


Society of America, 93 (5), pp. 2454, 1993.


10. A. Pilarski, J.L. Rose, and K. Balasubramanian,


“The Angular and Frequency Characteristics of


Reflectivity from a Solid Layer Embedded


Between Two Solids with Imperfect Boundary


Conditions,” Journal of the Acoustical Society of


America, 87 (2), pp. 532, 1990.


11. R. Tilgner, P. Alpern, J. Baumann, G.


Pfannschmidt, and O. Selig, “Changing States of


Delamination between Molding Compound and


Chip Surface: A challenge for Acoustic


Microscopy,” IEEE Transactions on Components,


Packaging and Manufacturing Technology – Part


B, 17 (3), pp. 442-448, 1994.


12. Y. Ranade, M.G. Pecht, and T. M. Moore, “ New


Findings in the Occurrence of False-Healing in


Plastic Encapsulated Microcircuits using Scanning


Acoustic Microscopy,” IEEE Transactions on


Components and Packaging Technology, 22 (3),


pp. 266-269, 1999.


13. A.X.H. Dang, I. C. Ume, and S. K. Bhattacharya,


“A study on warpage of flexible SS substrates for


large area MCM-D packaging,” ASME Journal of


Electronics Packaging, 122, pp. 86–91, June 2000.


14. S. Canumalla, L.W. Kessler, S.K. Bhattacharya,


“Characterization of thin layers in microelectronic


packaging using acoustic microscopy,”4th


International Conference on Adhesive Joining and


Coating Technology in Electronics Manufacturing,


pp. 225-229, 2000.


15. AMKOR product datasheet for S-CSP


16. D. Royer and E. Dieulesaint, Elastic Waves in


Solids I, (Springer-Verlag), 1999.


17. K. Graff, Wave Motion in Elastic Solids, (Dover


Publications), 1991.


18. J. L. Rose, Ultrasonic Waves in Solid Media,


(Cambridge University Press), 1999.


19. S. Canumalla, “Resolution of Broadband


Transducers in Acoustic Microscopy of


Encapsulated ICs: Transducer Selection,” IEEE


Transactions on Components and Packaging


Technology, 22 (4), pp.  582-592, 2000.


LIST OF SYMBOLS


fµ  - Peak or center frequency of the spectral response  of a transducer


BW – percent bandwidth of the spectral response of a  transducer


Γ  - the full-width at half maximum of the Gaussian  function describing the spectral response


354


.2


Γ


fσ


ampG -an arbitrary constant describing the gain or  amplification in the electronics


0δ  - an arbitrarily selected constant to model the  phase distortion found in some commercial  transducers


2 ×


= fπ


- the circular frequency  f  = frequency in MHz


219


water


×


is the attenuation of water at


25˚ C


),


i ηξ


- the incident, reflected and transmitted  pulses in medium i


( )f


ω −


-wavenumber in medium i with  compressional velocity ic , and k0 is the wavenumber  in water


iα  - measured attenuation coefficient in dB/mm


λ ,  - Lamé elastic constants


ρ  - density of ith layer


Zi – acoustic impedance of medium i )


( f


Λ  - magnitude of frequency spectrum of a  transducer


ih  - thickness of the thi  layer


min , f


- minimum and maximum frequencies


used in computing the pulse. For example, using a 500  MHz bandwidth oscilloscope and pulse, one can use  values of 1 and 500, respectively.


Beam-Based Localization Techniques for 0.18um IC Failure  Analysis after Reliability Test


Re-Long Chiu*, Hui Zhang, Wen-Szu Chung, Mark Cherng, Xu Liu


WaferTech LTD, Camas, WA, USA


Locating the defect site in current devices is  complicated by their density and size. Voltage  contrast (VC) imaging and backscattered electron (BSE) imaging are non-destructive beam-based  location techniques. We can locate the defect to  single poly line, contact and via by combining  EMMI, LC, layout and bit map address  information.


Some reliability failure analysis cases are presented  to demonstrate the effectiveness of the beam-based  techniques. VC imaging and BSE imaging are used  to locate the defect site precisely. The subsequent  steps include deprocess and precision FIB cut for  sample preparation. SEM or TEM is then used to  identify failures caused by gate oxide pinhole, contact junction leakage, high butted contact  resistance or tungsten residue.


The biggest challenge of integrated circuits failure  analysis lies in determination of the precise  location of electric defect [1]. Locating the defect  site in current devices is complicated by small  geometry, 0.18um or less, of the transistors used to  form the integrated circuit and the large number of  transistors which are combined to generate the  required logic and memory function. Photo  emission microscopy (EMMI), liquid crystal  microscopy (LC) and bit map information are most  often used to locate the defect. However, liquid  crystal thermograph and photo emission technique  may not precisely locate defects to single transistor  level due to current small geometry and multiple  metal layers. For the memory devices, we can  locate the defect site to the single cell by bit map  information. However, it is limited to further  pinpoint failure caused by poly gate leakage, high  contact resistance, contact leakage or metal-1  residue.


The scanning electron microscope (SEM) has been  used as a standard tool for IC failure analysis for  many years [2]. The SEM’s advantage is not  limited to higher magnification and surface  topography. Voltage contrast (VC) imaging has


been a unique technique to identify defects that are  difficult to locate by other techniques [3,4]. The  intensity of voltage contrast image is largely  determined by static charges on the integrated  circuits. The variation in brightness can be used to  determine the logic levels of digital integrated  circuit. The contrast of SEM image is affected by  operation voltage and sample’s physical properties  such as elemental atomic number, thickness, and  conductivity. By combining EMMI, LC, bit map, and voltage contrast imaging, we can locate the  defect to the poly, contact and via. The  backscattered electron (BSE) imaging detects  differences on elemental atomic number in the  sample. Therefore, BSE is powerful in locating the  defect caused by tungsten residue or metal void.


In this paper we present non-destructive beambased location techniques (A) low beam energy VC  imaging (B) high beam energy VC imaging and (C) BSE imaging to locate the defect site precisely  and perform the delayer, precision FIB cut, and  TEM analysis to solve the reliability problem. We  used the low beam energy (1 KeV) to locate  source/drain contact junction leakage caused by  cobalt salicide (CoSi) formation along the shallow  trench isolation (STI) corner and gate oxide pin  hole problem in the 0.18um IC. High beam energy (5 KeV) was used to locate high butted contact  resistance caused by the defocus in photo process. BSE imaging technique was used to locate the  tungsten residue that filled in the oxide void. Electromigration (EM) voids in metal lines were  also located by BSE image.


A. VC Imaging at low beam energy


The second electron emission efficiency is much  higher when electron beam operates at a lower  acceleration voltage. Therefore, SEM is normally  operated at low beam energy to get higher VC  imaging contrast.


Case 1: Gate oxide pin hole


One unit failed for standby current high was  chemically decapsulated. Initial optical inspection  of the device did not reveal any abnormalities. One  hot spot (Fig. 1a) was observed by emission  microscope inspection under normal testing


condition. There was no anomaly on the metal and  IMD layers observed by the optical microscope and  SEM inspection. The unit was deprocessed to the  poly layer by parallel lapping. Leaky poly line (Fig. 1b) at the EMMI hot spot site was observed  by the voltage contrast (1 KeV) inspection. The  poly layer was removed by the hot KOH solution. Gate oxide pinhole under the leaky poly line was  observed by SEM inspection as shown in Fig. 1c.


Figure 1 (a) One hot spot was observed by EMMI  under normal testing condition. (b) Leaky poly line  at the EMMI hot spot site was observed by the VC (1 KeV). (c) SEM photograph shows gate oxide  pinhole under the leaky poly line.


Case 2: Contact junction leakage


One SRAM chip failed data retention test at single  bit but passed all the other test items. Failure  analysis was started with bitmap. The failure bit  address was identified by the MOSAID tester.


The failed unit was chemically decapsulated. Initial  optical inspection of the device did not reveal any  abnormalities. No hot spot was observed by EMMI


and LC inspection under normal testing condition. There was no anomaly on the metal and IMD  layers observed by the optical microscope and  SEM inspection. The unit was then deprocessed to  the poly layer by parallel lapping. We did locate  the defect site to one single bit using bitmap  information. However, each cell has six transistors  and ten contacts. The low beam energy voltage  contrast inspection was then used to precisely  locate defect site. Two bright contacts (Fig. 2a) on  the NMOS at the failure address were observed by  the low beam energy voltage contrast (1 KeV) inspection. For the source and drain (S/D) contacts  of NMOS, the positive charge can not flows into  the substrate because the conductor is terminated  by a reverse-biased diode. Therefore, the contact  potential should be positive. However, two S/D  contacts are different from others, which indicates  junction leakage at these two contacts. TEM crosssection analysis was performed on the leaky  contacts. The TEM sample was prepared by the  precision FIB cut on the leaky contacts. Abnormal  CoSi profile along the STI corner was observed as  shown in Fig. 2b. The extended CoSi profile along  the STI corner was enhanced by the IM test. The  CoSi diffused along the STI interface causing the  contact leaky to the p-well.


Figure 2 (a) VC image shows extinction of NMOS  source and drain contacts. The beam energy used  was 1 KeV (b) TEM image of a FIB cross section  indicated the CoSi formation along the STI corner


close to P-well caused the data retention failure  after reliability test.


B. VC imaging at high beam energy


VC image reflects charging induced sample surface  and subsurface potential. For the defect which can  affect charges buildup at sample surface, the lower  SEM acceleration voltage exhibits the higher  secondary electron emission efficiency and higher  image contrast. However, for the defect which can  only affect the charges buildup at sample  subsurface, a higher SEM beam energy (5~15  KeV) is needed to generate subsurface charging  and enhance contrast.


Case 3: High butted contact resistance


One SRAM chip failed function test. Bit map was  used to find out it was a single bit failure. The  failed unit was then chemically decapsulated. No  anomaly on the metal and local interconnect layers. The local interconnect layers were removed by  parallel lapping. Low beam energy VC inspection  did not show any contrast difference. Figure 3a  shows SEM image by using the higher beam  energy VC (5 KeV) imaging inspection. For the L  type poly lines with butted contact to the PMOS, the normal bits are bright. The failure bit L-shape  poly line marked by dashed line under the butted  contact is dark. The contrast difference is caused  by high butted contact resistance to the L-shape  poly line and caused floating poly line at the failure  bit after HTOL test. TEM sample was prepared by  the precision FIB cut as shown in Fig. 3b. Dualfocus at the butted contact photo process was  implemented to resolve this problem.


Figure 3(a) SEM image of normal poly with butted  contact are bright. The failure bit poly is marked by  dashed line where it is dark. The beam energy was  5 KeV. (b) TEM cross section of butted contact  profile shows floating poly.


C.  Backscattered Electron (BSE) imaging


Unlike secondary electrons, backscattered electrons  escape from much deeper in the surface, most  coming from about 1/3 the maximum depth of the  electron beam/device interaction volume [2]. The  higher electron beam energy will get better BSE  imaging. The major factor determining BSE  contrast in images is the atomic number of the  target, indicating the nuclear scattering is the  principle electron interaction. Therefore, it is useful  to detect metal residue, metal voids under the  passivation or oxide layer.


Case 4: Metal voids after EM stress


A wide metal line (3um) test pattern failed EM test. BSE image was performed before the passivation  layer was removed. Fig. 4a shows the BSE image  of EM voids (indexed by the white arrow marker) on the wide metal lines that were stressed during  EM test. The narrow metal lines were dummy  metal lines without current stress. Fig. 4b is the  SEM cross section of metal voids in wide metal  lines. Higher magnification SEM picture in Fig.4c  shows that dummy metal line had some voids in  the ARC TiN/AlCu interface. It indicated that  metal voids already exhibited in as-deposited metal  lines and caused EM test failure.


Figure 4 (a) BSE image of voids on the wide metal  lines that were stressed during EM test. The narrow  metal lines were dummy metal lines without stress.


(b) SEM cross section view at the dashed line in  Figure 4a shows the metal voids in wide metal  lines. (c) Higher magnification SEM picture of  dummy metal line with some voids.


Case 5: Metal residue in a SRAM cell


A SRAM failed chip, the failed bit line address was  identified by MOSAID tester but the tester did not  localize the word line address. One hot spot was  observed by EMMI. BSE inspection was then  performed after bit line metal was removed by the  parallel lapping. Fig. 5a shows metal residue close


to the bit line contact. The precision FIB cut shows  the tungsten residue filling in the oxide void caused  bit line contact short to the metal-1 Vss as seen in  Fig. 5b.


Figure 5(a) BSE image showing abnormal bit line  contact  (b) FIB cross section showing W residue  caused bit line contact short to metal-1 Vss.


We have demonstrated nondestructive beam-based  techniques for failure analysis of IC devices. It is  very effective to use different beam voltages to  locate the defect sites in 0.18um devices. Some  cases were described to show the effectiveness of  combining this technique with EMMI, FIB and  TEM to pinpoint failures such as contact junction  leakage, gate oxide pinhole, high butted contact  resistance, metal voids and metal residue problem.


The authors would like to thank Dr. Chrong Niou  and Scott Liao for their help and valuable technical  discussion, Jason Higgins for some FIB cross  section work.


Dummy Metal


1. Shekhar Khandekar, Kendall Scott Wills, Microelectronic Failure Analysis Desk  Reference, Fourth Edition, p171, Electronic  Device Failure Analysis Society (1999)


2. Edward I. Cole Jr., Microelectronic Failure  Analysis Desk Reference, Fourth Edition, p133, Electronic Device Failure Analysis  Society (1999)


3. Valluri R. Rao, Paul Winer, Microelectronic  Failure Analysis Desk Reference, Fourth  Edition, p149, Electronic Device Failure  Analysis Society (1999)


4. Ann N. Campbell and Jerry M. Soden, Microelectronic Failure Analysis Desk


Reference, Fourth Edition, p161, Electronic  Device Failure Analysis Society (1999)


5. John Devaney Microelectronic Failure  Analysis Desk Reference, Fourth Edition, p275, Electronic Device Failure Analysis  Society (1999)


6. A. Nishikawa, N. I. Kato, Y. Kohono, N.


Miura, M. Shimizu, Proceeding of 25th


ISTFA, 239~244 (1999)


This paper outlines a methodology which  accurately identifies fault locations in Mixed  Signal Integrated Circuits (ICs).  The  architecture of Mixed Signal ICs demands more  attention during failure analysis because of the  complexity of measuring both the analog and  digital signals in a compact circuit.  In this  paper, the GHz range of data signal or radio  frequency (RF) signal from an internal IC circuit  will be extracted by a high-impedance active  single probe in order to find the internal IC  circuit failure locations.  The advantages of  using a single probe is that it can maneuver to  extract data almost anywhere in the circuit, providing ranges of bandwidth in GHz with no  loading effect on the circuits during  measurement.  The process of preparing a  sample and extracting a signal will be described.


The introduction of GHz Range Mixed Signal  Integrated Circuits (ICs) has produced a need to  create new techniques that are able to accurately  measure both analog and digital signals.  Many  of the conventional techniques quite often have  difficulty in accurately measuring the analog  signals, especially the GHz data signal or RF  signal.


In Mixed Signal ICs, the circuit is so compact  that the signals usually interfere with each other  during measurement.  Often the signal  interference makes it difficult to extract an  accurate quantitative measurement with a  conventional mechanical probe.


To enable successful failure analysis for Mixed  Signal ICs, we have created a fault analysis flow  chart (Fig. 1).  In order to properly find fault  locations, the following procedures need to be  followed:


Fig. 1 Fault Isolation Flow Chart


First, the failure mode needs to be defined. Once  the failure mode is defined, the circuit needs to  be analyzed in order to find the area where the  hypothesized failure occurs. Depending on  whether the failure can or cannot be pinpointed  from merely performing a circuit analysis, the  fault isolation process will be different.


Agilent Technologies, San Jose, CA, USA


A. If the failure can be pinpointed from  performing a circuit analysis then the device is  decapsulated and the Inter-Layer Dielectrics (ILDs) of the IC are de-layered. The de-layered  IC needs to be set up to run under simulated  normal operating conditions.


The area is then probed using a high-impedance  active single probe2, which can be run using a  computer controlled precision manipulator or  CAD navigator. The internal circuit signals are  then compared to design data or a known good  device to verify the fault-location.


The high-impedance active single probe  outperforms a conventional mechanical probe  due to a combination of high input resistance  and the low-input capacitance. As a result of this  combination, the usual adverse loading effects  are minimized and the GHz bandwidth  performance is maximized. These qualities allow  the active single probe to be used in high-speed  circuits.


B. If the circuit analysis is not able to pinpoint  the failure to a specific area then the device  needs to be handled differently.  The device still  needs to be decapsulated, de-layered, and run  under simulated normal operating conditions. However, in this case the probing process starts  with the failing pin and then continues in an  inward fashion along the signal path. The  internal circuit signals are then measured circuit  block by circuit block. The signals are compared  to design data or a known good device until a  transition point is found.  A transition point  takes place when a good signal is extracted after  a series of failing signals on the path.  The fault  can be located by looking at the last failing  circuit block along the path prior to the  transition point.


This methodology will be explained in more  detail through the use of a case example.  By  following this methodology, fault locations can  be more easily identified.


Case Example


Test Case Device


In order to demonstrate this particular Fault  Isolation Methodology, a Four-Channel Parallel  Fiber Optic Transceiver, which operates from 1  to 2.7 Gb/s per channel (Fig. 2 & 3) was chosen. The typical application of this device is as a  telecom and datacom switch or as a router rackto-rack connection.


Fig. 2 Four-Channel Fiber Optic Transceiver


Fig. 3 Functional Description of a Four Channel  Fiber Optic Transceiver


Identifying the Failure


The data that was gathered from the initial  design debugging process on a Four-Channel  Fiber Optic Transceiver IC indicated that the  receiver (Rx) had two types of failures.  The  receiver has four separate channels, all of which  are supposed to have similar differential output  peak to peak voltages ranging from 500 - 750  mV.  However, it was observed that each of the  four channels generated different peak to peak  output voltages wavering from 380 to 890mV (as seen in Fig. 4).  Not only did the output  values vary from channel to channel, but they  also varied from sample to sample.


RX Differential Output


Fig. 4 Four-Channel Fiber Optic Transceiver   Rx Differential Output Voltages with 600mV   target


Failure Verification with Circuit Analysis – Determining the Cause of Failure


If the failure can be pinpointed during a circuit  analysis, then the following method should be  performed, otherwise follow the method  described in Section B of the introduction.


There are three potential causes based on circuit  analysis for output voltage variation failure as  described below. By performing the following  tests, the possible causes of the differentialoutput voltage variation failure can be identified.


1.  Optical Input  Power vs. Output Voltage  Variation Test


The first test is to induce change into the input  optical power and then monitor the output  voltages to see if there are any changes caused  by the input power variation (Fig. 5).


Fig. 5 Observing Output Voltage Variations


In our case example, the IC evaluation board  was sampled with three different input optical  power levels:-10dBm (Fig.6), -17dBm, -20dBm.


However, no change occurred in the output  voltages, so the input power variation was ruled  out as a possible cause of failure.


Fig. 6 Output Voltage with -10dBm Input Power


2. Output Stage Load Resistor Verification  Test


This test measures the resistors at the output  stage circuit in order to verify if the resistor  values are correct (Fig. 8).


In our case example, an output stage load  resistor designed for 100 Ω was measured and  the data indicated resistance values of 95~97 Ω  was in spec, thus ruling out the possibility of  resistor failure.


3. Bandgap Reference Voltage Verification  Test


This final test uses a circuit-simulation computer  program in order to simulate a change in the  operational amplifier’s offset voltage.  The  operational amplifier is located in the bandgap  reference circuit (Fig. 7). If the offset of the  operational amplifier is changed, a different  bandgap reference output will be generated. The  output swing is determined by ∆V= I*R (R=100 Ω in differential) and I=Vbg*K (Vbg=bandgap  reference output, K=constant). So, if Vbg  changes then ∆V changes proportional to the  Vbg. (Fig. 8)


Fig. 7 Bandgap Reference Circuit Detail


Fig. 8 Rx output stage circuit


In our test case example, the offset voltages of  the operational amplifier are tested using both +/- 3.83mV. With a +3.83mV offset, the  simulated bandgap reference output is 1.245V  and the output swing changes to 674mV.  With a


– 3.83mV offset, the bandgap reference output is


1.169V with an output swing of 542mV (Figs 9 & 10).


The bandgap reference voltages should always  be at 1.2 V.  Since the bandgap reference  voltages with +/-3.83mV offset simulations  returned values between 542mV and 674mV, there was enough evidence to indicate a possible  problem with the bandgap reference circuits.


Fig. 9 Simulated Bandgap Reference Voltage  Circuit with +/-3.83mV Offset


Fig. 10 Simulated Output with +/-3.83mV Offset


However, to physically prove that the problem is  located within the bandgap reference circuit, the  bandgap reference circuit of the IC needs to be  probed with a high impedance active single  probe to measure and verify the bandgap  reference voltages.


In order to probe and verify the faults in the  circuit, the sample has to be prepared as follows:


Simulated Output Swing


-4.00E-01-3.00E-01-2.00E-01-1.00E-01


0.00E+00


1.00E-01


2.00E-01


3.00E-01


4.00E-01


Time Step


-3.83 mV Offset+3.83 mV Offset


Simulated Bandgap Reference Voltages


6.00E-01


8.00E-01


1.00E+00


1.20E+00


1.40E+00


1.60E+00


+ 3.83 mV Offset -3.83 mV Offset


A. Decapsulation of the Fiber Optic


Transceiver


After removal of the module connector and  optics subassembly, the module is decapsulated (Fig. 11).


Fig. 11 Module after decapsulation


Creep, fatigue


Degradation of


the dielectric


Stiction


Charging of


Figure 3: Expected failure and reliability issues in a  capacitive RF-MEMS switch.


In this paper we focus on RF-MEMS capacitive  switches. We discuss some typical failure modes. We  show that the most important failure mode  encountered in these devices is dielectric charging  leading to stiction. We describe different techniques  that can be used to analyse the RF-MEMS switches.


Sacrificial layer removal


The first problems may occur during the release  process of the bridges. The sacrificial layer  underneath the bridge metal has to be removed to  obtain a free standing bridge. If this removal is done  incompletely, residues of the sacrificial layer may  remain under the bridge, as shown in Fig. 4. In this  figure, the bridges were processed on top of a glass  wafer and the residues could be observed optically  through the back of the glass. If the processing is  done on a Si wafer, this is not possible. Lellouchi et  al. [6] showed that in this case infrared confocal


laser microscopy can be used to detect the nonreleased area.


Figure 4: Optical observation of Al bridges of RFMEMS switches through the backside of a glass


wafer. In a and b residues of the sacrificial layer


(photoresist) are observed after incomplete release  etch. c shows a sample where the release is complete.


A second problem that may occur after removal of  the sacrificial layer is stiction. This can be caused by  rinse fluid that remains under the bridge and causes  stiction due to capillary forces, as shown in Fig. 5. This can be avoided by freeze-drying, super-critical  drying, by using vapour HF in the case of a Si-oxide  sacrificial layer or oxygen ashing in the case of a  resist sacrificial layer. Figure 6 shows a SEM picture  of a stuck part (the beam seen at the front side) of an  RF-MEMS bridge.


Al bridge


sacrificial layer


substrate


rinse water


Figure 5: Stiction due to capillary forces, caused by  remaining rinse water. Top: the sacrificial layer is  present under the bridge. Center: after removal of the  sacrificial layer rinse water remains under the free


standing bridge. Bottom: the bridge is stuck due to  capillary forces during drying of the rinse water.


Figure 6: SEM picture of a capacitive RF-MEMS  switch with two bridge beams, showing stiction of  the beam in front (arrow).


Surface roughness: AFM


Stiction depends not only on humidity, but also on  surface roughness [7]. The smaller the roughness, the more prone a bridge is to stiction due to capillary  forces. The roughness can be studied using atomic  force microscopy. However, care has to be taken in  the interpretation of the results: because the RFMEMS bridge is processed on top of a sacrificial  layer, the roughness of the top side of the bridge is  not necessary the same as the one of the bottom side. Fig. 7 shows the result of an AFM study on a Al RFMEMS bridge. First an AFM measurement is  performed on the top of a bridge, as shown in Fig. 7a. Next the bridge is removed using scotch tape and  the bottom side is inspected using AFM (Fig. 7b). The results show clearly a smaller roughness at the  bottom side than at the top side.


Stress induced deformation: optical metrology


Another problem that can occur after release of the  bridge is deformation due to residual stress or a  stress gradient in the metal of the bridge.  If the  bridge material is not optimized for stress – ideally it  should have a small tensile stress – it may change its  shape after release. The processing parameters can  be optimized for stress by using typical stress test  structures, such as Guckel rings [8]. The center part  of these rings will bend if the material used is under  tensile stress. This can easily be studied using noncontact 3D optical surface metrology instruments  that are commercially available. A result of such a  measurement on a Guckel ring is shown in Figure 8. The center part of this ring is clearly buckled. The  amount of buckling depends on the stress and on the  diameter of the ring, and from a study of different


sizes information on the stress can be obtained. Figure 9 shows a 3D surface metrology measurement  on a RF-MEMS device. The bridge in this device is  clearly not perfectly flat, which might affect the  functioning of the device.


a     top side


b    bottom side


Figure 7: Left: microscope picture of a RF-MEMS  bridge, Right: AFM measurement of a 5 µm x 5 µm  area. a) Top side of bridge, Ra = 8.1 nm, b) Bottom


side of bride (removed using tape), Ra = 1.4 nm.


Figure 8: Optical metrology measurement of a


Guckel ring. Top: 3D picture, the colors indicate the  height. Bottom: Cross section along the ring’s beam, showing a clear inward buckling.


Figure 9. Non-contact surface metrology of an RFMEMS switch bridge. a. Top view, the colors


indicate height variations, b. Cross-sections along the  horizontal (x) and the vertical (y) direction.


Electrical lifetime measurements


In order to study the reliability of such switches, an  electrical lifetime measurement instrument was  specially designed and built for this application at  IMEC (patent filed). It allows a very sensitive  measurement of the switching induced capacitance  change, ∆C, of an RF-switch during reliability tests. Voltage pulses slightly higher than the pull-in voltage (i.e. the voltage required to pull the metal bridge  down to the dielectric) are applied with a certain


frequency and duty cycle, and ∆C is monitored as a  function of the number of pulses (i.e. pull-in events). A result of such a measurement is shown in Fig. 10. Here the switching induced change in capacitance is  plotted as a function of the number of switch cycles. In this case, the Al switch failed after 2x106 cycles. During this electrical testing, the out-of-plane  movement of the switches was also monitored using  a novel optical analysis technique, as will be  explained in the following paragraph. The failure  mode was found to be stiction of the bridge. The  cause of the failure was shown to be charging of the  dielectric. Indeed, when the switch is in the on-state, the metal bridge is in contact with the dielectric and  a high electric field is present across the latter. This  results in trapping of charges in the dielectric, which  in turn decreases the pull-in voltage of the switch, resulting in stiction.


Figure 10: Reliability study showing the switching  induced capacitance change as a function of switch  cycles. Failure occurred after 2 x 106 cycles.


Optical lifetime measurements: MOPS


It is not always straightforward to determine the  failure mode and cause from electrical measurements  on the RF-MEMS switches. Optical detection  methods that allow in-situ monitoring of the  movement of MEMS are for this application of great  interest. The instrument used for this purpose, called  in-house ‘MOPS’ (Mems Optical System) was  described in [9]. It consists of a dedicated  interferometer, acquisition and control electronics  and is based on the Optonor Micromap 5000  interferometric system (Fig. 11, right). This  instrument allows to image in-situ small (max. 80  nm) out of plane vibrations of structures with a 3 nm  resolution for frequencies up to 15 MHz. Slow


movements (<10 Hz) can be investigated over a  range of a few µm with a resolution of about 10 nm.  The system can monitor the movement of a device  directly, or detect the movement of a certain part of a  device with respect to another fixed reference part. Fig. 11 shows a picture obtained with this system on  a RF-MEMS capacitive switch.  An optical image is  depicted at the top. An image showing the  interference pattern is first taken without applying  any voltage. This image is used as a reference image. Images taken with an actuation voltage applied are  subtracted from the reference image. As a result, only changes in displacement are shown. An image  of a moving switch where the applied voltage is  below the pull-in voltage, resulting in a movement of  only the center part of the switch, is shown at the  bottom in Fig. 11.


Figure 11. Right: Photograph of the MOPS system. Left: top: Optical image of switch, bottom: image


showing that the center part of the switch moves.


Figure 12: Sequential pictures taken from a moving  defective micromachined relay vibrating at 1000 Hz, using MOPS.


The system allows us to make in-situ movies from  the moving parts of MEMS. An example of  sequential pictures from such a movie is shown in  Fig. 12. Here a relay moving at 1000 Hz is  monitored. The relay is fixed at the bottom side. The  movement clearly shows some anomalies in the  MEMS.


This system is used to monitor the movement of RFMEMS switches during electrical lifetime  measurements as shown in Fig. 10. It allows  correlation of electrical results with failure modes  such as stiction, partial stiction: i.e. one part of a  bridge is still moving while the other part is stuck, and anomalous movement: ex. upon applying a  voltage to a buckled bridge, the edges of the bridge  touch the dielectric first and the remaining part  follows later. This combination of electrical and  optical measurements is very important for a correct  interpretation of the failure mechanisms of these  switches.


0-level packaging


Stiction problems caused by humidity can be avoided  by packaging the RF-MEMS capacitive switches in a  hermetic encapsulate. This encapsulation is in  general done on wafer level, prior to dicing because  standard wafer sawing will if not destroy the device, at least introduce particles that can lead to failure. BenzoCycloButene (BCB), a commercial available  polymer [10], is a potential candidate for the  adhesive bonding of a cap (ex. Si or glass) to the  substrate, forming a 0-level package. Hermeticity  testing of cavities can be done using standard  methods (i.e. MIL-STD-883D) where both fine leak  and gross leak testing is carried out. However, because the cavities of such MEMS BCB-bonded  packages deal with volumes that are much smaller (at  least 1000 x) than the ones described in the MIL  standard, the standard test techniques are not  applicable [11]. The upper detection limit of the fine  leak tests was shown to be well below the lower limit  of the gross leak test, leaving a gap in the detection  region of these two techniques. Leaky cavities can in  this way still escape from detection with these  standard techniques. Jourdain et al. [12] showed that  this detection gap can be bridged through the use of  microbolometers and MEMS resonators.


In order to find out at which position the BCB-bond  of a sealed package fails, scanning acoustic  microscopy (SAM) can be used. Figure 13 shows a  SAM picture of a cavity that failed the gross leak  test.  It clearly shows the positions of bad bonding (dark areas indicated by arrows).


Figure 13. SAM picture of a Si cap bonded to a Si  wafer using BCB. The black areas indicate positions  where the bond failed (arrows).


Bad handling


SEM remains one of the most useful techniques for  failure analysis of MEMS. As all MEMS devices, RF  MEMS are also sensitive for ‘bad handling’, especially before packaging. An extreme case is  shown in Figure 14. Failure analysis of this device  was straightforward. Bad handling of this device  resulted in nice SEM pictures but also in a RFMEMS switch which is beyond repair.


Figure 14. SEM picture of a damaged RF-MEMS  switch.


In this paper we described some reliability and  failure analysis issues of RF-MEMS capacitive metal  switches. Issues such as residues, capillary and  charging induced stiction, stress induced buckling,


electrical lifetime testing, optical motion  investigation and 0-level packaging were discussed.  It is shown that commonly used techniques for  failure analysis, such as SEM, AFM and SAM, can  also be applied to study RF-MEMS switches. However, also dedicated techniques are required  such as instrumentation for electrical lifetime testing  and for monitoring of the movement of the switches.


This work was performed in the frame of the ESA  project MEDINA 14627/00/NL/WK and the EC  project MIPA, IST-2000-28276. The authors thank  Danielle Vanhaeren for AFM and metrology  measurements and Olivier Vendier (Alcatel Space  Industries, France) for providing the SAM pictures. Joern Dechow, Markus Ulm and the RF-MEMS team  of  Robert Bosch (GmbH) are thanked for providing  samples. The whole IMEC RF-MEMS team is  acknowledged for providing samples and for many  stimulating discussions.


1. G. M. Rebeiz, J.B. Muldavin. IEEE Microwave  magazine, pp. 59-64, Dec. 2001


2. J.J. Yao. Topical Review. RF MEMS from a


device perspective. Micromech. Microeng. 10, R9-R38, 2000


3. X. Rottenberg, Jansen H., Fiorini P., De Raedt  W. and Tilmans H.A.C. Accepted for


presentation at EUMW 2002, March 2002


4. C. Goldsmith, J. Ehmke, A. Malczewski, B.


Pillans, S. Eshelman, Z. Yao, J. Brank and M.


Eberly.  Proceedings IEEE MTT-S 2001


International Microwave Symposium, Phoenix, Arizona, 20-25 May, 2001, pp. 227-230, 2011


5. E. Ezhilvalavan and T-Y Tseng. J. Appl. Phys, 83(9), pp. 4797-4801, 1998


6. D. Lelluchi, F. Beaudoin, C. Le Touze, P. Perdu , R. Desplats. Proc. ESREF 2002, Rimini, Italy


7. W. M. van Spengen, R. Puers and I. De Wolf.


Accepted for publication in J. Micromech.


Microeng., 2002


8. H. Guckel., Burns D., Rutigliana C., Lovell E,


Choi B. J. Micromech. Microeng. 2 (1992),


USA, February, pp.86-95, 1992


9. van Spengen, W. M., De Wolf I., Puers, B., and  Vikhagen, E. In: Proceedings of the 27th


International Symposium for Testing and Failure  Analysis (ISTFA), 2001. pp. 357-364.


10. G.M. Rebeiz, J.B. Muldavin. IEEE Microwave  magazine, pp. 59-64, Dec. 2001


11. M. Nese, R.W. Berstein, I.R. Johansen, R.


Spooren. Proceedings of Transducers ’95, pp.


94-99, June 1995


12. A. Jourdain, P. De Moor, S. Pamidighantam and  H.A.C. Tilmans, Proceedings MEMS 2002, Jan. 20-24, Las Vegas, pp. 677-680, 2002


Jeremy A. Walraven, Edward I. Cole Jr., Danelle M. Tanner, Seethambal S. Mani, Ernest J. Garcia, and Marc A. Polosky


Sandia National Laboratories  Albuquerque, NM  87185-1081


Electrical and Physical Failure Analysis


Supporting the yield analysis is electrical and  physical failure analysis (FA).


a) Physical Failure Analysis


Low yielding wafers were subjected to electrical  and physical FA.  The combination of Liquid  crystal (LC), emission microscopy (EMMI) [3], and passive voltage contrast (PVC) [4] were  applied to isolate this failure mode.  Die from  across the wafer were examined.  LC and EMMI  both found repeating area defects, not a point  defect.  Missing pillars occurred randomly from the  same repeating area.  Wafers from different codes  and different lots were subjected to the same FA.  The same results occurred on multiple lots, multiple codes, and multiple technologies.   Further


isolation using PVC found missing pillars, shown  in Figure 6.  Without the pillars, the Tungsten  plugs punched through to the dielectric level below  but failed to touch the lower level via, creating an  opened failure mechanism.  In some cases, the  Tungsten plug managed to punch through and  touch the lower level plug.


Figure 6: Fault isolation found missing metal  pillars


Figure 7 shows a top down view of normal metal  pillar, missing pillar, and an eroded pillar with  cross sectioned.


Figure 7: Pillar patterning and metallization.


Since there is a repeating signature on this issue, photo mask of metal 4 was inspected for possible  defect.  Mask inspection did not find any defects.


b) Electrical Failure Analysis


Low yielding wafers from Figure 5 mostly failed  loose functional, a generic bin at probe.  To  understand more details, the wafers were also  subjected to all sites grid-IV (scribed line IV  structures) mapping.  Grid IV structure can be used  to measure metal line width, metal line resistivity, drive current, and other parametric data.  Then, the  electrical grid IV data was plotted against yield to  find a correlation.  Figure 8 shows the IV data of  multiple issue lots plotted against yield.  For this  issue, metal 4 line width (LW) was found to  correlate with yield.


Good Pillar↓    Missing Pillar↓      Eroded Pillar↓→


Figure 8:  IV parameters, eg. Metal 2 LW, M2  resistance (RT), Metal 4 LW, and M4 Metal 4  resistance plotted against yield.


Since “Positrak” and physical FA indicated Metal  4, focus was placed on the metal 4 line width  verses yield.  As metal 4 line width reduced so did  the yield.


c) KLA and Inline Inspections


Selected product types were subjected to intense  in-line inspections, which included optical and  KLA (Scanning Electron Microscopy based) inspection of metal 4 photo resists (PR) and metal  4 pillars.  At the outer edge of the wafer, photo  resist for M4 was found to be coned shape and  sometimes fallen aside.  Consequently, metal 4  would be coned shape (resistive) or missing  altogether.


Figure 9: Inline inspection find of fallen metal 4  photo resist.


Root Cause Analysis


Yield analysis indicated a metal 4 patterning issue, electrical analysis indicated a metal LW issue, physical analysis indicated a missing metal 4 pillar  and “flashy” yield lost, and in-line inspection  confirmed PR issue.  Photo focus/exposure margin  may be the cause.  Added to the issue was wafer  planarization.   Furthermore, PR etching and metal


etching also contributed to the definition of metal  pillars.


a) CMP and Planarization


What contributed to the photo problem was  planarization by CMP, and CMP uniformity  depended on metal density.  Wafers polished by  CMP have within die and within wafer thickness  variation.  The degree of within die variation  depends on the metal density.  CMP polished fast  around the outer edge, causing within wafer  thickness variation.  CMP recipes, CMP tools, and  metal-fill are needed to come together to improve  planarization across the wafer and within die. Figure 10 shows an example of within die  thickness variation.


Figure 10:  Within die thickness variation


b) Lithography-Focus/Expose Budget


Chip planarization and level of chip details added  to photo focus/exposure variation.  The stepper  focused/exposed on a set of mask, and stepped  across the wafer using the same set of mask.  Focused/Exposed on a set of mask is called flash  field.  A Flash field or a mask contains 1x1, 2x2, 3x3, 4x4 die, depending on the size of the die.  A  focus/exposure study was done to verify the degree  of within flash field focus variation and within die  focus variation.  The study also helped to  determine the focus/exposure margin.  Furthermore, using the same photo mask, experiments were carried out with different photo  resists to add more focus/exposure budget.  Figures  11 and 12 showed the results of focus/exposure  margin studies using PR1and PR2.  The Y-axis  shows the diameter of the pillar while the X-axis  shows the focus/exposure offset values.


From the images, PR2 gave much better pillar size  over the range of the focus/exposure values.   This  meant that PR2 can provide better metal definition  over the range of topology across the wafer. Furthermore, Figure 13 shows the top down view  of pillars from PR1 and PR2.


M4 Pillars Critical Dimention Focus Photo Resist #1


0.30


0.40


-0.75 -0.60 -0.45 -0.30 -0.15 0.00 0.15 0.30 0.45 0.60 Focus (um)


LCFP CD1P CD2P CD3P CD4P


Figure 11: Photo Resist 1 and pillar sizes over the  range of focus/expose margin.


M4 Pillar Critical Dimention Focus Photo Resist #2


0.55


0.60


0.70


0.75


-0.5 -0.4 -0.2 -0.1 0.1 0.25 0.4 0.55 0.7 0.85 Focus (um)


Figure 12: Photo Resist 2 and pillar sizes over the  range of focus/expose margin.


Figure 13: top row is PR1 and second row is PR2, with the same range of focus/exposure.


It’s clear from the study that PR2 gave a much  better pillar profile.  Lot splits were carried out  with 2 different resists and each resist with the  same range of focus/exposure offset.  The result  can be validated with actual wafer yield.  Figure 14  showed the yield result of a 304 cpw lot with a  missing pillar issue, half using PR1 and the other  half using PR2.


Figure 14: PR1 and PR2 vs Yield, 304 cpw yield  with respect to focus/exposure values.


From the photo studies, it is clear that PR2 showed  much more latitude in terms of line width  definition, and resulted in more consistent yield  with changes in focus/exposure conditions.


c) Metal Etch and Pillar Profile


Interacting with the focus/exposure offset is the  etching process.  Splits were run to determine  which etch tools would have better pillar profiles  and with which PR types.


The results are shown in Figure 15 below.  It was  found that, at least for upper metal layers, etch tool #2 is better than etch tool #1.  Arrows pointed to  pillars, which in Figure 16, shows the tracking of  pillar to wafer yield end-of-line.


Figure 15: Upper 2 rows are final pillars using etch  tool #2, and bottom 2 rows are final pillars using  etch tool #1.  Arrows pointed to narrowed pillars.


Figure 16: Metal etch #1, its pillar, and wafer yield.


CP1 GCW


Average


0 30 60 90 120 150 180 210 240


PFI66-.2 2


10.5


6.36396103


6.0


6.6717


PFI66-.1 2


94.5


19.09188309


81.0


20.0151


PFI66_nom 2


184.5


10.60660172


177.0


11.1195


PFI66+.1 2


174.0


45.254834


142.0


47.4432


PFI66+.2 2


201.0


9.89949494


194.0


10.3782


PFI220-.2 3


202.0


34.69870315


210.0


164.0


32.6172


PFI220-.1 3


209.66666667


14.6401275


212.0


16.3086


PFI220_nom 3


225.0


8.88819442


222.0


218.0


5.9304


PFI220+.1 3


194.33333333


27.7908858


204.0


163.0


17.7912


PFI220+.2 3


199.66666667


43.75309513


209.0


152.0


42.9954


44259 - Metal 4 PR Resist/Focus Offset Split - t l   i t/  ff t lit


Point Count Average StdDev.


Median


Q1


Q3


IQR


MAD


<--PR1


PR2-->


ME#1


Results and Corrective Action


The parameters that affected pillar profiles are  metal density, CMP planarization, focus/exposure  margin, photo resist type, and metal etch tool.  Due  to the missing pillars, the combination was  particularly critical at metal levels above M4.  Consequently, new CMP recipe was developed to  improve cross wafer uniformity.  Upper level metal  density was revised with new reticle to help with  CMP and Photo.  Photo changed the  focus/exposure optimal setting to get better within  die and within wafer variation.  For upper metal  level, only metal etch #2 can be used.


With the implementation of the changes, particularly photo exposure/focus margin and metal  etch combination, the yield showed immediate  improvement.  Figures 17 and 18 showed the  results of the implementation.  Note that yield  increased to 90% from 80% and remained there.


Agere Systems’ Orlando wafer fab has  implemented routine inline inspections and  measurement of pillars for all technologies  between 0.25µm to 0.16µm.  Moreover, metal  pillars are part of the structure being used to  determine optimum focus/exposure value.


Figure 17: 1236cpw yield with process changes


Figure 18: 542cpw yield result without the pillar  issue


Acknowledgement:


The authors would like to thank the FIB staff, Shawn Anderson and Ben Rossie, for their  dedication in the search for missing pillars.  Also, many thanks to Mike Twiford for some of the  electrical analysis, Brad Albers, Jeff Neve and  Todd Hendry for driving in-line inspections.


1) S. Whitlock, "Basic Area Dependency Yield


Model", Arizona State University's 2002 Modeling  and Analysis of Semiconductor Manufacturing


(MASM) Conference, author, (2002).


2) S. Whitlock, "Temporal Analysis of Spatial


Anomalies", Sematech's 16th Statistical Methods


Symposium, (1999).


3) H. Ishizuka, et al., “Advanced Method of Failure  Analysis Using Photo Spectrum Emission  Microscopy”, ISTFA Proceedings, 13 (1990).


4) J. Colvin, “A New Technique to Rapidly  Identify Gate Oxide Leakage in Field Effect  Semiconductors Using a SEM,” Proc. Rel. Phys. Symp., 28, 331 (1990).


Reliability and failure analysis of RF MEMS switches


Ingrid De Wolf, W. Merlijn van Spengen*, Robert Modlinski*, Anne Jourdain,  Ann Witvrouw,  Paolo Fiorini and  Harrie A. C. Tilmans


IMECvzw, Leuven, Belgium; *also with E.E. Dept. of K.U.Leuven, Belgium


In this paper we discuss reliability and failure  analysis issues of RF-MEMS capacitive switches. We describe specific instrumentation and methods  that can be used for testing and examination of these  switches. These include SEM, AFM, SAM, static and  dynamic optical investigation and electrical lifetime  testing. Processing as well as testing and packaging  issues are discussed.


RF-MEMS [1,2] are sometimes called the ‘next killer  MEMS’. They are developed for RF switching, tunable capacitors and adaptive impedance matching, this for use in base stations, anti-collision radars for  automotive, GPS, WLAN, mobile phones, phase  shifters for satellite-based radars, satellite  communication systems etc. They offer a  substantially higher performance (low loss, high  isolation, good linearity) than their solid state  counterparts  such as varicaps (pn-diodes), pin  diodes and GaAs field effect transistors (FET). In  addition, they allow for more miniaturization. Cost  savings are expected because they allow for planar  integration. For example inductors, tunable  capacitors and other components can be fabricated  on the same substrate. A market study (Nexus) showed that at this moment more than 100 institutes  and companies worldwide are involved in RF MEMS  design and development. The real breakthrough of  RF-MEMS is expected in the years 2004-2005.


RF-MEMS switches and tunable capacitors use  mechanical movement to achieve a short circuit or a  change in capacitance. Fig. 1 shows side and top  views of a capacitive RF-MEMS switch. A metal  bridge (mostly Al or Al alloys) is fixed at its ends to


the ground lines and bridges the signal line. The  signal line is locally covered by a dielectric, typically  SiO2, SiN or Ta2O5. When the bridge is in the up  position, the capacitance between the bridge and  signal line is small and the RF signal can pass  without much loss. When the bridge is pulled down, by applying a DC voltage between bridge and signal  line, the capacitance increases and the RF signal will  be shorted to ground. Because of under-etching  requirements, most bridges have small or larger holes  in them, as for example shown in the SEM picture of  Fig. 2.


SIDE VIEWS


ON-state


OFF-state


“small” C


“large” C


Highly resistive substrate


TOP VIEW


GND


signal


line


dielectric


Flexible metal bridge


RF in


RF out


Figure 1: Side and top view of a capacitive RFMEMS switch.


Fig. 2. SEM photograph of a RF-MEMS capacitive  switch [3].


The reliability of RF-MEMS is reported to vary  between 1 and 10 billion cycles. Some applications  require only one switching event, others more than  200 billion. Although mature MEMS switches are  reported on in literature, long term reliability has not  really been addressed yet. Reported reliability and  failure issues (Fig. 3) are the mechanical integrity of  the beam material, power handling, stiction and  charging of the dielectric [4,5]. Also the packaging  of the RF-MEMS is an important issue. It is  preferable that these devices be packaged at the  wafer level, in a low humidity hermetic package. Packaging is at the moment still the most expensive  part of the RF-MEMS. The effect of packaging on  functionality and reliability of the switches is also  still an issue of concern.


Surface micromachined micromirror technologies are  being employed for various commercial and  government applications.  One application of  micromirror technologies in the commercial sector  can be found in Digital Light Projection (DLP) systems used for theater and home entertainment  centers.  DLP systems developed by Texas  Instruments uses DMD technology (Digital Mirror  Device), an array of micromirrors, to project light  onto a screen [1].  This technology is also used by  Infocus projection systems and widescreen tabletop  televisions [2].  Here, the micromirrors act as  individual pixels, reflecting light onto the screen with  high “digital” resolution.  The most recent  application of surface micromachined micromirror  technology is optical switching [3], which uses  micromirrors to switch optical signals from fiber to  fiber for lightwave telecommunications [4].  Companies such as Lucent have fabricated entire  optical micromirror switching systems based on their  Microstar technology [5].  For government  applications, surface micromachined micromirror  arrays have been developed for potential use in a  spectrometer system planned for NASA’s Next  Generation Space Telescope (NGST) [6].


Various processing technologies are used to fabricate  surface micromachined micromirrors.  The  micromirror arrays developed by TI and Lucent [1,4] uses metal for their structural and reflective  components.  Micromirrors fabricated at Sandia  National Laboratories use the SUMMiT (Sandia’s  Ultra-planar MEMS Multi-level Technology) process  with metal deposited on the surface of mechanical  polysilicon components to reflect light.  Optical  micromirror arrays designed and fabricated at Sandia  for potential use in the NGST have undergone  reliability testing and failure analysis.  This paper  will discuss the failure modes found in these  micromirrors after reliability testing.  Suggestions


and corrective actions for improvements in device  performance will also be discussed.


Surface micromachined micromirrors have been  fabricated as a potential candidate to replace a  conventional fixed slit mask currently used in  spectrometer instruments for satellite imaging.  The  fixed slit mask is used to select a specific region of an  optical signal for analysis.  The micromirror array for  the NGST is designed to reflect light from objects in  space given off at near infrared wavelengths (0.6 – 20 µm) but optimized for 1 – 5 µm wavelengths.  The  NGST would be used with a 6.5 m diameter primary  mirror to replace the Hubble Space Telescope with a  primary mirror diameter of 2.4 m.  The NGST would  be inserted into space at an orbit beyond the current  orbit of the Hubble Telescope (380 miles) and even   the moon.  This is to reduce thermal noise.  A design  for the NGST is shown in Fig. 1.


Fig. 1.  NASA Goddard Space Flight Center concept for  the NGST.


Spectrometer


system


Light shield/


Solar panel array


Incoming  light


The micromirror technology designed to replace the  fixed slit mask operates in one of two states, off and  on.  In the on position, the light is directed into the  instrument, allowing the signal to be processed.  In  the off position, the optical signal is directed away  from the spectrometer.  This will reduce the noise  caused from extraneous optical signals entering the  spectrometer and allow easier processing of the  existing light entering the telescope.


Micromirror arrays have been available for several  years.  Significant research and development has  brought micromirrors from a laboratory wonder to  commercial applications.  Micromirrors can be  fabricated in 1-D, 2-D, or 3-D configurations.  In the  1-D configuration, the mirrors control the reflected  light by tilting about a single axis parallel to the plane  of the micromirror array.  The 2-D configuration  allows tilting along orthogonal positions both parallel  to the plane of the array.  3-D or analog architectures  steer light along the x and y planes as well as  perpendicular to the array [3].  The micromirrors  fabricated for potential use in the NGST have a 1-D  architecture.


The micromirror solution for the NGST required  fabrication of 4 million micromirrors.  Each  micromirror acts as an individual pixel, allowing  each micromirror to be addressed independently.  This array would consist of 2,000 x 2,000  micromirrors each with a 100 µm x 100 µm surface  area.  The large surface area allows more flexibility  in the actuation design and spring stiffness.  The  entire array of micromirrors would measure 20 cm x  20 cm.  The voltages required to move these  electrostatically operated mirrors will vary depending  upon various design parameters.  These parameters  include gap spacing between powered electrodes, spring stiffness, capacitor plate size, capacitor plate  location, and process materials (polysilicon, metal, etc.) used.  The entire system of micromirrors, and  detectors designed for the NGST will result in  approximately two orders of magnitude improvement  in sensitivity (and signal to noise) over previous  spectrometer systems.


Fabrication


The optical micromirrors used in this experiment  were batch fabricated using the SUMMiT V™ process, consisting of 5 layers of polysilicon (poly).  Fig. 2 shows the layers of the SUMMiT V process


[6].  The first layer (poly 0) acts as the initial  capacitive plate element.  By biasing the capacitive  plate, the mirror is pulled to the fixed plate via  electrostatic attraction, inducing tilt about the fixed  pivot point.  The poly 0 layer is separated from the  substrate by thermal oxide and silicon nitride.


Three poly layers provide structural stability and  mechanical motion.  Poly 1 is used to form the other  half of the capacitive plate element.  This component  is anchored to the mirror and is attracted to the poly 0  electrode (other half of the capacitive plate element) when it is biased.  The springs fabricated in poly 1  are anchored to both the mirror and the substrate.  These springs provide the restoring force needed to  pull the mirror back to the as-fabricated position.  They also serve as the suspension mechanism  preventing the mirror from contacting the substrate.  Poly 3 is used to make the mirror layer of the device.  The poly 4 and sacox 4 layers were not used in the  fabrication of this design.


In the unreleased state, sacrificial layers of silicon  dioxide (oxide) separate the structural poly layers (1-3) from each other, and poly 0.  The final step of the  fabrication process is the removal of the sacrificial  oxide layers using a hydrofluoric (HF) acid bath.  The acid bath (release process) etches away the  sacrificial oxide (sacox), releasing the poly structure  and allowing the free-floating components to move.


These micromirrors were fabricated without any  reflective metallization for testing purposes.  The  final product would be metallized to reflect the  desired infrared (IR) wavelengths into the IR  detectors and spectrometer.


Micromirror Operation


Micromirrors used in this experiment were batch  fabricated in various array sizes.  These arrays were  fabricated at a smaller scale than those proposed for  the NGST application.  The dense configuration  proposed for the NGST would allow for more control  over the light entering the telescope during  observation.


Densely configured micromirror arrays offer unique  challenges to actuator design and fabrication.  The  design constraints of the micromirror array required


Sacox 1 Poly 3


Sacox 3


Poly 0


Silicon Nitride


Poly 2


Sacox2


Poly 1


Thermal SiO2


Dimples


Substrate Poly 4


Sacox 4


Fig. 2.  SUMMiT V™ process shows various layers of  structural polysilicon, sacrificial oxides, and nitride layers.


the actuation mechanism (mechanism used to provide  motion to the device) be fabricated directly  underneath the mirror.  The mirror must also  maintain 10o of tilt when actuated.


The mirror angle in the off and on positions is  important in creating a properly functioning  micromirror array.  When the mirror is tilted to the  off position (power is applied and the mirror is tilted  10o), light is reflected off the mirror to a baffle that  does not enter the spectrometer instrument [7].  When  the mirror is in the on position it is in the asfabricated position and the light is reflected into an  IR detector array.  For this operation, it is crucial that  the micromirrors be accurately controlled.  Accurate  micromirror positioning is maintained through the  use of mechanical stops.  The position of these  mechanical stops is determined in the fabrication  process.  These mechanical stops are located directly  underneath the mirror.


The electrostatically actuated micromirror used in  these experiments consisted of capacitive electrode  pairs that actuate a 2 µm thick, 100 µm x 100 µm  area mirror.  Several micromirrors are fabricated to  form a 3 x 3 array shown in Fig. 3.  The center mirror  shown in Fig. 3 is in the actuated (pop-up) position.  This position corresponds to the off state for NGST  functionality.  The upper capacitive plate element is  attached to the mirror through a flexible torsion  spring element shown in Fig. 4.  This allows the  upper plate to rotate downwards about the pivot point  when a potential is applied to the poly 0 capacitive  plate [9].  The mirror and torsion springs are held at  ground while the poly 0 plate is biased.  As the plates


are brought closer together, the force between them  increases as:


F = 1/(gap spacing)2


Devices with large gap spacing will require a large  voltage to pull them into the actuated position.  Therefore, a compromise must be made between the  total tilt angle of the mirror and the actuation voltage  used to operate it.  Electrostatically actuated mirrors  with high tilt angles typically require high voltages (> 100 V)


Landing structures are fabricated along the top  actuation plate.  When the mirror is fully actuated, the landing structures contact a region of poly 0 that  is also held at ground.  This limited the tilt angle and  prevented lateral tilt along the width of the mirror.  AutoCAD rendered cross sections of the suspension  springs; landing structures, and poly 1 capacitive  plate elements are shown in Fig. 4.  The pivoting  design provides up to 10o of tilt per micromirror [8].  Using an off-center pivot point increased the degree  of tilt but resulted in a slightly higher actuation  voltage.  The use of a flexible capacitive plate design  shown in Fig. 4 mitigated this problem and resulted  in lower actuation voltages.  The voltage required to  pull the flexible capacitive plate down and position  the mirror to 10o of tilt is the “snap-in” voltage.  A  schematic of a micromirror and capacitive plates in  the snap-in position is shown in Fig. 4.


The micromirror array used in these experiments has  9 independently actuated mirrors positioned in a 3x3  configuration.  In characterizing the array, electrical  testing was performed on each micromirror  individually to verify functionality.  We used a  Pragmatic Model 2414A Arbitrary Waveform  Generator to provide a DC signal and a 15X gain  amplifier to boost that signal.  All voltages were


Fig. 3.  SEM micrograph of a surface micromachined


polysilicon micromirror array.  The middle mirror is in the


actuated (pop-up) position while the rest are in the asfabricated position


Fig. 4.  Schematic illustrating the actuation (pull down) of  the micromirror.


Actuated


mirror


Flexible pivot for  capacitive element


Capacitive


plate elements


Mirror pivot


measured with a Hewlett Packard Model 34401A  multimeter.  Only one mirror was tested at a time.  All other mirrors in the array were grounded during  testing to eliminate potential cross talk or other  interference issues.


All micromirrors were electrically inspected via  continuity testing to confirm no shorts or anomalous  electrical behavior were present prior to reliability  testing.  These tests showed that all the mirrors had  their electrical integrity maintained prior to snap-in  testing and electrical overstress.


The procedure to determine functionality began when


25.5 V was applied to the capacitive plate of the  mirror under test. The voltage was increased in 1.5 V  increments until snap-in or shorting occurred.  The  snap-in voltage is defined as the voltage required to  position a micromirror at 10o tilt.  If the mirror  shorted before snap-in, that voltage was recorded and  the next mirror was tested.  If snap-in occurred, turning the voltage off and on several times at the  snap-in voltage tested mirror functionality.  After the  snap-in voltage was verified, the voltage was  increased in 1.5 V steps until shorting occurred.  When shorting occurred, the voltage was recorded  and the next mirror was tested.


The data show a large variability in results for  functionality and snap-in voltage.  In Fig. 5, the  shorting voltages for the non-functioning mirrors  were plotted versus mirror location.  The code to the  mirror array is shown in the upper right hand corner  of the plot.  There is no correlation between shorting  failure and mirror location or die location.  The  average shorting voltage was 50.0 ± 4.9 V.


For those mirrors that did function and snap-in, the  data shows large variability in snap-in voltage from


mirror to mirror.  The data indicated no correlation  with mirror location in the array of die locations on  the wafer.  The 66 functional mirrors tested provided  the data shown in Fig. 6 where the data was sorted  according to snap-in voltage.  For reliable operation, a good separation between snap-in voltage and  shorting voltage is desirable.  The data indicates  some cases where snap-in and shorting occur at the  same point for snap-in voltages above 36 V.


Results of these snap-in electrical tests revealed that  micromirrors failed in one of two manners.  One  failure mode occurred at lower (ramp up) voltages.  The voltage was applied in steps and the micromirror  failed prior to actuation (no motion).  These failures  are electrical shorts where no motion was observed  and the mirrors are in the flat or as-fabricated state.  The other failure mode occurred at voltages at or  above the snap-in voltage.  Here, the mirror has  shorted after snap-in (full 10o of tilt).


Failure Analysis


Analysis of failed micromirrors was performed using  I-V electrical continuity, Nomarski-DIC optical  microscopy, scanning electron microscopy (SEM), focused ion beam (FIB), and thermally-induced  voltage alteration (TIVA) [10].  These techniques  rapidly identified the failure mechanism, failure site, and root cause of failure.  After verifying the short  and mirror position (flat or pop-up state), TIVA was  employed to locate the source of the short.  The  shorting location was later verified using both SEM  and FIB analysis.


Failure analysis of both failure modes revealed the  mirrors were shorted to different biased components  directly under the mirror surface.  Fig. 7 shows the


30 35 40 45 50 55 60 65 70


1 11 21 31 41 51 61


Mirror


Snap-In Shorting


Fig. 6.  This plot of the snap-in and final shorting voltage  of the functioning mirrors shows the variability of the data.


35 40 45 50 55 60 65 70


Mirror Location


H


Fig. 5.  This plot of the shorting voltage of the nonfunctioning mirrors shows the variability of the data.  The  mirror array code is in the upper-right corner.


A B C D E F G H I


micromirror positions for failed mirrors in the flat  and pop-up states.  Using Nomarski-DIC imaging, micromirrors that fail in the flat position (B, C, D) are bright, and those that failed in the pop-up position  (A, E, F, G, H, I) are dark.  The mirrors are labeled  A-I to indicate the location with the snap-in test of  Fig. 5.


For micromirrors that failed in the flat position we  observed irregularities in the suspension springs.  Mechanical components underneath the polysilicon  mirror could be analyzed using IR scanning laser  microscopy techniques.  The mirrors used in this  experiment were not metallized, allowing structural  characterization of the mechanical layers through the  mirror poly layer using IR.  IR analysis allowed  structural characterization of the entire 3 x 3 array as  well as each mirror independently.  Infrared (IR) imaging of a micromirror shown in Figs. 8a and b  revealed structural damage to one of the suspension  springs.  The damaged spring has a non-uniform  image (various light/dark contrast) when compared to  a structurally sound suspension spring (Fig. 8b) that  has uniform contrast down its entire length.


Analysis of this non-uniformity led us to focus on the  distorted spring region and the poly layer below it.  TIVA analysis of this area revealed a short along the  edge of the outer spring.  As shown in Figs. 9a and b, the reflected light image and TIVA image reveal a  short between the spring and the poly 0 power line  directly underneath it.  Further analysis using the FIB  showed points of contact between the springs and the  power line shown in Fig. 10.  When power was  supplied to the poly 0 capacitor plate, electrostatic  forces were generated between the poly 0 power line  and the suspension spring.  The power line supplies  voltage to the poly 0 capacitive plate, generating the  electrostatic force needed to pull the other capacitive


plate, connected to the mirror, into the tilted position.  These forces (in mirrors that failed in the flat  position) were strong enough to pull the spring into  contact.


Initial specifications and calculations showed the  springs were designed and fabricated at the desired  stiffness to prevent lateral pull down.  Unfortunately, the model to develop spring stiffness did not take into  account torsional effects along the width of the  spring.  In this failure mechanism, we believe the  suspension spring lacked the required torsional  support to prevent it from being pulled down during  power up.  This unaccounted lack of torsional rigidity  led to many mirror failures prior to actuation.


The other failure mechanism occurred in mirrors that  failed in the pop-up state.  Here, mirrors are fully  actuated but permanently stuck in the pop-up  position.  A stuck micromirror is shown in Fig. 11  with the failure site identified in the bottom portion  of the image.  Testing at voltages exceeding their


Fig 7.  Nomarski-DIC optical micrograph of a 3 x 3


micromirror array with mirrors failed in the flat and pop-up  states.  Mirrors are marked A through I to indicate mirror  location.


Flat


Pop


- up


Fig. 8.  Infrared image using a 100x silicon corrected  objective through two micromirrors.  a) Non-uniform  contrast along a deformed suspension spring, b) uniform


contrast along a functional suspension spring.


snap-in voltage, as shown in Fig. 6, resulted in failure  by electrical shorts.  Analysis of these mirrors  revealed a short along the edge of the capacitive  plates.  Contact feet are fabricated on the back end of  the poly 1 capacitive plate.  Its landing pad  counterpart is fabricated directly behind the poly 0  capacitive plate.  The landing pad is held at ground  while the poly 0 electrode is actuated.  The mirror is  pulled into the tilt position by electrostatic attraction  of the other capacitive plate.  The contact feet are  designed to land on the pad and prevent the upper  capacitive plate from contacting the bottom plate  when the micromirror is fully actuated.  During snapin voltage testing, the devices were fully actuated to  10o tilt.  The feet were in contact with the landing  pad.


Failure analysis of these shorts revealed tight space  tolerances and contact between the two capacitive  plates.  As shown in Figs. 12a and b, a TIVA spot is  observed along the back edge of the capacitive plate  element.  Further analysis using the FIB did not  reveal a contact spot, but it did reveal the close  proximity between the capacitive plates when  actuated beyond their snap-in voltage.  This tight  tolerance in Fig. 13 is in the area of the TIVA signal.  The arrow indicates where we believe contact  occurred.  FIB analysis showed less than 100 nm of  space between the capacitive plates when the device  was actuated with voltages greater than its snap-in  voltage.  We believe these micromirrors failed due to  contact of the capacitive plates shorting out the  device.  Although the short site could not be  identified, we believe contact occurred based on the  tight tolerance and over voltage stress test.  The


Fig. 9.  a) Reflected light and b) TIVA images revealing a  damaged spring and the location of the short.


Fig. 10.  FIB cross-section of the failed region shown in  Fig. 10b.  The suspension spring is in direct contact with  the power line directly underneath.


1.5 µm


Fig. 11.  SEM image of a mirror failed in the pop-up or  actuated position.


10 µm


Adhered side


increase in actuation voltage pulled the mirror closer  to the bottom electrode by bending the compliant  feet.  Flexure of these feet likely caused the back  edge of the mirror capacitive plate to contact the  biased capacitive plate resulting in the short.  FIB  processing of the failure area may have resulted in  releasing or cutting through the failure site.  The  voltages required to induce failure by this mechanism  can be very close to the snap-in voltage and are a  significant reliability concern.


Electrical testing caused micromirrors to fail in one  of two manners:  pull down of the suspension spring  to the poly 0 power line or contact of the poly 1


capacitive plate to the powered poly 0 capacitive  plate.  Both failure modes result in electrical shorting, rendering the device inoperable and stuck in either  the as-fabricated or pop-up position.  The voltages at  which these failure mechanisms can occur overlap, so  no trend determining the possibility of one failure  mechanism occurring over another can be  determined.


Micromirrors that failed due to spring contact with  the poly 0 power line were redesigned to eliminate  contact.  The power line was re-routed underneath a  different region of the mirror where no suspension  springs were present.  This resulted in a different  configuration of the micromirror array but eliminated  the spring contact failure mechanism.


Micromirrors that failed due to capacitive plate  shorting were redesigned to mitigate contact at  voltages slightly greater than the actuation voltage.  The space between the capacitive plates has been  increased when the device is fully actuated.  This  resulted in a larger ∆V between the snap-in voltage  and the short voltage.


Failure analysis results helped improve the overall  reliability and functionality of micromirrors failing  from electrical shorts.  Current failure mechanisms  were mitigated and new micromirrors were fabricated  that are more robust to electrical overstress.


The authors of this paper would like to thank the  microelectronics development laboratory staff for  their processing efforts, Sam Candelaria for testing  these parts and Alex Pimentel for his FIB work.  Special thanks goes to Richard Anderson and Daniel  Barton for reviewing this manuscript.  Sandia is a


Fig. 12.  a) Reflected light and b) TIVA images revealing  a short along the back portion of the capacitive plate pair.


Fig. 13.  FIB cross-section of the capacitive plate pair  believed to be the failure site indicated using TIVA.  FIB  analysis did not reveal a contact sight but did reveal a very  tight gap between the electrode pair when tilted.


1 µm


multiprogram laboratory operated by Sandia  Corporation, a Lockheed Martin Company, for the  United States Department of Energy under Contract  DE-AC04-94AL95000.  This work was funded under  CRADA SC98/1536 between NASA and Sandia  National Laboratories.


1. R. M. Boysel, T. G. McDonald, G. A. Magel, G. C. Smith, and J. L. Leonard, “Integration of  Deformable Mirror Devices with Optical Fibers  and Waveguides”, Proc. of SPIE, Vol. 1793 (1992), pp. 34-39.


2. http://www.dlp.com


3 S. J. Walker, D. J. Nagel, Report on “Optics & MEMS,” Naval Research Laboratories, Materials  Science and Technology Division, May 15, 1999


4. S. Arney, V. A. Aksyuk, D. J. Bishop, C. A. Bolle, R. E. Frahm, A. Gasparyan, C. R. Giles, S. Goyal, Fl pardo, H. R. Shea, M. T. Lin, and C. D. White, “Design Reliability of  MEMS/MOEMS


for


Lightwave  Telecommunications, Proc. from the 27th  ISTFA, Nov. 2001, pp. 345-348.


5. http://www.lucent.com


6. H. S. Stockman, editor, The Next Generation  Space Telescope, Space Telescope Science  Institute, Report # NP-1997(05)-016-GSFC/STScI M-9701, June 1997.


7. E. J. Garcia, M. A. Polosky, G. E. Sleefe, “Silicon Micromirrors and their Prospective  Application in the Next Generation Space  Telescope,” Proc. of SPIE 47th Photonic  Devices and Algorithms for Computing IV, July 2002, pp 1-15.


8. www.mems.sandia.gov


9. E. J. Garcia, “Pivoting micromirror designs for  large orientation angles,” Proc. of SPIE, Vol. 4178 Oct. 2000, pp. 126-136.


10. J. A. Walraven, E. I. Cole Jr., and P. Tangyunyong, “Failure Analysis of MEMS  Using Thermally-Induced Voltage Alteration”, Proc. from the 26th ISTFA Nov. 2000, pp. 489-496.


Cary Davis, Wes Mahin, and Becky Holdford.


Texas Instruments, Inc., 12500 TI Blvd, Dallas TX USA,


and Texas Instruments, Inc., 13536 N. Central Expwy, Dallas, TX USA


The Digital Micromirror Device (DMD) is a spatial


light modulation Micro-Optical Electro-Mechanical  Systems (MOEMS) device used in tabletop projectors, televisions and cinema projection systems.  This  device creates high resolution, high quality images


by deflecting/modulating light with microscopic  mirrors.  Failure analysis of these devices requires  superstructure, package, optics, and substructure  approaches. Particles within the active array of a  DMD are often killer defects, but those are the


subjects of an entire discussion of their own. This  paper will show evidence of failures associated with: windows in the package lids, failures of the  superstructure area, and failures within the  substructure.   Methods for removal of the mirrors,


as well as other structures, will be covered in greater  detail.  We will conclude with examples of analysis  areas in DMD devices that show how they differ from  other types of devices.


Dr. Larry Hornbeck of Texas Instruments invented  the DMD in the late 80’s.  The DMD has been  commercially available since 1995. (1)  Analysis of


the DMD has been taking place since Dr. Hornbeck  first tried to build one.  All DMD devices share a  basic architecture: a metal-ceramic package, a glass  window in the metal lid, the mirrors and their  supporting superstructure, and the addressing


substructure, which deflects the mirrors by  electrostatic forces.


The Substructure


The most understood part of DMD failure analysis is  the substructure analysis.  This analysis is much  like the analysis of any Static Random Access


Memory (SRAM), and this device is not a large one in  terms of storage size.  If we are analyzing a device of


approximately 800 pixels by 600 pixels, or SVGA, we


are only using a memory of about 480 Kbits.   Even a  device of XGA or SXGA size would only require  memory of 786 Kbits or at best just over 2 Mbits.  These are extremely small memory sizes in Y2002


standards. Standard memory analysis methods, except for the differences in memory mapping, may  be used to find the types of failure mechanisms that  occur in the substructure.  The most obvious  difference between the DMD and any other memory


is the method of output.  Standard SRAM sends bits  on I/O pins, where the DMD deflects a mirror to  several states.


The Package


The package part of DMD analysis requires  understanding of multilayer ceramic packages, interconnects, thermal effects on the superstructure  that are created by package changes, and


package/window interfaces.  Packages must be rigid  to prevent optical problems, thermally stable, and  capable of containing an atmosphere that must be  maintained to ensure proper functionality.  If the  internal atmosphere is allowed to equalize with


external environment, the unit life will be shortened.  Glass to metal seals are a somewhat understood  science, and ceramic packaging has been used for a  number of years in commercial as well as military  devices, but using both for an optical electronic


device requires a slightly different approach.  An  optical quality window ensures that the light from  the light source is neither lost nor changed in its  path by the glass.  Optical coatings are used to


reduce losses and reflections from the glass.  Any  material lodged within or stuck to the coating is an  opportunity for light loss or even a shadow of that  particle in the image.  Figure 1 shows just such  trapped carbon-based material that caused the final


image to be less than acceptable.  As light travels  through the window, a shadow of the material is cast


upon the surface of the mirrors.  This shadow is also  transmitted back to the window in reflection, and  therefore is a problem in at least two occurrences.  If


the window is observed using a directional light  source that is approaching the unit at an angle  similar to that used in the actual application, a pair  of dark or bright spots will be observed.


Figure 1. Carbon material which has dried on the


surface of the window.


The window must be removed mechanically before  further analysis is possible within the device.  This is  accomplished using methods dependent upon the  type package used.  Grinding through seam welds is


the most common method.  Extreme care must be  taken to prevent grinding into the operational cavity, as this will distribute metal particles freely  throughout that cavity and cloud the analysis.


The Superstructure


The superstructure required to build a DMD is a 3-D  array of metal and hollow space.  Fig. 2 shows this  as seen from an extreme viewing angle.


Figure 2.  Typical pixel as seen from extreme viewing  angle.


Failure analysis of this area requires a delicate  touch, both mechanically and electrically. A few


common analysis tools are needed when  deprocessing and analyzing the DMD. A variable


voltage (1 kV –25 kV) scanning electron microscope (SEM), a focused ion beam (FIB) tool, microscopy  with X-Y stages for locating areas within a few


microns, and laser cutting/marking tools help us  image and dissect the device.  The SEM may be one  of the most used tools discussed here.  A SEM is a  requirement mostly due to the three dimensional  nature of the DMD.  It is important to be able to


focus on the device surface metallization, the beam  or yoke structure, and the mirror structure all at the  same time.  The large depth of focus of the SEM  makes this possible.  If extreme tilt angles are


We would like to acknowledge the editorial


assistance and image captures provided by K. Harrison, C. Arroyo, J. Drummond, and R. Bickford  of the Dallas Device Analysis Operation.


(1) L.J. Hornbeck, “Digital Light Processing tm  and MEMS: Timely convergence for a Bright Future”. Plenary Session, SPIE Micromachining and  Microfabrication ’95, Austin, Tx, October 24, 1995,


p.2.


(2) J.I.Goldstein, D.E. Newbury, P. Echlin, D.C.Joy, A.D. Romig, Jr., C.E.Lyman, C. Fiori, and


E. Lifshin, “Scanning Electron Microscopy and X-Ray  Microanalysis: a text for biologists, materials  scientists and geologists”, 2nd Edition, 1992, 1981. Pages 79-147.


Wavefront Coded Imaging Systems for MEMS Analysis


Daniel L. Barton*, Jeremy A. Walraven*, Edward R. Dowski Jr.**, Rainer Danz***, Andreas Faulstich***, and Bernd Faltermeier***


*Sandia National Laboratories  Albuquerque, NM  87185-1081 **CDM Optics, Inc.


4001 Discovery Dr., Suite 2110  Boulder, CO  80303


***Carl Zeiss


Königsallee 9-21


37081 Göttingen, Germany


A new imaging technique called Wavefront Coding allows real-time imaging of three-dimensional  structures over a very large depth.  Wavefront


Coding systems combine aspheric optics and signal  processing to achieve depth of fields ten or more  times greater than that possible with traditional  imaging systems.


Understanding the relationships between traditional  and modern imaging system design through


Wavefront Coding is very challenging.  In high  performance imaging systems nearly all aspects of  the system that could reduce image quality are  carefully controlled.  Modifying the optics and using  signal processing can increase the amount of image  information that can be recorded by microscopes.  For a number of applications this increase in  information can allow a single image to be used  where a number of images taken at different object  planes had been used before.


Having very large depth of field and real-time  imaging capability means that very deep structures  such as surface micromachined MEMS can be clearly  imaged with one image, greatly simplifying defect  and failure analysis.


In MEMS analysis, traditional optical  characterization is performed for defect inspection, particle contamination, mechanical displacement (x,


y, and z-axis), thin film deflection, and general  failure analysis.  In each case, traditional imaging  system performance is limited by depth of field and  requires more time for imaging (through multiple  focal planes).  Increased depth of focus improves  analysis capabilities by having each mechanical layer  in focus for easier defect analysis.  Other imaging  tools and techniques such as scanning electron  microscopy (SEM) and scanning optical microscopy (SOM) require longer times for analysis and risk  compromising the failure mode.  SEM analysis risks  actuating the device by creating electrostatic forces  from the electron beam.  Large depths of focus are  obtained, but the surface is permanently modified by  carbon deposition (carbon cracking).


Increased depth of focus compared to that obtainable  from a traditional imaging system is possible through  a combination of aspheric optics and signal  processing.  The aspheric optics modify the imaging  system in such a way that the resulting images are  very insensitive to misfocus effects over a broad  range.  These optics also form images with unusual  blurs.  Signal processing that is independent of the  object being imaged and the amount of misfocus is  used to produce sharp and clear final images.  In  practice, the aspheric optics are placed near the back  aperture of microscope optics.  The signal processing  can be performed at camera frame rates via software  or hardware processing.


Test Sample Fabrication


MEMS used in this experiment were fabricated using  the SUMMiT V™ (Sandia’s Ultra-planar MEMS


Multi-level Technology) process [1].  The SUMMiT  V™ process consists of 5 layers of polysilicon (poly).  The first layer (poly 0) acts as the electrical contact  providing voltage for electrostatic actuation (device  movement).  Poly 0 is separated from the substrate by  thermal oxide and nitride layers.  In many SUMMiT  V™ designs, poly 1 and poly 2 are processed to form  a laminate layer (poly 1&2).  This laminate is  separated from poly 0 with 2 µm of sacrificial silicon  dioxide (sacox).  Poly layers 3 and 4 are fabricated, each separated by a layer of sacrificial oxide.  The  final step of the fabrication process is removal of the  sacrificial oxide using a hydrofluoric (HF) acid bath.  The acid bath (release process) etches away the  sacrificial oxide, releasing the poly structure thereby  allowing the mechanical components to move.  The  SUMMiT V™ process has 12 µm between the top  poly 4 surface and the poly 0 surface.  An illustration  of the SUMMiT V™ is shown in figure 1.


Fig. 1.  SUMMiT IV™ process shows various layers of  structural polysilicon, sacrificial and nitride layers.


The Limits of Traditional Microscopy


In optical microscopy in the microelectronics  industry, the focus is typically on spatial resolution.  Little attention is paid to the depth of focus, as it is  understood that, in order to gain depth of field, spatial  resolution has to be sacrificed.  The most common  equation used to describe the spatial resolution of an  optical system is


Res =


where λ is the wavelength of light and NA is the  numerical aperture of the optical system.  The depth  of field is also related to λ and NA by


M


ne


NA n


Field


Depth


where n is the refractive index (typically 1.00 for air), M is the lateral magnification and e is the smallest  distance that can be measured in the image plane of  the optical microscope.


A comparison of (1) and (2) clearly indicates that as  the resolution of the optical microscope increases (through increases in numerical aperture), the depth  of field decreases and vice versa.  To illustrate this, using a wavelength of 500 nm and NA values of 0.95  and 0.70 the values of resolution and depth of focus  calculated from equations (1) and (2) are shown in  Table 1.  The values in of depth of field in Table 1  were calculated using the first term in equation (1) only as the second term is small in comparison.


Table 1.  Calculated resolution and depth of field for  various NA values with λ = 500 nm.


NA = 0.70 NA = 0.95


Resolution (µm)


0.436


0.321


Depth of Field (µm) 1.020


0.554


The data in Table 1 also illustrates the need for  extended depth of field.  Even with a 0.70 NA  objective, the depth of field is only about 1 micron.  This depth is very small in comparison to the  thickness of modern integrated circuit and MEMS  technologies requiring the use of multiple focus  points for inspection of a given field of view.  The  rationale for the development of extended depth of  field optical systems is to address this need either by  clever optical system design and post-processing of  images or by combinations of traditional optics and  real-time image processing.


Extended Depth of Field Solutions


Confocal Imaging


Confocal techniques have been used in microscopy  for many years to improve depth discrimination to  allow separation of information in the image based  on depth (or height).  Confocal microscope systems  are configured as shown in figure 2 where the pinhole  is placed in close proximity to the detector (for a  scanning laser microscope).  In confocal imaging, the  axial dimension of the light at the focal plane can be  written as


sin 2


αλ ≈


where λ is the wavelength of light, α is the  acceptance half angle of the objective, n is the index  of refraction of the medium, do is the pinhole  diameter, and M is the magnification of the confocal  lens [2].  It is clear that as the diameter of the pinhole  decreases, the amount of depth discrimination  increases.  In other words, the ability to select a thin  vertical slice of the sample from which image  information is collected improves with smaller  pinhole sizes.


To use this capability for extended depth of focus  imaging, image slices at different stage positions (moving the microscope stage up or down) must be  acquired.  These images are then combined into a  single, high depth of focus image [3].


Point source (object)


Collector Lens


Focal


Plane


Pinhole


Detector


Objective Lens


Information above or below focal plane Information at  focal plane


Fig. 2  Confocal imaging system layout.


An example image sequence taken with a scanning  laser microscope (λ = 543 nm) with the pinhole  aperture in place is shown in figure 3.  Images (a) through (c) demonstrate the ability of a confocal  system to limit depth of focus and receive image  information from a thin layer around the point of  focus.  Image (d) shows the line used to create the zscan in (e).  The z-scan in (e) gives a good indication  of the depth of the sample and the selectivity of the  confocal system.  The information in (e) was used to  setup the image collection sequence (ten images in  this case) to create the confocal extended depth of  focus image shown in figure 3, image (f).  Image (f) clearly demonstrates that confocal systems can create  very high quality EDF images.  The only  disadvantage when compared to other EDF  techniques is that the confocal method cannot be  done in real time or at video rates.  The images must  be acquired serially and post processed into the EDF  image.


Nipkow disk plus Chromat C


In order to achieve extended depth of focus in real  time, a unique combination of a Nipkow spinning  disk [2, 4, 5] and a chromatic lens has been  developed [6].  This technique color-codes that  information so that portions of the image that are on  top appear toward the blue end of the spectrum and  portions that are on the bottom are toward the red.  The chromatic lens in this system creates axial  chromatic errors.  As would be expected from a  chromatic lens, the information is spectrally  dispersed allowing the color-coded extended depth of  focus image to be created.  The improvement realized  in this system (for a 50x/0.90 NA objective) was a  factor of eight increase in depth of focus.  For a  50x/0.90 NA objective, an increase from 0.6 µm to


4.7 µm depth of focus was achieved [6].  Figure 4  shows a comparison between a conventional optical


system with a normal depth of focus and the  Nipkow/chromat system for color-coded EDF.


An example image taken with this system is shown in  figure 5 along with a conventional image.  Figure 5  clearly demonstrates the improvement in depth of  focus over conventional imaging along with the  addition of color to enhance visual recognition of  feature depth order.  This system is well suited to  microelectronic device technologies, especially  integrated circuits, as the depth of focus improvement  is comparable to the depth of the technologies being  imaged.


c a


Fig. 3.  Confocal imaging sequence with (a) image focused  on the upper most features (b) focused on the large gear  (c) focused on the substrate (d)confocal image showing  location of z-section (e) z-section image (f) final extended  depth of focus image (all images taken using a 50x/0.75NA  objective).


Wavefront Coding


Wavefront Coding has been studied extensively but  has only recently become available to the  microsystems industry [7 - 11].  While the  application is fairly straightforward, the physics  behind the technology is fairly intricate and beyond  the scope of this paper.  Interested readers should  refer to the references in this section for more details


on Wavefront Coding theory.


DOF


Field of View


EDOF


Field of View(Spinning


Nipkow Disk)


Objective + Chromat C


Conventional  Brightfield


Confocal Scan Mode


Fig. 4. Optical layout comparing conventional (top) and  Nipkow/Chromat (bottom) extended depth of focus system.


DOF: 0.6 µm ( Apo 50 x / 0,9 )


EDOF: 4.7 µm


Chromat C


Fig. 5. Extended depth of focus using a Nipkow disk and a  chromatic lens.  Conventional image (left) and extended


depth of focus image (right).


The basic layout of a Wavefront Coded system is  shown in figure 6.  The addition of Wavefront


Coded extended depth of field (EDF) to a  conventional optical microscope only requires the  addition of an aspheric optical element or phase mask  be placed in the aperture stop above the objective  lens.  For best results, the phase mask must be  specifically designed for each objective lens and  designed for a specific level of EDF.  Imaging is  done through a video camera placed on the  microscope’s camera port.  Each video frame must be  processed using a kernel designed to recover the EDF  image from the raw optical information.


The most important element in this optical system is  the phase mask.  The phase mask is designed to  create an optical system that is invariant to focus.  The greater the degree of invariance, the greater the  depth of focus in the resulting image.  It was found  that a family of cubic phase pupil (CPP) functions


could be used to create this focus invariant optical  system [10].  The general formula for a CPP is given  by:


3 y


y


= α


where x and y are the coordinates in the plane of the  phase mask.  The value of α is given by the formula


πξ


where ξ is the total optical path difference introduced  by the phase mask and λ is the wavelength of light  being used.


Wavefront Coded  optical element


Digital signal   processing applied  to sampled image


Final  Image


Digital detector


Fig. 6. Wavefront Coded optical system diagram.


The general shape of the phase mask can be  visualized by setting α = 1 and plotting P(x,y) for x  and y values from –1 to +1.  The resulting surface is  shown in figure 7.


Fig. 7. Cubic phase mask used for Wavefront Coding.


It can be shown that image information in a single


frame is maximized with Wavefront Coding systems by capturing image information from a much  larger object volume than is possible with traditional  imaging systems.  Figure 8 shows a ray diagram  representation for a traditional imaging system along  the image plane.  A comparison of figure 8 with the


same system response for a Wavefront Coded imaging system (shown in figure 9) along the same  image plane shows the differences in image  information passed through the system.  In a  conventional optical system the focal point  corresponds to a single focal plane on the device.  This requires multiple images to be taken at every  structural level to obtain the required information.


49


49.5


50.5


mm


-0.1-0.05 0


0.05


Image plane location Image plane location


Fig. 8.  Ray diagrams for a traditional imaging system.


Wavefront Code  Imagin System


Fig. 9.  Ray diagram for a Wavefront Coded imaging  system.


The performance of optical systems is typically  quantified by analyzing the modulation transfer  function (MTF).  The MTF is a measure of the  microscope’s ability to transfer information (contrast  in the image) from the specimen to the intermediate  image plane.  Figure 10 shows the MTF information  from a traditional optical system at various amounts  of defocus in comparison to a Wavefront Coded


system before and after digital filtering.  In MTF  plots, better optical systems will have a greater  magnitude over a higher spatial frequency range.  The arrow from the “traditional system” label in  figure 10 identifies the traditional system response at  best focus.  The other traces for the traditional system  at increasing amounts of defocus approach zero  amplitude at low spatial frequencies.  The Wavefront  Coded system before filtering gives a similar  response to the defocused traditional system but the  response is invariant with focus.  The Wavefront


Coded system after digital filtering is also shown in  figure 10 where it shows a similar response to the  traditional system over a wide range of focus.  The


conclusion from figure 10 is that Wavefront Coding can produce images with greatly extended depth of  focus without loss in image quality.


0.9 1


Spatial frequency in lp/mm


Traditional System


Wavefront Coded® System


before filtering


Wavefront Coded® System  after filtering


Fig. 10. Modulation transfer function comparison between


a traditional optical system and a Wavefront Coded system.


Imaging fundamental objects, such as a point of light,


can be used to demonstrate how Wavefront Coding systems work.  An example is shown in figure 11.  A  traditional imaging system images a well focused  point of light and produces a clear image, as shown in  figure 11, image (A).   When the point of light is far  from the best-focused object plane the formed image  is not sharp and clear as seen in (B).  Numerous nonideal effects besides misfocus cause the out of focus  traditional image to be badly blurred. After  modifying the imaging system with a Wavefront


Coding aspheric optic, the in and out-of-focus  images (C) and (D) result.  Notice that there is very  little change in these two images with misfocus.  Since these images are not the same as the traditional  in-focus image, signal processing is needed.  The  signal processing acts to remove the specialized  image blur caused by the aspheric optics.  Since this  specialized blur is constant for a large range of  misfocus the signal processing is independent of the  amount of misfocus.  After signal processing, the  images of the point objects ((E) and (F)) are very  similar to that of the traditional in-focus image while  also being very insensitive to misfocus.


Analysis of an unreleased circular test structure  shown in figure 12 illustrates the difference in


conventional optical imaging vs. Wavefront Coded imaging.  All the levels of this test structure are in  focus at the same time.


In-focus


Out-of-focus


Fig. 11.  Imaging of point objects. Traditional images of  well-focused point objects form clear images (A).  When  the point object is far from the best-focus object plane a


blurred image results (B).  With Wavefront Coding, the  image of a point before signal processing has a nontraditional profile that is insensitive to misfocus (C and D).  After misfocus-independent signal processing, the final  image of the point is essentially the same as the in-focus, traditional image while also being independent of focus (E  and F).  All images have the same scale.


Fig. 12.  Traditional optical image of a circular test  structure focused on the bottom (poly 0) of the device


(right).  Wavefront Coding optical image of the same test  structure (left).  Note the depth of focus ranging from the


bottom of the device up to the top of the connecting joint  linkage arms ~12 µm above the surface.


To test the application of Wavefront Coding to the  analysis needs of MEMS devices, a number of  experiments were performed on a variety of samples.  The unique aspects of MEMS are the depth of the  structures and their lateral dimensions. The depth of  most structures posed little challenge for the


Wavefront Coding system.  There were situations  where features that move out of plane (pop up  mirrors, for example) stressed the technique.


Bond wires


For the first example, a relatively common but  difficult to image sample was chosen.  In order to  image a simple bond wire using a normal optical  microscope, a large amount of re-focusing is needed  because of the large vertical distance that the wire  travels through between the bond pad on the die and  the corresponding location on the package.  Typically, bond wire inspection is carried out under  low magnification microscopes that have a large  enough depth of field to inspect the wires at a single  point of focus.


Figure 13 shows an example image of a bond wire  taken using a 20x objective with and without the


benefit of Wavefront Coded EDF.  A quick  comparison of the two images in Figure 13 reveals  some very strong differences.  The non-EDF image  on the right shows the typical image quality obtained  with a traditional high magnification optical  microscope.  In the right image in figure 13, the  depth of focus is so small in comparison with the  vertical dimensions of the bond wire that even the top  of the bond area is out of focus when the point of  focus is set to the bond pad.  The EDF image on the  left in figure 13 shows almost scanning electron  microscope-like image quality.  The entire bond from  the bond pad to the wire at the edge of the field of  view is in focus.  There is also a strong 3-D effect on  the wire created by the intensity variations of  reflected light and the cylindrical wire with a shiny  surface.  This effect (which will also affect image  contrast in MEMS mirrors) is present on all surfaces  where the illumination source is reflected away from  the microscope objective.


Fig. 13.  Traditional microscope image taken with a 20x  objective (right).  Wavefront Coded image taken with the  same objective (left).


Pop-up mirrors


Mirrors have become very popular MEMS features  and, as they are reflective by design, pose significant  challenges for optical microscope systems.  As most  microscopes rely on light that is normal to the surface  for illumination, areas that reflect light away from the  objective lens create strong contrast differences that  allow quick ‘good’ versus ‘bad’ comparisons.  For  example, a mirror at an odd angle is easy to detect in  an array of mirrors that are at a common angle as it  will either appear bright or dark in comparison to  other mirrors.  The example in figure 14 illustrates  some of this effect.  This sample is a single pop-up  mirror that, as fabricated, had an equilibrium position  that left the mirror at about a 30-degree angle instead  of being flat.  Images (a) and (b) are typical images  taken using a 50x/0.90 NA objective.  Image (a) is  focused on the hinges while (b) is focused on the  mirror surface near the hinge.  The angle of the  mirror in this example required the addition of an  annular illumination source to achieve uniform  illumination.  Image (c) in figure 14 shows the


corresponding Wavefront Coded EDF image.  Image (c) demonstrates both the depth of focus  capability and the tolerance for illumination of this  technology.


Fig. 14. Images of an out of plane, pop-up mirror: (a) focused on the hinges without EDF, (b) focused on the


mirrors without EDF, and  (c) final EDF image.  All images  taken using a 50x/0.90 NA objective.


Samples at High Tilt Angles


This application described in the previous section of  imaging a tilted mirror brings up the question of  using a tilt stage under an optical microscope for  inspection of samples at significant tilt angles.  Inspection of MEMS devices that have features that  cannot be imaged from the top could be done if the  optical system would allow the sample to be tilted.  The example shown in figure 15 demonstrates this  capability.  This MEMS gear train was tilted to about  a 45-degree angle and imaged with and without the  EDF system.  Image (a) in figure 15 shows that  without EDF, the image is difficult to use and  requires inspection at multiple positions to observe  the full sample area.  Images (b) and (c) in figure 15


show Wavefront Coded EDF images using two  different phase masks.  The image in (b) was taken  with a modest phase mask that extended the depth of  focus but did not increase it sufficiently to keep the  entire field of view in focus.  In image (c), the phase  mask was changed to one that more appropriate for  the sample conditions.  The disadvantage of using the   stronger phase mask is the introduction of additional  noise.  A comparison of images (b) and (c) in figure  15 shows a modest increase in noise.  The noise can  easily be compensated for with additional digital  filtering.  The bottom line is to only a strong enough  phase mask to achieve the desired depth of field.


Fig. 15. Images of MEMS gears: (a) tilted gears imaged  with a 20x objective without EDF, (b) tilted gears imaged


with a modest phase mask (c) tilted gears imaged with a  stronger phase mask.  The large gears in the image are 500 µm in diameter.


Polysilicon Cantilever Beams


In this example, the effect of the EDF system on a  MEMS test structure that was unexpectedly out of  plane was evaluated.  The image sequence in figure  16, images (a) – (e) show the focus sequence needed  to image the complete depth of the sample.  The  waferfront coded EDF image (f) has all features in  sharp focus in a single image.


MEMS Gears


The final example is a MEMS gear sample taken at  normal incidence.  Images (a) through (d) in figure  17 show the through focus image sequence needed to  inspect the entire structure.  Image (e) in figure 17  accomplishes the same task in a single image using


the Wavefront Coded EDF technology.  For active  MEMS samples, the use of the real-time (video rate) capability of this EDF technology enhances the  ability to image multi-layer structures in motion  without the need to limit the observation to a  relatively small depth, i.e. with the entire structure in  focus, all aspects of the motion of the system can be  studied.


Fig. 16. MEMS test structure images at various points of  focus (a) – (e) without EDF and (f) with EDF (all images  taken with a 50x/0.90 NA objective).


In this paper, the theory and application of extended  depth of focus technology for optical microscopy  have been reviewed.  The competing technologies of


confocal, Nipkow/chromat, and Wavefront Coding for extended depth of focus have been compared both  for their operation characteristics and their flexibility.  While the confocal systems can achieve extended  depth of focus results that can be easily tailored to the  sample being imaged, the process of selecting the  parameters and collecting the image depth slices can  be time consuming and requires post processing of a  large number of images.  This technology, while very  powerful, does not lend itself to volume inspection of  samples because it cannot be done at video rates.  The unique Nipkow/chromat system also works very


well and does provide a real time EDF imaging tool.  The difficulty with this technology is that the system  must be designed to chromatically separate  information from a pre-specified depth range.  This  process, while adding color to a real-time EDF  technique, is best suited to applications with a known  depth requirement.


Fig. 17. MEMS gear sample with traditional brightfield  images at various points of focus in (a) – (d) and the  corresponding EDF image in (e).  All images were taken  with a 50x/0.90 NA objective.


Wavefront Coded EDF was introduced in theory  and studied through examples.  This method has  demonstrated a great potential for applications to  planar and non-planar samples and for imaging  samples at high tilt angles.  Through this study, the  need for additions such as oblique illumination  sources for surfaces at large angles with respect to the  normal optical axis was identified and tested.  Overall, the application of the powerful capabilities


of Wavefront Coded EDF to microelectronics and  MEMS technologies is just beginning to be realized.  In the near future, expect to see optical microscopes  with stages that can be tilted, objectives that have  small diameter cases to allow large sample angles, and annular illuminators to properly illuminate  samples with severe topography and reflective  surfaces.  On the image processing end, expect to see  very fast algorithms that can greatly exceed video  rate imaging and finely tunable noise filters to yield  perfect, diffraction limited EDF images.  Finally, the  development of a variable phase mask will create a  system where the depth of focus can be dialed-in to  the application in a process very similar to tuning the


parameters on a scanning electron microscope to  meet the needs of the sample.


Wavefront Coding and Wavefront Coded are  registered trademarks of CDM Optics, Inc.   SUMMiT V™ is a registered trademark of Sandia  National Laboratories.  The authors of this paper  would like to thank the microelectronics development  laboratory staff for their processing efforts.  Sandia is  a multiprogram laboratory operated by Sandia  Corporation, a Lockheed Martin Company, for the  United States Department of Energy under Contract  DE-AC04-94AL95000.


1. www.mems.sandia.gov


2. S. Yin, G. Lu, J. Zhang, F. T. S. Yu, and J. N. Mait, “Kinoform-based Nipkow disk for a  confocal microscope,” Applied Optics, vol. 34, no. 25, 1 September 1995.


3. T. R. Corle, C. –H. Chou, and G. S. Kino, “Depth response of confocal optical  microscopes,”} Optics Letters, vol. 11, no. 12, December 1986.


4. D. T. Fewer, S. J. Hewlett, and E. M. McCabe, “Laser sources in direct-view-scanning, tandemscanning, or Nipkow-disk-scanning confocal  microscopy,” Applied Optics, vol. 37, no. 2, 10  January 1998.


5. T. Tanaami, S. Otsuki, N. Tomosada, Y. Kosugi, M. Shimizu, and H. Ishida,  “High-speed 1-frame/ms scanning confocal microscope with a  microlens and Nipkow disks,” Applied Optics, vol. 41, no. 22, 1 August 2002.


6. Zeiss Axiotron product literature.


7. E. R. Dowski Jr., R. H. Cormack, and C. D. Sarama, “Wavefront coding:  jointly optimized  optical and digital imaging systems,” SPIE  Aerosense Conference, April (2000).


8. G. E. Johnson, E. R. Dowski, Jr., and W. T. Cathey, “Passive ranging through wave-front  coding: information and applications,” Applied  Optics, vol. 39, no. 11, 10 April 2000.


9. E. R. Dowski, Jr., and W. T. Cathey, “Extended  depth of field through wave-front coding,” Applied Optics, vol. 34, no. 11, 10 April 1995.


10. S. Bradburn, W. T. Cathey and E. R. Dowski, Jr., “Realizations of focus invariance in opticaldigital systems with wave-front coding,” Applied  Optics, vol. 36, no. 35, 10 December 1997.


11. S. C. Tucker, W. T. Cathey, and E. R. Dowski, Jr., “Extended depth of field and aberration  control for inexpensive digital microscope  systems,” Optics Express, vol. 4, no. 11, 24 May


1999.


required to see beneath a mirror, care must be taken  to remove all ferrous materials  (e. g., the lid weld  ring) as the residual fields in these materials might  interfere with the electron beam.  If an extreme angle  image is needed of a mirror in the center of the active


array, the adjacent mirror or mirrors must also be  removed either by probe or minimal laser  application.


Low accelerating voltage, approximately 1KeV, in the


SEM allows us a topographical view of the mirrors, yokes, or metallizations.  Higher values of Vacc in the  range of 20 to 25 KeV also yield useful information  due to the construction of the DMD and the  phenomenon of beam penetration.


Figure 3. Beam interaction volume as seen in High  Acceleration Imaging.


The electron beam interacts with the materials of the  DMD, causing secondary electrons to be given off.  This makes the image of the surface.  The interaction


volume or depth of penetration is dependent on the  Vacc and the material being imaged. (2).  Most of the


material in the DMD superstructure is the same type  and thickness, so the interaction volume is  dependent only on Vacc.  So by increasing the Vacc, imaging of materials below the physical surface of  the mirrors, such as particles, can be performed.  This is known as High Acceleration Imaging.  See  Fig. 3.  This technique can allow confirmation of a  fail site before mirror removal, as shown in Fig. 5.


Removal of the mirrors can be carried out by several  methods, but the most common method is exquisite  in its simplicity.  Common transparent adhesive tape  is applied carefully to the surface of the mirrors with


a light amount of pressure, then removed in one  motion.  With the tape come the mirrors, breaking  the hinges in the process.  The view of the  substructure surface is now unobstructed, and on  the tape we removed are all of the mirrors and yokes


available for inspection in an inverted position as in  Figure 4.


Figure 4. Tape after mirror removal.


This image shows the entire area of mirrors removed  using the tape, and an expanded view of a single  yoke/mirror assembly.  This is the view offered by  inspecting the rear of the mirrors, usually with a low


accelerating voltage in a Field Emission SEM.


Figure 5. View of material trapped behind the mirror  imaged using High Acceleration Imaging.


This allows us to inspect the lower surfaces of both  the yokes and mirrors.  If reasonable care is taken, no damage of the substructure surface is observed.


Removal of only the mirrors without damaging the  yokes requires a bit more finesse, and also an  isotropic dry etch.  While this is still a global  approach much like the transparent tape method, it  will fold the mirrors and leave the yoke assembly


available for inspection and analysis. This approach  is seen in Figure 6. Similar results are obtainable  using a laser-cutting tool for removing one or more  mirrors.  There is some variation in laser power


between units, and therefore each setup must be  worked with to obtain the optimum power and spot  size for single pulse laser mirror removal.


Figure 6. Mirror reduced using RIE isotropic etch.


This variance will determine whether we remove  mirrors, mirrors and yokes, or everything down to


the surface metallization.


The Difference


We have said that the substructure is essentially an  SRAM device that may be treated as if it were any  other SRAM.  That is true in much of the analysis of  the DMD, but some of the more common methods of  handling a device during analysis will create


problems when attempting them on a DMD with its  mirror superstructure still attached.  While  compressed air or nitrogen may be used in “normal” analyses to clean the surface of the unit, it would not


be recommended in DMD analysis.  Air pressure as  low as 15psig from a sprayer will remove all of the  mirror structure from a device in about 2 seconds, while causing multiple collisions across the surface  of the device.  Liquids that are commonly used for


cleaning the surfaces of semiconductor devices  during analysis cannot be used on the DMD


superstructure.  The capillary action between the  liquid and the mirror structures will break the  hinges and the mirrors will float around and


redeposit in an almost random manner.  While this  might seem to be a useful method for deprocessing  the unit, it leaves the analyst with a surface of  stacked or layered mirrors and yokes, with no idea of  where they originated.  Not all the differences are


negatives.  When a DMD is built with a window that  allows for optical observation of the peripheral I/O  driver circuits, one can perform emission microscopy  on these circuits without delidding the unit.


Electrostatic Discharge (ESD) protection circuits  have been imaged on devices without so much as a  scratch to the failed unit.  With no deconstruction of  the devices, there remains the possibility of retest or  further analysis at a future time.


The Future


Future analyses of DMD units may require more


sophisticated tools and different methods of  inspection.  Present studies include the use of such  tools as the SQUID (Superconducting Quantum  Interference Device) to determine current paths  without physically touching the unit, and the use of


electron beam probing tools to determine the nature  of the switching pulse train within the mirrors once  again without physically touching them.  Almost any  physical contact of the mirrors could very likely  destroy those mirrors and the structures beneath


them


The physical analysis of the Digital Micromirror  Device is a mix of different analysis techniques.  Observation of the substructure is performed using  presently available tools such as emission  microscopy, functional test equipment, optical


microscopy, and SEM/FIB.  Observation of the  superstructure may be performed using these same  tools, but also requires a 3-D thought process, as  well as transparent adhesive tape.  Taking care to


maintain superstructure integrity will allow for use  of High Acceleration Imaging as well as low energy  surface topographic imaging.

