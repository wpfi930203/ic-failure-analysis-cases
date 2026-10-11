---
title: "ISTFA-1999.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_45a2dbe6249a1088dcd3e181af3f70507295230462135641
file_size: 61467077
---

T. Ohnishi, H. Koike, S. Tomimatsu, K. Umemura, T. Kamino, Hitachi, Ltd., Hitachinaka, Ibaraki, Japan


Session 15: Backside Analysis


A Combined Infrared/Visible Photoemission Microscope ..................................................................457


A. Trigg, Institute of Microelectronics, Singapore


Correlation of Electronic and Thermal Properties of Short Channel nMOSFETS ............................465


M. Palaniappan, V. Ng, R. Heiderhoff, J. C. H. Phang, National University of Singapore, Singapore;G. B. M. Fiege, L. J. Balk, Universität Wuppertal, Wuppertal, Germany


Application of the Infrared Microscope (IREM1) for Flip - Chip (C4) Failure Analysis.....................471


A. N. Zaplatin, Intel Corporation, Folsom, California; F. J. Low, Infrared Laboratories Inc., Tucson,Arizona; S. Seidel, V. R. Rao, T. H. Loh, Intel Corp., Santa Clara, California


ISTFA ’99


Proceedings of the


25th International Symposium for


Testing and Failure Analysis


14-18 November 1999


Westin Hotel


Santa Clara, California


Sponsored by


Published by


ASM International


Materials Park, Ohio 44073-0002


Copyright © 1999


by


ASM International®


All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any means,electronic, mechanical, photocopying, recording, or otherwise, without the written permission of the copyright owner.


First printing, October 1999


Great care is taken in the compilation and production of this book, but it should be made clear that NO WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN CONNECTION WITH THIS PUBLICATION. Although this information is believed to be accurate by ASM, ASM cannot guarantee that favorable results will be obtained from the use of this publication alone. This publication is intended for use by persons having technical skill, at their sole discretion and risk. Since the conditions of product or material use are outside of ASM's control, ASM assumes no liability or obligation in connection with any use of this information. No claim of any kind, whether as to products or information in this publication, and whether or not based on negligence,shall be greater in amount than the purchase price of this product or publication in respect of which damages are claimed. THE REMEDY HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND SOLE REMEDY OF BUYER, AND IN NO EVENT SHALL EITHER PARTY BE LIABLE FOR SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES WHETHER OR NOT CAUSED BY OR RESULTING FROM THE NEGLIGENCE OF SUCH PARTY. As with any material, evaluation of the material under end-use conditions prior to specification is essential. Therefore, specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or reproduction,in connection with any method, process, apparatus, product, composition, or system, whether or not covered by letters patent, copyright, or trademark, and nothing contained in this book shall be construed as a defense against any alleged infringement of letters patent, copyright, or trademark, or as a defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


Library of Congress Catalog Card Number: 99-75503


ISBN: 0-87170-646-6


SAN: 204-7586


Materials Park, OH 44073-0002


Printed in the United States of America


iii


The photograph on the cover shows barrier metal which caused a short between two metal traces due to fabrication mask defect. Photograph is courtesy of Accurel Systems International, Sunnyvale, California


iv


The Organizers of the 1999 International Symposium on Testing and Failure Analysis would like to acknowledge and thank the following people for their assistance in editing this proceedings:


Richard E. Anderson


Sandia National Laboratories Albuquerque, New Mexico


Christian Boit


Infineon Semiconductors, AG Munich, Germany


Ann N. Campbell


James J. Erickson


Hughes Space and Communications Co.


El Segundo, California


Keenan L. Evans


ON Semiconductor Phoenix, Arizona


Steven Ferrier


SDG Analytic Inc.


Corvallis, Oregon


Leo G. Henry


ORYX Instruments Corp.


Fremont, California


Kultaransingh N. Hooghan


Lucent Technologies Allentown, Pennsylvania


Edward Keyes


Semiconductor Insights Kanata, Ontario, Canada


Steven J. Kirch


Intel Corporation


Kathy M. McCray


Diversified Technologies Resources Colorado Springs, Colorado


Gary M. Molle


Kaiser Electronics San Jose, California


Thomas M. Moore


Texas Instruments, Inc.


Dallas, Texas


James D. Plante


Adaptec, Inc.


Milpitas, California


H. Stan Silvus, Jr.


Southwest Research Institute San Antonio, Texas


Matt Thayer


Advanced Micro Devices Austin, Texas


Massimo Vanzi


Universita' di Cagliari Cagliari, Italy


Lawrence C. Wagner


Texas Instruments


Jane E. Wheeler


Surface Science Laboratories Mountain View, California


Vv


ISTFA ’99 Organizing Committee


|Sandra Delgado |Richard J. Ross |
|---|---|

|General Chair |Seminar Committee Chair |

|Accurel Systems International |IBM Corporation |

|Sunnyvale, California |Essex Junction, Vermont |

|Daniel L. Barton |Christian Boit |

|General Vice Chair |Seminar Committee Vice Cha |

|Sandia National Laboratories |Infineon Semiconductors, AG |

|Albuquerque, New Mexico |Munich, Germany |

|James B. Colvin |Anu Barman |

|Exposition Co-Chair |Audio Visual Chair |

|WSI |Lambda Advanced Analog |

|Fremont, California |Santa Clara, California |

|Catherine Renteria |Thomas M. Moore |

|Exposition Co-Chair |Publicity Chair |

|Compaq, Tandem Division |Texas Instruments, Inc. |

|Cupertino, California |Dallas, Texas |

ir


EDFAS 1999 Board of Directors


|Lawrence C. Wagner |Sandra Delgado |
|---|---|

|EDFAS President |EDFAS Member-At-Large |

|Texas Instruments |Accurel Systems International |

|Dallas, TX |Sunnyvale, CA |

|Edward I. Cole, Jr. |James J. Erickson |

|EDFAS Vice President |EDFAS Member-At-Large |

|Sandia National Laboratories |Hughes Space and Communications Co |

|Albuquerque, NM |El Segundo, CA |

|Gary F. Shade |Shekhar Khandekar |

|EDFAS Secretary |EDFAS Member-At-Large |

|Visteon Microelectronics |Level One Communications, Inc. |

|Colorado Springs, CO |Sacramento, CA |

|Daniel L. Barton |Richard J. Ross |

|EDFAS Member-At-Large |EDFAS Member-At-Large |

|Sandia National Laboratories |IBM Microelectronics Division |

|Albuquerque, NM |Essex Junction, VT |

|Christian Boit ||

|EDFAS Member-At-Large ||

|Infineon Technologies/FA ||

|Munich, Germany ||

.


vi


ISTFA ’99 Abstract Review Committee


|Advanced Techniques |FIB |
|---|---|

|Thomas M. Moore |Ann N. Campbell |

|Texas Instruments, Inc. |Sandia National Laboratories |

|Dallas, Texas |Albuquerque, New Mexico |

|Backside Analysis |Packaging |

|Dave Vallett |Kathy M. McCray |

|IBM Microelectronics Division |Diversified Technologies |

|Essex Junction, Vermont |Resources |

||Colorado Springs, Colorado |

|Case Histories I ||

|James Plante |New Subjects |

|Accurel Systems International |Jane E. Wheeler |

|Sunnyvale, California |Surface Science Laboratories Mountain View, California |

|Case Histories II ||

|Stan Silvus |Techniques |

|Southwest Research Institute |Ronald E. Pyle |

|San Antonio, Texas |Motorola SPS |

||Austin, Texas |

|Discretes |Discretes |

|Gary M. Molle |Gary M. Molle |

|Kaiser Electronics |Kaiser Electronics |

|San Jose, California |San Jose, California |

|ISTFA ’99 Other Committees |ISTFA ’99 Other Committees |
|---|---|

|Keynote Speaker Team |Massimo Vanzi |

|Sandra Delgado |Universita' di Cagliari |

|Accurel Systems International |Cagliari, Italy |

|Sunnyvale, California |Government Liason |

|Shekhar Khandekar |David Dylis |

|Level One Communications, Inc. |IIT Research Institute (IITRI) |

|Sacramento, California |Rome, New York |

|Seshu V. Pabbisetty |Publications Liaison |

|Texas Instruments Semiconductor Group |Vijay Chowdhury |

|Stafford, Texas |Altera Corp. |

||San Jose, California |

|International Liaisons ||

|Paolo Malberti |Panel Discussion Moderato |

|Swiss Federal Institute of Technology |Leo G. Henry |

|Zurich, Switzerland |ORYX Instruments Corp. |

||Fremont, California |

|Sumio Matsuda ||

|NASDA Tsukuba Space Center |Education Seminar Liaison |

|Ibaraki, Japan |Ann N. Campbell |

|Jacob Phang|Sandia National Laboratories |

|Jacob Phang |Albuquerque, New Mexico |

|The National University of Singapore ||

|Singapore ||

r


vii


1998 BEST PAPER AWARD


Micro-Raman Spectroscopy Evaluation of the Local Mechanical Stress in Shallow Trench Isolation CMOS Structures:


Correlation with Defect Generation and Diode Leakage


I. De Wolf, G. Groeseneken, H. E. Maes


IMEC


Leuven, Belgium


M. Bolt, K. Barla, A. Reader


Centre Commun Crolles, France


P. J. McNally


Dublin City University


Dublin, Ireland


1998 OUTSTANDING PAPER AWARD


The Challenges of Focused-Ion-Beam Chip Repair and Debug Assistance in the 0.25µm Copper Interconnect Millennium


S. B. Herschbein, L. S. Fischer, A. D. Shore, M. P. Tenney, T. L. Kane


IBM Analytical Services


Hopewell Junction, New York


Future ISTFA Dates


26th International Symposium for Testing and Failure Analysis


12-16 November 2000


Meydenbauer Convention Center Bellevue, Washington


Be sure to put this date on your calendar!


ix


First Announcement And


ISTFA 2000 • Call for Papers


26thInternational Symposium for Testing and Failure Analysis


Sponsored by The ASM Electronic Device Failure Analysis Society (EDFAS)


12-16 November 2000 • Meydenbauer Convention Center • Bellevue (Seattle), Washington USA


|ISTFA solicits original, previously unpublished papers on a wide range of Testing and Failure |ISTFA solicits original, previously unpublished papers on a wide range of Testing and Failure |
|---|---|

|Analysis topics of practical value to anyone working to detect, understand and eliminate electronic |Analysis topics of practical value to anyone working to detect, understand and eliminate electronic |

|device failures. Non-commercial papers from equipment vendors dealing with new or unique tools an methodologies, applications and results are welcome. Papers will be selected for inclusion in the technical program on the basis of appropriateness and quality of data, technical importance, novelty/originality, and interpretation of results. Paper acceptance is based entirely on the information included in the abstract. We are currently seeking papers on (but not limited to) the following relevant topics: |device failures. Non-commercial papers from equipment vendors dealing with new or unique tools an methodologies, applications and results are welcome. Papers will be selected for inclusion in the technical program on the basis of appropriateness and quality of data, technical importance, novelty/originality, and interpretation of results. Paper acceptance is based entirely on the information included in the abstract. We are currently seeking papers on (but not limited to) the following relevant topics: |

|• Advanced Fault Localization Techniques |• Defect Characterization Methods |

|• Device Processing and Deprocessing Methods |• Case Histories |

|• Discrete Component Failure Analysis |• Passive Component Failure Analysis |

|• Testing and Device Characterization |• Packaging Related Failures |

|• Backside and Flip-Chip Analysis Techniques |• Compound Semiconductor Devices |

|• Micro-Electro Mechanical Systems (MEMS) |• Signature Analysis |

d


ABSTRACT SUBMISSION GUIDELINES


Abstract Preparation:


1. Begin your abstract with the conference name, ISTFA 2000, followed by the title of your paper.


2. Type your abstract (two-page maximum) in English and include significant images, figures, references,


etc. All abstracts must adhere to the two-page maximum length to be considered.


3. At the end of your abstract, describe in 25 words or less, the significance of your work (conclusions


and benefits). Then list three (3) key words from your abstract that can be used for indexing in the


Conference Proceedings, and indicate to which topical area (from the list above) your abstract relates.


4. Provide the following information for the presenting author first, then for all co-authors of the work:


complete name (including Dr./Mr./Mrs./Ms./Prof. etc.), title, affiliation with complete mailing address


(no P. O. Box numbers), telephone and fax numbers, and e-mail address. This information must be


included with your abstract.


Abstract and Manuscript Deadlines:


1. Abstracts must be submitted by 1 MARCH 2000 to be considered for inclusion in the program.


2. A Conference Proceedings is planned for publication and distribution at the event. A full manuscript


must be submitted for review by 12 JUNE 2000, then in final camera-ready and electronic formats by


10 JULY 2000.


Abstract Submission Options:


• If your abstract contains images or figures, please e-mail it as a Microsoft Word file attachment to:


educatn@po.asm-intl.org. In the “Subject Line,” please enter ISTFA 2000.


• For a text-only abstract, the preferred method is to submit it via the EDFAS Website at


www.edfas.org/istfa and follow the instructions to submit your abstract online.


• If you absolutely cannot submit your abstract electronically, mail it to arrive before the deadline to:


ISTFA Conference Administrator, ASM International, Materials Park, Ohio 44073-0002 (telephone:


+440.338.5151).


Visit the EDFAS Website frequently at www.edfas.org for updates on this event.


xi


Preface


The twenty-fifth International Symposium for Testing and Failure Analysis is vastly different


from the first ISTFA. In those days failure analysis was fairly simple as were the devices.


Today, many advanced analytical tools and


techniques must be employed as the geometry has diminished and the technologies have become increasingly complicated by mixing


signals and employing more and more new materials.


This Failure Analysis symposium brings you the latest in techniques along with novel approaches to solving some unique and more common


problems. We have even added a Software session this year and will continue to add categories as methods and devices change


each year.


The new millennium will bring even more changes at a faster rate than we can imagine.


We rely on you, the Failure Analysts and Test engineers to develop and share new methodologies with your colleagues at our


annual Symposium and Seminar sessions.


Engineers from around the world participate each year to share their work and network with


each other. These are exciting times in the semiconductor/electronic industry and this years efforts reflect the newest ways to solve our ever


more challenging fabrication, assembly and packaging problems.


Thanks to everyone who contributed to this year’s symposium which took considerable effort to switch to electronic format for the symposium


presentations. I invite you to join again next year and encourage you to share your experience at a future symposium.


xiii


Table of Contents


Session 1: Advanced Techniques I


# Table of Contents


Terahertz Imaging: A New Technique for Inspection of Dielectric Materials........................................3


D. Mittleman, Rice University, Houston, Texas


Detecting Power Shorts From Front and Backside of IC Packages Using Scanning SQUID


Microscopy.................................................................................................................................................11


L. A. Knauss, B. M. Frazier, H. M. Christen, S. D. Silliman, K. S. Harshavardhan, Neocera, Inc.,Beltsville, Maryland; E. Fleet, F. C. Wellstood, University of Maryland, College Park, Maryland; M.


Mahanpour, A. Ghaemmaghami, Advanced Micro Devices, Sunnyvale, California


Session 2: Advanced Techniques II


Waveform Acquisition from the Backside of Silicon Using Electro-Optic Probing ...........................19


M. Bruce, G. Dabney, S. McBride, J. Mulig, V. Bruce, C. Bachand, Advanced Micro Devices, Inc.,Austin, Texas; S. Kasapi, J. Block, Schlumberger ATE, Austin, Texas


Optical Probing of VLSI ICs From the Silicon Backside .......................................................................27


T. Eiles, G. Woods, V. Rao, Intel Corporation, Santa Clara, California


Picosecond Imaging Circuit Analysis of the IBM G6 Microprocessor Cache.....................................35


M. McManus, P. Sanda, S. Steen, D. Knebel, D. Manzer, S. Polansky, IBM, Yorktown Heights, New York; B. Huott, S. Wilson, T. Pelella, Y. Chan, IBM, Poughkeepsie, New York


Electrical Probing and Surface Imaging of Deep Sub-Micron Integrated Circuits .............................39


K. R. Krieg, R. X. Qi, C. O. Lada, E. Dante, K. Choi, Micron Force Instruments, San Jose, California;D. J. Thomson, G. E. Bridges, University of Manitoba, Winnipeg, Manitoba, Canada


Session 3: Advanced Techniques III


Comparative TDR Analysis as a Packaging FA Tool.............................................................................49


C. Odegard, C. Lambert, Texas Instruments, Dallas, Texas


Light Emission Spectral Analysis: The Connection Between the Electric Field and the


Spectrum ....................................................................................................................................................57


D. L. Barton, P. Tangyunyong, J. M. Soden, C. L. Henderson, E. I. Cole, Jr., Sandia National Laboratories, Albuquerque, New Mexico; R. Danz, R Steiner, Carl Zeiss Inc., Jena, Germany;Z. Iwinski, Carl Zeiss Inc., Thornwood, New York


Temperature Profile Measurement and Failure Characterization of ESD Protection Devices Using


Spectroscopic Photon Emission Microscopy and Raman Spectroscopy...........................................69


M. S. Rasras, I. De Wolf, G. Groeseneken, J. Chen, K. Bock, H. E. Maes, IMEC vzw, Heverlee,


Belgium


Infrared Emission Spectroscopy as a Reliability Tool ..........................................................................77


Q. Kim, S. Kayali, Jet Propulsion Laboratory, Pasadena, California


xiv


Poster Session I - Advanced Techniques & Backside Analysis


Quantitative E-beam Probe for Valid High-Speed Measurements .......................................................87


C. T. Salling, Micron Technology, Richardson, Texas


Short High Voltage Stress for Design-to-Process Characterization....................................................97


B. Lisenker, D. Veinger, Y. Mitnick, Intel, Haifa, Israel


Automatic TEM Sample Preparation .....................................................................................................103


W. D. Kaplan, Technion-Israel Institute of Technology, Haifa, Israel; K. Kisslinger, R. Oviedo, National Semiconductor Corporation, South Portland, Maine; E. Raz, C. Smith, SELA USA Inc., Sunnyvale,


California


Failure Analysis of Sub-Micron Semiconductor Integrated Circuit Using Backside Photon


Emission Microscopy..............................................................................................................................109


S. Lim, J. H. Bi, L. C. Goh, S. P. Neo, S. Tatti, Chartered Semiconductor Manufacturing Ltd.,Singapore


Sample Preparation for Backside Failure Analysis Using Infrared Photoemission Microscopy....117


A. Trigg, Institute of Microelectronics, Singapore; P. Y. Loh, Ngee Ann Polytechnic, Singapore


Poster Session II - FIB and Case Histories


In-Situ Use of an Optical Microscope for FIB Microsurgery of Planarized Devices.........................127


P. J. Wolpert, R. A. Lee, FIB International, Santa Clara, California


Investigation on the Corrosion of Cu Metallization in the Focused Ion Beam System due to a


Low I2Background ..................................................................................................................................135


H. J. Bender, S. Jin, I. Vervoort, Y. Lantasov, IMEC, Leuven, Belgium


Tin Corrosion Induced by Corrosive De-Ionized (DI) Water................................................................141


S. Khandekar, L. Vedula, Level One Communications, Inc., Sacramento, California; V. Malshe,University Department of Chemical Technology, Matunga, Mumbai, India


Latch-Up Induced Slit Voiding in Aluminum Metal Lines....................................................................145


C. Zhang, L. Vedula, S. Khandekar, Level One Comuncations, Inc., Sacramento, California


Failure Analysis of Discolored Bondpads in Wafer Fabrication ........................................................149


Y. N. Hua, Chartered Semiconductor Mfg. Ltd., Singapore


Optimizing Contact Resistance at a Resistor/Conductor Interface via Thin Film Microanalysis and


Process Design of Experiments ............................................................................................................161


J. H. Linn, M. G. Shlepr, T. K. Thompson, Harris Semiconductor, Palm Bay, Florida


Session 4: Discretes I


Failure Analysis of Plastic Packaged GaAs and AlGaAs/GaAs LEDs ...............................................173


P. Mead, M. Burch, P. McCluskey, F. G. Johnson, University of Maryland, College Park, Maryland


A Technique for Measuring Device Temperature with High Accuracy in Accelerated Operational


Life Tests..................................................................................................................................................183


K. Takeda, M. Harigaya, Y. Miyazaki, NEC Corporation, Kawasaki, Kanagawa, Japan


Temperature Measurement on Micromachined IR Bolometers Using an Infrared Microscope......189


A. Trigg, U. Sridhar, Institute of Microelectronics, Singapore; H. S. Lee, G. Karunasiri, National University of Singapore


xv


Session 5: Software Tools


Automated Translation of Final Test Programs to Inexpensive FA Testers .....................................197


D. J. Bodoh, Motorola, Austin, Texas


FMECA Modeling - A New Approach.....................................................................................................203


Y. Bot, BQR Reliability Engineering Ltd., Rishon-Letsion, Israel


Session 6: Discretes II


Selective Au-Etching on Aged GaAs-Based Devices ..........................................................................211


M. Vanzi, A. Bonfiglio, P. Salaris, P. Deplano, E. F. Trogu, A. Serpe, Universita' di Cagliari, Cagliari,Italy; G. Salmini, R. De Palo, Milan, Italy


Nondestructive Detection of Cracks in Ceramics Using Vicinal Illumination...................................217


S. M. Hull, NASA Goddard Space Flight Center, Greenbelt, Maryland


Evacuated FM08 Fuses Carry a Sustained Arc in a Bus over 75 VDC...............................................225


H. Leidecker, NASA Goddard Space Flight Center, Greenbelt, Maryland; J. Slonaker, Unisys Corp.,Lanham, Maryland


Session 7: Techniques I


Advanced Statistical Tools for Improving Yield and Reliability .........................................................233


R. C. Kittler, Yield Dynamics, Inc., Santa Clara, California


An Application of Passive Voltage Contrast (PVC) to Failure Analysis of CMOS LSIs Using


Secondary Electron Collection ..............................................................................................................239


A. Nishikawa, N. I. Kato, Y. Kohno, N. Miura, ITES Co., Ltd., Shiga, Japan; M. Shimizu, IBM Japan Ltd., Shiga, Japan


Session 8: FIB I


Integrated Circuit Device Repair Using FIB System: Tips, Tricks, and Strategies...........................247


K. N. Hooghan, Lucent Technologies, Allentown, Pennsylvania; K. S. Wills, Texas Instruments,


Stafford, Texas; P. A. Rodriguez, Reactive Beam Technology Inc., Lewisville, Texas; S. J. O'Connell,Cyrix Corporation, Richardson, Texas


Modeling and Optimizing XeF2-enhancing FIB Milling of Silicon.......................................................255


N. J. Bassom, T. Mai, Micrion Corporation, Peabody, Massachusetts


Reliability Test Results for Pt FIB Interconnect Structures................................................................263


M. Zaragoza, Cadence Design Systems, Inc., San Diego, California


Focused Ion Beam Induced Effects on MOS Transistor Parameters ................................................273


A. N. Campbell, P. Tangyunyong, J. R. Jessing, C. E. Hembree, J. M. Soden, Sandia National


Laboratories, Albuquerque, New Mexico; N. Antoniou, Micrion Corporation, Peabody, Massachusetts;


W. E. Vanderlinde, Microelectronics Research Laboratory, Columbia, Maryland; M. T. Abramo, IBM Microelectronics, Essex Junction, Vermont


xvi


Session 9: Case Histories I


Relay Failures Specific to Space Applications ....................................................................................285


A. Teverovsky, Unisys, Lanham, Maryland


Failure Analysis of Autoclave-Stressed SRAMs with Aluminum Fuses............................................293


J. M. Moss, S. Subramanian, V. Soorholtz, M. Thomas, M. Gerber, Motorola, Austin, Texas; C. M.


Chan, Motorola, Kuala Lumpur, Malaysia


Electrostatic Discharge (ESD) Failures in Thin Film Resistors..........................................................297


Characterization of Gold Embrittlement in Solder Joints ...................................................................305


C. B. Bunis, AMP M/A-COM, Lowell, Massachusetts


Session 10: FIB II


In-Situ Dual Beam (FIBSEM) Techniques for Probe Pad Deposition And Dielectric Integrity


Inspection In 0.2µm Technology DRAM Single Cells ..........................................................................311


G. Zimmermann, R. Chapman, WhiteOak Semiconductors, Sandston, Virginia


Die Backside FIB Preparation for Identification and Characterization of Metal Voids ....................317


A. N. Campbell, W. F. Filter, Sandia National Laboratories, Albuquerque, New Mexico; N. Antoniou,Micrion Corporation, Peabody, Massachusetts


FIB Micromachining and Nano-Structure Fabrication.........................................................................327


R. A. Lee, P. J. Wolpert, FIB International, Inc., Santa Clara, California


Session 11: Case Histories II


Characterization and Fault Identification of Copper BEOL sub-0.25µm Six Level Metal


Microprocessor Designs.........................................................................................................................335


T. L. Kane, K. L. DeVries, M. T. Tenney, A. K. Patel, IBM, Hopewell Junction, New York


Analysis of Ohmic Contact Metal Deposition Defect Using FIB/SEM for a GaAs MESFET Clock


Buffer IC Device.......................................................................................................................................343


P. Y. Tsai, W. Bornstein, IBM Global Procurement, Hopewell Junction, New York


Identification of Subtle Isb Failure Mechanisms..................................................................................349


N. Wang, R. Zou, J. Wu, S. Daniel, W. Stevenson, Cypress Semiconductor Corp., San Jose,California


Session 12: Case Histories III


Investigation of High Frequency Failures on a 0.35µm CMOS IC ......................................................359


A. Kennen, J. F. Guravage, L. Foster, Analog Devices, Wilmington, Massachusetts; J. Kornblum,Analog Devices, Greensboro, North Carolina


BGA and Advanced Package Wire to Wire Bonding for Backside Emission Microscopy ..............365


J. B. Colvin, Consulting Services, Newark, California


Current-Signature-Based Analysis of Complex Test Fails .................................................................377


A. E. Gattiker, P. Nigh, IBM, Essex Junction, Vermont; W. Maly, Carnegie Mellon University,Pittsburgh, Pennsylvania


xvii


New Techniques for Logic Fault Diagnosis with a Case Study on the 440BX Chipset ....................389


S. Venkataraman, Intel Corporation, Hillsboro, Oregon; S. B. Drummonds, Intel Corporation, Santa Clara, California


Session 13: Case Histories IV


Electromigration and Electrochemical Reaction Mixed Failure Mechanism in Gold Interconnection


System......................................................................................................................................................399


H. Murayama, M. Yamazaki, ADVANTEST Corp., Gunma, Japan; S. Nakajima, NTT Electronics Corp., Kanagawa, Japan


Identification of Yield Limiting Defects in a 0.5 Micron, Shallow Trench Isolation Technology.....405


C. L. Henderson, C. E. Hembree, J. M. Soden, T. J. Headley, B. L. Draper, Sandia National Laboratories, Albuquerque, New Mexico


Visualization of Local Gate Depletion in PMOSFETs Using Unique Backside Etching and Selective


Etching Technique ..................................................................................................................................413


A. Nishida, T. Sekiguchi, T. Yamanaka, R. Yamada, K. Nakamura, S. Tomimatsu, K. Umemura, H.


Kakibayashi, Y. Yoshida, K. Funayama, S. Ikeda, Hitachi Ltd., Tokyo, Japan


Residual Photoresist Identified as Cause for Frequency-Dependent Signal-to-Noise Failure After


Autoclave Stress Testing........................................................................................................................419


M. J. McVeigh, National Semiconductor Corporation, Santa Clara, California


Session 14: Techniques II


From IDDQ Fault Detection to Defect Localization in Logic CMOS Integrated Circuits:


Key Issues................................................................................................................................................427


P. Perdu, R. Desplats, CNES - French Space Agency, Toulouse, France


Recent Advances in Broad Ion Beam Based Techniques/Instrumentation for SEM Specimen


Preparation of Semiconductors.............................................................................................................439


R. Alani, R. J. Mitro, Gatan Inc., Pleasanton, California; W. Hauffe, Dresden University of Technology,Dresden, Germany


A New Focused Ion Beam Microsampling Technique for TEM Observation of Site-Specific


Areas.........................................................................................................................................................449


References


1) P. R. Smith, D. H. Auston, and M. C. Nuss,“Subpicosecond photoconducting dipole antennas,” IEEE J. Quant. Elec., 24, 255 (1988).


2) S. E. Ralph, S. Perkowitz, N. Katzenellenbogen,and D. Grischkowsky, “Terahertz spectroscopy of optically thick multilayered semiconductor structures,” J. Opt. Soc. Am. B, 11, 2528 (1994).


3) Hu, B.-B. and Nuss, M. C., “Imaging with terahertz waves,” Opt. Lett., 20, 1716 (1995).


4) Mittleman, D. M., Jacobsen, R. H., and Nuss, M.


C., “T-ray imaging,” IEEE J. Sel. Top. Quant.


Elec., 2, 679 (1996).


5) Fattinger, Ch., and Grischkowsky, D., “Terahertz beams,” Appl. Phys. Lett., 54, 490 (1989).


6) Nahata, A., Auston, D. H., Heinz, T. F., and Wu,C., “Coherent detection of freely propagating terahertz radiation by electro-optic sampling,”Appl. Phys. Lett., 68, 150 (1996).


7) Wu, Q., and Zhang, X.-C., “Free-space electrooptic sampling of mid-infrared pulses,” Appl.


Phys. Lett., 71, 1285 (1997).


8) Lu, Z. G., Campbell, P., and Zhang, X.-C.,“Free-space electro-optic sampling with a highrepetition-rate regenerative amplified laser,”Appl. Phys. Lett., 71, 593 (1997).


9) Jacobsen, R. H., Mittleman, D. M., and Nuss, M.


C., “Chemical recognition of gases and gas mixtures with terahertz waves,” Opt. Lett., 21,2011 (1996).


10) Mittleman, D. M., Hunsche, S., Boivin, L., and Nuss, M. C., “T-ray tomography,” Opt. Lett., 22,904 (1997).


A scanning SQUID microscope can overcome some of these difficulties. A SQUID (Superconducting Quantum Interference Device) is a very sensitive magnetic sensor that can image magnetic fields generated by magnetic materials or currents (such as those in an integrated circuit). The current density distribution in the sample can then be calculated from the magnetic field image, and resolutions approaching 5 times the near field limit can be obtained.


We present here the application of a SQUID microscope to physical failure analysis and compare it with other techniques to detect shorted current paths in flip-chip mounted ICs and packages.


Introduction


In the late 1960s, Gordon Moore of Intel Corporation suggested that integrated circuits will double in complexity roughly every 18 months. This exponential increase in circuit complexity continues to tax our ability to debug and analyze failures in integrated circuits. Further complicating failure analysis is the industry’s recent trend toward flip-chip packaging. This requires that nondestructive


measurements be made through the silicon substrate.


As noted by Larry Wagner of Texas Instruments,“The tools we’ve become accustomed to using are in some jeopardy of not being able to meet our needs in


the very foreseeable future.” [1].


Of greatest interest to the failure analyst is the ability to see how the circuit is actually functioning, i.e.


what currents and voltages are occurring in the circuit during operation. Although techniques such as voltage contrast electron microscopy have some ability to detect circuit operation, they also have limitations. Voltage contrast microscopy can detect voltage differences, not actual voltage or current, and only in conductors near the surface of the chip.


11) Daubechies, I., Ten Lectures on Wavelets, Soc.


Ind. Appl. Math., Philadelphia, PA (1992).


ISTFA '99: Proceedings of the 25th International Symposium for Testing and Failure Analysis


Copyright © 1999 ASM International®


Electronic Device Failure Analysis Society, editor, p 11-16


All rights reserved.


DOI: 10.1361/cp1999istfa011


www.asminternational.org


# Detecting Power Shorts from Front and Backside of IC Packages Using Scanning SQUID Microscopy


Detecting Power Shorts from Front and Backside of IC Packages Using Scanning SQUID Microscopy


L. A. Knauss, B. M. Frazier, H. M. Christen, S. D. Silliman and K. S. Harshavardhan


Neocera Inc., Beltsville, Maryland


E. F. Fleet and F. C. Wellstood


Center for Superconductivity Research, University of Maryland, College Park, Maryland


M. Mahanpour and A. Ghaemmaghami


Advanced Micro Devices, Sunnyvale, California


Abstract


As process technologies of integrated circuits become more complex and the industry moves toward flipchip packaging, present tools and techniques are having increasing difficulty in meeting failure analysis needs. One of the most common failures in these types of ICs and packages is power shorts, both during fabrication and in the field. Many techniques such as Emission Microscopy and Liquid Crystal are either not able to locate power shorts or are inhibited in their effectiveness by multiple layers of metal and flip-chip type packaging.


Advanced Micro-Surgery Techniques and Material Parasitics for Debug of Flip-Chip


Microprocessor........................................................................................................................................477


R. H. Livengood, J. Giacobbe, P. Winer, J. Stinson, J. D. Finnegan, Intel Corporation, Santa Clara,California


Electronic Device Failure Analysis Society, editor, p 3-9


DOI: 10.1361/cp1999istfa003


Proceeding from the 25thInternational Symposium for Testing and Failure Analysis, 14-18 November, 1999, Santa Clara, California


# Terahertz Imaging: A New Technique for Inspection of Dielectric Materials


Terahertz Imaging: A New Technique for Inspection of Dielectric Materials


Daniel M. Mittleman


Rice University, Electrical and Computer Engineering Dept., Houston, Texas


Terahertz time-domain spectroscopy (THz-TDS) is a promising new technology which provides a relatively simple means of generating and detecting single-cycle pulses of far-infrared (or terahertz)radiation. One of the most interesting aspects of this system is its insensitivity to the thermal background.


This obviates the need for cryogenic apparatus; as a result, this may be the first portable far-infrared spectrometer.


Recent work has demonstrated the possibility of tomographic imaging using THz-TDS. In this imaging mode, a reflected pulse train is used to construct a three-dimensional representation of a composite material, using the timing between reflected pulses to determine the spacing between adjacent dielectric interfaces. Here, the transverse resolution is determined by the diffraction-limited focus of the THz beam, and is typically ~300 microns. The longitudinal (depth) resolution of ~100 microns is determined by the coherence length of the radiation, although the location of isolated surfaces can be determined with far higher precision.


Since many common packaging materials have high transparency in the THz range, this suggests the possibility of exploiting this new imaging system for non-invasive testing and on-line monitoring. The operation of the THz “T-ray” imaging system will be described, and several examples will be provided which illustrate its capabilities and limitations.


The far-infrared, or terahertz, region is one of the least explored ranges of the electromagnetic


spectrum. Until recently, it was relatively difficult to efficiently generate and detect terahertz (THz)radiation. Most THz sources were either low brightness emitters such as thermal sources, or cumbersome, single-frequency molecular vapor lasers.


Detection usually relied on bolometric methods,which require cryogenic operation and generally provided low sensitivity.


Recently, however, there has been a revolution in THz technology, as a number of newly discovered or re-discovered generation and detection schemes have revitalized the field. These techniques, based on frequency conversion using non-linear optics, are often simpler, more reliable, and potentially much less expensive than the more traditional approaches.


One of the earliest and most interesting of these nonlinear optical techniques is terahertz time-domain spectroscopy, or THz-TDS [1]. The key components of a THz-TDS system are a femtosecond laser and a pair of specially designed transducers. By gating these transducers with ultrafast optical pulses, one can generate sub-picosecond bursts of THz radiation, and subsequently detect them with high signal-to-noise.


These THz transients consist of only one or two cycles of the electromagnetic field, and they consequently span a very broad bandwidth. Bandwidths extending from ~100 GHz to 2 or 3 THz are routine, and more than 5 THz has been demonstrated


[2]. Furthermore, although the average intensity of the radiation is quite low, the high spatial coherence produces a brightness which exceeds that of conventional thermal sources. Finally, the gated detection is orders of magnitude more sensitive than typical bolometric detection, and requires no cooling or shielding of any kind.


More recently, advances in the data collection and processing rates have enabled the use of THz-TDS for imaging [3,4]. Images can be generated at rates up to 100 pixels per second, with high (~250 µm) spatial resolution. Figure 1 illustrates a THz “T-ray” image of a packaged integrated circuit, in which the metallic leads and the silicon IC are visible through the black plastic packaging. These recent advances have opened up a wide range of possibilities in the applications of far-infrared technology. Here, we review the technique of THz-TDS, providing several examples of images which illustrate its capabilities and limitations.


Terahertz Generation and Detection


Terahertz time-domain spectroscopy combines


ultrafast laser technology and optoelectronics to


generate and detect pulses of terahertz radiation,


whose duration is approximately one THz ‘optical’


cycle, less than one picosecond. Pioneered in the


mid-1980’s by groups at AT&T Bell Laboratories [1]


and IBM’s T. J. Watson Research Center [5], a typical


THz-TDS setup is shown in Figure 2. A mode-locked


solid state laser produces a train of optical (usually


near-infrared) pulses, of ~100 femtoseconds (10-13


sec) duration. This pulse train is split into two arms,*


one for the THz emitter and one for the detector. The


emitter is usually a semiconductor (typically GaAs)!


with some simple antenna structure lithographically


defined on its surface. These high-impedance dipole


emitters are typically DC-biased with a few tens of


volts. When a femtosecond pulse excites the


semiconducting material in the antenna gap with an


above-band-gap excitation, the photogenerated charge


carriers are accelerated by the applied bias field. The


rise time of this photocurrent can be nearly as fast as


the femtosecond optical pulse duration. This transient


current radiates according to Maxwell’s equations,


E(t) ∝ ∂j(t)/∂t. Because j(t) is approximately a step


function, the radiated field is close to a single-cycle


pulse, with extremely large fractional bandwidth.


When the radiation emerges from the rear surface of


the emitter, it is collected, first with a substrate lens,then using conventional far-infrared optics. The resulting THz beam can be collimated and focused just as any laser beam, except that the long wavelength radiation diffracts more readily than optical beams. Even so, a well collimated THz beam of ~1 cm radius can propagate for several meters before diffraction becomes significant. Using either reflective or transmissive optics, one can focus this beam to a diffraction-limited spot, with a minimum beam waist which approaches the wavelength of the light. Of course, the wavelength varies by more than one order of magnitude over the bandwidth of the pulse, so the behavior near the focal spot is quite complex. As shown in Figure 2, a sample may be positioned at the focal point of the THz beam, and images can be generated by measuring the transmitted THz pulse as a function of position on the object. In this fashion, ‘T-ray’ images can be generated at rates of up to 100 pixels per second [4].


The detection of these THz transients is accomplished using the second arm of the femtosecond beam. The detection relies on photoconductive sampling in an antenna similar to that used in the emission process.


When the femtosecond optical pulse arrives at the detector antenna, it generates charge carriers just as in the emitter. These carriers are accelerated, not by an externally applied DC field, but by the incident THz electric field. However, this acceleration only occurs if the THz field arrives at the detector at the same instant as the optical pulse. In that case, a current is generated across the antenna which is proportional to the THz electric field. Since the carrier lifetime in the semiconductor is quite short (only a few hundred


Figure 1 THz “T-ray” image of a packaged


integrated circuit, in which the metal leads and the circuitry are visible through the black plastic package.


The spatial resolution in this image is approximately 250 microns.


Femtosecond Laser


Scanning Optical Delay Line


THz


Transmitter


Current


Preamplifier


A/D converter


& DSP


THz Detector


DC bias


Sample


Figure 2 Schematic of the THz imaging system,


showing the femtosecond laser, scanning optical delay line, THz transmitter and detector, THz optics,the sample, and associated electronics.


femtoseconds), this antenna acts as a fast sampling gate which can be used to map out the temporal shape of the THz field. One simply measures the induced photocurrent in the detector antenna as a function of the delay between the arrival of the two pulses. This delay is systematically varied using a scanning optical delay line, as shown in Figure 2.


This measurement relies on the fact that the photogenerated electrons in the receiver antenna have a high mobility (because the induced current depends on the carrier mobility) and also a fast carrier lifetime(because a sampling measurement is only useful if the sampling window is fast compared to the transients being measured). These requirements place rather stringent demands on the semiconductor materials


)arb.unitsAmplitude(


used in the detector. Currently, low-temperaturegrown (LT) GaAs and radiation-damaged silicon-onsapphire are the two most common choices. These materials have been used for spectroscopic measurements spanning bandwidths from below 0.1 THz to beyond 5 THz. A typical THz pulse measured in this fashion is shown in Figure 3.


Recently, a second detection scheme has been gaining in popularity. This newer technique is known as freespace electro-optic sampling [6]. Here, the THz beam co-propagates with a synchronized femtosecond probe pulse in an electro-optically active material.


The electric field of the THz pulse induces a polarization rotation of the femtosecond probe beam,via the Pockel’s effect. This rotation can be measured as a function of the delay between the THz pulse and the optical pulse, giving a direct measurement of the THz electric field. In contrast with the photoconductive technique outlined above,the electro-optic non-linearity is non-resonant, and thus responds essentially instant-aneously to the applied field. As a result, this tech-nique can provide much more detection bandwidth, limited by the duration of the femtosecond probe pulses. Using ZnTe as a detector, bandwidths as large as 37 THz have been reported [7].


This detection scheme also permits focal plane imaging, using highly uniform electro-optic crystals,and a probe beam whose diameter is expanded to match that of the THz beam. This technique requires considerably more power in the femtosecond probe beam, which complicates matters somewhat.


Nonetheless, video-rate THz imaging (288×384 pixels) has been demonstrated recently [8].


It should be emphasized that both of these detection techniques are coherent; they measure the THz electric field E(t), not the intensity |E(t)|2. As a


result, the phase information is preserved, and one may determine both the real and imaginary parts of a sample’s dielectric function simultaneously and independently. This phase-sensitive detection has a further advantage in the near-complete rejection of incoherent radiation. Thus, these detectors generally operate at room temperature and in ambient light.


This obviates the need for the cumbersome cryogenic systems typically required in far-infrared systems.


Additionally, it permits spectroscopic and imaging


studies of hot samples such as flames or plasmas,whose large thermal signatures would ordinarily swamp an incoherent detector. An example of this is shown in Figure 4, which is an image of a ~1 cm gas flame [4]. Here, the contours indicate different transit times for the THz pulse through different regions of the flame. The variation is due to the change in refractive index of the air which results from heating.


This may be of interest in high temperature materials processing such as ceramic sintering, or in the monitoring of moderate to high density plasmas. The extreme sensitivity of THz radiation to liquid water is


of interest to the plastics industry as well as for evaluation of the moisture content of food products.


The various imaging modes, either transmission or reflection, using either amplitude or phase, afford a great deal of flexibility, and vastly broaden the range of possible applications of this technology. Of course, a great deal of work is still required. For example, although the femtosecond laser systems


F


Terahertz time-domain spectroscopy is a promising new technology, providing a unique means for accessing the far-infrared spectral range. Spectroscopists have only just begun to explore the many interesting possible uses for these single-cycle subpicosecond bursts of light. Because of the nature of the detection technique, these possibilities extend beyond the laboratory. Many ‘real-world’ applications of terahertz imaging are being envisioned, and this has motivated the ongoing development of a commercially viable system. Although significant work is still required, the future for T-rays looks bright.


0


1


2


3


4


5


1.0


1.1


1.2 Refractive index1.3


1.4


1.5


disketterear cover


front cover


Optical depth (mm)


Figure 9 Refractive index profile at one pixel on the floppy disk shown in Figure 8. The solid line is the


profile derived from a reflected waveform; the


dashed line is the actual profile. Discrepancies


between the two result from several approximations in the signal processing algorithm.


Adjacent contours correspond to shifts in the arrival time of only 5 femtoseconds


500 1000 1500 2000


-2 0 Amplitude (Volts)2 4


Delay (femtoseconds)


0 11


0 2 4 6 8 10


Frequency (THz)


Figure 3 THz electric field, and corresponding


frequency spectrum. The small ripples following the main pulse (and the small dip in the spectrum at ~0.6 THz) are the result of absorption from residual water vapor in the beam path.


10 15 20 25


0 10 20 30 40


position (mm)


Figure 4 THz image of a small gas flame, showing the variation in air density resulting from local heating.


Applications of Terahertz Imaging


The extremely high temporal resolution, coherent detection, diffraction-limited focusing, and relative simplicity of the THz-TDS system provide new and unique opportunities for spectroscopists. Even more interesting are the many possible applications of this imaging spectrometer, in such areas as gas sensing[9],package inspection and quality control, agricultural monitoring, and biomedical imaging[4]. Many of these ideas stem from two important facts: first, many common packaging materials, such as plastic,cardboard, and thin pieces of wood are largely transparent to THz radiation, and second, liquid water is strongly absorbing. Thus, it is possible, for example, to measure the water content of many prepackaged foods and other consumer products. The location of voids or objects buried in plastic is usually quite effective, as demonstrated by Figure 5. This shows a THz image of a portion of an automobile dashboard, which consists of two flat plastic shells with foam rubber filling the ~1 cm gap between them.


The THz image clearly shows the location of an air bubble in the foam rubber. This technique is quite general; images can be generated of a wide range of samples, including many packaged food products, and countless plastic and composite parts such as the packaging for integrated circuit chips.


0 10


Position (mm)


20 40


30


10


20


40


60


50


Figure 5 THz image of a portion of an automobile dashboard, in which a small bubble in the impact


foam is clearly evident (white area, at left).


-2 0 Amplitude(volts)2 4


Time (psec)


(a)


-1 0 1


6


(b)


Figure 6 THz waveforms (a) incident on and (b)


transmitted through a block of epoxy. The chirp


imposed on the waveform is characteristic of the


material, and may be used for materials identification,in conjunction with imaging.


One of the most interesting characteristics of THzTDS is the extremely short duration of the THz pulses. Because many materials have strong absorption or dispersion features in the far infrared,the temporal distortions which are imposed on the sub-picosecond pulses are characteristic of the materials with which the radiation has interacted. As a consequence, the distortions of the time-domain THz waveform can be used to identify or characterize the materials [9]. An example is shown in Figure 6,which depicts the waveforms incident on and transmitted through a block of epoxy. The strongly frequency-dependent refractive index of this material is evident in the ‘chirp’ exhibited by the transmitted waveform.


A second important advantage of the short pulse duration is that it enables tomographic imaging.


Here, the THz pulse is reflected off of a sample,rather than transmitted through it. If the sample consists of a number of dielectric layers or interfaces,then each interface gives rise to a temporally distinct reflected pulse. The timing between these pulses is related to the depth of each interface beneath the surface of the object. In this fashion, a full threedimensional representation of the object can be reconstructed [10].


Figure 7 shows an example, in which an incident waveform (a) is reflected off of a conventional 3.5-inch floppy disk. Each of the dielectric interfaces which comprise the sample is visible in the reflected waveform (b), including the front and back surfaces of both the front and rear plastic cover, and the magnetic recording material. Curve (c) represents the results of curve (b) after deconvolution of the instrument response, represented by (a). This procedure permits resolution of the front and back surfaces of the thin magnetic recording material,


unresolved in the raw waveform. The limit of the depth resolution is determined by the bandwidth of the THz radiation, and is approximately 100 microns in this example.


Note that the sign of each reflected pulse is related to the sign of the dielectric discontinuity at the corresponding interface. For example, in curves (b)and (c), a predominantly negative spike corresponds


kayldlmm


to a reflection from an air-to-plastic interface,whereas a predominantly positive spike corresponds to reflection from a plastic-to-air interface. This sign change is a consequence of the Fresnel equations for electromagnetic propagation, and can be used to encode further information in an image.


Figure 8 illustrates a tomographic image, using the same floppy disk of Figure 7. In Figure 8, the upper panel shows a conventional two-dimensional image of the floppy disk. The lower panel shows a tomographic “slice” through the disk, along the position indicated by the dashed line in the upper figure. In the lower figure, the vertical axis corresponds to depth into the object. Various structures within the floppy disk are resolved. The sign of the dielectric discontinuity at each interface is encoded into the image using the gray scale, with darker (lighter) interfaces representing positive(negative) refractive index steps. From data such as this, one can extract the full refractive index profile of the sample, using inversion algorithms similar to those employed in geological surveying. One can readily detect and locate any dielectric discontinuities with spatial extent comparable to or larger than the~250 micron spatial resolution.


In Figure 8, the ‘depth’ axis is not calibrated, since one does not know a priori the refractive indices of each of the layers which comprise the material. A close examination of this tomographic image reveals the difficulties which can arise as a result. For example, one can observe an apparent discontinuity in the diskette at the position x ~ 12 mm. This is a result of a change in thickness of the front plastic cover,which produces a change in the travel delay in the THz pulse reflected from the diskette. In order to calibrate this axis, one must know the refractive index profile along the propagation direction, at each horizontal position of the sample. If the refractive index of this plastic material were known accurately,one could account for this error in the image formation, in essence calibrating the depth axis.


15


25


35


-40


(


V


u


)


j


n


o


d-200


<


Delay (psec)


(c)


back cover


floppy disk


Figure 7 THz waveforms (a) incident on and (b)reflected from a 3.5-inch floppy disk. Curve (c)represents curve (b) after deconvolution of the instrument response.


!


s


A


20 30


5 4 3


w


a


p


e


,


2 1 0


x position (mm)


metallic hub


diskette


back cover front cover


Figure 8 Reflection image (top) and tomographic image (bottom) of a portion of a floppy disk. In the lower image, buried internal surfaces can be


discerned, including both surfaces of the magnetic recording material.


In principle, all of the information required for such a calculation is contained in the impulse response function of the medium, which can be derived from the reflected waveform via deconvolution, as shown in Figure 7c. One can derive a recursive algorithm,based on the Fresnel transmission and reflection coefficients, which generates the refractive index profile from the deconvolved waveform[10]. This relation is exact if the medium exhibits neither absorption nor dispersion over the bandwidth of the THz pulse, and if the finite bandwidth of the source(finite coherence length) is neglected. Figure 9 shows the refractive index profile derived using this approximate algorithm. Evidently, this procedure produces only an approximation to the actual profile(dashed line). The discrepancies are a result of the aforementioned assumptions. Development of a more accurate method for extraction of the index profile is a topic of current research.


Conclusions


The unique aspects of this new imaging technology have attracted interest from a number of industries,primarily in the manufacturing sector. The ability to image through most common packaging materials without the need for x-rays or other ionizing radiation is attractive in many quality control applications,particularly in consumer products manufacturing.


The coherent detection of the THz waveform also permits imaging of thermally active media, an ability possessed by no other far-infrared detection system.


used to drive the THz-TDS system have made dramatic progress in recent years, they are still largely research tools, and not yet robust enough for field deployment. One exception is the mode-locked fiber laser, in which the gain medium is a short length of erbium-doped optical fiber. These lasers are quite reliable, and are naturally compatible with fiber coupling of the THz emitter and receiver, a necessary step to avoid the alignment issues associated with free-space coupling of the femtosecond beams to the antennas. However, adapting the THz-TDS system for use with a fiber laser is by no means a simple task.


The most significant hurdle involves the materials used for THz generation and detection. New materials must be developed, since the commonly used semi-conductors do not absorb light at 1550 nm,the wavelength of the fiber laser. Other hurdles include finding a reasonable means for generating the optical delay required for the sampling measurements. A challenge which may be just as significant as these hardware issues is the development of signal processing algorithms, for extracting the desired information from the measured THz waveforms. Ultimately, the effectiveness of these algorithms will be the determining factor in the performance of the system. Although the best approach for de-convolution, denoising, and image formation are not yet clear, it appears that methods based on wavelet transforms hold a great deal of promise, due to the highly localized time-frequency character of the THz waveforms [11].


Modern ICs now have as many as four to seven layers of metal interconnects above the transistors.


The top layer of metallization is often a large area power or ground plane which may shield out all electric fields of the lower level conductors through the Faraday effect. Thus it is very difficult to do nondestructive evaluation of the lower level conductors,and impossible in a flip-chip configuration.


Furthermore, currents are not detected directly by voltage contrast, so failures such as a short circuit can only be detected indirectly.


The SQUID (Superconducting Quantum Interference Device) microscope overcomes many of these problems. It enables backside or through-thepackage imaging of current. These current paths can be compared to CAD layouts for short localization.


Scanning SQUID Microscope


A Scanning SQUID Microscope is a sensitive nearfield imaging system for the measurement of weak magnetic fields. This unique microscope can map out buried current-carrying wires by measuring the magnetic fields produced by the currents, or can be


12 used to image fields produced by magnetic materials.


By mapping out the current in an integrated circuit or a package, short circuits can be localized and designs can be verified to see that current is flowing where expected.


For the present experiments, we used Neocera’s SQUID microscope, MAGMA-C1, which is shown in Figure 1. This instrument is capable of measuring magnetic fields as small as 20 pT (about 2 million times weaker than the earth’s magnetic field).


The SQUID sensor is sensitive enough that it can detect a wire even if it is carrying only 10 nA of current at a distance of 100 µm from the SQUID sensor with 1 second averaging. The microscope uses a patented design to allow the sample under


investigation to be at room temperature and in air while the SQUID sensor is in vacuum and cooled to


less than 80°K [2]. During non-contact imaging of room temperature samples in air, the system achieves a raw, unprocessed spatial resolution equal to the distance separating the sensor from the current, or the effective size of the sensor, whichever is larger. To best locate a wire short in a buried layer, however, a Fast Fourier Transform (FFT) back-evolution technique can be used to transform the magnetic field image into an equivalent map of the current in an


integrated circuit or printed wiring board [3, 4]. The resulting current map can then be compared to a circuit diagram to determine the fault location. With this post-processing of a magnetic image and the low noise present in SQUID images, it is possible to enhance the spatial resolution by factors of 5 or more over the near-field limited magnetic image. This enhanced resolution describes how well a scanning SQUID microscope can resolve current paths in a sample. The system’s output is displayed as a falsecolor image of magnetic field strength or current magnitude (after processing) versus position on the


sample. After processing to obtain current magnitude,this microscope has been successful at locating shorts


in conductors to within ±16 µm at a sensor – current distance of 150 µm. The physics of SQUIDs and SQUID microscopy is described in more detail


elsewhere [5-7].


To evaluate the scanning SQUID microscope as a failure analysis tool, we investigated shorts at both the die level and package level.


Experimental Results:C4 Flip-Chip Devices


To compare the advantages of scanning SQUID microscopy over other failure analysis tools, three C4 flip-chip devices with five layers of metallization were selected. A photograph of this device is shown in Figure 2. These devices were yield rejects and the failure mode was established to be power shorts or Vcc-Vss shorts. A good device was selected as a control unit.


Backside Sample Preparation


For thinning the samples a polishing wheel with a


Micro Adjustable Tool [8] was selected. Since the thickness of the die’s substrate can affect the results on certain backside failure analysis tools and techniques, the substrates of the C4 die were thinned


and polished to 80 µm for maximum efficiency [9]. In order to keep the physical conditions of the samples the same through out the experiment, all the devices including the control sample were thinned.


Figure 1 Photograph of the commercial scanning SQUID microscope, MAGMA-C1, with electronics rack and probe station.


Figure 2 Photograph of a C4 flip-chip device.


Emission Microscope Analysis


Emission microscopes can detect metal-metal shorts


due to thermal radiation [10]. This also requires hundreds of milliamps of current. Even at a very high current, the filament which caused the short may vaporize and change the failure mode/mechanism.


Also, at high current, some transistors may go to saturation and misguide the analyst. In our case, the failed devices did not show any emission even at higher current (~2 mA), but the control unit showed several emission points which are characteristic of a good device.


Hot Spot Detection Technique


Ferrier in 1997 proved that liquid crystal techniques for very thick ICs (more than four layers of metallization) are impossible especially if the leakage


current is low [11]. In the case of a C4 flip-chip, the thickness of the substrate is about 80 µm thick,therefore Ferrier’s technique will not work. Another hot spot detection technique is the “poor man’s technique” in which the surface of the substrate is cooled by Freon gas. The device is then powered up and consequently the hotter spots on the die melt the thin layer of ice. When trying this approach on our samples, no hot spots were detected. The substrate was too thick, and the current was too low (~2 mA).


Scanning SQUID Microscope Analysis


The SQUID microscope was used to investigate the three C4 flip-chip devices. The samples were imaged nondestructively at a SQUID – current separation of


~350 µm (measured at the corner of the package)using currents as low as 170 µA at 2 kHz. Figure 3 shows the raw magnetic field image of the control sample overlaid on an optical photograph. The image corresponds to the z component of the magnetic field(perpendicular to the plane of the sample). The red and blue correspond to oppositely directed fields and the white corresponds to zero field in the z direction(in the simplest case, white corresponds to where current is flowing). In the majority of shorts, the location of the fault can be identified by the presence of a very intense localized magnetic field. This sample shows a complex distribution of magnetic fields resulting from the current as it follows a distributed path through the package and die. On the die there is a strong magnetic field in the lower left corner which indicates the presence of concentrated current. This is the result of normally higher levels of current in the buffer region of the die. This region corresponds to the location of emission sites observed with the emission microscope.


Figure 4 (a) and (b) show the magnetic fields of the two samples with power shorts overlaid on an optical image of the die. Figure 4(a) is a scan of a region


slightly larger than the die, and Figure 4 (b) is a scan of the lower left quadrant of the second die. In each image, the location of the short is indicated by a large localized magnetic field at different locations.


Figure 3 Magnetic field image of the control sample.


The gold bars are 3.42 mm long.


Figure 4 (a) and (b) Magnetic field images of power shorts in two different flip-chip devices. The gold bars are 3.42 mm long.


14 To more precisely localize the defect region, the


magnetic fields can be used to calculate the current path in the die. Figure 5 (a) and (b) show the current images for the shorted samples in the same order as the magnetic fields in Figure 4. These images are overlaid on the optical images of the die. The current images show a maximum corresponding to the most concentrated current and therefore the most probable location of the short. From these images the short


can be localized to a region of about 300 µm x 300 µm.


Experimental Results:Package Level


Package level shorts were also investigated with the scanning SQUID microscope on samples received from the Interconnection Technology Research Institute (ITRI). One example of a signal-to-ground short will be given here.


Figure 6 shows an optical photograph of the substrate. This sample had a short between two signal lines and ground. After applying 2 mA at 1 kHz to the appropriate lands on the back of the substrate, the SQUID microscope was used to map out the magnetic fields produced by the current. The magnetic image is shown in Figure 7(a). The magnetic fields are concentrated where the current is entering and leaving the substrate, but the general distribution of magnetic fields around the whole substrate indicates a general distribution of current as might be expected in the ground plane. Figure 7 (b)shows an overlay of the current image on the schematic of the ground plane. The current can be seen to short from a via to the ground plane where it is distributed through several current paths before converging at another via. The broad distribution of current leading up to the via on the left is in the supply wire attached to the land on the backside of the substrate ~ 1.5 mm away from the SQUID. The distribution of current on the ground plane is interesting, because one can see the current paths on the metallization between the rows of vias. If this were a normally functioning board, one could use that current distribution image to do device verification. From the image, the distribution of current is clearly not uniform possibly indicating a design or processing problem. Additionally, two weak current paths can be observed flowing diagonally toward the center of the substrate. These paths are actually ground lines on the Vcc plane in the next layer down indicating the ability to distinguish between current on different layers in the structure.


If the intensity of the image is turned down, the location of the shorts can be precisely located.


Figure 8 shows a close-up view of the current shorting from each of the vias to ground. In particular, it can be determined which side of the via


Figure 5 (a) and (b) Current images of power shorts in two different flip-chip devices. The gold bars are 3.42 mm long.


Figure 6 Optical image of substrate from ITRI.


15 is shorted and approximately where on that side of


the via reducing the area of interest to about 100 µm x 100 µm as compared to the size of the via which is~ 250 µm x 400 µm. This makes it easy to cross


section precisely and determine the cause of the problem.


As one can see from this example, it is possible to use this instrument to do short localization very precisely in a printed wiring board and verify design performance. These measurements can be made through multiple layers of metallization, and information can be obtained to indicate current on different layers. Although the current supplied in this case was > 1mA, high quality images can be obtained at current levels more than an order of magnitude lower.


The scanning SQUID microscope can be used to localize the region of shorts in dies and packages even when other techniques like emission microscopy and liquid crystal are ineffective. The high sensitivity of the SQUID sensor enables these


measurements to be made with currents less than 200


µA with a sample sensor separation of approximately 350 µm. The ability to sense and localize shorts at large distances makes this tool ideally suited for nondestructive evaluation of current paths in buried layers of packages and flip-chip mounted dies.


Acknowledgements


The authors would like to thank Marshall Andrews of ITRI for supplying the substrate sample.


Figure 8 Current path through short from via to


ground metallization at (a) first location and (b)


second location. The width of the signal lines in both


images is 50 µm. The full width of each image is (a)


4.53 mm and (b) 4.22 mm.


Figure 7 (a) Magnetic field image. (b) Current Image overlay on the ground plane schematic (current image has been rotated to match schematic).


1) J. Ouellette, The Industrial Physicist p. 11 June(1998).


2) World wide patents issued and pending.


3) J. P. Wikswo, Jr. “The Magnetic Inverse Problem for NDE”, in H. Weinstock (ed.),


SQUID Sensors: Fundamentals, Fabrication,and Applications, Kluwer Academic Publishers,pp. 629-695, (1996).


4) E.F. Fleet et al, “HTS Scanning SQUID Microscopy of Active Circuits”, Appl.


Superconductivity Conference (1998), to be published.


5) E.F. Fleet et al, “HTS Scanning SQUID Microscope Cooled by a Closed-Cycle Refrigerator”, Appl. Superconductivity Conference(1998), to be published.


6) J. Kirtley, IEEE Spectrum p. 40 Dec. (1996).


7) F.C. Wellstood et al, IEEE Transactions on


Applied Superconductivity, 7(2), 3134 (1997).


8) Mahanpour et al “ Techniques to Remove the C4 die from a Ceramic Package”, ISTFA ’98


9) Steven Chen et al “Infrared Imaging and Backside Failure analysis Techniques on Multilayer CMOS Technology”, IPFA ’97.


10) N. Khurana, “2nd generation Emission Microscopy and its Application”, ISTFA ’89.


11) S. Ferrier, “ Thermal and Optical Enhancements to Liquid Crystal Hot Spot Detection Methods”,ISTFA ’97.


Electronic Device Failure Analysis Society, editor, p 19-25


DOI: 10.1361/cp1999istfa019


# Waveform Acquisition from the Backside of Silicon Using Electro-Optic Probing


Waveform Acquisition from the Backside of Silicon Using Electro-Optic Probing


Mike Bruce, Greg Dabney, Shawn McBride, Jason Mulig, Victoria Bruce, Charles Bachand


Advanced Micro Devices, Austin, Texas


Steven Kasapi and Jeffrey A. Block


Schlumberger ATE, San Jose, California


A new tool (Schlumberger IDS 2000) has become available for acquiring waveforms from C4 (also known as flip chip) packaged IC’s. The waveform acquisition technique is based on electro-optic sampling through the backside of silicon. After explaining the physics of electro-optic sampling, the technique is demonstrated through the backside of Si on a simple diode test structure and a flip chip microprocessor. Also, many of the issues and challenges with this tool are discussed.


Conventional waveform analysis tools (eg. E-beam or electrical micro-probing) are not capable of acquiring signals from the backside of silicon, as required by C4 packaging, without extensive backside micro-structural modifications (eg. FIB, laser etching, etc). A new tool(Schlumberger IDS 2000) has been introduced which utilizes a novel electro-optic sampling technique to acquire waveforms through the backside of silicon [1].


The only sample preparation needed involves thinning and polishing the backside of the silicon.


Electro-optic Sampling


Theory


The basic physical effects in the interaction of light with silicon in an external electric field have been discussed previously. Most of the early work was performed at Stanford University, IBM, and the University of Washington [2-7] in the late 80's and early 90's. These investigations used lasers at 1.3 µm (0.95 eV). The IDS 2000 system uses a 1.06 µm (1.17 eV) laser which is slightly above the silicon bandgap. Using a laser tuned


close to the silicon bandgap gives rise to stronger silicon-light interactions, allowing successful probing of CMOS devices.


When an electric field is applied to silicon the field causes the valence and conduction bands to mix slightly,reducing the effective bandgap. This reduction in bandgap with an applied electric field is known as the Franz-Keldysh effect [8]. In doped silicon there is also an optical interaction between the light and the dopantinduced free carriers. The free carrier optical interaction is a quasi-plasma effect and is roughly proportional toλ•. The free-carrier absorption and refraction is more significant at longer wavelengths [9] but still plays an important role in the signal acquired by the IDS2000.


In a pn junction, such as that formed between a transistor drain or an antenna diode and the silicon substrate, the application of an electric field increases the width of the space-charge region. The increase in the space-charge region reduces the number of free carriers in that volume, thus reducing the free-carrier absorption.


When an integrated circuit is modulated by an electrical signal, electric field and charge density modulations occur within internal devices (ie, transistors, diodes,etc). The refractive index (n) and absorption coefficient(α) change according to:


∆n = noq2/(2ω2ε) [ ∆Ne/me + ∆Nh/mh]


(Free Carrier Refraction)


∆α = noq3/(ω2εc) [ ∆Ne/me2µe + ∆Nh/mh•µh]


(Free Carrier Absorption)


(1)


for free carrier modulation, and


∆n = a E2 (Electro-refraction)∆α = h E2


(Electro-absorption) (2)


for modulations in the electric field (Franz-Keldsyh effect). no is the quiescent optical index of refraction, c the speed of light, q is the electron charge, ω is the optical frequency, ε is the optical permittivity of Si, me and mh are electron and hole effective masses, µe and µh are electron and hole mobility, ∆Ne and ∆Nh are the electron and hole density changes, a and h are material dependent constants, and E is the electric field [9]. Thus a technique sensitive to very small changes in the index of refraction and/or absorption coefficient would be capable of observing modulations due to an electrical signal.


IDS 2000 System


The key components of the IDS 2000 are a confocal laser scanning microscope (LSM), precision timing electronics, data acquisition electronics, a modelocked Nd:YAG laser, and a GUI interface through which the user interacts with the system.


The LSM raster scans a laser beam to produce the image of the device layer. For initial alignment and navigation the system includes an 8x objective with a 4 mm field of view. A 100x objective lens with NA of 0.85 is used for high-resolution imaging and waveform probing. The laser beam Full-Width-Half-Max (FWHM) is less than


0.77µm which provides sufficient resolution for imaging and probing devices with 0.18 µm gate widths, as will be discussed in a later section. The 100x objective also contains a correction element to avoid spherical aberration from the silicon substrate. Without correction,the high index of refraction of the silicon would bend the rays of light more tightly at the edge of the beam than at the center and distort the focus. The aberration correction ring allows the system to achieve nearly diffraction-limited performance.


Once the node to be probed is visually located the LSM scanning mirrors are turned off and the mirrors are steered onto the node using a cursor on the LSM image displayed in the GUI. The light is focussed through the silicon substrate onto the diffusion of interest. An InGaAs photodetector detects the reflected beam.


Because of the confocal nature of the LSM, only the light which reflects off the region in focus (a diffusion region, for example) is detected by the photodetector.


The total detected reflected power is on the order of


0.1% of the incident power. In addition to isolating the diffusion region, the confocal LSM weakly converts phase modulation from refractive index changes into amplitude modulation.


The IDS 2000 also detects the incident laser power through an optical pick-off in the LSM. The incident component is used in a noise reduction scheme designed to cancel out laser amplitude noise.


The detected photocurrents are amplified and digitized with low-noise electronics by the data acquisition subsystem. The data is averaged repeatedly and displayed on a workstation as a time-varying waveform.


The reconstructed waveform amplitude is represented as a parts-per-million (ppm) modulation of the laser beam.


Typical modulation depths are in the range of 100 ~2000 ppm (parts-per-million) and acquisition times are typically a few minutes.


Even though the optical spot size is greater than some diffusion dimensions, the induced modulation from a single node is still detectable. In particular, as discussed above, refraction effects below the spot size can give rise to amplitude modulation signals. The pointing accuracy of the LSM is 0.04 µm, thus overlaying the CAD database to the LSM image can allow very precise beam positioning for accurate probing.


The laser pulses are generated by a 100 MHz actively modelocked Nd:YAG laser with a pulse width of approximately 35 ps. The typical energy per pulse delivered to the sample is 10-100 pJ. The modelocked laser's 100 MHz clock is synchronized by IDS 2000's timebase circuitry to the tester clock frequency.


The electrical waveform is optically sampled each tester loop by one pulse from the modelocked laser. The time of the pulse relative to the start of the loop is gradually increased to accumulate a stroboscopic measurement of the waveform. In order to perform this stroboscopic sampling, a phase shift is introduced between the laser clock frequency and the tester frequency, allowing picosecond control of the laser pulse timing relative to the tester clock. An electro-optic modulator selects one optical pulse per tester loop.


One key feature of the system is its ability to suppress the effect of vibrations on the measurement. Vibrations induced by the tester, floor vibration, or acoustic noise on the test floor can easily induce high levels of modulation in the precision LSM used in the IDS 2000.


To significantly reduce the effect of vibrations, the IDS 2000 uses a patented dual-laser noise cancellation scheme. One laser (a pulse-shaped continuous-wave Nd:YAG laser) acts as a monitor of sample vibration while the other laser (the modelocked Nd:YAG laser described above) performs the actual waveform sampling.


Basic System Performance


o0d lnPT ou /DG rp teK15/512 avg.


Schumberger25 MHz


Acquisition times are typically several minutes. The bandwidth of the system is nominally 8 GHz with a minimum resolution of 10ps per division. Waveform amplitude and timing repeatability has been established


NH


as better than 20%. With the CLSM, the backside near infrared imaging resolution is typically 0.8µm or better using the 100x 0.85NA lens.


Early Results


Initial Evaluation: Results from Test Chip


As an aid in the initial evaluation of the system, a test chip was utilized. The test chip was based on a 0.25µm technology and was the same process used for the flip chip microprocessor presented in the next section. Test chip die were thinned and polished to 80-125µm. Tests were conducted on gate protection diodes of n-channel transistors. Results from the gate protection diodes are shown in Figs. 1a-d. Fig. 1a is an oscilloscope trace of the input waveforms while Fig. 1b shows the waveforms measured with the IDS 2000. Fig. 1c is a backside image of the probed gate protection diode with a 20x20µm field of view while Fig. 1d is a larger field of view(160x160µm) image of the same diode. The diodes were driven by square pulse signals at 12.5 and 25MHz at both 25% and 50% duty cycle. The 100MHz ripple in the 12.5MHz signal is due to bleed through from the probe beam which samples at 100MHz. Signal speeds as high as 400MHz have been measured.


Dw* H0日


④m


hmos1_12.5_50%


Figure 1a Oscilloscope trace of input waveforms (12.5 and 25 MHz signals) to gate protection diode on test chip. 50% and 25% duty waveforms were measured at each frequency.


Figure 1b Early IDS2000 Waveforms of 12.5 and


25MHz signals measured on gate protection diode of an


n-channel transistor. Input waveforms are shown in Figure 1a. Subsequent improvements in the signal are shown in Figure 4.


Figure 1c Backside image of the probed gate protection


diode from which the waveforms in Figure 1b were


nmos1


2o


obtained. The field of view is


合509


￥


hmos


脑


fH100m20


长a3e


20x20µm.


Figure 1d A 160x160µm field of view image of the diode described in Figure 1c.


Initial Results from a Flip Chip Microprocessor


Shortly after the system arrived, waveforms were obtained from a flip chip microprocessor. Early results,shown in Fig. 2, were similar to the test chip. The signals were obtained from n+ active (in p-substrate)input protection diodes. All the waveforms were inverted relative to simulated waveforms; however,excepting the inversion, all the waveforms are in excellent agreement with the simulation. The causes of the inverted waveforms and methods for avoiding inversion are discussed later.


The signals, measured in parts per million (ppm)(represents the amount of differential laser power absorbed), are generally comparable to the test chip.


However, it is noted that signal quality does vary from node to node. Improvements to the signal are discussed in the next section.


|ADVANCED MICRO DEVICES |ADVANCED MICRO DEVICES |||||||||
|---|---|---|---|---|---|---|---|---|---|

|200 |ppm/div |5 |ns/div |28.966 |µs |delay |5/2048 |avg. ||

||||||||||A |

||2||||||一|||

||||||||||C |

||g||女|||||W||

1 LOCK 0


Figure 2 Initial IDS 2000 waveforms obtained from a flip chip microprocessor. Results of improvements described in the next section are shown in Figure 4.


System Considerations


Although the IDS2000 has proven capable of acquiring waveforms from the backside of silicon, initially the system presented some challenges before it could be fully utilized. Some the issues and lessons learned, some of which led to a considerable improve-ment in system performance, are described henceforth.


Stage drift and vibration


The stage is separated from the optical column through a large metal frame. This means the system is prone to drift which is attributed to mechanical stress relaxation and thermal expansion of the frame. A stage drift of less than 1µm can adversely affect signal acquisition. In practice, this has had the effect of limiting loop times to 150µs without intervention (i.e., refocussing). For longer loop times, user intervention is often required. An existing manual algorithm for probe tracking is being investigated for automatic probe tracking which would eliminate user intervention.


Laser stability


The actively modelocked probe laser used in the IDS 2000 requires a very close match between the clock frequency and the length of the laser cavity. For this reason, the 35ps modelocked laser can exhibit instability from time to time which can affect waveform acquisition. The laser sensitivity requires the user occasionally to temperature cycle or adjust the cavity length of the modelocked laser.


The modelocked laser is quite sensitive to temperature and pressure changes in the room; hence, it is very important to have a well-controlled environment.


The effect of the finite system bandwidth has not yet been observed in the data collected on logical transitions. We define the timing resolution as the minimum resolvable time difference between two transition edges; it is roughly twice the measured transition time divided by the signal/noise ratio. The system bandwidth is sufficiently high to allow timing resolution better than 30 ps. In Fig. 10 we show a timing edge with a 70 ps transition time. The bandwidth and step response of the system will be explored more fully in a future publication.


Figure 10 Fast transition times measured with laser


probing.


Comparison with Other Techniques


Laser probing compares favorably to alternative backside technologies: backside e-beam probing and emission-based signal acquisition. Backside e-beam probing relies on depositing a metal probe pad from the backside after focused ion beam milling through


the silicon substrate[*6]. Once the probe point is deposited, the probing proceeds as with frontside ebeam probing. However, creating probe points in this manner is very time-consuming and significantly limits the rate at which nodes can be probed.


Emission-based circuit diagnostics, which have been pioneered by Kash et al. [*7-10] at IBM, utilizes the


naturally occurring luminescence from every saturated NMOS transistor. Their technique, known as PICA (picosecond imaging circuit analysis),allows simultaneous acquisition of emission waveforms from many nodes within the field of view of a backside imaging system. Typical data from a CMOS circuit consists of a large emission peak at the time of a falling edge on the output of a gate; a much weaker peak is sometimes observable at the time of a rising edge. The IBM group has reported temporal resolutions of 30ps or better [*9] and has obtained good results on future process technologies such as SOI. The emission technique is completely noninvasive, as it is a passive probe. One drawback is that the emission is very weak, allowing detection of only about one photon per 106switching events. For long test patterns this can lead to acquisition times as long as several tens of hours. However, the long acquisition time is partially offset by the ability of PICA to obtain many waveforms in parallel. Another difference is that the emission waveform length can exceed several hundred nanoseconds while main500 yym1100wesr1.6705 μmdeley377/102vw.


taining its optimum time resolution, whereas laser probing gives a window of a few nanoseconds at the


||Laser Probing |PICA |
|---|---|---|

|invasiveness |negligible |none |

|voltage linearity |yes |no |

|parallel acquisition |no |yes |

|temporal resolution |< 30 ps |< 30 ps |

|waveform length at |2ns |>200ns |

|30ps resolution |2ns |>200ns |

|acquisition time (10us tester loop) |1-2 minutes |10 hours |

optimal time resolution.


Table 2 Comparison of laser probing and PICA


techniques.


Table 2 summarizes some key aspects of laser probing and PICA. The temporal resolution of the two techniques are comparable; the most obvious difference is the acquisition time. With a 10 µs tester loop, the laser probe typically requires 1-2 minutes to acquire a waveform. By contrast, acquiring a PICA waveform with the same tester loop length would require averaging for more than 10 hours. Loop lengths used in microprocessor analysis at Intel are often greater than 100 µs, making laser probing an indispensable technique.


Future Developments


Future challenges in the 0.13- and 0.10- micron process technologies are several. First, the trend for future microprocessors at Intel indicates that power dissipation for high-end server processors will continue to rise to 100W and higher as core frequencies climb into the multi-GHz range. Because


100 ps


of this, more advanced methods of chip cooling are sorely needed. Geometrical process scaling will continue to shrink diffusion sizes, which may make transistor access more difficult. To scale the laser spot size, a custom through-silicon immersion objective was designed. Fig. 11 shows a comparison in SRAM images taken under identical laser conditions with the standard 0.85 NA objective and the Intel immersion objective, which has a numerical aperture well above unity.


Figure 11 Comparison of imaging with the 0.85 NA lens used on the system with a new custom


immersion lens. The scanned range of the image is 20 microns.


The overall system-level challenge of minimizing system drifts and vibrations with a smaller laser spot will be considerable. Finally, novel substrate materials (SOI, etc.) may pose other challenges to the effectiveness of laser probing.


Conclusion


The development of through-silicon optical probing has led to a powerful new technique for circuit analysis and debug at Intel. With its excellent timing bandwidth and direct access to every signal on the chip, optical probing is delivering present results and has excellent prospects for scaling to the 0.13 micron process technology and beyond.


We would like to acknowledge the dedication and expertise of engineering teams at Schlumberger Diagnostic Systems and Checkpoint Technologies.


We also acknowledge sample prep-aration and validation hardware development groups at Intel.


1) M. Paniccia, T. Eiles, V.R.M. Rao, and W.M Yee, Proceedings of the International Test Conference, p. 740, (1998).


2) H.K Heinrich, Ph.D. Dissertation, Stanford University “A Noninvasive Optical Probe for


Detecting Electrical Signals in Silicon Integrated Circuits,” 1987; R.A. Soref and B.R. Bennett,IEEE J. Quant. Elect., QE-23, 1, 123 (Jan. 1987).


3) H.K. Heinrich et al., Appl. Phys. Lett., 48 (16),1066 (21 April 1986).


4) H.K. Heinrich et al., Microelect. Eng., 16, 313(1992).


5) N. Seliger et al., Microelect. Eng., 31, 87 (1996).


6) R.H. Livengood and V.R.M. Rao, “Focused Ion Beam Techniques for Debug of Flip Chip Integrated Circuits,” Semiconductor International, March 1998.


7) J.C. Tsang and J.A. Kash, Appl. Phys. Lett., 70,889, (1997).


8) J.A. Kash and J.C. Tsang, Phys. Stat. Sol. B, 204,507 (1997).


9) J.A. Kash et al., ISTFA ’98: Proc. 24thIntl.


Symp. on Testing and Failure Anal. (Materials Park, OH: ASM International), 483 (1998.)


10) J.A. Kash et al., IEEE J. Sol. St. Cir., 32, 3508(March 1998).


0.85 NA Lens


Intel Immersion Lens


20 µm


Electronic Device Failure Analysis Society, editor, p 35-38


DOI: 10.1361/cp1999istfa035


# Picosecond Imaging Circuit Analysis of the IBM G6 Microprocessor Cache


Picosecond Imaging Circuit Analysis of the IBM G6 Microprocessor Cache


Moyra McManus, Pia Sanda, Steven Steen, Dan Knebel, Dennis Manzer, Stas Polonsky


IBM T.J. Watson Research Center, Yorktown Heights, New York


Bill Huott, Steve Wilson, Tony Pelella, Yuen Chan


IBM S/390 Division, Poughkeepsie, New York


Picosecond Imaging Circuit Analysis (PICA) is a new technique shown here to be applicable to the analysis of complex VLSI circuits. PICA was used to diagnose a timing failure in the early design of the G6 microprocessor chip. The fault occurred at high frequencies upon consecutive writes. Using PICA,combined with programmable array built-in self test(RAMBIST) techniques, the problem was traced to a race condition in the write control circuits. This allowed timely correction of the design for product implementation.


Picosecond Imaging Circuit Analysis (PICA) [1] was used to diagnose an L1 cache timing fault which occurred in an early design version of the IBM S/390 G6 microprocessor. The microprocessor, built in IBM CMOS 7S technology with 0.2µm lithography and operating at 1.8V nominal, uses copper interconnects.


PICA, in conjunction with programmable RAMBIST [2,3] allowed observation of internal timings to find a race condition in the dynamic write control circuits which occurred when the cache was consecutively written. This resulted in rapid design correction, and ultimately, in a robust processor operating at high frequency. The PICA technique significantly reduced the total time spent debugging this problem to only about two weeks from start to finish. This paper will delineate the steps used, and the details of the analysis.


Method


PICA measurements were performed on a packaged chip with the substrate thinned to approximately 60 µm to minimize attenuation of the infrared (IR)emission through the doped silicon while maintaining a structurally and electrically sound module. The chip was socketed in a test board with the polished surface facing the imaging optics of the PICA system as shown in Figure 1. The backside of the chip faces a series of objectives on an IR microscope. The microscope is used to focus through the silicon onto the underlying circuitry, in this case a portion of the SRAM array and associated control circuits. The objectives provide the desired magnification. The capture is performed with a charge-coupled device(CCD) for the collection in the case of static detection of emission, and a microchannel plate photomultiplier detector for time resolved detection. Each detector is mounted on the microscope allowing for the physical alignment of the emission images over the microscope image of the chip without moving the test board and chip.


Imaging data are acquired of the emission from FETs of a CMOS circuit during switching [1,4-7]. The switching induced emission is therefore coincident with the electrical switching of the circuit and allows for its use in debug of timing problems in the circuitry. The imaging of the emission by a photomultiplier tube allows for the collection of data over the region of suspect circuitry. The off-line analysis of individual emission spots correlated to the design layout may then lead to the identification of the “bad” circuit.


PICA is the tool of choice in this case because it will allow for both the physical location of the failing circuitry as well as, in parallel, a full timing analysis of the circuits under investigation. [The technique has been described in full in the Conference Proceedings from the 24th International Symposium for Testing and Failure Analysis, in an article entitled Non-Invasive Backside Failure Analysis of Integrated Circuits by Time-Dependent Light Emission:Picosecond Imaging Circuit Analysis [4] ].


Figure 1 Picosecond Imaging Circuit Analysis


(PICA) system.


The test consisted of an infinite loop of write commands, possible using the programmable RAMBIST. The pattern was run at two periods:


1.5 ns, where the circuit was decidedly failing (fast),and at 2.2 ns, where it was passing (slow). The pattern was allowed to loop at each of these frequencies to acquire good CCD images of the suspect circuits. The same two tests were then run to provide good statistics for the PICA detector in order to view the timing behaviour of the suspect circuitry.


Results


The fault was identified by static emission microscopy to a region of the write control circuits.


This region glowed brighter when the fault was forced to occur by reducing the clock cycle. The CCD imaging at 40 times magnification (40X) of the chip under consecutive write conditions is shown overlaid on the corresponding physical design in Figure 2, for a failing (fast) frequency. In order to isolate the circuits of interest, the subtracted image(fast minus slow, with scaled acquisition times) is shown in Figure 3. The remaining emission is in the


region of the write control circuits, which seem to be“on” longer in the failing condition.


Figure 2 CCD image at failing frequency.


Figure 3 Resulting subtracted image.


PICA measurements were then used to derive the timing behaviour and the problem traced to a race between two signals to the write control circuits. A movie of the failure was made using 80X magnification in the region of the write control circuits. This visualization of the write control unit under a consecutive write test included two write control circuits (WCON) at the bottom of the image and the addressed wordline at the top of the frame, as is shown in Figure 4, taken at a passing frequency.


The pass gates of memory cells are visible, as well as


emission from the bit selector circuits. Figure 5 shows a frame of the movie taken at a failing frequency and shows the failing condition: emission is visible from the self-resetting WCON circuits as well as their reset delay chain (WCONRS). Timing analysis confirmed that the reset signal from WCONRS was on too long and collided with the forward path of WCON. This occurs at fast cycle times, but if the cycle is stretched, WCONRS is given enough time to finish, and the collision can be eliminated. The only other circuits seen in the emission image are the data out drivers (above the WCON emission) which are still active from the previous cycle at this fast cycle time.


Figures 4 Frames of PICA movie taken at a passing frequency.


The behaviour was quantitatively characterized using PICA waveforms [7]. Simulations of the delays in the reset circuit delay chain had predicted ample time for the switching of the outputs, and thus no timing collision between the WCON and WCONRS circuits.


The timing delays of the inverters which are suspected of causing the failure were extracted from the PICA data. The waveforms from individual inverters in the reset circuit delay chain are shown in Figure 6. The figure shows the waveform from the nFET of the first inverter of the chain (N84) as well as nFET n9. The delay from N84 to n9 measured by PICA is roughly 600ps which was found to be longer than the design target. Focused ion beam (FIB) repair verified the analysis and subsequent metal layer redesign produced a reliable solution.


Figure 5 Frame of PICA movie taken at a failing frequency showing emission from both the write control and write control reset simultaneously.


Figure 6 PICA waveforms showing the delay between two inverters.


In conclusion, PICA was used in conjunction with the unique S/390 programmable RAMBIST capabilities to efficiently resolve a timing fault which occurred during consecutive write cycles. The particular race condition found would have been extremely difficult to diagnose by conventional means. Identification of the circuit problem by PICA enabled a metal redesign allowing for on time delivery of the G6 product.


As microprocessors continue to grow in complexity,density and speed it becomes ever more important to have methods in place to analyze timing failures. We have demonstrated how PICA can play an integral role in the timing characterization and debug of a product level microprocessor.


Acknowledgments


The authors would like to thank Terrence Kane for his work thinning the chip. We gratefully acknowledge Mike Rosenfield, Paul Turgeon, Philip Wu, and Rocco Robertaccio for their continued support.


1) J.A. Kash and J.C. Tsang, Dynamic Internal Testing of CMOS Circuits Using Hot Luminescence, IEEE Electron Device Lett., Vol.


18, pp.330-332, 1997.


2) W. Huott, T.J. Slegel, T. Lo, P. Patel,Programmable Computer System Element with Built-In Self Test Method and Apparatus for Repair During Power-On, U.S. Patents 5659551 and 5805789, 1997.


3) P.G. Shephard III, W. Huott, P.R. Turgeon, R.W.


Berry Jr., P.Patel, G. Yasar, J. Hanley, F.J. Cox,Programmable Built-In Self Test Method and Controller for Arrays, U.S. Patent 5633877,


1997.


4) J.A. Kash, J.C. Tsang, D.R. Knebel, D.P. Vallett,Non-Invasive Backside Failure Analysis of Integrated Circuits by Time-Dependent Light Emission: Picosecond Imaging Circuit Analysis,Conference Proceedings from the 24th International Symposium for Testing and Failure Analysis, p. 483-489, 1998.


5) Dan Knebel, Pia Sanda, Moyra Mc Manus, J. A.


Kash, J. C. Tsang, Dave Vallett, Leendert Huisman, Phil Nigh, Rick Rizzolo, Peilin Song,Franco Motika, Diagnosis and Characterization of Timing-Related Defects by Time-Dependent Light Emission, Proceedings of the International Test Conference, pp. 733-739, 1998.


6) J.C. Tsang and J.A. Kash, Appl. Phys. Lett. 70,p.889-891, 1997.


7) P.N. Sanda, D.R. Knebel, J.A. Kash, H.F. Casal,J.C. Tsang, E. Seewann, and M. Papermaster,Picosecond Imaging Circuit Analysis of the POWER3 Clock Distribution, Digest of the IEEE International Solid-State Circuits Conf. 372,


1999.


Electronic Device Failure Analysis Society, editor, p 39-45


DOI: 10.1361/cp1999istfa039


# Electrical Probing and Surface Imaging of Deep Sub-Micron Integrated Circuits


Electrical Probing and Surface Imaging of Deep Sub-Micron Integrated Circuits


Kenneth Krieg, Richard Qi


Micron Force Instruments


Douglas Thomson, Greg Bridges


University of Manitoba, Canada & Micron Force Instruments


A contact probing system for surface imaging and real-time signal measurement of deep sub-micron integrated circuits is discussed. The probe fits on a standard probe-station and utilizes a conductive atomic force microscope tip to rapidly measure the surface topography and acquire real-time highfrequency signals from features as small as


0.18 micron. The micromachined probe structure minim-izes parasitic coupling and the probe achieves a bandwidth greater than 3 GHz, with a capacitive loading of less than 120 fF. High-resolution images of submicron structures and waveforms acquired from high-speed devices are presented.


The needle (or wire) probe and probe station have long been a mainstay in integrated circuit (IC) device characterization and failure analysis. The probe station provides a functionally flexible and mechanically stable platform for mounting the probe cards and manipulators needed to stimulate the device under test (DUT). Viewing of the DUT is typically performed with optical microscope mounted on the probe station.


This traditional probe station and needle or wire probe system has sufficed for many years to stimulate and measure signals from the internal nodes of integrated circuits. However, the size of the circuit elements comprising many present day IC’s is under


0.25µm and cannot be seen using probe station optical microscopes. Under an optical microscope,


even at substantial magnification, two 0.25µm devices, positioned 0.25µm apart, cannot be resolved.


Microelectronic circuit elements are typically of a size where optical imaging systems are no longer capable of the resolution needed to place probes on the measurement point of a DUT. Simply put, the


dimensions of microelectronics have shrunk below the size that can be imaged with optical imaging systems now on probe stations.


As the device geometry shrinks below 1.0µm, the large tip diameter of needle and wire probe pose significant electrical contact problems. For sub0.5µm circuit elements, contact with specific interconnect lines becomes almost impossible. As an example, Figure 1 shows a photomicrograph of a


typical etched-wire probe with a tip of 1µm in diameter and a set of three 0.5µm interconnect lines having 0.5µm


Figure 1 Typical 1µm etched wire probe near three


0.5µm interconnect lines.


spacing, using a Mitutoyo microscope with a 50X objective and 2X “zoom”. As one can easily notice,using even an etched wire probe of very small diameter, it is difficult to obtain a contact with only one of the metal traces. The situation worsens considerably when the interconnect or device size is


less than 0.5µm. To compound this problem, when contact can occasionally be made using traditional probe tips, the large capacitance and inductance associated with their size often changes the circuit characteristics, altering the true performance of the device or circuit. This effect is known as “probe loading” or “loading” of the DUT by the probe.


Numerous solutions have been proposed to eliminate the limitations of optical imaging and wire or needle probing for submicron IC’s. One of the most successful has been the electron-beam probing


technique [1]. This system combines imaging using a scanning electron microscope (SEM) with lowloading sampled electron-beam probing. Such methods are very expensive, require complicated preparation for the DUT (measurements must be performed in a vacuum system), require repetitive waveform stimulation, and have other limitations when the integrated circuit device size is less than


0.25µm. The repetitive sampling requirement of the


Laser source


Position sensitive


electron-beam probing method means that real-time


detector


events cannot be captured. An additional restriction of electron-beam probing methods is the inability to measure absolute voltage levels, which makes the technique difficult to apply to analog and mixedsignal IC’s.


Ideally, a solution to submicron imaging and probing would preserve the failure analysis industry’s investment in probe station technology. Users of probe stations often have considerable investment in customized add-on fixtures or instruments used to hold and stimulate samples, heat or cool the DUT,provide shielding for high-precision measurements,and provide special DUT environmental conditions.


There is also enormous cost associated with the software that controls and coordinates the probe station and these add-on fixtures/instruments.


Traditional probe stations are well configured to stimulate devices and mechanical probes are still useful when microelectronic devices have dimensions large enough to be imaged by probe station microscope systems. For many users, replacing their current probe station is a monumental task, causing major delays in the release of new products, and engendering significant development expenses.


The Atomic Force Microscope


Another method of visualizing submicron structures is to employ atomic force microscopy (AFM) or scanning probe microscopy (SPM) surface-imaging.


These techniques have achieved great success in providing images of nanometer and sub-nanometer structures in materials science, biology, chemistry,and physics applications.


The AFM senses interatomic forces that exist


between the probe tip and the substrate [1, 2, 3]. The AFM probe tip, which is similar in purpose to the phonograph stylus, is normally fabricated as part of a microfabricated silicon (Si) or silicon nitride (SiN)cantilever. In one method of operation, the probe tip is slowly lowered onto the substrate surface, with a computer monitoring the cantilever deflection. Once contact between the probe tip and the sample surface has been established, the probe tip is moved across the surface of the substrate in a raster pattern, while the vertical position of the cantilever is monitored.


Variations in substrate height (such as interconnects)cause the cantilever to deflect up or down. AFM imaging forces are normally in the 1-50 nanonewton range and cantilever displacement of less than 0.1nm can be measured. Figure 2 shows a schematic of a typical AFM cantilever and deflection sensing system.


Figure 2 Atomic force microscope motion sensing


using an “optical-lever” deflection measurement system.


In the AFM deflection sensing system, a laser impinges on the top of a reflective cantilever, the underside of which contains a micromachined tip. As the cantilever is deflected (for instance, by an IC interconnect, as shown in Figure 2) the angle of the laser reflection changes. This arrangement is known as an optical lever, since very small changes in cantilever deflection can result in large changes in laser position at the detector. A topographic image of the surface beneath the tip is generated by associating the deflection with the tip location, and displaying the result in a 2D or 3D format.


The extraordinary resolution of an AFM derives from its micromachined tip. A scanning electron microscope (SEM) picture of a typical AFM tip is shown in Figure 3. The single crystal Si or SiN fabrication process results in a tip whose final diameter is less than 10nm. Nanometer-scale tips are needed to obtain the resolution required for imaging and material characterization of deep-submicron IC structures.


Cantilever


Probe Tip


Figure 3 Scanning electron micrograph of a silicon AFM tip.


The AFM technique has been used extensively in microelectronic device characterization and failure analysis. In addition to the surface topography imaging abilities of the AFM, special-purpose conductive tips have been used to measure doping profiles (scanning resistance microscopy and scanning capacitance microscopy) and other material properties of semiconductor devices.


Despite its success in many device characterization and failure analysis applications, AFM technology has not been applied to probe station based testing.


This is because traditional AFM systems were designed to obtain resolutions well beyond 5nm and consequently were designed as large, highly-stable systems, whose size was as large or larger than a typical probe station. While such systems are ideal for obtaining measurements requiring high spatial resolution, they are incompatible with IC functional testing requirements.


The AFM Contact Probe


The analytical probe presented here applies AFM technology to the imaging and electrical probing of packaged parts and wafers on traditional probe stations. It enables the user to visualize the surface of the DUT with better than 50nm resolution and reliably obtain electrical contact with structures(interconnects and via plugs, for example) less than


0.5µm in size. The probe uses a conductive AFM tip to enable signals from the DUT to be captured in real-time. Its surface topography imaging capability can easily and quickly (under one minute) obtain pictures of deep-submicron structures on an IC with sufficient resolution to easily identify features of interest.


A significant challenge in the design of this AFMbased probe was assuring compatiblity with a wide variety of probe stations, prober-cards, microscopes and objectives, and other needle or wire probe manipulators. Figure 4 shows the probe mounted on the platen of a probe station with it probe tip positioned over a socketed device. The probe vacuum base and positioner is not much larger than a typical needle-probe manipulator and contains the cable connecting the probe with its controller. The base has manual adjustments for X and Y positioning.


However, to ensure the safety of the DUT and AFM tip, Z-axis motion is fully computer controlled.


A particularly important feature of the probe is its ability to access deep sockets or probe cards. To accomplish this, the AFM tip was located at the end of a long supporting structure. Figure 5 is an expanded view of the circled area of Figure 4,showing the tip portion of the probe. This figure also indicates another important feature of the probe design, optical access for the probe station mounted microscope. Though the probe can image the DUT surface to submicron levels, an optical microscopes is still useful for coarse placement of the probe tip and for placement of traditional needle- or wire-probes which can be used in conjunction with the AFMbased probe.


Figure 4 The probe mounted on a typical probe


station, with the tip portion circled.


Figure 5 Expanded view of the probe tip and DUT,


showing microscope objective optical access for


viewing DUT surface. Standard needle and wire probes


can easily be used in conjunction with the probe.


Deep-Submicron Imaging Capability


Surface imaging functions are designed to be simple and rapid, with sufficient resolution to easily locate


surface features much less than 0.5µm. Since the probe was intended to mount on a typical probe station, its imaging capability was not designed to be“metrology quality”. Therefore, image resolution is 50nm, which is far better than necessary to discern


two 0.18µm interconnect lines from each other in order to place the probe tip. The default imaging area


is 40µm x 40µm and an image of the surface area is generated in under one minute.


An example of a 40µm x 40µm scan is shown in Figure 6. This is a screen-capture of a scanned image from the user interface of the probe control software.


The DUT shown is an electron-beam test sample [5],


the brightly shaded regions are 0.5µm thick sputterdeposited aluminum alloy (99% Al/1% Si). The


Focus sensitivity


The signal strength is extremely sensitive to focus position. Furthermore, the optimal signal is not necessarily obtained at the best visual focus, but when the object is slightly defocused. For instance, in the test chip measurements the optimal signal on the gate protection diode of Fig. 1c was obtained when the focal position was moved about 1µm from the sharpest focus of the diffusion region. Once the optimal focus has been determined, a recipe for subsequent probing can be followed. In addition, as mentioned earlier, an aberration correction ring must be adjusted to minimize spherical aberration caused by transmission through the silicon substrate.


Voltage Measurements


It is currently not possible to calibrate absolutely the output amplitude of the IDS 2000 in terms of signal voltage because the signal amplitude depends strongly on focus and spot position, device geometry, and details of the manufacturing process. However, for a given probe position the signal is nearly linear in voltage [10],so risetime and other relative voltage measurements can be accurately made.


Waveform Inversion


As discussed in the theoretical section of this paper, the signal measured by the IDS 2000 is a combination of absorption and refraction effects. The absorption effects always give rise to a well-defined signal sign relative to the applied voltage. The refraction effects, however, are converted into amplitude modulation by a number of mechanisms.


One mechanism whereby waveform inversion has been observed involves the focus adjustment. The waveform inversion (phase change) can occur when one goes from being overfocused to underfocused. This is due to how the index of refraction changes the focal position, hence signal amplitude, on the pin hole of the confocal microscope. An example of this effect can be seen when comparing Figs. 1 and 2. Both waveforms were obtained from n+ gate diodes but Fig. 1 waveforms are not inverted while Fig. 2 waveforms are inverted. The waveforms in Fig. 1 were obtained when the image was underfocused (focused further into the substrate); Fig. 2 waveforms were obtained when the image was overfocused.


As expected, waveform inversion is also observed between waveforms from a p+ in Nwell and n+diffusion in p-substrate (assuming the same focal position and no unusual interference effects) of a transistor. The inversion occurs because the polarity of the electric field is inverted between the two types of diodes. This effect occurs regardless of absorption or refraction effects. An example of this type of inversion will be shown later in the “improved results” section.


In practice, techniques (e.g., pulse stretching, duty cycle changes, etc.) can be adopted which eliminate uncertainty in the waveform polarity arising from the above effects.


System Bandwidth


The system bandwidth is intrinsically very high. The contributions to system bandwidth are the laser pulse width (35 ps FWHM), the jitter in the phaselock circuit,


and photodiode pulse output (~15 ps RMS) to give a combined system bandwidth of ~8 GHz. As mentioned earlier, the IDS 2000 timebase board locks the laser clock to the tester clock. Although the jitter in the phaselock circuit is very low, the jitter in many testers can be very large, if it is even specified. In practice the jitter in the tester is the limiting factor in the system bandwidth.


Laser Intrusion


Since the photon energy (1.17eV) of the 1064nm wavelength laser is slightly above the bandgap energy of silicon, the laser is capable of generating electron-hole pairs in a circuit. Figure 3 shows the amount of induced photocurrent observed on the protection diode of Fig. 1.


As has already been mentioned earlier, the IDS 2000 has a reference laser and probe laser, both of which are at 1064nm. One curve from each laser is plotted in Fig. 3.


Photocurrent, typically in the nanoamp range, is observed from both lasers. Normally, this is not enough current to effect the waveform timing noticeably in circuits unequivocally biased (i.e., non-floating nodes);however, in pre-charged floating memory cells, a correlation has been observed between the laser power and the pulse width and timing of the discharge (read cycle). More studies, particularly of new technologies,are needed.


Gate Diode Leakage vs. IDS2k Laser Power


0*量 1


Photo-Current (nA)5


IDS2k Incident Photo-Detector Voltage


Reference Probe


Figure 3 Average diode current leakage resulting from


the IDS 2000 lasers. The diode in this measurement was


a gate protection n+ diode for a 0.25µm n-channel


transistor.


Incident and Reflected Light: Proper Balance


For optimal signal to noise, a proper balance of reflected and incident light intensity is needed, as indicated by the photo-diode detectors, for both the probe and reference lasers.


The IDS 2000 requires a certain range of incident and reflected power. In some applications it may be necessary to adjust the gain of the photodetector


amplifiers. For example, in a highly reflective device the incident power may be small while the reflected power may be much higher than optimal.


The front-end photodetector amplifier is an extremely


拾N41


low-noise circuit and does not lend itself well to conventional remote gain control techniques. However,it is relatively easy to modify the gain resistor with a set of jumpers and, once set, should prove suitable for similarly prepared samples.


tN


Laser Damage


When tuning the modelocked probe laser cavity, the


output laser power can become very high. As a result,t


性


damage to protection diodes such as used in Fig. 1 have been observed; in addition, some circuits have been made non-functional after tuning the laser. Hence, it is imperative to be careful where the laser is placed during a cavity tuning process.


Improved Results from a Flip Chip Microprocessor


By paying close attention to all the details just described,a significant improvement was obtained in the signal strength. The improvements are demonstrated in Fig. 4 on the microprocessor. In particular, note that the vertical scale in this figure has been increased to 1000 ppm/division (Fig. 2 was 200 ppm/div.). Signals of this caliber are now more typical of what is obtained from a probing session.


Figure 4 actually shows the results from two different units: one is a passing (labelled “Good”) unit while the other one is a failing (labelled “Bad”) unit. This is most evident when comparing the “good” and “bad”waveforms for data lines D1 and D5, respectively, in Fig. 4. The bad unit has an additional unexpected pulse~30ns wide in it; subsequently, the timing of the output pulse for the bad unit is also incorrect.


On a final note with regard to waveform inversion from different type diffusions, the data lines, D1 and D5, and the output waveforms were taken from n+ diffusions.


With the image overfocused, as in Fig. 2, the waveforms were inverted. However, the clock pulse (pclock, sc1,and sc1) waveforms, also overfocused, were obtained from p+ diffusions (in Nwell)—these waveforms are not inverted.


pclock


m


Output : Good


《Awn  D5 : Good


D1 : Good  temntkapttoerwetgnip七sodna  sc2


bat9x清


Ww女，党


sc1


Output : Bad


Antsngwywnd  D1 : Bad


D5 : Bad


hir


juthWiu


1000 ppm/div 20 ns/div 191.5 µs delay 8/2048 avg.in


ADVANCED MICRO DEVICES


Figure 4 Improved waveform results for the flip-chip microprocessor. Note the vertical scale on this plot is 1000 ppm per division as compared to 200 ppm per div.


in Figure 2. A comparison is also made between a good


(passing) and bad (failing) unit: especially note the


differences in the “good” and “bad” waveforms for the data lines D1 and D5, respectively.


A novel backside waveform acquisition tool (IDS 2000)from Schlumberger, based on electro-optic sampling,has been demonstrated. Waveforms were initially obtained from a backside test chip, then demonstrated on a flip chip microprocessor. Many issues and challenges with the system have been noted. Improvements in these areas have led to greatly improved system performance.


Acknowledgment


The authors would like to thank the following individuals for their support: Rick Johnson, Mike Dobrovolski, Brennan Davis, Matt Thayer, Jeff Birdsley, Glen Gilfeather, Lee Rusk, Bill Boothby, Ken Kuchar, Rama Goruganthu, Danny Stone of Advanced Micro Devices; Dan McCollom and Rajesh Jain of Schlumberger.


1) M. Paniccia, E. Eiles, V.R.M. Rao, and W.M. Yee,“Novel optical probing technique for flip chip packaged microprocessors,” Proceedings of the 1998 International Test Conference, p. 740 (1998).


2) B.R. Hemenway, H.K. Heinrich, J.H. Goll, Z. Xu,and David M. Bloom, "Optical Detection of Charge Modulation in Silicon Integrated Circuits Using a Multimode Laser-Diode Probe", IEEE Electronic Device Lett. EDL-8, 346 (1987).


3) H.K. Heinrich and D.M. Bloom, Method and means for optical detection of charge density modulations in a semiconductor, United States Patent 4,758,092.


Stanford University (1988).


4) H.K. Heinrich, D.S. Kent, and L.M. Cropp,"Backside Optical Measurements of Picosecond Internal Gate Delays in a Flip-Chip Packaged Silicon VLSI Circui," IEEE Photonics Techn. Lett.


3, 673 (1991).


5) H.K. Heinrich, N. Pakdaman, J.L. Prince, D.S.


Kent, L.M. Cropp, "Picosecond Backside Optical Detection of Internal Signals In Flip-Chip Mounted Silicon VLSI Circuits," Microelectronic Engineering 16, 313 (1992).


6) G.N. Koskowich, Voltage measurement in silicon and gallium-arsenide technologies using optical phase modulation, Dissertation, University of Washington (1988).


7) G.N. Koskowich and M. Soma, "Optical Charge Modulation as an Internal Voltage Probe for CMOS IC's" IEEE J. of Quantum Electronics 24, 1981(1988).


8) L.V. Keldysh, "The effect of a strong electric field on the optical properties of insulating crystals,"Soviet Physics JETP 34, 788 (1958).


9) R.A. Soref and B.R. Bennett, "Electrooptical Effects in Silicon," IEEE J. of Quantum Electronics QE-23, 123 (1987).


10) M. Paniccia, R.M. Rao, and W.M. Yee, "Optical Probing of flip chip packaged microprocessors," J.


Vac. Sci. Technol. B 16, 3625 (1998).


Electronic Device Failure Analysis Society, editor, p 27-33


DOI: 10.1361/cp1999istfa027


# Optical Probing of VLSI IC’s from the Silicon Backside


Optical Probing of VLSI IC’s from the Silicon Backside


Travis M. Eiles, Gary L. Woods, and Valluri Rao


Intel Corporation, Santa Clara, California


Non-invasive internal circuit node waveform


acquisition is a critical part of design debug and failure analysis at Intel and in the rest of the semiconductor industry. In the past, the most widely used technique for non-contact probing has been


electron-beam probing of metal lines from the front side of the die. With the advent of C4 packaging technology, Intel has developed, in conjunction with a technology partner, an integrated, laser-based


↓


optical backside probing system. This system has been proliferated at Intel and has been used for


CMOS circuit diagnosis on a number of products [*1].


In this paper we will describe the basic system operation, the electro-optic effect in silicon which is used for the signal acquisition, and then the entire probing environment. We will then discuss recent results and present a comparison with other waveform acquisition techniques. We will conclude with a brief discussion of developments needed to scale the technique to future processes.


System Operation


The optical probing system utilizes a compact modelocked (ML) diode-pumped Nd:YAG laser with a


1.064 µm wavelength as the light source for imaging and signal acquisition. This laser has several essential characteristics: (1) a wavelength tuned to correspond to the silicon bandgap, yielding both (a) substantial transmission through a doped substrate while maintaining as good a diffraction-limited spot size as possible and (b) the maximum electro-optic effect in silicon; (2) short pulses (~35 ps) for high sampling bandwidth, and (3) ultra-stable, low-jitter oscillation performance required for excellent timing resolution and accuracy.


Figure 1 Phase-locked loop circuit used for optical


probing. The inputs are the tester clock and trigger.


The circuit synchronizes the ML laser oscillation


frequency (100 MHz) with an arbitrary test


frequency. Variable timing delays and single pulse


picking are used to deliver the laser pulse at the


proper instant for stroboscopic sampling.


The laser’s natural output pulse frequency of 100 MHz is not directly compatible with probing microprocessors executing typical test patterns. This is because test patterns are exercised with clock frequencies that are fine-tuned for the circuit behavior that needs to be diagnosed. Because of this,a phase-locked loop (PLL) circuit is used (Fig. 1) to maintain synchronicity between the 100 MHz laser and the tester running at an arbitrary frequency. The PLL also controls optical modulators which blank all but a single pulse every test loop, so that this lone pulse is delivered to the sample at a precise point in time relative to the tester pattern (see Fig. 2).


Phase


Comparator


Variable


Phase→Delay


100 MHz VCXO


Tester


Clock↓FrequencyDivide-by-M→FrequencyDivide-by-N


ML


Laser


Variable>Delay


Trigger


→Feedback


Optical Modulator


Figure 2 Timing diagrams of the (A) tester clock, (B)


circuit voltage waveform to be collected, and (C) the probing pulse. The pulse is “walked through” the time sweep of interest to sample the averaged


waveform stroboscopically.


The waveform is sampled many times at each time step and then averaged. The laser pulse is then phase-shifted by precise delay generators in the timing circuit to move the pulse to the next time step.


In this way, the waveform is built up stroboscopically as the microprocessor is operated in a continuously repetitive test loop and the laser pulse is swept through the entire time region of interest. The magnitude of the time step depends on the total time region of interest, and can be as small as 1 ps.


Timing accuracy is on the order of 10 ps and system bandwidth corresponds to the 35 ps laser pulse width and negligible electronics jitter. The user interface is similar in form and function to those on industry standard electron-beam probing systems, and includes an oscilloscope-like waveform acquisition window.


To allow access to sub-micron features, along with high-resolution imaging for navigation, the laser pulse is delivered to the sample through a diffractionlimited confocal laser scanning microscope (LSM)modified for signal acquisition. The scanning mirrors of the LSM are used to generate a raster image, as well as for directing the beam to the desired probe point within the field of view. An infraredcompatible microscope objective (0.85 numerical aperture) with aberration correction for throughsilicon focusing is used to create a sub-micron laser spot. Transistors fabricated using Intel’s 0.25 and


0.18 micron technologies are readily visible in the LSM image. The LSM is also custom designed for low-noise optical signal collection. A simplified system schematic is shown in Fig. 3.


Figure 3 Simplified schematic of the optical probing


system. The x-y-z stage and LSM are rigidly


attached to the DUT and vibrationally isolated from the environment.


Because of the small signal levels and high-resolution imaging (leading to a small depth of focus), mechanical vibration levels on the order of even a few nanometers would be disastrous for signal acquisition, as the modulation of the reflected signal would be dominated by these non-periodic,vibrationally-induced fluctuations. A vibration cancellation technique was developed to greatly reduce these effects. A low-power, continuous-wave laser(again diode-pumped Nd:YAG operating at 1064 nm wavelength) is modulated to form a wide pre-pulse(~150 ns) which is applied at a fixed time relative to the tester pattern, while the probing pulse is swept in time. The “reference” pulse traverses the same optical path, including the optical fibers connected to the LSM inputs and outputs, as the probe pulse.


Taking the ratio of the probing laser reflectivity to the reference laser reflectivity allows the slowly varying(~100 Hz) vibrational fluctuations to be removed from the processed signal. The ratio technique is sufficient to cancel out noise due to the level of mechanical vibrations (+/- 75 nm) that are often experienced by the sample. However, this technique makes it impossible to measure steady state high or low signal levels, as is possible on e-beam probing systems due to the stronger voltage contrast signal.


Both the probe and reference lasers, with their optical modulators and beam-combining optics, are placed on a modular optical table inside the prober head.


The output is then fiber-coupled to the LSM. The LSM is moved on a precision stage. Reflected signals in the LSM are fiber-coupled to a sensitive photodiode and amplifier circuit. The analog signals are digitized and then processed and displayed on the oscilloscope window.


Test loop


Tester period


10 ns


B


C→


Tester Laser


1.06um


PLL


Pulse Picker


Detector王


Fiber


Vibration Isolation


LSM


XYZ stage DUT


GUI


Electro-Optic Effects in CMOS Probing


Laser probing makes use of an ultra-fast electro-optic effect that modulates both the phase and amplitude of the focused light reflecting from transistor diffusion.


In silicon, the electro-optic effects are chiefly free carrier modulation and the Franz-Keldysh effect. The free carrier modulation depends on the density of


Typical Wevelorms


injected carriers, while the Franz-Keldysh effect depends on the electric field. Table 1 displays the


1000 ppm/di1 mn/diw 2.9016 us delay0/32 .


various electro-optic effects and the ways in which they can modulate light transmission [*2].


||Phase modulation |Absorption modulation |
|---|---|---|

|Electric Field |Electro- refraction |Franz-Keldysh effect |

|Carrier Density |Plasma- |Free carrier absorption |

|Carrier Density |optical effect |Free carrier absorption |

Table 1 Electro-optic effects in silicon. The vertical column distinguishes the cause of the electro-optic effect (Electric field or carrier density); the horizontal row separates the way the effect modulates the light


(phase or amplitude modulation). Measurements


indicate the predominant effect in advanced Intel


CMOS processes to be the plasma-optical effect.


Observations of the dependence of the modulated signal on various experimental conditions have yielded clues as to the dominant effect. First, we have performed interferometric experiments to demonstrate that phase modulation dominates over the absorptive component. The interferometric apparatus will be described in a future publication. A smaller residual amplitude-modulation effect remains. The electric field-driven modulation due to the FranzKeldysh effect is a simple explanation for how the reflected signal is modulated by the potential, and thus the electric field, on transistor diffusion.


However, measurements have shown that the optical modulation tends to increase as the laser power is increased. This non-linear effect demonstrates that free carrier modulation is the stronger of the two effects in the laser power range available in the probing system. The question of invasiveness of these photo-injected carriers is discussed below.


The optical modulation measured by the system is a ratio of reflected signal over the incident signal, and is displayed on the user interface as the dimensionless modulation in parts-per-million (ppm).


Excellent signals are available in a short averaging time (1-3 minutes). A voltage calibration to the optical modulation has proven to be very focusdependent and hence not sufficiently reproducible,and the system is thus not used for accurate analog voltage measurements in which an a priori ppm-tovoltage calibration is required. However, we have found that, for a given focus, the signal is linear in the applied voltage. It is in timing measurements where the system has proven to be invaluable. An example is shown in Fig. 4, showing the optical modulation (in ppm) plotted against time for the sampled waveform.


Figure 4 Typical optical probing waveforms


acquired on a 0.18-micron process.


Photocurrent invasiveness


Laser probing of integrated circuits has been explored since the mid-1980s [3-5]. Most of the previous work has concentrated on using lasers with a 1.3 µm wavelength, which is longer than the onset of silicon interband absorption at about 1.1 µm. However, our system uses a laser at 1.064 µm, which is short enough to generate a significant amount of photocurrent, potentially leading to inaccurate probing results due to invasiveness. We expected the effect to be most pronounced on low-capacitance nodes,where the laser photocurrent would dominate the current drive capability of the transistors.


A study of the effects of photocurrent shows that the laser pulse does not lead to inaccurate probing results for a wide range of nodes being probed. As a first evidence of this, we examined the timing of an edge from a low-capacitance node. We found that the edge timing was essentially independent of laser probe power, for a wide range of powers up to the highest available in the instrument (Fig. 5).


chanckyotw


-100


>200ps<


Transition edge [ps]-500


①


O0


-0


100


5 10 15 20 25 30 35 40 Laser power [arb.]


n-channel


Figure 5 Transition edge shift as a function of laser


power applied to a low-capacitance circuit node. The large error bars are due to uncertainty in transition


point due to the noise on the acquired waveform.


The laser power range is typical for that used in the optical probing system.


At the highest laser level, we estimate the peak power density of the probe laser to be around 500 MW/cm2.


The effects of photocurrent depend on the type of device being probed, i.e., NMOS or PMOS. For the former, the laser pulse can be modeled as a pulsed current source between the drain and Vss, while for a PMOS transistor the pulse can be modeled as a current source between the drain and Vcc. These are shown in Fig. 6. For a falling edge on the output of the inverter, probing the NMOS (PMOS) will tend to move the transition edge earlier (later.) However, we observe essentially no difference in timing between the edges of waveforms acquired on NMOS and PMOS transistors, even when probed at the highest powers available. Fig. 6 shows a pair of waveforms from such a pair of transistors.


Vout


Vin


0Vcc00


古Vss


Vcc


=Vss


b


↑


Figure 6 Circuit schematics for a CMOS inverter (a)


photocurrent induced when probing a p-channel


diffusion, charging the node, and (b) photocurrent induced when probing an n-channel device,


discharging the node. Data collected on the output p- and n-diffusion show no perceptible timing shift,


indicating the lack of invasiveness on waveform acquisition for the probing laser


Probing Environment


The C4-mounted microprocessor is mechanically thinned and polished by standard industry practices,after which an anti-reflection coating is applied to the polished silicon to reduce the 31% Fresnel loss at the silicon/air interface. The global thinning is necessary to achieve the required laser transmission incident on and reflected from the probe point. These sample preparation methods have a very high success rate,and are completely non-invasive to the electrical behavior of the microprocessor. The time required for the complete sample preparation process is less than three hours. The thinned processors are run at full frequencies with a range of standard industry debug testers. The sample, socket, and test board are electrically coupled to the debug tester by a lowvibration cable interface, but are mechanically anchored to a floating table which supports the sample assembly and the microscope stage. The backside of the chip then faces down, and is probed from beneath as with other direct-dock probing systems (Fig. 7). The precision stage is vibrationisolated from the floor, and vertical sample vibration levels as small as +/- 75 nm are achieved, even with the system located on “noisy” industrial test floors.


Figure 7 Schematic of the fixturing used in laser


行MN


pass


Navigation to the desired transistor location is done using the backside LSM image and automated linking


美y广


to the backside CAD layout databases (Fig. 8). The


fail


complete setup time is about one hour or less.


h


Figure 8 Backside through-silicon LSM image, and


corresponding backside layout database. P- and n-


可


channel transistors are clearly apparent, as well as shallow trench isolation features.


季


Since microprocessors dissipate power during testing,the probing environment must allow for control of


差


the temperature of the chip. The Intel C4 process


imW0


heg


using high-performance organic land grid array(OLGA) packages requires us to make special effort


the


in designing the thermal solution platform. The


won


dominant thermal path for heat removal from the chip is from the exposed surface of the silicon. Because of the short depth-of-focus with the high-resolution lens,slight thermal expansion in the package makes proper laser focusing difficult unless a very stable thermal control system is applied. To cool the die, a copper heat spreader is firmly pressed against the silicon,with a thermally conducting material interposed between two for improved heat conduction. This leaves portions of the die covered for thermal contact,while other portions are exposed for probing visibility. The cooling plate is thermally anchored to


a heat exchanger fixture through which constanttemperature air is circulated. Temperature gradients of several degrees-C/W are often observed between the hot spot on the silicon and the thermal reservoir.


These large temperature differences are due to the global die thinning which restricts the cross-sectional area for heat flow. For most IC’s this is sufficient for acceptable thermal control.


Literally thousands of waveforms have been acquired on several Intel microprocessors and memory chips on both the 0.25- and 0.18-micron Intel processes.


Examples are shown in Fig. 9.


Figure 9 Typical waveforms taken during debug of


an Intel microprocessor on a 0.18-micron process.


Waveforms marked “pass” and “fail” are acquired when the DUT is registering those test conditions.


Acquisition times are typically 1-3 minutes for acquiring high quality waveforms. Test loop lengths are routinely between 50 and 300 µs. However, on several occasions, high quality waveforms were acquired with test loops as long as 1 ms. Both n- and


Cable


Interface


Board &


Socket


Microscope Objective


AR coating


1009ai-2一1-22MnrtILSdolay0/2046v


Thinned DUT


C4


Package


Laser Beam Cu Heat


Spreader


p-diffusions are probed successfully, giving optical probing access to every circuit node on a chip. More extensive averaging is done if the best possible signal-noise ratio is required for high-precision timing measurements. Crosstalk (picking up unwanted signal from a neighboring diffusion when probing) has never been observed, even on nearminimum diffusion spacing in advanced CMOS processes.


three interconnect structures have 0.5µm linewidth and 0.5µm spacing. Even at this “low-magnification”the imaging capability far exceeds that obtainable from an optical microscope (see Figure 1 for comparison).


Surface visualization and electrical probing are performed using the same image. To make electrical contact with a feature in a displayed image the user simply clicks the mouse at the position where the contact is to be made.


Figure 6  640µm x 40µm Real-Time AFM probe


image of three 0.5µm Al interconnect lines having a


0.5µm spacing.


To ensure accurate placement of the probe-tip and obtain more detail of the DUT region of interest, the probe software enables the user to “zoom” the display to show a smaller region in greater detail.


This “zoom” is not simply a software rescaling of the already captured image, but a physical zoom of the desired region, providing the capability of showing features in much greater detail.


For instance, Figure 7 shows a “zoom” of the interconnect corners in the previous image to an


8µm x 8µm size. Note that at this resolution, one can clearly see sub-0.1µm surface details. On the user interface of the probe control software, such an image might be displayed in a 6 inch x 6 inch window,allowing great ease of probe placement on submicron features.


The forces used during surface scanning (imaging)are so small that hundreds of scans of the same area can be performed without damage to fragile submicron metalizations. This is a dramatic improvement over traditional needle or wire probes, where the large contact forces can cause significant damage to the submicron DUT features.


Figure 7 8µm x 8µm “zoomed” image of the interconnect corners from Figure 6. The image


was generated by rescanning the surface at


higher resolution.


Electrical Probing


600


The probe accepts a variety of tip assemblies designed for specific probing tasks. Tip assemblies


400


are easily replaceable and plug into the front of the


200


probe. Among the tip assemblies available are:precision low-frequency, low-leakage, 300 MHz low-


人0


loading active buffer, and a variety of RF and


microwave passive-divider assemblies. Low-loading


-200-


(high resistance, very-low capacitance) tip assemblies with bandwidths beyond 1GHz are planned. Figure


-400


8 is a schematic illustration, showing electrical


-600-


probing of a submicon interconnect. The box labeled“Passive/Active Electronics” indicates that the tip


24.624.825.025.225.425.625.826.0


assembly can contain a variety of electrical contact


Time (nsec)


signal conditioning. Similar to traditional probes the output is directly connected to the users test equipment. Since the AFM tip is extremely small, its capacitive loading to the DUT is corresponding small. The active probe assemblies have less than 100 fF loading at the probe tip.


Examples of the high-speed digital and microwave electrical probing capability of the probe are provided in Figures 9a and 9b. For this test, a 120ps risetime


pulse stimulated a 50 Ω 1mm microstrip transmission line. The probe tip assembly used was a 40:1 passive


voltage divider (using a 2KΩ divider-resistor). The probe output was connected to a Tektronix SD26 sampling head (20GHz BW, 17.5ps rise-time) on a Tektronix 11801B oscilloscope. Figure 9b shows the signal measured with this probe tip assembly. The through-line test structure also enables the stimulus signal to be measured directly by the oscilloscope for comparison. The measured stimulus is shown in


Figure 9a. These measurements clearly show that the rise-time measured using the probe (Figure 9b) is equivalent to that of the stimulus (Figure 9a).


Figure 8 Diagram of probe signal path. The probe provides signals that can be connected directly to the users test equipment.


Figure 9a 120ps risetime pulse measured directly from signal generator and applied to the test


structure.


An example of the low-loading active probe response provided in Figure 10, using a 300MHz 40:1 active


probe-tip assembly. For this measurement, a 50Ω coplanar transmission line was stimulated with a 250Mb/sec clock waveform. As can be seen from Figure 10, the measured rise-time is actually slightly better than that provided by a 300MHz BW.


Figure 11a shows a 200Mb/sec 8-bit pattern measured using the 300MHz 40:1 active divider probe on the same coplanar transmission line. For comparison,Figure 11b shows the same signal measured using a Tektronix SD14 active probe (3GHz BW) at the same point on the transmission line.


Active/Passive Electronics


40.0


20.0


10.0


0.0


人-20.0


E-10.0


-40.0


-20.0


-60.0


-30.0


-80.0


26.626.827.0


27.227.427.627.828.(


70.080.090.0100.0110.0120.0130.0 V7


Figure 9b Measured signal using a passive 40:1 divider probe tip assembly (2KΩ input resistance).


Figure 10 Response of the 300MHz 40:1 active divider probe tip assembly, stimulated by 250Mb/sec clock signal.


Figure 11a Measured signal using a 300MHz 40:1 active divider probe tip assembly, stimulated by a 200Mb/sec, 120ps rise-time bit pattern [10101110].


3.0


2.0


6^


mV10


VoltsE


个


-1.0


-30


-2.0-


-50


70.075.080.085.090.095.0 Time (nsec)


50.060.070.080.090.0100.0110.0


Figure 11b Measured signal using a Textronix SD14


active probe (3GHz BW), stimulated by same


200Mb/sec pattern.


Summary and Conclusions


A new submicron contact probing system designed for surface visualization and real-time signal measurement of deep sub-micron integrated circuits was discussed.


This analytical-probing tool, based on atomic force microscopy technology, extends the capability of traditional probe stations to deep-submicron integrated circuit technology. Images were presented showing the probe’s capability to image DUT surface


structures well below 0.5 µm. High-magnification probe images of interconnect structures were show indicating better than 50nm image resolution.


The probe can be equipped with various tip signalconditioning tip-assemblies including precision lowfrequency tips, and passive and active, low-loading /high-frequency tips. Electrical measurements from


the probe were presented showing ≥ 3GHz bandwidth for a 40:1 passive-divider probe (2K input resistance)


and ≥ 300MHz performance for a low-loading activedivider probe.


1) J. Thong, Electron Beam Testing Technology,Plenum Press, New York (1993)


2) G. Binnig, C. F. Quate, and Ch. Gerber, Phys.


Rev. Lett., 56, 930 (1986)


3) G. Binnig and D. P. E. Smith, Rev. Sci. Instrum.,57, 1688 (1986)


4) J.F. Grifith and D.A. Grigg, J. Appl. Phys., 74,R83 (1993)


5) H. Richter, Test Chip for the Characterization of Electron Beam Measurement Systems, Microelectronic Engineering, 16, 225-232 (1992


Electronic Device Failure Analysis Society, editor, p 49-55


DOI: 10.1361/cp1999istfa049


# Comparative TDR Analysis as a Packaging FA Tool


Comparative TDR Analysis as a Packaging FA Tool


Charles Odegard


DSP Solutions Packaging Development, Texas Instruments, Dallas, Texas


Craig Lambert


Application Specific Products, Test Technology Center, Texas Instruments, Dallas, Texas


Time domain reflectometry (TDR) is increasingly being utilized as a failure analysis tool in the semiconductor industry. TDR can provide fast,nondestructive analysis of packaged integrated circuits. With one measurement, TDR analysis can provide instant identification of the general region of the fail site, whether it exists in the substrate,interconnect region, or in the die. A digital sampling oscilloscope with a TDR module supplies a fast risetime voltage edge to the signal pin of interest, and then records the subsequent voltage edge reflections.


The time delay between the incident and reflected electrical signals are analyzed to characterize the electrical path of the signal pin. Initial implementation of TDR as an FA tool by the authors was in a comparative analysis method, where the TDR measurement from an unassembled substrate is used as the basis of comparison for the TDR measurement from the failing unit. Current development focuses on signature analysis of the TDR waveform for a given substrate path (including BGA substrate, flip-chip solder bump and pads, and flip-chip die). Interpretation of the TDR measurements for both comparative analysis and signature analysis of the TDR waveform will be discussed in this paper.


Packaging failure analysis encompasses a broad range of potential failure mechanisms that can occur in any of the three main regions of the packaged device, including the die, the substrate, and the interconnect region. Failure can occur as a result of a processing flaw, such as in the manufacturing of the package substrate or the integrated circuit. Failure can also occur during package assembly, such as misplaced or missing solder bumps in flip-chip devices, or shorting of adjacent wires in a wirebond


device. Finally, failure may be induced during reliability testing, often related to a marginal assembly or processing step.


With such a large group of potential failure mechanisms, it would be useful to have a fast,nondestructive method of isolating the failure to one of the three main fail sites: the die, the substrate, or the interconnect region. Subsequent analysis could then focus on the appropriate fail site region and significantly reduce the FA cycle time by eliminating the analysis of areas that are not the fail site regions.


Currently, the two nondestructive techniques that are used for initial fail site isolation are scanning acoustic microscopy (SAM) and real time x-ray (RTXR)analysis [1-3]. Commercially available SAM equipment can resolve defects such as nonwetting solder bumps in flip-chips, die cracks, and delaminations between interfaces. However, resolution constraints and absorption or scattering of signal often prevent identification of sub-micron defects in the die or interconnect region, or larger than micron size defects in some laminate substrates.


Commercially available RTXR equipment can


resolve defects as small as 1-3 µm, but only within a limited power range (less than 20 watts).


Consequently, some defects requiring large tilt angles and higher power to penetrate greater specimen thicknesses may not be detected with RTXR analysis.


Resolution and absorption constraints also prevent identification of sub-micron cracks at the bump/pad interface or within the die metallization layers. This paper shows that time domain reflectometry (TDR)can be used as a nondestructive technique that is complementary to SAM and X-Ray analysis.


The fundamentals of time domain reflectometry are described in application notes and equipment manuals from the manufacturers of TDR equipment[4-6]. TDR is a method of characterizing an electrical


path by sending a step function voltage into the path and monitoring reflections that return from the end of the path, or partial reflections from elements along the path [4-6]. The time delay between the incident and reflected electrical signals is analyzed to characterize the electrical path. It is a mature technology that has traditionally been used for determining fault location of cables (coaxial and twisted pair) and other transmission lines [6-9].


Since the velocity of propagation of the electric signal along the transmission line depends on the dielectric constant of the material surrounding the transmission line, TDR has also been used to characterize systems based on their dielectric property [11].


The use of TDR in the microelectronics industry is not new. TDR has been used to characterize transmission lines in packaged IC’s [12-14]. As a packaging FA tool, TDR can be used to characterize whether a signal pin is an open or short-circuit, and measure the length of the electrical path.


Discrepancies between the measured and expected characteristics of the electrical path could then lead to identification of a fault location. Only a decade or so ago, commercially available TDR equipment had slower rise times, in the range of 50 picoseconds or more. Recently, the convergence of commercially available TDR equipment with fast rise times (less than 35 ps reflected rise time, 10% to 90%) and longer path lengths in chip-scale packages (typically 10-20mm) has created the current opportunity to use TDR to determine fault location in chip scale packages as well as in many of the traditional packages.


Experimental


A digital sampling oscilloscope with a TDR module was used to supply the fast rise-time voltage edge and to record the voltage edge reflections. Contact to the device under test was made with a probe tip and grounding contact, connected to the TDR module through an SMA cable. Figure 1 shows the TDR waveform that was acquired before probing onto a device, where the first steep rise corresponds to the incident TDR step function voltage leaving the sampling head, and the second steep rise corresponds to the reflection of the step function voltage returning from the end of the probe tip.


No sample preparation is needed to acquire the TDR waveform of the signal pin of a packaged device.


The same is true for board level analysis when the printed circuit board has through hole vias to serve as contact points to the signal pin of interest. The device under test is placed on a flat, ESD protected work area so that the probe tip and grounding wire can be connected to the signal pin of interest and the closest ground pin, respectively, of the device under


test. Grounding further away from the signal pin will cause more aberrations in the acquired waveform,which would complicate the analysis.


Figure 1 TDR waveform, showing the initial incident TDR step and the reflection step returning from the end of the probe tip.


Since the first part of the TDR waveform is not needed for the analysis, the entire waveform is translated to the left to focus on the reflection step returning from the probe tip. Figure 2 illustrates the resulting waveform, where the steep rise corresponds to the reflection of the step returning from the end of the probe tip (the second step shown in Figure 1).


Figure 2 TDR waveform, focusing on the reflected step returning from the end of the probe tip.


Once the probe tip contacts the signal pin, the reflection step of the waveform will extend further along the time axis. The time difference between the reflected signals of the probe tip and the device under test is equivalent to twice the electrical length of the transmission line of the device under test. Figure 3 shows the TDR waveform for the signal pin of a packaged FC-BGA device. Note that the reflected step of the signal pin in Figure 3 is located approximately 500 picoseconds after the reflected step of the probe tip, shown in Figure 2.


-0.3-0.25-0.2 0-0.15人 6


e-0.1 E-0.05 0


0.05


0.1


800


1000


Time (ps)


-0.6


-0.5 (V)Voltage-0.4


-0.3


-0.2


-0.1 0


0 500 1000 1500 2000 2500 3000 3500 4000 4500 5000


Time(ps)


Figure 3 Typical TDR waveform of a signal pin of a packaged FC-BGA device.


Signature Analysis Of TDR Waveform


The length of the electrical path of a transmission line can be calculated by multiplying it’s velocity of propagation (VOP) by half the time measured between the reflected signal of the probe tip and the reflected signal of the transmission line endpoint.


This is demonstrated with the TDR waveform of a FC-BGA substrate shown in Figure 4. The VOP value for the strip transmission line of this substrate(with copper trace lines embedded in FR4 material) is


1.4x108 m/s [15]. The time measured between the reflected signals of the probe tip and the end of a substrate is 230 ps. This value represents the amount of time for the electrical signal to propagate down the transmission line of the substrate, encounter the endpoint, and then return along the transmission line back to the probe tip. The calculated distance to the end of the electrical path of the signal pin is therefore


16.1 mm. This is in good agreement with the actual length of the substrate trace (16.3 mm).


Figure 4 TDR waveform of an unassembled


substrate.


A FC-BGA signal pin was selected to illustrate signature analysis. An experimental approach was taken to directly correlate the contours of the TDR waveform with each element of the FC-BGA electrical path. The electrical path elements include the die, bump, substrate pad, and substrate trace line.


Initially, the TDR waveform was recorded for a given signal pin of a complete FC-BGA device. Segments of the electrical path were then removed incrementally by backside parallel polishing until the underlying layer was exposed and the TDR waveform was recorded at each increment, as shown in Figure 5. The segments removed include the die,the bump array and substrate pads, and finally, the substrate trace line.


The waveforms shown in Figure 5 demonstrate that each element in the electrical path corresponds to specific contours along the waveform of the complete package. Signature analysis can then be applied in failure analysis by comparing the waveform of the signal pin of a failing device with these signature waveforms. The point at which the waveform of the failing unit deviates from the signature waveform would indicate where the fault is located


Figure 5 TDR waveforms corresponding to a) a


complete FC-BGA package, b) removal of the die, c)removal of the bump array and substrate pad, and d)removal of the substrate trace line.


Comparative TDR Analysis


Comparative analysis studies are expected to be the most frequent application of TDR as a packaging FA tool. This type of analysis requires little interpretation of the contours on a given waveform for a failing pin.


Comparison of the waveform from the failing unit with waveforms from a correlation unit, and from an unassembled substrate, provides fast and accurate identification of the main fail site. This technique can be applied to many package types (flip-chip,wirebond microBGA, leadframe, etc.), as well as devices mounted on printed circuit boards.


For the case of a FC-BGA package, a typical waveform of a correlation unit signal pin was shown in Figure 3, and the waveform of the corresponding signal pin on the unassembled substrate of the correlation unit was shown in Figure 4. Overlaying these two waveforms, as shown in Figure 6, clearly identifies the limits for the three main fail site regions(substrate, interconnect, or die). The waveform of


-0.3-0.25-0.2-0.15-0.1


|


-0.05 0


Probe tip


contact point


End of signal pin path


-0.3-0.25-0.2-0.15c


i


-0.1-0.05 0


400 600600


(V) Complete with die(V) Removed die


(V) Removed bumps(V) Removed trace


c b


/


End of


substrate path


the probe tip is also shown to illustrate the beginning of the electrical path. A waveform that terminates to the left of the substrate waveform indicates an open in the substrate. A waveform that terminates just to the right of the substrate waveform indicates an open in the interconnect region, or an open in the die if a waveform terminates tens of picoseconds to the right of the substrate waveform.


The most challenging aspect of comparative TDR analysis is distinguishing between a failure at the interconnect region and a failure in the die, since the distance between these regions can be as small as several microns. In such instances, it would be helpful to build a database of waveforms associated with each fail site to provide a correlation for future analyses. Also, since the substrate would be eliminated from consideration in this instance,destructive techniques such as deprocessing or crosssectioning could be pursued to verify the failure without concern about destroying the substrate.


Comparative TDR analysis has been successful for fail site isolation on a variety of package types. The results section shows analysis of 1) FC-BGA packages with various fail sites, 2) a wirebonded BGA package, mounted in a standard socket, and 3) a wirebonded BGA device in a board assembly.


Figure 6 Overlaying TDR waveforms of the


FC-BGA correlation unit, the unassembled substrate,and the probe tip.


Results And Discussion


Three FC-BGA units were analyzed. In each case,the appropriate signal pin waveforms for a correlation unit and an unassembled substrate were also acquired. The corresponding signal pin waveform of the failing device was then overlayed with these two waveforms on a single graph. The first case, shown in Figure 7, documents an open failure in the substrate, which was confirmed optically (Figure 8).


A crack in the trace line, resulting from the cracked laminate material, was the cause of this open. The second case, shown in Figure 9, documents an open failure at the interconnect region, also confirmed


optically (Figure 10). Nonwetting of the solder bumps between the die and substrate was the cause of this open. The third case, shown in Figure 11,documents an open in the die. Deprocessing of the die to further isolate the cause of this open within the die was not performed.


-0 .3-0 .2 5-0 .2


>


-0 .1 5-0 .1-0 .0 5 0


0 .0 5


20 0


4 0 0


60 0


80 0


10 0 0


T im e (p s )


S u b tra te


F a ilin g U n it


C o rre la t io n U n it


Figure 7 TDR analysis of a failing FC-BGA unit,showing that the open is in the substrate.


Figure 8 Optical image of the cracked trace line in the substrate causing the open in Figure 7.


Figure 9 TDR analysis of a failing FC-BGA unit,showing that the open is in the interconnect.


TDR analysis can also be used for fail site isolation of short-circuits, as in the case of a fine-pitch wirebond BGA device that failed short-circuit continuity test. Curve tracer analysis verified that the signal pin was shorted to ground. It was not known,however, where in the package the short was occurring.


-0.3-0.25-0.2-0.15-0.1-0.05 0


Vo lta ge(V)


Correlation Unit


Subtrate


-0.3-0.25-0.2


-0.15-0.1-0.05 0


Failing Unit


Figure 10 Optical image of the nonwetting solder bumps causing the open in Figure 9.


Figure 11 TDR analysis of a failing FC-BGA unit,showing that the open is in the die.


Since the pitch between individual signal pins was so small for this packaged (approximately 0.5 mm) it was not practical to manually place the probe tip and ground connections on the contact leads of the package. A standard socket for the device was used to provide a wider pitch array of the pins. The signal pin waveform for the empty socket was acquired to indicate which contours on the waveform were associated with the packaged device that was placed in the socket. The waveform of a correlation unit in


8


the socket was also acquired. Figure 12 shows the


。


three waveforms.


The waveform of the failing unit in Figure 12 is shifted positively along the y-axis relative to the other waveforms. The positive shift in the reflected signal waveform is characteristic of short circuit termination of the transmission line, indicating that the signal pin is shorted to ground.


Figure 12 TDR analysis of a failing wirebond device mounted in a socket, showing a short-circuit in the failing unit.


The waveform of the failing unit can be made to overlap the other waveforms by mathematically shifting the data of the waveform negative 0.45V, as shown in Figure 13. The overlapping initial contours of the three waveforms correspond to the electrical path through the socket. The point at which the waveform of the empty socket diverges from the other waveforms indicates the point at which the electrical path of the device begins. The waveforms of the failing unit and the correlation unit overlap for approximately 250 picoseconds. At that point, the waveforms begin to diverge (the correlation unit waveform begins to increase and the failing unit waveform continues to decrease). This point of divergence corresponds to the point at which the short-circuit fault is located.


Figure 13 TDR analysis of the failing wirebond


device mounted in a socket, where the waveform of


the failing device is shifted to overlap the other


waveforms.


Although further analysis on this unit was not performed, analysis of an identical short circuit failure on another device from the same lot of units revealed that a metal bridge extending between the source and drain of the output transistor was the cause of the short. The metal bridging was found after deprocessing and removal of the metal3 layer,and subsequent inspection with a scanning electron microscope.


Vo lta ge(v)


-0.5-0.4-0.3)VVoltage (-0.2总总。


0.2


0.3


0.4


Empty Socket


Socket w/ Correlation Unit


Socket w/ Failing Unit


-0.5-0.45-0.4-0.35 0-0.3


八


6-0.25 E-0.2-0.15-0.1-0.05 0


Socket w/ Failing Unit (Adjusted)


Component level analysis is not the only application of TDR. A wirebond BGA device mounted on a printed circuit board was tested to determine if the fault location was in the board or in the packaged device. The signal pin waveform was acquired first for an unassembled board, then for a correlation board assembly (both the board and mounted device are known to be good). Finally the signal pin waveform for the failing board assembly was acquired. The overlaying waveforms are shown in Figure 14, suggesting an open fault within the package, near or within the die. The TDR analysis was accomplished nondestructively since through hole vias in the board were available to make contact to failing signal pin.


Figure 14 TDR analysis of board assembly, showing


that the open is in the wirebonded BGA package.


Future Development


Widespread acceptance and implementation of comparative TDR analysis within the packaging FA community will require enhancements in both equipment hardware and data analysis methods.


Manual placement of the probe tip and ground connection onto BGA balls or fine pitch lead fingers is awkward and tenuous, at best. The use of a microprobe station with 3-axis microprobe manipulators would make the measurement much easier to acquire, and would facilitate future automation of probe placement. Development of signature analysis software would also aid in analysis and isolation of the fault location.


Summary


Comparative TDR analysis has been successfully implemented as a fast and accurate method for initial isolation of fault location in packaged devices. We have demonstrated that this type of analysis can isolate the failure to one of the three main regions: the die, the substrate, or the interconnect region. TDR analysis is capable of detecting both open and short circuit defects on a component level as well as for board mounted packages. The technique can be applied to both flipchip and wirebonded package types.


The authors wish to thank their colleagues at Texas Instruments for their contributions to the development and implementation of this technique at TI, including Darvin Edwards, Mike Lamson,Michelle Nguyen, Jeff Tregre, and Fred Langford.


Special thanks to Cheryl Hartfield for her editorial review of this paper.


1) Package Analysis: SAM and X-Ray, T.M.


Moore and C. Hartfield, in Failure Analysis of Integrated Circuits, Tools and Techniques, L.C.


Wagner, ed., Kluwer Academic Publishers,Boston (1999).


2) Acoustic Microscopy (C-AM), T.M. Moore, in


人


Characterization of Integrated Circuit Packaging


an


Materials, T.M. Moore and R.G. Kenna, eds.,Butterworth-Heinemann, Boston (1993).


3) X-Ray Radiographic Inspection, J. Colangelo,ibid.


4) 4, Digital Sampling Oscilloscope User Manual,Tektronix Model 11801C.


5) TDR Tools in Modeling Interconects and Packages, Tektronix Application Note.


6) Time Domain Reflectometry Theory, Hewlett Packard Application Note 1304-2.


7) Measurement and location of dielectric anomalies in field aged XLPE cables, Y.P.


Aksenov, V. Arsentiev. M. Golovkov, Y.S.


Pintal, J.C. Bromley, A. Glodjo, and W.


McDermid, Conference Record of the 1994 IEEE International Symposium on Electrical Insulation IEEE, New York, (1994) p.89-94.


8) No small change (compact time-domain reflectometers), W.R. Campbell, TelephoneEngineer-and-Management. vol.94, no.23 (1990)p.54-6.


9) Using The Time Domain Reflectometer To Check For And Locate A Fault, M. Ramphal, E.


Sadok-E, Third International Conference on CANDU Maintenance Proceedings. Canadian Nucl. Soc, Toronto, Ont., Canada (1997) p.1-5.


10) An Automatic Fault Detection And Location Technique In Low Voltage Distribution Networks, S. Navaneethan, J.J. Soraghan, W.H.


Siew, R. Muirhead, and J. Livie, Proceedings of EMPD '98. 1998 International Conference on Energy Management and Power Delivery, IEEE,New York (1998) p.732-6 vol.2


-0.35-0.3-0.25 0-0.2 6


e-0.15-0.1(-0.05 0


In all IC technologies dielectric materials are used to both electrically isolate conductor layers and to passivate and protect the surface from mechanical damage. These layers have been engineered with knowledge of electrical and mechanical properties and usually a disregard for their optical properties. From an optics perspective, thin dielectric layers are used to make interference filters and their index of refraction and thickness are used to control the spectral response.


Fig. 12 shows the relationship between the dielectric layers and the light emission sites and their indices of refraction. For front side light emission analysis, light from the emission site will have to pass through the composite layer of SiO2 (inter-level dielectrics and passivation) before escaping into the air. The impact of the dielectric layers on the light emission spectrum depends on each layer’s thickness and index of refraction. For this example, d1 is the composite dielectric thickness that is assumed to be SiO2 with an index of refraction of 1.46. The other indices of refraction needed are those of silicon and air (3.5 and


1.0 respectively).


At normal incidence, the reflection coefficient of light at a wavelength λ0 (vacuum wavelength) can be related to the material properties shown in Fig. 12 by [7]


))


sin(


n(j


cos(


n(


(r


2 1


λ


δ


+


−


=


where


λπ


The percentage of light transmitted into the air is related to the reflection coefficient by


∗


⋅


(T


where r(λ0)*is the complex conjugate of the reflection coefficient r(λ0). Note that when n1d1/λ0 is an integer(which occurs when the round trip phase change is an integral number of half-wavelengths) the reflection coefficient is only a function of the initial and final materials and not the dielectric layer itself.


From these equations, the transmission spectrum can be calculated for a dielectric layer of any thickness.


Fig. 13 shows the resulting transmission spectra for dielectric layers of 500 and 5000 nm. A comparison of the two curves shows two important details. First, the maximum and minimum transmission percentage will always be constant (in this case, Tmax = 94 % and Tmin = 69 %). Second, the frequency of the undulations in the spectra depend on the thickness of the dielectric layer with a thinner layer having fewer peaks and valleys in the transmission spectrum.


Air, n0 = 1.0


|SiO2, n1 = 1.46 |d1 |
|---|---|

|Si, n2 = 3.5 Emission site |Si, n2 = 3.5 Emission site |

Figure 12 Orientation of dielectric layers for front side light emission analysis of ICs.


500


700


900


1100


65 70 75 80 Transmission (%)85 90 95


5000 nm 500 nm


Wavelength (nm)


Figure 13 Transmission calculations for a SiO2 film on a Si substrate at normal incidence.


This relatively simple theory can be complicated to use in practice. In present IC processes, the multitude of different dielectric materials that have different dielectric constants can make this single layer example a much more complicated multi-layer problem. The other main issue that complicates this theory is the presence of non-normal components of light from the emission site. While this is present on all light emission processes from silicon ICs, it is particularly important when the structure obscures the normal component of the emission. This can happen when light is emitted from a gate oxide failure where the gate polysilicon will act to filter the normal component. The overlying metal can act in the same manner. For this analysis, only the normal component was considered to demonstrate the influence of the dielectric materials on the resulting light emission spectrum.


To demonstrate the effect of a dielectric thickness change on the light emission spectrum, a pn junction was reverse biased and a spectrum was measured before and after a wet dielectric etch. The resulting light emission spectra are shown in Fig. 14 (10.0 V reverse biased n+p junction, I = 890 µA) for the two dielectric thicknesses. The overall shape of the envelope has not changed but the spectral content between 650 nm and 950 nm shows some dramatic differences. The etch removed an estimated 500 nm per minute, so the


transmission spectrum was calculated for 4500 nm (the normal dielectric thickness for the technology) and for 3500 nm (after a 2 minute wet etch) and is shown in Fig. 15.


0.6


0.8


after oxide etch


before oxide etch


Figure 14 Emission spectrum before and after a 2 minute oxide etch.


3500 nm 4500 nm


Figure 15 Calculated transmission changes for two composite SiO2 thicknesses.


The theory presented in this section demonstrates that the spectral content of the light emission could also be used to measure the composite dielectric thickness by locating the peaks and valleys in the spectrum and fitting the data to a calculated transmission spectrum.


The process would need to include the non-normal components to be accurate.


Gate Oxide Failure Example


Several ASICs failed tests after dynamic burn-in. The burn-in conditions consisted of applying a vector set at


6.0 volts for 168 hours and 125°C. One IC (SN 199)failed IDDQ tests after one hour in burn-in; another IC(SN 234) failed also failed IDDQ tests after 14 hours in burn-in. Electrical testing on a bench setup indicated IDDQ several orders of magnitude above the limit of


100 µA. IDDQ was stable with respect to time. Photon emission microscopy was performed on the samples.


The results indicated multiple light emission sites on both ICs (see Fig. 16).


Spectral emission analysis was then performed on the two ICs (Fig. 17 shows two spectra from one of the failures at two different voltages). The spectra for these two ICs are quite similar, showing a large peak at approximately 800 nm with multiple minor peaks embedded within the broad peak. It should be noted that these spectra do not appear to be indicative of simple forward-bias light emission or simple reversebias light emission. Rather, the spectra are more complex, indicating that multiple phenomena may be occurring in the gate oxide region.


Intensity (arb. units)Normalized


The defect sites were localized by deprocessing to the polysilicon and performing EBIC analysis. The samples were then further deprocessed to the gate oxide layer to determine the cause of failure. SEM examination of the gate oxide region revealed a small“divot” in the gate oxide region that corresponded to the light emission and EBIC sites (see Fig. 18). It was concluded that the gate oxide shorts occurred between the polysilicon gates and the channel at the divots during burn-in.


Figure 16 Photon emission image of SN 234.


Polysilicon Stringer Example


In the last example, a low yield wafer lot was analyzed to identify the cause of leakage paths in a gate to gate leakage test structure. The test structure has 130 pairs of gates patterned over a single gate oxide region.


Failing structures had gate to gate resistance values of around 6 kΩ•with a linear I-V characteristic. Several samples were removed from an affected wafer and packaged to facilitate failure analysis. The thermallyinduced voltage alteration (TIVA) technique [8] was used to localize the affected gates. The results showed that on one failing test structure, approximately 30% of the gates were affected. Although TIVA could


successfully identify which gates were affected, only the metal to polysilicon contacts of affected gates were visible in the images. Light emission analysis was also done to further characterize the leakage paths. The example shown in Fig. 19 has four visible emission points, all of which are on the same side of the test structure.


300 400 500 600 700 800 900 1000 1100 1200


580.3 nm


942.8 nm


838.4 nm


814.5 nm


760.8 nm


659.4 nm


5.0 V


6.0 V


Figure 17 Light emission spectra from a suspected gate


oxide failure at two different supply voltages. The


wavelengths of the various peaks in the spectra


have been identified.


Figure 18 Location of one of the defects of SN 234.


Spectral information was also collected from several emission sites. An example spectrum is shown in Fig.


20. This spectrum resembles the gate oxide leakage spectra shown in Figs. 11 and 17. All three spectra have high electric field-related information and also have a peak between 700 and 900 nm. These peaks are far enough away from the upper limit for this spectrometer that they can be distinguished from the roll off in response above 950 nm.


Figure 19 Light emission analysis of gate to gate leakage failure.


0.4 a0.6口0.8 q


日


U n1.2


1.6


1.8


Relative Intensity (arb. units)


Figure 20 Spectrum of light emitted from emission sites in Figure 19. (Applied bias was 8.0 V, 1.39 mA,5 minute exposure time).


The structure was deprocessed to allow for a detailed inspection of the light emitting areas. Inspection using


0.25um 20kv 40kx


a scanning electron microscope (SEM) showed that the cause of the leakage was polysilicon stringers (Fig. 21).


The stringers were present on both n-channel and pchannel test structures but were only conductive on the n-channel devices. The 40 nm wide stringers were located on one side of the gate oxide region only and at a distance of 300 nm from the field oxide edge.


Figure 21 Polysilicon stringers found at light emission locations.


This analysis has successfully demonstrated the relationship between the electric field and the presence or absence of short wavelength light emission from silicon ICs under the conditions associated with the most common IC failure modes. A spectrometer was used to confirm the predictions from basic device physics. Several failure analysis cases were presented to demonstrate the utility of spectral analysis as a tool for understanding the origin of the light detected from an IC with an undetermined failure mode. The conclusion from this study is that signature analysis may not be able to provide a definitive root cause but can provide detailed information about the nature of the light emission. This information can help confirm the root cause after further analysis is performed.


The authors would like to thank Cornelia Siemens for investigations on the transmission gratings and Richard E. Anderson for his review of this manuscript. Sandia is a multiprogram laboratory operated by Sandia Corporation, a Lockheed Martin Company, for the United States Department of Energy under contract number DE-AC04-94AL85000.


1) D. L. Barton, P. Tangyunyong, J. M. Soden, A. Y.


Liang, F. J. Low, A. N. Zaplatin, K. Shivanandan,and G. Donohoe, ISTFA 96, pp. 9 – 17, 1996.


2) G. Chynoweth and K. G. McKay, Phys. Rev., 102(2), 369-376, 1956.


3) M. Rasras, I. De Wolf, G. Groeseneken, H. E.


Maes, S. Vanhaeverbeke, P. De Pauw, ISTFA 97,pp. 153 – 157, 1997.


4) J. M. Tao, W. K. Chim, D. S. H. Chan, J. C. H.


Phang, and Y. Y. Liu, IRPS 96, pp. 360 – 365,


1996.


5) S. M. Sze, Physics of Semiconductor Devices, John Wiley & Sons, Ch. 2 & Ch. 12, 1981.


6) E. S. Wang, Fundamentals of Semiconductor Devices, McGraw-Hill, Ch. 4, 1978.


7) E. Hect and A. Zajac, Optics, Addison-Wesley, Ch.


9, 1974.


8) E I. Cole, P. Tangyunyong, and D. L. Barton, IRPS 98, pp. 129 – 136, 1998.


12.100*5.00 kV1pmSANDIA#2008*14 APR 99


Electronic Device Failure Analysis Society, editor, p 69-76


DOI: 10.1361/cp1999istfa069


# Temperature Profile Measurement and Failure Characterization of ESD Protection Devices Using Spectroscopic Photon Emission Microscopy and Raman Spectroscopy


Temperature Profile Measurement and Failure Characterization of ESD Protection Devices Using Spectroscopic Photon Emission Microscopy and Raman Spectroscopy


Mahmoud Rasras, Ingrid De Wolf, Guido Groeseneken, Jian Chen,Karlheinz Bock and Herman E. Maes


IMEC, Leuven, Belgium


In this paper, Photon Emission Microscopy (PEM) and micro-Raman Spectroscopy (µRS) are applied for temperature profile measurements and failure characterization in gg-nMOS ESD protection devices. The measurements were carried out in avalanche and snapback biasing conditions. A correlation between the temperature profile obtained by µRS and the light emission location, measured by PEM, is observed for non-degraded devices. In addition, ESD-degraded devices were studied. PEM, µRS, Spectroscopic Photon Emission Microscopy (SPEM) and electrical measurements were used to investigate the origin of the light emitted at the failure site. They showed that the light emission occurring at the failure site is due to impact ionization.


Photon Emission Microscopy (PEM) has been widely applied for the monitoring of snapback in ESD protection devices, and for failure localization [1-4]. A uniform triggering of ESD devices in snapback is essential for high ESD robustness. The possible occurrence of a non-uniform snapback can easily be detected by PEM. In some cases, instability was observed in the current flow region, i.e. the snapback region jumped from one side of the gate to another [5].


The reason for this non-uniform distribution of the light and current along the gate width under snapback conditions, and for current flow instability, is not entirely clear. Possible explanations are attributed to local changes in the electrical field due to electron trapping in the oxide, or due to thermal effects [1]. The latter possibility was never further investigated because the local lattice temperature in such devices was never


measured. Measuring the lattice temperature would also be useful for the simulation of ESD events.


Degradation in gg-nMOS is in general attributed to the presence of a conduction path due to growth of filamentation needle from the drain to the source junctions (a spike) [4] . PEM results show that damage is visible as local emission spots [1-4]. The origin of the light emitted at the failure site is not clear. In this paper,we apply micro-Raman spectroscopy to measure the local lattice temperature in gg-nMOS ESD protection devices. We compare the results with PEM images. In addition, degradation of these devices by TLP-stressing is investigated in detail by µRS, PEM and SPEM. The results of these techniques are compared with the data from electrical measurements.


Grounded-gate nMOS transistors (gg-nMOS) were fabricated in a 0.5 micron CMOS process. The gate,source and substrate are connected, and grounded during the measurements. This process included, for ESD considerations, a silicide blocking option [5]. The devices were designed with a wide and entirely symmetrical metal routing, minimizing any series resistance and allowing uniform injection of the current at the contact holes. Transistors with widths of 50 µm were investigated. The gg-nMOS devices which were studied with µRS had a silicide spacing of 4 µm at the drain side and 2 µm at the source side. A layout of a typical gg-nMOS is shown in Fig. 1. The top side is the drain, the bottom side the source. Different parts are marked for later reference. Also special transistors,which had similar processing as the gg-nMOS devices,were investigated. In these devices, the gate, source and substrate are separately accessible.


Silicide


Raman


Drain contact


Source contact


LOCOS corner


Gate corner


Gate


Figure 1 Layout of a gg-nMOS.


Spectral emission microscopy experiments were performed with a modified Hypervision system[6] which has a GENIII-NIR detector. In addition to conventional emission microscopy experiments, this system allows the measurement of the emitted light spectrum through insertion of a direct vision prism. This system can acquire a continuous spectrum in the wavelength range from 500 to 1100 nm.


Micro-Raman spectroscopy experiments were performed using a DILOR Raman system. The 457.9 nm line of an Argon laser was used for excitation. The diameter of the focused beam spot on the sample was ≤1 µm. The Raman experiments were done on gg-nMOS devices. The sample was moved in steps of minimal 0.1µm using an XY-stage, in such a way that a scan was made along the width of the gate, at its drain side (see arrow in Fig. 1). At each point a Raman spectrum was recorded. Fig. 2 shows a typical Raman spectrum of crystalline silicon. The silicon Raman peak is visible at 521 cm-1. In order to determine its frequency, the peak is fitted with a Lorentz function. The plasma lines of the laser, which are also visible in the figure, are used as reference [7]. They are fitted using a Gaussian function to determine their frequency. Variations in the position of the plasma line are due to instrumental variations(laser, room temperature, air pressure, etc.). The Raman spectra are corrected for these variations. The frequency of the Si Raman peak, ω, depends on the local temperature and on the local mechanical stress [7]. This frequency is ~ 521 cm-1 at room temperature, for stress free samples. It increases if compressive stress is present in the sample, and it decreases if the Si is under tensile stress. It decreases with increasing Si lattice temperature.


600 Intensity (a.u.)400 200


580


560


540


520


480


Raman shift (cm-1)


Si Raman peak


Plasma line


M


Figure 2 Typical Raman spectrum of crystalline silicon,showing the Si Raman peak and plasma lines from the laser.


Temperature Profile Measurements


As it is of interest to know which temperatures are present in the device during different biasing stages from avalanche to snapback, we performed microRaman spectroscopy experiments on a 50 µm wide ggnMOS. The probing laser beam could reach the silicon next to the gate and the silicon Raman peak is measured.


Figure 3 demonstrates the Raman results obtained on unbiased device. The full line in this figure represents the Raman shift measured when scanning across the device. The dotted line represents the Raman intensity.


The scan direction is as indicated by the arrow in Fig. 1.


The right side of Fig. 1 corresponds with the right side in Figs. 3. A drop in the intensity is observed when crossing the metal connection between gate and source(arrow on dotted line). Left and right from the gate (< 0µm and > 50 µm), the shift of the Raman frequency from the stress free value is zero. However, next to the gate, the shift becomes negative, indicating tensile stress in the silicon near the gate. A Raman shift of about 0.3 cm-1 is observed. Assuming uniaxial stress, the relation between Raman shift (∆ω) and stress is [7]:


σ (MPa) = - 434  ∆ω (cm-1)


(1)This means that a shift of 0.3 cm-1 corresponds to a tensile stress of about 130 MPa.


-2.5 Raman shift (cm-1)-2.0-1.5


-1.0-0.5


60 40 20


0 -20


Position (µm)


600el 500y


u 400)300


shift


intensity 10 mAw


0 mA


Figure 3 Raman frequency shift from the stress free value (left axis) for a gg-nMOS device under ID = 0 mA and 10 mA bias. The dotted line denotes the intensity of the Raman peak for 0 mA (right axis). The arrow


denotes a local minimum in the intensity at the gatesource metal contact.


When applying a constant current to the device, the temperature increases. This gives rise to an additional negative shift of the Raman peak. An example of this is shown in Fig. 3 for a current of 10 mA. Notice that this curve is broader than the 0 mA curve. This is because the temperature is also increasing in areas outside the gate, even at the right side of the metal connection between gate and source.


The Photon Emission Microscope (PEM) was used to monitor the current flow in this device for increasing currents. The sequential PEM results are shown in Fig. 4. These figures have the same orientation as the layout shown in Fig. 1. At 1 mA, during avalanche breakdown, localized emission spots can be observed at the device corners. The corners in the junction along the drain perimeter of the gg-nMOS device are indicated in Figure 1 (black triangles). One can distinguish two LOCOS corners and two gate corners. Avalanche breakdown at the junction is expected to occur first at positions with highest electrical field, which is indeed at these corners [5]. Two spots are visible at the left side,one at the gate corner (bottom) and one at the LOCOS corner (top). One spot is visible at the right side, at the gate corner. The fact that no spot is observed at the right LOCOS corner indicates small variations in the local electrical field. At 5 mA, light is visible along the whole width of the gate, indicating that avalanche breakdown occurs in this whole region. At 10 mA, snapback of the voltage to 7.3 V occurs, but the device triggers only at the right side. Only at higher currents is the whole width of the device triggered. This non-uniform triggering of


ESD protection devices was discussed previously by C. Russ et al. [5].


l


0V, 0mA


12.13V, 1mA


10.2V, 5mA


7.28V, 10mA


7.31V, 50mA


8.12V, 100mA


D


II


G S


S


Figure 4 PEM images of a 50 µm wide gg-nMOS for different applied currents at the drain (ID).


-5


(cm1)Raman shift -4Nmmy-3


-2


-1


150


50room (K)T-T 0


10 30 75


26


Figure 5 Raman frequency shift (left axis) and


corresponding increase in lattice temperature (right axis)of a 50 µm wide gg-nMOS (same device as in Fig. 4) for different ID (in mA).


In order to distinguish between the effect of stress and of temperature, the curves in Fig. 5 were corrected by extracting the Raman shift at zero bias. In this figure, the shift of the Raman frequency from its control value (no stress, room temperature) is plotted as a function of the position along the width of the gate of a gg-nMOS, for different stress currents. This shift is corrected for mechanical stress effects and only reflects the influence of the local temperature on the Raman frequency. So,Fig. 5 shows the influence of the temperature only on the Raman shift. It is clear that for increasing currents,the Raman shift becomes more negative. This indicates higher temperatures. Indeed, the relation between the


frequency of the Si Raman peak and the temperature is given by [8]:


∆ω = -0.025 ∆T


(2)


The local temperature, as calculated from the Raman shift, is shown on the right axis. We did not observe a clear correlation between these Raman results and the PEM pictures at low currents (ID < 5 mA). This is partly due to the effect of the laser light, used to measure the Raman spectra, on the functioning of the device at low stress currents. Indeed, the laser light generates electronhole pairs near the gate. When forcing a constant current through the device, these electron-hole pairs may add to the current, such that a lower voltage is required to keep the same constant current. This effect is especially pronounced at the edges of the gate. Although it is small,we noticed that it affects the I-V characteristics of the device. Nevertheless, the temperature profile shows some remarkable features. At 5 mA (7.2 V), the temperature seems to be uniform across the device. In this case there was probably avalanche breakdown across the whole width of the device (picture of 5 mA in Fig. 4). There is some drop at the right side, but this is likely to be due to a measurement error, because it was not observed in other devices. At 10 mA (7.16 V) the device is already in snapback. The overall temperature along the gate increases, with a maximum at the left side. This could correspond with a local triggering of the device. For 26 mA (7V) this maximum moves from left to right. At 30 mA (7V) the maximum temperature is again located at the left side of the gate. This current flow instability, i.e. a jumping from one side of the gate to the other side (along the width) of the not-uniform snapback location was discussed by Russ et al. [5]. In PEM pictures from similar devices, they could see the light spot (as the one in the 10 mA photograph in Fig. 4)jumping in a random way from right to left. Measuring one Raman peak (at one location) takes 30 s. A whole scan along the gate of the device takes about 45 min. It is very likely that, if the device was not completely triggered, such a jumping took place during the Raman experiments. This could explain that maxima in the temperature are visible at both sides of the gate. The side where the triggering occurred most has the highest temperature. For higher currents (75 mA (7.7 V) and 100 mA (8V)) the device is completely triggered (as for the 50 mA and 100 mA pictures in Fig. 4). The temperature profile also becomes more uniform. Sharp temperature peaks become visible at the edges of the gate. In the 100 mA picture of Fig. 4, one can observe an upward extension of the emitting region at the edges of the gate. This could explain the temperature peaks.


These Raman results show a clear correlation between the local temperature along the gate width and the PEM images.


Failure Analysis


Devices degraded after ESD stress were analyzed by PEM. Localized light emission spots were clearly observed, as shown in figure 6. Degradation in ggnMOS is in general attributed to the presence of a conduction path due to growth of filamentation needle from the drain to the source junctions (a spike) [4]. The origin of light emission at the defect site was never thoroughly investigated. We used PEM, SPEM, Raman spectroscopy and electrical measurements to study these failed ESD protection devices in more detail.


Micro-Raman Spectroscopy


In order to find out whether biasing the device would show an important increase in the temperature near this defect site, micro-Raman spectroscopy experiments were also performed for different biasing conditions.


Raman spectra were measured along the width of an ESD damaged, 50 µm wide, gg-nMOS This was done for the device from Fig. 6. The results are shown in Fig. 7. They were corrected for effects of mechanical stress on the Raman shift as was done for Fig. 5. In this damaged device, we did expect a local increase of the temperature near the damage site. However, an overall increase of the temperature along the gate with increasing current is observed. Only at 50 and 100 mA,a local increase of the temperature near the damaged site is seen (arrows in Fig. 7). These results indicate that some current may still flow in the device outside the damaged area. It is unlikely that the temperature is localized at the emission site and shows a variation along the gate width as can be seen in Fig. 7. Further, we can conclude that the light detected at the damage site is not due to temperature. Indeed, this emission is already detected by PEM at very low currents (lower than 10 mA), where the temperature is still below 50oC, as can be seen in Fig. 7. Only temperatures higher than 300oC can be detected in our PEM system.


Figure 6 Localized emission spot in a gg-nMOS after TLP stressing, as observed by PEM.


-6 Raman shift (cm-1)-5-4


远


-3-2


T


-1 0


80 60 40 20 0 Position (µm)


250 200 150 100 50 0


10 25


3100


Figure 7 Raman frequency shift (left axis) and


corresponding lattice temperature change (right axis) in


H


a 50 µm wide ESD damaged gg-nMOS (same device as人 in Fig. 6) for different ID (as indicated, in mA).a


Another example is illustrated in Fig. 8. Figure 8a shows the PEM image of a 50 µm wide ESD damaged device.


PEM clearly shows a local emission spot near the right side of the device. The image is somewhat disturbed by a bond wire which crosses the device to make contact to the source side (bottom). Fig. 8b shows the result of a Raman scan, starting near this bond wire and ending at the left side of the device. A clear drop in the intensity and an increase of the FWHM is observed at the same location of the emission spot of Fig. 8a, i.e. at about 40µm from the left edge of the gate. This indicates that the silicon is locally not crystalline any-more, but damaged


[9]. The left edge can be recognized in this picture by the local increase in the intensity (at position about 50 µm). In addition to the changes in Raman intensity and FWHM, also a decrease of the Raman peak frequency down to –2.4 cm-1 was observed. This indicates that the device from Fig. 8 is locally highly damaged, and that this damage in the silicon is probably close to the surface. This is confirmed by SEM(scanning electron microscopy) pictures from this device, as shown in Fig. 8c. The bond wire, which is visible in Fig. 8a, was removed. In this picture, a clear filamentation can be observed at about 40 µm from the left gate edge. This defect seems to cross the entire device, starting at the drain contact, crossing the gate,and ending at the source contact. The data from Fig. 8 clearly show a relation between the PEM, Raman and SEM observations.


600△


n500


C


300


6.5


6.0


5.5WF


5.0M


4.5)


4.0


3.5


Figure 8 PEM image, Raman data and SEM image from the same ESD-damaged device. a: local emission is detected by PEM, b: Raman shows a local increase of FWHM (dotted line) and decrease of the intensity (full line), c: SEM picture showing a defect (arrow) at the same location.


40 µm


Spectral Photon Emission Microscopy


In order to investigate the origin of light emission in more detail, the damaged devices were studied with Spectroscopic Photon Emission Microscope (SPEM).


Emission spectra from devices with degradation ranging from low-level damage (low leakage currents) to completely damaged (high leakage currents) were obtained using SPEM. These experiments were performed on special transistors, similar to the ggnMOS ones, but the gate, drain and substrate are separately accessible, so that the current at these different contacts could be measured independently. The emitted spectra taken at different level of damage at constant drain voltage are shown in Fig. 9. They are characterized by a broad-spectral distribution.


10-2 10-1 100 Intensity (a.u)101 102 103


5V, 367µA


5V, 30µA  5V, 5µA


Figure 9 Measured spectral distribution of the light


emitted from the failure location. Spectra were obtained at the same drain voltage (VD) for devices with different degradation levels (various leakage currents).


These spectra are similar to the ones emitted by hot carriers in an nMOS [10-12]. This suggests that light emitted at the failure site is generated by hot carriers.


Fig. 9 shows a clear relation between the spectral intensity and the leakage current of the devices: For the same applied drain voltage (VD) the spectra show a uniform shift towards higher intensities with increasing leakage current. The hot electron temperatures (Te) were calculated from these spectra, assuming a Maxwellian electron energy distribution. The obtained values for Te are in the range of 3900 K for all spectra. This shows that for the same VD, Te does not depend on the degradation level.


Fig. 10a shows the variation of the spectra obtained from one of the degraded devices (367 µA at 5V) at different drain biases. Calculation of the electron


temperature [13] (Fig.10b) indicates almost a linear dependence of Te on the drain voltage. The electron temperature varies from 1330 to 4420 K as the drain voltage changes from 3 to 6V, respectively. All these observations indicate that the emitted light is caused by hot electrons generated in the damaged region at the drain side. In order to further confirm this observation,electrical measurements under different biasing conditions were performed.


Unassembled Board Board w/ Failing Unit


Board w/ Correlation


11) Theoretical Background for the TDR Methodology, H.H. Nissen and P. Moldrup Proceedings of the Symposium: Time Domain Reflectometry Applications in Soil Science,Tjele, Denmark: Danish Institute of Plant and Soil Science (1994) pp. 9-23. SP report no.


11,Volume 3


12) Electrical Evaluation of the BIPS-0 Package,Patrick D. Boyle, Digital (WPL) Technical Note TN-29, Palo Alto CA, July 1992.


13) 13. Characterization and modeling of packages by a time-domain reflectometry approach, Van Hauwermeiren, L.; Herreman, M.; Botte, M.; De Zutter, D. Components, Hybrids, and Manufacturing Technology, IEEE Transactions 478-482 Aug. 1992


Vol. 15 Issue:


14) Mission reliability improvement by marginal checking, Boenning-R-A, Proceedings-of-theAnnual-Reliability-and-Maintainability-Symposium, Piscataway, NJ, USA. (1990) p 53-58


15) MECL System Design Handbook, 4th Edition,Bill Blood, Motorola U.S.A. (1988) p. 48.


Electronic Device Failure Analysis Society, editor, p 57-67


DOI: 10.1361/cp1999istfa057


# Light Emission Spectral Analysis: The Connection Between the Electric Field and the Spectrum


Light Emission Spectral Analysis: The Connection Between the Electric Field and the Spectrum


Daniel L. Barton, Paiboon Tangyunyong, Jerry M. Soden, Christopher L. Henderson,and Edward I. Cole, Jr.


Sandia National Laboratories, Albuquerque, New Mexico


Rainer Danz and Reinhard Steiner


Carl Zeiss, Jena, Germany


Zbigniew Iwinski


Carl Zeiss Inc. Thornwood, New York


The device physics necessary to gain theoretical insight into the relationship between the bias conditions and the associated electric field for semiconductor structures in various failure conditions such as forward and reverse biased junctions, MOSFET saturation, latchup, and gate oxide breakdown are examined. The relationships are verified by light emission spectra collected from test samples under various bias conditions. Several examples are included that demonstrate the utility and limitations of spectral analysis techniques for defect identification and the associated, non-electric field related information contained in the spectra.


In our previous work [1], we reviewed the basics of light emission to stress the need to move to nearinfrared detector technologies to better match the camera response to the emission from silicon-based devices. Fig. 1 shows the emission spectra from both forward and reverse biased pn junctions [2]. From these data, we argued that all spectra collected from silicon devices would follow these two curves and would depend on the electric field governing the emission process.


The relationship between the electric fields associated with the various defect conditions encountered on microelectronic devices and the light emission spectra from these defects have interested the failure analysis community for years. The intent is to use the light emission spectrum to help identify the type of failure and limit the need to deprocess the sample to identify the root cause, saving both time and money. The problem has been the availability of spectrometers that are capable of measuring the spectral content of the very weak light emission produced by failing


semiconductor devices. Spectrometers are now available that can verify our argument and give insight into different light emission signatures.


The spectrometer system used in this study and the interpretation of spectra from the most common defect classes (listed in Table 1) are described to demonstrate the strengths and weaknesses of spectral analysis.


0.3 0.4 0.5 0.6 0.7 0.8 0.9 1.0 1.1 1.2 1.3 1.40


10 20 30 Intensity (arbitrary units)40 50


Forward Bias


Reverse Bias


Wavelength (microns)


Figure 1 Measured emission spectra from forward and reverse biased Si, pn junctions [2].


Table 1 Light Emission Processes and


the Associated Electric Field


|Light Emitting Process |E-Field |
|---|---|

|Forward biased junctions Reverse biased junctions Latchup Transistor saturation Gate shorts |Low |

|Forward biased junctions Reverse biased junctions Latchup Transistor saturation Gate shorts |High |

|Forward biased junctions Reverse biased junctions Latchup Transistor saturation Gate shorts |Mixed |

Spectrometer Theory of Operation


In recent years, there have been several papers published on spectrometers suitable for analyzing light emitting defects on silicon ICs [3, 4]. The spectrometer used in this study (EmSpec) works by collecting collimated light from the device-under-test (DUT) with an objective lens and passing it through a transmission grating as shown in Fig. 2. The grating splits the diffracted light into its zero order (emission spot) and higher diffracted order (“plus-minus”) components. The diffraction pattern is subsequently focused onto a cooled, CCD camera. Since the spectrometer uses a blazed transmission grating, most of the emission light intensity is concentrated within the (“plus”) first order.


The spectrometer is calibrated by collecting a spectrum from a point-like, halogen light source at a fixed color temperature (3200 K) and correcting the spectrum to match the appropriate blackbody spectrum. In its present state, the spectrometer has the same spectral response as the Si CCD camera used for image collection (400 – 1100 nm). Future versions will be available with extended response into the near infrared(to 1400 nm).


|1|1|α |
|---|---|---|

|Carrier plate|||

60.


Carrier plate Grating (plastics, refractive index n)α = prism angle (blaze angle)


古


δ = deflection angle (ß of the first diffraction order)g = grating (grism) constant


电话500900200800980100011801208


Figure 2 Principle of operation of a blaze transmission grating used in the EmSpec spectrometer.


昌


The principle of a blaze transmission grating is based


Intensity (arb. units)昌


on the Echelette type shown in Fig. 2. When δ = ß the


“blaze condition” is met. The blaze-wavelength, λb,follows the equation


20-


( )


[


]


α


sin


arcsin


g


f500600700000980100011001208


The spectral detection range (spr) is given as


spr


7.0


≤


The EmSpec prism is designed for λb ≈ 600 nm and therefore the wavelength range of 400 nm to 1200 nm.


There is a linear relationship for the distance between the zero order and the diffracted orders. Wavelength calibration can thus be easily done using a narrow-band interference filter and only depends on the tube lens.


In contrast to the wavelength calibration, the system calibration (meaning the influence of the optics including the different coating layers and the sensitivity of the CCD target) has to be done for each objective lens. The system calibration is accomplished by treating the emission spot as a weak fluorescence signal. A point-like, auxiliary halogen light source at a fixed color temperature (3200 K) is used as a calibration standard. The wavelength spectrum for the halogen source is calculated by applying Planck´s black body radiation formula


) ν


−ν


ν


c


dv


K


E


kT


where h is Planck’s constant, c is the speed of light, k is Boltzmann’s constant, and dν is the frequency interval.


The calibration factors are then obtained by matching the experimental light emission spectrum shown in the bottom curve of Fig. 3 to the theoretical blackbody radiation spectrum shown in the top curve of Fig. 4.


Once calibrated, spectral analysis is done by positioning the zero order diffraction pattern to the left hand side of the image, inserting the EmSpec filter into the beam path, and collecting a light emission image.


160


80


Figure 3 Theoretical black-body radiation spectrum(top) and an uncorrected experimental spectrum(bottom) from a halogen light source.


δ = ß


Forward Biased pn Junctions


Forward bias is perhaps the most straightforward bias condition by which light is emitted from a silicon pn junction. The theory behind this type of emission process is very well understood as every light emitting diode (LED) is based on a forward biased pn junction.


The section begins with a brief review of the physics behind a pn junction under forward bias and an extension of that theory will be used to describe basic LED operation. This review will give a basis for the understanding the emission spectrum from silicon devices under forward bias.


Fig. 4 shows the band structure of a pn junction with no applied bias (top) and under a small forward bias(bottom). Applying a forward bias reduces the width of the depletion layer, lowers the barrier height for carrier transport across the junction, and splits the fermi level into quasi-fermi levels (indicating non-thermal equilibrium carrier concentrations on either side of the junction). Under this condition, the resistance across the junction will be very low, allowing little excess energy (energy greater than the bandgap energy) to be imparted to carriers. In the depletion approximation, all of the applied potential is theoretically placed across the depletion layer. Thus, the applied forward voltage acts against the built-in junction potential to reduce the electric fields across the depletion region.


At applied biases larger than the built-in potential, the depletion region and the electric field will cease to exist. A small field is created in the region where excess majority carriers are injected but acts mainly on the majority carriers to preserve space charge neutrality.


In this situation, electrical properties are dominated by minority carrier injection across the metallurgical junction. The equations that describe the minority carrier injection process can be found in most device physics textbooks [5, 6]. For electrons injected into the p-side of the junction, the electron diffusion current can be written


LnNa


N


L


qD


I


qV


2 i


f


For holes injected into the n-side of the junction, the hole diffusion current can be written


LpNd


2(N/T-2].i


In these equations, Vf is the applied forward bias voltage,Dn and Dp are the minority carrier diffusion coefficients,Ln and Lp are the minority carrier diffusion lengths and Nd and Naare the doping densities on the n- and p-sides of the


junction respectively. From these equations it is evident


that the current in an n+p junction will be dominated by electron injection into the p-side of the junction and most of the light emitted will be from radiative recombination taking place in the p-type material.


In addition to minority carrier diffusion currents, there will be a recombination current in the space charge region with a magnitude that is related to the width of the depletion region


rec


W


qn


τ


where τ is the carrier lifetime in the space charge layer and W is the depletion layer width. For forward biases,the depletion layer width decreases and eventually reaches zero where the recombination current, Irec,must also go to zero.


x


-xn


xp


Depletion layer


p-Si


n-Si


Ec


Ev


Vbi


Ef


εm


No applied bias


Vbi- Vf


Efn


Efp


Vf


Forward bias


Figure 4 pn junction in thermal equilibrium with no


applied bias (top) and with a small forward bias (bottom).


The final current component is from the tunneling of carriers across the junction. This current is significant only for heavily doped junctions.


Light emission from forward biased junctions, or electroluminescence, needs large numbers of electrons and holes to be co-located spatially and for those carriers to re-combine radiatively. Most LED designs started as simple diffused or grown junctions that inefficiently placed large concentrations of electrons and holes in a not so well confined area near one side of the junction. This process might be considered the“brute force” approach where light can be generated but with very low quantum efficiencies (much less than 0.1% of the electrical power is converted into optical power). As LED technologies are developed, the trend is to create abrupt changes in materials or heterojunctions where the sudden change in index of refraction is used to confine the injected carriers in a potential well to increase their recombination efficiency. With this design, external quantum efficiencies over 1% have been achieved. The most efficient LED designs create ultra-thin layers of material that form quantum wells where carrier confinement and the density of states are enhanced significantly. Quantum well LEDs with over 10%external quantum efficiency have been manufactured.


For ICs, the conditions will never be optimized to achieve efficient light emission from forward biased junctions. By the nature of the manufacturing process where heavily doped source and drain regions are needed to reduce contact resistances to transistors, very inefficient light emitters will result. In general, the recombination of electrons and holes under forward bias will be split between radiative (photon emission)and non-radiative (phonon emission) recombination.


The radiative recombination rate (or the spontaneous emission rate) is a function of the concentrations of electrons and holes or


Bnp


Rsp =


where B is the radiative recombination coefficient and n


units) Intensity (arb.Relative


and p are the electron and hole concentrations.


In indirect gap semiconductors, like silicon, nonradiative recombination will be dominated by Auger recombination. In Auger recombination, the energy released when an electron and hole recombine is transferred to another electron or hole instead of being emitted as a photon. The Auger recombination rate is related to the cube of the carrier concentration


A Cn R =


where C is the Auger recombination coefficient and n is the carrier density in the material. The Auger process dominates other forms of recombination when the concentrations of electrons and holes are high or when


high levels of carriers are injected across junctions.


These arguments suggest that in the normal source and drain junction regions found on most MOS technologies light will be emitted with very low efficiencies.


Based on the theory presented in this section, light emitted from a forward biased junction should not be spectrally broadened by the presence of high electric fields and thus should be centered around the bandgap of the material. The intensity of the emission should increase with the bias current and should not significantly broaden with the applied voltage. To test this assertion, a series of emission spectra were collected from the drain to body junction of an nchannel MOSFET from a 0.5 µm CMOS process. The resulting spectra are shown in Fig. 5 and demonstrate the relationship between forward current and emission intensity. If the spectra in Fig. 5 are normalized to the same peak intensity, the curves lay precisely on top of each other demonstrating the lack of broadening under increasing applied voltage. An interesting feature in Fig. 5 is the observed change in I-V characteristics that took place when the measurements were made. As the voltage was increased, hot carrier damage reduced the forward current for the 2.5 V and 3.0 V spectra.


Overall, the forward biased spectra demonstrate excellent correlation with the described theory. The only exception is the spectrometer’s inability to resolve a peak around the silicon bandgap (1100 nm). A spectrometer with near infrared sensitivity would resolve this peak.


1.2


3.0 V, 26.3 mA


2.5 V, 23.7 mA


2.0 V, 35.20 mA


1.5 V, 16.48 mA


Figure 5 Light emission spectra from a forward biased pn junction at various currents.


Reverse Biased pn Junctions


The physics behind light emission from a reverse biased pn junction is very different from that of a forward biased pn junction. Under reverse bias, the fermi level is again split into quasi-fermi levels but, in this case, the bias causes the depletion region to widen and the electric field across the junction to increase. This arrangement is illustrated in Fig. 6. The underlying physics can be understood mathematically using the


abrupt-junction model. In this model, the expression for the electric field is very simple with


R


bi −


ε


where W is the depletion layer width given by


[28si(NA+ND(


)7/%21


bi


Si


L9(NAND(Vbi-VR)VVNNNNq2


Vbi is the built-in potential across the junction, and VR is the applied reverse bias.


The current under reverse bias is dominated by tunneling and recombination in the space charge region instead of minority carrier injection as was described in the forward biased case. A general expression for the tunneling current density can be written


3q8h


π


= 1


q3


exp-4


exp


q


J


π212E221


*


t


where m* and q are the effective rest mass and electrical charge of the carrier, ε •is the electric field and Eg is band gap energy, h is Planck’s constant.


9


VR


Reverse bias


Figure 6 Reverse biased pn junction.


Avalanche multiplication or impact ionization of carriers under reverse bias conditions leads to junction breakdown. Under controlled conditions (i.e. where the current is limited), junctions can operate nondestructively while avalanche breakdown occurs. The additional carriers increase the intensity of the light emitted by the junction. The distribution of energy varies from the bandgap energy or less up to the applied reverse voltage. Most carriers lose varying amounts of energy through impact ionization creating an emission spectrum that is most intense near the bandgap energy and decreases toward higher energies (shorter wavelengths). The low energy limit is closely coupled to the applied reverse bias and the electric field across the depletion layer.


The same n-MOSFET drain junction used for the forward bias emission study shown in Fig. 5 was placed under reverse bias. The results in Fig. 7 show that the emission intensity at short wavelengths increases in relation to the bandgap emission as the reverse bias is increased. Light emission intensity in Fig. 7 increases with increasing electric field across the pn junction.


The light emission spectrum also broadens with increasing electric field across the pn junction. These spectra are in contrast to those for the forward biased condition that have little or no dependence on the electric field but have strong dependence on the minority carrier injection currents.


80.6 S0.8


1.0 C1.2!


u1.4 n


2.2


12.0 V


10.0 V


8.0 V


Figure 7 Light emission spectra from a reverse biased n+p junction at various voltages.


MOSFETs in Saturation


Since a number of defects can drive a transistor into saturation, many light-emitting defects encountered during failure analysis would fall within this category.


This section uses data collected from an n-channel MOSFET under various bias conditions as an example.


The spectra (Fig. 8) show that the visible light emission(< 770 nm) is controlled by the length of the pinchoff region in the transistor and the voltage across it. From basic device physics, it is well known that the drain to source current in a MOSFET in saturation is related to the gate to source voltage by


)2


TH


GS


eff


ox


DS Leff


L W


IDS=μCoxµ= ](VGS-VTH)2,,


where VGS is the applied gate to source voltage, VTH is the threshold voltage, µ is the carrier mobility, COX is the oxide capacitance, W is the channel width, and Leff is the effective channel length between source and drain diffusions.


The current is controlled by VGS modulating the width of the pinchoff region and thus, the electric field responsible for transporting carriers from the channel to the drain. Since the channel is pinched off at the point where the voltage between the source and drain is less than VGS – VTH, the electric field between the pinchoff point and the drain can be written as


'


DS


where L’ is the length of the pinched-off channel. As VGS decreases, the voltage across the pinchoff region increases while the length of the pinchoff region decreases; both effects increase the electric field between the source and drain. This effect is clearly demonstrated in Fig. 8 where the fraction of the light emitted at short wavelengths increases as VGS reduces toward the threshold voltage.


1.2 x 30 µm n-MOSFET VDS = 5.0 V


VSB = 0 V


4.25 V


3.75 V


3.125 V


2.5 V


2.0 V


1.75 V


VGS = 1.5 V


Figure 8 Light emission spectra from an n-channel


MOSFET at various gate voltages.


The spectra in Fig. 8 show a better match to the reverse biased junction emission (Fig. 7) than to the forward biased junction emission (Fig. 5). For both reverse biased and saturation emssion cases, the spectral content is strongest at wavelengths near the bandgap and the short wavelength components vary with the electric field and not the current. The similarities between Fig. 7 and Fig. 8 are important for circumstances where the spectral content of the light


emission is used for defect identification. A distinction can be made between a forward biased pn junction and a saturated transistor but not from a reversed biased junction.


Latchup


Latchup and snapback have been a concern for process and circuit designers for decades. Even with the advanced understanding of this phenomenon within the microelectronics community, failures still occur. The classic model for latchup in CMOS ICs uses two parasitic bipolar transistors connected to form a siliconcontrolled rectifier (SCR). When the SCR goes into its“ON” or low impedance state, all three of the SCR junctions are forward biased, placing the bipolar transistors in saturation. For these conditions, the expected emission spectrum is of the same general shape shown in Fig. 1 for a forward biased pn junction.


The difference is the relatively large area occupied by the parasitic SCR in comparison to a single pn junction and the resulting magnitude of current drawn by the circuit during latchup. For these reasons, the entry in Table 1 for latchup indicates that it is a low electric field process and should have a light emission spectrum that is dependent on minority carrier injection and bias current.


An example of light emitted during latchup is shown in Fig. 9. This sample was found to have a region where latchup could be triggered by a laser pulse (1064 nm,less than 100 mW). The laser pulse was used to identify the location of the affected circuitry. The light emission spots in Fig. 9 are relatively large indicating that an area much larger than a single transistor is involved. The spectrum taken from one of the light emitting sites is shown in Fig. 10. The spectrum is identical to that shown in Fig. 6 for a forward biased pn junction. In an earlier work on near-infrared (NIR)light emission analysis [1], it was argued that the spectral content would be strongest in the near infrared


Normalized Intensity (arb. units)


but would be detectable with a non-NIR camera because of the area involved. The small portion of the emitted energy in the visible would be easily detected because of the large number of photons generated by circuits in this condition.


Figure 9 Light emission from induced latchup.


Figure10 Light emission spectrum from latchup.


Gate Oxide Failures


The last case described in Table 1 was for gate oxide failures. In Table 1, the electric field associated with emission from gate oxide failures is listed as “mixed”.


“Mixed” in this case refers to the possibility that the electric field strongly depends on the quality of the resulting junction formed when the gate oxide breaks down. To demonstrate this theory, the gate oxide from an n-MOSFET was stressed to failure using a voltage ramp method where the voltage across the oxide was slowly increased until a sudden change in conductivity was observed. After the first change in conductivity,the emission spectrum was measured. The spectra,shown in Fig. 11, that were taken for gate biases of 6.0,


8.0 and 10.0 V strongly resemble spectra from a reverse biased pn junction except for the presence of an 825 nm peak in the 10.0 V spectrum. The presence of a peak at 825 nm indicates that most carriers are losing about 1.5 eV during their radiative transitions. As the voltage was increased to acquire a 12.0 V spectrum, a second abrupt change in conductivity was observed where the


current-voltage characteristics changed to resemble a forward biased pn junction. The spectrum in Fig. 11 for


1.0 V was measured after this change in conductivity.


This spectrum matches the forward biased pn junction indicating that a “better” junction had been formed.


It is clear from this analysis that the identification of a gate oxide failure from the light emission spectrum can be difficult and will depend on how the junction was formed and the voltage applied to it. Additional information such as the shape of the emission source(i.e. Does the emission come from a small spot or from a rectangle that has the dimensions of the transistor channel?) will be needed to avoid a false identification.


1.0 V


Figure 11 Emission spectra from a damaged gate oxide after one and two changes in conductivity.


Effects of Thin Dielectric Films on Transmitted Spectra


One of the observations made during this analysis was the presence of structure in some of the light emission spectra that could not be explained by known transitions in silicon-based devices. Examples of transitions that can lead to spectral features are transitions between impurity states and deep levels.


These transitions generate peaks in the emission spectrum that would be at lower energies (longer wavelengths) than the bandgap. The presence of short wavelength features indicates that other factors are influencing the emission spectrum.


口


The detected signal was preamplified by an Ithaco


do


Model 164 prior to being fed into an Ithaco Dynatrac


1.4141.4191.4241.42P1.484-201


393 Lock-In amplifier. The whole system was


Eminlion Photon Energy(av)


controlled by a personal computer. This system was also equipped with an electronic strobing or grating capability, so that it could determine the timing of the device performance and band edges of optical emission.


Electrical Measurements


Fig.11 shows the measured substrate hole current(dashed curve, ISub), and the drain current (full lines, ID)for a degraded device (Fig. 11a, device A), and for a fresh one (Fig. 11b, device B). Measurements were performed at different gate biases (VG). At zero gate voltage (VG=0), there is a clear difference between the degraded (Fig. 11a) and the fresh (Fig. 11b) device. The degraded device shows a high leakage current. Applying a small gate bias of 0.5 V allows for a channel current to flow between the source and the drain. Fig.11 indicates that indeed a channel current is measured in addition to the leakage current in the degraded device. In the fresh device only the channel current is observed. At VG = 1 V there is no significant difference anymore between the currents measured in device A and in device B. This shows that the channel current increases with VG, while the leakage current is not affected by a positive gate voltage. This demonstrates that the leakage current flows along a resistive path in the silicon bulk and is not influenced by interface traps at the gate oxide-substrate interface. It indicates that local perforation of the junctions generates this resistive path between the drain and the source. The number of these paths, as discussed by Bock [14] controls the leakage current.


For VG= 0 V, the drain current in device A is due to the leakage path formed between the drain and the source.


These electrons can reach a space charge region near the drain. They can gain enough energy there due to the drain electric field, hence impact ionization can occur.


From SPEM it was found that the electron temperature(energy) could only be affected by the drain voltage, and was not influenced by the degradation level, i.e. the magnitude of the leakage current. This confirms that the impact ionization occurs close to the drain, and not in the channel. Depletion of this resistor at relatively high drain voltages generates impact ionization at the drain junction.


The multiplication factor (M) is measured with the gate,substrate and source junctions firmly grounded. M is defined as the ratio between the substrate current and the source current (M =Isub/Is). Fig. 12 indicates this value


for the degraded device A and the fresh device B. The


measured multiplication factor from the leakage current


in device A has a similar dependence on the drain


voltage as the measured value from a good device after


applying a small bias to the gate. In addition, the


measured M for both devices shows a similar


dependence on the applied gate voltage. This again1 confirms that impact ionization occurs at the drain side


of the leakage path in the degraded devices. In addition,


it also explains that the failed devices can still reach


10-2


10-1 100 Intensity (a.u)101 102 103


6V, 951µA  5V, 367µA   4V, 206µA  3V, 120µA


Figure 10a Measured spectral distribution of the emitted


light at the failure site as a function of the drain bias for言the device with highest leakage current (367 µA at 5V,see Fig. 9).


5000


4000


t)3000


2000


1000比


5.5


5.0


4.5


VD (v)


Figure 10b Measured electron temperatures (Te)


determined from the light spectral distribution (Fig.10a)at different drain biases. A linear correlation with the drain voltage is observed.


snapback, as can be seen in Fig. 11a. The current through the leakage path generates holes due to impact ionization in the drain field. These holes can forward


bias the source-substrate junction. As a result, this can drive the device into the snapback biasing regime, even after the device has been failed.


10-12


10-10


a10-8王10-6 10-4


10-2  F


12


VD (V)


ID


|ISub|


a n s


VG=0.5V


VG=1V


VG=0V


a) Degraded (120nA @5V)


量


-12 10-10 10-8 10-6 10-4 10-2


(>


VD (v)VG=1V0


十


b) Non degraded


」


Figure 11 Measured drain current (full lines, ID),substrate current, (dotted lines, Isub) at different gate


重


bias in the range of 0 to 1V. a) Degraded device. b)


土


Fresh device.


10-5


10-4


10-3


∑10-2 10-1


101中


Non_Deg


Deg


0 Deg, VG=0V


Figure 12 Measured multiplication factor M for:Circles: degraded device at VG=0; Dotted lines:Degraded device at VG= 0.5, 1V; Full lines: Nondegraded device at VG=0.5, 1V. The multiplication factor for both devices has a similar dependence on the gate voltage.


In this paper, it was shown that micro-Raman spectroscopy is a useful technique to study the local stress and the local temperature in ESD protection devices (ggnMOS) along the width of the gate for different biasing conditions. A tensile stress was found near the gate.


Temperatures up to 200°C where obtained for currents up to 2mA/µm. A good correlation was found between light emitted by these devices, measured with PEM, and the local temperature.


Devices degraded by ESD stressing were also investigated by Raman spectroscopy, PEM and SEM.


PEM showed localized emission spots at the defect sites.


It was demonstrated that Raman spectroscopy can be used to locate the defect along the width of the gate.


This was confirmed by SEM. The Raman data also showed that the temperature at the defect site is not much higher than in the remaining part of the gate,indicating that the light emitted at this site is not due to a high local temperature.


From SPEM and electrical data it was concluded that the light emitted by the failure site is generated during electron impact ionization due to the high electric field at the drain, and it is certainly not due to a high local lattice temperature. This fact was further confirmed by the presence of a substrate hole current. In addition, it was shown that the multiplication factor of a damaged device was similar to the one of a fresh device. Again,this shows that for both cases the substrate hole current


has the same origin, i.e. impact ionization. It was also shown that the leakage path is not directly related to gate oxide interface traps.


The authors thank Bart Keppens for the TLP experiments, and Philippe Roussel and Veerle Simons for SEM measurements. Christian Russ is acknowledged for discussions and advice.


1) N. Khurana, T. Maloney, and W. Yeh, in Proc.


IRPS Symp., 1985, pp. 212-223.


2) A. Amerasekera, L. van Roozendaal, J. Abderhalden, J. Bruines, and L. Sevat, in Proc. EOS/ESD Symp., 1990, pp. 143-150.


3) M. Hannemann, A. Amerasekera, in Proc. ESREF Symp., 1990 pp. 77-83.


4) C. Duvvury, and A. Amerasekera, in Proc.


EOS/ESD Symp., 1995, pp. 162-173.


5) C. Russ, K. Bock, M. Rasras, I. De Wolf, G.


Groeseneken, and H. E. Maes, in Proc. EOS/ESD Symp, 1998, pp. 177-186.


6) M. Rasras, I. De Wolf, G. Groeseneken, and H. E.


Maes, Microelectronics and reliability Vol. 37: pp.


1596-1598 (1997).


7) De Wolf I., Semicond. Sci. Technol. 11, 19 (1996)


8) Raman and Luminescence Spectroscopy for Microelectronics. Catalogue of optical and physical parameters. (European Commission EUR 18595 -Nostradamus project SMT4-CT-95-2024), Ed. I. De Wolf, J. Jimenez, J.P. Landesman, C. Frigeri, P.


Braun, E. Da Silva, E. Calvet, 1998.


9) De Wolf I., Chapter 10: Semiconductors, in Analytical Applications of Raman Spectroscopy,Ed. M.J. Pelletier (Blackwell Science), 1999.


10) J. KÖlzer, C. Boit, A. Dallmann, G. Deboy, J. Otto,and D. Weinmann, J. Appl. Physics71 (11), 1992,pp. R23-R41.


11) Bude J., N. Sano and A. Yoshii. Phys. Rev. B, 45(11), pp. 5848, 1992.


12) L. Selmi, H. S. Wong, E. Sangiorgi, M. Lanzoni,and M. Manfredi, IEDM Tech. Dig., 1992, pp.131-134.


13) A. Toriumi, M. Yoshimi, M. Iwase, and K.


Taniguchi, IEDM Tech. Dig., 1985, pp.56-59.


14) K. Bock, C. Russ, G. Badenes, G. Groeseneken, and L. Deferm. In Proc. EOS/ESD Symp., 1997, pp.


308-315.


Electronic Device Failure Analysis Society, editor, p 77-83


DOI: 10.1361/cp1999istfa077


# Infrared Emission Spectroscopy as a Reliability Tool


Infrared Emission Spectroscopy as a Reliability Tool


Q. Kim and S. Kayali


Jet Propulsion Laboratory, California Institute of Technology, Pasadena, California


In this paper, we report on a non-destructive technique, based on IR emission spectroscopy, for measuring the temperature of a hot spot in the gate channel of a GaAs metal/semiconductor field effect transistor (MESFET). A submicron-size He-Ne laser provides the local excitation of the gate channel and the emitted photons are collected by a spectrophotometer. Given the state of our experimental test system, we estimate a spectral resolution of approximately 0.1 Angstroms and a spatial resolution


of approximately 0.9 µm, which is up to 100 times finer spatial resolution than can be obtained using the best available passive IR systems. The temperature


Figure 3 Direct and indirect band structure of


semiconductor device materials, involved in optical


emission including photons (ω), phonons (Ω) and excitons (ωe).


Many reports have appeared identifying various photoluminescence (PL) emission characteristics in GaAs multiple-quantum well devices. The spectral characteristics involving the intrinsic and extrinsic radiative recombination of free excitons have been well established to explain the device material quantum-well structures. The intrinsic emissions of the excitons have been observed even at room


temperature as dominant radiative transitions.[8-9]The temperature dependence PL spectra of many


B e a m R ef lecting↓Mir r or


different GaAs devices can be found elsewhere. [10-


E x p a n d e r


H e _ N e ↓ L a s e r


C h o p p e r 1 D U T


11]


One of the many practical applications of this spectral dependence of band shifts and broadening of device materials upon device temperatures is to predict the temperature of a powered device by


F i l t e r


calibrating an unpowered device at different


controlled temperatures. The true operating temperature of the micron-size powered GaAs MESFET local channel can then be found by measuring the shifts of the spectral band of the multi-quantum well devices.


In this paper we describe a novel, nondestructive


S p e c t ro p h ot o m e t er


experimental procedure for channel temperature measurement and then discuss the results of the actual measurements to summarize our conclusions.


The thermal dependence on PL from semiconductor material has been well understood in principle, but it has been difficult to utilize optical techniques to measure the emission spectrum from a fabricated device until the advancement of optical manipulation techniques and computer image processing technology. The technology can now precisely locate a one-micron diameter exciting laser beam, such as a helium-neon laser, on positions of IC components that are most vulnerable to thermal degradation due to high power or stress. The PL light collected


nondestructively from a specific component of a fabricated device at cooled (84.8 K) and room


w e


temperature can then supply device inforormation,


C o n d ucti on ↓B a n d↓E dge W r


including the temperature profile of the device


4 ↓ ↓ E x c it o n↓E ner g y ↓ L e v e l


) 丄


component. The cooling was achieved by the miniature Joule-Thomspon refrigerator from MMR


V a le n ce↓ B a n d↓E d g e


Technologies, Inc.


This method utilizes the latest optical manipulating system, triple grating spectrophotometer technology and up-to-date computer image processing techniques


0  k


0 k


to precisely locate the emission source of the ICs


most vulnerable to power system operation.[12-13] A dual micromanipulator is coupled to a thermoelectrically cooled photomultiplier tube (PMT),wavelength scanning system, and conventional lockin amplifier to detect and amplify the extremely fine device response or photoluminescence (PL) light of the IC gate materials. Computer data processing techniques were employed to boost system sensitivity for signal analysis.


Figure 4 shows a diagram of the PL measurement system. The technique uses a well-focused incident laser beam to generate electron-hole pairs in the semiconductor gate material.


Figure 4 Diagram of channel temperature


measurement system.


The basic setup consists of three major parts: (a) an optical probing stage with a microscope, (b) a gated monochromatic-intensifier with a cooled photomultiplier tube and, (c) data processing and control computer. The micromanipulator adjusts a specific gate portion of a device under test onto the miniaturized focused probing helium-neon ion laser beam. This allows the illuminating photons to excite the valance band electrons to conduction bands in the active channel of the GaAs MESFET. Some of the free electrons and holes will bind together to form excitons near the doping ions next to the conduction bands. Some of these impurity bound excitons will be de-excited into the valence band by interacting


with the excitons and the lattice phonons. When this transition occurs the photons will be emitted in all directions. The spectrophotometer monitors the emission spectrum modulated by the excitons near to


POD


the conduction bands. The emission exciton bands


Unpowered


will be modulated by the lattice phonons, which


好800


Pdwered


represent the temperature information of the


n600U


microelectronic device under tests. The spectro-


甲


E400


photometer used for these tests was Jarrell-Ash


2OD


Monspec 27. A thermoelectrically cooled photo-


管


multiplier tube (Hamamatsu R943-02/RCA 31032)


ltyintena莒


was used for the detection of the spectrophotometer.


resolution (<0.02 K/µm in our case) is dependent upon the spectrometer used and can be further improved. This novel technique can be used to estimate device lifetimes for critical applications and measure the channel temperature of devices under actual operating conditions. Another potential use is cost-effective prescreening for determining the 'hot spot' channel temperature of devices under normal operating conditions, which can further improve device design, yield enhancement, and reliable operation. Results are shown for both a powered and unpowered MESFET, demonstrating the strength of our infrared emission spectroscopy technique as a reliability tool.


Thermal and mechanical failures on ICs in interconnect metallization and multilayer structures of advanced microelectronic devices have been recognized in the application of many commercial, military and space projects. Thermal degradation induces electrical and mechanical stress on power transistors.


Precise knowledge of the local channel temperature of a GaAs Power MESFET during operation is critical to determining the expected lifetime and overall device reliability.


The polarized liquid crystal technique, which is destructive, has been utilized for estimating device


temperatures with a spatial resolution of about 1µm.


On the other hand, non-destructive passive infrared temperature measurement techniques provide temperature measurements with a spatial resolution of


15 µm, which is too coarse for determining local distribution of state-of-the-art microelectronic device temperatures with submicron gate structures.


We have developed an alternative optical technique based on visible/near infrared emission spectroscopy to provide high resolution, non-destructive channel temperature measurements of the hot spot in the gate channel of a GaAs MESFET.


The development of laser action in crystals doped with magnetic ions has brought a great interest to the field of solid state spectroscopy. The knowledge of the energy levels and transitions of a fluorescent system can be expanded by spectroscopic research.


Also the presence of lattice vibrations gives rise to temperature dependent effects in the observed


spectra[1]. Interpretation of these effects can yield information concerning the interaction of host lattice phonons with the electrons on the impurity/doped ions.


An isolated impurity/doped ion in an excited electronic state can decay by three processes: (1)radiative decay through an electronic transition,giving rise to the emission of a photon; (2)radiationless decay through a vibrational transition,giving rise to the emission of phonons; and (3)vibronic decay through a coupled vibrationalelectronic transition, giving rise to the absorption or emission of a phonon with the emission of a photon.


The inverse of the fluorescence decay time of the excited state will be the sum of the decay probabilities of these three processes. Analogous excitation processes occur in the absorption of light by the impurity or doped ions. Electronic transitions


provide information on the energy levels of the impurity ion while radiationless and vibronic transitions provide information on the electronphonon interaction.[1]


Radiative and vibronic transitions can be observed directly in optical spectra whereas radiationless transitions are observed only indirectly through the temperature dependence of spectroscopic data.


Figure 1 shows a diagram of vibronic and radiative transitions in both absorption and emission. The radiative transitions give rise to zero-phonon lines in the spectra. Vibronic sidebands will appear on both the low energy and high energy side of these lines.


In absorption spectra the low energy vibronics are


Zero-phonon line


due to the concurrent absorption of a photon and a phonon whereas in the fluorescence spectra the low


(a) Weak Interactions


energy vibronics are due to the concurrent emission


Vibronic Sidebads


of a photon and a phonon. Similarly, the high energy vibronics in absorption are due to the simultaneous absorption of a photon and emission of a phonon while in the fluorescence spectra they are due to the


INTENSITY


(b)Intermediate Interactions


simultaneous emission of a photon and absorption of a phonon. Thus, the absorption and emission spectra should appear as mirror images on either side of the zero-phonon line. However, since the intensity of these sidebands is proportional to the probability of absorption or emission of phonons, the low energy


(c)Strong Interactions


absorption vibronics and high energy emission


vibronics are generally not observed at low temperatures where few phonons are available for absorption.


WAVELENGTH


Figure 1 Diagrams of vibronic and radiative


transitions for both in absorption (a)


and in emission (b) of photons.


Three types of spectral profiles can be observed,depending on strength of the electron-phonon interaction. These are shown in Figure 2 for typical fluorescence spectra. For weak electron-phonon interaction most of the emission occurs purely radiatively. This gives rise to a very intense zerophonon line with a weak, structured vibronic sideband consisting mostly of one-phonon emission


transitions. As the strength of the electron-phonon interaction increases more emission occurs in the vibronic sideband and less in the zero-phonon line.


The vibronic bands can be much broader and less structured when multi-phonon transitions are important and in some cases the zero-phonon line is not observed at all. As temperature is increased the relative intensities and shape of the vibronic sidebands change due to the change in the probability of absorbing and emitting phonons. Phonon scattering and radiationless transitions also cause a change in the width and position of the zero-phonon line with temperature.


E1↑台°一Phonons


女Phonons


Figure 2 Three types of profiles in optical spectra for weak(a), intermediate (b), and strong (c) electronphonon/exciton interactions.


There are two purposes for studying the spectra of


Photons


impurities in solids: to characterize and understand


Zerothe optical properties of the system; and to obtain


Zerophonon


information on the phonons of the host crystal and


phonon


line


how they interact with the electrons on the impurity.


E0


This paper is concerned mainly with the latter purpose. This information on the lattice dynamics is


Absorption


Emission


interesting because of the important role played by phonons in the thermal, electrical, and optical


properties of solids.


The most powerful technique currently used for studying lattice vibrations is neutron scattering.


Despite the wealth of information which has been obtained from this technique, it does have some limitations such as the need for expensive equipment,a relatively low resolution, and the fact some materials cannot be investigated because they have a low scattering cross section or high absorption cross section for neutrons. Infrared absorption and Raman and Brillouin light scattering provide complimentary techniques for investigating lattice vibrations. These methods have higher resolution than neutron


scattering but first order phonon processes are limited to the center of Brillouin zone by momentum conservation. Second order processes are not subject to this restriction but it is usually quite difficult to unfold the combined density of phonon states. These techniques are also limited by rigorous selection rules.


Perhaps the most attractive feature of vibronic spectroscopy for investigating lattice vibrations is that, compared with the other methods, it is a very


simple and inexpensive experimental technique [2]. It also has been shown that information on phonon eigenvectors as well as eigenfrequencies can be obtained from vibronic studies, which is not available


by other methods [3]. Phonons from all parts of the Brillouin zone may be active in vibronic transitions although they are subject to certain selection rules.


These phonons can be identified even though it is sometimes quite complicated to do so. One of the major problems in using vibronic spectra is that the presence of an impurity center may perturb the lattice modes or introduce local vibrational modes which must be distinguished from the normal lattice modes.


It is important to note that the structure observed in vibronic spectra represents an effective phonon distribution (weighted by the electron-phonon interaction) and not the actual phonon density of states of the crystal. This information is useful itself in understanding the absorption and luminescence properties of the systems and how they change with temperature. It is also possible to use this data to obtain information concerning the lattice dynamics of the host crystal. However, this involves determining the frequency dependence of the electron-phonon coupling parameters. Two methods have been used to do this: One is to assume a simple model for the coupling parameters and use the long wavelength


limit of their frequency dependence [4]. This can then be divided out of the measured effective phonon distribution leaving the phonon density of states of the pure crystal. The second method is to formulate from first principles a lattice dynamic model for the crystal with an impurity and from this calculate the


predicted shape of the vibronic sidebands[3]. This is by far the most elegant technique for interpreting vibronic spectra and using it makes vibronic spectroscopy the most powerful method for studying lattice dynamics. However, this is a very complicated procedure and to avoid the use of many adjustable parameters in the model it is necessary to have a significant amount of other experimental data available on the crystal. In many cases the first,simpler method gives a good approximation to the true phonon density of states. It should be noted that all of the information on lattice phonons is contained in the one-phonon sideband and in both techniques this must first be projected out of the total observed vibronic spectra.


Based on the theory of lattice dynamics, band shifts and broadening of solid state semiconductor device crystal materials due to temperature variation have been well understood in principal. The thermal shift of a radiative optical spectral line is the statistical algebraic sum of the shifts of the two levels involved in the transition allowed by the selection rules of the electron-phonon interaction as shown in equation (1).


δ Ei =(


Ej(<i|H|j><j|H|i>)


><


Where


<i⏐( <j⏐) and EI ( Ej) are the initial(intermediate) quantum states and energy levels,


H’ = iV1q


1 2一


Mv


4πMv2诸


H'=iV1Σq


ω


(bq - bq+),


H” = - V2


Σqq(@q@q)(bq-bq+)


4πMv2π 2Mv4hh)qq'(ωq ωq')(bq - bq+)*(bq' - bq'+), and


H = Hlatt + Hion,exc + Hint ,


Hlatt = k (hωk)1/2(akak+ + Hatt= ∑k (hok)1/2(akak++1),1),


Hion,exc = Ho + Hcryst + Hso,


Hint =V1ε + V2 ε2 + …..,


ε =iV1Σq= iV1q


q险


πω


H: ion-vibration interaction Hamiltonian,


h: Plank's constant,


V1,V2: interaction matrix constants,


ωk,ωq: photon and phonon frequency,


M, v: Mass and velocity of the electron,


ak,bq, and ak+, bq+: annihilation and creation operators of photons and phonons.


However, the crystalline field at the ion, varying in time with the thermal lattice vibrations (phonons) of the neighboring ions, sets up an interaction between the ionic system and the normal modes of the lattice vibrations in the semiconductor lattice. The lattice vibrations include the local vibrational modes and the neutral excited mobile states (excitons) of a crystal bound to neutral donors and acceptors in doped semiconducting materials. Such interaction information obtained from spectral lines has been used in the past to explain the temperature dependence of the relaxation time of crystal ions in semiconductor band structures, as shown in Figure 3. The width of a spectral line is the statistical sum of the energy spread of the two energy levels involved and may also be


broadened by the same mechanisms. [5-7]


A micromanipulator stage with a resolution of 0.1


µm was used to position the device under test so that the laser beam exclusively impinges at the desired position of the device. Light emitted from the illuminated spot on the device was reflected by a beam splitter to a chopper and then focused onto the spectrometer slit. The light signal was also low-pass filtered to discriminate against illuminating laser wavelength. The output of the lock-in amplifier is digitized, and then processed in a personal computer to obtain the spectrum of infrared emission stimulated by the laser beam.


Figure 5 Cross-section of a typical GaAs MESFET.


The GaAs power MESFETs (see Figure 5) used for this investigation were mounted on a Cu/W carrier,and the JPL hybrid laboratory bonded the wires for controlling gates and power supply.


Results and Discussion


The emission spectrum of commercially available GaAs MESFETs was reproduced to identify the reported donor bounded exciton bands with no power applied, at temperatures of 84.8 and 299.1 K. Not shown in Figure 6, the emission peak at a wavelength of 1.41373 eV for the higher temperature (299.1 K)


exceeded the emission peak for the lower temperature(84.8 K) by about 16.30 meV.


Figure 6 Typical Emission Spectrum of the powered


and unpowered GaAs MESFET Gate at 84.8 K.


In another measurement run of the same setup,indicated in the Figure 6, the exterior of the device was maintained at 84.8 K and power was applied; the emission peak of 1.42265 eV for this case was shifted by 7.38 meV from the zero power case at 84.8 K. By linear extrapolation, this wavelength shift indicates that under power, the temperature of the gate rose about 97.3 K above the device operating temperature of 84.8 K.


The obtained results were in general agreement with


theoretical calculations [5-8] using equation (2), which is derived from equation (1):


Ecv (T) – Ecv (To) = - α (T+β)


where,


Source


Drain


T = Channel Temperature To = Operating Temperature Ecv = Energy Bandgap


n-GaAs


α = Slope of the Extended Plot (Fitting parameter)


Semi-Insulating GaAs


β = Debye Temperature (Fitting parameter).


The test system constructed, utilizing for general setup the Microelectronic Advanced Laser Scanner(MEALS), was reported elsewhere[12-13]. Utilizing the micromanipulator stage, a He-Ne laser beam


(λ=6238 Angstrom) with a beam diameter of 0.9 microns was precisely adjusted to the exact gate


position (resolution less than 0.1 µm) of the GaAs MESFET device. Discrimination of the emission light signal from the illuminating light was achieved by placing a low-band pass filter between the reflecting mirror (beam splitter) and the spectrometer,as shown in Figure 4. A lock-in amplifier, equipped with a cooled photomultiplier tube, was used for the detection of standard synchronous signals. Data collection and manipulation was performed using a personal computer with the appropriate software tools.


A commercially available GaAs MESFET, with gate dimensions of 0.5 micron (refer Figure 5), was mounted in the test fixture and emission spectra were successfully obtained. The emission spectrum obtained by this test setup, shown in Figure 6,indicates that this technique can be effectively manipulated to collect extremely faint gate emission spectra. The collected emission spectrum(shown in Figure 6) from the free excitons were identified and measured at an operating temperature of 84.8 K. The free exciton emission band shift of the unpowered GaAs MESFET gate was calibrated by the two different temperatures of 299.1 and 84.8 K. The shift was 16.30 meV. In order to remotely measure the local temperature rise of the gate due to the device operation, the emission band shift of the same gate from unpowered to powered were monitored at one(84.8 K) of the calibrated low temperatures. The shift was 7.38 meV.


The technique exploits the temperature dependence of the wavelength of the peak of the stimulated infrared emission spectrum. This wavelength increases approximately linearly with temperature – a consequence of the fact that the energy band gap of these semiconductor material decreases with temperature. Thus, if the temperature dependence of this wavelength is known, it can be used to determine the local temperature in the device while operating at various power levels.


It is well known that the emission bandshift of a semiconductor material is inversely proportional to


the material temperature [6-11] due to the first approximation of the electron-exciton interaction at this temperature range. Thus utilizing the bandshifts,one can calculate the localized hot gate temperature rise of the powered device under test. Equation (1)and information summarized in Table I reveal that the localized hot gate temperature of the device rose by 97.0 K during the operation at 84.8 K. The temperature rise was also compared with the conventional IR measurement technique, which has a resolution between 15 and 100 microns. The average temperature rise with this conventional technique was about 88.8 K. The main difference probably is due to the size of the measurement objective. The temperature rise measured by the infrared radiation technique is not the true local gate temperature but averages temperature of the gate with other parts of the device.


Table I Summary of Band Shift Data


|Test |Band Position (eV) |Power Applied ||
|---|---|---|---|

|Temperature |Band Position (eV) |Power Applied ||

|299.1K |1.41373 |No ||

|84.8 K |1.42265 |Yes ||

|84.8 K |1.43003 |No ||

Gate Temperature Rise


= T–To


= (299.1 K– 84.8 K) x (1.43003


–1.42265)/(1.43003–1.41373)


= 97.0 K.


A lifetime prediction of a device such as power MESFETs is based on the activation energy calculated by a distribution of mean time to failure(MTTF) at different device operating temperatures.


One of the most (VENERABLE) portions of the power GaAs MESFETs is the gate. Thus measuring the correct device operating temperature has a vital impact on product reliability.


Industry-wide implementation of this technique for most semiconductor devices, including silicon devices, requires only minor equipment modifications;the addition of a miniature spectrometer and a refrigerator to the existing micromanipulator under the microscope. The cryogenic system may not even be needed for some semiconductor devices if a known strong impurity spectrum near the band gap is used as the probing tool.


In this paper, a new non-destructive submicron-size spot temperature assessment technique based on visible/near infrared emission spectroscopy was discussed. It was demonstrated on commercially available GaAs MESFETs and found to have general agreement with calculated results.. A non-destructive submicron-size spot laser beam provided by a He-Ne laser was used to excite an extremely small local area of the gate channel of a GaAs MESFET under various operating conditions. The data collected shows a much higher localized “hot spot” temperature of the device than observed using typical IR techniques. This is due to the high-resolution capabilities of this technique. Given the state of the experimental test system, we estimate a spatial resolution of about 0.9 microns and a spectral resolution of about 0.1 Angstroms. This provides 15 -100 times finer spatial resolution than can be obtained using the best passive IR systems available.


The temperature resolution (< 0.02 K/µm) of this technique depends upon the spectrometer used, and can be further improved.


The authors are grateful to their numerous colleagues for providing technical information for this paper including Charles T. Crusan, R. Ruiz, Duc T. Vu,Russel A. Lawton. and James O. Okuno of JPL


The research described in this paper was carried out by the Center for Space Microelectronics Technology, Jet Propulsion Laboratory, California Institute of Technology, under a contract with the National Aeronautics and Space Administration.


Reference herein to any specific commercial product,process, or service by trade name, trademark,manufacturer, or otherwise, does not constitute or imply endorsement by the United States Government or the Jet Propulsion Laboratory, California Institute of Technology.


1) Baldassare Di Bartolo, Optical Interactions in Solids, John Wiley & Sons, Inc,, New York,


1968.


2) Analysis of the Vibronic Spectrum of Chromium Doped Strontium Titanate, Q. Kim, Richard C.


Powell, and T.M. Wilson,Phys. Rev. B, 12, p.


5627, 1975.


3) W. E. Born, Phys. Rev. Vol 185, 1969.


4) A. A. Maradudin, Solid State Physics, Vol. 18, p.


273, edited by F. Zeits and D. Turnbull,Academic Press, New York, 1966.


5) A. Kiel, Thermal Broadening of the Moessbauer Line and Narrow-Line Electronic Spectra in Solids, Phys. Rev. 126, p. 1292, 1962.


6) R. H. Silsbee, Thermal Broadening of the Moesbauer Line and Narrow Line Electronic Spectra in Solids, Phys. Rev. 128, p.1726, 1962.


7) C. D. Thurmond, The Standard Thermodynamic Functions for the Formation of Electrons and Holes in Ge, Si, GaAs, and GaP, J. Electrochem.


Soc. 122, p.1133, 1975.


8) M. I. Nathan and G. Burns, Recombination Radiation in GaAs, Phys. Rev. 129, p. 125, 1963.


9) J. C. Sarace, R. H. Kaiser, J. M. Whelan and R.


C. C. Leite, Injection Luminecsence in GaAs by Direct Hole-Electron Recombination, Phys. Rev.


137, p. A623, 1965.


10) R. C. Miller, D. A. Kleinman, W. A. Nordland,Jr., and A. C. Gossard, Luminescence studies of optically pumped quantum wells in GaAsAlxGa1-xAs multilayer structures, Phys. Rev.B,


22, p. 863, (1980)


11) P. W. Yu, S. Shaudhuri, D. C. Reynolds, K. K.


Bajaj, C. W. Litton, W. T. Masselink, R. Fischer,and H. Morkoc, Temperature Dependence of Sharp Line photoluminescence in GaAs-Al0.25 Ga0.75 As Multiple Quantum Well Structure,Solid State Comm., 54, p. 159, 1985.


12) [Q. Kim, and George Soli, Laser Scanner Tests for Single Event Upsets, NASA Tech Briefs, 16, p.56 , 1992.


13) S. K. Mendis, S. E. Kemeny, R. C. Gee, B. Pain,Q. Kim, and E. R. Fossum, CMOS Active Pixel Image Sensors for Highly Integrated Image System, IEEE J. of Solid-State Circuits, 32,p.187, 1997.


Electronic Device Failure Analysis Society, editor, p 87-96


DOI: 10.1361/cp1999istfa087


# Quantitative E-beam Probe for Valid High-Speed Measurements


Quantitative E-beam Probe for Valid High-Speed Measurements


C. T. Salling*


Micron Technology Texas, Richardson, Texas


*Current Address: Dallas Semiconductor, Dallas, Texas


The development of semiconductor products increasingly requires doing high-speed measurements with internal probe. For high-speed DRAMs, this demands a combination of sub-20 fF capacitance, sub100ps sampling time, and sub-20ps accuracy that is not available with commercial mechanical probes.


Commercial e-beam probers are the most promising tool, but their suitability for accurate measurements has not been determined. This paper reports the timing accuracy for the IDS-10K+ prober to establish the basis for quantitative high-speed measurements.


The ultimate accuracy of the IDS-10K+ is determined by inherent errors due to timebase inaccuracy and voltage noise. These factors yield a uncertainty of ±.


60ps when measuring time intervals of 500 ps or longer, ± 10% for intervals in the range 80-500ps, and a minimum error of ± 8ps for intervals shorter than 80ps. Timebase drift causes an additional uncertainty of less than ± 20 ps over a 4 hour period.


Internal signals were measured on DRAM circuits to determine the effect of all errors. Simple methods are shown for measuring sub-100ps edges and for determining the sampling time. The minimum sampling time is shown to be 65ps for a 40ps pulsewidth. Edge positions were repeatedly measured to quickly determine the uncertainty from all random errors. For sub-500ps edges, this is less than ± 10 ps for metal probe points and ± 16 ps for passivated circuits. For edges with transition times longer than 500ps, the uncertainty increases with transition time.


This is consistent with the observed distortion of these waveforms by a changing low-frequency background,so that timing accuracy becomes dominated by voltage errors for slow edges.


Mechanical probe and e-beam measurements of delay times were compared for a set of 9 signals. The observed 30-400 ps discrepancy cannot be explained by the effect of the mechanical probe's risetime or load capacitance. The largest disagreement occurs in a particular region of the circuit and the discrepancy increases with transition time. It appears that local interference is the dominant source of errors that are not inherent to the prober. When the interference is synchronous with the test cycle, systemmatic errors result. When the interference is asynchronous, random errors are produced.


FIB probe points were made on a passivated sample to compare delays times measured on bare metal and on the passivation surface. Edges probed on the passivation were shifted by ± 20 ps with respect to bare metal.


The sources of error are now sufficiently characterized to use the IDS-10K+ for valid high-speed internal probe, in which the uncertainty for any given measurement is already known or readily determined.


A new approach to internal probe is needed to develop integrated circuits with data rates exceeding 400MHz.


For example, in DRAM circuits, it is necessary to


measure 200ps transitions on 20 fF nodes, and subnanosecond delays with sub-20ps accuracy.


Commercial mechanical probes (Pico-probe) do not provide the combination of small capacitance and fast response time that is required for high-speed internal probe. Commercial e-beam probers (Schlumberger)promise zero load capaci-tance and 40ps beam pulsewidth. However, they are generally not used for quantitative high-speed measurements, because their timing accuracy has not established. Other options,such as backside optical probes or AFM-based mechanical probes, are generally considered to be still under development.


Throughput has become more of an issue than ever,due to the proliferation of new circuit designs. E-beam provides high throughput because it can probe the passivation over a circuit node. This capability has led to the extensive use of e-beam for fault location in logic circuits, where sub-100ps accuracy is not required. The dominant tools for e-beam probe in the semiconductor industry are the IDS-10K and IDS-5K series tools manufactured by Schlumberger.


In this paper, the sources of error for timing measurements are analyzed and experimentally quantified for the IDS-10K+ e-beam prober. All measurements were done at room temperature with a working distance of ~10mm. The beam current was 5 nA (HR mode) or 15 nA (Normal mode). DRAM circuits were probed as die on wafers and exercised with simple Write/Read tests using a Tektronix 9003 pattern generator.


Uncertainty in Timing Measurements


Timing measurements consist of measuring a time interval, t, on a signal or set of signals. Two commonly measured time intervals (Fig.1) are the delay time,tAB, between transitions on signals A and B, and the transition time, tT , of a single edge. In general, time intervals are measured between individual points, tj ,on a discrete time axis. These endpoints are defined by particular voltage values on the signal. For delay times, the points tj are defined to be at midpoints of edges A and B, where the voltage is 50% of the transition amplitude. For transition times, the interval is defined by the 10% and 90% voltage points.


These measurements can be analyzed in terms of the uncertainty, δtj, in measuring the position of any given point on the voltage waveform. If the each endpoint, tj,of an interval has a 3σ uncertainty ±δtj, then the 3σ uncertainty in the measured interval is simplyδt = ± 2 δtj .


Figure 1 The intervals tAB (delay time) and tT


(transition time) showing the endpoints, tj , that define them. The uncertainty , ±δt , in any interval can be found by determining the errors, ±δtj , for arbitrary time points.


There are a variety potential contributions to uncertainty in an e-beam timing measurement. The potential errors occur by three basic mechanisms: (1)direct shifts of the tjaway from their correct positions along the scope time axis, (2) noise and other voltage errors which lead to incorrectly locating the tj , since these are defined by voltage values along the signal,and (3) errors in placing the scope measurement cursors.


The errors also fall into two groups, according to how they behave. The first group is inherent to the prober.


They originate in its timebase, voltage measurement system, finite sampling time, and discrete time axis.


They are reproducible factors in every measurement and can be readily characterized. Most of these can be minimized and some turn out to be insignificant.


However, these errors determine the ultimate accuracy that can be obtained with the tool. The second group strongly depends upon the signal and circuits being measured. They are errors due to interference,charging, contamination, circuit geometry and probe placement. They change with time and location on a circuit. The only efficient course is to determine their effect on repeatability and understand them from a few specific cases.


Inherent Sources of Error


The errors inherent to an e-beam prober are not correlated. Thus the total, best-case uncertainty in a measured interval can be estimated from the individual errors due to the timebase, voltage measurement,sampling time, and discrete time axis:


δt=(δt2timebase+δt2voltage+δt2sampling+δt2discrete)1/2 (1)


This expression can be applied to find the uncertainty in the measurement of a delay time, transition time,clock period, or any other interval.


Discrete Time Axis


The time axis of the scope tool on the IDS probers is discrete, just as for a digitizing oscilloscope. There are 50 time points per division. Thus, for a given time/division setting, the interval between successive data points is 0.02(time/div). To measure an arbitrary time interval, the operator places cursors at the endpoints and the value of the interval is displayed. In most cases, endpoints do not happen to coincide with the scope data points. The worst case is when they fall mid-way between successive data points. Then, the error in measuring each end of the interval is


0.01(time/div). Thus, without interpolating between data points, the discrete time axis adds an uncertainty to interval measurements that is given by:


δtdiscrete = = ± 0.02 (time/div)


The fastest time scale on the IDS-10K+ and IDS-10K is 50ps/div. Thus the above error can be reduced to ±1ps, insignificant compared to other errors.


Timebase


E-beam probers use electron sampling pulses to


determine a circuit node's potential at one instance in


time and displays this data point on the scope window.


This process is repeated until a waveform is


constructed from many individual data points. The


timebase creates a delay between the time when a


trigger pulse appears at the prober's trigger input and


the time, tj, when the electron sampling pulse arrives


at the probed surface. The timebase inaccuracy is the


difference between the actual time tjwhen the signal is


being sampled and the time where the resulting data


point is displayed on the scope's horizontal axis. In


addition to the trigger pulse, an external clock can be


supplied to the IDS-10K+ to reduce timebase


inaccuracy. The external clock is a copy of the clock0


signal that is sent to the device under test. The3


timebase counts out a user-defined number of clock


cycles and then sets relatively short delays to acquire


the desired set of waveforms. The external clock


mode was used for all of the timing measurements


reported in this paper.


Experiments show that the measured position of an


edge depends upon beam energy, pulsewidth, and


acquisition mode (linear or random). Thus, the same


values for these parameters were used within any


given set of measurements.


The timebase inaccuracy was measured over a 12ns


interval using the 1 GHz sine wave signal from an HP8660 frequency synthesizer as a time standard. The sine wave traveled along a 50 Ohm coaxial cable to a bare metal surface in the IDS-10K+ and then into the 50 Ohm input of a Tektronix 784C oscilloscope. An early zero crossing of the sine wave was chosen as a reference point. The times corresponding to various voltages were measured with respect to the reference point using the IDS-10K+ and the Tektronix 784C.


The reported error is the difference between the measured time points and the model values from a mathematical sine function. For example, the time to the first zero crossing after the reference point is


500.00 ps for a pure 1GHz sine wave. The measurements were done using the 500ps/div time scale on both tools. Thus, cursor placement errors add an uncertainty of ±5ps to the measurements. The reported error is an overestimate of the timebase inaccuracy because it includes any deviation of the measured signal from a pure sine wave, due to an imperfect source or nonlinearity in the fixturing.


The plots in Figures 2 and 3 show the measured timebase error for an individual time point as a function of the its position along the scope time axis.


The plot in Fig. 2 shows the error measured using just the zero crossings of the sine wave. The worst-case error is +40ps/-20ps for the IDS-10K+ and +10ps/-5ps for the Tektronix 784C oscilloscope. The plot in Fig. 3 shows a magnified view of the 0-1000ps region of Fig. 2. In this measurement, 17 data points over the 1000 ps interval were compared to model values for one cycle of a pure sine wave. This data shows that there are 5ps fluctuations over intervals of 50ps. To be cautious, assume these fluctuations can be present over shorter intervals, where there is no data.


Figure 2 Timebase inaccuracy for the IDS-10K+


(diamonds) and the Tektronix 784C (squares) over a 12ns interval of the scope time axis.


-20


-10」0 10 S


a20 30 40 50


8000


12000


Scope Time Axis (ps)


Figure 3 Detailed structure of timebase inaccuracy for the IDS-10K+ over the 0-1ns interval in Fig. 2.


For delay times measured between two signals, there is also an error from drift in the timebase, tester, or device. Drift won't be a problem if the external clock feature is used and if the prober triggers off the clock instead of still using the trigger edge. However, this has not been checked experimentally. Figure 4 shows the result of repeatedly measuring a 130ps edge in a DRAM with respect to a reference point on the scope time axis. The edge was measured over a period of 4 hours, and was found to move, on the average, to earlier positions on the time axis. Since the pattern generator was powered on only 20 minutes before the start of these measurements, these measurements include the effect of all sources of drift as well as all other random sources of error. Since the peak to peak variation of a edge position is 20ps, the uncertainty in the timebase errors functions (Figures 2 and 3) due to timebase drift is less than ± 10 ps. The repeatability data for seven sub-500ps edges, shown in Fig. 8 ,support this conclusion.


Figure 4 The position of a repeatedly measured edge(with respect to an arbitrary time point) as a function of elapsed time since the first measurement. The curve is a guide to the eye.


Since the timebase errors are relatively stable over a measurement session, we can use the plots in Figures 2 and 3 to estimate its magnitude. By examining these plots, one can see that the worst-case error for any given time interval is set by the maximum differential error for that interval, regardless of where it occurs along the scope time axis. For example, the worst-case error for intervals of 500ps or less is set by the steep positively sloped region that begins at 2000ps in Fig. 3 and the steep negatively sloped region that ends at 4000ps. Consider measurements of two 500 ps delay times between edges which occur at the ends of these two steep regions. The error is + 50ps for the first delay and -30ps for the second delay. There are a number of similar steep regions for delays longer than 500 ps. Thus, a simple and cautious characterization of the timebase error is to say that it is ± 50 ps for intervals of 500ps or more. For delays shorter than 500ps, the worst-case error is when the interval occurs on the steep slope, where the error is ±10% of the measured interval. Finally, the worst-case error for intervals shorter than 80ps can be estimated as ±5ps from the plot in Fig. 3. These results are summarized in Fig. 7 .


Voltage Errors


E-beam probers use an indirect method to determine circuit voltages. The potential on the probed surface shifts the energy distribution of the secondary electrons. This changes the fraction of them that make it past a retarding grid on their way to the secondary electron detector. A feedback circuit adjusts the grid potential to maintain a constant detector current. Thus,the grid potential tracks the voltage on the surface. The feedback circuit must make many corrections to converge correctly to the probed potential. Each data point displayed along the scope face is the result of many electron pulses, on successive test cycles,sampling the circuit at a particular time.


The random noise on e-beam probed signals is the result of several factors: shot noise due to the finite number of secondary electrons, convergence errors of the feedback circuit, and jitter in the timebase, tester,or device. In addition to random noise, there is a


Edge Position (ps)


known systematic error due to the nonlinear response of the voltage measurement system of e-beam probers.


The amplitudes of the transitions in memory circuits fall within a relatively small range. This reduces the voltage nonlinearity's effect on common timing measurements.


-10-5 Error (ps)0 5 10 15 20 25


630 640 650 660


250


Elapsed Time (minutes)


The voltage-related error in an interval can be


Scope STAR1.0.1 Copyright (c) 1999 Schlumberger ATE


estimated from the inverse slew rate, dt/dtV , at the


In the next step, increased voltage (Vcc) was applied to units in static mode for a short period of time. We chose to apply the stress in static mode in order to apply voltage stress (and not current/temperature) to the transistor gates. Sicc vs. V, T and emission measurements were taken after the stress. This sequence was repeated until the first abnormal emission was detected.


During the experiment, the distinctive effect of leakage defects (because of charging) on stand-by-current behavior was shown. On units #1 and #3 no emission sites were observed before stress. Exponential IV slope of both units was approximately 1.5 at room temperature. On unit #1, no measurable change in static current was observed during five stress steps, when no emission sites were detected. After the sixth stress step 4 emission sites were detected. At the same time, a strong change of unit static I/V was observed. Sicc value increased twofold, and the exponential IV slope decreased from 1.5 to 1.3 at room temperature (see Fig.4).


sIcc ~ exp(1.28Vcc)


four emission sites


sIcc ~ exp(1.50Vcc)no emission sites


1.E-041+slcc, A1.E-03


1.E-02


2.5


Vcc, V


Figure 4 Static current I/V curves at different steps of the stress. A clear change of Sicc curve was observed at the same step in which emission points were detected.


A similar, but weaker effect, was seen on unit #3 after one step of the Vcc stress, when one emission spot was detected. Together with the change of static IV, the temperature dependence of the unit’s static current changed. Sicc increased more strongly at lower temperatures than at higher ones, and the slope of the Sicc vs. T curve decreased (see Fig.5). In addition, the“defective” I/V behavior (exponential slope of ~1.3)was observed on the “fresh” #2 unit from the same experimental group. This unit had one emission site prior to the Vcc stress, probably as a result of similar stress in the process.


no emission sites one emission site


1.E-04


1.E-03


280


290


310


320


Temperature, K


Figure 5 Sicc of #3 unit at Vcc=1.8V as function of


temperature. Circles depict current values before


stress; Triangls depict values after stress when one


emission point was detected.


All detected emission spots on units in the experiment were concentrated in a small area in n-MOS transistors of identical buffers. The same emission sites and gate leakage were observed on the same product units that failed in HVELT, and on the fresh units that were not subjected to any stress. All buffers with emission had high ratio antennas on the gates, however those antennas were not the largest antennas in the product.


FA on the stressed and fresh units verified gate leakage at emission locations. Electrical measurements of ondie transistors performed at emission locations on several units confirmed gate-to-source leakage (Fig.6)with values in the micro-ampere range.


Vss


The


leakage Lpath


Figure 6 Leakage path in the damaged buffer at emission location.


Results of the Experiment


1. The results of step 1 units show an excellent correlation between: leakage sources caused by process charging on the fresh units; units stressed by High Voltage Electrical Life Test (HVELT);and units stressed by high voltage applied in very short time duration.


2. The robustness of the design is quickly verified, and


the weakest place is localized on a very limited


sample size.


3. There is a distinct effect of leakage defects due to


charging on stand-by-current behavior.


4. The results on step 2 showed no pronounced


leakage sources in EMIC.


slcc at Vcc= AV,81.


We showed that the behavior of many units is the same as single unit behavior, and the behavior of a single unit is the same as single transistor behavior. Therefore, the weakest place in the product was localized just on single units, by means of short time stress at elevated voltage. At that weakest place, gate oxide of transistors had maximum damage by process charging because of a specific design configuration.


Units with typical and abnormal slopes were characterized in an emission microscope in static state.


The numbers of emission sources were detected and the correlation with the abnormality of the slope was obtained. Typical BI showed the reduced reliability of abnormal slope units, and FA of BI failures showed that the failure and the emission points locations are the same.


This is the first time that we have applied accelerated Vcc voltage stress in static mode to typical units. The stress resulted in the appearance of the same emission points and change in the slope (similar to the results for abnormal slope units). This emission location indicates the weak points in the design-to-process interaction.


Proposed fast stress enables the detection of design/manufacturing potential problems in a very short time (in comparison to hundreds of hours of typical BI stress). We propose to perform FA analytical/imaging analysis of new products in order to obtain better electrical characterization of weak points that are the result of problems in the design-to- process interaction.


We also propose to implement this method for reliability characterization, low yield analysis and for process monitoring.


We would like to thank Avi Avraham, Ron Wittenberg and Avi Strum for their support in this project, Gila Yampolsky for helping with emission imaging,Valentina Korchnoi for sample preparation, and Tiran Cohen for helping to set up the test.


1) C. Weber, B. Moslehi and M. Dutta, “An integrated framework for yield management and defect/fault reduction,” IEEE Trans. Semicond.


Manufact., V. 8, pp. 110-120, 1995.


2) W. Needham, C. Prunty and E. H. Yeoh, “High vollume Microprocessor Test Escapes, an analysis of defects our tests are Missing,” International Test conference, pp. 25-34, 1998.


3) R.K. Gulati and C. Hawkins, “Iddq testing of VLSI circuits,” Kluwer Academic Publishers, Boston,


1993.


4) B. Lisenker, Y. Mitnick, “Fault model for VLSI circuits reliability assessment”, International Reliability Physics Symposium, p.319, 1999


5) M. Bohr and Y. El-Mansy, “Technology for advanced high-performance microprocessors”,IEEE Transactions on Electron Devices, V.45,pp.620-625, 1998.


6) S.M. Sze, “Physics of Semiconductor Devices 2nd.


Ed.”, Wiley, 1981


7) J. P. Mc Vittie, “Process Charging in ULSI:Mechanisms, Impact and solutions”, IEDM proceedings, p.17.1.1, 1997


8) P. Tobias, D. Trindade, “Applied reliability“, Van Nostrand Reinhold, 1995


Electronic Device Failure Analysis Society, editor, p 103-107


DOI: 10.1361/cp1999istfa103


# Automatic TEM Sample Preparation


Automatic TEM Sample Preparation


Wayne D. Kaplan


Department of Materials Engineering, Technion – Israel Institute of Technology, Haifa, Israel


Ron Oviedo


National Semiconductor Corporation, South Portland, Maine


Kim Kisslinger


Efrat M. Raz


SELA U.SA., Inc., Sunnyvale, California


Colin Smith


The rising demand in the semiconductor industry for higher spatial resolution in the analysis of device defects has focused attention on the use of transmission electron microscopy (TEM). However,conventional TEM sample preparation may be difficult and time-consuming, and depending on the operator may result in a low yield of quality specimens. One solution to this problem is the use of focused ion beam (FIB) milling for the final stage of TEM sample preparation. However, specimens have to be mechanically thinned prior to FIB processing,and the need to characterize specific devices requires a pre-FIB preparation method to isolate specific regions on the wafer. An innovative and automated solution that isolates specific devices and prepares TEM specimens for subsequent thinning by FIB has been developed. Based on controlled microcleaving technology, the system automatically performs the pre-FIB preparation in less than 30 minutes. An important added benefit is that the target area to be analyzed can be positioned at a specific distance from the sample edge, thereby facilitating the final FIB milling stage. The thinned specimen is automatically packaged for subsequent FIB processing and TEM.


Details of the method and examples showing TEM results from tungsten filled vias are presented.


Transmission electron microscopy (TEM) is a fundamental characterization technique in materials science, and one of the only methods which provides a myriad of crystallographic, morphological and


chemical information with high spatial resolution [1].


While TEM is extensively used in basic research and in development, it is rarely used in industry for process monitoring, due to the extensive amount of


time required to prepare TEM specimens. With the continuing reduction in size of devices in the semiconductor industry, process monitoring often requires TEM investigations that provide microstructural characterization not available from scanning electron microscopy (SEM). However, the rigid specification requirements for quality TEM specimen preparation are, at the moment, the limiting factor in the use of TEM in the semiconductor industry.


Non Site-Specific Sample Preparation


The requirements for a quality TEM specimen are extremely rigid. Specimens are normally 3.0mm in diameter, and often less than 100µm in thickness.


The center region of the specimen must be transparent to electrons, and must include the region to be investigated (see Figure 1). While the preparation of plan-view specimens from bulk materials is fairly straightforward, the specimen preparation method required to provide specimens for the investigation of thin films on a substrate (cross-section specimens), or devices on a substrate, is extremely complicated.


Figure 1 Schematic drawing of a TEM specimen.


Cross-section specimens of thin films on a substrate are usually prepared by first sectioning the substrate,and gluing sections ‘face-to-face’, in order to achieve a 3.0mm thick slab of material containing the thin films at the center of the slab. For substrates with a thickness of less than 1.5mm, additional sections are glued ‘face-to-back’ in order to reach a total slab thickness of 3.0mm (see Figure 2). In order to provide a final specimen with sufficient mechanical rigidity, the sectioned slabs are then inserted and


glued inside a metal or ceramic tube [2, 3]. Disks of


3.0mm diameter are then sectioned from the tube and mechanically thinned to less than 100µm in thickness.


Chemical or electro-chemical thinning techniques are usually not possible for cross-section specimens, due to the varying thinning rates of the different materials, so ion-milling is the method of choice to thin the center of the 3.0mm disk to a thickness transparent to high energy electrons. In order to induce preferential ion-milling at the center of the specimen (the region containing the thin films)mechanical dimpling of the center region is normally required prior to ion-milling.


While this method can produce quality cross-section TEM specimens, the process is extremely time consuming, and requires individual expertise. In addition, the process always includes a fairly high percentage of specimens which are not sufficiently thin for TEM investigations. Furthermore, if TEM investigations of individual devices in the thin film are required, this method is not viable, since it is not possible to ensure that the region of interest will be exactly in the center of the 3.0mm specimen.


Site-Specific Sample Preparation


In recent years focussed ion beam (FIB) milling has been used to produce cross-section TEM specimens of individual devices (site-specific) in thin film semiconductors [4-7]. The advantage of FIB is that the region which is thinned is constantly monitored using secondary electrons. However, the use of FIB milling to produce electron transparent specimens also requires mechanical thinning of the specimen prior to FIB processing. Thinning requires operator expertise and is time consuming, thus limiting the application of FIB/TEM in process monitoring, failure analysis and research and development. This paper describes an automated solution that isolates specific devices and prepares TEM specimens for subsequent thinning by FIB.


Figure 2 Non site-specific cross-section TEM sample preparation sequence.


Methodology


The pre-FIB preparation process is conducted automatically by a computer controlled system called the TEMstation (manufactured by SELA). A wafer segment is first cleaved from the wafer using a


microcleaving system [8]. This stage requires about 15 minutes, and produces a wafer segment containing the region of interest. The cleaved segment is entered into the stand-alone system, which performs a preliminary sawing procedure to reduce the sample


size to 2.5mm × 2.5mm (see Figure 3).


Figure 3 Preliminary sample slicing procedure.


A slicing procedure then thins the sample (adjacent to the region of interest) to 20µm (see Figure 4),significantly reducing subsequent FIB milling time.


Figure 4 Slicing of the sample.


0.6mm


The sample is then automatically bonded to a sample stub (see Figure 5), which following additional


-350.8mm0.


truncation and separation cutting operations, results in an end-specimen that is seamlessly mounted for


Sample Stub


both FIB milling and TEM (see Figure 6).


-f<200um


Figure 5 Bonding the sample on a sample stub.


Region of Interest


This pre-FIB preparation method is based on


2.5mm


Segment


controlled microcleaving of the wafer segment,which determines the location of the region of interest on the final section. The system accepts micro-cleaved samples ranging in size from 2.1mm ×


2.1mm to 13mm


Operator Designated


× 20mm.


-Reduced


The system produces an end-specimen that contains


sized sample


one cleaved edge (a high quality edge) and one sliced edge. Detailed SEM investigations have not revealed microcracking due to cleaving or slicing, and show a maximum of 2µm chipping on the sliced edge. This minimizes surface flaws, which could act as crack initiation sites and lead to failure of the specimen during handling.


The system end-specimen is automatically packaged in a clamping device, greatly simplifying sample handling and FIB interfacing for continued thinning(see Figure 6).


Fine Blade


End-specimen


Clamping Device


Thinned Edge


20 microns


Figure 6 End-specimen packaging for FIB processing.


Region


The result of this process is a section thinned to 15-


of Interest20µm in 15 minutes (see Figure 7).


20um- Region of Interes


Region of Interest,


03mm


Adaptable


Section A-A


Figure 7 End specimen dimensions.


Bonding Area


Such a section requires a nominal FIB milling time of 90 minutes to produce the final TEM specimen.


Furthermore, the system is fully automated, and operator support is not required after insertion of the wafer segment into the system. The system is well suited to a multi-user environment, and requires no expertise or previous experience, allowing the


preparation of 3-4 samples/hour. The system end specimen is free of “process dirt” and requires no cleaning (the process does not use water).


In order to demonstrate the output of the system,TEM specimens were prepared from tungsten vias located on a conventional silicon wafer. As a result of microcleaving, the region of interest is located at a pre-defined (variable) distance from the cleaved edge. The system automatically slices the specimen using a high-speed blade, after which it is automatically bonded to the sample stub. After bonding,the thickness of the specimen is reduced from the back side of the wafer at the region of interest, to


Sliced


Cleaved minimize subsequent FIB milling time (see Figure 8).


Figure 8 Plan-view optical micrograph of the


thinned specimen.


Figure 9 presents a low magnification SEM micrograph of the final specimen, showing the sample after thinning. Towards the center of the wafer is the region of interest, which was thinned using FIB milling. Figure 10 presents a higher magnification SEM micrograph of the thin membrane containing the region of interest.


Thinned Membrane


Tungsten Via


Figure 9 Low magnification SEM micrograph of the final specimen showing the edge of the sample, after thinning by the system and subsequent FIB milling.


1.0μm


Figure 10 Higher magnification SEM micrograph of the thinned membrane.


Figure 11 presents a low magnification bright field TEM micrograph of the region of interest. Figure 12 presents a higher magnification bright field TEM


20μm


micrograph, showing the morphology of the via, the metal lines, and the TiN diffusion barrier located between the metal and the oxide.


Silicon


1.0 μm


Figure 11 Low magnification bright field TEM


micrograph of the region of interest.


5.0 kv x350 85.7μm


Figure 12 Higher magnification bright field TEM micrograph.


An innovative and automated solution that isolates specific devices and prepares TEM specimens for subsequent thinning by FIB milling has been developed. Based on controlled microcleaving technology, the TEMstation automatically performs pre-FIB preparation in less than 30 minutes. An important added benefit is that the target area that is to be analyzed can be positioned at a specific distance from the sample edge, thereby facilitating the final FIB milling stage. The thinned specimen is automatically packaged for subsequent FIB processing and TEM.


1) D. B. Williams and C. B. Carter, Transmission Electron Microscopy, Plenum Press, N.Y.


(1996).


2) Strecker, U. Salzberger, and J. Mayer, Praktische-Metallographie, 30[10], 482-495 (1993).


3) D. Brandon and W.D. Kaplan, Microstructural Characterization of Materials, p 190, John Wiley & Sons, N.Y. (1999).


4) J.F. Walker, D.F. Moore, and J.T. Whitney,Microelectronic-Engineering, 30[1-4], 517-522(1996).


5) Y. Kitano, Y. Fujikawa, T. Kamino, T. Yaguchi,and H. Saka, J. Electron Microscopy, 44[5], 410-413 (1995).


6) Y. Kitano, Y. Fujikawa, H. Takeshita, T.


Kamino, T. Yaguchi, H. Matsumoto, and H.


Koike, J. Electron Microscopy, 44[5], 376-383(1995).


7) M.H.F. Overwijk, F.C. Van Den Heuvel, and C.W.T. Bulle-Lieuwma, J. Vacuum Science &Tech., 11[6], 2021-2024 (1993).


8) C. Smith, “Microcleaving”, European Semiconductor, (1/1995).


Electronic Device Failure Analysis Society, editor, p 109-116


DOI: 10.1361/cp1999istfa109


The progress of modern day integrated circuit fabrication technology and packaging has made fault isolation using conventional emission microscopy via the top of the integrated circuit more difficult, if not impossible. This is primarily due to the use of increased levels and density of metal-interconnect,and the advent of new packaging technology, e.g.


flip-chip, ball-grid array and lead-on-chip, etc.


Backside photon emission microscopy, i.e.


performing photon emission microscopy through the bulk of the silicon via the back of the integrated circuit is a solution to this problem. This paper outlines the failure analysis of sub-micron silicon integrated circuits using backside photon emission microscopy. Sample preparation, practical difficulties encountered and case histories will be discussed.


With aggressive progress into deep sub-micron ULSI,emission microscopy performed from the front side of the integrated circuit has become more difficult,and at times impossible. This is primarily due to 2 reasons :


(i) Scale down of geometry and increased complexity of the modern day integrated circuits (IC)has led to the use of increased levels of metal interconnects. This problem is compounded by aggressive design rules, which make interconnects on the same level spaced so closely that it has become very difficult for any emitted photons originating from a defect at the silicon substrate to escape to the top of the IC for detection. This is further aggravated by the reduction in the magnitude of leakage currents due to the use of lower operating voltage, of


which the consequence is less intense emissions.


This problem will apparently perpetuate with the next generation technology which uses even tighter interconnect design rules as a result of using lower resistance interconnect (e.g. copper)and high k-dielectric,


(ii) The advent of new packaging technology, e.g.


flip-chip and lead-on chip (LOC) used commonly for dynamic random access memory(DRAM), makes performing emission microscopy via the chip front totally impossible.


Principle


Silicon is almost transparent to wavelengths around 1070nm. Above and below this wavelength, photon transmissivity through the silicon is attenuated due to absorption. Most defect types emit at wavelengths from 500nm to 1300nm and since photon emission is isotropic, it is therefore possible to view the emission through the silicon substrate.


Fundamentally, performing backside emission microscopy is no different from that of conventional frontside emission microscopy. The device failure is electrically replicated and emission microscopy performed. The only difference is that the backside approach captures the emission through the back of the IC chip or wafer. For packaged parts, the back of the IC chip has to be made accessible for the analysis.


This is accomplished via delicate sample preparation,described in the next section.


Photon emission is caused by 3 fundamental mechanisms, inter-band recombination via direct or indirect transition, intra-band recombination or Bremsstrahlung. Typical defects causing photon emission include :


• gate-oxide rupture,


• hot-carrier effects,


• CMOS latch-up,


• junction spiking,


• avalanche breakdown,


• crystal dislocation & stacking fault


• forward biased junctions


• junction leakage


The pre-requisite for detecting photon emission from the back of the integrated circuit is to expose the silicon substrate on which the integrated circuit is built on. This is not a problem for wafers, but for packaged devices, the molding compound and the die paddle has to be removed. This can be accomplished with mechanical milling using commercially available computer numeric control (CNC) milling machine from emission microscope manufacturers.


The precision milling machine is used to bore and remove the epoxy molding compound and subsequently, the die paddle. This is followed by a mirror polish of the bulk silicon (shown in Figure 1).


The surface of the bulk silicon has to attain a mirror finish. This is to reduce internal reflection so as to obtain a reasonably clear image or emission. An uneven surface due to chipping or scratches,sometimes created during the milling process, causes shadows (shown in Figure 11) on the illuminated image and can mask emissions. Attention should therefore be paid to the quality of the surface finish.


Figure 1 Schematic showing backside photon


emission analysis for a packaged part.


Figure 2 Different types of packaged ICs with the back of die exposed for emission microscopy.


For wafer level analysis, no elaborate sample preparation is required for back-grinded wafers, since the back surface is already polished to a mirror finish.


For wafers with no back-grind, the silicon-oxide and silicon nitride on the wafer back surface can impede imaging. These layers need to be removed and can be done so by fine milling using the CNC milling machine or a hand-held drill. Chemical means using reactive ion etching and chemicals were experimented, but did not produce an acceptable surface finish.


Electrical biasing to the wafer level device is provided via micro-probing. This is accomplished on a ‘backside’ probe station. The wafer is held face down with its backside facing the emission camera,and the micro-probes access the bondpads on the wafer from under the wafer surface (shown in Figure 3). The whole backside micro-probing setup is literally upside down.


Figure 3 Schematic showing backside photon


emission analysis on wafer using micro-probing.


Figure 4 A 0.5um device viewed through 60um of p-type silicon substrate. The n and p source/drain of transistors are visible.


Silicon Substrate Thinning


Thinning of the silicon substrate is advocated in some


related backside analysis literature [1] and [2] as a means to reduce the silicon filtering effect. This call comes from the fact that photon transmissivity through doped silicon bears an inverse exponential relation to the thickness of the silicon. Therefore, the thinner the silicon, the higher the photon transmission.


Figure 5 Plot shows that transmissivity for both


heavily doped N+ and P+ silicon is improved by


several orders of magnitude if the thickness of the silicon bulk is reduced. (Adapted from W. Spitzer& H.Y. Fan, Physics Review, 108, 2 (1957)


pgs 268-271)


Joseph, et al. [4] and Hurley, et. al. [2] reported that in heavily doped silicon, the large number of free carriers released by the dopants causes strong photon absorption making it almost opaque, while photon transimissivity through lightly doped silicon experience a much lower degree of absorption. There


were also reports by some authors [5] and [7] that


thinning the thickness of silicon has little or no significant effect on photon transmissivity.


Generally, our experience shows that thinning the silicon does help in improving the image clarity, but thinning beyond a critical thickness does not further improve the clarity of the image. Figures 6 and 7 show that a clearer image can be obtained after thinning the silicon substrate to 150um as compared to the same device with 480um silicon. Further thinning of the device to 50um did not help to improve the image further, shown in Figure 8.


However, we have also been able to obtain very clear images and emissions from devices which were not thinned, as an example, Figure 13 shows a device viewed through 480um of silicon (the doping density was comparable for both devices).


The conclusion drawn from our experience is that the quality of image is highly dependent on the size of the structure or feature that is imaged. For large devices, e.g 0.6um or 0.5um technology devices,thinning is not a critical requisite for low and medium doped silicon, but may further improve the clarity of the image. For small geometry devices, e.g. 0.35um,


0.25um and beyond, thinning is most likely necessary, even for lightly doped devices, to obtain an image of reasonable clarity.


1 Wdv 区 200 ps/dlvFDelay: 19.62 nsAwg:364xo Tr9 4(File 7 Setup 7lWaveform ) Trigger ]


(-clp)


interval's endpoints and the peak-to-peak voltage error,


PW: 4n ps (nd) 医院


Lin indp Raw Feg SA--0.75GHz


δV on the signal:


δtV = ± (dt/dV) δV


(3)


For delay time measurements with the voltage error


H=FON


dominated by high-frequency noise, δVnoise, the


山=s0


uncertainty is:


1=t 0644


δtnoise = ± (tT/ 0.8V) δVnoise


(4)


1=8 0:4


Ip =50lp2


where V is the amplitude of the transition. For a 2V,


Tein


200 ps transition and 50 mV peak-to-peak noise, this becomes ± 6ps. A 50 mV noise level can be achieved


TimeCuaon-12.00.-188.00.324.00


after a few minutes of averaging for a beam pulse width of 100ps and LP=3. The use of substantially longer averaging risks charging the probed region.


Sampling Time


Each data point on the scope display is an average of the probed signal's potential over a finite sampling time, tsample.


The sampling time is determined by a


several factors: (1) the setting of the beam pulsewidth,


Tp, in the scope tool, which is not calibrated to a direct


measurement of the beam pulse shape, (2) the


automatic smoothing of a number of points, LP , to0


give the displayed waveform, (3) jitter in the timebase,S


and (4) the transit time effect, due to the fact that theu


secondary electrons are still affected by the circuit1.*1 potential for ~12 ps as they leave the probed surface.


We can obtain a rough estimate for the sampling time


by considering the first two effects and using Tp for


the actual electron pulsewidth:


tsp = Tp (LP - 1) (time/div)/50


(5)


The sampling time was experimentally measured by examining the apparent transition time tT' of a fast edge as a function of tspand using the following model:


tT' = ( tT2 + tsample2 )1/2


(6)


where tT is the actual transition time, and tsample is the total sampling time. Fig. 5 shows the measured edge at different values of the pulsewidth parameter,and Fig. 6 is a plot of the 10-90 transition time as a function of tsp . By extrapolating the tT' vs. tsp curve to tsp = 0, the measurements give a value of 80ps for the actual edge transition time. The measured sampling time is listed in Table 1, along with estimated values from Eqn. 5, for several pulsewidth parameter settings.


Figure 5 A fast edge in a DRAM circuit measured for various settings of the pulsewidth parameter, Tp. In order from top to bottom, the curves are for Tp = 40ps,50ps, 100ps, 200ps, 500ps, and 1000ps.


Figure 6 The measured transition time for an internal


DRAM signal as a function of the sampling time


estimated by Eqn. 5. The actual transition time of an edge can be determined by measuring this curve and


extrapolating to tsp = 0. For the present case, this


yields tT = 80 ps.


0 e200!400 U600 a


w800 d1000


◆


1200


200 400 600 800 1000 1200


Sampling Time (ps)


Table 1 Measured and Estimated Sampling Times


|Tp (ps) |Tp (ps) |tsample |tsp |
|---|---|---|---|

|40 |40 |65 |40 |

|50 |50 |80 |70 |

|100 |100 |110 |120 |

|200 |200 |390 |220 |

|1000 |500 |630 1010 |520 1020 |

Ultimate Accuracy


By applying the quantitative results of the preceding


section, we can now estimate the best possible


accuracy and determine the operating conditions that


yield this performance.


To achieve the level of accuracy described by Eqn. 1,


other sources of error must be made negligible. Thus,ps)Accuracy (the best accuracy is obtained by probing signals on


clean, bare metal surfaces that are surrounded by


insulator that has not been significantly charged by


excessive probing or, especially, SEM imaging. The


probed location is sufficiently far from lines whose


signals have transitions near the one being measured.


The minimum time/div is used that allows accurate


determination of the levels before and after the


transition. The sampling time is adjusted to give the


best trade-off between edge distortion at long


sampling times and voltage noise at short sampling


times.


Figure 7 shows the net uncertainty for measured


delays between symmetric transitions as a function of


delay time. For symmetric transitions, finite sampling


time is not a factor. It only broadens the transitions


without shifting their midpoints. Timebase inaccuracy


is the factor over which we have the least control. It


determines the measurement uncertainty of intervals


larger than ~80ps. Below 80ps, the uncertainty


becomes constant and can be estimated from the


errors due to voltage noise, discrete time axis and


timebase structure (Fig. 3):


δt = ± ( δt2noise + δt2discrete + 25ps2) 1/2 (7)


With a 50ps/div time scale, and 50mV peak-to-peak


noise, the minimum error is ±8ps.


For transition time measurements, the broadening due


to finite sampling time is added to the uncertainty in


Fig. 7 , where now the horizontal axis is the measured


transition time.


Figure 7 Ultimate accuracy of the IDS-10K+ as a


function of the time interval being measured.


Repeatability


The above discussion shows that the uncertainty in a timing measurement has contributions from a variety of sources. Some of these errors are systematic:background signals from interference, timebase inaccuracy, voltage detector nonlinearity, and finite sampling time. The magnitude of these errors is the same when a given measurement is repeated. We can estimate the uncertainty these cause in a measurement by taking the worst-case error and saying that this much error might be present in the measurement.


Most of the sources contribute random errors:voltage noise, drift of the probe's position during a measurement due to sample motion and charging,discrete time axis, any drift (timebase, tester or device), and signal distortion due to charging and contamination. The error from these factors varies when a measurement is repeated. Thus, the net uncertainty due to all the random errors can be estimated from the spread in values for repeated measurements of any particular time interval. This practice provides a way to quickly determine the uncertainty from random errors for any particular probe point, circuit geometry, measurement conditions, etc. The repeatability for measuring a


10 0


0 500


Time Interval (ps)


given time point on a signal is defined as the uncertainty:


δ tj = ± 3σ


(8)


where σ is calculated from repeated measurements of tj . The δtj for both endpoints of an interval are then added to give the uncertainty in any particular interval.


To learn the uncertainty from random errors in delay time measurements, the transition midpoints for various signals in a DRAM circuit were measured 3-21 times and the ± 3σ values were calculated. The measurements were done on the bare metal lines of an unpassivated wafer at nominal device operating conditions. The probe conditions were: 500ps/div,ext. CLK=30, scope delay = 16-28ns, Tp = 100ps,LP = 3, Normal beam mode, LIN sampling. The results for seven signals are plotted in Fig. 8 as a function of edge transition time. Also shown is a line that approximates the uncertainty from inherent factors:


δtj = ± ( δt2noise + δt2discrete ) 1/2


(9)


where the terms in parentheses are now the errors on a single tj ( the transition midpoint) due to voltage noise and the discrete time axis. For these measurements, the error from voltage noise is


0.018 tT (with tT in picoseconds) and the error from the discrete time axis is 10 ps.


The repeatability sub-500ps edges was at or below the inherent uncertainty of ~ ± 10 ps. This result shows that all of the other random sources are negligible,since they are comparable to the human error which partially cancels the effect of the discrete time axis in locating the transition midpoints. This experiment supports the use of Eqn 9 to obtain a safe estimate of repeatability for transitions shorter than 500ps. The only transition above the inherent repeatability has the largest transition time. This is also true for other slow transitions not plotted in Fig 8, for which the repeatability gets worse as the edge's transition time increases. For the slowest transitions, random distortions of the transition region are apparent from one measurement to the next. These results indicate that the repeatability of transitions slower than 500ps is determined by random voltage errors. The most likely cause of these errors is interference that is not synchronous with the test pattern (e.g. 60Hz noise).


Figure 8 The uncertainty, ±δtj , in an edge's position as a function of its transition time tT' . This


uncertainty is the net result of all random errors. The line approximates the contribution from inherent random errors, given by Eqn 9.


Probing Passivated Circuits


Signals on a passivated wafer of DRAM die were measured by probing the passivation and comparing these to signals from bare-metal probe points created by FIB. The transition midpoints agreed to within±20ps as seen in Fig. 9 below. The passivation data was taken repeatedly to investigate random errors.


The results for a fast edge are shown in Fig. 10 and show ±16ps repeatability for a single edge having a measured transition time of 130ps.


Figure 9 Three DRAM signals probed at the surface of the die's passivation and on bare-metal FIB points.


0 10 20 30 40 50


Transition Time (ps)


Figure 10 Repeatability of a 130 ps edge when


measured by probing the passivation. The uncertainty from all random errors is ± 16ps.


E-beam vs. Mechanical Probe


E-beam and mechanical probe results were compared by measuring a set of signals on an unpassivated wafer with each technique. An example of such measurements on three signals is shown in Figures 11 and 12.


Figure 11 Signals A (top), B (center) and C (bottom)from an unpassivated wafer probed using the IDS10K+.


Figure 12 Signals A (top), B (center) and C (bottom)


for the same die, test, and tester, probed using a


Model 28 Picoprobe.


The delay times, tAB, and transition times, tT, for 9 signals were measured and compared. The results are given in Table 2. The signal names are given in the first column. Signal 1 was used a reference for the delay time measurements. The delay times measured by e-beam are given in the second column, and the discrepancy between e-beam and mechanical probe delay times are listed in the third column. The e-beam and mechanical probe values for edge transition times are given in fourth and fifth columns, respectively.


Table 2 Comparison of E-beam and Mechanical Probe Timing Data


|Signal |EB tAB (ns) |MP-EB tAB (ps) |EB tT (ps) |MP tT (ps) |tT Model |
|---|---|---|---|---|---|

|1 (Ref.) |0 ||130 |400 ||

|2 |1.50 |+ 160 |450 |700 |- 10 |

|3 |2.21 |- 40 |210 |450 |- 17 |

|4 |3.24 |- 40 |2800 |2400 |-220 |

|5 |2.16 |+ 400 |2240 |2400 |-220 |

|6 |4.48 |+470 |7000 |8950 |-220 |

|7 |8.58 |- 30 |272 |490 |- 31 |

|8 |11.36 |+ 170 |870 |1160 |+ 14 |

|9 |11.55 |+160 |340 |380 |+ 70 |

The discrepancies were analyzed in terms of known errors for each technique. The measurements show that each technique distorts the signal, only in different ways. Mechanical probe adds ringing and gives a longer apparent transition time due to its longer risetime (350ps specified for Model 28) and load capacitance added to the circuit nodes (40fF specified). E-beam probe typically has interference and charging effects, as well as an initial transient of undetermined cause. Interference that is synchronous with the test cycle appears the same in each repeated measurement, and asynchronous interference appears as a changing background. Analysis of the data indicates that the main sources of error and uncertainty for each technique are as follows:


Mechanical Probe:


1. Transient response of probe: unknown response


during fast transition, overshoot/ringing


afterwards


2. Risetime large compared to transition time: shifts


location of transition midpoint


3. Probe Capacitance broadening transition for lowC nodes


E-beam:


1. Interference: 170ps for fast edges, up to 1ns for


5ns edges


2. Timebase errors: ~ ± 60 ps for intervals longer


than 500ps


2. Errors in placing scope cursors due to waveform


structure


A simple model for the effect of mechanical probe response time predicts an error, δt , in the measured delay time:


δt =0.625 [ ∆tTSignal - ∆tTRef_ ]


(10)


where ∆tTSignal and ∆tTRef_ are the differences between the measured and actual 10-90 transition times for the signal and the reference. This error is presented in Table 2 in the last column, labeled "tT Model". For sub-1000ps edges, the e-beam values are used for actual values. For longer edges, ∆tTSignal is assumed to be zero. By comparing the second and last columns in Table 2 , it can be seen that broadening of short transitions (e.g. the reference transition) does not explain the observed difference between mechanical probe and e-beam.


Load capacitance of the mechanical probe also does not explain much of the difference. The largest discrepancies occur for nodes with unusually large capacitance, where the probe load capacitance will have the least effect.


The signals with ~170ps discrepancy occur in one location on the circuit, and the signals with ~400ps discrepancy occur in a neighboring part of the circuit.


Also the discrepancy increases with increasing tT.


Thus, the most likely remaining cause of the discrepancy are consistent errors on the e-beam signals due to interference in some locations that is synchronous with the test cycle. Measurements on neighboring lines can be used to identify the interference source and subtract them from the data.


The IDS-10K+ can be used to make timing measurements with known accuracy using the results of this paper. The inherent accuracy is sufficient for most quantitative high-speed measurements, and can be attained largely by eliminating interference errors and optimizing the prober's operating conditions. The timebase errors and sampling time for a particular tool can be readily determined, as can the uncertainty from random errors. Due to the availability of sampling times as short as 65ps, and the importance of interference errors, the accuracy of e-beam internal probe is actually aided by the drive toward increasing


fast edges in circuits, in sharp contrast to mechanical probe.


I thank Surendra Madala, Lisa Davis, Al Fixl, Steve Casper, and Vernon Rogers for helpful discussions and other support of this work; Dwayne Dohmann,Kevin Trapp and Gary Howe for the mechanical probe data; and Minjae Cho for the FIB work.


Electronic Device Failure Analysis Society, editor, p 97-102


DOI: 10.1361/cp1999istfa097


# Short High Voltage Stress for Design- to- Process Characterization.


Short High Voltage Stress for


Design-to-Process Characterization.


Boris Lisenker, Dmitry Veinger and Yuri Mitnick


Intel Israel (74) Ltd., Haifa, Israel


In modern semiconductor manufacturing there is a requirement for constant decrease in new process and new product development cycles. Faster synchronization between the design and the process may be achieved by improved feedback from the VLSI product back to the process (process-to-design interaction).


Design rules are developed at an early stage of process development. Products on the new process usually exhibit design marginality that indicate that in some process corners the design cannot withstand process induced damage or process instability. In order to overcome this problem, design characterization versus process induced instability and stress is required.


The design characterization process is complicated by the peculiarities of the submicron CMOS process,where there are difficulties in maintaining process uniformity. Examples of these difficulties are geometrical proximity effects in lithography and plasma etching that cause variations in critical dimensions (CD), gate oxide (GOX) and inter-layer dielectric (ILD) thickness, and consequently variation in transistor characteristics. The complexity of process related variations make it difficult to estimate the margin of the design. It has been observed that yield loss in new products is primarily due to parametric variation problems resulting in systematic failure [1].


Microprocessors on 0.35 µm and 0.25 µm CMOS process also show a high level of parametric (soft)failure [2]. Thus, particle defects will not continue to dominate parametric yield loss.


For losses caused by parametric deviation, it is easy to define the normal range of the parameter- baseline. The yield loss is more probable for larger deviation. At some


level of deviation, failure becomes unavoidable (usually this point is called ‘cliff’). The distance from the cliff is the margin. The lower the margin, the higher the probability that the deviation will turn out to be a latent defect. Latent defects may lead to circuit level performance degradation,and cause product failures in the field.


Static current (Sicc) based testing is an example of a technique that provides parametric fault detection and location procedures [3]. Short-channel CMOS VLSI circuits can be presented in standby mode as a single effective MOSFET with inherent defects. It is shown in


[4] that normal units can be separated from defective ones by means of measuring Sicc current versus Vcc.


Normal Sicc vs. voltage behavior is exponential. The electrical characterization of microprocessors gives electrical signatures that correspond to integrated defect mechanisms. Failure analysis (FA) has more capabilities in root cause investigation than electrical testing on the integrated level. In the past, FA efforts were mostly dedicated to location of random defects(normally, particle defects).


In the case when design is strongly influenced by parametric deviations in the process, there is a conceptual change in the approach to FA. A weak point in design-toprocess interaction is much more likely to cause failure than a random defect or particle. The FA of such a unit will not find the root cause of any failure according to ordinary FA procedures. In such cases, a totally different parametric approach needs to be applied.


In this paper we propose to apply FA capabilities to a flow with the aim of defining the product margin in a given process flavor. The experiments are performed on a microprocessor manufactured on a 0.25 µm CMOS process [5].


The first part of this approach is to define the parametric baseline of the product, that is, to learn what is normal, and which parametric behavior is failureprone. The parametric difference will then characterize the margin.


The role of FA in this stage is to apply different analytic and imaging techniques for the inspection of the units which represent the baseline (second section).


In the second part we will present the way to elucidate and measure the margin on each unit. The best way to do that is by means of the stress (third section). In conclusion, we will expand the knowledge obtained from FA for the characterization of product health.


Therefore, the role of FA is to provide sound analytical evidence that correlates with some electrical signature.


Parametric Product Baseline


The internal world of short-channel CMOS VLSI


circuits may be represented as a network of randomly


connected elements of 2 types: linear resistors for


interconnects including conductive defects, and,FF lOFEMOST Apnonlinear resistance for MOSFET’s in the off state [4].


The Ioff current flowing through nonlinear resistance is


the basic law of transistor Ioff current:


anJaV⋅+⋅•⋅=2eedslong_offshort_offL1BL1AVExpII (1)


where A and B are process dependent coefficients [6].


We characterized the p- and n- channel transistors


(0.25 µm CMOS process) for several effective channel


lengths (Le) and drain bias (Vds) in the off- state (see


Fig.1). We used measurements on a target transistor, an


oversized transistor (1.1* Le_target) and two


undersized transistors (0.85*Le_target, 0.95*Le_target)a that corresponded to the model. We then designated0


) ( )2e


O


by Ioff slope. Fig.2 shows thatd


the Ioff slope and absolute value of Ioff agree with


Eq.1.


We applied transistor characterization data to the VLSI


circuit. We assumed that the process will give us a


Gaussian variation of CDs on the die, and tried to


estimate Sicc. We obtained Ioff vs. CD as χ2


distribution with the maximum substantially lower than


the target dimension. In practice, transistors with


substantially higher Ioff will shunt other transistors [4].


Therefore, defect-free VLSI circuit static current


dependence on Le may be modeled as:


+K2⋅+


L 1


k


1exP k1一1


~


Ioff


Sicc


where k1 and k2 are constants that correspond to product level regression.


We performed the experiment on a microprocessor manufactured on a 0.25 µm CMOS process. The characterization showed the range of Sicc slope versus voltage to be between 0.9 and 2. Faster units have greater slopes due to CDs. This range is in agreement with our transistor characterization. Therefore, target transistor Ioff slope determines the Sicc slope of the VLSI circuit.


1.1*Le_target, slope 0.70


target Le, slope 1.37


0.9*Le_target,


slope 2.65


0.85*Le_target,


slope 2.74


1.E-11


1.E-10


鱼层1.E-09


1.E-08


1.E-07


1.E-06


1.E-05


VDS, V


Figure 1 Ioff current of p-MOSFET’s with different gate length.


0.5


d1.5 2


1.E-09 1.E-08


IOFF current at VDS=2V, A


n-MOSFET


p-MOSFET


Figure 2 Relation between Ioff current at Vds= 2V and Ioff(VDS) exponential slope for n-MOSFET’s and pMOSFET’s. Four points for each curve correspond to


0.85,0.95,1, 1.1 skews of target Le.


In addition to normal Leff variation driven contribution to the Sicc current, which is inherent to the process,there are the following defect sources: transistors with a much shorter than targeted Leff, or width, due to random high poly CD deviation; transistors with gate oxide (GOX) charging; and narrow transistors with field oxide charging. In addition, charge in the gate oxide causes a shift in threshold voltage (Vth), and also contributes to Ioff. GOX charging high poly CD variations are strongly design dependent. Due to proximity and layout related effects, charging may increase due to the geometry of the metal line that is connected to the gate [7a]. All the leakage mechanisms mentioned above appear to be defect related sources that contribute to Sicc.


These mechanisms have a current versus voltage slope that is different from Ioff. When defect contribution is significant, the contributed change to the Sicc slope is also pronounced. Figure 3 illustrates this statement. The stress induced leakage current of the GOX gives very high leakage contribution at lower voltages, in comparison to normal, and is saturated at higher voltages. When added to the exponential characteristic of Ioff current, the contribution of the stressed GOX will reduce the slope of Sicc, and will increase its absolute value at lower voltages. Defect leakage source has a similar impact on the dependence of Sicc on temperature. Shorted gate oxide resistance has weak temperature dependence, while off-state transistor leakage increases exponentially with temperature increase. Therefore, we anticipate that a defective unit will have a weaker Sicc versus temperature slope than a normal unit.


Figure 3 Ig-Vg characteristics for N-well capacitor.


Curve 1- intrinsic IV (first sweep from 0 to –6V), curve 2 – 2nd sweep stress induced IV, curve 3 – 3rd sweep and curve 4 – 4th sweep.


FA techniques have huge advantage over electrical characterization: they can resolve locally the sources of the leakage by means of emission imaging techniques.


GOX capacitor leakage (Fig.3) is difficult to distinguish when there is a background of high normal Ioff leakage of a transistor at the product level. On the other hand, it can be easily imaged in an emission microscope (EMIC). This is due to the fact that a leakage source is localized at one damaged point of the capacitor, where the current flows through the silicon cause photon emission.


In our experiment, the units with normal slope did not show emission/leakage sources, while the units with the low slope showed between one to four leakage sources.


The same characterization was applied to the units that passed a high voltage lifetest (HVELT). Failed units showed leakage sources at the same locations. Here we integrated electrical charac-terization on a large sample size (Sicc) with an FA imaging technique (leakage source detection). We found that high leakage sources are located at the nodes where long metal lines were connected to the gates. We assumed that these lines may act as antennas for the plasma induced charge. The sources of leakage were the cause of functionality failure after HVELT but we also characterized functional units that had the same leakage sources. The defect may cause immediate functional failure (due to charge in the process), and reliability failure in production BI/ HVELT/ in the field. At the same time,the defect may cause additional leakage, but this does not harm the product. The difference lies in the different margins of the units for the defect. The question is, how to estimate this margin?


We can collect statistics for different electrical measurements and define normal baseline behavior,and we can relate the deviations from the baseline to different defect mechanisms. Each defect mechanism has its own risk in the functionality and reliability of a product. Therefore, in order to improve technology and yield, it is important to estimate the product margin with regard to the most dangerous defect mechanisms.


Application of Voltage Stress to Margin Definition


A reliable product withstands numerous stresses in the manufacturing process and in the field. It is important to estimate the degradation of the defect mechanism in order to predict reliability. The estimation of the degradation impact in time may be accelerated by voltage, current, and temperature [8].


In our experiment, electrical and EMIC characterization indicated the presence of a gate oxide degradation mechanism. The importance of the role of gate oxide quality in modern VLSI is crucial. Leakage through damaged gate oxide can easily cause functional


failure through stuck at, bridging or other fault models.


Parametric shifts due to GOX damage occur in Sicc and Fmax. The gate oxide degradation mechanism is strongly process and design dependent. In modern submicron technologies, gate oxide quality is influenced by plasma in different process steps (plasma charging is equivalent to voltage stress). Many geometrical design related considerations are involved.


The size of the metal line connected to the gate defines the amount of charge that is transferred to the gate from the plasma. This effect is covered by an antenna ratio design rule that defines the relation between metal and gate sizes. The current path from the gate to the substrate is design related, therefore the build up of potential on the gate varies widely. In the early stages of process development it is difficult to introduce design rules that cover all the problems related to gate oxide plasma charging. Beyond that, the design rules are a trade-off between real design needs and transistor level stress data. Therefore, charging cannot be eliminated completely.


One of the best techniques of charge related GOX degradation is constant voltage stress [7]. The design of our experiment included baseline characterization(electrical and EMIC), and FA of BI failures. Next, we introduced constant voltage stress in order to accelerate the degradation mechanism.


Experiment details: Typical units from two steps of the same product design were chosen for the experiment: a step (step 1) with large antenna ratios (leakage sources were associated with these points), and another product step (step 2) where only low antenna ratios were permitted. Before the experiment, all units passed normal BI and were tested to check for functionality and Sicc. The units were prepared for backside emission measurements in order to obtain full chip transistor visibility.


After preparation, the units were loaded on a tester and inserted in static mode. Sicc was measured as function of supply voltage (Vcc) and temperature (T). Emission measurements (EMIC) were performed at nominal Vcc conditions and room temperature.


# Failure Analysis of Sub-Micron Semiconductor Integrated Circuit Using Backside Photon Emission Microscopy


Failure Analysis of Sub-Micron Semiconductor Integrated Circuit Using Backside Photon Emission Microscopy


Lim Soon, Bi Jian Hua, Goh Lian Choo, Neo Soh Ping & Sudhindra Tatti*


Chartered Semiconductor Manufacturing Ltd Quality & Reliability Assurance Department


Failure Analysis Group


* Technology Development Group, Singapore


(iii)


All 5 units were tested, bitmapped and static current measured again. No units were found defective after the back thinning.


The experiment indicated that the sample preparation process was safe and did not alter the device functionality. During sample preparation, proper care and precaution should be taken to avoid causing ESD damage to the device.


Practical Considerations


The backside technique is not intended to replace the conventional front-side approach, but rather to complement existing fault isolation techniques. The backside approach entails a delicate sample preparation process, which is avoided in conventional front-side approach. For example, decapsulating a packaged IC using a jet-etcher for front-side emission analysis is much easier and faster than the backside milling process. Furthermore, the backside approach brings forth some issues which the analyst should consider and resolve.


Possible sample damage


The backside sample preparation or silicon thinning process entails an inherent risk of damaging the sample during milling of the molding compound or silicon substrate. This risk increases especially for small and thin packaged parts because the tolerance for error becomes very critical and the part can be easily damaged. Over-thinning the silicon on a wafer can also damage the sample, shown in Figure 9. Once the sample is damaged, it implies the end of the analytical effort and possibly the loss of information which are critical for decision disposition.


Figure 9 Crack on the thinned region of a wafer.


Remaining silicon thickness at the thinned region is approximately 200um.


Difficult for further analysis


Observing emission in the integrated circuit is frequently insufficient in helping the FA engineer


arrive at the root cause of the failure. Further physical analysis, e.g. layer strip-back by application of chemical wet etch or reactive ion etching, is frequently required to expose the location of the emission for inspection in the scanning electron microscope. Samples which are too thin (after thinning) pose a big challenge for further physical analysis as they can be easily damaged during the delayering process.


Viability of electrical biasing


IC sockets of standard packages for packaged part backside analysis are not commercially available. For analysis on packaged parts requiring only static biasing for a few pins, wires can be soldered onto the leads for this purpose (Figure 10). For packaged parts requiring electrical biasing for more than a few pins,customised sockets have to be fabricated. Similarly,for wafer backside micro-probing, existing commercial backside probe-stations allow up to 4 or 6 probes to be used due to space constraint. For wafer level devices requiring more, probe cards can be used. However, landing a probe-card with the wafer facing down can be a challenging task especially for small geometry devices.


Figure 10 A 28PDIP device with wires soldered to the leads to provide electrical bias to the device.


Longer analysis time


The backside sample preparation is a delicate procedure. Consequently, this extends the analysis time, which sometimes is difficult to justify in a competitive foundry manufacturing environment. If emission can be observed using the front-side approach, then the analyst is probably better off using the front approach so as to reduce the overall analysis time.


Case History


(1) 0.5um PDIP device with EOS failure.


Several 0.5um packaged devices failed pin leakage test after burn-in. As the driver circuitry connected to the leaky pin were obscured under broad metal power buses, backside analysis was applied to locate the fail site. The molding compound and die paddle were removed using mechanical milling to expose the silicon substrate. The exposed silicon substrate was polished to a mirror finish before subjected to analysis. An emission was observed at the first ntransistor connected to the bonding pad, shown in Figure 11. The site of emission was deprocessed to polysilicon for further examination. The cause of the emission was identified to be gate to source/drain leakage as a result of an electrical over-stress (EOS)event during the burn-in process (Figure 12).


Figure 11 Emission image acquired via the backside of a 0.5um PDIP device. Emission was observed on an n-channel transistor of an inverter connected to a bondpad. With this technique, the exact location of the emission/defect can be precisely identified. The black mist/shadow near the top of the micrograph is caused by internal reflection as a result of unevenness on the surface of the silicon after milling.


Figure 12 Site of emission stripped back to expose polysilicon. Fused polysilicon shorting the gate to the source/drain of the transistor was observed.


Acc.V Spot MagnDet WD


fm


5.00 kV 3.0  25579xTLD 4.9 UNIT 42.WF2


(2) 0.35um GOI test structure failure.


A wafer level 0.35um gate-oxide integrity (GOI) test structure was submitted for failure analysis. From the top, the structure was totally concealed by dense dummy metal lines such that emission was not observable. Backside analysis was performed for the device without thinning the silicon substrate. This was due to several considerations :


(i)


the sample was unique, it was definitely not worth the risk associated with thinning,


(ii)


well doping level of the device was low, and


reasonably clear image was obtainable.


Backside wafer level micro-probing was performed


Pin A4


to replicate the electrical failure. A single emission site was observed originating from the edge of the polysilicon gate (Figure 13). A pin hole was observed after layer strip-back at the location of emission.


(Figure 14)


Vdd=2 8V:1=-4.05mA


Figure 13 Point emission observed through the


silicon substrate on a Gate-Oxide Integrity test (GOI)structure. It can be observed that the emission


originated from the poly/diffusion edge. Emission is


viewed through unthinned silicon ~ 480um thick.


Figure 14 SEM micrograph of the site of emission after strip-back to silicon substrate. Pinhole on the substrate, a result of gate-oxide rupture, was


observed.


(3) 0.30um SRAM with Iddq failure.


A low yielding wafer with high Iddq as major cause of failure was submitted for failure analysis. This device had 2 levels of very dense metal interconnects which masked any observable emission. Backside analysis was performed using backside wafer probing to locate the source of leakage. Emission was observed (Figure 15) and layer strip-back performed for inspection at the emission site. Poly to diffusion


contact bridging due to micro-masking was observed(Figure 16).


Bondpad


StUCur3:ntest


unit1


Figure 15 Emission observed via backside analysis.


Emission is viewed through 480um of p-type silicon.


Figure 16 Poly to diffusion contact bridging was observed after exposing site of emission.


(4) 0.35um test structure failure due to polysilicon bridging to source/drain diffusion


A wafer level electrical test structure for polysilicon bridging was submitted for failure analysis. The polysilicon comb structures were fabricated under bonding pads which concealed a large part of the structure, shown in Figure 17. Backside wafer probing was applied and photon emission analysis performed. Emission was observed coming from the structure, and further analysis showed the failure to be due to residual polysilicon filaments (Figure 18).


Figure 17 Optical photo showing the top metal


interconnects and bonding pads concealing most part of the test structure.


Spot Magn


5.00kV 3.059222xTLD 4Det WD aAche


Figure 18 Residual polysilicon filament observed at site of emission after stripback.


Acc VSpot MagnDet oD


+1um


5.00 kV 3.0 28040x TLD 4.3 CSM FA LAB.UNIT


Backside photon emission microscopy is an important and effective complementary fault isolation technique for failure analysis of deep sub-micron ULSI devices. As wafer fabrication technology progresses, the use of dense multi-level metallization and advanced packaging technology present problems which render conventional front-side emission microscopy less effective. The backside approach is a viable solution to these problems.


However, the backside approach entails a delicate sample preparation process which also brings forth issues that the analyst has to consider and resolve.


1) T.W. Lee and S.V. Pabbisetty, Microelectronic


Failure Analysis Desk Reference, 3rd ed., ASM International, 1997.


2) Ching-Lang Chiang and Daniel T. Hurley,Dynamics of Backside Wafer Level Microprobing, 1997.


3) W. Spitzer and H.Y. Fan, Infrared Absorption in N-Type Silicon, Phsics Review, Vol. 108, No.2,pp. 268-271, 1957.


4) T.W. Joseph, A.L. Berry and B. Bossman,Infrared Laser Microscopy of Structures on Heavily Doped Silicon, Proc. ISTFA, pp1-7,


1992.


5) N.M. Wu, K. Weaver and J.H. Lin, Failure Analysis From Back Side of Die, Proc. ISTFA,pp 393-399, 1996.


6) S.S Lee, J.S. Seo, N.S. Cho, S.Daniel,Application of Backside Photo and Thermal Emission Microscopy Techniques to Advanced Memory Devices, Proc. ISTFA, pp 63-66, 1997.


7) K. Naitoh, T. Ishii, J. I. Mitsuhashi, Investigation of Multi-Level Metallization ULSIs by Light Emission from the Back-Side and Front-Side of the Chip, Proc. ISTFA, pp 145-151, 1997.


Electronic Device Failure Analysis Society, editor, p 117-124


DOI: 10.1361/cp1999istfa117


# Sample Preparation for Backside Failure Analysis Using Infrared Photoemission Microscopy


Sample Preparation for Backside Failure Analysis Using Infrared Photoemission Microscopy


Alastair Trigg


Institute of Microelectronics, Singapore


Loh Peak Yong


Ngee Ann Polytechnic, Singapore


For conventional photoemission microscopy the silicon is thinned to a few tens of micrometres for backside imaging since silicon is opaque in the visble part of the spectrum. However, at wavelengths greater than approximately 1050 nm, most silicon is effectively transparent. Hence, the use of an infrared


photoemission microscope (IRPEM) operating at wavelengths of 1100 to 2500 nm, usually eliminates the need for thinning, except where the silicon is heavily doped. However, the plastic encapsulation of packaged devices must be removed and the die surface polished. A polishing system has been evaluated and optimised for this purpose. Surface roughness (Ra) of 1 nm or better was obtained.


Representative applications are shown and discussed.


Photoemission microscopy is a widely used tool for failure analysis both of packaged devices and wafers.


Over the last few years there has been growing interest in imaging the photoemission from the backside of the die or wafer. There are several advantages to this:


• Failure sites are often hidden beneath metallisation. This is increasingly a problem as more levels of metal are used. Even where emission is visible the metallisation can obscure its origin and confuse interpretation.


• Imaging from the backside does not require potentially destructive decapsulation techniques to be used on the surface of the die.


• For flip-chip mounted devices, backside imaging is the only way of imaging the device without destroying the connections to the outside world.


The tendency for more complex ICs to have many metallisation layers and the increasing use of flip chip technology is accelerating this trend. In conventional PEM, imaging light in the visible and very near infrared range, the silicon must be thinned to a thickness of a few tens of micrometres in order for photoemission to be detected from the back surface.


This can be a difficult and time consuming process,requiring, for packaged devices, precise knowledge of the position of the die in the package.


Commercial equipment, based on numerically controlled milling machines, has been developed for this purpose [1,2]. These are not always ideal for the a failure analysis laboratory, handling devices from many different manufacturers whose dimensions are not precisely known. An alternative approach is to use infrared photoemission microscopy. This has several advantages over conventional photoemission microscopy in the visible part of the spectrum which have been discussed elsewhere [3 - 7].


The main advantage for backside failure analysis is that at wavelengths greater than that corresponding to the band-gap, lightly doped silicon is effectively transparent to infrared. Based on optical parameters given in reference 8 the transmission of a silicon wafer between 800 and 2600 nm for dopant levels


between 1016 and 5x1018 cm-3 can be calculated(Figure 1). Up to 1017 cm-3 (approx. 0.1 ohm-cm resistivity or greater) the free carrier absorption is low but at higher dopant concentrations it becomes


progressively greater until at 5x1018 (approx.


0.01 ohm-cm) the peak transmittance is only about 20%. Thus for most devices based on N or P substrates no thinning of the silicon is necessary. For N+ and P+ substrates thinning may be necessary for infrared imaging. Even where no thinning is needed,it is still necessary to remove the package material from devices and to polish the back surface of the silicon since this is usually lapped and quite rough.


For this purpose a backside polishing system


developed by South Bay Technology (SBT) [9] has been evaluated and the grinding/polishing conditions optimised to meet the requirements of a well polished surface in minimum time.


Figure 1 Calculated transmission of 0.7 mm thick silicon wafer for various dopant densities.


7


The Infrared Photoemission


Microscope (IRPEM)


The microscope has been described in detail previously [6] . In summary, the IRPEM comprises a probe station on which is mounted the sample, which may be either a packaged device or a wafer, a lens turret which allows lenses to be selected to give the correct magnification, an illuminator, an infrared(IR) camera with a wavelength range of 800 to 2500 nm, and associated electronics and computer so


that the image can be displayed on a monitor.


Incorporated into the IR camera is a filter wheel which enables the spectral response to be determined


so that different mechanisms can be separated. The filters are centred at 850, 1100, 1250, 1650, 2150,and 2300 nm. A schematic of the apparatus is shown


in Figure 2.


Figure 2 Schematic of IRPEM.


Backside Polishing System


The model 575 Backside Emission Analysis Preparation System (BEAPS) manufactured by South Bay Technology is a polishing machine used to


100%


polish flat a predefined area, maintaining die


1E16


planarity within 10 µm with little supervision.


1E17


Schematics of the apparatus are shown in Figures 3 &


4. Further details can be found in Reference 9.


5E17


1E18


(%)Transmission


2E18 5E18 008001200160020002400 Wavelength (nm)


2. Support arm, 3. Arbour shaft,


4. Oscillating stage, 5. Grinding/polishing wheel,


6. Pedestal for rotating specimen, 7. X-axis adjustment.


Figure 3 Plan view of polishing system.


1. Micrometer to adjust depth, 2. Contact for LED,


3. Support arm, 4. Grinding/polishing wheel,


5. Sample, 6. Pedestal for rotating specimen,


7. Specimen stage, 8. Arbour shaft.


Figure 4 Front view of polishing system.


The specimen is mounted on the specimen stage using a low melting point wax. Grinding wheels of 10 and 5 mm widths are supplied. Polishing wheels comprise brass discs of 5 or 10 mm width on which polishing papers can be applied using double-sided adhesive tape. Alternatively they can be used to


Filter wheel


95555←Focal


plane array


Lens


polish the sample using diamond paste. For final polishing a felt wheel impregnated with colloidal silica can be used. The sample can be oscillated so as to increase the polishing area in one direction. This is necessary for dies larger than a few mm if a reasonably flat polished surface is to be obtained.


The sample can also be rotated but this facility was not found to be useful in the present work.


Results From Polishing Trials


Coarse Grinding


For plastic packaged devices it is first necessary to grind away the mould compound, the die paddle and the die attach adhesive before polishing the silicon.


For wafers, the silicon is already exposed and for flip chip devices the silicon may be exposed or there may be a glob top material over it. It was found that moulding compound or glob top material could be rapidly ground away using the coarse grinding tool supplied by SBT but that this caused severe damage if allowed to penetrate to the silicon. The polishing machine is fitted with a micrometer which enables a predefined amount of material to be removed. In practice the amount of material to be removed is not always known in advance so this may be of limited value in these cases. For most devices it proved adequate to allow grinding to the die paddle. Once the die paddle was exposed the coarse grinding tool


was removed and 5 or 6 µm abrasive used thereafter until the silicon was fully exposed. It is essential to ensure the sample is repositioned at exactly the same location after each grinding/polishing step. The small amount of backlash in the rotating stage sometimes caused problems in this respect. Methods of minimising this problem were to coarse grind a larger area than that required for final polishing or to clamp the rotating table in position.


Optimisation of Polishing Procedure


For the purpose of optimising the polishing procedure, samples of silicon wafer approximately 1 cm square, with a typical lapped back surface were used. In order to minimise the time taken for the experiments the samples were not oscillated so that the polished area has the shape of the polishing wheel, i.e. 5 mm wide in one direction and having a radius of approximately 25 mm in the other. For the polishing trials a profileometer (Dektak 8000) was used to evaluate the performance. This provided three parameters, average surface height (ASH), average surface roughness (Ra) and average surface waviness(Wa). ASH gives a step-height measurement in applications where roughness or noise is present on the profile trace. It computes the difference between two average height measurements, so as to indicate the depth of material removed. Ra is the arithmetic average deviation from the mean line. For this work a


short (high) pass filter of 20 µm was used for calculating roughness data. This filters out low frequency waviness signals and allows high frequency roughness data to pass through. Wa is the average deviation of waviness from the mean line(corresponds to Ra). For this work a long (low) pass


filter of 200 µm is used for calculating waviness data.


This filters out high frequency roughness signals and allows low frequency waviness data to pass through.


For the initial trials only the Ra and Wa were measured. The sample surfaces were also evaluated qualitatively both by eye and using an optical microscope.


Initial Trials


In the initial trials the performance of different polishing media, were evaluated. For each trial the sample was polished successively for 30 minutes


using 6/5 µm, 3 µm, 1 µm diamond or silicon carbide abrasive, followed by colloidal silica. Between each polishing step the sample was thoroughly cleaned using isopropanol. A low polishing load was used.


The results obtained are shown in Table 1.


Table 1 Results of initial polishing trials.


||Polishing medium |Ra (nm) |Wa (µm) |Comment |
|---|---|---|---|---|

||Diamond paste |5.4 |4.7 |Few scratches but very |

||Diamond paste |5.4 |4.7 |uneven with obvious |

||Diamond paste |5.4 |4.7 |furrows |

||Diamond cloth |2.8 |9.2 |Few scratches but |

||Diamond cloth |2.8 |9.2 |uneven |

|carbide |Silicon paper |3.0 |2.5 |Very few but deep scratches. Flat surface |

|paper |Diamond |2.2 |1.9 |Very few scratches. Flat surface |

One lubricant, based on ethylene glycol was used for all the work described here. Another lubricant supplied by South Bay Technology, whose composition was not known, was tested but was found to evaporate too quickly for consistent results to be obtained.


On the basis of the results obtained, subsequent evaluations concentrated on the diamond and silicon carbide papers. The latter while not providing such a good final surface finish is substantially cheaper so it


was decided to use silicon carbide for the 5 µm and 3µm polish steps and evaluate the relative performance of the two media for the 1 µm step.


0 50 100 150


Time (min)


0g 600g 1200g


0 100 200 300 400 500


Time(min)


|||11|
|---|---|---|

|◆|||

0 20 40 60 80 1 0 120


0g 6 0g 1


300 Roughness (um)400


Ti


i )


600g 120 g


Determination of Optimum Load


Weights can be mounted on the arm of the polishing machine so as to increase the load on the polishing wheel. In general for mechanical polishing, high loads increase the rate of removal. For metallographic applications, care has to be taken to ensure that


um)Waviness (


smearing does not occur, particularly in soft materials but for the current application this is not a concern.


Using the 5 µm silicon carbide paper the amount of material removed as a function of time and load was determined together with the parameters of Ra and Wa. The results are shown in Figures 5 – 7.


Figure 5 Depth of material removed


as a function of load and time.


Figure 6 Roughness as a function of load and time.


Figure 7 Waviness as a function of load and time.


As expected the higher load increased the rate of removal and it appears that with zero load there is very little removal occurring after the first 2 minutes.


Both the Ra and Wa values increase with time,indicating that the final surface is actually rougher than the initial lapped surface of the silicon. The dependence on load is not very clear, particularly after 10 minutes. It was observed that because of the design of the arm on which the polishing wheel is mounted, the application of the load tilted the polishing wheel, resulting in uneven polishing. This was particularly severe with 1200 g load. A modification was subsequently made so that the weights are positioned directly over the polishing wheel. At 1200 g load it was also found that the paper tended to tear or peel off the polishing wheel. Hence further work used 600 g as the standard load for


polishing. Since the 5 µm abrasive increases roughness compared to the lapped back surface it is used only to remove the die paddle and die attach adhesive from packaged devices, to remove glob top from flip-chip devices or where it is required to thin the silicon.


Determination of Optimum Time for 3 µm Abrasive


The samples were first polished using 5 µm abrasive for 5 minutes as described above and the roughness of each sample measured at two locations. They were


then polished for varying times using 3 µm paper and the roughness measured again. The results obtained are shown in Figure 8. It can be seen that the maximum reduction in roughness occurs after 10 minutes polishing time.


0 50


200 Roughness (A)250


5um 1st


5um 2nd


3um 1st


3um 2nd


Roughness (A)0


1um 1st


1um 2nd


100 150 200 250


5u 1st 5um2nd 3um1st 3um2nd


0 20 40 60 80


3um 1st 3um 2nd 1um 1st 1um 2nd


0 0108 620 a


u30u s


s40 V50


Figure 8 Roughness of samples after various


polishing times for 3 µm silicon carbide.


Wear Out Effects


Unlike a conventional polishing wheel, where the area of abrasive is far greater than the area of the sample, the area of abrasive on the grinding wheel is relatively small, for a 5 mm square chip just 31 times greater than the chip area. There was therefore a concern that the lifetime of the abrasive might be limited by wearout. This effect was studied by


polishing samples using 5 µm silicon carbide and 6 µm diamond papers for various times. The results obtained are shown in Figure 9. The diamond paper is clearly more resilient whereas the silicon carbide paper is seriously degraded after 5 minutes.


Therefore, although silicon carbide paper gives acceptable results in terms of roughness, it is not recommended for applications in which longer polishing times are required


Figure 9 Depth of removal against time for silicon carbide and diamond papers.


Figure 6 Image taken through 480um of unthinned p-type medium doped silicon. The features on the device can still be made out.


Figure 7 Image of the same device in Figure 6 taken


through 150um of silicon. The image clarity is


improved.


Figure 8 Image taken through 50um of p-type


silicon. There is no observable improvement in the


quality of the image as compared to that taken


through 150um of silicon shown in Figure 7.


Sample Integrity After Thinning


It is important to ensure that the sample integrity and electrical functionality is preserved after sample preparation for backside analysis. Concerns were raised as to whether the high speed mechanical milling used for removing the molding compound and thinning the silicon substrate may cause the generation of intense heat that is high enough to affect the device characteristic or in the worst case destroy the device.


A simple study to ascertain this was performed. Five 84PLCC samples (0.35um 1 Mbit SRAM test chip)were polished to various thickness of remaining silicon substrate: 150um, 130um, 100um, 80um and 50um. The experiment was performed in the following sequence :


All 5 units were tested and bitmapped prior to thinning. Static current of each device in standby mode was also measured. All 5 units were verified to be good both functionally and parametrically.


All 5 units were thinned to a remaining silicon thickness of 150um, 130um,100um, 80um and 50um.


The extensive use of planarization in many of today's


leading process technologies significantly reduces the effectiveness of FIB circuit modification and debugging. Planarization has played a significant role in the development of denser chips with increasingly smaller geometries. Fully planarized devices offer little or no surface features on which the FIB operator relies for orientation and alignment. These conditions lead to increased debug cycle times and decreased success rates using the FIB. Recent FIB tool advancements in the field of C4 (controlled-collapse chip connection) flip-chip packaged device modification and debug have also made it easier to work on highly planarized conventional wire-bond technology. The integration of an optical microscope with an infrared camera into the work chamber allows the operator to view the circuitry under the surface layer. This paper will offer several techniques for overcoming the challenges that planarized devices present by using this in-situ optical microscope.


When properly implemented, these techniques can significantly improve the success rate and throughput time of device modification on highly planarized parts.


Focused ion beam tools acquire images using secondary electrons and ions that display surface topography very well, but provide little information at depth. Traditional FIB circuit modification has relied on direct correlation of surface features with measurements taken from printed diagrams or images to place the mill boxes in the proper locations. On non-planarized devices, this method works very well as multiple metal layers can be seen using the secondary electron imaging of the tool (Figure 1).


Figure 1 FIB SE Image of a non-planarized device showing top and underlying metal layers.


More recently, CAD navigation databases have provided a stronger tool for placing the edits and aligning devices, but this method also relies on surface features for accuracy.


Planarization


As silicon technology has advanced, escalating device integration and complexity has increased the number of active devices per unit area of the chip dramatically. Multiple level metalization is needed to provide interconnections between each of these active devices. Each metal level must be planarized once it is formed in order for the next higher layer to be created. Without planarization, further metalization at these complexities would be impossible due to depth-of-focus and conformity issues.


Planarization can be divided into four categories qualitatively: (Figure 2).*


a) Smoothing: Corners are rounded and sidewalls are sloped, but the step height is not significantly reduced.


b) Partial Planarization: Smoothing plus a reduction in step height locally.


c) Local Planarization: Complete filling of smaller gaps (1 to 10 mm); total step height to flat areas not significantly reduced.


d) Global Planarization: Local Planarization plus a significant reduction in step height.


Figure 2 The four qualitative categories of


planarization.


Even local planarization can cause difficulty to the FIB operator if the edit area is too far from surface metalization. Figure 3 is an example of local


planarization over a 150 X 150 µm area. Notice the charging effects and pinholes caused by scanning the beam across this area. These are common features that occur in highly planarized devices that add to the difficulty and affect both the time and the yield of the edit. The charging causes the beam to drift and the bright pinholes are a result of ESD and can damage the device. These effects are further described in the example in the next section.


Figure 3 A secondary electron image of a locally planarized device.


Optical microscopes


Optical microscopes have played an important role in failure analysis laboratories since the beginning of the silicon era. Powerful plain light microscopes allow visualization of most metal lines in today's traditional wire-bond packaged chip technologies.


Recent use of infrared light equipped microscopes has also allowed engineers to image through the backside of thinned down C4 packaged devices.


Optical images can be taken that show multiple metal layers and can then be used to align mill boxes on those layers below the surface (Figures 4a, 4b, 4c,4d). Two powerful features of using a microscope outside the FIB chamber are the ability to change magnifications and focus depths. Magnification changes are unavailable, currently, to the in-situ microscopes, but changing the focus depth is not.


Figures 4a, 4b, 4c, and 4d are optical images that show the same area of the device as in Figure 3 at two different magnifications and with a partially completed mill. The mill box in Figures 4b - d has


drifted approximately 5 µm across the part due to localized surface charging. A relatively low beam current (100 pA) and “Ion Mode” milling with charge neutralization was needed in order to complete this edit.


000a


光


Figure 4a Optical image of area in Figure 3 at 200X magnification.


Figure 4b 500X optical image showing Metal 4 in focus with FIB mill box superimposed.


Challenges


As silicon technology presses forward, designers pack more and more elements into a single chip. This leads to an ever-increasing task of failure analysis and debug on devices that contain five, six, and even up to seven layers of metal interconnect. These devices invariably contain a high degree of planarization, which makes it virtually impossible to perform even simple edits without detailed information on each layer of the chip. Traditional device modification has relied on printed maps of the


Figure 4c 500X optical image showing Metal 3 focus with FIB mill box superimposed.


Figure 4d 500X optical image showing Metal 2


focus with FIB mill box superimposed.


logic design or on optical or other images showing surface features. As microchips have become more complicated and our tools for modification more powerful we have started to rely on CAD databases and image overlays for higher levels of accuracy. All of these tools have one thing in common; they all rely on surface information to accurately and precisely place edits on the chip. On devices that have global and even local planarization, these techniques are inadequate. To compound matters, planarized areas also show a higher degree of surface charging and ESD due to the materials used in the chemicalmechanical polishing (CMP) process.


Techniques


"Seeker holes"


One technique that has been common for some time is to open a "seeker" hole to a lower level metal. This requires the operator to locate an appropriate area near the intended site and open a window to the lower level metals without damaging the device.


Once exposed, the metal layer(s) can be aligned using any of the standard methods and the proper location for the edit can be found (Figure 5)*. Use of this approach, however, necessitates an easily identifiable metal line in close proximity to the area of interest.


This technique is not always available due to the lack of a suitable area in which to open and align to.


Another factor to consider when employing this method is that care must be taken so as not to cut any of the metal lines opened for alignment. As the density of the active regions of a chip increase, the interconnect geometry shrinks and this makes for very thin metal lines.


Figure 5 Seeker hole used to locate five


separate nodes.


Overlays


Another common technique today uses the image overlay features of most advanced FIB tools. Stored TIFF images, scanned logic plots, or CAD navigation database information can be used, with alignment features, on a local area of interest that contains some surface elements in which to align. Using the software controls of the FIB tool, a coordinate system can be transposed onto the stage from the database or image by locking common reference points. Once locked, the operator can navigate to the intended locations using the overlay and the software will


adjust for scale and rotation. This technique requires a very accurate stage and a process that is well controlled in order to place the mill correctly. Only the top model FIB tools, specifically designed with stage accuracy in the sub-micron range, allow this procedure to work consistently on fully planarized or flip-chip packaged devices. For the most advanced chips, laser encoded stages are required and considerable thought must go into choosing proper alignment marks in order to land the beam in the proper place.


The above two techniques can be combined by milling alignment marks, such as seeker holes or


small (<20 µm) crosses, into the surface of the chip.


The device can then be removed from the FIB chamber and an optical microscope is used to generate an overlay image that contains the marks or seeker holes and the buried metal layers. The device is returned to the FIB chamber and the overlay method is used to place the mill boxes with much higher confidence. The drawback with this technique is that the time involved with sample exchanges and alignment can be very intensive.


In-situ optical scope


The tool used in this paper was designed for backside circuit modification and thus is configured with a relatively low resolution, infrared camera and microscope. Higher power oculars and plain light systems are available and are much more appropriate for front side high-end microsurgery. In this model FIB, the microscope is positioned off-axis from the ion beam due to chamber space considerations. Thus,a stage shift is required in order to use the microscope (Figure 6). Because of this optical axis offset, the stage must be as accurate and repeatable as possible, as numerous optical to FIB image translations compound the stage error. In this case,the specified stage accuracy of the tool was


± 0.25 µm over an 8-inch area.


Figure 6 Screen shot of stage translation to optical position.


The use of the in-situ optical microscope technique can be demonstrated by the following example.


Figure 7 is an image of a fully planarized


140 X 140 µm area of a device. Again, note the charging effects and pinhole ESD damage associated with this material. The two boxes on the image were aligned using an optical image taken inside the chamber (Figure 8). The mill boxes in Figure 8 were placed so that their outer edges lined up with the thin horizontal Polysilicon lines visible in the center of the image. This marked the maximum upper and lower edges of the isolation cut on the higher vertical trending Metal 2 line. The isolation cuts had to be made precisely between the gaps indicated by the two thin Polysilicon and one wider horizontal Metal 1 lines in the image. The stage was returned to the FIB axis and the mills were partially completed. A second optical image was taken showing the location of the incomplete mills in relation to the circuitry below(Figure 9). Once the mill locations were verified, the isolation cuts were completed successfully. Due to the extremely fragile nature of polysilicon, a seeker hole could not be used for vertical alignment in this situation. A seeker hole was used, however, for the horizontal placement of the mill boxes. This is pointed out at the top of Figure 10 as the dark box running across the three vertical Metal 2 lines.


Figure 7 FIB SE image of a fully planarized area with two aligned edit boxes.


Figure 8 In-situ optical image showing alignment of edit boxes.


Figure 9 In-situ optical image of partially completed mills, verifying placement of edits.


Figure 10 In-situ optical image showing placement of seeker hole at top.


This example demonstrates two powerful techniques of using an in-situ optical microscope for microsurgery. The first is actual placement of edit boxes with a high level of accuracy. The second is the ability to verify the mill locations after placement,but before metal lines are opened.


Limitations


The main limitation of this technique, namely resolution, is apparent in the example given above.


The infrared microscope is not well suited for small


geometry devices and the images reflect that shortcoming. The inability to change magnifications is another serious limitation that needs to be addressed. Global alignment from the surface is still required in order to find the general area of interest.


A small magnification lens would help to locate the area and a high magnification lens could be used to place the edits. The other limitation to consider is the stage accuracy due to the movement between optical and FIB image locations. A coincident axis alignment between the FIB column and the optical microscope would alleviate this problem somewhat, but then the issue of either milling or viewing at an angle would need to be addressed.


The task of performing device debug and circuit modification has been complicated by the extensive use of planarization on most modern chip technologies. Traditional techniques have always relied on some surface information near the intended edit locations for alignment, orientation, and placement of mills. Without those local alignment features, previous techniques such as seeker holes and image overlays are much less effective. With the inclusion of an optical microscope inside the FIB chamber, the problem of performing microsurgery on highly planarized devices is simplified. In many cases it is no longer necessary to expose underlying metal layers using seeker holes or removing the sample form the chamber to check alignment marks.


Combined with a highly accurate stage (± 0.25 µm),an edit location can be found optically and the boxes placed or alignment marks made with confidence in a very short time. The operator can begin the edit and continually verify placement optically, provided the microscope has suitable resolution.


The limitations of this technique are apparent,however, when resolution of the smallest lines comes into play. The infrared setup used on most flipchip FIB tools is not suitable for high-end microsurgery tasks. The inability to change magnifications is also a serious drawback that could be remedied by inclusion of a mechanized ocular turret. The stage accuracy required for off axis optical imaging is also an issue,but presently, the most advanced tools are capable of providing this.


1) C. Y. Chang and S.M. Sze, ULSI TECHNOLOGY, p 425, McGraw Hill, 1996.


2) S. X. Li, “Performing Circuit Modification and Debugging Using Focused-Ion-Beam on MultiLayered C4 Flip-Chip Devices”, ISTFA Proceedings, 15 – 19 November, 1998.


3) C. Burmer, S. Gorlich, S. Pauthner, “Layout Overlay Techniques to Improve Failure Analysis”, ISTFA Proceedings, 15 – 19 November,


1998.


4) Micrion Corporation: “Micrion 9800 FlipChip Focused Ion Beam System Operator’s Reference Manual”, Chapters 13 – 14 (1997).


Electronic Device Failure Analysis Society, editor, p 135-140


DOI: 10.1361/cp1999istfa135


# Investigation on the Corrosion of Cu Metallization in the Focused Ion Beam System Due to a low I2 Background


Investigation on the Corrosion of Cu Metallization in the Focused Ion Beam System Due to a low I2 Background


H. Bender, S. Jin, I. Vervoort and Y. Lantasov


The corrosion effect of an I2 background during focused ion beam (FIB) analysis of Cu-metallization structures is investigated. In-situ Cu corrosion in the FIB system can occur even if the I2 gas has not been used anymore in the last 24 h before the loading of the Cu sample in the system including several vents and pump-downs of the chamber in that period.


Hence the I2 can have a long-term memory effect and is not compatible with FIB analysis or modification of devices with Cu metallization. Compositional and structural analysis shows that the reaction product is CuI.


Determination of Optimum Time for 1 µm Abrasive


The samples were first polished using 5 µm abrasive for 5 minutes and then using 3 µm abrasive for 10 minutes as described above and the roughness of each sample measured at two locations. They were then


polished for varying times using both 1 µm silicon


carbide and 1 µm diamond paper and the roughness measured again. The results obtained are shown in Figures 10 & 11.


||曝||
|---|---|---|

||88||

|81|||

Figure 10 Roughness of samples after various


polishing times for 1 µm silicon carbide paper.


Figure 11 Roughness of samples after various


polishing times for 1 µm diamond.


Both diamond and silicon carbide papers give similar results of 2nm roughness for all times of 5 minutes and more. One possibility is that the profileometer is unable to resolve roughness at this scale. Four samples, silicon carbide and diamond polished after 5 minutes and 40 minutes, were therefore examined using an atomic force microscope (Digital Instruments Nanoscope III) in tapping mode. The results are shown in Table 2.


Table 2 Summary of the Ra results obtained using the atomic force microscope.


||Roughness (Ra) (nm) |Roughness (Ra) (nm) |
|---|---|---|

||25µm2 area |Box statistics |

|1µm SiC for 5min |1.885 |0.691 |

|1µm SiC for 40min |5.622 |1.164 |

|1µm diamond for 5min |6.388 |2.793 |

|1µm diamond for 40min |4.284 |2.757 |

0 100 200 Depth (um)300 400 500


siliconcarbide diamondpaper


Because the total imaged area is very small it was found that different regions of the sample could give quite different results and that the roughness was often dominated by a few features. In the atomic force microscope it is possible to select a box to exclude such features and this gave rather more consistent values. On this basis the silicon carbide appears to give a better result although visually the diamond polished surface looked better.


Determination of Optimum Time for Colloidal Silica


Unlike silicon carbide or diamond polishing,colloidal silica is a chemical mechanical polish, i.e. it chemically attacks and removes silicon at the same time as mechanically abrading it. Experience in other application has indicated that there is no advantage in polishing for long times. Since colloidal silica polishing uses a felt polishing wheel the load has to be reduced. Experimentation showed that even with no additional weights on the wheel the felt was seriously deformed. The polishing machine has provision to apply weights to counterbalance the natural weight of the polishing arm and it was found that a 600 gram counterweight prevented overdeformation while still providing a reasonable pressure. Samples which had been previously


polished down to 1 µm abrasive were polished using the colloidal silica for 5 minutes.


The measurements of roughness obtained using the profileometer are summarised in Table 3.


Table 3 Comparison of roughness between 1 µm polish and colloidal silica.


parison of roughness between 1 µm polish and colloidal silica.


|Sample |Roughness after 1 µm polish (nm) |Roughness after 1 µm polish (nm) |Roughness after 1 µm polish (nm) |Roughness after colloidal silica |Roughness after colloidal silica |Roughness after colloidal silica |
|---|---|---|---|---|---|---|

||Dektak |AFM 25µm2 |AFM Box |Dektak |AFM 25µm2 |AFM Box |

|1 |2.3 |1.9 |0.7 |3.9 |0.8 |0.2 |

|2 |2.0 |6.3 |2.8 |2.5 |0.9 |0.2 |

While the profileometer indicates that the roughness increases, the AFM shows that there is in fact an improvement. However, there is a problem in removing all the colloidal silica particles after polishing. It was found to be essential to rinse and


ultrasonically clean the sample immediately after removing it from contact with the polishing wheel ensuring that it was not allowed to dry. Even then significant contamination of the surface by colloidal silica particles could be observed using the AFM.


Optimised Procedure


For small die, < 5mm, the optimised procedure based on the work described above is:


Set weights on polishing machine to + 600gram.


Coarse grind the mold compound until the die paddle is revealed.


Grind away die paddle using 5 µm silicon carbide or 6 µm diamond paper. If grinding with silicon carbide,paper needs to be replaced every 5 minutes.


Alternatively 3 µm diamond cloth can be used at this stage.


Polish for 10 minutes using 3 µm silicon carbide or diamond paper.


Polish for 5 minutes using 1 µm diamond paper.


Set weights on polishing machine to - 600gram.


Polish for 5 minutes using colloidal silica on felt wheel.


Immediately clean away colloidal silica residue.


For larger dies the machine should be set into the oscillating mode with a travel equal to or longer than the size of the die. The additional volume of material to be removed is calculated and the polishing times listed above increased appropriately. For longer polishing times diamond paper is recommended.


Based on this procedure packaged devices have been ground and polished to a mean roughness, as measured using the AFM, of 0.2 nm.


Applications


In order to validate the polishing process it has been applied to some simple device structures. In the first instance an operational amplifier chip (UA741CP) in a DIL plastic package was ground and polished as described above. It was operated with an input voltage of 1 V and an output current of 2mA. A typical backside image is shown in Figure 12. Here the photoemission image at 1250 nm (yellow) is superimposed on an illuminated image (blue). For comparison purposes another device was opened by conventional decapsulation using hot fuming nitric acid. Whereas two features can be observed in the backside image, only one of them, Feature A, could be observed from the front side. Measurements of the relative intensities from front and back sides indicated that the backside emission was approximately 5 times more intense. The spectral distribution indicated that the emission emanated from bipolar transistors in forward bias [6].


500 µm


Figure 12 Backside photoemission image of operational amplifier at 1100 nm wavelength


Transistor Array


In most bipolar devices, p-n junctions are designed to operate with current flow only in forward bias. Using a packaged transistor array enables the p-n junction to be reverse biased. (CA3046). An illuminated image of the whole IC is shown in Figure 13. Note that the formation of intermetallic compounds in the bond pads is clearly visible from the backside of the chip.


In Figures 14 & 15 emission images (yellow) are shown superimposed on the illuminated image (blue)for forward and reverse bias.


1 mm


Figure 13 Illuminated image of transistor array.


Figure 14 Forward bias PEM image from backside.


Figure 15 Reverse bias PEM image from backside.


For forward bias the intensity of emission at 1250 nm from the back surface was 3.7 times higher than from the front surface, while for reverse bias the intensity was 30 times higher.


ma o


Because these simple devices have relatively large feature sizes they are not very suitable for


5457


demonstrating the use of backside photoemission microscopy at high magnifications. For this purpose a microprocessor device was ground and polished in the same manner as described previously. A high magnification image of an input protection structure with a 5 volt input is shown in Figure 16.


50 µm


Figure 16 Input protection structure of


microprocessor. IRPEM image from backside.


A backside grinding and polishing technique for infrared photoemission microscopy has been developed capable of removing the plastic encapsulation and die paddle from a packaged semiconductor device and producing a silicon surface with a mean roughness of better than 1 nm. In order to minimise polishing times, high loads are required and this has necessitated modifications to the polishing system. The efficacy of this approach has been demonstrated by application to two bipolar devices. In both instances the intensity of emission from the back surface was considerably greater than from the front.


1) D T Hurley, "High Speed Diamond Based Machining of Silicon Semiconductor Die in Wafer and Packaged Form for Backside Emission Microscopy Detection", US Patent No 5698474 December 1997.


2) C Chiang, N Khurana, D T Hurley & K Teasdale, "Backside Emission Microscopy for Integrated Circuits on Heavily Doped Substrate",Proceedings of 24th International Symposium on Testing & Failure Analysis 447 - 453, 1998.


3) S Chen, B Shinseki, C Barutha & T Kha,"Infrared Imaging and Backside Failure Analysis Techniques on Multilayer CMOS Technology",Proceedings of the 6th IPFA 17-20, 1997.


4) D L Barton, P Tangyunyong, J M Soden, A Y Liang, F J Low, A N Zaplatin, K Shivanandan &G Donohue, “Infrared Light Emission from Semiconductor Devices”, Proceedings of the 22nd International Sym-posium for Testing &Failure Analysis, 9-17, 1996.


5) K Shivanadan & K Nyunt, “Application of an Infrared Astronomy Camera System for Photo Emission Microscopy”, Proceedings of the 21st International Sym-posium for Testing and Failure Analysis, 69-71, 1995.


6) A D Trigg, "The Infrared Photoemission Microscope as a Tool for Semiconductor Device Failure Analysis", Proceedings of the 6th IPFA 21 -26, 1997.


7) N M Wu, K Weaver & J H Lin, "Failure Analysis from Back Side of Die", Proceedings of the 22nd International Symposium for Testing and Failure Analysis, 393- 399, 1996.


8) J C Sturm & C M Reeves, "Silicon Temperature Measurement by Infrared Absorption: Fundamental Processes and Doping Effects", IEEE Transaction Electron Devices 39(1), 81-88,


9) S P Roberts & J M Patterson, "A Study of Effects of Backside Thinning on Integrated Circuits using a Precision Diamond Wheel Apparatus", Proceedings of the 24th International Sym-posium for Testing and Failure Analysis, 441 - 445, 1998.


Electronic Device Failure Analysis Society, editor, p 127-133


DOI: 10.1361/cp1999istfa127


# In-situ use of an Optical Microscope for FIB Microsurgery of Planarized Devices


In-situ use of an Optical Microscope for FIB Microsurgery of Planarized Devices


Patrick J. Wolpert and Raymond Lee


FIB International, Inc., Santa Clara, California


Copper metallization is introduced in the new generations of silicon devices. The optimization of the processing requires the analysis of the metallization structure by different analytical techniques, among which Focused Ion Beam (FIB)and Transmission Electron Microscopy (TEM). On the other hand there is also a need for correcting design errors in test devices by re-routing the interconnections with the Focused Ion Beam tool.


Halogen gasses (e.g. I2, Cl2) are typically used for modifications on devices with Al-interconnects for the selective etching of the Al-lines and they are also applied for the fast milling of the largest trenches during the preparation of TEM specimens. The challenges for FIB repair of devices with copper interconnects are discussed before [1] and it is shown that copper corrosion occurs due to exposure of Cu to Br2 in the FIB.


In this work the corrosion of Cu metallization due to focused ion beam analysis in the presence of an I2 background is discussed. The corrosion products are


analyzed by energy dispersive X-ray spectroscopy,Auger electron spectroscopy and electron diffraction in the TEM.


Experiments


The analyzed samples are damascene trenches in SiO2 with different degrees of Cu filling. The Cu is deposited by electroplating with a TaN barrier or electroless with a TiN/Ti barrier.


The FIB analysis is performed in a FEI200 system equipped with Pt, I2, XeF2 and H2O gas injectors for gas-assisted FIB. Auger electron spectroscopy is


done at 3 keV with a 0.5 µA electron beam in a PHI600 system. For energy dispersive X-ray analysis a Noran system attached to a scanning electron microscope is used. The TEM analysis is done in a high-resolution Jeol Electron Microscope 200CX.


FIB milling with I2


A most severe case of the effect of I2 on Cu metallization is illustrated in Figure 1. In this experiment 4 craters have been milled through a 1


µm thick Cu layer on a TaN/oxide stack. The craters are 500 µm apart. The first crater is made by standard cross-section milling (8×4 µm2, initially 2700 pA and finalized with 150 pA), while the second crater is milled similarly after deposition of a Pt protective layer on the surface. The third crater is smaller and


made with a lower beam current (3×3 µm2, 150 pA).


The fourth crater is milled with I2 enhanced etching with the gas needle inserted at the standard position


(~100 µm out of the field of view and ~100 µm above the surface). During the milling the pressure


rises from initially <1 10-7 mbar to ~4 10-6 mbar.


The actual pressure at the nozzle just above the surface of the sample is not known, but is surely


several orders of magnitude higher. Almost from the beginning of the milling of this crater a change of the reflectivity of the surface around the crater as well as around the 3 previously milled ones can be noticed on the low magnification optical image of the sample holder. The FIB image (Figure 2) of the area around the fourth crater shows a strong corrosion of the Cu in the whole circular spot seen optically. The corrosion product consists of a grainy material which is very bright in the FIB image, i.e. which is a conducting material. A similar corrosion of the Cu is also observed at the other three positions. The comparison of the initial cross-section (Figure 3a)and the image after the corrosion (Figure 3b) for the crater with the Pt protection layer shows a strong swelling of the layer indicating that the corrosion is not just a surface effect but extends throughout the full Cu layer. The size of the corroded spots (see Figure 1) is much larger than the area around the craters which has been imaged with the ion beam and is larger for the bigger craters (1 and 2). This indicates that the corrosion starts on the redeposited material which is expected to be present in a larger area and amount around these craters than around crater 3. This also agrees with the sharp edge of crater 4 at the side where the needle protected the surface from redeposition. The reactivity of the redeposited material will be high so that the Cu will react quickly with the I2 gas while the unscanned areas are still protected by the thin native oxide on the Cu. Once corrosion has started on the thin coverage of redeposited material around the milled structure, the native oxide loses its protective capability and within a few minutes the full Cu layer corrodes.


Figure 1 Optical microscopy image of the corrosion spots around the 4 milled craters : 1 to 3 are made without I2 (1 : 2700 and 150 pA, 2 : Pt protection and further as 1, 3 : 150 pA) and 4 is subsequently milled with I2 (150 pA). The corrosion spots form during the milling of crater 4. The approximate position of the gas nozzle is indicated.


A similar experiment is done with the crater with the I2 made with the needle not inserted. The measured pressure rise (to ~4 10-6 mbar) is similar as in the first experiment but the pressure above the surface will now be more close to the measured pressure. Around all previously milled structures corrosion is also in


this case quickly observed during the milling of the last crater with the I2. However the extent of the corrosion spot is less, and the swelling of the corrosion product near the Pt reference surface is much less, i.e. the corrosion goes less deep in the Cu layer.


Figure 2 FIB image (45º tilted) of the area around the fourth crater showing the corrosion of the surface.


The rectangular depression around the crater is due to


imaging at a higher magnification before taking


this image.


Figure 3 FIB images (45º tilted) comparing the


initial cross-section of crater 2 (a) with the same area after the corrosion (b) showing the strong swelling of the material.


FIB Milling Without Intentional I2 Introduction


The above results clearly show that the use of I2 is not acceptable for samples with Cu metallization.


The problem is however even more severe as Cu corrosion has also been observed on samples which are analyzed without the intentional use of I2. The recent history of the chamber turns out to be crucial to avoid any corrosion. After an extensive use of I2 in the system the vacuum does not quickly recover to


its best base pressure (< 1 10-7 mbar) and can remain relatively bad also during the analysis of the next samples even if this includes several vents of the chamber in between. In the worst cases the vacuum


stays for longer time in the high 10-6 mbar range and under such circumstances fast corrosion can be observed of Cu layers. An example is shown on


Figure 4a of a 3x3 µm2 crater milled with a 1000 pA Ga beam through a 1 µm Cu layer. This sample is loaded shortly after an almost full day of using I2 for device modifications on structures with standard Al metallization. The crater on Figure 4a is milled without prior imaging of the region and the image is taken with a single image grab immediately after the milling of the crater. Corrosion is observed in the


circular spot with diameter ~ 40 µm around the milled via. Figure 4b shows the same area the next morning with the sample stored in the FIB system overnight. It can be seen that the full area which is scanned with the Ga ion beam to acquire the image of Figure 4a has corroded. Moreover, in this case the corroded material has been delaminated. This is probably due to bad adhesion of the corroded material with respect to the underlying barrier/oxide so that due to charging of the corroded block during the short imaging done before acquisition of Figure 4b the whole block of corroded material jumped away. Similar delamination effects have previously also been observed due to a combination of weak adhesion and charging during FIB imaging of isolated damascene Cu trenches under "normal", i.e.


corrosion free conditions.


On thin Cu layers the corrosion effect can sometimes be noticed immediately during the cross-section imaging even if the vacuum is relatively good (low


10-6 mbar range). This is illustrated on Figure 5 for a 200 nm electrochemically deposited Cu layer that only partially fills the trenches. A protective Pt layer is deposited before the cross-sectioning in order to allow the accurate study of the layer thickness and trench filling. Already during the initial FIB image of this cross-section (Figure 5a), a degradation of the Cu layer is observed and a bright grainy material grows on top of the Pt surface. For comparison Figure 5b shows a "normal" cross-section through a similar structure taken at a later moment.


Figure 4 FIB image of the corrosion around a crater(3x3 µm2, 1000 pA) milled with an unintentional I2 background (a) and the same area after an overnight storage in the FIB chamber (b) (Image b is 45º tilted).


Figure 5 FIB cross-section images (45º tilted) of a


quickly corroded 200 nm thick electrochemically deposited Cu layer in a damascene trench structure


(a) and of the "normal" trench structure (b).


The alteration of the Cu layer continues during the


further storage of the sample in the FIB chamber


without further investigation, i.e. without interaction


with the Ga ion beam. Figure 6 compares the


morphology after the initial imaging and after a ~ 1 h(storage in the FIB chamber.


Figure 6 FIB images (45º tilted) of the initial (a) and final corrosion (b) of a partially filled Cu damascene trench structure.


Chemical Analysis


The chemical composition of the corrosion products is further analyzed by Auger electron spectroscopy(AES). The spectrum measured on the surface shows only the peaks of Cu and I (Figure 7). The O peak is expected at a position between the major I peaks and is therefore difficult to measure. However, the relative intensities of the different I peaks indicate that O can only be present in trace amounts. Also no Ga is found in the corroded material. The carbon observed in the surface spectrum is due to some absorption from the air during transport from the FIB to the AES system.


Due to the large roughness of the grainy material accurate depth profiling is not possible by Auger spectroscopy. Information on the bulk composition is obtained by energy dispersive analysis in a scanning electron microscope operated at 20 keV. The spectra show strong peaks of Cu and I, so that it can be concluded that the I measured with AES is not just a surface effect but that the whole Cu layer is converted to a Cu-I phase in agreement with the observed large swelling of the layer.


0 500 1000


d d1500 2000


H n2500


3000


3500


230


430


630


830


1030


KINETIC ENERGY (eV)CKLL


IMNN


CuLMM


CuMVV


1um


Figure 7 AES spectrum of the corroded material


shows only peaks of Cu and I, while O and Ga are absent. (The C signal is due to some absorption from the atmosphere).


TEM


The corrosion effect is also observed on specimens prepared by FIB for TEM analysis. The standard


trench milling procedure is used for the FIB preparation [2-4]. For this study damascene trench structures with a thin Cu seed layer deposited by an electroless process are used. A specimen, which is prepared with only a few hours between the last use of I2 and the loading in the FIB, is shown in Figure 8.


It can be seen that crystallites with dimensions of 50-200 nm are spread over the full transparent area of the specimen. The crystals have the highest density near the original position of the Cu seed layer, but are also present on the oxide and on the silicon substrate.


The crystals have a triangular or hexagonal shape.


Analysis by electron diffraction (Figure 9) allows to identify the crystals as cubic CuI (ZnS-structure with a = 0.60427 nm).


Although no crystals are seen on the top view FIB image taken at the end of the TEM preparation(Figure 10a), the above results on the crosssectioning of thin Cu layers indicate that the corrosion must have started immediately after the specimen preparation and is not due to the storage of the specimen in air before the TEM examination. A FIB image taken a few days later, after the TEM study, shows the crystals sticking out of the thin lamellae (Figure 10b).


The investigation of several specimens shows that the corrosion effect becomes worse for decreasing time between the last use of I2 and the loading of the specimens in the FIB chamber. Even after 24 h with 5 ventings of the system, the corrosion can still be noticed.


Figure 8 TEM image of a 0.5 µm damascene trench structure with a thin Cu seed layer deposited by an electroless process showing strong corrosion of the Cu layer.


Figure 9 The electron diffraction of the hexagonal crystal is due to the [111] zone of cubic CuI.


Discussion


The observations on the corrosion of Cu in the FIB are :


- The corrosion occurs in all areas that are even only shortly exposed to the Ga ion beam during the navigation of the stage or by fast image grabs. This indicates that even a partial removal/damage of the native oxide suffices to start the corrosion.


- Also the redeposited material can induce the corrosion.


- The corrosion is more severe for higher I2


pressures on the Cu surface, but can also occur in-situ in the FIB with the system at a relatively low pressure after extensive use of I2 for other applications. I.e., the corrosion effect is not related to moisture from exposure to the atmospheric ambient after unloading of the specimens.


- The Cu areas which are initially not attacked do not show any corrosion during at least a subsequent half year storage in air.


- Thin Cu layers, as e.g. seed layers or in thinned TEM specimens, are very sensitive and can quickly be fully destroyed


Figure 10 FIB top view image taken at the end of the TEM specimen preparation (a) and a few days later after the TEM investigation (b).


- The origin of the iodine in case that it is not intentionally introduced, must be related to desorption of iodine which is absorbed on the chamber walls during the previous use of I2 for other investigations. Also some reduction of the vacuum pump efficiency seems to occur after extensive use of I2.


- Although it is difficult to quantify, it seems that the corrosion sensitivity is higher in the period after the exchange of the I2 crucible of the gas source. This might indicate that moisture absorbed in the crucible during the exchange of the I2 crystals may play a role to increase the corrosion rate.


- The Cu or Cu-I compound diffuses over the surface.


- There is no correlation between the method of Cu deposition and the corrosion sensitivity.


The corrosion products look very similar to those reported by Herschbein et al [1] after the use of Br2 gas-assisted etching. They also found a severe damage hundreds of microns out of the field of view.


The present experiments show that this effect is related to corrosion started at the redeposited material around the field of view.


For comparison, vias have also been milled with the XeF2 gas through the 1 µm Cu layer on TaN/SiO2.


The pressure in the chamber rises in these cases to~2.3 10-6 mbar. The XeF2 has no effect on the milling rate of the Cu compared to equal milling conditions without gas assistance. The full removal of the Cu in the vias requires a considerable overmilling as the milling rate strongly depends on the grain orientation. At the borders of the milled structures the milling progresses faster due to reflection of ions on the via walls. No corrosion of the Cu on the imaged surfaces or on the via walls is observed, i.e. the XeF2 is not harmful for the Cu metallization and can hence be used without any problems for the etching of vias through oxide or nitride passivation layers during device modifications.


In order to fully avoid the corrosion problem, an interval of at least 48 h is necessary between the use of I2 and the subsequent analysis of Cu samples in the FIB.


This is particularly important for TEM specimen preparation as the remaining thin lamellae will quickly corrode. Furthermore the TEM specimens must subsequently be transported in air and are often stored for some time before the TEM analysis so that there might be a risk that any started corrosion might continue further before the TEM analysis. I2 should not be used for milling the large trenches during the FIB preparation of Cu containing specimens.


These results have also important implications for FIB device modification work and clearly indicate that I2 (and probably also all Cl or Br based gas chemistries) is not compatible with Cu metallization.


Even for wide cuts at the end of the modification work the application of I2 will be risky as any previously depassivated Cu near the vias milled for the deposition of new connections and which is not well protected by the new Pt (or W) metal track will definitely quickly corrode. Furthermore as the CuI is conductive and can migrate over the surface, even in wide cuts the corrosion product might reconnect the cut wire. The long memory effect makes the use of iodine too risky for any modification work on devices with Cu metallization.


C. Drijbooms and P. Van Marcke are acknowledged for the FIB and AES analysis. The TEM investigations are performed with the instruments at the EMAT laboratory of the University of Antwerp(RUCA).


1) S.B. Herschbein, L.S. Fischer, T.L. Kane, M.P.


Tenney and A.D. Shore, Proc. ISTFA98, 127-30(1998).


2) E.C.G. Kirk, D.A. Williams and H. Ahmed, Inst.


Phys. Conf. Ser. 100, 501-6 (1989).


3) H. Bender, P. Van Marcke, C. Drijbooms and P.


Roussel, in : Characterization and Metrology for ULSI Technology: 1998 International Conference, eds D.G. Seiler, A.C. Diebold, W.M.


Bullis, T.J. Shaffner, R. McDonald, E.J. Walters(American Institute of Physics, Woodbury)


p. 863-7 (1998).


4) H. Bender, Inst. Phys. Conf. Ser. in press (1999).


Electronic Device Failure Analysis Society, editor, p 141-143


DOI: 10.1361/cp1999istfa141


# Tin Corrosion Induced by Corrosive De-Ionized (DI) Water


Tin Corrosion Induced by Corrosive De-Ionized (DI) Water


Shekhar Khandekar, Lakshmi Vedula


Level One Communications Inc., Sacramento, California


Prof. Vinod Malshe


University Department of Chemical Technology, Matunga, Mumbai, India


Very highly purified water such as De-ionized (DI)water tends to become very corrosive once exposed


to the atmosphere. This “Hungry Water” as known in the water purification world is known to be a


major source of corrosion [1]. The DI water was responsible for corrosion of tin during autoclave(pressure cooker) testing of Integrated Circuit (IC)devices assembled in plastic Quad Flat Package(QFP) with fine pitch leads. The copper leads of these packages are plated with solder. The copper leads of the packages are plated with solder composed of Lead and Tin. Due to the effect of corrosive water, Tin from solder corroded during the autoclave testing and formed thin whiskers of solder.


These whiskers created a leakage path between the leads causing the devices to fail for pin to pin leakage.


With the increase in pin count together with reduced dimensions of the packages, the lead pitch keeps shrinking. Reliability qualification of packages with such small lead pitch has been a challenge. With such fine dimension packages, it is necessary to take care of the qualification environment so as to minimize the possibility of failures due to contaminants present in the environment. This issue becomes more critical in moisture related stress tests.


Before an IC product is released for production, it has to go through several reliability qualification tests.


Autoclave or pressure pot testing is one such test.


Autoclave test is performed to simulate the worst case conditions of a warehouse storage environment.


Fine pitch QFP packaged devices were stressed in pressure pot environment with a temperature of


121°C and atmospheric pressure of 15 psi for 168 hours (per Jedec JESD22 method A102-B). The pressure pot testing was performed after a package


preconditioning test[2]. The preconditioning consisted of devices subjected to 192 hours in 30°C/60%Relative Humidity environment (per Jedec JESD A113, Level 3 Preconditioning) followed by 3 cycles in a convection oven to mimic circuit board assembly. After the 168 hours of autoclave testing,the devices were tested on an Automated Test Equipment (ATE). Pin to pin leakage failures were observed on the ATE. Figure 1 shows the I/V curve of a leaky pin in comparison with a normal pin.


Figure 1 I/V Curves on the Failing Pins Before and After the Autoclave Test


Analysis of Results


The failing devices were inspected under optical microscope. A thin white and shiny whisker like deposition was observed between random pins on the package. The SEM image of the device leads at different levels of magnification, after 168 hours of autoclave test are shown in figures 2(a) and 2(b).


Thin whisker formation was between the failing pins


-60-40-20 0 Current (uA)20 40 60


-0.5


Voltage (V)


I/V Curve Before Autoclave I/V Curve After Autoclave


and their adjacent pins. These whiskers created a leaky path between adjacent pins. Cleaning the leads with a metallic brush could not eliminate this thin whisker like deposition. After the devices were decapsulated, the I/V characteristics of the failing pins were measured. These I/V characteristics did not show any kind of leakage between the adjacent pins.


(a) Magnification - 22X


(b) Magnification – 80X


Figure 2 SEM image of QFP device after


Autoclave testing.


Set of Experiments


The failing devices from autoclave test were baked for 24 hours. The devices were then tested on the ATE. It was observed that all the failures recovered after the bake. The devices were then re-stressed in autoclave chamber for 168 hours and no failures were observed during subsequent ATE testing.


The water used for the autoclave testing was next tested for any possible contamination. One of the tests was to check it’s pH value. The pH value of deionized (DI) water being used in autoclave chamber was measured to be at 5.3. The water fresh out of the


DI water system was measured to be at 7.0, but as the water was exposed to the atmosphere, the pH value dropped to 6.3 within few minutes. As the pH value of a substance decreases, the acidity increases.


During the autoclave testing the water was transported from the DI water system to the autoclave chamber in a container. While this water is poured into the autoclave chamber, it is exposed to the atmosphere, which causes the decline in the pH value of that water. The same experiment was repeated using distilled water and it was observed that the reduction in pH value of distilled water was not as drastic as DI water.


Results of Experiments


During autoclave testing, DI water is used to introduce humidity in the stress environment. It is usual practice to transport the water from the deionizer to the autoclave test chamber. This DI ultrahigh pure water devoid of any organic salts, in the


jargon of water treatment is termed as "Hungry Water" and is known to dissolve carbon dioxide(CO2) from the atmosphere rapidly. Carbon dioxide concentration in atmosphere is about 440 ppm.


Carbon dioxide is soluble in water containing inorganic salts. The solubility is highly pH dependent. In presence of alkalinity, solubility of carbon dioxide increases which effectively neutralizes alkalinity. A common observation in the water treatment is that the pH of treated water continuously goes down from the water source to the stress test chamber.


In ultra-high purity water, CO2 exists as free CO2.


The value of pH, CO2 partial pressure and temperature govern solubility of CO2 in water.


Corrosion is the principle effect of dissolved CO2.


Gas dissolves in water producing corrosive carbonic acid.


H2O + CO2 → H2CO3 → H++ (HCO3)−


The low pH resulting from this reaction leads to corrosion of metals. The corrosion is also enhanced by presence of oxygen (O2), which is up to 7 ppm in water. For water containing 1 ppm total alkalinity,the pH would be as low as 6.3 and concentration of CO2 in water would be about 60 ppm in ultra-high purity water; pH may be still lower resulting in higher solubility.


Tin metal from the solder on the pins is corroded by H+ ions liberating hydrogen (H2). The metal precipitates as carbonate at the site of corrosion by the following over all equation. The tin carbonate is highly conductive and thus forms the electrical path between the leads. The edges of metal are the active area and the corrosion started at sharp edges. The tin


leaching out from the pins can form a thin layer between the pins since on the QFP package, the pitch is very fine, resulting in a leakage path.


Sn + H2CO3 → SnCO3 + H2


All these failures recovered when they were baked.


The baking converted the tin carbonate into tin hydroxide, which is an insulator, hence once the devices recovered, they could not be failed. Subsequent exposure to autoclave testing formed corrosive whiskers on top of the tin hydroxide, but was not thick enough to form another leakage path.


The assumption that the DI water is ultra-pure and that it can be used for any application without any adversarial effects is not entirely true especially in pressure cooker tests. The microelectronics industry


has not been aware of the “Hungry Water”phenomenon, which is prevalent in the water purification industry. Once the water for the autoclave testing was changed from DI to regular distilled water, the incidence of corrosion dropped off completely. If DI water is to be used, caution should be taken to transport it from the DI water system to the chamber without any exposure to atmosphere.


1) Betz Handbook of Industrial Water Conditioning, 1991.


2) T. Yoshida, T. Takahashi and S. Koyama, “ A New Accelerated Test Method for Moisture Resistance of Plastic Encapsulated LSIs”, Proc.


IRPS, pp. 268-271, 1985.


Electronic Device Failure Analysis Society, editor, p 145-148


DOI: 10.1361/cp1999istfa145


# Latch-Up Induced Slit Voiding in Aluminum Metal Lines


Latch-Up Induced Slit Voiding in Aluminum Metal Lines


Chunyu Zhang, Lakshmi Vedula, Shekhar Khandekar


Latch-up induced during High Temperature Operating Life (HTOL) test of a mixed signal device fabricated with 1.0µm CMOS, double poly, double metal process caused failures due to an open in aluminum metal line. Metal lines revealed wedge voids of about 50% of the line width. Triggering of latch up mechanism during the HTOL test resulted in a several fold increase of current flowing through the ground metal line. This increase in current resulted in the growth of the wedge voids leading to failures due to open metal lines.


The trend to shrink device geometries in microelectronic integrated circuits (ICs) for low cost, high speed and high performance has brought with it a new set of metallization problems. Electromigration and thermal-stress induced stress-void formation are noticeable issues in the present generation of aluminum metallization. Wedge voids on metal lines of about 50% of the line width are not unusual due to the thermal-stress in the metal and associated dielectric layers deposition process. These voids do not pose an immediate problem during the normal operation of the device. However, in an event of electrical overstress due to latch-up condition in the devices, the current density in the metal lines is higher than in normal operating conditions. High current density accelerated the growth of the wedge voids in the metal lines resulting in the failures due to open metal lines.


As a common practice in IC industry, an IC device is typically tested in several reliability qualification tests before it is released for production. HTOL testing is one of such tests. HTOL test is performed to simulate the operation of the IC in normal


conditions. The temperature is raised to accelerate the time required to complete the testing.


The devices stressed during the HTOL tests were


fabricated with 1.0µm CMOS, double poly, double metal (with no barrier metal), non-epi process. These devices experienced a latch-up phenomenon and a ground metal line with an over 50% line-width voiding became open. The metal lines were without any barrier metal making them more susceptible for stress voiding as well as weaker against latch-up currents.


As the device was re-designed to make it more robust against latch-up and the process was re-done, the devices were observed to be able to sustain the latchup currents without metallization failures.


Failure Description


A qualification lot of 129 devices were submitted for HTOL testing at 150ºC. During the HTOL testing,the devices were powered at 5.5V and supplied with a clock signal of 512kHz. At a read point after 21.5 hours, all the devices were removed from the burn-in board and tested on an automated test equipment(ATE). Two of the 129 devices failed for transmit pulse template and were subsequently submitted for failure analysis. HTOL testing of the other 127 devices continued. There were no failures recorded during the subsequent read points of 168, 500 and 1000 hours. Another lot of 76 devices was also subjected to same HTOL testing. At a read point of 500 hours, one device failed for the same failure mode as the two devices previously detected. Bench testing verified that the devices had no signal at the Twisted Pair (TP) output pins in Transmit All Ones(TAOS) mode.


Analysis Results


The failed devices were chemically decapsulated.


Initial optical inspection of the device did not reveal any anomalies. Photoemission analysis of the devices using an emission microscope under normal operating condition did not exhibit any abnormal emission sites. The devices were then depassivated in CF4 and O2 plasma in an RIE. One of the three failed devices was then micro-probed. Micro probing of the transmit functional blocks eliminated possibility of any failure in the driver circuitry. The micro probing however revealed a floating ground line in DAC(Digital to Analog Converter) circuitry. Inspection with higher magnification microscope revealed an open metal1 ground line in all three devices. The open in the metal1 line was in shape of a slit. The optical micrographs of the slit open on two failed devices are shown in figures 1a and 1b. In comparison, the ground line in the same area on a good device is continuous, as shown in figures 2a and 2b.


The devices were then deprocessed to metal1 level using RIE dry etching. Figure 3 shows the Scanning Electron Microscope (SEM) view of the slit open in metal1 on one of the devices. The open was located at a flat section of metal1 line with no steps within a few microns of the anomaly. The exact location of the open on other failed devices varied, but it was generally in the same section of the ground line where the line had the smallest width. Inspection of entire die revealed grainy metal lines and wedge shaped notches. Further inspection of the stressed but passing devices from the same lot did not reveal opens. However wedge shaped notches in the metal lines were observed. This indicated that the wedge shaped notches were the result of high temperature stress testing.


Although statistically the number of failures was high(3 out of 205), the occurrence was random. A series of experiments were carried out to correlate the failure and the causes. These experiments were based on the experimental data that was available and data that could be made available by practical means in limited test time.


The development of the slit like void could be attributed to one or the combination of the following


two causes; one is the classical stress voiding [1, 2],the other is the electromigration (EM)[3–5]. The shape and the location (on the same ground line) of the slit open led us to believe the failure was related to or accelerated by EM. In order for EM to occur,significant amount of current must be carried by the metal line.


To measure the actual current in the ground line in the DAC circuitry under normal operating conditions,the ground metal line was cut to measure current.


The ground line was cut using Focused Ion Beam(FIB). This allowed connection of a current meter in series with the metal line. The current measurement was conducted on a good device under normal operating conditions at temperatures ranging from


25°C to 130°C. The higher temperature reading was to duplicate the temperature conditions of HTOL.


The current through the broken line on the failed devices was also measured under the same


conditions. Increasing the temperature from 25°C to 130°C slightly decreased the current through the line.


As soon as the continuity was established within the broken ground line due to the insertion of the current meter, the failed devices resumed normal functions.


The magnitude of the current was only 500 µA on both stressed but passing devices and the failed devices. This current represents significantly lower current density than is required for a metal line to fail for open due to EM. This line was designed to carry


400 µA of current in the ground line.


It has been observed that inadvertent latch-up conditions could be caused during the HTOL as well as the bench set-up testing. The latch-up was indicated by a significant jump in total current drawn by the device from the 5V power supply. These devices were fabricated on non-epi silicon wafers,which could be more susceptible to such behavior. It was also found that supplying the TP output pins with short pulses of negative voltage could induce the same behavior.


To observe the location of possible latch-up sites, the experiment was repeated while the decapsulated device was inspected with a photoemission microscope. A photoemission site was noted in the DAC circuitry during the high current phenomenon. The observed emission site in the DAC circuitry suggested that the ground might have been subjected to excessive currents during this high current phenomenon. This high current phenomenon could be due to the transients in the power supplies used to power up the burn-in boards during HTOL.


It is a well-known fact that devices fabricated with epi-silicon are more immune to latch-up phenomenon. To compare the latch-up susceptibilities of non-epi and epi devices in the actual design, the current in the ground line was also measured on same type of devices that were fabricated with epi silicon.


These devices were metallized without any barrier layer under either metal1 or metal2, which could make them more susceptible to stress migration and EM. In addition to the observations and findings on the failed devices and the stressed but passing devices, a small number of devices were also


fabricated with TiN barrier layers in the metallization. It has been known that the addition of TiN or TiW barrier layers greatly enhance the immunity to slit voiding. The barrier layers improve the stress characteristics and provide a shunt path in the event of a wedge shaped void that might create an open in the aluminum metallization. Having some devices that have the TiN barrier will enable us to compare the test results after HTOL testing on devices with and without the barrier metal.


The object of the above mentioned process experiments was to determine the role of stress voiding and latch-up. For carrying out the experiments, fabrication of engineering wafers using different process options such as wafers with and without epitaxial layers was required.


During the first set of experiments, a current meter was connected in series to the ground line with the slit void. To measure current in the same ground line of a good device, FIB was used to cut the ground line open The current as a function of operating temperature is plotted in Figure 4. The current almost decreases linearly as the device temperature is increased. This indicates that the device was not subjected to over-current in normal operating state.


The reduction in current was an indirect result of negative temperature coefficient of poly-silicon resistor network in the DAC circuitry.


The current measurement results of devices in latchup condition were compared to normal operating condition in Table 1. The devices from both the epi and non-epi process were used for the current measurement. A significant increase in the current flow in the ground line was noted when the devices were subjected to latch-up condition.


In the case of non-epi devices, the current in the line increased by 80 times, while in the epi devices, the current only increased by 28 times. This indicated that during latch-up conditions, the ground line in the DAC circuitry is subjected to higher current and that epi devices, though still susceptible to latch-up conditions, draw a lower current in the ground line.


With the mask layout and processing steps being the same, the epi devices provide an advantage of lower currents in the parasitic transistors that form the latch-up path.


Table 1 Current measurements at the ground line in the DAC circuitry at room temperature.


|Test Conditions |Non-epi, stressed |Epi |
|---|---|---|

|Normal Operation |500µA |500µA |

|Latch-up |40mA |14mA |

A sample of devices that had metallization with a TiN barrier under aluminum was subjected to 1000 hours of HTOL and the testing did not exhibit a single failure. Although inspection of the surface of the metallization did reveal similar wedge shaped voiding, it was with a much lower frequency.


Design modifications were made to the transmit circuits to make the device more robust against latchup. Experiments proved that devices with design fix for the latch-up no longer exhibit emissions sites in the DAC circuitry under repeated attempts to induce latch-up.


Further stress testing was done on the same devices that were fabricated using an epi process. Testing of these devices on a bench set-up in burn-in configuration did not reveal any failures of the metal line. In addition, some of the non-epi devices were stored in a high temperature storage environment(150oC for 168 hours) to accelerate the growth in these wedge voids. No significant increase in the size of the wedge voids was observed after the high temperature storage testing. This leads us to conclude that these failures are not the classic cases of stress voiding, electromigration or latch-up but a combination of all three effects causing the early failure of the device.


1) F. G. Yost, D. E. Amos and A. D. Romig Jr.,“Stress-Driven Diffusive voiding of Aluminum Conductor Lines”, Proc. IRPS, pp. 193-201,


1989.


2) H. Kaneko, M. Hasunuma, A. Sawabe, T.


Kawanoue, Y. Kohanawa, S. Komatsu and M.


Miyauchi, “A Newly Developed Model for Stress Induced Slit-like Voiding”, Proc. IRPS,pp. 194-199, 1990.


3) S.H. Kang, F.Y. Genin, C. Kim and J.W. Morris Jr., “Further investigations of the microstructural mechanism of electromigration failure in Al-Cu lines with quasi-bamboo microstructures”, MRS Proc., Vol. 428, pp. 255-260, 1996.


4) Y-C. Joo, S.P. Baker, M.P. Knauss and E. Arzt,“Electromigration in single-crystal aluminum lines pre-damaged by nanoindentation”, MRS Proc., Vol. 428, pp. 225-230, 1996.


5) 0S. Bauguess, L.H. Liu, M.L. Dreyer, M.


Griswold and E. Hurley, “Effects of accelerated stress conditions on electromigration failure kinetics and void morphology”, MRS Proc., Vol.


428, 93-99, 1996.


Figure 1a Optical micrograph (at 1600X) of the slit open found in the ground line in the DAC circuitry of one the failed devices.


Mag = 18.05 KX


Figure 1b Optical micrograph (at 2000X) of the slit open found in the ground line in the DAC circuitry of another failed device.


Figure 2a Optical micrograph (at 1000X) of the


ground line on a good device.


Figure 2b Optical micrograph (at 2000X) of the ground line on a good device.


Figure 3 SEM view of the slit open in the ground line at metal1 level.


Figure 4 Current through the ground line as a function of device temperature.


455 460


000


465


470


475


4800


Current (uA)485


490


495


505


100 120 140


Temperature (C)


Electronic Device Failure Analysis Society, editor, p 149-159


DOI: 10.1361/cp1999istfa149


# Failure Analysis of Discolored Bondpads in Wafer Fabrication


Failure Analysis of Discolored Bondpads in Wafer Fabrication


Younan Hua


Chartered Semiconductor Manufacturing Ltd., Singapore


Discolored bondpads & non-stick failure in 0.6 µm wafer fab process with the hot Al alloy metallization was investigated. SEM, EDX & AES techniques were used to identify the root causes. Failure analysis results showed that discolored bondpads & non-stick failure were caused by TiN residue introduced during L95 bondpad opening wafer fab process. TiN residue on bondpad might have led to non-stick bondpad issue. The results also showed that it was difficult to determine the trace amount of TiN residue on bondpad using EDX technique due to its limitations.


In this work, Auger surface analysis technique was used to determine TiN residue on bondpads with Al/TiW/Ti metallization. Auger results showed that Ti & N peaks were detected on discolored bondpads.


It has resulted in non-stick bondpad failure. The solution to eliminate TiN residue on bondpads was to increase etch time at L95 bondpad opening wafer fab process. After using the new recipe with longer etch time, Auger results on the bondpads showed that no Ti & N peaks were detected and the bond-pull testing also passed.


Aluminium bondpads on semiconductor chips play an important role in IC device reliability and yield.


Discolored bondpad problem is a major issue as during bondpad bonding at assembly house it may result in non-stick bondpad failure. Discolored bondpad problem may relate to either wafer fabrication or assembly process. Sometimes, discolored bondpad is due to assembly process. For example, in our previous paper, a case of discolored bondpads due to galvanic corrosion was studied [1]. The results showed that galvanic corrosion problem occurred in


0.8 µm wafer fab process with the cold Al alloy metallization, and it was due to DI water problem during wafer sawing at the assembly house. A lot of pinholes with a nuclear centered in the hole were formed on bondpads due to galvanic corrosion during wafer sawing, and then Si debris was dropped around the hole. Finally, the pinholes & Si debris on bondpad resulted in discolored bondpad & non-stick bondpad issue. As an interesting investigation results,this discolored bondpad failure due to galvanic corrosion is always found in the devices with the cold Al alloy metallization. However, the similar failure is never found in the devices with the hot Al alloy metallization. In our fab, there is no discolored bondpad failure due to galvanic corrosion in the devices with the hot Al alloy metallization (0.6 µm wafers), but we found another kind of discolored bondpad problem, which was not related pinhole issue or galvanic corrosion problem. In this paper, we will investigate this kind of discolored bondpad failure in 0.6 µm wafer fab process with the hot Al alloy (Al-Si, 0.8%-Cu, 0.5%) metallization.


It was reported that non-stick bondpad was found on some wafers at our customer’s assembly house. Initial optical inspection on the failed dies found the discolored bondpads. This problem may be due to either fab process or assembly process. In order to find the root cause, as such, some dies with the discolored & non-stick bondpads were subjected to failure analysis. SEM, EDX & Auger techniques were used to identify the root causes.


SEM & EDX Analysis


A strip of framelead with discolored & non-stick bondpads were randomly sampled and subjected to failure analysis. SEM & EDX analyses were carried out with 5-15 kV electron beam voltage and 10 mm working distance using Philips XL 30 FESEM (Field Emission Scanning Electron Microscope). A Lithiumdrifted silicon EDX detector is mounted at the left rear corner thus resulting in an azimuth angle of 45°.


The calibration energy scale of the spectra was performed by using Al/Cu samples at their respective Kα peaks (Al Kα line 1.486 keV & Cu Kα


8.040 keV) with 5000 counts. To achieve accurate EDX results, ZAF standardless EDX quantification method [4] was used:


Wiw = (ZAF) i Ki


Where Wiw is weight fraction of element i analyzed without coating correction; Z, atomic number correction factor; A, absorption correction factor; F,fluorescence correction factor and Ki, intensity ratio of Ii(UNK)/Ii(STD) of element i.


As normal failure analysis, sample is coated with Au or Pt. Therefore, Wiw is not to be real values due to coating effect. In order to achieve more accurate results, EDX data have to be performed coating correction. The formula used is as follows:


-


(100 100


w'


Where Wiw' is weight fraction of element i analyzed with coating correction. Wiw is weight fraction of element j introduced by coating process or sample preparation. Quantified EDX results can be expressed as both weight fraction and atomic fraction. The atomic fraction (Wia') can be calculated from the weight fraction (Wiw') using (3):


/A


(W


a'


Where Wia' is atomic fraction of element i analyzed with coating correction. Wiw' & Wjw' are weight fraction of element i & j analyzed with coating correction, and Ai & Aj are atomic weight of elements i & j.


AES Analysis


In wafer fab, Auger electron spectroscopy (AES) has been widely used for failure analysis. It is a commonly used surface analytical technique due to the fact that the kinetic energy of Auger electrons for all elements (except H and He) cam be less than 2000 eV and the escape depth of electrons within this energy range is limited to approximately the top 5 nm of the sample surface. Moreover, it has the particular advantage of being easily applicable to the light elements such as C, N, O, F, etc. In this study, Auger electron spectroscopy (AES) was used to determine TiN residue on the discolored bondpads. Depth profiling was carried out using a VG ESCALAB 220i-XL XPS/AES machine. The conditions used are:operating vacuum at 3 x 10-9 mBar, electron gun beam energy at 3 keV & ion gun beam energy at 4 keV. Measurements were made at the as-received surface of each bondpad, and following argon ion etching to depths of 50 Å, 100 Å & 150 Å. These etch depths are equivalent argon ion sputter depths using a Ta2O5 standard. The relative atomic concentrations(at%) were derived from the Auger survey spectra.


The values were calculated by first measuring elemental peak-to-peak heights in the survey scans and then applying sensitivity factors based on standard spectra of pure elements or selected compounds [2]:


(I


std


i =


Where Ii is the peak-to-peak amplitude of the element i from the test specimen, Istd is the peak-to-peak amplitude of the element i from the standard, Si is the relative sensitivity factor and Di is a relative scale factor between the spectra for the test specimen and standard.


Results & Discussions


Optical & SEM Results


Optical inspection found that there were 4 kinds of dies on the strip of framelead which were good die with all bonded pads (Figure 1), bad die with only one non-stick pad (Figure 2), bad die with all non-stick pads (Figure 3) and bad die with all discolored pads(Figure 4). Moreover, discoloration of bondpads can find under optical using low magnification (Figure 5,left) & high magnification (Figure 5, right).


In order to understand the details, SEM analysis was subjected to the bad die with all discolored bondpads.


The results showed that the grain size at the center of bondpads was smaller than that at the edge of the bondpads (Figures 6-7). Close-up SEM views are shown in Figure 8 for the edge area of the bondpad in which the grain size was bigger & Figure 9 for the center area of the bondpad in which the grain size was smaller. Similar results are seen on the other dies.


From the SEM results, we understood that the difference of the grain size on bondpads has resulted in discolored bondpads optically.


EDX Analysis Results


EDX results on the discolored bondpad showed no abnormal element was detected using 5 kV beam acceleration voltage (Figure 10). However, based on this EDX result, we still cannot confirm whether there is TiN residue on bondpad or not. The reasons are:(a). Although N Kα peak can be excited using 5 kV beam voltage energy, it may not be detected by EDX due to lower sensitivity of N element to EDX detection; (b). The amount of TiN residue is too few to be detected by EDX due to lower limit of detection of EDX for N element; (c). Ti Kα peak cannot be excited using 5 kV beam accelerating voltage.


Therefore, in order to determine TiN residue on bondpad by detecting Ti Kα peak, high kV beam acceleration voltage should be used.


We can theoretically estimate the beam voltage used.


From the EDX theory, the critical excitation energy of Ti Kα is 4.965 keV and that corresponds to a critical wavelength:


398.


E=


hc


v c


Where λ is in Å and E is in keV. In this case, the critical excitation wavelength of the K shell of Ti Kα line is 2.497 Å. This means that the excitation wavelength from excitation source must be shorter than 2.497 Å.


On other hand, we can obtain the short wavelength limit of an excitation source. According to DuaneHune relation:


eV


hv


This expression signifies that the energy of any electromagnetic radiation in the emission spectrum can never be higher than the kinetic energy of the electrons. Equation (6) is more conveniently written:


12.398


(7)


Where λ0 is in Å and V0 is in kV. Using Equation (7),we can estimate the short wavelength limit of excitation source or voltages used for a characteristic x-ray line analyzed.


However, the actual voltage used in EDX should be


1.5 2.0 times of the theoretical values. In general,therefore, the beam voltage used practically is as much as 1.5-2.0 times of the critical excitation energy. For convenience, if we use the energy of the characterization x-ray line to replace 12.398/λ0 in Equation (7), then we can obtain a estimation formula:


Vi = k Ei


Where the value of k is 1.5-2.0, E i in keV and Vi is in kV. Using Equation (8), we can quickly estimate the actual beam voltage used for a characteristic x-ray line interested. For example, in this case, if we use ETi is 4.510 keV (Ti Kα), the actual voltage used(VTi) is about 9 kV (k = 2) or above. We have done some experiments on a bondpad using different voltage from 5 kV to 20 kV to detect Ti Kα peak. The results are listed in Table 1. From the data listed in Table 1, we can see that Ti Kα peak was not detected using the voltage below 10 kV beam voltage.


However, Ti Kα peak was detected using 10 kV &above (in Table 1, Kα line was detected for Al & Ti and Mα line was detected for W).


From the above discussion, we understand that to determine TiN residue by detect Ti Kα, the beam acceleration voltage of 10 kV or the above should be used. However, another problem raised is that the electron penetration will be about 1 µm (Al) using 10 kV & 2 µm (Al) using 15 kV as shown in Table 2 which describes the penetration depths for these electrons as the approximate penetration depth for xrays (some possible elements in wafer fab).


As results, the signal from underneath TiW barrier metal layer will be also detected. This will result in confusion in identification of Ti peak. It is unable to identify whether Ti peak is from surface TiN ARC residue or from underneath TiW barrier metal layer.


For example, EDX results detected on a bondpad with Al/TiW/Ti metallization are shown in Figure 11(10 kV) & Figure 12 (15 kV). However, we cannot determine that the Ti Kα peak in Figures 11-12 is from surface TiN residue or underneath TiW barrier metal layer. As such, we think that it is impossible to


identify TiN residue on bondpad using EDX technique and suggest using Auger surface analysis technique to determine TiN residue on bondpad with Al/TiW/Ti metallization.


Table 1 EDX results (wt%) detected on the bondpad by using different beam accelerating voltage from 5 kV to 20 kV


Table 2 Electron penetration (in microns) vs beam accelerating voltage


|Z |Ele. |10 kV |15 kV |20 kV |25kV |30kV |
|---|---|---|---|---|---|---|

|13 |Al |1.0 |2.0 |3.4 |4.9 |6.7 |

|14 |Si |1.2 |2.2 |3.7 |5.5 |7.5 |

|22 |Ti |0.6 |1.2 |2.0 |2.9 |4.0 |

|29 |Cu |0.3 |0.6 |1.0 |1.5 |2.0 |

|74 |W |0.1 |0.3 |0.5 |0.7 |0.9 |

|79 |Pt |0.1 |0.3 |0.5 |0.8 |0.9 |

Auger Results


In this case, Auger analysis was used to determine TiN residue on discolored bondpads & non-stick bondpads. Auger depth profiling was made at the asreceived surface of each bondpad, and following argon ion etching to depths of 50 Å, 100 Å & 150 Å of the bad die. Auger results showed that Ti & N peaks were detected on a discolored bondpad of the bad die & a spectrum of the as-received surface is shown in Figure 13. XPS analysis confirmed the presence of Ti & N (Figure 14). The relative atomic concentrations (at%) derived from the Auger spectra are shown in Table 3 (S1). To check whether the other wafers are affected or not, the similar Auger depth profiling analysis was subjected on the two wafers. The results showed that Ti & N were detected on a wafer with discolored bondpads (Table 3, S2).


However, no Ti & N peaks were detected on another wafer without discolored bondpads (Table 3, S3).


Auger results showed that Ti & N peaks were also detected on another two wafers from OQA (Table 3,


S4) & in-line (Table 3, S5). Based on the Auger results, we suspected that TiN residue had resulted in discolored & non-stick bondpads.


Root Causes, Solution & Preventive Actions


Root Causes


|Z |5 kV |6 |7 kV |8 kV |9 kV |10 kV |11 kV |12 kV |
|---|---|---|---|---|---|---|---|---|

|Z |5 kV |kV |7 kV |8 kV |9 kV |10 kV |11 kV |12 kV |

|Al |100 |100 |100 |100 |100 |98.5 |96.6 |94.2 |

|Ti |0.0 |0.0 |0.0 |0.0 |0.0 |1.5 |3.4 |5.8 |

|W |0.0 |0.0 |0.0 |0.0 |0.0 |0.0 |0.0 |0.0 |

|Z |13 kV |14 kV |15 kV |16 kV |17 kV |8 |9 |20 kV |

|Z |13 kV |14 kV |15 kV |16 kV |17 kV |V |V |20 kV |

|Al |90.3 |85.3 |80.6 |77.3 |75.0 |70.1 |66.7 |63.7 |

|Ti |7.6 |9.0 |9.4 |9.6 |9.8 |10.0 |9.8 |9.6 |

|W |2.1 |5.7 |10.0 |13.1 |15.2 |20.0 |23.5 |26.7 |

After performing more fab & FA investigations, it is concluded that discolored bondpad & non-stick bondpad issue were due to TiN (ARC layer) residue on bondpads. The possible root causes might be: (a).


Thickness of passivation layer was higher than normal value; (b). Thickness of TiN ARC layer was higher than normal value and (c). TiN ARC layer was under-etched during L95 bondpad opening fab process.


Cross sectional SEM on passivation & Auger depth profiling on ARC layer were done & results confirmed that thickness of passivation & TiN ARC layer was in the normal value (about 350 Å). As such,we strongly think that the above (a) & (b) may not be the root cause & it might be (c) TiN ARC layer under-etched. In order to confirm this suspicion, a wafer from the same Lot with S3 was performed reetched using the old recipe at L95 bondpad opening,and then, it was subjected to Auger analysis. The result shows no Ti & N peaks were detected (Table 3,S6). Comparing the results of S6 to S4, we concluded that that the TiN residue was due to under-etched.


Solution


After performing some experiments, we believe that TiN ARC layer under-etched problem was due to L95 bondpad opening etch recipe sensitivity to RT%(Recticle Transmission). The throughout rate study &window check results showed that high RT%contributed to TiN residue on bondpad problem,while low RT% didn’t have this problem. The results also showed that with longer L95 etch time setting,the TiN residue was totally etched. In other word,shorter L95 etch time setting in the previous recipe caused ARC layer under-etched & TiN residue on bondpads. Therefore, the solution to eliminate TiN residue on bondpads is to increase TiN ARC layer etch time in new etch recipe of the bondpad opening.


After performing more experiments, the suggestion is to change the dielectric etch time from 60 sec(passivation nitride etch step)/65 sec (passivation oxide etch step)/30 sec (TiN ARC etch step) to 65 sec(passivation nitride etch step)/70 sec (passivation oxide etch step)/70 sec (TiN ARC etch step). After increasing the etch time, the problem of TiN residue


on bondpads was eliminated. Comparing results are shown in Figure 15 & Table 3. From Auger results,we can see that Ti & N peaks were detected on bondpads using the old etch recipe, but no Ti & N were detected on bondpads after using the new recipe(Table 3, S7).


Preventive Actions


Except for controlling strictly the thickness of passivation & TiN ARC layer and using the new etch recipe for L95 bondpad opening, we also implemented a weekly Auger monitoring action. One wafer is randomly pulled from the production line & sent to do Auger analysis every week to ensure the good quality of bondpads. The monitoring results from the first 3 months are listed in Table 4. The results showed that after using the new etch recipe, no TiN residue was detected on bondpad again as the concentrations of Ti & N detected on surface of bondpads were 0.0 at% or less than the lower detection limit of Auger analysis. Moreover, we also sent some wafers to do bond pull & ball shear testing


at the assembly house. The results showed that the total number of WPT failures & peeling was zero.


Summary & Conclusion


In this paper, discolored bondpads & non-stick failure in 0.6 µm wafer fab process with hot Al alloy metallization was investigated. Fab investigation &FA results showed that discolored bondpads & nonstick failure were caused by TiN residue on bondpads introduced during L95 bondpad opening fab process.


The TiN ARC layer under-etched problem was due to etch recipe sensitivity to RT. The solution to eliminate TiN residue on bondpads was to increase etch time from 30 sec to 70 sec at the TiN ARC layer etch step. After using the new recipe with longer etch time, Auger results on bondpads showed that no Ti &N peaks were detected and the bond-pull testing also passed. Moreover, after discussion, we concluded that it is impossible to determine the trace amount of TiN residue on bondpads by detection of Ti peak using EDX technique. Auger surface analysis technique is recommended to determine TiN residue on Al/TiW/Ti metallization bondpads.


Table 3 Relative Atomic Concentration (at%) from Auger Survey Spectra


|Sample No. |Etch |C |N |Ti |O |F |Al |
|---|---|---|---|---|---|---|---|

|Sample No. |Depth |||||||

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |0 |10.2 |14.6 |11.7 |63.5 |0.0 |0.0 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |50 |6.3 |39.4 |19.7 |34.6 |0.0 |0.0 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |100 |0.0 |24.2 |9.2 |12.2 |0.0 |54.5 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |150 |0.0 |3.5 |2.5 |16.7 |0.0 |77.3 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |0 |6.4 |9.3 |7.6 |42.6 |0.0 |34.2 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |50 |2.6 |26.2 |12.8 |21.5 |0.0 |37.0 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |100 |2.2 |14.8 |6.5 |13.9 |0.0 |62.6 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |150 |1.3 |3.3 |2.5 |15.7 |0.0 |77.2 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |0 |4.4 |0.0 |0.0 |26.9 |4.6 |64.1 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |50 |0.0 |0.0 |0.0 |9.4 |0.0 |90.6 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |100 |0.0 |0.0 |0.0 |8.9 |0.0 |91.1 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |150 |0.0 |0.0 |0.0 |1.4 |0.0 |98.6 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |0 |10.3 |8.8 |6.5 |40.0 |0.0 |34.4 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |50 |0.0 |27.1 |14.5 |29.5 |0.0 |29.0 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |100 |0.0 |32.0 |12.7 |13.3 |0.0 |41.9 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |150 |0.0 |7.1 |2.8 |13.1 |0.0 |77.0 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |0 |3.0 |15.2 |10.5 |56.8 |1.3 |13.2 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |50 |0.0 |29.9 |18.0 |19.8 |0.0 |32.3 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |100 |0.0 |23.7 |12.0 |5.8 |0.0 |58.4 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |150 |0.0 |14.3 |8.4 |4.4 |0.0 |72.9 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |0 |0.0 |0.0 |0.0 |25.8 |6.18 |68.02 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |50 |0.0 |0.0 |0.0 |5.0 |0.0 |95.0 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |100 |0.0 |0.0 |0.0 |2.6 |0.0 |97.4 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |0 |3.5 |0.0 |0.0 |26.0 |5.4 |65.2 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |50 |0.0 |0.0 |0.0 |7.4 |0.0 |92.6 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |100 |0.0 |0.0 |0.0 |5.2 |0.0 |94.8 |

|S1 A die with Discolored Bondpads S2 A wafer with Discolored Bondpads S3 A wafer without Discolored Bondpads S4 A wafer (OQA) With discolored Bondpads S5 A wafer (in-line) With discolored Bondpads S6 A wafer after Re-etch using The old recipe S7 A wafer after Etch using The new recipe |150 |0.0 |0.0 |0.0 |2.5 |0.0 |97.5 |

Note: The quantification figures are based on the sensitivity factors experimentally or obtained from Handbook of Auger Electron Spectroscopy (2nd Edition, Physical Electronic Inc., USA,1976) and are subjected to be about 20% error.


Table 4 Weekly Auger monitoring results on surface of bondpads (the first 3 months after using the new etch recipe) (as received at%)


|Sample |C |Si |N |Ti |O |F |Al |
|---|---|---|---|---|---|---|---|

|1 |3.6 |0.0 |0.0 |0.0 |44.0 |7.0 |45.4 |

|2 |3.8 |0.0 |0.0 |0.0 |33.7 |4.2 |58.3 |

|3 |3.4 |0.0 |0.0 |0.0 |34.4 |5.1 |57.1 |

|4 |1.1 |0.0 |0.0 |0.0 |35.1 |5.9 |57.1 |

|5 |0.0 |0.0 |0.0 |0.0 |37.4 |3.9 |58.7 |

|6 |2.1 |0.0 |0.0 |0.0 |33.3 |9.4 |55.2 |

|7 |0.0 |0.0 |0.0 |0.0 |35.6 |7.6 |56.8 |

|8 |6.1 |0.0 |0.0 |0.0 |27.2 |5.8 |61.0 |

|9 |4.5 |0.0 |0.0 |0.0 |35.1 |5.0 |54.1 |

|10 |1.2 |0.0 |0.0 |0.0 |29.8 |4.9 |62.8 |

|11 |3.4 |0.0 |0.0 |0.0 |31.4 |6.0 |57.7 |

|12 |2.8 |0.0 |0.0 |0.0 |33.7 |5.5 |58.1 |

|13 |2.3 |0.0 |0.0 |0.0 |30.3 |12.6 |54.8 |

|14 |2.6 |0.0 |0.0 |0.0 |34.4 |6.3 |56.8 |

|15 |2.0 |0.0 |0.0 |0.0 |35.9 |8.2 |54.0 |

|Ave (at%) |2.6 |0.0 |0.0 |0.0 |34.1 |6.5 |56.5 |

The author would like to thank Dr Lau Chi-Kwan& Shailesh Redkar (QRA, CSM), Low E. C. &Chuah Alex (Etch, CSM) and Mo Z. Q. (PSB,Singapore) for their technical advice.


1) Younan Hua, “A Study on Discolored Bondpads and Galvanic Corrosion”, the proceedings from the 24th International Symposium for Testing &Failure Analysis, p269-272, 15-19 November 1998, Dallas, Texas, USA (1998).


2) Simon Thomas & Howard M. Berg, “Microcorrosion of Al-Cu Bonding Pads,” p153-158,IEEE/IRPS (1985).


3) R. K. Lowry and J. H. Linn on the 18th International Symposium for Testing & Failure Analysis, Los Angeles, California, USA/17-23 October, p165 (1992)


4) Younan Hua, Z. R. Guo and K. W. Chau,“Studies of ZAF Standardless EDX Quantification Method and Application in Failure Analysis of Semiconductor,” Journal of Trace and Microprobe Techniques, 15 (1), p13-31(1997).


Figure 1 Optical photo shows that all bondpads were bonded on the good die.


Figure 2 Optical photo shows that there was a nonstick bondpad on the bad die as shown by the arrow.


Figure 3 Optical photo shows that all bondpads were non-stick pads on the bad die.


Figure 4 Optical inspection found all bondpads were discolored bondpads on a bad die.


Figure 7 SEM micrograph shows that the grain size at the center of bondpads was smaller that that at the edge of the bondpads.


Figure 5 Optical photo shows that discoloration of bondpads can find under optical using low


magnification, (left) & high magnification.


Figure 8 Close-up SEM view shows that the grain size was bigger at the edge of bondpad.


Figure 6 SEM micrograph shows that the grain size at the center of bondpads was different from that at the edge of the bondpads.


Figure 9 SEM view shows that the grain size was


smaller at the center of bondpad. The smaller grain size has resulted in discoloration optically.


Figure 10 EDX (5 kV) results on discolored area of bondpad shows that no abnormal element was detected.


Figure 11 EDX (10 kV) results show that except for Al peak, Ti Kα peak was also detected on the discolored bondpad. However, it is difficult to identify Ti Kα peak was from surface TiN residue or underneath TiW barrier metal layer.


Figure 12 EDX (15 kV) results shows that except for Al peak, W Ma and Ti Kα peaks were detected on the


discolored bondpad, which were from the underneath TiW barrier metal layer.


Figure 13 Auger spectrum shows that Ti & N peaks were detected on the discolored bondpad


Figure 14 XPS Analysis confirmed that the presence of Ti & N on discolored bondpad


Figure 15 After using the new etch recipe at L95 fab process, no Ti & N peaks were detected by Auger analysis


Electronic Device Failure Analysis Society, editor, p 161-169


DOI: 10.1361/cp1999istfa161


Proceeding from the 25th International Symposium for Testing and Failure Analysis, 14-18 November, 1999, Santa Clara, California


# Optimizing Contact Resistance at a Resistor/Conductor Interface via Thin Film Microanalysis and Process Design of Experiments


Optimizing Contact Resistance at a Resistor/Conductor Interface via Thin Film Microanalysis and Process Design of Experiments


J.H. Linn, T.K. Thompson, M.G. Shlepr


Harris Semiconductor, Palm Bay, Florida


Electrical data from chromium-silicon-carbon (CrSiC)thin film resistors (tfr) consistently showed highly variable contact resistance (Rc) to the aluminum (Al)interconnect. Transmission electron microscopy data from CrSiC/Al interfaces exhibiting high Rc showed a conformal, amorphous layer sandwiched between the tfr and Al. Auger data from the tfr/Al interface showed this ‘crud’ layer to contain increased C, S, and SiOx. Auger data from CrSiC films on test wafers exposed to the process steps before Al deposition showed additional growth of the ‘crud’ layer after each photoresist (PR) operation. In addition, Rc variability was reduced on product wafers from split lots when 2x the normal PR strip time was used compared to the normal strip time. A Designed Experiment (DOE) to examine improving the removal of this ‘crud’ layer was run on product lots utilizing two factors: the standard strip and a two-step strip. Electrical results for both Rc and die yield were significantly improved using the two-step process. The variability of the Rc was also reduced.


Good electrical contact between thin film resistors (tfr)and the aluminum (Al) interconnect used to electrically contact the tfr terminations is essential for optimum integrated circuit (IC) performance.


Contamination at the tfr/Al interface can lead to electrically open resistors, resistive interfaces that increase contact resistance (Rc), or corrosion of the tfr and Al. Electrically open resistors oftentimes cause the IC to completely fail. Contact resistance can increase the effective series resistance in the circuit.


This will often cause electrical parameters like the IC output voltage to be shifted from nominal values.


Internal matching feedback loops utilizing the tfr can also be shifted, oftentimes affecting the device stability. Corrosion of the tfr or Al can increase series resistance over the life of the device, resulting in shifted device parameters leading to premature failure of the IC [1].


Figure 1 Contact resistance between the CrSiC tfr and the Al from several product wafer test structures. Note


the tail above the upper specification limit of 200.


Electrical data from an IC process utilizing chromiumsilicon-carbon (CrSiC) tfr showed highly variable Rc to the Al termination. The Rc typically varied from nominal to greater than 2.5 times nominal (Figure 1).


It was observed that electrical parameters like resistor match were also shifted from nominal values. This was believed to be due to the Rc variability. This paper will present analytical data from both nominal and shifted tfr/Al interfaces. This data was used to identify


the root cause of the elevated Rc. This paper will also present the results of a Designed Experiment (DOE)that identified the optimal processing parameters which minimized the Rc and Rc variability.


Material and Methods


Electrical Testing


Five test structures were measured per wafer to identify wafers with nominal and high Rc. The test structure design (Figure 2) allows the measurement of four-terminal resistance by forcing a specified current and measuring the resulting voltage. It is designed to minimize the sensitivity of the Rc measurement due to alignment variations. This structure works by placing two contacts in parallel such that a misalignment increases the Rc of one contact while decreasing the Rc of the other. Therefore, the total resistance of the two contacts is maintained.


Figure 2 Electrical test structure used to measure Rc on product wafers. Current is forced between points A and B and a voltage drop is measured between points C and D.


Transmission Electron Microscopy


TEM was used to characterize the microstructure of the tfr and the contact between the tfr and Al alloy at the Al termination. The Rc of the test structures from fully processed wafers were measured. Vertical sections of test structures with high, mid-range, and low Rc values were prepared for TEM by Focused Ion Beam (FIB) milling. All FIB sections were of sufficient length to examine the entire resistor length including both leading edges of the tfr/Al termination.


Brightfield images were recorded from several locations along the length of the resistor and Energy


Dispersive Spectroscopy (EDS) was used to identify elemental composition of selected structures.


Scanning Auger Spectroscopy


SAM was used to investigate the composition of the material at the tfr/Al termination. The Rc of test devices from fully processed wafers was measured.


Interfaces which had high and low Rc were investigated by stripping the Al interconnect with HCl and analyzing the surface of the CrSiC tfr. Tfr sheet films were also prepared and exposed to all aspects of the processing prior to Al deposition. Wafers were sampled at each unit process for analysis to determine which operations were altering the surface of the tfr.


Auger surveys were collected at 3 KeV in a large area raster to help reduce surface desorption.


Designed Experiment


Two lots were split between two solvent strip treatments. Treatment 1 was our standard strip process utilizing a Semitool single chemical spray processor.


Treatment 2 was a dual strip process using a Semitool dual chemical spray processor. The standard strip process consisted of a spray of EKC 805 at 85oC for 6 minutes followed by a 5 minute spin/ rinse/dry. The dual strip process consisted of a 7 minute spray of EKC 830 at 85oC followed by a 15 minute spray of EKC 311 at 65oC with a 5 min spin/rinse/dry.


The use of FIB allowed preparation of clean, vertical TEM sections through devices with measured Rc values. This allowed direct microstructural comparisons of the tfr and tfr/Al terminations on devices with a range of known Rc values. This was the optimal situation for relating observed structural differences to measured functional properties. The use of FIB also produced fewer sample preparation artifacts than standard grinding and polishing techniques which, for soft materials such as aluminum,tend to capture polishing debris.


The structure and thickness of the tfr was similar for all three devices examined here. The tfr appeared as an 7-8 nm dark band when imaged along the sample surface plane. No additional layers were visible and the tfr retained an uniform intensity during sample tilt studies. Thus, the vertical structure of the tfr appeared to be a single homogeneous layer that was 7-8 nm thick. EDS data from analysis points (40 nm diameter) on the resistor showed a distinct chromium


peak. It was concluded that the structure of the tfr did not account for the differences in the observed Rc range.


However, the structure of the tfr/Al termination differed considerably between the three devices(Figure 3). In addition to the above described tfr layer,both the high and mid-range Rc devices had an addition layer present between the tfr and Al alloy.


This additional layer appeared to be amorphous as it did not change contrast during sample tilting and was about twice as thick on the high Rc device (Figure 3A)than on the mid-range device (Figure 3B).


Examination of the leading edges of the Al terminations showed that this unknown layer appeared not to extend beyond the edge of the aluminum.


Again, a clear chromium signal was obtained by EDS from analysis points on the tfr for both the high and mid-range devices.


This unknown layer was not present at the tfr/Al terminations of the low Rc device. Furthermore, the structure of the low Rc tfr under the aluminum appeared altered having acquired a mottled appearance(Figure 3C) that extended to the leading edges of the aluminum. The distribution of this modified structure suggested a reaction between the aluminum and tfr.


No definitive chromium signal could be obtained from the tfr/Al termination on this device. The diffusion of chromium into the aluminum and its subsequent dispersion below EDS detection limits could account for this lack of chromium signal.


It was concluded that the amorphous ‘crud’ layer was responsible for the Rc between the tfr and aluminum interconnect. This ‘crud’ layer resulted in a graded functional response, being twice as thick on high Rc devices as mid-range devices, and blocked the alloying of the tfr and aluminum that occurred on the low Rc device. A more detailed examination of the composition of the ‘crud’ was necessary to understand how and when it formed.


SAM


Auger data from the surface of the tfr under the Al showed that this ‘crud’ layer contained increased levels of carbon (C), sulfur (S) and silicon oxide(SiOx). To better characterize the formation of this‘crud’ layer, sheet tfr films were processed through the photoresist (PR) operations for tfr patterning and first and second aperture etch. These operations occurred prior to Al interconnect deposition. Figure 4 shows the Auger spectrum of the as-deposited tfr. Figure 5 shows the tfr surface after the first PR operation - tfr patterning. Tfr patterning involves PR deposition,


exposure, develop, tfr etch in the open PR areas with a wet etch solution, and PR solvent strip. Note the increased C signal and a slight broadening of the SiOx/Si peak after this process. It appears that the growth of the ‘crud’ layer has begun.


The Auger data from the tfr surface after the first and second PR operation - first aperture etch - is shown in Figure 6. First aps etch involves PR deposition,aperture pattern exposure, develop, a wet oxide etchant to etch the apertures and a PR solvent strip. Clearly a marked increase in the C is noted. S is also noted and is most likely from an interaction of the tfr surface and the PR solvent strip. The PR solvent strips employed in these operations have demonstrated detectable quantities of S based compounds.


Auger data from the tfr surface after the first, second and third PR operation - second aperture etch - shows slightly less C than the tfr surface after first aps etch(Figure 7). Second aps etch is an analogous operation to the first aps etch described above. However, the C is still considerably higher than observed on the asdeposited tfr film. We believe this demonstrates the typical wafer-to-wafer variability of the ‘crud’ layer formation.


Auger depth profile data (Figures 8a and 8b) show a definite increase in the thickness of the ‘crud’ layer after the PR operations. These data also suggest that the crud layer has an oxide component to it as the oxygen (O) profile follows the profile of the C within the ‘crud’ layer. We believe the O is associated with an increase in SiOx formation on the surface of the tfr.


To test this hypothesis, wafers processed through all three of the PR operations were exposed to a 1x, 2x and 4x the nominal 40:1 (water:hydrofluoric acid) HF dip used prior to Al deposition. The dip is used to help reduce the native SiOx thickness and, thus, improve the tfr/Al contact. Auger survey data from these three tfr surfaces are shown in Figure 9. These data indicate that the longer the 40:1 exposure, the more the C and O signals decrease. Therefore, the ‘crud’ layer is thinned by the 40:1 etch. Since this etch targets oxides of silicon, not organic based films, the film must have an ‘organo-silicon oxide’ composition.


These data clearly show that the exposure of the tfr film to the PR and PR solvent strip results in the growth of a C, S, and SiOx containing ‘crud’ layer.


The presence of S incorporated into this ‘crud’ layer further suggests that the layer is most influenced by the solvent strip chemistry. In addition, the PR and


Figure 3 Structure of Thin Film Resistor/Aluminum Termination. Typical microstructure


extending over the tfr/Al termination for devices with (A) high (B) mid-range and (C) low Rc.


Magnification is equal for all three images and the scale bar is given in (C). VTEM; B = [011]Si,Brightfield. ppt., precipitate; Rc, contact resistance; rx., reacted; Unk., Unknown.


Figure 4 Auger data from the surface of the as-deposited CrSiC film.


Figure 5 Auger data from the surface of the CrSiC film after the tfr patterning.


Figure 6 Auger data from the surface of the CrSiC film after the tfr patterning and after the first


aperture etch.


Figure 7 Auger data from the surface of the CrSiC film after the tfr patterning, the first aperture etch, and the second aperture etch.


Figure 8 Auger profile data from CrSiC films after (a) deposition and (b) the first two photoresist


operations.


Figure 9 Auger data from the surface of the CrSiC after tfr patterning, first and second aps etch,


and a (a) 10 s, (b) 20 s and (c) 40 s 40:1 HF dip.


solvent strip exposures increase the growth of SiOx on the tfr surface. This ‘crud’ layer can effectively interfere with the tfr/Al termination contact formation,resulting in increased Rc. The data also indicates that there is a wafer to wafer variability in the growth of the ‘crud’ layer. These analytical data suggested a need for an organo-silicate strip chemistry to reduce the Rc variability.


DOE Results


In-line electrical test results indicated a significant reduction in Rc was achieved when using the dual strip process (EKC 830/311). Wafer probe results also show the dual strip process gives significantly higher die yield. The key component of the dual strip process is the EKC 311 Post Etch Residue Remover. This cleaning solution is a hydroxylamine (HDA) based chemistry which has been proven to effectively remove positive photoresist, sidewall polymers, and etching residues from oxide, metal, and polysilicon etch processes [2]. The increased yield is believed to be the result of EKC 311 removing the ‘crud’ layer and, therefore, providing an improved and more consistent ohmic contact to the tfr. The pre-dual strip data showed a much wider distribution (Figure 1)when compared to the current data with the new process (Figure 10).


• Highly variable Rc values were noted on an IC process that was experiencing reduced yield.


Many of the yield-reducing parameters could be directly related to this variable Rc.


• TEM sections of test structures with elevated Rc values showed a ‘crud’ layer between the tfr and Al termination. The thickness of the ‘crud’showed a direct relation to the measured Rc.


• SAM analysis of the tfr showed the ‘crud’ to be a sulfur containing silicone that grew during photoresist processing. As indicated by thickness,the growth of this ‘crud’ was variable.


• A two-step process that stripped the ‘crud’ layer from the tfr surface before Al deposition was tested. This modified process reduced Rc variability and significantly increased yield.


1) L. Bos, IEEE Trans. Comp. Pack. Manuf. Tech.


Pt. A, 17, 359-65 (1994)


2) Wai Mun Lee, "A Proven Sub-Micron Photoresist Stripper Solution For Post Metal And Via Hole Processes," EKC Technology, Inc (1996).


Figure 10 Contact resistance between the CrSiC tfr and the Al from several product wafer lots after


implementation of the new strip process.


Electronic Device Failure Analysis Society, editor, p 173-181


DOI: 10.1361/cp1999istfa173


# Failure Analysis of Plastic Packaged GaAs and AlGaAs/GaAs LEDs


Failure Analysis of Plastic Packaged GaAs and AlGaAs/GaAs LEDs


Patricia F. Mead, Melody Burch, Patrick McCluskey


CALCE - Electronic Products Systems Center


F. G. Johnson


Laboratory for Physical Sciences, University of Maryland, College Park, Maryland


Failure and degradation mechanisms of plastic packaged LEDs that have been subjected to high levels of moisture, current bias, and elevated temperature conditions have been investigated and analyzed. The investigation included electrical characterization and a variety of failure analysis techniques including photoluminescence (PL),electroluminescence (EL), cathodoluminescence(CL), and environmental scanning electron microscopy (ESEM). Our results highlight the usefulness of simple screening techniques to monitor the quality of newly manufactured LED packages.


Our results also indicate that for AlGaAs structures,degradation of the light output and electrical performance involves a complex interaction between temperature, relative humidity at the LED surface and voltage bias.


In recent years, there has been an increase in the use of LEDs as optical sources in a variety of applications. LEDs are commonly seen in computers and radios as indicators, but they also have more unique uses. For example, these optical sources are responsible for correlating the mechanical translation of a computer mouse with the motion of the cursor on a monitor. They may also be used in conjunction with a photodetector and a transistor to provide electrical isolation between high and low voltage networks. As the applications in which LEDs are incorporated become more critical, reliability of the devices becomes an increasingly important concern.


For years the military has employed hermetic packages for optoelectronic and other electronic applications, due to reliability concerns. However,with the rapid growth of the computer and electronics industry, economic demands have shifted modern trends from expensive hermetic packages to low-cost,


nonhermetic plastic packages [4].


Before plastic packages can completely replace their hermetic counterparts, a better understanding of the failures in nonhermetic environments must be achieved. This research is being conducted to determine the failure modes and mechanisms associated with plastic packaging for AlGaAs/GaAs and GaAs LED devices under various temperature,humidity, and current bias conditions.


Experiment


Test Devices


There were two main types of LEDs studied in this experiment - Group 1 LEDs which were composed only of GaAs layers, and Group 2 LEDs which contained AlGaAs epilayers on a GaAs substrate.


Both groups of LEDs are topped with aluminum bond pads to which a gold wire is attached, and the devices are connected to a leadframe with a silverfilled epoxy. The LEDs are embedded in a soft silicone buffer inside of a hard encapsulant housing.


Figure 1 illustrates a cross-sectional view of a buffer coated LED.


The use of buffer coatings to provide more reliability protection of optoelectronic components has been adopted by several commercial manufacturers including AT&T, Delco, British Telecom, and


Figure 1 Schematic of the LED device crosssection


Ball Bond


Buffer Coating


Wire Bond


LED Die


Table 1 Stress Test Conditions for Group 1 Devices


Test Name


Description Initial/Final Conditions


Temperature Step


Current Step


Cycling Parameters


Typical Light Output Degradation


LTSS


Low


Temperature Step Stress


-10 C / 25mA-50 C / 45mA over 56 hours


-10 C


+5mA


N/A


Coated LEDs, negligible Uncoated LEDs, over 70%


TC


Thermal Cycling


-35C / +85C @40C/min ramp over 25 hrs, 5cycles/hr


Unstressed Unstressed


Hitachi. The coatings offer an increased barrier to moisture induced corrosion, as well as relief from mechanical stress. Hitachi has been using silicone gel as a corrosion prevention coating for over 8 years.


According to Blade, the silicone coating is not a moisture seal since it is permeable to water. Rather,the mechanism of the corrosion protection is the attachment of the ends of the long chain silicone molecules to the surface of the die. If the resultant dense forest of molecules is tightly arrayed, no water pools or water-filled voids would be formed. If there are no such water-filled voids, there would be no


place for water to dissolve corrosive ions [1].


Accelerated Stress Test Program


For both groups of LEDs an accelerated test program was implemented to achieve degradation of the LED light output. Following accelerated testing, the light output degradation for each device was recorded,then electrical characterization and failure analysis was performed. The test programs for the two LED groups differed in the types of accelerated tests performed, and the level of light output degradation achieved.


Accelerated test specifications and the typical light output degradation following testing for the Group 1(GaAs) LED devices are shown in Table 1. There were three basic test cells, low temperature stepstress (LTSS), temperature cycling (TC), and unstressed for devices which did not undergo stress testing. In addition to the various stress testing cells,a small portion of the Group 1 LED packages were assembled without a buffer coating in the plastic package. These devices are termed uncoated devices.


Failure analysis procedures for the Group 1 devices included photo- and electroluminescence imaging.


For Group 2 (AlGaAs) devices, the accelerated tests consisted of temperature/humidity/bias (THB) stress testing. Thus, test cells for the Group 2 LEDs were categorized based on three major stress parameters:


• current bias level (zero bias, 16mA, 40mA)


• ambient temperature (85 C, 121 C)


• ambient percent relative humidity (55%, 100%)


Also, the following convention has been adopted to describe the THB accelerated test parameters:


HB where


H = 2 for 85C/55%RH (1200 hrs)


4 for 121C/100%RH (250 hrs)


B = O for no current bias


L for 16 mA


H for 40 mA


For Group 2 LEDs, the failure analysis consisted of scanning acoustic microscopy, photo-, electro-, and cathodoluminescence imaging, and environmental scanning electron micrographs. Typical light output degradation performance for the Group 2 LEDs is listed in Table 2.


Table 2 Typical Light Output Degradation of


Group 2 LEDs


Temperature/


Humidity


Conditions


Current Bias(mA)


Typical Light


Output


Degradation


40%


16


50%


121 Co / 100% RH(250 hrs)


5%


20%


85 Co / 55% RH


(1200 hrs)


Electrical Characterization


Electrical characterization was performed on 320 Group 1 LED packages and 109 Group 2 LED devices. The LEDs were electrically characterized using an HP4145B Curve Tracer, and the I-V data generated from the curve tracer was downloaded into a computer worksheet for mathematical analysis.


The recorded parameters included forward and reverse biased current versus voltage (I-V) curves,from which breakdown voltage and leakage characteristics were determined. Five characteristic regions of the I-V curve have been defined to describe the observed electrical performance. Figure 2 illustrates the defined I-V curve segmentations.


• FS1: Forward slope 1 characterizes the rate of current increase between 0V LED bias and the turnon voltage. This parameter characterizes forward biased leakage currents.


• FS2: Forward slope 2 characterizes the rate of current increase following turn-on.


• RS1: Reverse slope 1 characterizes the rate of increase in current between 0V LED bias and breakdown. This parameter characterizes reverse bias leakage currents.


• RS2: Reverse slope 2 characterizes the rate of increase in current for bias values less than the breakdown voltage.


• BD: Breakdown voltage is the x-intercept at the onset of reverse breakdown.


The defined slope characteristics for each LED were calculated and analyzed based on the LED accelerated test conditions outlined in Table1 above.


Photoluminescence (PL) and electroluminescence(EL) measurements were performed on both Group 1 and Group 2 LED devices at the University of Maryland’s Laboratory for Physical Sciences. In each case, the measurements were achieved using the setup shown in Figure 3.


For a PL measurement, a laser is used to induce electron-hole pair recombination, and there is no requirement for electrical excitation of the LED. The excited carriers are generated in a layer near the surface of the die, equal to the absorption depth for the laser wavelength. EL, however, requires that the leads of the LED be connected to a current source,and the light generated is by recombination of electrically excited carriers in the LED active region.


The current source employed for the EL measurements was the ILX Lightwave LDX-3545 Precision Current Source, and the OmniChrome argon-ion laser was used as the PL excitation source.


The laser has an operating wavelength of 514.5nm


and an output power range of 0.5-80 mW. The lowpass filter removes the reflected laser signal by inhibiting the transmission of all wavelengths less than or equal to 550.0nm into the spectrometer. The SPEX Spectrometer Model 1702 has a resolution of 20 Angstroms/mm, a pathlength of 0.75m, and a period of 600 lines/mm. A chopper wheel is used to cut the light at a frequency of 400 Hz, and a germanium detector is connected to a lock-in amplifier that feeds directly into the computer.


Cathodoluminescence (CL) measurements were also performed at the Laboratory for Physical Sciences.


CL examinations were performed inside of a scanning electron microscope (SEM) chamber that is equipped with CL capabilities. Finally, crosssectional analyses were performed using an environmental scanning electron microscope (ESEM)housed at the University of Maryland Center for Microanalysis.


This section of the paper outlines the results from each of the analysis activities listed above; electrical characterization, PL and EL measurements, CL measurements, and cross-sectional analyses.


Electrical Characterization Group 1: GaAs LEDs


Fifteen sets of Group 1 LEDs were subjected to electrical characterization. Thirteen of the fifteen sets contained twenty LEDs, and the two remaining sets contained thirty LEDs. A subset of the test population included LED packages for which the buffer coating had not been included. Thus, the Group 1 LED study not only investigated the effect of different accelerated test conditions on the LED performance, but also the variation in performance,due to the lack of a buffer coating in the LED package. The devices that lack the buffer coating are Power


Meter


Argon-Ion


Chopper


LED


Lowpass Filter


Spectrometer


Lock-in


Amplifier Computer


Germanium Detector


mirror,


density filter


lens


Figure 3 Set-up for luminescence


BD


RS2


FS1


RS1


Figure 2 A schematic of the defined slope


regions and breakdown voltage on the I-V curve.


FS2


denoted in this paper as uncoated LED devices. Four of the fifteen sets consisted of uncoated devices, and the I-V curve data recorded from the uncoated population is distinguishable in Table 3 by an asterisk.


Table 3 lists average values of the previously discussed slope segments taken from the I-V curve data. The standard deviation for each calculation is also listed. For each case a normal distribution was


assumed, and data points that did not fall within 3σ of the average value were not included in the calculation. It was noted that for some instances, a normal distribution does not yield the best fit for the parameter distribution. These cases are generally identified by a standard deviation that is more than 30% of the average value.


From the table, it is evident that the uncoated devices exhibit larger leakage rates than their coated counterparts in both the forward and reverse biased leakage regions (RS1, FS1) of the I–V curve. For the low temperature test cell (LTSS) parts, the average RS1 values for the uncoated devices were typically an order of magnitude larger than that of the coated LEDs. This observation suggests that uncoated devices are characterized by leakier currents and softer breakdowns. No trend was observed for the FS2 values, which provide information on device ideality factors and contact resistance.


In comparing the performance of coated LEDs that underwent temperature cycling (TC) and LTSS testing, the results do not show any significant differences. However, contrary to what was expected, the coated LED samples that did not undergo stress testing did exhibit a large leakage rate in the reverse biased regime (RS1). Also, set 23 exhibited very high leakage currents in the FS1 regime, but the large standard deviation value for this set highlights the large variance in performance.


Finally, Table 4 lists the average breakdown voltages for the Group 1 devices. The data suggests a difference in the BD performance of coated and uncoated LEDs prior to stress testing. After testing has been employed, the coated and uncoated devices exhibit similar BV performance. One other observation that is not readily indicated from the data in Table 4 is that the uncoated LEDs typically exhibited a softer transition to breakdown as compared to the coated devices.


Group 2: AlGaAs LEDs


The electrical characterization data for the Group 2 LED devices is summarized in Table 5. Here, the IV curve data is sorted by the THB test cells. The data suggests several interesting trends. First, the application of a current bias during the test results in a much less negative characteristic breakdown


voltage. Second, at 85°C/55% RH (test cells 20, 2L and 2H), the leakage rate increased with the current bias in both the forward and reverse biased regimes.


However, the leakage rates for 121°C/100% RH tested packages (test cells 40, 4L and 4H) decreased as the current bias increased. There was no general trend apparent for the turn-on region (FS2) of the I-V curves. In general, the best performance occurred for cases where the accelerated test current bias was zero. However, the performance at 16mA and 40mA is dependent on some function of the combined ambient temperature and humidity conditions. These results suggest that the degradation mode for electrical performance may be different for the two temperature/humidity stress levels tested.


Photo- and Electroluminescence Measurements Group 1: GaAs LEDs


Both PL and EL measurements of Group 1 LED devices revealed that the absence of the silicone buffer coating induces a measureable blue shift in the peak emitted wavelength of the LED towards a shorter wavelength. This phenomenon is illustrated in Figure 4, which shows PL graphs for a coated and an uncoated LED. The graph shows a 20nm difference between the peak emitted wavelength for coated and uncoated devices. Also, the shift is more dramatic on the right side of the distribution. This effectively means the width of the emission peak is narrowed for the uncoated LED. However, the peak may actually be two unresolved transitions. This is more evident in Figure 5.


Figure 5 shows PL graphs for coated Group 1 LEDs that have undergone LTSS and TC testing, along with an unstressed Group 1 LED. Application of the accelerated stress conditions resulted in a small 5nm shift in the LED wavelength (when compared to an unstressed part), and again the width of the emission peak is affected. In this case however, the more narrow peak occurs for the unstressed LED, and the peak is broader for the TC and LTSS stressed LEDs,respectively. Close examination of the peak also shows some indication that there may be two unresolved peaks in the PL graph.


Table 3 I-V Characteristics of Group 1 LEDs


FS1 (pA/V)


FS2 (mA/V)


RS1 (pA/V)


Set No.


Average


St. Dev


Std. Dev


Sample Size


Temperature Cycle (-35C to 85C) over 125 cycles


550


20.7


0.68


107


22


19.6


0.99


41


4.9


180


18.2


4.73


7.1


18


710


90


19.2


0.71


27


9.2


Low Temp Step Stress (-10C to –50C), 25mA to 45mA over 156 hrs


790


19.7


0.54


42


36


1.03


70


0.49


21


820


130


0.67


6.3


20.3


0.58


9*


930


28.7


2.89


408


96


Unstressed


20*


1460


720


16.7


0.34


146


21*


1590


116


28


22*


1310


740


15.8


3.74


151


67


23


1450


1140


0.90


111


141


24


620


19.1


0.84


87


57


29


notes:


* Denotes sets with uncoated LEDs


Table 4 Average Breakdown Voltages for Group 1 LEDs


Stress


Breakdown Voltage (V)


-39.99


-42.20


LTSS*


-41.00


59


-35.90


Unstressed*


-42.27


Table 5 I-V Characteristics of Group 2 LEDs


BD (V)


RS1(pA/V) FS1(pA/V) RS2(nA/V) FS2(ma/V)


2O


-9.35


86.98


4O


-9.68


11


31


87.58


2L


-2.47


87.43


4L


-0.61


81


82


86.35


2H


83


87.21


4H


-1.09


58


86.52


PL graphs from Group 2 (AlGaAs) LEDs are shown in Figure 6. The figure shows the PL intensityof an unstressed LED and an LED taken from the 4LH THB test cell. The graphs show that THB conditions can cause a general suppression of the PL intensity,as well as broadening of the LED emission.


EL measurements from Group 2 devices are shown in Figures 7 and 8. The results show that certain THB conditions can induce a significant wavelength shift in the LEDs, compared to their performance prior to testing. From Figure 7, it is shown that a device


tested with 121°C/100%RH conditions experienced a


35nm shift towards a shorter wavelength, while a


device aged at 85°C/55%RH conditions experienced only a 5nm shift. Finally, from Figure 8, it is shown


that for 121°C/100%RH tested devices, the shift in wavelength only occurred when a current bias was applied during testing. For devices tested at 16mA and 40mA, the observed wavelength shift was 25nm and 30nm, respectively.


In his review of deep centers in silicon carbide,Lebedev performs EL measurements on various polytypes of SiC. He observes shifts in the maximum peak towards shorter wavelengths (in the case of a wider gap polytype) or to longer wavelengths (in the case of a narrower gap polytype) [2].


Lebedev explains that the results may be the result of band widening, but he also mentions that the observed behavior may be explained by studying impurity luminescence bands. Also, it is important to determine the radiative recombination mechanism responsible for the observed emission.


Table 6 lists the radiative and non-radiative recombination mechanisms that occur in semiconductor materials. Lebedev describes the shift of the peak to shorter wavelengths as the level of excitation increases as a distinctive feature of donoracceptor recombination [2]. Also, for Group 2


Figure 7 EL intensity graph comparing stressed


and unstressed Group 2 (AlGaAs) devices.


-70


-60


-10


6000


7000 8000


9000 10000 11000 12000


Wavelength (Angstroms)


EL Intensity vs. Wavelength


121C/100%RH


85C/85%RH


Figure 8. EL graph comparing Group devices following 121°C/100%RH testing.


7000


0mA


16mA


40mA


-35


-25


-15


6000 7000 8000 9000 10000 11000 12000


Figure 6 PL intensity vs. wavelength graphs of an unstressed (top) and a THB stressed Group 2 AlGaAs LED.


PL Intensity vs. Wavelength


Figure 4 PL intensity vs. wavelength graph comparing a coated and an uncoated Group 1(GaAs) LEDs. Both devices were unstressed.


9000


10000


11000


Without Buffer Coating


With Buffer Coating


Figure 5 Photoluminescence intensity vs. wavelength graph comparing stressed and unstressed Group 1


GaAs LEDs. All devices were properly coated.


-45


10000 11000 12000


Unstr LTSS TC


devices, wavelength shifts may be related to changes in the aluminum content of the active region. Indeed,the observed blue shift could be caused by a 2%change in the aluminum content of the active region.


Further study is needed to determine the cause for the observed PL and EL behavior.


Table 6 Radiative and Non-Radiative


Mechanisms [5]


Radiative


Non-Radiative


Band to band


Phonon emission


Band to acceptor


At dislocations


Donor to acceptor


At impurities


Thru isoelectric center


At lattice vacancies


Cathodoluminescence and Cross-sectional Analysis


Both a backscattered electron image and a photon image were obtained from the CL investigation.


Figure 9 presents the top view of a Group 2 LED device in both image formats following 121C/100%RH/16mA THB testing. The photon image clearly illustrates the extent to which the light emission is constrained only to the edges of the surface emitting device. Pey et al., using CL micrographs to examine the light emission of LEDs,discovered two main types of defect structures: small


black spots (typically less than 10µm across) which they later classified as dislocations, and large diffuse dark regions, which were later described as stacking


faults [3]. The vast dark regions seen in the photon image of Figure 9 did not fit either of the defect types. Thus, it was decided that the lack of light was due to another defect mechanism.


One possible cause for the obstruction of light emission may be a film that appears to cover a large portion of the top surface of the die. A magnified view of the surface reveals cracks in what is believed to be a corrosive oxide layer, seen in Figure 10.


Since the CL investigation revealed the presence of a film on the surface of the LED die, cross-sectional analyses were performed to support these findings.


Cross-sectional analyses were performed on Group 2 die that had been tested at the two different temperature/humidity conditions. Figure 11 contains micrographs of devices that had been stressed at 121 C/100%RH and at 85 C/55%RH. Both devices had a current bias stress of 16mA.


The cross-sectional analysis confirmed the presence of a corrosive oxide layer. The material appeared to be most abundant on the p-layer, which is the top layer of the device. Also, by comparing the two stress conditions, it is evident that the higher temperature/humidity conditions cause the corrosive material to develop not only on the p- and n-confining layers but


also on the top surface (as was seen in the CL pictures, Figures 9 and 10).


The observed surface oxide layer for Group 2 devices is consistent with previously reported studies on


AlGaAs devices [6, 7]. Dallesasse et al. reported degradation of AlGaAs heterostructures that had been


in dormant storage for several years [7], and Kish et al. further reported that the corrosion mechanism was


more prevalent in the p-doped epilayers as well [8].


A proposed reaction mechanism that is driven by the aluminum content of the die has been reported by


Ashby et al. [9] However, this mechanism has only been proposed for a high temperature wet-oxidation process. In this case, a stable Al2O3 layer is produced, and the layer is transparent at the emission wavelength of the semiconductor. Our surface layer appears however to be porous in nature, and it also is not transparent and likely inhibits the light output power.


It should be noted that scanning acoustic microscope images of the Group 2 packages analyzed in this investigation did reveal extensive delamination at the package leadframe. This would enable the ingress of


Figure 9 Backscattered eimage (l) and photon


image(r) of a Group 2 LED following


121°C/100%RH/16mA testing.


Figure 10 Close view of cracks on the top surface of Group 2 LED seen in Figure 9.


moisture into the package and therefore promote moisture driven corrosive reactions. We also have observed that the corrosive reaction is enhanced when the structure is forward biased, so that packages that were not current (or voltage) biased during THB testing did not exhibit the corrosive layers, as shown in Figures 9, 10 and 11.


Role of Photon Density


Some discussion of the role of photon density on this


process has also been discussed in the literature [10].


Maranowski describes the impact of blackbody radiation on the oxidation mechanism in temperature environments greater than 400oC. This environment clearly is not present at the temperature conditions studied in this experiment. However, photon enhanced degradation mechanisms should be considered in this analysis. For our study, the maximum photon density will occur at 40mA current bias, and it is assumed that the photon density is zero when the current bias is zero. While we did not observe significant differences in light output performance between devices biased at 16mA and 40mA (see Table 2), it is clear that for zero current bias (also zero voltage bias), the degradation is significantly slower. As well, the electrical performance of Group 2 devices stressed at 85oC/55% RH became worse as the current bias (and photon density) increased. (see Table 5) The opposite was true when the test conditions were increased to 121oC/100% RH. Here, the leakage current performance improved as the current bias increased from 16mA to 40mA.


Based on these observations, it is suspected that the two temperature/humidity environments chosen in this study promote different dominant degradation modes. When the ambient humidity is 100%, the effect of humidity dominates the LED degradation,while the effect of temperature (or current bias)dominates when the ambient humidity is reduced to 55% RH. The temperature at the die surface has the effect of driving off the humidity, thereby reducing the rate for a humidity driven reaction mechanism.


Thus, the lower surface temperature at 16mA bias compared to 40mA bias would explain the better electrical performance for 121oC/100%RH/40mA THB conditions as compared to 121oC/100%RH/16mA THB conditions. (see Table 5) On the other hand, the better performance of 85Co/55%RH/16mA stressed devices as compared to 85Co/55%RH/40mA devices indicates that some factor other than humidity dominates the observed degradation mode.


For this case, the dominant degradation mode is more likely driven by temperature, or some effect that is inversely proportional to humidity. Finally, from Table 2, the light output performance of Group 2 LEDs is not significantly tied to current bias.


However, the degradation is enhanced by the application of a current (or voltage) bias, as compared to unbiased devices. Also, the effect of temperature and humidity (even without a current bias) is apparent, as the light output degradation is near 50% after 250 hours for 121oC/100% RH conditions, compared to 20% at 85oC/55% RH for 1200 hours. These results suggest a complex interaction related to temperature, humidity and voltage bias. Again, more investigation is needed to confirm this assertion.


In reviewing the combined light output performance,electrical performance, luminescence characteristics,and cross-sectional analyses of plastic packaged GaAs and AlGaAs/GaAs LED structures, several observations are summarized as follows. First, the use of a soft buffer coating to relieve mechanical stresses on the LED die is imperative for reliable optical performance. Packaged GaAs LEDs that had been tested and that did not contain the buffer coating exhibited over 70% reduction in the light output power within 160 hours of low temperature testing,and within 125 cycles of temperature cycle testing.


The coated die exhibited negligible optical degradation as a result of the accelerated testing stresses. Also, prior to the application of the temperature and bias stress testing, there were 3 distinct differences between the uncoated and coated LED devices. The uncoated die exhibited an emission wavelength that was characteristically shorter than the emission observed from the coated die. There also was a difference in the breakdown voltage characteristics between coated and uncoated LED die. Finally, the leakage rates for the uncoated


Figure 11 Cross-sections of a 121C/100%RH (l)and a 85C/55%RH (r) Group 2 device


For each case, the in-test current bias was 16mA.


devices were larger than in the case of the coated LED devices. Surprisingly, we observed that the leakage performance for coated devices following stress testing was better than for unstressed devices.


Based on these results, it would appear that a program to monitor the emitted wavelength and basic I-V characteristics of the LED (even before qualification or accelerated testing) can signal problems in the packaged LED product.


Another observation that can be concluded from our investigation is that degradation of AlGaAs LED structures under THB conditions involves a complex mechanism related to temperature and moisture on the die surface, as well as current or voltage bias.


Photon density may play a small role as well, but this has not been confirmed through our present investigation. We have however, observed that the light output performance of the AlGaAs LEDs is not greatly affected by increased current bias or greater photon density. Rather, ambient temperature, relative humidity at the die surface and voltage bias appear to be better correlated to the light output performance.


The electrical performance is more complex. With 85oC/55% RH stress conditions, the breakdown voltage and leakage rate performance improves as the injected current is lowered, while the opposite was true when 121oC/100% RH conditions were applied.


We believe the two cases indicate different dominant degradation modes. In the case of 121oC/100%RH,the degradation is more correlated to humidity at the surface of the LED die. In the case of 85oC/55%RH ambient conditions, the degradation is better correlated to current bias and temperature.


It is our hope that this investigation can be used in conjunction with other studies to gain a complete understanding of the LED degradation in nonhermetic packages in high temperature and humidity environments.


The authors wish to express thanks to Keith Rogers and Craig Hilman of the CALCE Center Failure Analysis Laboratory. This work has been sponsored in part by National Science Foundation grant#ECS9702329.


1) Blade, J. "The effectiveness of silicone gels for


corrosion prevention of silicon circuits: The final report of the IEEE computer society computer packaging committee special task force" IEEE Transactions on Components, Hybrids, and Manufacturing Technology vol. 14 (2), 1991.


2) Lebedev, A. "Deep level centers in silicon carbide: A review". Semiconductors - American Institute of Physics vol. 33 (2), 1999.


3) Pey, K. L. et al. "Optoelectronic material analysis and device failure analysis using SEM cathodoluminescence". Proc. of the International Symposium on the Physical and Failure Analysis of ICs. Singapore, 1993.


4) University of Maryland - CALCE Electronic Products and Systems Consortium "Introduction and Overview - Plastic Encapsulated Microelectronics", 1998.


5) Wittpahl, V. et al. "A degradation monitor for the light output of LEDs based on cathodoluminescence signals and junction ideality factor". IEEE, 1996.


6) Dallesasse, J.M. et al., “Hydrolization oxidation of AlxGa1-xAs-AlAs-GaAs quantum well heterostructures and superlattices,” Appl. Phys. Lett.


57 (26), 24 December 1990.


7) Dallesasse, J.M. et al., “Environmental degradation of AlxGa1-xAs-GaAs quantum- well


heterostructures,” J. Appl. Phys. 68 (5) 1 September 1990.


8) Kish, F.A., et al., “Dependence on doping type(p/n) of the water vapor oxidation of high-gap AlxGa1-xAs,” Appl. Phys. Lett. 60 (25), 22 July


9) Ashby, C.I., et al., “Wet oxidation of AlGaAs:


the role of hydrogen,” J. Appl. Phys. 82 (6) 15 September 1997.


10) Maranowski, S.A., et al., “Photon-induced anisotropic oxidation along p-n junctions in AlxGa1-xAs-GaAs quantum well heterostructures,” Appl. Phys. Lett. 62 (17), 26 April


Electronic Device Failure Analysis Society, editor, p 183-188


DOI: 10.1361/cp1999istfa183


# A Technique for Measuring Device Temperature with High Accuracy in Accelerated Operational Life Tests


A Technique for Measuring Device Temperature with High Accuracy in Accelerated Operational Life Tests


K. Takeda, M. Harigaya, Y. Miyazaki


NEC Corporation, Kawasaki-shi, Kanagawa, Japan


This paper describes a new technique for measuring junction temperature with high accuracy in accelerated operational tests (junction temperature≥200º) based on the measurements of temperature dependence of gate-leakage current on a GaAs FET(gate-leakage method). The gate-leakage current on the GaAs FET is monitored in the accelerated operational tests. Then, junction temperature and thermal resistance are calculated from the temperature dependence of the gate-leakage current, especially from the temperature dependence in high temperature region. We have measured the junction temperature and the thermal resistance using this method in accelerated operational tests, and have confirmed that the junction temperature can be estimated within a range of ten degrees. The results by this method have been compared with data of simulation, and the validity has been confirmed.


It is important to obtain high precision temperature data in accelerated operational life tests which are implemented to determine failure mechanism and MTTF (Mean Time To Failure). Conventionally,some useful techniques have been used as methods for measuring thermal resistance and junction temperature, such as:


A) a method with a infrared scope (infrared method)B) a method using temperature dependence of Vf of the diode which is placed near the active area(∆Vf method)


C) a method using temperature dependence of the device itself by power-on/off (∆Vgs method) [1,2].


These methods, however, have the following problems:


A) resolution of detector in infrared method


B) error depends on the monitoring at the position separated from the heating element in ∆Vf method


C) error depends on the time lag of power-on/off in Vgs method


D) condition which is different from that of the practical accelerated operational tests


We have developed the gate-leakage method to solve these problems. In this paper, the principle of the gateleakage method is described in detail, and the validity of the method is discussed on the basis of the experimental results.


New Technique


The principle of new technique, the gate-leakage method, is stated in this section. The thermal resistance and the junction temperature in accelerated operational life tests are estimated from the gate-leakage current which is monitored during the life tests. Figure 1 shows the GaAs FET in accelerated operational tests. Here we suppose making some examinations in which some ambient temperature (Ta) and some power (=Vds×Ids)conditions are controlled. The gate-leakage current (Ig)on the GaAs FET is monitored under some Ta conditions and under some power conditions. In each examination, gate-voltage (Vgs) is controlled to keep the power constant (Vds is kept constant, and Ids is also kept constant by controlling Vgs). Figure 2 shows temperature dependence of Ig obtained in the examinations explained above. The temperature dependence of the gate leakage-current in the high temperature region is shown in Figure 3.


The thermal resistance (θ) is related with ∆Ta and∆Power


θ = ∆Ta/∆Power.


(1)And the junction temperature (Tj) is calculated from Ta and Power.


Tj = Ta +θ Power.


The gate leakage-current can be given as the following expression:


Ig = -(AI0+AIgen),


A : area of junction


Igen : recombination current by generation and recombination of carrier in


depletion layer


I0 = q


Np


Ln Dn


Pn


Lp Dp


Dp,Dn : diffusion constant of


hole, electron


Lp=(Dp τ p) 1,2 : diffusion length of hole


Ln=(Dn τ n) 1,2 : diffusion length of


electron


Pn: density of hole in n type material in


equilibrium ~ ni2/NA


Np: density of electron in p type material in equilibrium ~ ni2/NA


ni2 = NAND exp  φ−kTq


ø : diffusion potential


Igen = q τ effni x


τ eff : effective life time of carrier in depletion layer


x : depletion width


Figure 2 Ig versus Ta of GaAs FET in accelerated operational tests


Ln(-Ig)


Power 1


Power 2


∆ Ta


T1


T2


Figure 3 Ig versus Ta in the high temperature region


Sourc


Vds


Figure 1 GaAs FET in accelerated operational tests


Power = Vds x Ids


Drai


Ids


Ig


Vgs


Ta


AI0


Figure 4 Current versus Voltage of FET’s gate-source


Igen has great influence on Ig when ni is small, because there are following relations: I0∝ni2 ,Igen∝ni. In other words, Igen has great influence on Ig when temperature is in low region. In high temperature region we don't have to consider the influence of Igen. The high temperature region of Figure 2 is shown in Figure 3.


The thermal resistance in accelerated operational tests is calculated using equation (1) from the temperature delta and the power delta at every power condition.


And the junction temperature in accelerated operational tests is calculated using equation (2) by the thermal resistance, the temperature and the power.


Experimental Results


In this section, we present an example of the junction temperature and the thermal resistance in accelerated operational tests estimated using the gate-leakage method. Figure 5 shows the GaAs FET we have used in our experiments. This FET has the following dimensions:


Lg = 0.18 µm


Wg=200 µm (100 µm × 2 fingers)


We have measured the junction temperature and the thermal resistance in accelerated operational tests under the condition-1. (The condition-1 is Ta=200º,Power=168mW at Vds=4.0V and Ids=42mA). The gate-leakage current on the GaAs FETs (we have used 8 pieces of FETs composed of 4 pieces 2 diffusion lots) have been monitored in the accelerated operational tests under the following conditions:


Ta = 150,175,200ºC


Power = 4,40,168mW


(Vds=4.0V, Ids=1,10,42mA)


Power-1:168mW (Vds=4.0V,Ids=42mA)Power-2:40mW (Vds=4.0V,Ids=10mA)Power-3:4mW (Vds=4.0V,Ids=1mA)


Figure 6 shows an example of Ig versus Ta on one FET monitored at each condition. We have calculated the junction temperature and the thermal resistance of condition-1 using Figure 6.


From Figure 6, we have read the values of temperature at which the value of Ig in the Power-2 curve is equal to that in the Power-1 curve. Then, the thermal resistance is calculated from the temperature gap using equation (1), and the junction temperature is cal-culated using equation (2). In the same way, we have read the values of temperature at which the value of Ig in the Power-3 curve is equal to that in the Power-1 curve. Then, the thermal resistance and the junction temperature are calculated using equation (1)and equation (2). The data of Table 1 are the results of the junction temperature and the thermal resistance calculated on every FET.


Consequently, the value of the junction temperature in accelerated operational tests under condition-1, has been estimated at 228ºC ~ 237ºC. In other words, we have estimated the value of temperature increase up to 28ºC ~ 37ºC, and have confirmed that the junction temperature can be estimated within a range of ten degrees in accelerated operational tests.


Figure 5 Optical Microscope image of the GaAs FET using our experiments


Table 1 The results of junction temperature and thermal resistance (at Ta=200°C,Power=168mW)


calculated using the gate-leakage method.


The results using Ta versus Ig at


the Power-1 and the Power-2


The results using Ta versus Ig at the Power-1 and the Power-3


Lot Device No.


junction temperature[ºC]


thermal resistance[ºC/W]


The results of


junction


Temperature[ºC]


by every lot


232.2


191.4


231.2


186.0


232.8


195.3


195.1


233.2


197.7


236.4


216.5


231.8


189.1


236.6


217.7


231.2~ 236.6


229.5


175.8


228.9


172.0


229.8


177.4


229.9


178.1


230.2


180.0


230.4


181.1


228.9~ 230.4


Total


229.5~ 233.2


175.8~ 197.7


228.9~ 236.6


172.0~ 217.7


Ta−ln(−Ig)


(4V,42mA/4V,10mA/4V,1mA)


1.00E-08


1.00E-07


1.00E-06


1.00E-05


1.00E-04


125


145


165


185


205


225


245


Ta[°C]


Figure 6 The results of Ig measurement in accelerated operational tests(The results of Ig measurement in Power1, Power2 and Power3)


Power1=168mW(4V,42mW)


Power3=4mW(4V,1mW)


Power2=40mW(4V,10mW)


Discussions


The results of table 1 shows that the junction temperature estimation can be made within a range of ten degrees using our method, even if the intersample variations or inter-lot variations are considered. The new technique we developed, the gate-leakage method, can inspect the device temperature with high accuracy in accelerated operational life tests.


Figure 7 and Figure 8 show the thermal analytical simulation in accelerated operational tests under condition-1. This simulation has been operated in the way where the rectangular thermal source of base surface is a set of point thermal sources or small hemisphere thermal sources. And the temperature of every coordinate is a set of the effects of the point thermal sources [2-15] . As the results of the thermal analytical simulation, the temperature increase is 30ºC~ 70ºC on the average (the peak thermal of climb was 98ºC).


The results by our method have been compared with data of the simulation and we have considered following:


• measurement results of our method are the average data of the whole FET


• there is the radiation of heat from the nodes in the practical measurement


Therefore, we have concluded that the validity of the results by our method have been confirmed.


We have developed a new technique for measuring the junction temperature with high accuracy in accelerated operational life tests.


The junction temperature and the thermal resistance are estimated from the temperature dependence of the gate-leakage current which is monitored during the life tests. We have measured the junction temperature and the thermal resistance using this method in accelerated operational tests (junction temperature≥200ºC), and have confirmed that the junction temperature can be estimated within a range of ten degrees. The results by this method have been compared with data of simulation, and the validity has been confirmed.


1) H. F. Cooke, MICROWAVES and RF., August,85-87, (1986)


2) M. S. Fan, Reliability of Gallium Arsenide MMICs., 384, (1992), John Wiley & Sons


3) J. S. Blakemore, J. Appl. Phys., vol.53, R123-R181, (1982)


4) S. Adachi, J. Appl. Phys., vol.58, R1-R29, (1985)5) S. Adachi, J. Appl. Phys., vol.54, 1844-1848,(1983)


6) J. L. Wright, B. Marks, and K. D. Decker, IEEE SEMITHERM Symposium Dig., 131, (1991)


7) C. C. Lee, A. L. Palioc, and Y. J. Min, IEEE CHMT., vol.12, 701-709, (1989)


8) C. C. Lee, A. L. Palioc, and Y. J. Min, IEEE CHMT., vol.12, 710-716, (1989)


9) L. Palioc, Y. J. Min, and C. C. Lee, J. Appl.


Phys., vol.65, 4438-4444, (1989)


10) D. Smith, GaAs IC Symposium, 187-190, (1991)11) D. Smith, A. Fraser, and J. Oneil, IEEE SEMITHERM Symposium Dig., (1986)


12) K. Poulton, K. L. Kundsen, etal, IEEE J. Solid State Circuit, vol.27, 1379-1387, (1992)


13) W. B. Joice, Solid State Electron., vol.18, 321-322, (1975)


14) C. Lee, Y. J. Min, and A. L. Palioc, J. Appl.


Phys., vol.64, 410-415, (1989)


15) L. Selmi, and B. Ricco, IEEE Trans. ED., vol.40,273-277, (1993)


0 20 40 60 80 100 120


The thermal analytical simulation(@Ta=200°C, Power = 168mW)


Figure 7 The results of the thermal analytical simulation in accelerated operational tests(Ta=200°C, Power=168mW(Vds=4V,Ida=42mW))


Figure 8 is shown from this direction


The thermal analytical simulation


(@Ta=200°C,Power=168mW)


Figure 8 The results of the thermal analytical simulation in accelerated operational tests(Ta=200°C,Power=168mW(Vds=4V,Ids=42mW))


Source this section


Electronic Device Failure Analysis Society, editor, p 189-193


DOI: 10.1361/cp1999istfa189


# Temperature Measurement on Micromachined IR Bolometers Using an Infrared Microscope


Temperature Measurement on Micromachined IR Bolometers Using an Infrared Microscope


A D Trigg, U Sridhar


H S Lee & G Karunasiri


Electrical Engineering Department, National University of Singapore


Thermal properties are critical to the performance of micromachined silicon bolometers. In order to verify thermal models of the device, a means of measuring the local temperature distribution over the element is required, as it is heated by passing current through a thin film titanium meander. Because of the very low thermal mass of the membrane a non-contact method of temperature measurement is needed. Most conventional thermal imaging systems operate in the


wavelength range 5-15 µm and offer poor spatial resolution but in this work an infrared microscope,operating at shorter wavelengths, was used.


The microscope comprises an objective lens which focuses radiation onto a cooled (77K) cadmium mercury telluride focal plane array sensitive over the range 800 nm to 2500nm. For this application a bandpass filter centered at 2150 nm was used. Good agreement was obtained between finite element modeling of the temperature distribution, using ANSYS, and the measured data.


Infrared Imaging


An ideal surface that absorbs all wavelengths of electromagnetic radiation incident upon it, is also the perfect emitter of all wavelengths of radiation and is termed a blackbody [1]. The continuous-spectrum radiation that it emits is called blackbody radiation.


By 1900 this radiation had been study extensively,and several characteristics had been established.


First, the total intensity M (the average rate of radiation of energy per unit surface area or average power per area) emitted from the surface of an ideal radiation is proportional to the fourth power of the absolute temperature T. This is given by the StefanBoltzmann law, Equation 1.


M = σT4


where σ, the Stefan-Boltzmann constant is equal to 5.67x10-8 W/m4K4


Second, the intensity distribution can be measured and described by the intensity per wavelength interval M(λ), call spectral emittance. Thus M(λ) dλ is the intensity corresponding to wavelengths in the


interval from λ to λ+dλ. The total intensity M, given by Equation 1 is the integral of the distribution function M(λ) over all wavelengths, which equals the area under the M(λ) versus λ curve, Equation 2.


Planck’s law gives this relation for a black body,Equation 3.


where:


λ =


wavelength in µm,


C1 = first radiation constant = 3.74x10-16 Wm2 C2 = second radiation constant = 1.44 x 10-2 Km T =


absolute temperature.


The Planck radiation law also contains the Wien Displacement law and the Stefan-Boltzmann law as consequences. The Wien Displacement law can be derived from Equation 3 by setting dM/dλ = 0 to find the value of λ, at which M(λ) is maximum:


λmT = 2898 (µm)


σ


∞


T C2


C1


To decide which part of the infrared spectrum to use for imaging objects at a distance we need to know the wavelength corresponding to maximum intensity and where the atmosphere has a high transmittance. From Figure 1, in which the transmittance of the atmosphere is superimposed on the smooth curve of Equation 3, it can be seen that for room temperature,T = 293K, Mλ has its maximum at 10µm and that this coincides well with a transmission window of the


atmosphere in the range 8 – 12µm. Hence this is the window most frequently used in thermal imaging.


Figure 1 Blackbody radiation at 293 K and


atmospheric transmission.


Infrared Bolometers


A thermal sensor works according to a two step process. First, the incident radiation is absorbed in the detector whose temperature increases. As the second step, this temperature increase is measured as a change of an electrical parameter. This two step transduction process is slower than the single step process of photonic devices, but other advantages of thermal detectors, operation at room temperature,wide spectral response range and low cost make them very attractive for development.


An array of elements, each 50 µm square, forms the imaging bolometer. Each element comprises a free standing, thin membrane of silicon nitride supported at two corners, on which there is a titanium meander.


The membrane absorber is isolated from the heat sink to give minimum heat capacity and maximum temperature change for a given amount of radiation.


The radiation flux is measured as a change in resistance of the titanium meander. The process is shown schematically in Figure 2. The incident radiation is absorbed causing the metal (resistor) to heat up. This causes a variation of the resistance which is determined by an external circuit. The membrane is designed to absorb the infrared radiation


in the range of 8-12µm (atmospheric window). Heat loss from the membrane occurs by conduction to the silicon substrate, which acts as a heat sink to provide fast response, and by air convection. The silicon substrate also dissipates the bias-current power.


Figure 2 Operation of an infrared bolometer.


The behaviour of the heat flow and temperature in thermal system is described mathematically by the same equations as those used in electrical systems.


This enables a thermal system to be described by means of electrical equivalents, which is convenient because of the advanced description and analysis tools available for electrical circuits.


The heat balance equation for the bolometer is :


where :


∆T = temperature difference between bolometer and heat sink


C = heat capacity


G = thermal conductance


W = incident IR power


t = time


The thermal conductance, G, and the thermal capacity, C, are the two most important thermal parameters of a thermal detector, which can be defined as:


and


dQ/dt = the heat flow from the detector to its surrounding.


In the steady state condition the heat balance equation for Equation 5 becomes:


G W


T =


∆


0 5 10 15 20 25 30


13


Wavelengt h (micromet res)


0 10 20 30 40 50 60 70 80 90 100


Ts


Heat sink Absorber/


membrane


Ts+∆T


G


dt


Cd


dt dQ


G∆=


K W


T Q


C∆∆=


K J


Experimental Model


In order to verify thermal models of the device, a means of measuring the local temperature distribution over the element is required, as it is heated by passing current through the titanium meander. Typically a current sufficient to raise the temperature to 100°C is used. Because of the very low thermal mass of the membrane, a non-contact method of temperature measurement is needed.


Experimental observations were made using an infrared microscope developed at the Institute of Microelectronics, Singapore. The microscope has been described in detail previously [2] . In summary it comprises a probe station on which is mounted the sample, a lens turret which allows lenses to be selected to give the correct magnification, an illuminator, an infrared (IR) camera with a wavelength range of 800 to 2500 nm, and associated electronics and computer so that the image can be displayed on a monitor. Incorporated into the IR camera is a filter wheel which enables an appropriate wavelength range to be selected. The infrared microscope operates at shorter wavelengths, 0.8 - 2.5


µm, than most commercial thermal imaging systems,typically 5-12 µm, thus enabling it to provide better spatial resolution. For this work images were obtained using a filter transparent to radiation from


2.0 - 2.4 µm. A schematic of the apparatus is shown in Figure 3.


Figure 3 Schematic of the IR microscope.


The device was mounted on a temperature-controlled platform (Hot Chuck). An initial, illuminated image,was obtained using a shorter wavelength filter,Figure 4.


Figure 4 Illuminated IR image of bolometer.


Image width = 100 µm.


Thermal images of the bolometer were then obtained at a series of increasing currents. Two lenses were used, a conventional microscope objective designed for near infrared (NIR) imaging and a reflecting lens.


The latter provided significantly better spatial resolution, 2-3 µm, at the 2.0 - 2.4 µm wavelength used for thermal imaging. See Figures 5 & 6.


Figure 5 Thermal image of bolometer with current of 650µA. Conventional NIR lens.


Figure 6 Thermal image of bolometer with current of 500µA. Reflecting lens.


The FMECA New Approach


As stated above, the new approach introduces the new terminology for Next Brother Effect (NBE). In this case, the functional tree may be identical to the project tree, as presented in Figure 2.


The NBE is used here to propagate the ASIC failure modes to its brothers in the hierarchic functional tree.


Function A failure mode is propagated, by the computerized program tool, to function 1.1 and function B failure mode to function 1.2. This method completely and accurately supports the required functional tree as presented in Figure 1.B. In addition


it assures that the α’s sum, as explained earlier, will never exceed 1.


Evidently, in most cases, the NBE methodology provides the designers with capabilities to use the project tree as a functional tree and thus reduce, in most cases, the need for the construction and maintenance of a separate functional tree. Thus, the PCB and systems designers, supporting the concurrent engineering approach can perform the FMECA.


Function 1.1


ASIC (FR=100)


Function


A B


Ratio


αA αB


Function 1.2 System


Level


Function A


FR


αA


System Level


Next Higher


Effect (NHE)failure


propagation


Function B


αB


Figure 1 Traditional FMECA Concept


The New BIT Approach


The usage of NBE opens the door for a tremendous improvement of BIT designs in the name of Good


Modes© (GM). In case a sub-block fails (function A in our example) it may cause the next function (1.2 for example) to change its functionality to a new state where it is still operational. For example, when a CPU controls two redundant valves, identified failure of one valve will cause the software to use only the second valve, yet using the second valve is a Good


Mode©.


In any one of the functional tree levels, a good mode,NBE or NHE may be a failure mode. Thus, the algorithm propagates good modes in the functional tree in an identical way to the failure modes. The computerized tool calculates the good mode“positiveness”, e.g. its occurrence rate. A good mode signals a failure in the system while the "positiveness"is a good factor that means how well the system can identify a failure. The designer can use both, the positiveness and the criticality values, in making a decision whether it is cost effective to develop the specific BIT.


It is evident that the good mode terminology can improve the BIT design. It assures, that for mixed a hardware-software system, that a failure mode is identified by the brother of a higher hierarchic levels,and thus assures its identification.


Binding RBD and FMECA


The RBD describes systems blocks and sub-blocks depen-dence in a reliability point of view. In many cases (such as telecommunication network) one can view a well-designed RBD in a functional tree structure, e.g. it can be directly used for FMECA. In the CARE software, we elaborate on the algorithm and method to computerize this approach. See figure 3 and figure 4.


We showed in this article that by using new


terminology of “Next Brother Effect©” and “Good


Modes©” as part of the FMECA and BIT computerized tools:


We introduced new terminology to enhance the wellknown standards, while assuring their full support.


Functional trees can become very similar to the project trees, functional trees construction time is reduced by factors.


Designers can have greater flexibility in describing the failure modes and achieve more accurate and more accessible BIT designs.


ASIC


(Functions A and B)


Function 1.2


Next Brother Effect(NBE) failure


Next Higher Effect(NHE) failure


Figure 2 The CARE® New FMECA Concept


Figure 3 The CARE® Example of a network model in RBD


Figure 4 The CARE® Example of FMECA screen


Reference


1) Y. Bot, “Reliability and Cost Optimization”,Probab-ilistic


Safety


Assessment


and Management ESREL-96’ June 24-28 1996,Crete, Greece, Proceedings, Volume 1, pp. 261.


2) Y .Bot, “ORLA: Optimum Repair Level Analysis”, Integrated Logistics & Concurrent Engineering, ILCE-94’ February 7-11 1994,Montpellier, France, Proceedings, pp. 213.


3) Y. Bot & A. Zvigoren, “Shrinked Logistic Support Analysis” The Tenth International Conference of the Israel Society for Quality”,November 14-17, 1994, Jerusalem, Israel Proceedings, Part II, pp. 826.


4) Y. Bot & Y. Herrer, NRCN, “Usage of


Commercial Methods for Reliability Prediction in various Industries”, The Eleventh International Conference of the Israel Society for Quality,November 19-21, 1996, Jerusalem, Israel Proceedings, pp. E.342, H.281


5) Y. Bot, “Failure Mode Analysis as a driver to Safety Analysis”, The Eleventh International Conference of the Israel Society for Quality,November 19-21, 1996, Jerusalem, Israel Proceedings, pp. E.405, H.353


6) Y. Bot, BQR, A. Zvigoren, Rafael,“Troubleshooting Diagram Generator”, The Eleventh International Con-ference of the Israel Society for Quality, November 19-21, 1996,Jerusalem, Israel, Proceedings, pp. H.185


7) Y. Bot, “RAMCAD: Automatic FMECA for Electronic Digital Systems", The Eleventh International Conference of the Israel Society for Quality, November 19-21, 1996, Jerusalem, Israel Proceedings, pp. H.47


8) Y. Bot, “FMECA for Software and Hardware”,The Third National Conference of the Israel Society for Quality, November 15-16, 1995, TelAviv, Israel Proceedings, pp. 344


9) Y. Bot, “Integrating Reliability Analysis Tools in AD/ CAE”, ASME International Electronic Packaging Con-ference, InterPACK ’97 June 15-19, 1997, Kohala Coast, Island of Hawaii Proceedings, pp. Track #3, Session 3.1


10) Y. Bot, “Reliability of Electronic Components,Failure Rates Prediction Methods” International Conference on Safety and Reliability ESREL ’97 17-20, June 1997, Lisbon, Portugal Proceedings,pp.


11) Y. Bot, “Electronic Systems fails even when they do not operate”, Industries Magazine, 15.7.1989 pp. 37


12) Y. Bot, “Software Failure Analysis for Electronic Systems”, Technologies Magazine, Volume 139,January 1996, pp. 36


13) Biography


14) Yizhak Bot, President and Chief Technical Officer.


15) BQR Reliability Engineering Ltd. P.O.Box 208,Rishon-Lezion 75101, Israel


16) Phone: 972 - 3 - 966 3569


17) Internet (e-mail): bot@bqr.com


Internet Home Page: www.bqr.com


18) Mr. Bot is a Certified Reliability Engineer from ASQC (1982) and studied Electronic Engineering in Tel-Aviv University (1977-1980).


19) Mr. Bot has more than 25 years of experience in RAMS and ILS. He was the RAM/ILS manager of many defense and commercial projects of more that US500 Million Dollars. He has written articles for leading magazines, conducting seminars and gives lectures worldwide. He is also


the inventor of CARE®.


20) From 1989 he is the president of BQR, a leading consulting and software developing firm.


Previous employment as a Reliability and ILS Engineer: freelance adviser (1984-1989), Tadiran Telecommunication (1980-1984) and IDF (1970-1980).


Electronic Device Failure Analysis Society, editor, p 211-215


DOI: 10.1361/cp1999istfa211


# Selective Au-Etching on Aged GaAs-based Devices


Selective Au-Etching on Aged GaAs-based Devices


M. Vanzi, A. Bonfiglio, P. Salaris


University of Cagliari, DIEE-INFM, Cagliari, Italy


P. Deplano , E.F. Trogu, A. Serpe


University of Cagliari, Dipartimento di Chimica e Tecnologie Inorganiche e Metallografiche


G. Salmini, R. De Palo


Pirelli Cavi e Sistemi S.p.A., Viale Sarca, Milano, Italy


A specific problem in failure analysis of InGaAs/AlGaAs laser diodes asked for a deprocessing tool able to selectively etch gold from a Ti/Pt/Au triple metal layer. Attempts made by the usual I2/KI etch confirmed the damage that it causes to the crystal stack, and non-uniform attack of gold. A new etch,indicated as Epta-Methyl-bis-diodine, has been successfully employed. Careful time control and detailed characterization of the complex metallization pattern of the devices allowed not only to properly expose the Pt layer, but also to preserve the overall electrical connection, thus maintaining the capability of both measuring the electrical characteristics at low current injection and collecting the EBIC signal from the etched device.


The analysis of 980 nm SL SQW InGaAs/AlGaAs pump laser diodes has pointed out the occurrence of some failures that are likely to be originated somewhere far from the optically active layer and then under laser operation, progressively approach the light emission area until it is penetrated, thereby causing sudden and extended defects in the strained


InGaAs lattice after long regular laser operation [1].


The sudden occurrence of the failures, and the location of some defective areas inside the optical cavity, far from the mirror edges, excluded an external source (COD) for the observed phenomenon.


Failure analysis was able to reveal the final damage by EBIC and addressed FIB cuts across the defect pattern (Fig.1).


Figure 1 30 keV EBIC (left), SEM before (middle)and after (right) FIB cuts.


Nevertheless, we have not been able so far to select a cut with the whole damage evolution clearly detectable.


When metal removal has been done by means of the familiar iodine-iodide I2/KI etch, mainly for increasing the EBIC resolution, the disappointing result was that the semiconductor was etched and that surface contamination or possibly the locally different Au grain distribution in aged devices, made the etch non-uniform. Attempts to allow longer etch times or use more concentrated solution, for complete Au dissolution, destroyed the thick Au pads which bond the gold wires to the triple metal, opening the electrical connection.


Another method has been followed based on lifting off the triple metal by etching the dielectric which separates it from the crystal surface for most of the die. As can be seen in fig.2, the dielectric layer is interrupted on the ridge where the metal directly contacts the semiconductor with the aim to focus the current onto the required stripe of the active layer.


In this case, not only the electrical contact was lost again, requiring mechanical probing to restore EBIC,but also FIB/TEM investigation revealed surface damage at the metal-semiconductor interface (fig.3).


gold


GaAs/AlGaAs/InGaAs


Si3N4


Figure 2 Schematic structure of the laser


metallization. The lateral silicon nitride allows


current flow only across the ridge. Gold is separated from semiconductor by a Ti/Pt barrier


Figure 3 surface damage after removing the Ti/P/tAu metal layer by pulling it away.


This is likely to be caused by pulling away the ohmic contact, as the only anchorage stripe of the lifted-off triple metal. It also points out the possibility that the observed damage comes from local interdiffusion phenomena, whose products have also been removed with the overlaying metal.


The careful re-examination of the available FIB cross sections, even taken at non-defective points of reference devices, pointed out in only one case (fig.4)a very faint indication of possible cracks in the Pt barrier, that could confirm the interdiffusion hypothesis.


1 µm


Figure 4 Possible cracks at the Pt interdiffusion


barrier.


The obvious requirement of more sound results asked for the only suitable way of revealing Pt cracks:complete and selective Au removal from the Pt layer,and direct SEM observation.


The first step is to characterize the whole ridge structure. FIB slices (Figure 5) greatly ease the work,providing a means to link the topographical information of SEM with the structural insight of TEM(Figure 6, 7).


The previous methods have proven unsuitable, thus new chemistry has been investigated for this specific case.


Figure 5 FIB slice of the beginning of the ridge.


Figure 6 Comparative images of the ridge cross


section, taken at SEM (left) and TEM (right). The


ridge is 3 µm wide.


As can be seen in fig. 7 etching has to remove a gold layer of no more than 200 nm, over an equally thick Pt layer. Selectivity is mandatory.


The small thickness of the ridge gold coating also suggests a way for preserving the electrical continuity even after etching gold.


Surface damage


Active layer


Figure 7 More detailed TEM image of the metal


structure, at one of the lateral edges of the ridge. The thin Ti layer is nearly undetectable. The bright thin layer covering gold is likely to be a reflow residual of the mirror coating.


Taking into account the relative thickness of the other gold parts: the bond pads (fig.8) and the bonded wires(fig.9), it seems possible to expose the Pt surface on the ridge while only slightly reducing the huge thickness of gold in pads and wires by time control of the etch actio. This calls for another property of the etch: uniform action and low sensitivity to surface geometries.


bond pad


ridge


Figure 8 The bond pads at the ridge sides are much thicker than its total metallization.


Wire bond


Figure 9 The bond of the gold wire is even much thicker than the pads. The dashed line encloses the area of fig.8.


Therefore, selectivity and uniformity are required to a superior level. Moreover, based on the difficulties of the other Au removal methods (cyanides are poisonous, mercury is polluting, aqua regia is dangerous to handle), if anything new can be invented, it should be highly appreciated if safe for both operators and environment, and easily handled.


The Epta-Me-2I2 Etch


The new etch [2] is based on the bis-diiodine adduct of


N,N’-dimethylperhydrodiazepine-2,3-dithione,shortly indicated as D.2I2, where D stands for the eptamethyl (Epta-Me) donor , prepared by mixing D and I2 in a 1:2 molar ratio in CHCl3 at room temperature and allowing slow evaporation to obtain orange-brown shiny crystals.


Both Tetra-Hydro-Furane (THF) and acetone can be used as solvents for the Epta-me-2I2 crystals.


The solution in THF (concentration tested from


2.1x10-3 M to 4.3x10-3 M) has a red-orange color which turns into red-brown as gold powder is added,and after relatively short time, the powder disappears.


This reaction is performed under mild conditions and without any protection against air and/or moisture.


This should be compared with other reagents which operate with polluting materials, or require strictly anhydrous and anaerobic conditions, or require long reaction times, which in turn display poor uniformity on extended surfaces.


When the solution is allowed to evaporate, well shaped [AuDI2]I3 crystals appear, as the result of the reaction scheme of Figure 10. The square-planar configuration of the gold atom well fits the bond distances offered by the sulfur atoms of N,N’-Dimethylperhydrodiazepine-2,3-dithione, which acts as an S,S-chelating ligand.


In Epta-me-2I2, the oxidation potential displayed by the Epta-Me ion is high enough to allow oxidation of many noble metals (Cu, Ag, Ni, Pd, Au).


Nevertheless, it is not sufficient to achieve Pt oxidation. This is the basis for selective etching of Au towards Pt, which holds even at high temperature along many days of reaction.


Figure 10 Reaction scheme for the new etch.


crystal


Si3N4 Au


Pt


500 nm


Application to Aged Devices


There is a big difference between the chemical tests on Au powder and the effective work to be done in the case of aged devices. In this case, in fact, grain distribution of the film, its surface contamination, its shape and the presence of possible other materials to be preserved, in particular the Au thick bonding pads and the connecting wires, are all further complications to be faced to check the effectiveness of the etch.


Many considerations suggest that the new etch could work: #1) Its solvent is a good cleaner for surface contamination coming from the test environment,which is not the case for the other etches. #2) The observed reactivity on powder indicates that the crystal structure may be of minor concern. It could be expected that the main factor in defining the reaction time is the thickness of the gold layer. In this case, the careful control of the etch time should allow complete removal of gold from the Pt barrier while merely thinning the Au bond pads and the wires, which would preserve the electrical continuity. #3) Both preparation and use are cheap and not critical, are safe to the operator and non- polluting, which can make the difference for a good success of the method.


An optical microscope is sufficient to detect the accomplishment of gold removal from the stripe, by observing its reflected color and its cleanness(Figure 11).


Figure 11 Optical micrographs of an aged laser diode before (upper) and after (lower) gold removal from the ridge area. Cleanness of the surface is achieved at complete Au dissolution.


The etch time for cleaning the Pt surface, at 25°C and continuous agitation, ranges from 5 to 10 minutes as


the concentration is diluted from 4.3x10-3 M to


2.1x10-3 M.


The removed gold thickness is about 0.5 µm, less by far than the thickness of both the bond pads (about 3


µm) and the wires.


In ideal conditions, the electrical continuity is preserved.


Some trouble is given by the reflow of the mirror dielectric coating, which masks the surface of the ridge for some ten micrometers at its edges, as yet revealed in the previous optical micrographs, and more detailed in Fig.12.


The residual dielectric layer is visible (refer back to fig.7) and is very thin. It is likely to be mechanically weak, and crack at the chip edge, and at the ridge corners. This allows slow but significant etchant penetration, which should ultimately lift off the layer,and clean that part of the Pt surface. Nevertheless,the groove of the gold grains in the thick bond pads suggest avoiding this long etch time, in order to preserve electrical continuity.


The most convincing demonstration of the effectiveness of the new etch comes from the inspection of the exposed Pt surface.


Fig. 13 shows the regular surface, while fig.14 reveals a crack, running parallel to the bottom edge of the contact, perfectly matching the faint crack image of the TEM cross section in fig.4, whose existence here is definitely stated.


10 µm


Figure 12 Exposed Pt on the ridge is indicated by the clean surface, even at SEM imaging, while the


enhanced grain structure of the bond pads revealed an


incomplete Au etch, as required. Residual mirror


coating masked the reaction on the right side.


Figure 13 (at bottom left) SEM image of the regular Pt surface on the top of the ridge.


Figure 14 A Pt crack is revealed on the Pt surface.


The new Epta-Me-2I2 etch has been considered for deprocessing gold-based metallizations in GaAs based devices.


It has proven effective, uniform, selective even towards Platinum, easy to handle, safe and not polluting.


Its potential applications in microelectronics may easily be extended to processing.


Further refinements will test the etch in inexpensive acetone solvent, and will also study the possibility of trimming its action selectively towards the other noble metal of the considered technologies, in particular Platinum.


1) M. Vanzi, A. Bonfiglio, P. Salaris, P. Deplano,E.F. Trogu, A. Serpe, G. Salmini, R. De Palo:


“Gold removal in Failure Analysis of GaAsbased laser diodes”, in press on Microel.Reliab,


2) F. Bigoli, P. Deplano, M.L. Mercuri, M.A.


Pellinghelli, G. Pintus, A. Serpe and E.F. Trogu:“A powerful new oxidation agent towards metallic gold powder”, Chem.Commun, 1998,pp.2351-2352.


Electronic Device Failure Analysis Society, editor, p 217-223


DOI: 10.1361/cp1999istfa217


# Nondestructive Detection of Cracks in Ceramics Using Vicinal Illumination


Nondestructive Detection of Cracks in Ceramics Using Vicinal Illumination


Scott Hull


NASA / Goddard Space Flight Center, Greenbelt, Maryland


Cracks and other defects in ceramic materials can be difficult or impossible to examine and photograph due to the extreme lack of contrast. A method for inspecting translucent ceramics using scattered light,also known as vicinal illumination, will be described.


This method has been known in the ceramics industry for quite some time, but is not well known in the testing and failure analysis community. Electronics applications include substrates, packages, multilayer capacitors, and thin film resistors.


Ceramic materials are used in electronic applications as microcircuit packages and substrates which carry signals and power between microcircuits. Fine cracks in ceramic materials can result in mechanical failures,electrical failures, and loss of hermeticity. Often, fine cracks are difficult or impossible to detect using standard nondestructive inspection techniques such as visual inspection, ultrasonic inspection, or vapor crack detection. Dye penetrant inspection is usually effective, but contaminates the part, which is unacceptable for space flight hardware.


One effective nondestructive inspection method of detecting cracks involves examining the way in which light scatters through the ceramic material when viewed with a standard bright field reflected light microscope.


This method, termed vicinal illumination, has been used for detecting cracks during failure analyses of several part types, and screening of space flight hardware. The technique has proven effective on several different types of ceramic materials as well. A related method for use with dark field equipment has also been used to successfully locate otherwise invisible cracks.


Cracks in ceramic devices can cause degradation of their performance, or even catastrophic failure in some applications. Nearly invisible microcracks can propagate under stress, resulting in mechanical failure. For this reason, in critical applications it is imperative that such cracks be detected prior to use.


Several techniques are available to locate and characterize cracks in ceramic materials. Each has advantages and limitations which can affect the choice of the optimum inspection method for a given application.


Visual examination is usually performed on ceramic materials at some time during their manufacture or use. A large crack which significantly displaces the surface of the part will probably be detected at that time. Visual inspection is fast and inexpensive, but small cracks may go undetected. One way to enhance visual inspection is to spray a relatively expensive inert fluorocarbon vapor over the ceramic surface.


The fluorocarbon seeps into any cracks in the surface,and retains a shiny appearance after the remainder of the fluorocarbon evaporates. This method is capable of pointing out small cracks more effectively than a simple visual inspection, but requires a skilled operator to interpret the various defect indications.


A similar technique uses a dye to penetrate into cracks and clearly indicate their location. Dyes are available which are visible using either white or ultraviolet light. Dye penetrant inspection is among the most effective and widely used techniques for detecting cracks, but it requires that the part be contaminated with a dye which may not be entirely removed.


X-ray radiography and acoustic microscopy have also been suggested as crack detection methods for ceramic materials. Radiography is not successful for crack detection unless the crack is parallel to the xrays, and exhibits an appreciable gap. Since this is not usually the case for cracks in ceramics, this method is rarely useful. Acoustic microscopy (also known as ultrasonic inspection or C-SAM) has been used to detect known cracks in laboratory samples with some success. This method, however, is limited by the necessity of immersing the part in water and by the rather time consuming inspection process. A crack could also be overlooked easily using acoustic microscopy, due to difficult gating issues and spurious signals from echoes in the part.


One effective non-invasive method of optical crack detection involves introducing light into the sample and observing the way in which the light scatters through the ceramic material. Ceramicists have reportedly used this technique to observe cracks in research samples for many years1, but the technique is not widely used in testing and failure analysis. The technique has been referred to as "vicinal illumination" because the sample is illuminated near,but not directly onto the area of interest. 2 Because it is totally nondestructive, this method can be used for screening, quality control, and failure analysis. The technique is nearly as fast as visual inspection, and requires little or no sample preparation. Operators can be taught to perform this technique in minutes using a standard bright field microscope. The main limitation to the usefulness of the light scattering inspection method is that the material must be inherently translucent.


In vicinal illumination, light is refracted into the sample in a small area, and scatters outward in all directions. If the light encounters a crack, the majority is reflected back toward the source, and very little is transmitted across the crack. This causes a high contrast delineation between bright and dark areas at a crack surface.


Material properties


Light scattering inspection has been used successfully on several different types of translucent materials.


The important factor is the ability of the material to scatter light uniformly. As a rule of thumb, vicinal illumination inspection can be performed successfully


on materials similar to a business card in translucence. Grain size, material composition,additives, porosity, and surface finish all can affect the light scattering ability of the material.


Quantifying this property is difficult, since no standard measures of light scattering or translucency of ceramic materials seems readily available.1 In an attempt to quantify the differences between the light scattering capacity of different materials, the percent transmission of white light through samples of different materials was measured. From this data and the sample thickness, an absorption coefficient can be computed for each material using the formula:


αχ


0ll


ln


where l/l0 is the ratio of light transmitted through the sample, χ is the sample thickness, and α is the absorption coefficient. 3


The light transmission properties of several samples of typical ceramic materials were measured using a visible light 630 nm laser and a power meter. The results are shown in Table 1. The lack of homogeneity in the samples and the effect of thickness is clear from these measurements. For instance, the measurements for aluminum oxide varied inversely with sample thickness. It is believed that thinner samples exhibited more internal reflection, scattering the light further from the source, outside the power meter window area. The inherent material properties such as grain size and density also induced some variation in the data.


In general, light scattering inspection is successful for materials with an absorption coefficient of 40 to 200.


In the case of a transparent material, light is transmitted through the material, and is not refracted sufficiently to scatter to the sides. Dark field light scattering works well for the more transparent materials (absorption coefficient of approximately 50 to 100). Bright field inspection can be used with the more transparent materials as well, but the dark field technique is preferred due to simpler setup and faster inspection. Materials with an absorption coefficient of 100 to 200 are best inspected using the bright field technique. An opaque material such as a business card reflects and absorbs the light as it enters the material, preventing it from scattering.


Table 1 Absorption coefficient for several ceramic materials.


Material


Thickness


α (inch-1)


Preferred Vicinal Inspection Method


Glass Slide


0.038


Not Applicable to Transparent Samples


Aluminum Nitride


0.054


73


Dark Field


0.104


45


0.107


56


Aluminum Oxide 96%


0.025


167


Bright Field


Aluminum Oxide 99.5%


0.026


182


0.042


121


0.122


51


Business Card


0.011


535


Compare signals are simpler than driven signals.


Compare signals are either strobes, in which the comparison is made within a very small unit of time,or a window in which the comparison is made throughout a large unit of time. The strobe and window offsets are specified in the edgeset.


Requirements for a Test Pattern Translation System


We developed a test pattern translation system around the following requirements.


Once translated, the test patterns must validly stimulate the device. Bench top testers, because they are an inexpensive solution for the FA lab, do not offer the same features as production models.


Therefore, a direct translation of file formats is not possible, because the production test may make use of its enhanced features. Typically, these enhanced


features are timing related or opcode related. Our system had to consider the reduced feature set of the bench top tester.


The test patterns must be as similar as possible to the original production patterns. This requirement,in contradiction to the first requirement, is what makes the translation complicated. The reduced timing capabilities of the bench top require the system to adjust the timing in the vectors without violating set up and hold times.


The system should require little engineering effort. Our previous attempts at test pattern translation for bench top testers required a large amount of engineering effort. The system was not automated, because all the timing information from the production patterns had to be discarded, in order to build patterns that would function with the limited timing capabilities of the bench top tester. Instead of discarding the original timing information, our test translation system had to modify it to meet the requirements of the bench top tester.


Overall Design


The system is made up of three components. The first component, ATE-SIM, reads the files from the production ATE equipment and translates the pattern into an events format, described below. The second component, TIMING, reads the output of ATE-SIM and a setup file and modifies the timing in the pattern to fit the constraints of the bench top tester. The final program, FORMAT-BT, formats the output of TIMING into a readable file for the bench top tester.


Design of ATE-SIM


The purpose of ATE-SIM is to translate the production test files into a format that describes the driven and compared values at each device pin with respect to time.


For example, if ATE-SIM reads the following from the production test files,


Pattern File


Vector 0: Drive ADDR_BUS to hex 5 with edgeset ES1.


Vector 1: Drive ADDR_BUS to 0, with edgeset ES1.


Edgeset File


ES1: The length (the period) of ES1 is 40ns.


ADDR_BUS is a NR signal, with an offset at 10ns.


Pin File (describes pin groupings)


ADDR_BUS is a bus made up of four pins: A3,A2, A1, A0


Then it will generate an events format output that has a time-stamped vector every time a signal changes,


10ns: A3=0, A2=1, A1=0, A0=1.


50ns: A2=0, A0=0


That is, at 10ns, "5" will be driven onto the pins that define ADDR_BUS. At 50ns (40ns edgeset period +10ns offset), "0" is driven onto ADDR_BUS.


Because A3 and A1 are already 0, no transitions are defined at 50ns. The output file only contains 1-to-0 and 0-to-1 transitions.


ATE-SIM follows several steps to translate the production files into an events format, as described below:


1. The production files are read in and parsed.


Irrelevant data is discarded. Relevant data is translated into data structures to be used by ATE-SIM.


2. A trigger channel is added to the internal data structures. We use one channel of the bench top tester to trigger the oscilloscope. This step inserts that channel into the test.


3. The edgesets are scaled to a new clock period, if desired.


4. The edgesets are simplified to account for some of the features not present in the bench top tester.


For example, RC signals -- signals that are surrounded with their complement -- can be converted to non-return signals if the bench top tester does not support RC. Simplifications that change the shape of the signal are done here,because unimportant shapes can be ignored.


Typically, RC is used on a bus to force the entire bus to switch, but the actual complement data is unimportant to the device operation.


5. A cable delay can be added to the edgeset data structures to account for the finite signal propagation time in the bench top tester's cable system. If it takes 5ns for the system clock edge to propagate down the cable, and 5ns for a response to return, then ATE-SIM can delay all compares by 10ns. However, compares that get pushed past the end of an edgeset may have to be eliminated, so they don't overtake a drive in the next vector.


6. Finally, the simulation starts. Starting at the beginning of the test pattern file, each vector is applied to its edgeset in turn. The edgeset and the vector together define a waveform for each pin during that vector, which is written to the output events file. Meaningless events, like a 1 transitioning to a 1, are eliminated so only 1-to-0


and 0-to-1 edges are written to the file. The next vector to apply is determined by the opcodes.


Some if-then conditions may not be testable in simulation, so a default choice is applied. The simulation stops under the same conditions that cause the production tester to stop.


Design of TIMING


TIMING reads the waveforms that are generated from ATE-SIM and moves the edges on the waveforms so they solve three conflicting goals:


1. The edges must fall within the timing constraints of the bench top tester.


2. The waveforms must be as close as possible to the original waveforms.


3. The device's setup and hold times must not be violated.


Our bench top tester's timing constraints include:


1. The maximum vector frequency is 25MHz.


2. Only one edgeset is allowed per pattern.


3. All signals within a group of signals must have the same timing and edge shape.


4. Drive signals can only be NR, R0, R1 or returnto-inhibit.


5. Compare strobes are allowed. Compare windows are not allowed.


6. In the one edgeset, only 12 unique drive edge offsets and four unique compare edge offsets are allowed. These are called “timing generators,”and can be assigned as the leading or trailing drive edge or compare strobe of any signal. The timing generators define the offset of the edge within the vector.


TIMING requires three inputs:


1. The test pattern represented in an event format as generated by ATE-SIM.


2. The period and name(s) of the system clock(s).


3. The signal grouping information from the original production test files.


TIMING consists of five steps. Steps 1 and 2 process the input data and extract the relevant timing from the output of ATE-SIM. Steps 3 and 4 set up and perform


the simulated annealing optimization algorithm [1],which solves a set of discretized simultaneous equations to find the best edgeset possible. Finally,step 5 post-processes the vectors and writes out the data.


Step 1: One Edge per Clock. In a typical microprocessor, the system clock is the highest frequency signal because it is the reference for the other inputs and outputs. To most efficiently use the limited vector frequency of the bench top tester, this system clock is assigned as a R0 or R1 edge shape, so the system clock period is equal to the vector period.


Any other signals operating at less than the system clock frequency can be the NR edge shape.


Step 1 of TIMING cyclizes the event format test pattern file into cycles of the clock period. These rules are applied to each signal in each cycle:


1. If more than one drive edge exists in a cycle,eliminate all but the last drive edge.


2. If a compare window exists in a cycle, or if more than one compare exists in a cycle, eliminate all but a strobe at the beginning of the first compare.


3. If both drive edges and compare edges exist in a cycle, eliminate all but the last drive edge.


At first glance, these rules would seem to violate the integrity of the pattern. In most cases, however, they do not. First, because ATE-SIM has done a simplification of its own (converting RC to NR), many signals already are simplified to one edge per clock.


Second, compares can be eliminated without changing the state of the device under test.


The following pseudocode listing details step 1:


For each event-driven vector V


Cycle = int(timestamp of V /


clock period)


Offset = (timestamp of V / clock


period) - Cycle


Append V to cycle CCycle with


offset Offset


For each cycle Ci


Apply rules (1)-(3) of step 1


above


Step 2: Get Edgesets. The cycles that were found in step 1 contain both edge timing information as well as the value to which the edge transitions. Step 2 of TIMING extracts only the timing information from those cycles by classifying each cycle into a set of single-clock edgesets. Because of the bench top tester's constraint (3), the timing of an entire signal group is extracted, rather than the timing of individual signals.


An edgeset E1 contains a set of (signal group, edge timing) pairs, describing the timing of the edges of each signal within a cycle C1. The systems clocks are not included in the edgeset. The following pseudocode listing details step 2:


Create an empty set of edgesets, E For each cycle Ci


Create a new edgeset etmp from Ci If the (signal group, edge


timing) pairs in etmp is a


significant subset of any


edgesets in the collection of


edgesets E,


Destroy etmp


Associate the similar edgeset es with Ci


Else


Add etmp to the collection of edgesets E


Associate Ci with etmp.


Step 3: Compute Cost Functions. As our bench top tester constraint (2) describes, only one edgeset is allowed for the entire pattern. This edgeset is defined as the “best” edgeset, as compared to the edgesets in E from step 2. The comparison between the "best"edgeset and the edgesets in E is made with a cost function. which is applied in step 4 while computing the best edge set with the simulated annealing algorithm.


Each of the edgesets found in step 2 defines a timeordered list of signal edges O1-On. The best edgeset that TIMING finds is one that fits the following conditions.


1. The offset of each edge is as close as possible to the original offsets.


2. The order of the edges is as similar as possible to the original order.


The cost function is built based on three assumptions about the relationships of the edges in each edgeset.


1. The first edge in an edgeset should remain at its original offset.


2. The difference between a compare offset and the previous drive edge offset should remain unchanged.


3. The difference between a drive edge offset and the previous drive edge offset should remain unchanged.


The cost function sums the energy stored in algorithmic springs attached between the edges in each edgeset in E. The relationships above determine which edge pairs get springs. The energy in a spring is defined as


Energy = k x2


where k is the spring constant (including the factor of 1/2 that is usually separated from k) and x is the displacement from the rest position. If the best edge set contains the exact same edge relationships as the edgesets in E (an ideal, but unlikely solution) the


total energy is zero because none of the springs are stretched or compressed. Any difference between the best edgeset and E creates tension and compression in the springs, and raises the total system energy.


TIMING further assumes that the edgesets in E are minimum setup and hold times, so it influences the solution to maintain at least these minimums by increasing the spring constant k if the difference in two edge offsets becomes less than its original offset.


The cost function computed is a set F of tuples(signalA, signalB, difference, kLess, kGreater).


The following psuedocode listing details step 4:


For each edgeset ei in E


Get the ordered list of edges O1-


On in ei


Set inputEdge to null


For each signal edge Oi with


If inputEdge is null


Add (Oi, Oi, Offset, 1, 1)to F


Add (Oi, inputEdge, OffsetinputEdgeOffset, 10, 1)to F


If Oi is an input signal


Set inputEdge to Oi


Set inputEdgeOffset to Offset


Step 4: Compute the Best Edgeset. Step 5 applies the simulated annealing algorithm [1] to find the best edge set, given the bench top tester constraints and the cost function F.


The following pseudo listing details step 5.


For each of the 12 drive timing generators DGi


Choose a random value less than


or equal to the clock period


for DGi


For each of the 4 compare timing generators CGi


for CGi


For every signal group in the best edge set Ebest


Choose a random drive and/or


compare timing generator to


attach to it


Apply the simulated annealing algorithm to minimize the total energy of Ebest. Each iteration,choose a random timing generator or a random signal group to randomly modify.


To compute the energy Etotal in the Ebest,


Set Etotal to 0


For each member (signalA, signalB,difference, kLess, kMore) of the cost function set F,


If signalA and signalB are


equivalent


Add kLess*(difference - offset of signalA in Ebest)2to Etotal


NewDifference = (SignalA offset in Ebest - SignalB offset in Ebest)


If (NewDifference <difference)


Add kLess*(NewDifferencedifference)2to Etotal Else


Add kMore*(NewDifferencedifference)2to Etotal


Step 5: Write Output File. Step 5, the final step,writes the edgeset and vectors in an appropriate syntax for the translation to the bench top tester format with FORMAT-BT.


Design of FORMAT-BT


Compared to the other tools, FORMAT-BT is relatively simple. It reads the output of TIMING and translates it into a binary format that is directly read by the bench top tester. FORMAT-BT compresses vectors by looking for repeated sequences of vectors and rolling them into a loop.


Results and Conclusions


This vector translation package has been very effective in our lab for translating arbitrary functional final test patterns to run on the lab's bench top tester.


Occasionally, some hand manipulation is required to fix compare timings, which is a very simple task.


Less often, the resulting drive timings do violate the specifications, which put the device into an invalid state. When this occurs, an engineer familiar with the device must debug the test.


The author would like to thank Feng Lu (formerly of Motorola) and Anthony Blakely (Motorola) for developing a script that makes these tools easy to use,and for extensively testing these tools.


1) Press, William H. Numerical Recipes in C. 2nd ed. Cambridge University Press, 1992.


Electronic Device Failure Analysis Society, editor, p 203-207


DOI: 10.1361/cp1999istfa203


# FMECA Modeling - A New Approach


FMECA Modeling - A New Approach


Yizhak Bot


BQR Reliability Engineering Ltd. Israel


FMECA tools must be included into the designers tools suite in order to support the new vision for a concurrent engineering environment. To support this new vision we introduce a major enhancement to the Failure Mode Effects and Criticality Analysis (FMECA) to provide a more accurate, simpler, accessible and frequently used computerized analysis tool. We introduce new terminology to enhance the well-known standards,while assuring their full support. Using the new terminology, functional trees become very similar to the project trees and can be drawn as block diagrams, e.g.


the time spent on constructing the functional trees is reduced by factors.


FMECA is used to analyze systems assemblies failure mode effects on the overall system functionality (endeffects). The FMECA results serve as the main input to define Built In Tests (BIT) that can automatically detect and isolate system failures as they occur and act as required to increase system availability.


FMECA is also serves as a dictionary of failure modes for safety and logistics analysis.


In this article we present a new approach to the FMECA algorithm. The basis for this new approach is two-folded:


Introducing new FMECA terms: "Good Modes©"(GM©) and "Next Brother Effects©" (NBE©).


Binding together the system Reliability Block Diagram (RBD) and the FMECA analysis. In order to do so, we use an innovative algorithm for virtual dynamic functional trees. This computerized algorithm automatically constructs a separate functional tree for each failure mode.


These terms lead to a much more flexible computerized failure modes analysis tool mechanism and (most important) BIT definitions enhancement, which increase systems reliability, safety and supportability and shortens maintenance times.


Objective


• Solving FMECA standards draw-backs


• Offering new FMECA approach


• Enhancing systems reliability and availability via


BIT enhancement


• To develop a data base of Failure Modes and


Effect with a criticality number to be used by


Safety analysis


Supportability analysis


• To develop the new advanced FMECA integrated


CARE® (Computer Aided Reliability Engineering)


software tool.


The Traditional FMECA Problem


Traditionally, the FMECA is performed using the systems’ functional tree. This tree represents signals/data flow from the lowest level functional block(a leaf) up through its higher level functional blocks,using the Next Higher Effect (NHE) term.


The existing standards approach draw-back is clearly apparent in the new high-tech ASICs, mainly CPUs,where each component fulfills a large set of functions,which are not related directly. The only reasons for including them into a single ASIC are space and cost.


For example there are micro-controllers that include Communication, Chip select and I/O mechanisms where in case one of them fails, the other may be fully operational.


To better visualize the problem, consider the project tree presented in Figure 1-A. Assume the ASIC fulfills two functions (A and B) where failure of function A affects function 1.1 and failure of function B affects function 1.2. The functional tree for this case is as presented in Figure 1-B.


The ASIC failure rate can be predicted by any prediction method. The rate of function A failure is the multiplication of the ASIC failure rate by a user defined ratio αA. The rate of function B failure is the


multiplication of the ASIC failure rate by a user defined ratio αB. The α’s sum should never exceed 1,


because the functions total failure rate can not exceed the ASIC failure rate.


The traditional FMECA tools support such a case by forcing the analyst to create the split ASIC tree as


described in figure 2-B and remember all of the α’s in order to make sure their sum does not exceed 1. In


cases where there are many sub functions, the α’s handling becomes impossible to maintain.


Converting Raw Images to Temperature Distributions


It is not possible to measure with absolute precision the radiation emitted from a surface, and real surfaces are not blackbodies, so in order to convert intensity to temperature it is necessary to generate a calibration


Focal plane array


Bond pads


curve. For this work, calibration curves for both lenses were generated by raising the temperature of the hot chuck and recording an image at each temperature, with no current passing through the device. The intensity at each temperature was averaged over the central 25% of the image. A typical calibration curve is shown in Figure 7.


Figure 7 Typical Calibration Curve.


Results & Discussion


Using these calibration curves, the temperature of the


bolometer membrane was calculated as a function of


power input (current x voltage), see Figure 8.


Figure 8 Dependence of temperature on power input.


The curve is not quite linear, as would be expected if the only means of heat transfer is conduction to the substrate. There are several possible reasons for this.


At low temperatures the intensity increases only very slowly with increasing temperature so there is a large potential error in the measurements. At high temperatures radiative heat transfer may play a significant part and this would lead to non-linear behaviour. Another potential cause of errors is that the thin silicon nitride membrane is partially transparent to the infrared radiation. For the calibration measurements both the membrane and the silicon behind it are at the same temperature whereas


with current flowing through the meander the silicon behind the membrane is close to ambient temperature. The effect of this would be to underestimate the temperature of the membrane with current flowing.


In order to convert a “raw” thermal image into one in which temperatures at particular locations can be determined, it is necessary to use an algorithm to convert counts per pixel to temperature and to make a correction for changes of emissivity across the sample. Temperature calibration curves can be fitted


well by an equation of the form T= AX2 + BX + C,where X = log intensity. This is the basis of the "fit"data in Figure 7. Previous experience has shown that while the use of additional polynomial terms improves the fit at the measured points, they often lead to unrealistic behaviour between the points.


Even when the whole of the scene is at a constant temperature the image may not display a uniform intensity. This is due to local variations in emissivity,surface texture and pixel to pixel variations in the gain of the infrared focal plane array. To compensate for these variations a “flat field” image was generated from the calibration image at 100°C. The flat field image is the reciprocal of the calibration image scaled to have a mean value of 1. If it can be assumed that the emissivity, local texture effect and gain at each pixel are constant for all temperatures then multiplying each image by this flat field should give a true indication of temperature. In order to obtain temperature maps this flat field correction was first applied after which the polynomial algorithm described above was used to convert intensity to temperature. Using this approach a temperature distribution across the device was obtained, see Figure 9.


110


170


190


210


0.00E+00


5.00E-04


1.00E-03


1.50E-03


2.00E-03


2.50E-03


3.00E-03


Power Input (watts)


Reflecting lens Conventional lens


Colour range 30 - 100 °C in 10 °C intervals


Figure 9 Temperature distribution over bolometer


with a current of 500 µA and voltage of 2.71 V.


Comparison of this temperature map, obtained by thermal imaging, with one generated using an Ansys finite element model [3], indicates close agreement for the temperature rise at the centre of the bolometer element. The finite element model gives a maximum


of 110°C, while thermal imaging indicates a maximum temperature of 100°C. Possible reasons for the 10°C discrepancy include:


In the finite element model:


• An underestimate of the heat transfer convection coefficient on the membrane surfaces.


• The omission of radiative heat loss.


In the thermal imaging:


• The partial transparency of the silicon nitride affecting the calibration curve.


Infrared thermal imaging has proved to be a powerful technique for the determination of thermal properties of micromachined sensors and to validate thermal models. It provides non-contact, quantitative temperature distributions with a spatial resolution of better than 3 micrometres.


1) J.P Holman, “Heat Transfer”, seventh edition.


2) A D Trigg, "The infrared photoemission microscope as a tool for semiconductor device failure analysis", Proceedings of the 6th IPFA 21 -26, 1997.


3) H S Lee, G Karunasiri, A D Trigg, U Sridhar,"Comparison of Thermal Modeling & Thermal Measurements of Infrared Microemitters", To be published.


Electronic Device Failure Analysis Society, editor, p 197-201


DOI: 10.1361/cp1999istfa197


# Automated Translation of Final Test Programs to Inexpensive FA Testers


Automated Translation of Final Test Programs to Inexpensive FA Testers


Dan Bodoh


Motorola Semiconductor Products Sector, Austin, Texas


To isolate defects in microprocessors, the failure analyst must exercise the device under the failing conditions. Exercising the device with a tester and the final test program is a natural choice. However,populating a lab with production testers can be prohibitively expensive.


Bench top testers are an inexpensive alternative. The constraints of these testers make automated test program translation tools hard or impossible to use.


In this paper, we describe an automated translation tool that approximates the original test program with very small engineering time, taking into account the target bench top tester's constraints.


The tool consists of three parts. First, the production test is simulated, creating a file that represents the waveforms an oscilloscope would see at the device pins. The second step is the most complex and unique part of the tool. It guesses the setup and hold time built into the production test, and manipulates the timing to fit within the constraints of the bench top tester. The final step reduces vector memory requirements and does the final format translation.


Definition of Tester Terms


Testers drive signals onto the pins of a device and compare the signals driven by the device to their nonfailing values. A pattern is one logical test in an entire suite of tests -- the test program.


The pattern consists of many vectors. Each vector defines the driven-to or comparison value (the 1's and 0's) of each pin of the device within a small time period -- the tester cycle or vector period. Each vector may have an attached opcode, such as a GOTO or IF… THEN, that defines the address of the next vector.


The vector defines the driven or compared values, but does not define when those values are driven or compared. This timing is defined by an edgeset,associated with the vector. The edgeset defines the shape of the signal on a pin during the vector period and the offsets of the edges in the signal shape.


Driven signals have a limited number of shapes,including non-return (NR), return-to-1 (R1), returnto-0 (R0), or return-to-complement (RC). An NR signal has at most one edge per vector. At the time offset specified by the edgeset, an NR signal transitions to the value specified in the vector.


The return-to-x signals have either zero or two edges per vector. At offset time 0 in the vector, a return-tox signal has a value of "x". At the leading edge offset, the return-to-x signal takes on the value described in the vector. At the trailing edge offset,the return-to-x value takes on the "x" value.


The field diaphragm is located such that it is focused at the sample plane. Closing the field diaphragm results in a small roughly circular area of light near the center of the field of view. It is the field diaphragm that creates the small spot of light used for vicinal illumination inspection.


Procedure


Bright field crack inspection is performed by opening the aperture diaphragm fully to maximize the light input, and closing the field diaphragm fully to create a small spot of light. Any filters between the light source and the sample should be removed if possible.


Inspection can be performed using any magnification, but a 10X objective with 10X eyepieces(final magnification of 100X) seems to be the best general starting point. The sample should be brought into focus and examined in the field of view outside the bright area. Magnification up to 500X can be used to further refine the beam size and placement relative to a suspected crack.


The sample should be examined around the entire perimeter, watching for an abrupt line of high contrast. As the sample is moved so that the light spot traverses the crack, the bright and dark areas should exchange places. It should be noted that any opaque metallization on the surface of the sample may alter the light path, and could be mistaken for a crack. Also, it can be helpful to displace the field diaphragm to the edge of the field of view, if the microscope has such an adjustment.


Dark field inspection is performed in a similar manner, but requires a more transparent sample. A high intensity concentrated light source (a fiber optic gooseneck lamp, for instance) should be positioned close to the sample, nearly perpendicular to the surface. Examination is performed using a typical low magnification (10X to 120X) stereo inspection microscope. Because dark field inspection can be performed at lower magnification, it is usually faster than the bright field technique for inspecting large samples. As with the bright field method, abrupt bright and dark contrast indicates the presence of a crack.


Case Histories


Thin Film Substrate (Figures 1, 2) 5


Electrical testing of a high frequency amplifier for use on the TOPEX satellite revealed that several thin film microwave substrates had cracked during mounting into the chassis. A nondestructive method of screening was required to ensure that the remainder of the substrates in the chassis did not contain any latent defects. Standard visual inspection was not considered reliable, and the use of dye penetrant would have contaminated the space flight hardware. A bright field microscope was fitted with a long working distance lens from a macro camera for


the inspection. A video camera and large screen television were added to reduce eye strain and allow several people to inspect the samples simultaneously.


Each of approximately one hundred substrates was inspected around the perimeter, and through the center of the substrate. No additional cracks were observed in electrically functional areas, and the amplifier was flown with a high level of confidence.


This amplifier is still in operation today.


Figure 1 An overall view of a cracked amplifier


Figure 2 A vicinal illumination close-up view of the crack indicated by the arrows.


Alumina Package (Figures 3, 4) 6


A hybrid microcircuit used in the POLAR spacecraft failed electrically during testing. The package, which was made from thick film substrate material, was inspected using bright field light scattering, which revealed a crack across one corner. This technique was also able to show the shape of the crack. From this information the crack initiation site was traced to


one of the package leads. It was subsequently discovered that moisture leaking through the crack had caused dendritic growth within the package,leading to the electrical failure. This failure was associated with a lack of hermeticity in the ceramic package.


Figure 3 An overall view of the hybrid package.


Figure 4 A vicinal illumination close-up view of the crack which resulted in a leak path. Vicinal


illumination was used to trace this crack across the entire corner of the package.


Multichip Module (Figures 5, 6)


Bright field inspection of a multichip module showed a small chip-out in one comer of an alumina substrate. The chip-out seemed to be isolated from any electrical circuitry, and not a reliability risk.


Vicinal illumination, however, revealed a crack extending from the chip-out toward an electrical connection, which could eventually result in device failure during use. The existence of this crack underscores the need for careful handling and


inspection during the processing of advanced components.


Figure 5 An overall view) of a chip-out in a


multichip module.


Figure 6 A vicinal illumination view of the same area Vicinal illumination revealed a crack extending from


the chip-out toward active circuit metallization.


Aluminum Nitride Substrate (Figure 7)


Several five inch square aluminum nitride substrates were evaluated to determine their suitability for use in multichip module packages for space flight use.


Throughout the evaluation, dark field light scattering inspection was used to determine the mechanical integrity of the samples. Following a thermal cycling test, one chip-out and several secondary cracks were observed in one comer. During subsequent tests, the status of the cracks was closely examined, and no further crack propagation was observed.


Figure 7 Dark field light scattering photograph


showing damage to the corner of an aluminum nitride substrate.


Multilayer Ceramic Capacitor (Figures 8, 9)


Multilayer ceramic chip capacitors are prone to fracture during manufacture and also during soldering operations. When such a fracture occurs across opposite plates a current leakage path can be formed,resulting in unacceptable electrical performance. The two cracks shown in this example are currently benign since one crack extends through the cover plates to a single conductor plate and the other extends through two common conductor plates. Such cracks can, however, develop into moisture leakage paths or catastrophic mechanical failures.


Figure 8 Bright field view of a multilayer ceramic capacitor.


Figure 9 Vicinal illumination view of the same


capacitor. Note the crack to the right of the light spot which was revealed only using vicinal illumination.


Thin Film Resistor ESD Damage(Figures 10, 11)


An investigation of an open circuit failure in a hybrid for the Hubble Space Telescope indicated that the resistor had failed as a result of electrostatic discharge(ESD) damage. A study was then conducted to determine the pertinent design characteristics for ESD susceptibility. In the course of this study many resistor networks using different patterns, materials,and resistance values were intentionally exposed to ESD pulses. The vicinal illumination technique was used to examine each resistor and determine the location and nature of the effect on the resistive elements. The examples shown include high voltage transverse cracks, corner cracking, and internal arcing over laser kerfs.


Figure 10 Vicinal illumination photograph showing electrostatic discharge damage on a thin film


nichrome resistor within a resistor network.


Figure 11 Vicinal illumination photograph showing


electrostatic discharge damage on a thin film


nichrome resistor within a resistor network. This damage was completely invisible using standard lighting.


The vicinal illumination technique has been successfully used to detect cracks in many types of ceramic materials. The effect of inherent material properties on the suitability of the technique has been studied and discussed. Several case histories have shown the efficiency and effectiveness of both bright field and dark field techniques used for failure analysis, screening, and routine evaluation. This inspection method has become an important tool for inspection and analysis of many ceramic materials for space flight applications.


1) M.J. Viens, Effect of microstructure on impact damage of polycrystalline alumina, University of Massachusetts, Master of Science thesis (1986).


2) V. Freschette, Personal conversation, New York College of Ceramics (1993).


3) L.H. VanVlack, “Physical Ceramics for Engineers”, Addison-Wesley, Reading, MA, p.


207 (1964)


4) D. Johnson-Walls, M.D. Drory, A.G. Evans,D.B. Marshall, and K.T Faber, Evaluation of the Reliability of Brittle Components by Thermal Stress Testing, Journal of the American Ceramic Society, Vol. 68, No. 7 (1985)


5) S. Hull and J. Evans, NASA Goddard Space Flight Center Parts Analysis Laboratory,FA00257, Greenbelt, MD (1990).


6) P.O'Shea, NASA Goddard Space Flight Center Parts Analysis Laboratory, FA31448, Greenbelt,MD (1993).


Electronic Device Failure Analysis Society, editor, p 225-229


DOI: 10.1361/cp1999istfa225


# Evacuated FM08 Fuses Carry a Sustained Arc in a Bus over 75 VDC


Evacuated FM08 Fuses Carry a Sustained Arc in a Bus over 75 VDC


H. Leidecker


NASA/Goddard Space Flight Center, Greenbelt, Maryland


J. Slonaker


Unisys/NASA GSFC Operations, Lanham, Maryland


The FM08 style fuse is specified to interrupt an overcurrent of up to 300 A in a bus of up to 125 VDC,but this applies only when its barrel is filled with air.


When placed into a space-grade vacuum, the FM08 style fuse exhausts its air within a year. Then, the probability of an enduring arc is high for all ratings when the bus is above 75 VDC, and the overcurrent is large. The arc endures until something else interrupts the current. The fuse can violently eject metal vapor or other material during the sustained arcing.


The evacuated FM08 does not develop a sustained arc when interrupted in a bus of 38 VDC or less, at least when there is little inductance in the circuit. This is consistent with its successful use in many spacecraft having buses in the range 24 to 36 volts.


The FM08 style fuse is widely used throughout the spacecraft industry. For example, there are several hundred on a typical National Aeronautics and Space Administration (NASA), Goddard Space Flight Center(GSFC) spacecraft, and there are almost a thousand on the Hubble Space Telescope. GSFC uses these fuses almost without exception in buses of nominally 28 VDC, for which the usual range is 24 to 32 VDC, with a few reaching 36 VDC. For this range of bus voltages,these fuses satisfactorily interrupt overcurrents even after many years in space.


Military standards and specifications do not address all applications in all situations. For example, the FM08 is defined by MIL-PRF-23419/8, which speaks only to behaviors in air; behaviors in a vacuum environment


are not mentioned [1]. The space community has known since about 1970 that it is necessary to derate the current ratings of the FM08 series in order to obtain


adequate mission lifetimes, especially after the fuse exhausts its internal air into a space-level vacuum.


At the beginning of this decade, Mr. Richard A.


Williams demonstrated that depressurizing a fuse of conventional design (a wire filament contained within a normally air-filled barrel) could lead to sustained arcing. He patented an alternate design[2], and described in the “prior art” section the enduring arc he observed upon overcurrenting an evacuated 10 A conventional fuse with a 17 A current in a bus of 100 VDC. He did not report his observations except in this patent, and they did not become widely known.


There are two published studies [3, 4] of enduring arcs that form when a tin whisker is shorted across 50 VDC at pressures less than 0.5 torr. In atmospheric air, tin whiskers fuse open at a current of a few milliamperes; however, at sufficiently reduced pressures, the puff of tin vapor is ionized into a plasma that evolves into an enduring arc carrying a current of hundreds of amperes.


Circumstances had acquainted us with the details


of this work [5]. Thus, when we were asked by the Canadian Space Agency in January 1999 whether the FM08 style fuse might develop an arc after becoming evacuated and then subjected to an overcurrent in the International Space Station(which uses a nominally 125 VDC bus), we responded that this was likely. We then demonstrated that sustained arcs did happen at this bus voltage for fuses evacuated to 1.0 torr, at least at large overcurrents, and published NASA Parts Advisory NA-045 (March 1999).


We carried out a second series of tests that showed that the threshold voltage for arcing was in the neighborhood of 60 to 75 VDC for fuses evacuated to 1.0 torr, at least for large overcurrents.


The purpose of this paper is to describe these on-going series of tests. The goal is to characterize the FM08 style fuse well enough to evaluate the risk (if any) when using it in busses with voltages higher than the traditional (nominal) 28 VDC.


Parts Description


Aspects of the construction of the FM08 style fuse and its behaviors are specified in MIL-PRF-23419/8. The FM08 is a fast acting, compact fuse rated for use in buses up to 125 VDC, except for the 15 A current rating which is rated for use in buses up to 32 VDC. These ratings apply only when the fuse is used in air. The FM08 is comprised of a metal filament passed through a ceramic body tube (4.8 mm long, 0.68 mm inside diameter) and wrapped around each end of the tube,with a short overhang. An end cap lead assembly (a copper lead butt-welded to a brass end cap) with a solder preform is slid over the end of the tube, trapping the wrapped–around end of the filament. The preform is melted, soldering the filament to the end cap. This ensures an electrical connection between the lead and the filament, and it weakly seals the end cap to the tube’s end. Then the assembly process is repeated at the other end. A sleeve made of irradiated polyvinylidene fluoride (Kynar) is slipped over the fuse,extending slightly beyond each end-cap. The sleeve is heated, which shrinks it tightly around the barrel and end caps, creating a seal that has sometimes been called“hermetic,” and adding mechanical support in the axial direction. See Figure 1 for a drawing of the construction of the fuse. Each candidate for FM08 status has the leak rate of this seal checked by a hot oil immersion test; however, this only demonstrates that


the leak rate is below about 10-5 atm-cc/s[6]. The volume of the barrel’s cavity is 0.0015 cc, and a leak


rate of less than 1.6×10-11 atm-cc/s is needed to maintain the cavity’s pressure above 1 torr for twenty years (a desirable design life for the fuse) in a spacevacuum environment. Analysis of the failure of three FM08 fuses used on the Solar Maximum Mission,launched in 1980, indicate that each of these fuses leaked down to a cavity pressure of some 0.1 torr in


nine to ten months, implying a leak rate of (5.1 to 5.7) ×10-10 atm-cc/s.


The material of the filament is not specified directly;however, conformance with the specified cold and hot resistances and with the specified interruption times constrains the material. The filament material is pure nickel for current ratings between 1/8 A and ½ A; an alloy of copper and silver (50% by weight) for ratings between ¾ A and 4 A, and pure copper with a silver jacket for ratings between 5 A and 15 A. Only the filament changes as the current rating changes (except that the diameter of the leads attached to the 10 A and 15 A ratings are larger).


Item Item Name Material


1 Outer Sleeve Polyvinylidene fluoride modified by radiation 2 Barrel


Ceramic (MIL-I-10, Grade L3B)


3 Filament Wire


Ni for ½ A and below,


Cu/Ag alloy ¾ to 4 A


Cu, Ag coating above 5A


4 End Cap


9010 brass alloy Au plated


5 Lead


Soft copper, Au plated


6 Solder


98% Sn, 2 % Ag (232°C)Figure 1 Schematic drawing if an FM08 fuse.


The numbered items are described above.


Experimental Procedure


We obtained FM08 fuses from space flight residuals and the commercial version of FM04(series 275) for the testing. The FM04 style is identical in construction to the FM08 fuse except that the external leads have tin plating instead of gold plating. The specifications provide for upgrading the FM04 to FM08 status when a sublot passes the extra tests called out in MIL-PRF23419/8. This had been done for some of the specimens we used.


Each fuse in the experiment was serialized and the


cold resistance at 22 to 24 °C was measured using Kelvin-style connections: the uncertainty was


typically less than 0.04 mΩ. A small hole was cut through the Kynar sleeve and the ceramic body tube using a diamond saw, so that the interior of the fuse would quickly equilibrate to the pressure of a test chamber. (We note that this also allows material to escape rapidly during arcing, and thus limits the internal pressure built up by the arcing.


In a later series of tests, we will seal the venting hole after the fuse’s barrel has been evacuated, and before arcing.) The cold resistance was remeasured and compared to the earlier values. Any fuse whose cold resistance changed by more than 3% was removed based on probable damage induced during cutting. However, a notch cut halfway through the filament of a 15 A fuse would


increase the cold resistance by only 1%; the increase is less for fuses with smaller current ratings. Using a 30 X microscope, the filament was inspected through the hole and no blade markings were noted on any of the several dozens inspected.


The fuses were placed one at a time into a chamber whose pressure could be brought to any measured pressure down to 0.5 torr. Current was provided by a stack of car batteries (each nominally 12.4 V), a bounceless switch (mercury wetted power relay), a


protection fuse (30 A slow blow ATO fuse; I2⋅t =1050 A2-s), a 5.00 mΩ current shunt, an adjustable carbon stack power resistor, and a fuse holder. Short straight lengths of heavy gauge wire were used to minimize stray inductance (measured to be less than 10 mh) and excessive resistance. The total resistance of the circuit, exclusive of the resistance of the fuse, is called the ballast resistance; it can be adjusted to be as low as 0.10


Ω. The voltage across the fuse, the voltage drop across the shunt resistor, and the voltage delivered by an active clip-on current probe were monitored using a digital oscilloscope. The equivalent circuit is shown in Figure 2.


Figure 2 Electrical schematic of the test station used to overcurrent the fuses.


The ballast resistance was set (using the adjustable carbon stack power resistor) so that the maximum current was 100 A, simulating a dead-shorted fuse. The actual current flowing through the fuse before its filament melted depended on the current rating of the fuse and on the voltage chosen for the run, and was sometimes much lower than 100 A. For example, the


cold resistance of a 1/8 A fuse is 2.1 Ω ± 10% and its hot resistance is 8.0 Ω ± 15%. Therefore, at 37.3 volts(three batteries), the maximum current available is 17 A at the start of the overcurrent, dropping to less than 4.6


A as the filament melts, when the ballast resistance


is set to its minimum value of 0.10 Ω.


The intent is to simulate a “hard short circuit”interruption within a space system. However, our present choice is not as severe as MIL-PRF-23419 specifies for the FM08 style fuse: it is specified to interrupt 300 A at 125 VDC without developing a sustained arc, without rupturing its case or spreading debris or vapor, and without restriking;further, the post-interruption resistance must


exceed 10,000 Ω.


The chamber that contained the fuse and current shunt was pumped down to a pressure of 1.0 to 1.5 torr. Throwing the bounceless switch started the test. This switch also triggered the storage oscilloscope, recording the voltage across the fuse,the voltage across the current shunt and the voltage from the current probe. A digital record was made of each run. Ten specimens were destructively tested at each voltage level.


During a normal event, a fuse will interrupt the current flow within the time listed in the MIL-PRF23419. This event was viewed as clearing by having the fuse filament heat, melt, and then vaporize in its normal time period. Normally,when overcurrent interrupts the fuse filament, an arc is formed during the vaporization of the filament, but is suppressed by the surrounding air that absorbs the heat of the arc and quenches it very rapidly. In a sustained arc situation, the arc is launched from the cathode end during the vaporization of the filament like that in the normal clearing event, however the arc remains. This arc produces and sustains a hot metal vapor plasma that increases with size as it consumes the surrounding metal. Several physical factors known to control arc formation are available voltage,internal pressure, ballast resistance, inductance,and ambient temperature.


There is always a spark whenever two currentcarrying contacts are separated in a bus exceeding 10 to 12 volts. This happens in a circuit breaker, or a relay, or a power switch, or the separating parts of the filament of a fuse. The designer works to ensure that the duration of this spark is not so long that the power that is let through the device interferes with its use. Other things being equal,the duration of the spark increases with the bus voltage, until a point is reached when the cathode develops “cathode spots,” each able to supply a current of roughly a hundred amperes so long as bus voltage is supplied and suitable material


remains at the cathode: this is a sustained arc [7,8,9].


For each of the fuses we studied, the overcurrent and the pre-arcing time for the filament to separate are


related by “I2⋅t = constant”; the value of the constant depends on the rating, and is known to within about 25% for each rating of the FM08 style fuses. See


Table 1. Any test for which the observed I2⋅t value exceeds the tabled value is carrying overcurrent for a


prolonged time, and the excess amount of I2⋅t is a direct measure of the extra energy let through. However, we are most interested in those cases in which the arcing endures until some other component interrupts the current. Then, the energy let through can reach enormous values, limited only by the robustness of the other circuit components and not by the fuse. Further,the internal arc can rupture the case of the fuse and broadcast debris and soot.


Table 1 Values of the Cold Resistance, and Values of


I2⋅t That Produce a Normal Interruption by Melting


Rated Current


(A)


Rcold±10%(mΩ)


I2⋅t(A2⋅sec)


1/8


2100


7.93 × 10-4


¼


7.84 × 10-3


3/8


420


2.12 × 10-2


½


4.62 × 10-2


¾


55.0


0.361


23.0


2.30


14.0


4.90


11.0


24.6


60.6


The voltage and current traces were used to classify each run as “no sustained arc” or as “sustained arc”.


See Table 2. Inspection shows that the probability of a sustained arc is zero for a bus voltage of 37.3 VDC.


The probability of a sustained arc is high as the bus voltage exceeds 75.0 VDC. For intermediate bus voltages, the probability scatters, and a dependence on the current rating of the fuse is apparent; still, a probability for sustained arcing of even 10% is unacceptably high for spacecraft use and this happens for the 7 A rated fuse for buses as low as 50 V.


Not Applicable to Opaque Samples


The thickness of the ceramic part also contributes to the amount of light available for inspection. Light scattered through a relatively thin sample is reflected by the back surface, resulting in increased brightness on the sample surface. Scattered light would tend to be hemispherical in a thicker sample, resulting in less usable light for crack detection. It is important to note, however, that there is sufficient light for vicinal illumination to be effective for bulk samples so long as a crack is open to the surface of the material.


Inspection applications


Light scattering inspection was most successful for white aluminum oxide electronic substrates and packages. Unfortunately, most ceramic electronic packages are made with black or purple colored materials. Additives in these materials cause them to be more opaque, and therefore difficult samples for light scattering crack detection. One of the case histories involves such a material, however.


This technique was also used to locate cracks in an aluminum nitride plate which was designed as the base of a multichip module package. Vicinal illumination also has revealed cracks in beryllium oxide substrates used in high power electronic devices. In addition, a porous silicon dioxide glass substrate used in a large charge coupled device had the ability to scatter light due to internal reflections off the voids within the material.


Vicinal illumination has been used by other investigators to confirm the location of cracks in BaTiO3 multilayer capacitors. 4 This technique has been used on capacitors for failure analysis, and also as a screening technique for cracks in the cover plates. Inspection of cracks in capacitors is most successful following metallography. The conductor plates in the capacitor act as mirrors to extend the useful inspection distance laterally.


A recent application of vicinal illumination is the detection of electrostatic discharge (ESD) damage in thin film resistors. Scattered light travels through a ceramic substrate beneath the opaque resistive trace.


If the trace contains ESD damage, the light shines up through the lightning-like damage path showing the absence of resistive material.


Microscope Setup


For the purposes of this paper, there are two basic types of reflected light microscopes; bright field and dark field. A stereo microscope that would be used for a typical low magnification visual examination uses dark field lighting to produce an image. Light is reflected off the surface of the sample from some angle other than perpendicular, and travels through the objective to the eyepieces. Dark field microscopes are often equipped with external light sources which can be positioned at any angle.


Bright field reflected light microscopy (also known as coaxial or epi illumination) requires that the light be introduced from an internal light source through a beam splitter so that the light strikes the sample normal to the surface being examined. Most bright field microscopes contain two diaphragms used mainly to reduce glare in the image. Because of their different locations in the light path, the effect of each is unique. The aperture diaphragm controls the amount of light entering the back focal plane of the objective. Closing the aperture diaphragm excessively results in a darker image and decreased resolution.


These limitations make it difficult to search for relationships in data unless they are already anticipated, or to find relationships which involve interactions between factors, e.g. process tools at different steps.


Supplier-based offerings for data storage and analysis would have evolved faster relative to internal efforts at major companies had there been more well-defined industry standards for database design, data access methods, or analytical tool capabilities. Larger


companies have been driven to create such standards internally while smaller companies have relied on piecemeal internal efforts coupled with what they perceived as the most flexible and affordable supplier based tools.


Extending Database Designs


Data from a broad array of data sources is needed to support root cause identification for reliability failures or customer returns. For analysis of reliability failures the database should store and index data from the reliability lab back through final test, assembly,wafer sort, and fab. In addition, for customer returns,the database needs to also be capable of mapping a package mark code to one or more backend lot numbers. Given a set of lot numbers from which the part(s) originated, the system needs to know the process flows those lots followed and be able to retrieve key data for all or some of the steps within these flows. For each lot and processing step, this should include the begin- and end-processing timestamps, equipment used, and any data collected.


If lot numbers change due to use of sub-lots in the back-end then the database needs to maintain traceability over the split process. In the ideal case,the reliability or failure analysis engineer could use the system to retrieve and analyze all lot history and engineering data to establish a root cause. If traced to a processing excursion, they could then determine what other lots might be in jeopardy, trace these lots forward to customer orders, and notify other effected customers.


Today very few companies have such comprehensive data environments in place with the applications capable of supporting these analyses.


Use of Data Mining


Once the data is brought together through whatever means are necessary, the analysis tools must then be capable of finding patterns in the data to explain observed behaviors. The process of finding hidden patterns in data to help explain the behavior of one or more response variables is called data mining [2-4]. It differs from other methods of modeling in that there is no preconceived model to be tested. Rather, a model needs to be found using a pre-set range of explanatory variables. In general these variables may have a variety of different data-types and include outliers and missing data. Some of the variables to be included in the model may be highly correlated and the underlying relationships may be non-linear and include interactions.


In all cases we are seeking methods to automatically search for structure in the data. Without such capabilities the engineer is doomed to viewing endless lists of trend charts and scatter plots to look for relationships. Success in this process relies on being able to page quickly through the plots, having sufficient time to view all of the charts, and maintaining lots of patience. With luck a relationship is found, it is shared with the cognizant process engineers, and evaluated as either root cause or a dead end.


Defined as above in this broad fashion, data mining can be performed using a number of analytical techniques. Some of these techniques involve the use of traditional statistics, while others employ more exotic techniques such as neural nets, association rules, and decision trees. We’ll look at each of these techniques individually. In all cases we are seeking to establish a model to explain the variation of a response across a set of observations together with the ability to accurately predict the response for new data we may encounter.


Statistical Methods employ such tried and true techniques as ANOVA, regressions, and contingency analyses. In using these techniques you must have a model or class of models in mind and create programs that evaluate each model across one or more ranges of the explanatory variables. The success of such efforts depends on picking the right class of models to fit.


For instance, if the true behavior is quadratic and you develop an automated routine to search for a linear model then the fit and predictive power could be poor.


Neural nets offer the opportunity to create a model using technology similar to the learning patterns of the human brain. A neural net model consists of a network of nodes on input and output layers separated by one of more hidden layers. Each input and output layer node is associated with a variable in the dataset.


Nodes have connections to all nodes in adjacent layers. Response functions on each hidden layer node determine how a signal from the input direction is propagated to nodes in the output direction. The network is trained by adjusting the weights on the hidden layer nodes to minimize the error in the outputs across a set of training data. The trained network can then be used to make predictions for new data. This method of use is called supervised learning. It has been shown that under certain conditions a model with a single hidden layer is equivalent to multiple linear regression. Neural net models are useful when large amounts of data need to be modeled and a physical model is not known well enough to use statistical methods. One of the


downsides of the approach is that it is difficult to make a physical interpretation of the model parameters. Also, the predicted outcomes of the model are limited to the scope of the training set used. In that sense it is not able to discover any new relationships in the data and hence is not really data mining.


Association Rules is a tool used to look for patterns of coincidence in data. For instance, how often do failing lots go through various combinations of deposition and etcher combinations. In it’s simplest form this is the same as a contingency table. In more advanced forms the order with which events occur is also taken into account. For example, how often do failing lots go through two reworks at first metal and are then etched on a certain etcher. Association rule analysis is useful in discovering patterns of behavior but does not produce a predictive model.


Decision Trees are analytical tools for developing hierarchical models of behavior. The tree is built by iteratively evaluating which variable explains the most variability of the response based on the best rule involving the variable. Classes of rules include linear models, binary partitions, and classification groups.


Other classes of models could also be considered. A binary partition of a continuous variable would be of the form: ‘If e-test variable T1234 < 1.23e-5’. Such a rule would partition the data into two groups, one group for which the rule is true and another for which it is false. The root node of the tree involves a rule that explains the most variability of the response. The child nodes are built by finding other variables that explain the most variability of the data subsetted by the first node, etc. The process stops when a point of diminishing returns is reached in a manner similar to automated step-wise regression procedures. Decision trees are useful when the relationships are not known and when you need to make broad categorical classifications or predictions. They are less useful when you need to make precise predictions for a continuous variable.


Overall, decision trees offer the most power in detecting hidden trends in data, in being most physical, and in offering the predictive capability needed to understand patterns of behavior. For this reason we proceed further in the current discussion using decision trees as the reference data mining method.


Relation to Knowledge-Based Systems


We will now look at the relationship between decision trees and knowledge-based systems such as expert systems, signature analysis, and classification trees.


Expert systems provide the capability to create hierarchical knowledge systems given a set of rules.


The systems generally guide a user through a decision making or diagnostic process. Data mining using decision trees provides another method of deriving rules upon which expert systems are built.


Signature analysis is a form of expert system that is specifically designed to assimilate clues associated with diagnostic data to fingerprint a process failure.


Here again, decision trees can help to discover patterns that associate a given failure with a set of process conditions. Once associations are known they can be applied to new data through signature analysis to implicate likely process conditions that led to the failure. In a similar manner, historical data could be used to derive rules for suggesting next steps in a failure analysis given the results obtained thus far.


Classification trees are a special case of decision trees when the response variable is categorical. They can be built with or without the use of data mining technology if the knowledge can be obtained through other means.


Data Mining Applications


In this section we will explore how data mining using decision trees and the use of a comprehensive engineering database can be used to help solve several yield and failure analysis problems. In each case availability of a comprehensive engineering database and advanced analytical tools, such as data mining using decision trees, is crucial to the solution of a complex yield or reliability problem.


Scenario #1: a customer has returned some parts from an order due to early failure. The failure is traced to a process problem at one of the diffusion steps based on signature analysis using rules derived from a decision tree analysis of historical data. The engineering database is then used to:


1. trace the mark date code on the failed parts to a single fab lot number,


2. provide the date-time that this lot went though the suspect diffusion step and the specific furnace and tube that was used,


3. interrogate the tool event history to discover that a problem was found and fixed 2 days after that lot went through the tube,


4. provide the list of lots that went through the same tube after the failed lot but before the fix was put in place,


5. trace this list of lots forward to mark date codes and other customer orders,


This information was then communicated to the product line who drafted a communication to the other effected customers notifying them of a possible problem with their order and suggesting a recall of the effected parts.


Scenario #2: a rise in the number of early life failures across several products on the same fab technology prompts the reliability engineer to do a commonality analysis of the processing history of the failed parts. The first steps in the analysis are to use the engineering database to:


1. look up the fab lot numbers associated with the all of the parts tested on this same technology in the last 3 weeks,


2. retrieve the fab lot history and in-line data for this set of fab lots


Once this data is available data mining is performed on the dataset to discover that the rate of failure on the lots is tied to use of a specific deposition tool at either of two metalization layers within a window of process dates. The decision tree results are supported by trend charts of the failure rates versus the date through the deposition system. The decision tree results and the supporting charts were then shared with the fab engineering group for follow-up. The fab engineers use the engineering database to investigate events and comments logged to the tool history during the suspect time period in an attempt to discover clues for the window of failures. After retrieving the data and performing a brief review, they begin the analysis by using data mining to compare the tool history of the failed tool to that of other similar tools used at the same time.


Scenario #3: yield through a bond strength test is beginning to drop. The responsible engineer uses the engineering database to retrieve lot history information through assembly for all of the lots


tested in the last three weeks. This includes material batch numbers and sub-contractors used at various steps. Data mining is then used to derive a model relating the measured bond strength results on each lot to this lot history information. The decision tree shows that one of the sub-contractors is the culprit but that they are only having a problem with one of the package types. As part of an integrated analysis environment, the engineer plots out the supporting box plots and trend charts that allow the relationships shown in the decision tree to be more clearly visualized. The data and charts are then communicated to management and the subcontractor is contacted as the first step in fixing the problem.


Commercial Availability


Many companies have built portions of the capabilities described above. To be effective the engineering database must be comprehensive and integrated tightly with the engineering analysis environment. It should be able to be distributed across separate servers and physical locations. The engineering analysis environment must offer a full suite of graphics and statistics tools including such advanced technologies such as data mining. It should integrate with the engineering database and offer the user the capability of transparently retrieving data regardless of its location. It should also offer the capability of integrating with legacy systems as if they were part of the main database environment.


A wide variety of standalone data mining tools are available on the commercial market. Some are general-purpose tools and others are tailored to use in specific industries such as finance or retail. To be truly effective as a tool to improve yield and reliability, such software technology needs to be available as part of an integrated yield management software environment. Otherwise, the engineer will be faced with importing and exporting data from one tool to another depending on where they are in the analysis cycle. To achieve this ease of use, data mining needs to be available as part of a commercially acquired yield management system, or it needs to be integrated in a seem-less fashion with an in-house system. The latter case requires both a fully functional programmatic interface as well as an adequate internal staff to set-up and maintain the integration.


Today there are few commercial products that provide both the breadth of database capabilities and the advanced data analysis features we have


described, however such product offerings are beginning to emerge. Among others, Yield Dynamics has recently introduced their Genesis yield management software that incorporates a proprietary data mining module within their full product suite. In evaluating this and other offerings, care should be taken to insure that purchased products can be integrated with existing systems and there is flexibility in the hardware that can be used. Ideally, a supplier will provide a product that can be installed in such a manner so as to complement existing capabilities and provide a path for a phased migration to more complete use. Preference should also be given to those solutions that allow you to leverage hardware and software systems already in place.


Another component of the cost for new systems capabilities is that of setup and integration. Setup includes installation and configuration on the target hardware platform. Integration involves interfacing to existing data sources. Integration costs can be large if the legacy databases are varied and complex.


Availability of a high-level data integration language is desirable for maximum productivity in this effort as well as lower future maintenance costs.


Future Trends


Future work in the development of data mining software will extend options for visualization, use of alternate algorithms, and efficiency. Data mining tools will become more prevalent in yield management software. In addition, the leading yield management companies will continue to integrate in new statistical technologies and intelligent data access routines to support automated searches for more complex patterns of process variation. Scripting languages will be extended to support more sophisticated monitoring capabilities. Database offerings will provide more extensive schemas for the efficient storage and retrieval of new forms of data and images. Pre-computed summary information within the database will be more comprehensive to make certain forms of analysis both easier and more efficient. Some standards will begin to evolve driven by SEMATECH and other consortia that seek to promote open plug-and-play type architectures for yield management software. As a result of these trends, the tools available for yield and reliability analysis will improve further in capability and efficiency.


Today’s systems for the analysis of yield and reliability are emerging from an embryonic phase.


Islands of data and analysis capability are growing together through the efforts of in-house developers and emerging third party suppliers. Driving forces of more complex processes and problems that span larger regions of the process make such efforts a requirement for competitive I.C. manufacturing. Key to the development of integrated capabilities to meet these needs will be the use of a comprehensive engineering database, intelligent data access routines,and advanced statistical technology such as data mining.


Special thanks to Weidong Wang and Jon Buckheit of Yield Dynamics, Inc. for their careful reading of this manuscript and to Nick Atchison of Silicon Systems,Inc. for his encouragement on the topic.


1) W. Maly, “Testing-Based Failure Analysis: A Critical Component of the SIA Roadmap Vision”, Proc. of ISTFA 1996, pp. 3-6 (1996)


2) C. Westphal and T. Blaxton, Data Mining Solutions, John Wiley and Sons, New York(1998)


3) J. Friedman, “Data Mining and Statistics: What’s the Connection”, www-stat.stanford.edu/reports/friedman (1997)


4) G. Shapiro et. al., “An Overview of Issues in Developing Industrial Data Mining and Knowledge Discovery Applications”, Proceedings of KDD-96, pp. 89-95 (1996)


Electronic Device Failure Analysis Society, editor, p 239-244


DOI: 10.1361/cp1999istfa239


# An Application of Passive Voltage Contrast (PVC) to Failure Analysis of CMOS LSIs Using Secondary Electron Collection


An Application of Passive Voltage Contrast (PVC) to Failure Analysis of CMOS LSIs Using Secondary Electron Collection


Akira Nishikawa, Naoko I. Kato, Yoshiteru Kohno, Nobuhito Miura


ITES Co., Ltd., Shiga, Japan


Masao Shimizu


IBM Japan, Ltd., Shiga, Japan


This paper describes a method for applying passive voltage contrast (PVC) in the failure analysis of CMOS LSIs using a conventional scanning electron microscope (SEM), and demonstrates the effectiveness of this method.


It was confirmed by measurement of the stage absorption current that the combined emission efficiency of secondary and backscattered electrons from aluminum is larger than 1 at acceleration voltages lower than about 2.5 kV.


This means that local positive charges should be generated on a conductor in association with its irradiation with an electron beam at a relatively low acceleration voltage. However, a pn junction connected to the conductor would change the potential. The potential is still positive if the conductor is connected to a reverse-biased diode but becomes lower if such a diode is forward-biased. The PVC signal observed on the conductor should be defined according to the bias state of any diode connected to the conductor.


Application Results


Case 1: Open Defect in a Logic LSI


A logic LSI was determined to be the cause of an IDD (power supply current) leakage failure in a wafer-level electrical test conducted because of a yield problem.


In photo-emission analysis, observation of temporary photo-emission just after VDD application suggested


an open defect in a conductor2).


Fig. 6 shows the results of PVC observation after the passivation and interlayered dielectric films had been deprocessed by RIE. The suspicious conductor localized by photo-emission analysis has a dark contrast, confirming that there is an open defect and that the via hole indicated by arrow is open.


Figure 6 PVC observation in Case 1.


Fig. 7 shows the result of cross-sectional TEM analysis. It reveals that failure was caused by incomplete formation of the intermetallic layer between the layer metal aluminum and the liner metal titanium of the via hole material.


Figure 7 Cross-sectional TEM observation in Case 1.


Cross-sectional SEM analysis does not allow us to detect a narrow space like this. It was found that PVC observation allows detection of such a narrow spaces that can be detected only by cross-sectional TEM analysis, not by cross-sectional SEM analysis.


Case 2: Short-circuit Defect in a Memory LSI


A DRAM embedded in an LSI was detected as the cause of a single cell failure (SCF) after reliability stress testing, but the LSI tester did not localize the failure mode.


Fig. 8 shows the results of PVC observation after deprocessing to a word line (W/L). Normal W/Ls have a dark contrast, because they are isolated from the substrate by the field oxide and gate oxide as same as type a) contact and are charged positively.


But one W/L has a bright contrast, confirming that there is a leakage path from the W/L to the substrate.


Consideration of the leakage path confirmed by PVC,the address location of the SCF cell detected by the LSI tester, and the cell structure enabled us to predict the short path between the W/L and the trench capacitor in the memory cell.


Figure 8 PVC observation in Case 2.


Fig. 9 shows the result of cross-sectional TEM analysis of the predicted short path. It confirms that a void in the poly-Si in the trench capacitor caused the short-circuit defect between the W/L and the trench capacitor.


Figure 9 Cross-sectionl TEM observation in Case 2.


Case 3: Dislocation in a Projection-Type Liquid Crystal Display


A "not turn on" failure was detected in a cell of a projection-type light valve (LV) liquid crystal display during turn-on testing after assembly.


An LV has about one million identical unit cells, each of which consists of an n-MOS transistor and a reflective metal mirror connected to the drain, as in a DRAM.


Fig. 10 shows the results of PVC observation of a metal mirror after disassembly. The mirrors of the normal cells have a dark contrast, because they have a type b) contact and the np junction that is reversebiased. But the failed cell has a bright contrast,confirming that there is a leakage path in the drain.


Figure 10 PVC observation in Case 3.


Fig. 11 shows the results of cross-sectional TEM analysis of the drain contact of the failed cell. It reveals that dislocations caused the leakage. It was found that they were produced by cyclic deformation induced by the vibration during the ultrasonic cleaning after dicing.


Figure 11 Cross-sectional TEM observation in Case 3.


We have described a method for applying passive voltage contrast (PVC) in the failure analysis of CMOS LSIs, using a conventional SEM. It was confirmed that the PVC signal observed on the conductor should be defined according to the bias state of any diode connected to the conductor. Some case studies were described to demonstrate the effectiveness of combining this method with crosssectional TEM observation.


Acknowledgement


The authors wish to thank K. Nishimura, J.


Matsuzawa and K. Takagi of the ITES Semiconductor Failure Analysis Laboratory for useful support.


1) Thomas W. Lee and Dr. Seshu. Pabbisetty,Microelectronic Failure Analysis: Desk Reference 3rd editon, p 163, ASM International,Material Park, Ohio (1993)


2) Nishikawa, N. I. Kato, J. Matsuzawa, K. Takagi,N. Miura: Proc. of 24th ISTFA, pp 157-162(1998)


3) V. Liang, H. Sur, S. Bothra: Proc. of 24th ISTFA,pp 221-225 (1998)


4) H. Sur, S. Bothra, R. Lei, J. Hahn, H. J. Brugge:Proc. of 24th ISTFA, pp 273-278 (1998)


5) H. Lorenz, C. Engel: Proc. of 24th ISTFA, pp 289-295 (1998)


Electronic Device Failure Analysis Society, editor, p 247-254


DOI: 10.1361/cp1999istfa247


# Integrated Circuit Device Repair using FIB system: Tips, Tricks, and Strategies


Integrated Circuit Device Repair using FIB system:Tips, Tricks, and Strategies


K. N. Hooghan


Lucent Technologies, Allentown, Pennsylvania


K. S. Wills


Texas Instruments, Stafford, Texas


P.A. Rodriguez


Reactive Beam Technology, Lewisville, Texas


S. O’Connell


Cyrix Corp., Richardson, Texas


Device repair using Focused Ion Beam(FIB) systems has been in use for most of the last decade. Most of this has been done by people who have been essentially self-taught. The result has been a long learning curve to become proficient in device repair.


Since a great deal of the problem is that documentation on this “art form” is found in papers from many different disciplines, this work attempts to summarize all of the available information under one title.


The primary focus of FIB device repair is to ensure and maintain device integrity and subsequently retain market share while optimizing the use of the instrument, usually referred to as ‘beam time’. We describe and discuss several methods of optimizing beam time.


First, beam time should be minimized while doing on chip navigation to reach the target areas. Several different approaches are discussed: dead reckoning,3-point alignment, CAD-based navigation, and optical overlay. Second, after the repair areas are located and identified, the desired metal levels must be reached using a combination of beam currents and gas chemistries, and then filled up and strapped to make final connections. Third, cuts and cleanups must be performed as required for the final repair. We will discuss typical values of the beam currents required to maintain device integrity while concurrently optimizing repair time. Maintaining device integrity is difficult because of two potentially serious interactions of the FIB on the substrate: 1) since the beam consists of heavy metal ions (typically Gallium)the act of imaging the surface produces some physical damage; 2) the beam is positively charged and puts


some charge into the substrate, making it necessary to use great care working in and around capacitors or active areas such as transistors, in order to avoid changing the threshold voltage of the devices.


Strategies for minimizing potential damage and maximizing quality and throughput will be discussed.


Introduction and Background


FIB systems have come a long way from their original application, which was mask repair.


Presently FIB systems are used for a number of applications in the semiconductor industry, primarily in the failure analysis and device debug regimes. Due to their unique ability to cut metal lines and deposit conductors and insulators, these systems are increasingly used for repairing prototype chips, to yield the required results, prior to reworking Silicon.


In the semiconductor industry this has the greatest impact, saving the company a lot of time, money and,subsequently market share. In the highly competitive environment prevalent today, gaining and keeping market share is of utmost importance, hence the need for quick and efficient device debug at the prototype chip level.


Taking all this a step further, the next important part is being able to get a high success rate for the reworked prototypes. This is true because, despite the FIB being able to do a lot of “magic,” it does come with an attached price tag.


FIB Basics Recap.


Image Formation And Capabilities


A typical contemporary FIB system uses a Gallium Liquid Metal Ion Source (LMIS). An extractor voltage of 25 to 50 kV is applied to field ionize Gallium ions from the source. These ions are then collimated and focused using a series of electrostatic lenses, apertures (or crossovers) stigmators etc. to focus and strike the sample. Beam deflectors then help to raster the focused ion beam thus formed across the sample. Either a Multi channel Plate or a Channel electron multiplier detector, collects the secondary electrons or ions thus generated, to form an image of the surface on a screen. Proprietary software then allows one to generate patterns on the screen, thus allowing the ion beam to raster in a rather focused and concentrated manner within those patterns. Material is removed by physical sputtering of the sample surface within the pattern. Metal deposition takes place when an organometallic precursor gas is introduced near the sample surface where the beam is scanning. This is achieved by using a needle, valve, and crucible. The beam strikes loose the metal atoms from the precursor gas, and they deposit on the surface in the shape of the drawn pattern. The residual gas is pumped away. [1,2]


Beam Induced Damage


The FIB system is very similar to a scanning electron microscope (SEM) with a couple of major differences. First, the FIB system uses positively charged Ga+ ions, instead of electrons, to raster the sample surface to form an image. Secondly, the typical SEM lacks the software to generate patterns for the electron beam to raster within a drawn pattern(with the exception of script capability).


The mass of the Ga+ ion is about 125 times more than that of an electron, besides being positively charged.[3] Thus the damage inflicted upon the sample surface by the ion beam is essentially twofold. It physically sputters away more of the sample surface, (even while imaging) and pumps charge into the sample surface, which is detrimental to the devices lying below the surface. The detrimental effects on the sample surface and devices has been documented elsewhere[4,5,6] and, suffice to say, one needs to be aware of these effects and try to minimize them, while working on devices undergoing modification/repair.


Device Repair: Needs And Objectives


Needs


The need for device repair arises typically when there is a mismatch between schematics and layout, beyond those caught by schematic verification programs. This mismatch is then traced to the individual devices/components/cells etc., and a fix is proposed.


Eventually all mismatches are fixed by reworking Silicon. Unfortunately, reworking Silicon is easier said than done, in terms of time and money. Each mask change entails a processing delay of 2-3 weeks,and costs several thousands of dollars. All this time the customers are waiting for the device so they can carry out subsequent tests in their systems.


Occasionally device modifications are done to probe signals also, in order to aid in the debugging process.


Objectives


FIB systems can carry out the proposed fixes,typically within a matter of hours. The devices can then be tested for optimum performance, almost right away. Any further bugs that surface later on can be addressed the same way and fixed similarly. Many times the same chip/device can be used to carry out multiple modifications, as needed, with the primary objective being to have a functional device at the end.


This is keeping in mind the surface and subsurface damage as mentioned above. Having devices which are functionally “dead” or have significantly altered parameters, are of little use to anyone. Some of the parametric changes can be remedied but that involves additional steps and subsequently more time.[4]Hence, it augurs well for the person carrying out the repair/modification to be conservative and not try to rush getting the modification done. Optimizing the“beam time”, so as to impart minimal damage, and still carry out the modification/repair in a timely manner is the key to successful device repair.


Strategies To Achieve Objectives


The strategies for achieving the above mentioned device repair objectives are as follows:


1) Planning, 2) Sample mounting, 3) Imaging, 4)Navigating, 5) Milling vias, 6) Filling vias and depositing connections, 7) Cutting lines and 8)Cleanup of overspray.[7, 8]


1) Planning: This is by far the most important phase of a whole device repair project. The design engineers handling the project need to test the device in question, both before and after


decapsulation. This is to preclude the possibility of working on devices which are already altered or dead. Next, plots need to be generated.


Ideally, one plot of the overall chip, and plots zoomed in to the desired location are good. In addition, it would be good to have an all level metal plot of the desired location. This is highly recommended so that one knows the location of active circuitry on the levels below. It behooves both the FIB and the design engineers to sit together and discuss the proposed fixes before starting. This is to make sure that there are no metal tracks (to be deposited) that a) cross each other, and b) run over capacitors or other active devices. Observations by the authors showed evidence of damaged capacitors whenever metal tracks were laid across, or attached to capacitors directly. [8] Also, as has been mentioned earlier,FIB irradiation leads to parametric changes in transistors below the surface, and needs to be kept to a minimum. [5, 6]


This is also a good time to consider rerouting connections so as to reduce their length. Typically this could be achieved in one of two ways.


Use an existing (but preferably redundant) metal runner, which can be used to carry the connection“piggy back”. That is to say, make connections on two points on the line using the FIB, and disconnect on the outer sides of the FIB connections. One can then use the existing length of the line for reducing beam time. On the other hand, if a spare gate is far away, maybe one is available nearby to render the same result. Both these examples entail additional time spent by the designers on their layout software, but the outcomes will be a reduction in time, by at least half or more in many cases. Of course, less beam time leads to less substrate damage, and hence better chances of getting working devices at the end.


TIP: Also at this time design/FIB engineers need to gather information for navigating to the desired locations. This could be in the form of 3-point co-ordinates, CAD files and/or data-bases,etc. This is in addition to the plots mentioned earlier.


2) Sample mounting: This is essential from two


perspectives. The first being to keep the sample chip stationary on the chuck, and secondly to


ground the chip by making sure the leads touch a conductive grounded surface. This is done in


order to help dissipate a lot of the charge build up on the surface of the chip, due to beam raster and


irradiation. Also, effective grounding helps in


efficient End Point Detection (EPD).


To ensure proper grounding of the chip, a vise works very well. Standard vices are available from FIB manufacturers which clamp the chip and also ground the leads at the same time.


Another way of grounding is to use conductive metal (Al or Cu) tape to position the chip on to a metal (preferably Al) chuck, or stub. Smaller chucks or stubs are available from Electron Microscopy supply companies, larger ones(typically 3”to 6” in dia.) can be machined as per the needs of the laboratory.


TIP: On a grounded chip the bond pads light up well. [7] Also, in case charging of the sample persists, one can do either a local platinum, or a global carbon coat. The carbon thus deposited can be plasma ashed later on (please make sure to ground all leads prior to carbon coating and to remain grounded until after ashing). One can also use a low energy electron charge neutraliz-ation technique to help dissipate surface charge.


3) Imaging: Selection of imaging current depends on the surface charge induced and also the resolution. As mentioned earlier, in order to reduce charging, get better resolution, and impart minimal substrate damage, one needs to dissipate the induced surface charge. In addition to what is mentioned above one can reduce the beam current and the number of pixels to reduce charging. But one can only go so low on beam current before the yield becomes low.


TIP: Empirically, the authors have noted that using a global carbon coat, along with a beam current of about 40 pA to image gave the best results and least damage [8]


4) Navigation: This phase of the repair is next in importance only to planning. In fact, both complement each other well. Getting to the region of interest quickly can be achieved effectively by one of many methods. These being: a) dead reckoning b) 3-point align c) CAD based navigation, and d) optical overlay. [7, 8]


a) Dead Reckoning: This is just what the name suggests, getting to the region of interest using visual references. This is primarily limited to analog circuits (some digital),where one has unique circuit features, which are not readily repeated elsewhere on the chip. Figures 1.a, b, c illustrate this concept


aptly. The figures show typically how the designer goes to the region of interest and shows what needs to be done.


b) 3-point alignment: Using this navigation tool one aligns the stage to 3 user defined Cartesian co-ordinates, usually along three corners of the chip.[7] Figure 2 shows typically the points used in aligning or“mapping” the external coordinate system.


Once the alignment is done, one can move around the chip in the “user units” instead of the stage units.


Figure 1 Dead Reckoning sequence. (a) Overall chip plot, area of interest outlined. (b) blow up of outlined area. (c) X= FIB cut location, Metal 3 runs vertical,Metal 2 runs horizontal. Plots courtesy C.H. Holder,Lucent Technologies, Allentown, PA.


(d)


Figure 2 3-point align sequence. (a) overall chip outline with points marked. (b), (c), and (d) showing close-ups of individual points. All alignment points are at top level metal.


Plots courtesy R. Aguilar, Lucent Technologies, Allentown, PA.


One has to make sure that the points chosen to carry out the alignment are on top level metal, and quite distinct. Corners of power or ground buses (running around the chip)usually are easily visible and far enough away from the bond pads to do the alignment quickly. The next step would be to enter the co-ordinates for the region of interest,compare with the zoomed in plot for the same area. After identifying the lines in question, it is usually a good idea to print out the screen image, compare it with the plot and carry out the repair “on paper.” Thus one would know at that point, how the repair can be carried out at that location. In case one needs to do more than one chip this would be a good time to mark the location for realignment on the next chip, and save the printout also. [7, 8,]


Therefore, for failure analysis applications, if the bias state of a diode connected to a suspicious conductor is known, the PVC observation is useful for determining whether there is an open defect or a short-circuit defect.


Some case studies are presented to demonstrate the effectiveness of the method. Cross-sectional TEM observations of defects localized in this way are also included.


Failure analysis of CMOS LSIs plays an important role in early ramp-up of production yield,improvement of process windows, and maintainance of high yield. Quick failure analysis and rapid feedback to manufacturing process is a mandatory requirement for failure analysts, because low yield raises production costs and reduces reliability.


Many techniques have been proposed for failure analysis. Scanning electron microscopy is one of the


most popular and has been used for many years1).


When a specimen is irradiated with an electron beam,information on the specimen's surface shape,material, and so on is obtained from the detected secondary or back-scattered electrons.


During failure analysis using a conventional scanning electron microscope (SEM) for inspection, it was observed that the contrast of the metal conductor line of interest was different from that of the others, and an open defect was found in the conductor. It was inspected in non-bias application, but it had a dark contrast as if it were biased positively.


This phenomenon is called passive voltage contrast


(PVC)1-5). We consider that a local positive charge is generated by irradiation with an electron beam, and that this charge causes the contrast. This paper describes an experiment using a conventional SEM to confirm the charge-up phenomenon, and discusses a method for applying PVC to failure analysis in order to determine whether the failure mode is OPEN or SHORT. Some case studies are presented to demonstrate the effectiveness of this method.


Background


Fig. 1 shows the PVC observed during failure analysis after the passivation and interlayered dielectric films had been deprocessed by reactive ion etching (RIE). We used a Hitachi S800 as a conventional SEM and conducted observation at an acceleration voltage of 1 kV. The contrast of the conductor indicated by arrow 1 is dark, whereas all the others are bright. It seems to be biased positively.


Following the same signal line, we see that its contrast turns at the via indicated by arrow 2, where the contrast of the upper conductor is dark and that of the lower one is bright. Subsequent cross-sectional observation revealed the via hole was open.


Figure 1 Passive voltage contrast.


Fig. 2 shows a schematic illustration of the observation results. The conductor after the open defect has a dark contrast, while the one before it has a bright contast. This difference is considered to result from the charge-up induced by the electron beam.


Figure 2 Circuit diagram.


A charge-up induced by irradiation with an electron beam is defined by the relative quantities of the primary electrons and emitted secondary and backscattered electrons. It is well known that the emission efficiency of secondary electrons is higher than 1 at a


relatively low acceleration voltage1). To understand the PVC mechanism, we tried to measure the combined emission efficiency of secondary and backscattered electrons, using a conventional SEM.


Since it is difficult to measure the efficiency directly by using a commercial SEM, we focused on the stage absorption current and calculated the emission efficiency by measuring the current.


First, we connected a current meter to the terminal of the stage of a commercial SEM, then directed an electron beam onto the Faraday cup and measured the primary electron beam current (Ip) as the stage absorption current. Next, we irradiated the aluminum surface of the SEM stage with the electron beam and measured the absorption current (Ia). The difference between Ip and Ia, Ie (=Ip-Ia), means the amounts emitted as the secondary and back-scattered electrons, and the emission efficiency (E) are calculated as follows:


Ip


Ia


Ip Ie


Fig. 3 shows a schematic illustration of the experiment.


Figure 3 Experimental method


We used a Hitachi S800 as a commercial SEM and a Keithley 617 as a current meter. The SEM was set to a normal observation condition: the condenser lens column was 10, and the aperture was 4.


Currents ranging from a few pA to a few hundred pA were measured in normal observation conditions. Fig.


4 shows the results of the experiment. It was confirmed that the combined emission efficiency of secondary and back-scattered electrons from


aluminum is larger than 1 at acceleration voltages lower than about 2.5 kV.


Figure 4 Results of emission efficiency measurement.


An internal metal conductor of a CMOS LSI has a contact with the substrate somewhere in a chip. The contacts, except for the power and GND bus, are categorized into the following three types. Fig. 5 shows schematics of them.


Contact a) Input to gate conductor (terminated by gate oxide)


Contact b) Output of n-MOS transistor drain(terminated by an np junction)


Contact c) Output of p-MOS transistor drain(terminated by a pn junction)


Figure 5 Conductors’ contact with the substrate.


We now consider the contrast of a metal conductor that is assumed to have only one of the above contacts and to be irradiated by an electron beam at an acceleration voltage of 1 kV.


Previous experimental results show that the combined emission efficiency of secondary and back-scattered electrons from aluminum is larger than 1 at an acceleration voltage of 1 kV. Consequently, the potential of the conductors should become higher,because a local positive charge is generated.


However, the contacts cause the following phenomena:


Contact a) The positive charge cannot flow into the substrate, because the conductor is terminated by gate oxide, so its potential is still positive and a dark contrast is observed.


Contact b) The positive charge cannot flow into the substrate, because the conductor is terminated by a reverse-biased diode, so its potential is still positive and a dark contrast is observed.


Contact c) The positive charge flows into the substrate, because the conductor is terminated by a forward-biased diode, so its potential becomes lower and a bright contrast is observed.


Therefore, if the contact type of a suspicious conductor is known, passive voltage contrast (PVC)observation, using a conventional SEM at a relatively low acceleration voltage, can determine whether or not there is an open defect and a short-circuit defect,and localize the defect location. It is very useful for failure analysis of CMOS LSIs.


In the example in Fig. 1, the conductor before the open defect has a bright contrast, because it is connected to an output of a p-MOS transistor drain,which is a forward-biased diode, and the conductor after the open defect has a dark contrast, because it is only connected to a gate input and is charged positively. The via hole at which the PVC turns from bright to dark has an open defect.


The metal filament of the FM08 is so small, for most ratings, that the air within the barrel is enough to absorb the heat of the spark, and quench it so rapidly that there is negligible energy let through. The exception is the 15 A rating: the specification only rates this example for use in a bus of 32 VDC. The filament of this rating is large enough that internal air at a nominal one atmosphere (760 torr) is not enough to quench the spark excited by buses at above 32 VDC and below the 125 VDC rating. In previous experiments, using a 300A overcurrent value at 1 torr pressure, it was found that


three out four 15 A fuses sustained an arc using


49.7 V (4 batteries). It is no surprise that reducing this air pressure, already inadequate at 760 torr,down to the region of 1 torr, would still not quench the spark supported by this quantity of metal vapor.


Table 2 Results of the Overcurrent Testing


Rating(A)


37.3 V(3 bat)


49.7 V(4 bat)


62.0 V(5 bat)


74.4 V(6 bat)


86.8 V(7 bat)


Number of fuses that had a sustained arc in a sample of 10


NT


NT = Not tested


Conclusion and Recommendations


A soft vacuum environment (1.0 to 1.5 torr) within the FM08 style fuses has been shown to cause a sustained arc within the fuse at bus voltages of 50 VDC and above. Under a high current short situation, where a fuse could go into a sustained arc mode, damage to the fuse and surrounding mounting is probable. More importantly, the fuse will not protect the power system as intended. For many designs, the next upstream fuse will interrupt, isolating systems that should still be allowed to be powered. This problem will propagate further if the same arcing happens in that next upstream fuse. Typically, in space systems,reliability is sought from redundancy: a failed unit is cut off the bus and a working one is substituted.


This approach fails when one or more fuses develop a sustained arc, rather than interrupting per design intent, upon experiencing an overcurrent.


We believe that the successful operation of the FM08 style of fuse in GSFC spacecraft has been dependent on the use of a nominal 28 VDC bus,with the tacit voltage derating by a factor of more than four from the specified 125 VDC. Our intentions are to extend the derating criteria at GSFC for the use of this style of fuse to include the need for a voltage derating, as well as the current derating already in use.


More testing at other overcurrents, other barrel pressures, and other ambient temperatures is needed. In addition, conditions affecting “restrike” potential,including the role of inductance in the circuit, are needed.


This work has been supported by the Parts Branch at the Goddard Space Flight Center in Greenbelt Maryland. The authors appreciate the valuable assistance of Mr. Prashant Patel in the testing laboratory, and conversations with the manufacturers of this type fuse.


The authors thank Mr. Rodney Woolley (Canadian Space Agency) for bringing this problem to our attention, for pointing out Mr. Williams’ patent, and for many useful discussions.


1) MIL-PRF-23419, Military standard for fuses. See also slash sheets MIL-PRF-23419 /8, /4, and /11.


2) Patent US5446436: “High voltage high power arc suppressing fuse”; Inventor: Mr. Richard A.


Williams (Palo Alto, CA); Applicant: Space Systems/Loral, Inc. (Palo Alto, CA); Issued Aug.


29, 1995. Abstract: A high voltage high power fuse for use in a low pressure environment such as space.


3) J. H. Richardson, and B. R. Lasley, "Tin Whisker Initiated Vacuum Metal Arcing in Spacecraft Electronics," 1992 Government Microcircuit Applications Conference, Vol. XVIII, pp. 119 -122, November 10 - 12, 1992.


4) D. H. Van Westerhuyzen, P. G. Backes, J. F.


Linder, S. C. Merrell and R. L. Poeschel, "Tin Whisker Induced Failure in Vacuum," 18th International Symposium for Testing & Failure Analysis, pp.407 - 412, October 17,


1992.http://misspiggy.gsfc.nasa.gov/whisker/


5) MIL-STD-202, Method 112A, Condition A. (Seal testing)


6) Max F. Hoyaux, Arc Physics, Springer-Verlag,1968


7) Handbook of Vacuum Arc Science and Technology edited by Raymond L. Boxman, D. M. Sanders, P.


J. Martin. Noyes Publications, New Jersey, 1995.


8) Circuit interruption: theory and techniques, Edited by Thomas E. Browne, Jr. Marcel Dekker, Inc.,New York and Basel, 1984.


Electronic Device Failure Analysis Society, editor, p 233-238


DOI: 10.1361/cp1999istfa233


Advanced Statistical Tools for Improving Yield and Reliability


Richard Kittler


Yield Dynamics, Inc., Santa Clara, California


Keywords


software statistics databases


testing traceability


yield


Significance


Failure analysts will be introduced to data mining and its relationship to other statistical techniques for


improving yield and reliability.


Analysis of manufacturing data as a tool for failure analysts often meets with roadblocks due to the complex non-linear behaviors of the relationships between failure rates and explanatory variables drawn from process history. The current work describes how the use of a comprehensive engin-eering database and data mining technology over-comes some of these difficulties and enables new classes of problems to be solved. The characteristics of the database design necessary for adequate data coverage and unit traceability are discussed. Data mining technology is explained and contrasted with traditional statistical approaches as well as those of expert systems, neural nets, and signature analysis. Data mining is applied to a number of common problem scenarios. Finally,future trends in data mining technology relevant to failure analysis are discussed.


The field of failure analysis plays a critical role in all areas of the yield ramp on a new technology or a new product introduction. With each succeeding generation process limits are being pushed into areas where it is increasingly difficult to forecast reliability and trace failures back to root cause [1]. Use of ad hoc statistical methods has often met with roadblocks due the complex non-linear behaviors of the relationships between failure rates and explanatory variables drawn from process history. Customer returns or failures during qualification typically involve small sample sizes from which little can be gleaned related to root cause.


The current work describes how the use of a comprehensive engineering database and data mining technology overcomes some of these difficulties and enables new classes of problems to be solved. The characteristics of the database design necessary for adequate data coverage and unit traceability will be discussed. Data mining technology will be explained and contrasted with traditional statistical approaches as well as those of expert systems and neural nets.


The relationships to signature analysis and classification trees will be explored. A number of common problem scenarios will be discussed.


The outlook for commercial availability of such capabilities will be surveyed and the system integration costs associated with their installation will be projected. Finally, the future of these new data mining and database technologies will be discussed as it applies to further improving the productivity of failure analysts.


Current Approaches and Limitations


Use of data analysis as a tool for failure analysis relies on ready access to broad classes of data as well as powerful analytical tools. Today most companies have islands of data. This data is a mixture of toolbased databases and file systems created by the analytical tools provided by suppliers, as well as inhouse efforts at consolidating data from varied sources. The in-house efforts have evolved based on the scope of the analyses that were deemed necessary during succeeding generations of technology. While customers would like all data to be easily available to the analysis tools of their choosing, suppliers are often most interested in keeping the data their tools generate accessible only by the add-on analytical packages they offer. There are as of yet very few standards for the interchange of data in defined formats even though the low-level SECS protocols have matured. Because these tools have evolved slowly it is rare that the database capabilities have kept up with analytical needs in an efficient fashion.


For example, few databases support traceability of lot numbers across facilities and access to associated data in a transparent fashion. These limitations make it difficult to correlate final test or reliability results to fab tool or process data except via tedious manual methods.


Data analysis tools range from those provided on the analytical tools to ad hoc environments in third party packages such as MS/Excel, SAS, and SPLUS. In the interest of creating analysis capabilities that span categories of data, e.g. fab, sort, assembly, and final test, many larger semiconductor companies have created in-house applications written on top of some of these third party tools. Recently a base of independent software suppliers has begun to emerge to fill the need for powerful, flexible analysis capabilities that span this range of data. This contrasts with the ongoing evolution of tool-based analysis capabilities driven by the hardware suppliers. Due to the costs of developing analysis capabilities internally, and their reliance on the availability of data, such tools rarely extend beyond ad hoc manual charting, regressions, and ANOVA.


TIP: Although only three points are required for this method, it is a good idea to have all four corners of a chip covered. After the alignment co-ordinates are entered, one can verify the accuracy of the alignment by asking the stage to go to the remaining point. This would tell one roughly how much “off” the alignment has turned out to be.


c) CAD based navigation: In a CAD based system one gets a visual representation of the circuits using the CAD design data.


Using standard tools and packages available,one can use the layout, schematic data and netlists, cross link these data with the FIB system software, and gain an on screen representation of the circuit. The design engineer can lay out the design change on a separate file, which can be pulled up to(theoretically) carry out the change. Despite all this sophistication, stage accuracy is really what determines where you are on the chip. The bottom line is that though one can see all layers from the database link, one still needs some top-level features to align and get to lower level nodes. In order to accurately go to lower level nodes, one needs an extremely accurate stage and/or needs to open holes in the passivation layer to confirm FIB locations. (FIB manufacturers now offer extremely accurate laser stages).[15] Another point to be careful about is that when the needle is extended to start the repair, it deflects the beam slightly and realignment needs to be done.


TIP: Find a non-critical lower level geometry you can safely expose for alignment purposes only. If this is successful without the needle retracting, one can count on the alignment accuracy.


d) Optical Overlay (Image-to-Image


registration)


This method of navigation is used primarily for finding nodes which are in the lower level metals, typically metal 1 in a 5 or 6 level metal device. This is carried out by overlaying the FIB image with an image of the same area showing the different metal layers. The latter could be part of a CAD data base, or a scanned image of the plot.


What is crucial is the presence of three alignment marks in the field of view on the FIB image, which can be correlated to the CAD database or scanned image. It is good to have these on top level metal.[7, 8, 9]


TIP: For today’s devices with planarized surfaces, in case one does not have a surface feature in the reasonable field of view, one can do the following: use 3-point align to go to the desired location; mill an outline box,or crosses on either side of the cross-hairs.


Next take the chip out and look at the chip under an optical microscope, take pictures,at least one of which show the corners of the milled box or crosses. Then scan the pictures in and do an image-to-image registration.[10]


5) Making vias: Once the region of interest is located, the next thing to do is to make vias in order to connect to the desired metal levels. In general one mills vias with the same beam current used for imaging. Typically, vias on toplevel metals are a couple of microns on a side.


Lower level vias need to be larger than ones for top level metal, so as to ensure better contact and lower contact resistance.[7, 11] Use of gas assisted etching(GAE) has been documented elsewhere [8, 9, 12] and suffice to say that using GAE has a couple of significant advantages. First, the time the beam is rastering reduces considerably(typically a reduction by a factor of 9, for insulator enhanced etch), and second, there is very little redeposition, thereby ensuring a cleaner via, and subsequently better fill and contact. And, of course, less beam time means less beam induced damage.


TIPS: Milling vias with GAE and a beam current between 30-50 pA gives optimum results. Use


rectangular patterns instead of square to increase total size of the via. Watch the real time monitor[RTM], update box, etc. to see when you hit metal. [7, 8, 10]


6) Filling vias and making connections: Note: All numeric references to filling and deposition are with respect to Platinum only. Similar numbers for W deposition need to be empirically ascertained.


Via filling: Top level metal vias can be filled in by inclusion in the interconnect pattern,but lower level vias need to be filled in before strapping across, in order to ensure good contact to the lower level metal. The main problem associated with filling vias is usually “voiding”. This happens when the via fills too fast, fills (bridges) over the top and does not make contact to the metal below. This is typically seen in the filling of the lower level metals. One of the ways to avoid this is to make the fill patterns smaller than the via itself. (This is true for top level connections also)[7, 8] Observations made by the authors have shown that any deposition that runs less than 2 ½ minutes generally leads to voiding in the vias, and the longer interconnects do not attain the thickness they are set for in the software. This is true up to about a beam current of 500 pA. [8]


Connections: Typical interconnects run between 5-75 microns long, 1-4 microns wide and about a micron thick. Selecting a beam current is typically based upon 2-6pA/ sq. micron of the pattern. A good idea would be to use this in conjunction with the 2 ½ minute guideline mentioned earlier.[7, 8] For longer interconnects, one can do the following. Make contacts on both ends of the connection, use a lower beam current to lay a 5% trace down all along, and then bump the beam current up and make the final connection. It is a good idea not to grab too many frames with the higher beam current, but to use the RTM,update box, etc. to check for drift.[8] Other methods of making long inter-connects are discussed in ref.13 and 14.


TIP: Adjust the dimensions on the patterns in order to get a minimum 2 ½ minute deposition. This way vias and interconnects should turn out satisfactory.[8]


7) Cutting Lines: Lines are cut after all depositions are complete, so that overspray does not refill the cut lines. Use of oxide selective and metal selective gases help expose, and cut the metal lines quickly and cleanly. Beam currents between 30-50 pA are good for exposing the metal lines initially. In order to maintain control over the cutting of lines, a nominally higher beam current (70-100 pA) is highly recommended, along with using enhanced etching gas. Also switching gases for the barrier metals results in quicker and cleaner cuts.[7, 8]


TIP: Switch between gases to cut through oxides, metal interconnects, and barrier metals in order to get cleaner cuts, in a shorter time frame.


8) Cleanup of Overspray: Overspray occurs when metal is deposited outside of the pattern,typically due to redeposition and interaction of the FIB induced secondaries and the gas. More frame grabbing during deposition causes more overspray.[7, 8] Cleanup typically consists of isolating the deposited tracks from one another.


This can be achieved by a) Outline boxes around depositions, b) Connecting filled mill boxes around depositions (wherever outline boxes are not practical, and c) Imaging at a high magnification with the insulator enhanced etch needle extended and gas flowing. In case of cleanups it is a good idea to watch the RTM, update box, etc.


and see the surface go dark, at which point either quit milling or in the case of method (c) move around. Beam currents typically used for cleanups would be between 70-100 pA.


TIP: During cleanup, when milling using filled/outline boxes make sure that the boxes do not cross depositions already made!


Device repair using a FIB system helps debug discrepancies in prototype chips in a fast and cost effective manner, prior to re working Silicon.


Unfortunately there is a price tag attached in the form of physical damage and surface/subsurface charge accumulation. Hence it behooves the FIB engineer and the design engineer to keep these effects in mind and carry out the repair with minimal damage and parametric alteration. In order to achieve this, one has to optimize “beam time”. Hence the need for effective planning before starting the repair and deciding what one needs to do: how to get there(navigation), opening up the desired metal levels(milling vias), filling them up and making


interconnects (filling and strapping across), severing lines (cutting) and isolating the depositions close enough to short out (clean up). Happy FIBBING and good luck!


Acknowledgements:


The primary author wishes to acknowledge his present coworkers for their help, guidance, and support. Special thanks to M.C. Hughes, Lucent Technologies for scanning in the plots, and for help in going through the manuscript. The author would also like to acknowledge Mrs. T.K. Hooghan, and J.L.


Moore, Lucent Technologies for help with reviewing the manuscript. Many thanks to C.H Holder, and R.


Aguilar, Lucent Technologies for providing the plots used in here.


The primary author also wishes to acknowledge the guidance, help, and encouragement provided @ Beam It Inc., during the authors tenure there. Without the support of my coworkers we would not be able to run experiments, have stimulating discussions, and come up with innovative solutions to problems. Lot of our success was gauged from the feedback provided to us by our customers, as to the integrity of the devices Fibbed. Unfortunately, severe restrictions on time and finances did not allow us to better quantify our experiments as well as we would have liked to do.


The authors also wish to thank Peter Carleson, FEI Hillsboro, Oregon, for his constant support, and permission to use some of his pictures. Also the authors would like to thank John Walker FEI, Europe,for many stimulating discussions.


1) Future of Focused Ion Beam systems, Jon Orloff,Metro Microscopy Meeting, Paramus, N.J.


4/27/99


2) Liquid Metal Ion sources and Limits on Focused Ion Beam Imaging Resolution, Jon Orloff,Course notes, The Essentials of Focused Ion Beam Technology, University of Maryland,October, 5,6 1997.


3) Focused Ion Beam Applications, Peter Carleson,Metro Microscopy Meeting, Paramus N.J.


4/27/99.


4) K. S. Wills and S. V. Pabbisetty, “Microsurgery Technology for the Semiconductor Industry,” in Electronic Failure Analysis, desk reference,1998, pp. 227-276.


5) A. N. Campbell and J. M. Soden, “Voltage Contrast in the FIB as a Failure Analysis Tool,”in Electronic Failure Analysis desk reference,1998, pp. 129-135.


6) J Benbrick, G. Rolland, P. Perdu, B. Benteo, M.


Casari, R. Desplats, “Focused Ion Beam Irradiation Induced Damages on CMOS and Bipolar Technologies,” Proceedings, ISTFA ’98,pp. 49-57.


7) “Integrated Circuit Modification”, Peter Carleson, Course notes, The Essentials of Focused Ion Beam Technology, University of Maryland, October, 5,6 1997.


8) Numerous discussions, experiments and notes compiled while working @ Beam-It Inc.


Carrolton, TX, during the authors tenure there carrying out contract FIB work.


9) K. Van Doorselear, R. Young, N. Dawes,“Golden Devices II: Alchemy in the .35µ Era,”Proceedings, ISTFA, ’96, pp.27-35.


10) Private discussion with John Walker Ph.D., FEI Europe.


11) R.A.Lee, T.R. Lundquist, “Low Resistivity Depositions Within High Aspect Ratio Holes,”Proceedings ISTFA’ ’96, pp. 85-88.


12) Applications note, “Focused Ion Beam Applications Using Enhanced Etch,” John. F.


Walker, FEI Europe, Ltd.


13) K. Van Doorselear, M. Van Den Reeck, L. Van Den Bempt, R. Young, J. Whitney, “ How to prepare Golden Devices Using Lesser Materials,”Proceedings, ISTFA, ’93, pp.405-414.


14) K. Van Doorselear, L. Van Den Bempt, “How To Use Cu-Plating for Low-Ohmic Long Distance FIB Connections,” Proceedings, ISTFA,’94, pp. 397-405.


15) http://www.knights.com


Electronic Device Failure Analysis Society, editor, p 255-261


DOI: 10.1361/cp1999istfa255


# Modeling and Optimizing XeF2- enhanced FIB Milling of Silicon


Modeling and Optimizing XeF2-enhanced FIB Milling of Silicon Neil J Bassom and Tung Mai


Micrion Corp., Peabody, Massachusetts


Wide variations in the dose enhancement factor observed when milling silicon using Focused Ion Beam (FIB) XeF2 Gas Assisted Etching (GAE)prompted the development of a simple model of the GAE process. The model accounts for three material removal mechanisms: regular sputtering; gas-assisted sputtering; and spontaneous chemical reactions. An expression linking the dose enhancement factor, εd,


to the gas and milling parameters has been derived.


Experiments show that εd behaves as predicted; good


quantitative agreement is achieved over wide ranges of milling parameters for εd values between 20X and


2500X.


Conditions required to minimize variations in d and maximize material removal rates, M, are derived. It is shown that if the dose per unit area per raster is below a threshold value then εd and M depend only


on the average current density J (the area of the box divided by the beam current). A consideration of the J regimes used for front-side and back-side FIB work shows why changes in εd have not previously been a


problem but are inevitable when milling the large trenches characteristics of Flip Chip circuit modification work. While εd changes dramatically


there is a region of J values for which M is approximately constant.


FIB is a vital tool for failure analysis and device development applications. In many applications the sputtering action of the ions is enhanced by introducing a gas to the chamber; material removal is then enhanced through chemical reactions. The use of gas can speed up material removal, provide


selectivity between materials, and produce cleaner cuts for high aspect ratio mills. In general, particular gas/material combinations are characterized by the dose enhancement factor εd, which is defined as the


depth achieved by a GAE mill of a certain dose per unit area divided by that depth achieved by a nonGAE mill of the same dose.


In conventional (front-side) FIB circuit repair applications the selectivity aspect is usually the more important effect, as only small volumes need to be removed and the mills themselves rarely take longer than a few minutes. Values of εd for various


material/gas pairs are well known and provide useful rules of thumb for operators. Implicit in this use of εd is the idea that εd values are fixed. In general, under


conventional conditions this assumption holds well.


With the advent of Flip Chip technologies has grown a need for FIB to be able to make circuit modifications from the back-side of devices. In response systems have been developed capable of using high (tens of nA) beam currents in conjunction


with special XeF2 gas delivery systems to remove large (up to 106 µm3) volumes of silicon. Experience with such systems has clearly shown that the concept of a single εd value is inadequate - large differences in εd are seen depending on the milling conditions.


This work was undertaken in the hope that a better understanding of GAE behavior would enable εd


variations to be eliminated, or least compensated for.


The Model: Assumptions and Results


A number of models of FIB GAE milling have been described in the literature. In general, they are built on extensions of a model of broad area ion beam


GAE [1, 2, 3], modified to allow for the fact that in the


FIB any region of the sample is periodically illuminated by a high intensity beam. Experimental investigations have mostly used small FIB beam currents into small mill areas and have been concerned with maximizing dose enhancements [e.g.


4, 5, 6], although some studies have examined the use of high beam currents (e.g. over 10 nA) and


considered etch/deposition rates [7, 8]. No work to date has examined systems in which spontaneous etching occurs, and the maximum dose enhancements seen are generally in the 10X-100X range.


In FIB GAE work the ion beam, of current I, is scanned in a serpentine fashion over the mill area. At dwell points separated by distances p in the x and y directions the beam dwells for a time τd before moving


to the next dwell point. The dwell point pixel spacing p is normally chosen to be comparable with the diameter of the beam. The model allows for three milling mechanisms: regular sputtering; gas-assisted sputtering; and spontaneous etching. Details of the model are given at annex A. The result is that for large mills (large meaning that the box contains a number of dwell points >> 1) in systems limited by the supply of gas (as is the case for the system studied here) the dose enhancement factor is given by:


α is a constant describing how much more efficient an ion is at removing material when gas is present than when it is not


β is a constant describing the rate at which gas molecules spontaneously remove material


r is the rate at which gas molecules evaporate/spontaneously react with the surface


k/n is a constant (which describes the relative probability of a gas molecule sticking to a vacant surface site and the density of such sites)


g is the rate at which gas molecules arrive at and adhere to a fresh surface (measured here through the chamber pressure)


d is the dose per unit area per raster, measured in C/m2 (1 nC/µm2 = 1000 C/m2) (d = τdI/p2)


A is the area of the mill (in m2)


I is the beam current.


In the case that A<<p2/rτd, which, with typical gas parameters, will generally hold for mills smaller than


about 80 µm x 80 µm, the expression approximates to:


Where J is the average current density (the beam current divided by the area of the mill). If the supply of gas is not the limiting factor then εd is expected to


be independent of gas pressure.


Experimental investigation


All experiments investigated the milling of silicon using XeF2 gas in a Micrion 9800FC FIB system.


The 9800FC is equipped with a 50 kV two lens ion beam column capable of delivering beam currents up to 27 nA. The system features a special gas delivery system providing high gas flux for the quick removal of large volumes of material. Gas delivery rates can be varied by changing the flow of gas through a variable leak valve. A feedback loop monitors the pressure on the chamber side of the valve and controls the valve to maintain the set point. Typical values for the set point are up to 2.5 Torr or so; these values are held to within around 0.2 Torr during milling.


An integrated optical microscope allows the depth of trenches to be quickly and easily measured in situ to an accuracy of a micron or so. The parameters of all mills were chosen such that the depth was at least


30µm, so measurement errors are kept below a few percent.


The Si/XeF2 system was selected for two major reasons. Firstly, this system is of great practical interest for FIB flip chip circuit modification work -oftentimes large volumes of silicon must be milled away to reveal fiducial marks and work site areas.


Second, XeF2 attacks silicon very aggressively. The high reaction rate implies that the value of r should be higher for this system than for many others and the fact that etching of silicon occurs spontaneously


implies a non-zero value for β. It was hoped that these factors would allow a range of GAE regimes to be investigated. The backside of a silicon wafer was used for the milling. All sites were given a low dose


mill (0.2 nC/µm2) immediately before the GAE mill started in order to clean the surface of contaminants(this dose should remove ~50 nm of material).


The first experiments were designed to investigate the behavior of εd as the flux of gas molecules is


changed. There is some difficulty in determining how best to analyze this - the factor g which enters the model is a combination of the flux of gas molecules and the sticking probability, and neither is known.


The two options are to plot εd against either the leak


valve set point or against the pressure in the chamber(or the rise in chamber pressure), assumed to be proportional to the gas flux at the sample. The chamber pressure is measured by a cold cathode ionization gauge (CCIG) located distant from the sample, and is certainly much lower than the pressure


β


−−


β−α


I Ad


rAd


kd


dr g


J g


≈


at the sample surface. Which is selected does not alter the general shape of the results. Figure 1 shows the dependency of εd on g, as measured through the


chamber pressure, for mills with A=6400 µm2,I=10 nA, p=0.4 µm, τd =0.3 µs.


Figure 1 Dose enhancement factor as a function of the chamber pressure.


A linear dependency of εd on pressure (r2=0.976)indicates that we are indeed in the gas-limited regime for all attainable gas fluxes. For all subsequent experiments the leak valve set point was held constant at 2.2 Torr. Measured chamber pressures


fluctuated between 1.15-1.20x10-5 Torr. Note that using the CCIG pressure as the measure of g requires that the factors concerning sticking probabilities originally contained in the definition of g must be


absorbed into the terms α and β, along with constants relating the gas molecular flux to the nozzle geometry and chamber pressure. Making this change does not affect the predictive power of the model


since the gas related terms are of the form gα and gβ,so that such factors can be contained in either g or α/β. It will however affect the numerical values of α and β. The change is introduced at this late stage in order that the equations stated above be (FIB)system-independent.


Experiments were then performed to examine the effects of the refresh time, τr (the time between


successive visits to a pixel by the beam). A series of mills was performed and the sizes of the mill boxes varied, so changing the refresh time. All other


parameters were held fixed, with I=10 nA, p=0.5 µm,τd=0.2 µs. The results are shown in Figure 2.


Figure 2 Variation of the dose enhancement factor with the refresh time.


It is clear that for the lower refresh times the prediction that εd should be proportional to the


refresh holds very well (ignoring the last point the correlation coefficient is 0.9997). The gradient of this


curve implies a value of α=4.1x107 m2A-1Torr-1. The deviation which is seen at seen at the high refresh times is taken as an indication that the condition A<<p2/rτd necessary for the enhancement to be proportional to the refresh to hold is no longer met.


This implies an upper limit for r of 20 s-1 or so.


The next experiments looked at the variation of εd


with changes in the dose per unit area per raster. This was done by holding A (2,500µm2), p (0.3µm), τr(15,000µs), and τd (0.5µs) constant while I was varied over the range 0.5-19.4 nA. W predict that εd


should be inversely proportional to the dose per unit area per raster, so that τd versus 1/I should be a


straight line through the origin. Figure 3 shows the observed behavior. The graph shows two distinct regimes. At lower values of 1/I, i.e. higher beam currents, εd behaves as expected. The gradient


implies that α=4.75x107 m2A-1Torr-1, in reasonable agreement with the value deduced from the refresh


experiments. Some considerable variation in α might be expected since, as discussed above, it includes the geometrical effects of nozzle placement, and between each set of experiments the gas delivery system was retracted and extended again.


2.00E-06


4.00E-06


6.00E-06


8.00E-06


1.20E-05


1.40E-05


1.60E-05


CCIG pressure (torr)


0.000E+00


5.000E-03


1.000E-02


1.500E-02


2.000E-02


2.500E-02


Refresh (s)


Figure 3 Dose enhancement factor as a function of beam current.


At lower beam currents (≤2 nA) deviations from the line are seen. This is believed to result from the breakdown of an assumption (see appendix) of the model that the ion beam is the dominant mechanism for gas molecule removal during the time when the beam exposes an area. The reasonableness of this interpretation is supported by a rough estimation of the relative ion and gas fluxes. At 1 nA the average ion flux during the dwell time exposure is


~7x1021 m-2s-1 (ignoring geometrical averaging effects, which will reduce this figure). Although we do not know the actual gas flux it is estimated that the


mass flow upper limit is around 10 µmols/min [9]. If we assume that all of these molecules strike the


surface in a circle 750 µm in diameter (roughly the diameter of the gas delivery nozzle) then the gas flux


is estimated at ~2x1023 m-2s-1 (this ignores the fact that gas molecule trajectories may not be confined to a cylindrical shape, an effect which would reduce this estimate) (note that the gas setpoint pressure, of


2.2 Torr, is measured between the variable leak valve and the vacuum chamber - during GAE mills the chamber pressure, as measured at the distant CCIG,


is typically ~10-5 Torr.)


The final set of experiments also looked at the variation of εd with changes in the dose per unit area


per raster. For these mills however the change in dose was effected by holding A (2500 µm2), p (0.3 µm), τr(3x105 µs), and I (10 nA) constant as τd was varied over the range 0.2-10 µs. Figure 4 shows the results,plotting εd against 1/τd.


Figure 4 Dose enhancement versus 1/dwell.


At the low 1/τd end of the curve εd is not directly proportional to 1/τd, as would be predicted. This


deviation results from the breakdown of the assumption that the ion beam is the dominant effect during exposure of an area. As the dwell time becomes longer the effects of gas molecules arriving during the dwell time (ignored in the model) become important.


Comparison of model to experiment


The model provides a good qualitative explanation for the behavior of εd over a very wide range of


milling parameters. In order to determine how well the quantitative behavior could be modeled a least squares fit was carried out on all of the data except the lowest beam current and longest dwell time experiments (as discussed above, the experiments clearly show that the assumptions underlying the model are breaking down in these cases, which are not of practical interest for large-scale FIB work).


Figure 5 Predicted versus fitted dose enhancement factors


Figure 5 shows the results of a fit using


α=5.8x107m2A-1Torr-1,


β=3.6x107 m2C-1Torr-1,r=7.14 s-1, k/n=19.2 m2C-1. The straight line is y=x:if the model were perfect all points would lie on this


Predicted vs observed dose enhancement (fitted parameters, high current data)


0 500 1000 1500 2000 2500


1500


2500


Observed dose enhancement


0.00E+00 2.00E+08 4.00E+08 6.00E+08 8.00E+08 1.00E+09 1.20E+09 1.40E+09 1.60E+09 1.80E+09 2.00E+09


1/beam current (1/A)


0.00E+00 5.00E+05 1.00E+06 1.50E+06 2.00E+06 2.50E+06 3.00E+06 3.50E+06 4.00E+06 4.50E+06 5.00E+06


1/Dw ell


line. The level of agreement encourages us to use the model to explore optimizing FIB milling.


Implications for FIB GAE


We can use the fact that the model correctly predicts the dependency of εd on milling parameters to


investigate the effectiveness of alternative milling strategies. For typical Flip Chip mills 1/J may have


values between about 2x10-2 µm2/pA and ~3 µm2/pA(from a 1 µm x 1 µm mill at 50 pA to a 250 µm x 250 µm mill at 20 nA). 1/J values for conventional applications would typically be in the range 2-


6x102 µm2/pA (from a 1 µm x 1 µm mill at 50 pA to a 25 µm x 25 µm mill at 10 nA) mills using . In general operators use larger beam current for larger area mills, so minimizing 1/J ratio changes - in the Flip Chip case however mill areas vary so widely that the 1/J values span a wide range.


Figure 6 shows the behavior of εd as a function of 1/J


for various values of d (using the fitted values for the model parameters). In all cases a large variation is seen. As d is lowered the variations between the curves are minimized, and we conclude that in order to minimize the dependency on d we should use


parameters such that d≤0.00005 nC/µm2. We are forced to conclude that even in this case variations inεd will inevitably be seen over the range of 1/J values


used in Flip Chip work. These curves help to explain why variations in εd are not troublesome in


conventional FIB GAE. The restricted range of 1/J values means that the variations as a function of area and beam current are small and the fact that the 1/J values are low mean that differences between mills using different d values (i.e. different dwells, beam currents, pixel spacing) are also small.


Figure 6 Dose enhancement factor as a function of average current density for various dose/unit


area/raster values.


At this stage it is useful to reconsider why εd is a


useful concept at all. Firstly, a high value provides reassurance that we will have adequate selectivity for the material we need to mill and the ability to mill


high-aspect ratio holes, both vital for circuit


modification purposes [10] . Second, it provides, in conjunction with the (known) dose delivered to a mill, a handy method for estimating how deep a mill will be. For the Flip Chip applications where εd


variations are large we have only the latter motivation; we are milling homogeneous material, so selectivity is not important, however, we still want to be able to estimate how deep a mill will be. By definition, the rate at which a mill etches into the substrate, M, is given by:


where s is a constant which we arbitrarily set to unity.


Figure 7 shows the variation of M with 1/J for mills with various values of d.


Figure 7 Milling rate as a function of average current


density for various dose/unit area/raster values.


The curves show three distinct regions. At the left hand side the presence of gas is essentially irrelevant


- we are using such high beam currents into small areas that the milling is dominated by regular sputtering. At the right hand side we are using such small currents and large boxes that the milling rates tend towards the spontaneous rate. As in the dose enhancement case, using mill parameters such that


d≤0.00005 nC/µm2 minimizes the differences between mills. Moreover, for small values of d there exists a central region where the mill rate is essentially flat. In this region, extending to from


1/J=10-2 µm2/pA to about 1/J=1 µm2/pA, the fact that (for a given size mill) using a small beam current gives a higher dose enhancement factor is almost completely counterbalanced by higher rate at which a large beam current delivers dose. For values of


1/J>1 µm2/pA the mill rate follows the approximate rule that M(1/J)0.44 is a constant.


These results suggest that the milling rate, rather than the dose enhancement factor, may be the more appropriate tool for estimating how deep very large GAE mills will be. For fast and predictable GAE milling of large boxes we should use large beam


currents to try and keep 1/J<1 µm2/pA and use dwell


r dd


s Mτε=


1.00E+00


1.00E+01


1.00E+02


1.00E+03


1.00E+04


1.00E-02


1.00E-01


1/J (µm^2/pA)


Dos e


enh anc em ent


d=0.00001 nC/µm^2 d=0.00005 nC/µm^2 d=0.0001 nC/µm^2 d=0.001 nC/µm^2


Mill ing rat e


(ar bitr ary uni ts)


times and pixel spacing such that d≤0.00005 nC/µm2. If the mills are so large that we cannot keep 1/J<1 µm2/pA then we can scale the expected milling rates according to the rule that M1(A1/I1)0.44 = M2(A2/I2)0.44.


1) T.M.Mayer and R.A.Barker, J. Vac. Sci.


Technol. 21, 757 (1982)


2) S.S. McNevin and G.E. Becker, J. Appl. Phys.


58, 4670 (1985)


3) W.E. Vanderlinde and A.L. Ruoff, J. Vac. Sci.


Technol. B 6(6), 1621 (1988)


4) A. Gandhi and J. Orloff, J. Vac. Sci. Technol. B 8(6), 1814 (1990)


5) L.R. Harriott, J. Vac. Sci. Technol. B 11(6),2012 (1993)


6) L.R. Harriott, R.R. Kola, and G.K. Celler, SPIE 1924, 76 (1993)


7) R.J. Young, J.R.A. Cleaver, and H. Ahmed, J.


Vac. Sci. Technol. B 11(2), 234 (1993)


8) H.-C Petzold, and P.J. Heard, J. Vac. Sci.


Technol. B 9(5), 2664 (1991)


9) J.D. Casey Jr., Private Communication


10) J.D. Casey Jr., A.F. Doyle, R.G. Lee, D.K.


Stewart, and H. Zimmermann, Microelectron.


Eng. 24, 43 (1994)


11) V. Scheuer, H. Koops, and T. Tschudi, Microelectron. Eng. 5, 423 (1986)


Appendix: Details of the model


Consider an ion beam, of current I, scanned in a serpentine fashion over the mill area. At dwell points separated by distances p in the x and y directions the beam dwells for a time τd before moving to the next dwell point. An arbitrary refresh time τrefresh may be


defined in software as the minimum time which must elapse between successive dwells at the same point.


If the box dimensions (X,Y) are small, so that the time taken to raster the beam (~XYτd /p2) is less than•τrefresh then the system pauses at the end of a raster until τrefresh seconds have elapsed before


beginning the next raster. For generality, we can describe the mill using a repeat time τ r defined by:


Gas molecules arrive and adhere to a fresh surface at a rate g (molecules per unit area) per second and


evaporate with a characteristic time of 1/r seconds.


The factor g incorporates gas flow rate, nozzle geometry, and sticking probability factors. Three mechanisms operate to remove material:


Ion sputtering: the removal of material solely under the action of the incident ions(i.e. the etching which occurs in the absence of any gas). This term is important only for determining the base removal rate against which dose enhancement factors are defined.


Gas-assisted sputtering: etching via chemical reactions which require the energy of the ion. This is the dominant process in most GAE work.


Spontaneous etching: For some gas/material combinations (including the XeF2/Si system


examined here) spontaneous etching can occur. In such cases etch effects are seen in areas which have been exposed to the gas but not scanned by the beam. Generally such effects are undesirable, as they lead to uncontrolled etching - however, for the high removal rates required in some applications there is little choice but to use gas/substrate combinations which are so reactive that spontaneous etching does occur.


Consider a single raster. As the basis for the model we assume that from time 0 to τd of each raster the


beam exposes an element of the surface. Each


incident Ga+ ion sputters secondaries - it is these secondaries which may interact with filled acceptor sites at the surface in gas-enhanced reactions. From time τd to τr the gas density at the surface builds up


until the beam next visits the area.


Ignoring transient effects occurring at the start of the mill (i.e. assuming that the mill has many rasters and the total milling time is long compared with the other characteristic times of the system - both of which are easily satisfied for mills of practical interest) we expect the proportion of filled sites to vary betweenθ2 (at times just before exposure to the beam) to θ1


(at times just as the beam moves on). Considering the depth removed per raster by each milling mechanism we make the following assumptions.


Ion sputtering: Depth is proportional to the dose delivered per unit area per raster, d:


refresh


XY


min


Sputtering


Depth


where the factor f allows for the number of secondaries generated per incident ion, density of the substrate, probability of secondaries escaping, etc.


Gas-assisted sputtering: Depth is proportional to the number of filled acceptor sites which take part in the reactions:


Spontaneous etching: Depth is proportional to the mean proportion of filled acceptor sites multiplied by the time taken to complete a raster:


By definition, the dose enhancement factor is the depth removed when gas is used in conjunction with a certain dose divided by the depth removed by the dose in the absence of gas. Denoting the dose enhancement factor as ε d we have:


Denoting the density of acceptor sites at the surface by n and the flux of ions by i (note that i is not the beam current, but the current density, multiplied by geometrical factors describing the number of dwell points per unit area, and the charge on the ion) the


rate equations for θ are given, following Scheuer et al[10] as, for 0<t<τd:


and, for τd<t<τr:


If ion bombardment dominates during exposure to the beam then the first of these reduces to:


We solve the last two equations subject to the constraints that θ is continuous at τd, and that θ (t=0)= θ(t=τr). Writing α = f2/fl, β = f3/f1, and k=iτd/d


where d is the dose per unit area per raster we obtain:


There are two extreme cases to consider:


High gas flux, g>>nr, gτr/n>>1. In this case the availability of acceptor sites determines the reaction rate - gas is supplied at a high enough rate that sites are filled as soon as they become vacant through evaporation or spontaneous or ion-induced reactions.


In this state, which has been observed experimentally, εd will have at most only a weak


dependence on gas flux, since


In the majority of systems, in which spontaneous


etching is not observed (β=0) there will be no


dependence on g.


Low gas flux, g<<nr. In this case the supply of gas limits the reactions, and εd is proportional to the gas


flux, since:


Initial experiments clearly showed that this regime held for the system investigated. If additionally rτr<<1, so that exp(-rτ r)~1-rτ r, then


If the refresh time is determined by the time taken to raster the beam, as is usually the case for large mills,then we can rewrite these equations using the facts that τr =Aτd/p2 and d=Iτd/p2, where A is the area of


the box and I the beam current.


and, when A<<p2/rτd:


GAE


θ


= r3f


Spon


tering)


Depth(Sput


Depth(Spon


Depth(GAE)


∂∂θ


1(g


∂


∂θit


][


βτ


+β


nr


ng


g n


d n


ατ


Electronic Device Failure Analysis Society, editor, p 263-272


DOI: 10.1361/cp1999istfa263


# Reliability Test Results for Pt FIB Interconnect Structures


Reliability Test Results for Pt FIB Interconnect Structures


Michael Zaragoza


Cadence Design Systems, Inc., San Diego, California


The reliability of FIB deposited Pt structures is assessed through lifetesting of product die and through stress testing of via-intensive test structures.


Data is also presented for Pt resistance monitors collected over a 21 month period aimed at assessing the stability of the FIB deposition process. Two product types were subjected to HTOL and HTSS conditions at 125°C followed by temperature cycling.


The test structures were stressed at different combinations of temperature ranging from 100°C to 140°C and with currents up to 5 mA. Neither product type experienced any FIB related failures whereas the test structure saw 70% fallout due to degradation of the Pt material within the vias. Temperature cycling did not precipitate any failures. The Pt resistance monitor data showed that film resistance increases with film thickness indicating the incorporation of organic byproducts from the deposition process.


Focused Ion Beam (FIB) modification of Al interconnects has become an established practice for correcting design errors in integrated circuits. The success of the modification can depend not only on the correct implementation of the design fix but also on the stability of the FIB connections over time.


Due to the time required to re-spin a design through a fab it is often necessary that the FIB modified devices remain functional for a relatively long period of time in an operating environment similar to that of the final product. Ideally the FIB device would be able to withstand temperature, current, and thermal cycling.


Unfortunately there is little published data to support this expectation.


Consequently a series of experiments was conducted to determine the reliability of FIB interconnect structures.


FIB Reliability Issues


The process of FIB modification alters the mechanical and materials integrity of the device,changes that can influence the reliability of the product. For instance it is well established that the interlevel and passivation dielectric films exert tremendous mechanical stress on Al lines1,2 which results in stress gradients that cause Al diffusion5,6,inducing voids and decreasing electromigration resistance. By FIBing in windows and cuts, points of zero stress can be created that can lead to stress gradients. From a materials perspective the FIB process introduces several chemical elements known to interact with Al. Halogens, commonly used in gasassisted etching, can cause Al corrosion. In the Pt deposition process, the Ga ion beam is used to dissociate a Pt organicmetallic gas adsorbed onto the device surface. Thus the deposited film is a mixture of Pt, Ga, and C. From Energy Dispersive X-ray Spectroscopy (EDXS) analysis, the typical concentrations of FIB deposited Pt is ~ 85% Pt, ~13%Ga, and ~2% C. Pt readily forms intermetallics with Al3,4 in a fashion similar to Au and Al, which could possibly lead to Kirkendall voiding5,6. Although the Ga concentration is relatively low, consideration of the Al-Ga phase diagram7 suggests the possibility that Ga could diffuse into the Al, disrupting both films.


Thus the integrity of the Pt patch must also be considered in discussions of reliability effects.


Possible Pt patch failure mechanisms could include line migration analogous to Al electromigration,phase separation of the Pt film into its separate components, or delamination due to thermal coefficient expansion (TCE) mismatch between the Pt and substrate. Also possible are fatigue induced failure of Pt filled vias due to TCE action.


For any process to be reliable it must also be manufacturable meaning that the process must produce consistent results from run to run over a long period of time. In the case of FIB the critical performance parameter is resistance of the FIB connection. Therefore along with any reliability testing it is necessary to collect data demonstrating the basic stability of the FIB process.


To investigate the reliability of FIB structures two experimental approaches were used. The first was to place FIB modified product die on lifetest to evaluate FIB reliability in a product environment. The second approach was to create FIB test structures that could be directly stress-tested. Also, Pt resistance monitors were run weekly to assess the consistency of the deposition process.


All experiments were conducted on a FEI 611 FIB system with Pt deposition using the gas methylcyclopentadienyl trimethyl platinum. The ion beam energy was 25 KeV and the beam current density for Pt depositions was ~6 pA/ µm2. The nominal thickness for the depositions was 1.0 µm using a beam dwell time of 0.4 µsec and 0% beam overlap.


For the product lifetest, two product types were selected based on the availability of ATE test vectors for the FIB modified product. A description of the product technologies is listed in Table 1 along with the test conditions, number of parts tested, and hours on test. Product A was tested under HTOL (High Temperature Operating Life) conditions with a clock speed of 0.6 MHz and with the power pins at Vdd and the ground pins at 0 volts. The FIB modifications on Product A involved routing clock lines from Metal 2 to Metal 1. From circuit simulations it is estimated that ~100 µA of current passed through the FIB straps during each clock cycle. Product B was tested under HTSS (High Temperature Steady State)conditions with bias applied to the power pins and


with the signal and ground pins at 0 volts. The modifications on Product B involved strapping Metal 1 lines connected to poly gates to a Metal 1 ground connection. All parts were assembled in ceramic packages prior to FIB and were then hermetically sealed and tested for yield prior to lifetest.


The same FIB modification process was used on both products. The process consisted of milling vias 1.5µm x 1.5 µm through the passivation and/or interlevel dielectric with a beam current of 200 pA. To exclude the possibility of halogen-induced failures, gasassisted etching was not used. The vias were connected by Pt in a single deposition, i.e. the vias were not backfilled prior to depositing the strap.


The width of the strap was defined by a raster pattern


2.0 µm wide and the strap extended beyond the via opening by 0.5 µm. For the cut process, iodine gasassisted etching was used. The cut window was sized so that a 2.0µm gap would be milled into the Al line.


Table 2 details the number and lengths of the Pt straps and the number and layers of the cuts.


There were four readout points during lifetest: 168 hrs, 500 hrs, 1,000 hrs, and 2,000 hrs. However the Product A lifetest was terminated at 1,650 hrs due to scheduling conflicts. Following lifetest, the Product A parts were subjected to temperature cycling for 250 cycles from –65°C to 125°C with 20 minute soak times and a 20 minutes transition interval.


In the second approach FIB test structures were created by modifying interconnect structures on test chips from the Product B technology. This group of parts came from the same lots used to qualify the Product B technology although the structures modified had not been previously subjected to any temperature or current stress testing. Two types of structures were created and FIBed onto one die. The die were packaged in 40 pin DIPs and wire bonded prior to the FIB work. The packages were nonhermetically sealed so that the structures could be examined for wearout during the course of testing.


The design of the structures follows.


Table 1 FIB Modified Products Placed on Lifetest


PRODUCT


TECHNOLOGY


METAL


LEVELS


CONDITIONS


QTY.


HOURS


1.0 µm/ 5V CMOS


Al/ Si


HTOL, 125°C


1,650


0.8 µm/ 5V CMOS


Al/ Cu/ Si


HTSS, 125°C


2,000


Table 2 Description of FIB Modifications Used on Products A and B


Straps


Cuts


S1


S2


S3


C2


C3


7 µm


14 µm


M2


M1


15 µm


86 µm


MANY LINKS is a via intensive structure with vias sized at 1.5 x 1.5 µm, milled through passivation to expose Metal 3. The vias were then connected in pairs by oversized Pt patches 4 µm wide. A single deposition was used for filling the vias and depositing the Pt. The Pt patches were oversized to minimize the likelihood that the Pt connection would be the failing feature. A schematic diagram for this structure is shown in Figure 1. The MANY CUTS structure (see Figure 2) consists of ten parallel Metal 3 lines that were milled through (i.e. cut open)simultaneously, leaving an open slot across the structure 2 µm wide.


Via


X


Cut


Pt Patch


Figure 1 Schematic diagram of MANY LINKS test structure. FIB connections were to top level metal.


The pads are directly wire bonded to the package.


X X X X


Pad


Figure 2 Schematic diagram of the MANY CUTS structures with the X's indicating location of the cuts.


The cuts are in the top level metal.


For the temperature and current stressing, the parts were placed in the Cadence Reliability Engineering LifeTest System (RELTS). This system consists of a series of ovens with test boards configured such that each FIB structure could be individually biased. The boards were connected to a switch matrix card so that resistance of each structure could be measured in situ.


The bias stress tests were done under constant current conditions such that if the resistance changed then the applied bias was automatically adjusted to keep the current level constant.


Bias conditions were selected based on the electromigration limit of the Product B technology,which is approximately 2mA for lines and vias or 105 A/cm2. The bias and temperature conditions are given in Table 3 along with the number of parts tested for each condition. The table reflects the intent of the experiment to extract preliminary FIB reliability data


so a wide range of conditions was used but at the expense of running multiple samples per condition.


Temperature cycling was performed on several parts at the same conditions as the product parts.


Al wire bonds


Pt strap


Pt steps


Vias milled through passivation


Figure 3 Schematic diagram of the Pt resistance


monitor structure. The Pt steps were used to minimize stepcoverage effects due to the pad height of 2.8 µm.


The strap length is 75 µm.


The Pt resistance monitors were created by connecting two bond pads with a Pt strap. A schematic diagram of the structure is shown in Figure


3. The FIB process was similar to that used on the product die. First vias were milled through the passivation using a window 1.5 µm x 1.5 µm. The center of the vias were placed 2.25 µm from the passivation edge. To minimize stepcoverage effects caused by the height of the pads, Pt lines 4 µm wide,2 µm long and 1.0 µm thick were deposited adjacent to the pads. The Pt strap was then deposited using a raster pattern 57 µm x 2 µm wide which simultaneously filled in the vias. The straps were deposited to a thickness of 1.0 µm based on deposition rates supplied by the manufacture. To insure that the measured resistance was from the strap only, gas-assisted etching was used to clear the Pt overspray to within 1.0 µm of the line. The structures were made on test chip die from the Product B technology. The die were assembled in 40 pin ceramic packages and wire bonded prior to FIB modification. The pad arrangement allowed 32 structures to be placed on one die. Resistance was measured at the package leads and less than 0.5 Ω of resistance was contributed from the package leads and wire bonds. Each week four Pt resistance monitors structures would be deposited in succession and the resistance measured. The structure with the median resistance value for that run would then be cross-sectioned to determine its cross-sectional area.


Table 3 Number of Structures Stressed per Condition


0 mA 2 mA 4 mA 5 mA


100 °C


125 °C


⎯


140 °C


0 500 1000 1500


Dec96


Jan97


Feb97


Mar97


Apr97


May97


Jun97


Jul97


Aug97


Sep97


Oct97


Nov97


Dec97


Jan98


Feb98


Mar98


Apr98


May98


Jun98


Jul98


Aug98


Time (weeks)


Figure 4 Pt monitor resistance data. The bold


vertical lines mark when new Pt sources were


installed. Data was collected over a 21 month period.


0 500 1,000 1,500 2,000 2,500


Cross-sectional Area (um2)


Figure 5 Cross-sectional area versus resistance for the Pt resistance monitors. All lines were deposited at 1 µm nominal thickness.


Pt Resistance Monitors


Pt resistance was found to be extremely variable, both over time and within a given run as shown in the trend data plotted in Figure 4. Resistance values ranged an order of magnitude from ~200 Ω to over 2,800 Ω with the median resistance at ~600 Ω.


Figure 4 shows that the resistance of the FIBdeposited Pt appears to decrease with continued use of the Pt crucible.


Figure 6 FIB cross-sections of Pt resistance monitors with high and low resistance. The top cross-section is of a 2,100 Ω line and the bottom cross-section is of a 450 Ω line. Magnification is 8400x for both


pictures. Samples are tilted at 45°.


In order to understand what line parameters, if any,affected the resistance variation, the cross-section data was plotted against resistance and is shown in Figure 5. This plot shows the surprising result that for the FIB deposited Pt lines the resistance increases as the cross-sectional area increases, directly the opposite of metal films. The implication is that the thicker films contain more organic byproducts or unreacted precursor compound. Close monitoring of stage current during depositions showed little variance, indicating that the thickness variation most likely is due to gas flux changes during deposition.


The difference in deposition rate does not appear to affect the film’s microstructure as shown in FIB cross-sections of a low resistance line and high resistance line. (see Figure 6) Both films have the same amorphous film structure. EDXS analysis did not reveal any significant compositional differences.


However the typical C concentration of 2% is near the detectability limit of EDXS so even a 2X


difference in C content would be difficult to measure.


Replacing the injector nozzle used to direct the gas onto the deposition site did not effect the resistance or film thickness results.


0 2 4 6 8 10 12


250-350 350-450 450-550 550-650 650-750 750-850


Resistance Range (ohms)


Figure 7 MANY LINKS time zero resistance


distribution. Four lots, indicated by the bar shading,were produced over a four week period.


FIB Test Structure Time Zero Evaluation


The time zero resistance values were measured for all structures prior to lifetest. These results are plotted in Figure 7. The Many Link structures had a reasonably tight time zero distribution, however the measured values were 2x greater than predicted based on the median sheet resistance derived from the Pt resistance monitors. This more than likely reflects the fact that via resistance dominated the resistance value. The Many Cuts structures read electrically open as designed.


Test Results


Product Level Lifetest Results


Both Product A and Product B were tested out to the maximum hours shown in Table 1. The parts passed all functional tests at every readout point and at final test. The FIB connections on several parts were then examined for evidence of aging. A FIB cross-section of one of the connections from Product A is shown in Figure 8. This figure shows no evidence of aging or breakdown of the via or lines and is representative of all the vias and lines examined. These results indicate that FIB modifications in a product environment are reliable up to 125°C.


Figure 8 FIB cross-section of the 7 µm strap from Product A. The Pt has all the appearances of an asdeposited line. There is no indication of interaction between the Pt film and the Al. The crease at the step is a typical Pt stepcoverage phenomenon.


Table 4 Summary of RELTS test results for the Many Links structures showing number of hours on test.


Values in bold italics indicate time-to-fail based on structures failing continuity


S/N


Hours


2 mA


4 mA


5 mA


100°C


128


5,565


103


179


117


1,117


2,700


104


105


106


86


118


129


2,550


131


125°C


120


119


126


5,530


127


536


140°C


124


122


1,680


1,150


123


1,600


Al


RELTS


The RELTS test environment is often more effective at precipitating failures than product level lifetest because it permits the direct stressing of process structures. As such the structures are exposed to conditions that do not typically occur on products and hence are more likely to yield failures. This in fact was the case with these tests. The RELTS results are summarized in Table 4, where electrical continuity was used as the pass/fail criterion. The data in the table shows that over the course of the test, 70% of the Many Links experienced open circuit failures.


The fallout only weakly correlated with the stress conditions. To see if the time zero resistance values affected the fallout, a comparison was made between the failing and passing structures which is charted in Figure 2. The chart shows that the fails occurred across all the resistance values. There was also no correlation between the time-to-fail and the initial resistances.


250- 350 350- 450 450- 550 550- 650 650- 750 750- 850


TIME ZERO RESISTANCE


FAILS


PASSES


Figure 2 Frequency distribution of time zero


resistance values for the MANY LINKS structures placed on RELTS. Failures occurred across all resistance values.


0 100 200 300 400 500 600 700 800


1000 2000 3000 4000 5000 6000


Time (hours)


#128


#130


Figure 10 Plot of In situ resistance measurements for MANY LINKS #128 and #130 stressed at 125°C/0 mA. No significant change in resistance occurred.


Figure 11 FIB cross-section of Part #128 exposed to


100°C for 5,565 hours. The Pt film has the same


appearance as the as-deposited film.


Figure 12A Planer SEM micrograph of Link 4 on part #103 where melting occurred on the


right side via.


The RELTS results do support the findings from the product level lifetest in that the two Many Links stressed at 100°C and 0 mA did not fail. One advantage of the RELTS system is that in situ resistance data can be collected for the structures being tested. The data for parts #128 and #130 is shown in Figure 10 where it can be seen that the resistance remained stable throughout the test. For this reason these units were left on test until 5,600 hours. Cross-sections were then done on three links from each part to look for evidence of wearout. All the structures examined showed no sign of degradation. (see Figure 11)


In the case of all parts that failed under the higher stress conditions, the vias were the point of failure.


For Many Links #103 - #107 the rapid fallout resulted from failing to properly current limit the current sources during power up which apparently lead to EOS type damage in the vias such as shown in Figure 12A. The balling up of the Pt indicates that melting of material had occurred. Inspection of the via cross4.5 kx


section (Figure 12B) by Scanning Electron Microscopy (SEM) shows spheres due to local melting on top of the Pt line and that the underlying material is darker in contrast suggesting local changes in composition. Cross-sections of other vias where local melting had occurred had similar appearance.


None showed evidence of Pt/ Al intermixing,indicating that the local temperature had not exceeded the eutectic point of Pt and Al of 657°C. The Ga-Pt phase diagram. (see Figure 13)


Figure 12B SEM micrograph of the via shown in Figure 12A after cross-sectioning. There is no


indication of Pt-Al intermixing.


Figure 13 Ga-Pt phase diagram. From Guex &


Feschotte, JLCM; 46, 1976; pp 101 - 106.


does show that under equilibrium conditions and at high Ga concentrations (> 85%), Pt can form a eutectic with Ga. This is significantly higher than the typical Ga concentration of ~13% for the as-deposited films. One possible source for additional Ga could be from the via milling operation where clusters of Ga might form. If this were the case the local Ga concentration might be high enough that with the EOS spike there was sufficient energy to induce a sudden phase reaction between the Pt and Ga causing a liquid to form that diffused up to the surface. After current limiting the current source only one out of ten parts failed by the melting mechanism (#120).


Figure 14 SEM micrograph of a via cross-section from MANY LINK #124. The material in the via has a darker contrast and a coarse texture compared to remainder of the film. There is also a distinct


interface separating this region.


For the remaining parts, degradation of the Pt material in the vias was found in a large percentage of vias cross-sectioned. One example is shown in Figure 15. The material in this via has a darker contrast than the rest of the film and it is separated by a sharp interface. Two other examples are shown in Figure 16 and Figure 18 where the samples were Au coated, which allowed better resolution in the SEM but eliminated much of the image contrast. These samples show voiding of the Pt material and volume contraction. For the samples that were current stressed, there was no correlation between the Pt degradation within the vias and whether the via was on the anode or cathode side of the circuit. However the application of current does appear to have some effect in precipitating failures.


Unfortunately, attempts at identifying the composition of this material on a few samples by Scanning Auger Microscopy were unsuccessful because in each case the via material “blew out”


13.3 kx


VIA


during spot mode analysis. In view that the Pt resistance monitor data indicates that the as-deposited Pt film contain organic material, it is hypothesized that this was a result of trapped organic material,possibly unreacted Pt compound, decomposing under the electron beam.


As shown in Figures 16 and 17, as the via fill material undergoes volume contraction it pulls away from the via sidewalls and bottom, reducing the area of contact. As previously pointed out, the resistance of the Many Links is dominated by via resistance so one would expect resistance values to increase as the vias aged and that the time-to-fail should correlate with the extent of via degradation. From a sampling of cross-sections, the general trend was that for parts that failed in less that 1,000 hours, ~75% of the vias underwent degradation whereas as for parts that failed in more than 1,000 hours, ~ 33% of the vias were affected. A graph of resistance versus time is displayed in Figure 17 which shows that for the former group, resistance began rising within the first few hundred hours while for the latter group the resistance remained relatively stable until the time of failure.


Some of the open circuit failures were analyzed using voltage contrast SEM to identify the failing via. A cross-section of one of these sites is shown in Figure 18 but the general observation was the same with all the sites examined. In all cases volume contraction of the Pt material had occurred to the point that the material completely disconnected from the Al. Note that the other via in this pair shows no evidence of degradation.


Figure 15 SEM micrograph of a via cross-section


from part #125. The Pt material within the via is


pocketed with voids and has separated from right


sidewall and bottom. The sample was Au coated


which reduced the contrast between the via material and the remainder of the film.


Figure 16 Part #125, Link 2 cross-section. Note pronounced separation of material from sidewall.


This sample was Au coated.


0 250 500 750 1000 1250 1500 1750 2000


500 1000 1500 2000 2500 3000


#124#125


#122


#129


Figure 17 Resistance data for some MANY LINKS structures.


Figure 18 Cross-section of failing link on part #122.


The point of electrical failure is the left side via


where complete separation of the via material from the Al has occurred. Note that the right side via has not undergone any phase formation.


Areas of separation


Point of complete discontinuity


Temp Cycling


There was no evidence of FIB related wearout on any of the parts temp cycled. A graph of resistance versus temp cycling for the Many Links structures is shown in Figure 19. It shows that one of the five parts did fail continuity at 1,400 cycles but inspection and cross-sections of that unit did not reveal any signs of wearout suggesting that the fail was package related.


In fact the Al pad metallization on all the parts was extensively hillocked at end of the test which might account for the resistance increase observed on the other two parts. Cross-sections of the Many Cuts structure showed no evidence of Al migration into the cut area and the Product B parts that were temp cycled passed all functionality tests.


0 200 400 600 800 1000


300 600 900 1200 1500 1800 2100


Number of Cycles, -55 C to +125 C


Figure 17 Temperature cycling resistance data.


Arrow points to unit that failed continuity.


The product level lifetest results demonstrate that it is possible to make reliable FIB structures. Although these parts were tested at 125°C for up to 2,000 hours,none of the vias cross-sectioned showed evidence of via related degradation and there was no indication of any other type of wearout within the FIB structures or the Al. The RELTS results indicate that this may be an upper limit to what the Pt structures can tolerate.


With higher temperatures and with the application of current, significant fallout occurred on the Many Link structures due to degradation of the Pt film within vias. However the degradation phenomenon did not show a strong correlation to stress conditions indicating the influence of some other factor. One possible clue for this is indicated by the Pt monitor resistance data.


The Pt monitor resistance data indicates that the organic content of the as-deposited films effects the final resistance. The Pt deposition process involves the adsorption of the Pt precursor gas, methylcyclopentadienyl trimethyl Pt on to a surface where it


is then dissociated by the ion beam. However not all of the organic material desorbs during the dissociation process resulting in films with much higher resistance values than the pure film. The adsorption rate is directly related to flux so that if the flux increases it can be expected that the organic content of the deposited film will also increase. As proposed by Puretz and Swanson8, at higher flux rates, film thickness should increase but with a corresponding increase in film resistance due to unconverted Pt precursor material remaining. This is in fact what is shown in Figure 5 which demonstrates that the gas flux varies over the life of the Pt source. However this does not explain why the Pt resistance monitor data was so variable run to run.


Another factor influencing deposition yield is topography. This effect is most evident from the cross-section micrograph in Figure 14 which show that the Pt thickness is greater in the via area than over passivation even though the depositions were done as a continuous scan. This requires that the deposition yield be higher in the vias than at the surface for the same gas flux. This observation is consistent with Tao, et al,9 who reported that Pt deposition yields inside a trench 0.5 µm wide and


0.7 µm deep to be 8 times higher than on a flat surface. With this deposition rate difference one would expect that a via would fill up in the time required to deposit 0.1 µm of Pt over passivation and that the resulting film would be the same height over the via as the passivation. This is what is shown in Figure 11.


One possible explanation for the accelerated deposition effect is that the aspect ratio of the via traps the precursor gas, effectively increasing its concentration, resulting in the higher deposition yield but producing a film higher in organic content. It would also be expected that the vias would contain a higher concentration of Ga as residual from the milling operation. Thus with the higher organic and Ga content, the via composition affects the resistance variability as well as the long term reliability.


Based on the results of the Many Link test structures,this study shows that at high temperatures and high current stress, FIB deposited Pt films can undergo degradation within the vias which can leads to volume contraction and subsequently higher resistance and open failures. Based on a very limited sample size it is concluded that this mechanism is thermally activated above 125°C but might depend on the concentration of organic byproducts and residual


Ga within the vias. Thus higher temperature and application of current do not have a systematic effect on failure rate. Data from Pt resistance monitors shows that film resistance increases with film thickness indicating the presence of organic byproducts within the Pt films. Temperature cycling did not precipitate any failure modes on the product parts or the test structures. The FIB modified products stressed at 125°C with little or no current stressing did not experience any failures and showed no evidence of Pt degradation within the vias.


The author would like to acknowledge the contributions and efforts by several Cadence colleagues. Dan Perry for running all the reliability tests which included making custom modification to the RELTS system, Sam Dixon and Kathy DeLima for the FIB work, and Mark Nakamoto and Riko Radojcic for insightful discussions and encouragement’s. Thank you.


1) Sinha, et al., “Thermal Stresses and Cracking Resistance of Dielectric Films (SiN, Si3N4, and SiO2) on Si Substrates”, J. Appl. Phys. 49 (4),April 1978.


2) E. Fleck, “Controlling Stress in Oxy-Nitride Films”, ASM Newsletter, Vol. 1 (2), December


1985.


3) Yue, et. al., “Stress Induced Voids in Aluminum Interconnects”, Proc. Intl. Rel. Phys. Symp.,


4) Turner, et. al., “The Influence of Stress on Aluminum Conductor Life”, Proc. Intl. Rel.


Phys. Symp., 1985.


5) E. Colgan, “Phase Formation and Dissociation in the Thin-film Pt/ Al System”, J. Appl. Phys. 62(4), 15 August 1987, pp. 1224 - 1231.


6) C. Smithells, Metal Reference Handbook, 5th Ed., Butterworths, 1976, pp. 414.


7) E. Philofsky, “Intermetallic Formation in Gold -Aluminum Systems”, Solid State Electronics,Vol. 13, 1970, pp. 1391 - 1399.


8) K. Okumura, “Degradation of Bonding Strength(Al Wire - Au Film) by Kirkendall Voids”, J.


Electrochem. Soc., Vol. 128, No.3, March 1981,pp. 571 - 575.


9) C. Smithells, Metal Reference Handbook, 5th Ed.,Butterworths, 1976, pp. 403.


10) Puretz and Swanson, “Focused Ion Beam Deposition of Pt Containing Films”, J. Vac. Sci.


Technolo. B 10(6), Nov/Dec 1992.


11) Tao, et. al., “Focused Ion Beam Induced Deposition of Platinum for Repair Processes”, J.


Vac. Sci. Technolo. B9(1), Jan/Feb 1991


Electronic Device Failure Analysis Society, editor, p 273-281


DOI: 10.1361/cp1999istfa273


# Focused Ion Beam Induced Effects on MOS Transistor Parameters


Focused Ion Beam Induced Effects on MOS Transistor Parameters


Ann N. Campbell, Paiboon Tangyunyong, Jeffrey R. Jessing, Charles E. Hembree,Daniel M. Fleetwood, Scot E. Swanson, and Jerry M. Soden


Nicholas Antoniou


Micrion Corporation, Peabody, Massachusetts


William E. Vanderlinde


Microelectronics Research Laboratory, Columbia Maryland


Marsha T. Abramo


IBM Microelectronics, Essex Junction, Vermont


We report on recent studies of the effects of 50 keV focused ion beam (FIB) exposure on MOS transistors.


We demonstrate that the changes in transistor parameters (such as threshold voltage, Vt) are essentially the same for exposure to a Ga+ ion beam at 30 and 50 keV under the same exposure conditions.


We characterize the effects of FIB exposure on test transistors fabricated in both 0.5 µm and 0.225 µm technologies from two different vendors. We report on the effectiveness of overlying metal layers in screening MOS transistors from FIB-induced damage and examine the importance of ion dose rate and the physical dimensions of the exposed area.


Focused ion beam (FIB) technology has become increasingly important for performing circuit modifications in support of the design verification phase of IC manufacturing. The successful use of FIB technology for these applications significantly reduces the development costs and time-to-market of new products. Because of the importance of these tools in both design verification and failure analysis applications there has been growing interest in understanding the possible side effects of FIB exposure on ICs.


Two recent studies have systematically investigated the effects of FIB exposure at the transistor level to understand the basic phenomena and likely damage mechanisms [1,2]. Both Campbell et al. (1997) [1] and Benbrik et al. (1998) [2] investigated the effects of 30 keV Ga+ exposure on MOS transistors for submicron


and older technologies. Both studies showed that transistor parameters, such as threshold voltage (Vt) and transconductance (gm), change in response to FIB exposure. Both studies also found that the magnitude of transistor parameter changes increases with higher ion dose and smaller gate areas for a given technology.


Campbell et al. showed that FIB-induced changes in transistor parameters were bake-recoverable and that they could be prevented by the use of electron flood charge neutralization [1]. Also, they found that the observed changes in transfer characteristics were consistent with the development of oxide- and interface-trapped charge as a result of FIB exposure.


These defects were likely caused by sample charging,but the possibility of ionizing radiation-induced defects was not ruled out.


Benbrik et al. studied the effects of FIB exposure on CMOS inverters, diodes, and bipolar devices in addition to MOS transistors [2]. They found that MOS technologies are less sensitive to FIB-induced degradation than bipolar technologies and concluded that input protection structures play an important role in protecting MOS ICs. They also suggested that overlying metal signal and power lines may protect active regions. These authors related the transistorlevel damage to sample charging during FIB exposure.


Ion columns with reduced spot size (~5 nm) and increased operating voltage (50 keV) are now commercially available. A primary purpose of this study is to examine the effects of FIB exposure at 50 keV and compare them with the results of exposure at 30 keV. In addition, we describe several other experiments aimed at obtaining a better understanding of the degradation mechanisms involved. One set of


experiments examines the dose rate dependence of FIBinduced damage and another evaluates the effectiveness of overlying metallization layers in screening MOS transistors during FIB exposure.


Experimental Approach


MOS transistors fabricated from different technologies were used as the test vehicles for evaluating the effects of FIB exposure. The transistors were characterized electrically by measuring the transfer characteristic(drain current, Id, vs. gate voltage, Vt) both prior to and following FIB exposure. The changes in transistor parameters, such as threshold voltage (Vt) and/or transconductance (gm) were used to monitor the effect of FIB exposure on the MOS transistors. In general, a different transistor was used for each data point.


The technologies studied in this work included two 0.5µm CMOS technologies from an R&D wafer fab and an industrial 0.225 µm CMOS technology. The details of these technologies and the transistor geometries used in these experiments are shown in Table 1. The dimensions “0.5 µm” and “0.225 µm” are the minimum as-drawn feature sizes and will be used generically to refer to these technologies. However, the actual sizes of the transistors used in a given experiment may vary.


Both n- and p-channel transistors of several geometries were exposed to the FIB with ion doses ranging from~10-4 nC/ µm2 to ~10-2 nC/ µm2. Ion exposures in this range are representative of the ion doses that result from image acquisition during navigation to an area of interest. As a general rule of thumb, a dose of 4 nC/µm2 removes approximately one micrometer of typical IC materials such as Al, Si, and SiO2.


Two different FIB systems were used for the ion exposure experiments. A Micrion 9000 FIB system with 25 nm minimum spot size was used for FIB exposure at 30 keV. The 50 keV exposures were performed in a Micrion 9500 system with 5 nm minimum spot size. Exposure of the MOS transistors was performed with the electron floodgun both active and disabled. The floodgun directs a low energy (~ 80 eV) spray of electrons at the sample surface to counter the charging effects of Ga+ ions. Except where indicated, all experiments were performed at the wafer level with the substrate grounded through the sample stage and with the transistor terminals floating.


Blind navigation was used whenever possible to position the transistor of interest under the ion beam without delivering an imaging dose to other areas on the test chip. Navigation to the transistor of interest was accomplished by moving a known distance from a reference point on the die. Navigation between dice was accomplished by using the FIB system’s wafer map function. The ion dose was delivered to the sample surface above the test transistor. As shown in Fig. 1,the exposed area was somewhat larger than the transistor itself. Figure 1 is an optical photomicrograph of one of the 0.5 µm technology transistors with a 70µm x 70 µm FIB-exposed area indicated by the box. A square or rectangular region ranging from 40 µm x 40 µm to 100 µm x 100 µm in size (depending on the experiment) was used for the FIB exposures.


The desired dose per unit area was achieved either by using the FIB system’s milling function or by“grabbing” one or more single-frame images of the area of interest. The milling parameters (pixel spacing and pixel dwell time) were adjusted to match those used in grabbing single-frame images. The intent of the experiment is to simulate the exposure that occurs during “grabbing” images in the FIB system while navigating to an area of interest.


Table 1 Summary of Test Transistor Technologies


Technology Minimum Leff


Metallurgy


tox


Isolation Passivation Transistor Geometry


0.5 µm


Planarized, 3-level aluminum with W plugs


12 nm LOCOS


1.2 µm


phosphosilicate glass


W = 20 µm


L = 0.5, 0.6, 0.75,and 1.0 µm


12 nm Shallow trench isolation


0.225 µm


n-channel: 0.12+/- 0.04 µm


p-channel: 0.14+/- 0.04 µm


Planarized, 6-level copper


3.5 nm Shallow trench isolation


0.4 µm


Si3N4 over


0.45 µm SiO2


W = 9 µm


L = 0.225 µm


The ion dose delivered in a single-frame image, Do, is calculated from the expression Do = [(Ib)(td)/XpYp)],where Ib is the beam current in nA, td is the time (in seconds) that the ion beam dwells at each pixel, and Xp and Yp are the pixel spacings in the x- and y-directions.


In most experiments, the beam parameters used were td= 16 µs, Xp and Yp = 0.195 µm, and Ib = 660 pA. The pixel spacing corresponds to a 512 x 512 pixel image of an area 100 µm x 100 µm in size, or to a 256 x 256 image of a 50 µm x 50 µm area. Under these beam conditions, each raster scan delivers an ion dose of about 2.7 x 10-4 nC/ µm2 and removes less than a monolayer of material from the sample surface.


A set of experiments was conducted to compare the FIB effects resulting from “default” milling parameters and a different set of “image frame grab” parameters.


The Ib for these experiments was 1.7 nA. The parameters used for the “image frame grab” mills were Xp and Yp = 0.39 µm and td = 1 µs, and those used for the “default” mills were Xp and Yp = 0.02 µm, and td =5 µs. With these beam parameters, the dose delivered per raster in the “default” mill is almost 1800 times greater than by the “image frame grab” mill. The total number of rasters delivered at a given dose for the“default” mill is proportionally smaller. The total process time to deliver a given dose is the same for the two process types, and therefore the overall dose rate(total dose/time) is the same. However, the instantaneous dose rate increases for longer pixel dwell time and smaller pixel spacing, and is therefore considerably higher for the “default” milling condition.


Substrate


Figure 1 Optical image showing the FIB-irradiated


region (indicated by the white box) around a 20 x 0.6µm n-channel transistor. The bond pads are visible at the corners of the image.


We developed a special test structure to evaluate the effectiveness of an overlying metal structure in shielding a transistor from FIB-induced parameter shifts. The test structure is implemented in the 0.5 µm CMOS technology with LOCOS isolation and consists of unmodified n- and p-channel transistors as well as transistors with a metal pad completely covering the gate and active regions. A photomicrograph of one of the special transistors is shown in Fig. 2. All of the interconnections to the transistors are at the M1 level.


The metal shield is implemented at either M2 or M3 for a given transistor and is connected to the substrate(ground potential) while the other device terminals are floating. The area exposed by the FIB was 60 µm x 60 µm and was centered on the 75 µm x 75 µm shield.


Finally, we used scanning force microscopy (SFM) to investigate the effects of FIB exposure on the sample surface. Both topology and surface potential imaging were used in our study. This work was performed in a modified Digital Instruments Dimension 3000 system.


Shield


Figure 2 Optical image showing a test transistor with a shielding pad. The shield is tied to the substrate, which is at ground potential in our experiments.


Comparison of 30 and 50 keV Exposure


The effects of FIB exposure at 30 and 50 keV were studied for the 0.5 µm CMOS technology fabricated with LOCOS isolation. The area exposed by the ion beam was 100 µm x 100 µm, completely covering the transistor as well as some of the metal interconnections to the device terminals (see Fig. 1). The ion beam parameters were adjusted so that Ib = 660 pA at the two ion energies.


The only difference between the test conditions at 30 and 50 keV was the larger spot size at 30 keV. The other beam parameters were the same for both sets of experiments. The ion doses were 2.7 x 10-4, 5.4 x 10-4,and 2.7 x 10-3 nC/µm2, corresponding to 1, 10, and 20 individual “frame grabs”. The individual transistor terminals were floating and the substrate tied to ground.


Individual Id vs. Vg curves were collected for each of the transistors. An example of these data is given in Figure 3 for an n-channel, 20 x 0.6 µm transistor which received an ion dose of 5.4 x 10-3 nC/µm2. As before


[1], we found a general trend toward larger parameter shifts at smaller transistor geometry; for simplicity, we show results for just one geometry. The results for 20 x


0.6 µm n- and p-channel transistors are shown in Figs.


4 and 5. The changes in Vt (∆Vt = Vt post-FIB minus Vt pre-FIB) as a function of ion dose are fairly comparable for ion beam exposure at 30 and 50 keV. In general,the magnitude of ∆Vt is greater for n-channel than for p-channel transistors in this technology. Our results show that electron flood charge neutralization is highly effective in minimizing transistor parameter shifts at both 30 and 50 keV, consistent with our previous findings for 30 keV ion exposure for this material [1].


Figure 3 Pre- and post-FIB Id vs. Vg curves for an nchannel, 20 x 0.6 mm transistor which received an ion dose of 5.4 x 10-3 nC/µm2.


Figure 4 ∆Vt as a function of ion dose for 20 x 0.6 µm n-channel transistors at 30 and 50 keV FIB exposure,with and without electron flood charge neutralization.


The measurement error is ~ 0.003 V.


0.000


0.001


0.002


0.003


0.004


0.005


0.006


-1.6-1.4-1.2-1.0-0.8-0.6-0.4-0.2


floodgun


no floodgun


p-channel (20/0.6)


without floodgun:50 keV


30 keV


with floodgun:


50 keV


Total Ion Dose (nC/µm^2)


Figure 5 Changes in Vt as a function of ion dose for 30


and 50 keV FIB exposure of 20 x 0.6 µm p-channel


transistors, with and without electron flood charge


neutralization. The measurement error is ~ 0.003 V.


We also measured the effects of 50 keV FIB exposure on 20 x 0.6 µm MOS transistors fabricated with shallow trench isolation (STI). The beam conditions


were identical to those used for the LOCOS material,


and the results were very similar. The 50 keV results for both LOCOS and STI n-channel, 20 x 0.6 µm transistors exposed without electron flood charge


neutralization are plotted in Figure 6.


0.000 0.001 0.002 0.003 0.004 0.005 0.006


-0.4-0.2


n-channel (20/0.6)


0.6 µm LOCOS isolation


0.6 µm STI


Figure 6 ∆Vt as a function of ion dose for 20 x 0.6 µm n-channel transistors fabricated with both LOCOS and STI. FIB exposure was performed at 50 keV without charge neutralization. The measurement error


is ~ 0.003 V.


1.E-13


1.E-09


1.E-01


Vg (Volts)


post-FIB pre-FIB


n-channel (20/0.6)without floodgun:50 keV


Effects of FIB Exposure on 0.225 µm Technology


The effects of 50 keV ion beam exposure on test transistors fabricated in a 0.225 µm CMOS technology were also characterized. The results of exposure of 9 x


0.225 µm n- and p-channel transistors without charge neutralization are given in Figs. 7 and 8. The


difference in vertical scale between these figures (mV)


and Figs. 4 – 6 (V) should be noted. These results show no increase or decrease in the magnitude of ∆Vt with increasing dose for the 0.225 µm transistors, in contrast to the monotonic increase with dose observed for the 0.5 µm CMOS n- and p-channel transistors.


Furthermore, the magnitude of ∆Vt is at least two


orders of magnitude smaller than that observed for the


0.5 µm transistors. These 0.225 µm transistors have input protection diodes and also share a common gate


electrode with several other transistors. Thus, there are


several paths to dissipate the charge on the gate during


FIB exposure. In contrast, the 0.5 •m technology


transistors do not have these features.


0.000 0.002 0.004 0.006 0.008 0.010 0.012


-70-60-50-40-30-20-10 0 10


n-channel (9/0.225)no floodgun


Figure 7 Shifts in Vt as a function of ion dose for 9 x


0.225 µm n-channel transistors. Ion exposure was at 50 keV without charge neutralization. The measurement


error is ~ 3 mV.


-8-6-4-2 0 2 4 6 8 10 12


p-channel (9/0.225)no floodgun


Figure 8 Shifts in Vt as a function of ion dose for 9 x


0.225 µm p-channel transistors. Ion exposure was at 50 keV without charge neutralization. The measurement error is ~ 3 mV.


We also measured the effects of FIB exposure on another set of 0.225 µm n-channel test transistors that do not have input protection diodes but do have a common gate. For exposure with an ion dose of 5.4 x 10-3 nC/µm2 without electron flood charge neutralization, we observed ∆Vt values of approximately –0.12 V for the smallest transistor geometry (0.35 x 0.25 µm),and much smaller values (-0.02 V) for 10 x 10 µm transistors. These ∆Vt results show similar dosedependence but are still at least an order of magnitude smaller than those observed for the unprotected nchannel 0.5 µm technology transistors (Figs. 4, 6).


However, a direct comparison of the results of FIB exposure on these two technologies is not appropriate because of the many differences (e.g., design,processing, oxide thickness, and levels of integration)between them.


Effects of Shielding on Transistor Parameter Shifts


The results of FIB exposures performed on shielded 20 x 0.6 •m n-channel transistors are given in Table 2.


Table 2 Effect of Shielding on n-channel Transistors Ion Dose = 0.011 nC/µm2


Transistor


Type


Charge


Neutralization


∆Vt (V)


No shield


No


-0.4


M2 shield


0.049


M3 shield


0.065


No Shield


Yes


M2 Shield


-0.003


M3 Shield


FIB exposure was performed at 50 keV with a dose of


0.011 nC/µm2 both with and without electron flood charge neutralization. The data clearly show that the grounded shielding plate significantly reduced the magnitude of the parameter shifts even when charge neutralization was not used. For example, a substantial∆Vt (about 0.4 V) was observed for n-channel transistors when no shielding pad was present. With an M2 or M3 shielding pad, ∆Vt is 0.04 – 0.06 V. The use of electron flood charge neutralization further reduced the magnitude of ∆Vt to 0 – 0.006 V for the n-channel transistors with or without the shielding pads. The measurement error is ~3 mV.


Dependence of FIB Effects on Dose Rate


A set of experiments was performed to compare the results of the “image frame grab” and “default” mills described in the Experimental Approach section. Both n- and p-channel, 0.5 µm technology transistors fabricated with the LOCOS process were exposed to an ion dose of 0.02 nC/µm2 at 30 keV without electron flood charge neutralization. The results of this experiment are given in Table 3. Each table entry is the average of two measurements. The magnitude of ∆Vt for the n-channel transistors is about 35% larger for the higher instantaneous dose rate (“default” mill), but is about 25% lower for the p-channel transistors. The measured ∆Vt values were comparable at the two dose rates when the floodgun was used. In our previous study [1], ion exposure was performed entirely in the“image frame grab” mode. The dose rate was varied in one experiment by changing the ion beam current. In that case, the variation in transistor parameter shifts with dose rate for the same total dose were small [1].


Table 3 Effect of Instantaneous Ion Dose Rate


Ion Dose = 0.02 nC/µm2


Transistor type


W/L


Default Mill


Image Grab Mill


n-channel 20/0.5 1.35 ± 0.02


0.99 ± 0.002


n-channel 20/0.6 1.38 ± 0.03


1.07 ± 0.02


p-channel 20/0.5 -.48 ± 0.03


-0.68 ± 0.04


p-channel 20/0.6 -.49 ± 0.02


-0.72 ± 0.03


Effect of Exposed Area


The effect of the size of the area exposed to the ion beam on the magnitude of ∆Vt was also examined. In


this experiment, the same ion dose (10-2 nC/µm2) was delivered to two different sized regions (1600 µm2 and 6400 µm2) above the test transistors. The transistors with 80 µm x 80 µm exposure received 4x the amount of Ga+ ions as those with smaller area exposure.


Transistors built in the 0.5 µm technology with STI were used for these experiments, which were


performed at 50 keV. Table 4 shows that the magnitude of ∆Vt increases with exposed area for


transistors of two different gate lengths, and that the


effect is more pronounced for the n-channel transistors.


Table 4 Effect of Exposed Area on Parameter Shifts


Ion Dose = 0.01 nC/•m2


80 µm x


80 µm box


40 µm x


40 µm box


n-channel 20/0.5 0.769


0.259


n-channel 20/0.6 0.598


0.307


p-channel 20/0.5 -0.313


-0.237


p-channel 20/0.6 -0.311


-0.191


The data set in Table 4 is small, and thus additional experiments will be required for corroboration.


Physical Evidence of Damage


Scanning force microscopy was used to examine the passivation surface above several 0.5 µm transistors following FIB exposure at 30 keV. Packaged transistors were used for these experiments but no electrical connections were made to the device terminals. Imaging of the surface topology was performed following FIB exposure to look for evidence of physical degradation, and surface potential imaging was use to look for residual surface charge. The same field of view (40 µm) is used for the results shown in Figures 9 – 11.


Fig. 9 shows both topology and surface potential images of the passivation surface above an n-channel transistor that received a large ion dose of 0.5 nC/µm2 with electron flood charge neutralization. These images are featureless, indicating that the passivation surface is smooth and that no residual surface charging is apparent.


Figure 9 (a) Topology and (b) surface potential images of a planarized n-channel transistor after a high-dose FIB exposure of 0.5 nC/µm2 with electron flood charge neutralization. (a) and (b) are the same field of view.


The results were very different when charge neutralization was not used during milling. The topology image shown in Fig. 10a is of the FIBexposed area of the passivation. The RMS roughness of this area is 1 – 2 nm, with the exception of a few areas that resemble small “bumps” with a height of 5 –10 nm. These “bumps” were observed on the sample surface following an ion dose of 0.1 nC/µm2 and were not visible with optical or SEM imaging. Fig. 10b shows that the variation in surface potential of this area is very small following the 0.1 nC/µm2 dose exposure.


The same n-channel transistor received an additional


0.5 nC/µm2 dose, again without charge neutralization.


The additional FIB exposure apparently converted some of the “bumps” into “pits”, as shown in Fig. 11a.


In addition, residual charge was observed after the subsequent higher-dose exposure (Fig. 11b). The solid arrow in Fig. 11b indicates the area of greatest residual charge, which coincides with a “bump” visible in Fig.


11a (also indicated by a solid arrow). Four other areas with less residual charge are indicated by the dashed arrows in Fig. 11b. These areas coincide with “pit”location in Fig. 11b. The occurrence of a large residual charge at one of the “bump” locations suggests that charge build-up occurs at these locations prior to an electrostatic discharge (ESD)-like event. Subsequent electrical measure-ments indicated the presence of a gate oxide short defect in this transistor.


Figure 10 (a) Topology and (b) surface potential


images of a planarized n-channel transistor after FIB exposure of 0.1 nC/µm2 without electron flood charge neutralization. (a) and (b) are the same field of view.


Figure 11 (a) Topology and (b) surface potential


images of the same planarized n-channel transistor in Fig. 10 after an additional FIB exposure of 0.5 nC/•m2 without charge neutralization. (a) and (b) are the same field of view.


We have measured the effects of 50 keV FIB exposure on two similar 0.5 µm CMOS technologies and on a


0.225 µm CMOS technology. The size of the parameter shifts (∆Vt) obtained for the 0.225 µm technology are very different from those for the 0.5 µm technology, which is to be expected given the many


differences between these technologies, including gate


dielectric thickness, number of levels of integration


(and hence thickness of the stack), input protection diodes and common gate electrodes in the 0.225 µm technology transistors, and the materials used.


Our findings show that the amount of transistor


degradation at a given ion dose (measured by threshold


voltage shift) is comparable for 30 and 50 keV


exposures with the same beam parameters for a given transistor technology, as demonstrated for the 0.5 µm technology. We have also shown that the ion dose rate


and size of the area exposed have moderate effects on∆V. This indicates that the magnitude of the parameter shifts is related to the amount of sample charging and


charge-up rate rather than to the ion energy per se. The


main effect of energy observed to date is that the dose level which a transistor can sustain prior to failure (e.g.,by a gate oxide short) is reduced somewhat at the higher energy.


It should be noted that FIB exposure on the unshielded


0.5 µm transistors is truly a “worst case” situation.


These transistors are completely isolated, without the charge dissipation paths that would be present in a real IC. The 0.225 µm transistors with common gate electrodes and protection diodes are closer to the structures encountered in actual use condition. We have also demonstrated that metal shielding helps reduce the effects of ion beam exposure. A large fraction of the transistors in today’s ICs are at least partially shielded by overlying metallization lines and power buses.


We have performed most of the FIB exposures with a single ion beam current. This was done because the emphasis in this study was to compare the effects of FIB exposure at different ion beam energies and on different technologies. Ion beam current was a variable in our earlier study [1].


In practical terms, our findings indicate that it is always best to minimize the amount of FIB exposure of the sample if subsequent electrical operation is to be performed. Whenever possible, it is of benefit to navigate to the area of interest by using one or more of the available methods, including the use of known x-y coordinates of the area of interest and CAD navigation software. The use of measures to reduce sample charging, including electron flood charge neutralization and sample grounding, is always advisable.


Degradation Mechanism


It is known that charge accumulation can adversely affect transistor operation, causing effects ranging from subtle (and sometimes recoverable) parameter shifts to catastrophic (irreversible) damage of pn junctions and gate oxide. Charge accumulation on transistor electrical nodes and construction layers can occur both during fabrication (such as during plasma processes) and after fabrication due to testing, handling, and assembly electrostatic events. Excessive charge accumulation in the sample (enough to cause the electric field in the gate oxide to exceed a critical threshold) can result in Fowler-Nordheim tunneling of electrons from the silicon such that impact ionization generation of electron-hole pairs becomes significant. [3] . This in turn can result in a large density of oxide- and interface-trapped charge. The Ids-∆Vt charac-teristics for the 0.5 µm tech-nologies (see Fig. 3) exhibit a subthreshold stretchout following FIB exposure. Such


stretchout is associated with the presence of interface traps. The post-FIB Ids-Vgs characteristics for the 0.225µm technology exhibit essentially no change or small parallel shifts relative to their pre-FIB values. The latter condition is consistent with oxide-trapped charge.


A number of our findings indicate that the primary transistor degradation mechanism is due to the charging effect of the Ga+ ion beam. The effectiveness of the electron floodgun (which is used to provide a charge neutral surface and to effectively tie all transistor terminals to one potential) in minimizing parametric shifts strongly supports this hypothesis. Degradation effects are minimized with the incorporation of an overlying metal plate (which serves as a crude Faraday cage). When this plate is grounded during FIB exposure, it would cause the electric field between the deposited positive charge on the passivation and the silicon substrate to be significantly altered. As a result,the electric field in the vicinity of the transistor is reduced, and thus the likelihood for interface trap creation is much less. The diode-protected 0.225 µm technology transistors exhibit small degradations, while the unprotected devices show relatively larger parameter shifts. Clearly, the accumulated charge on the protected gates has an alternate path to the substrate, whereas the unprotected gates will dissipate charge almost exclusively through the gate oxide.


Additional support for charging as the primary degradation mechanism is found in the dependence on exposure area (∆Vt increased as the exposed area increased), independence of ion energy, and the occurrence of parameter shifts in a radiation-hardened CMOS technology (the STI 0.5 µm technology).


Perhaps the most compelling evidence for chargingrelated degradation is the physical evidence of damage to the passivation. Comparison of the SFM topology and surface potential images suggests that localized charge accumulation occurs in the high resistivity passivation prior to an ESD-like event resulting in a dielectric failure. However, ESD-like events can also be non-fatal [4-7]. High electric field transients can produce shifts in Vt and other parameters due to oxide and interface trapped charge. ESD events in packaged ICs have been observed to alter transistor parameters within the IC, beyond the common manifestations of current leakage or shorts in I/O protection circuitry. In several cases, it has been shown that the alteration of transistor behavior is due to charge accumulation on the passivation layer above the affected transistors [8-10].


The accumulation of charge can be localized, especially for high resistivity passivation materials. Alternatively,such local charging might occur if the charge generation rate is high compared to the dissipation or neutralization rate or if the dissipation or neutralization


mechanisms act in a nonuniform manner. The localized accumulation of charge on dielectric surfaces(“charge packets”) during ESD events has interesting parallels to the features observed in the SFM topology and surface potential images of transistors after FIB exposure.


Our previous experiments on biased capacitors indicated the occurrence of radiation-type damage in the FIB system [1]. We do not discount these earlier findings, but believe that they are a secondary or tertiary effect compared with degradation due to sample charging.


We have described our recent investigation of the effects of ion energy during FIB exposure on MOS transistors and have shown that the magnitudes of transistor threshold voltage shifts (∆Vt) are comparable for FIB exposure with 30 and 50 keV ions. We have shown that, while the effects of FIB exposure increase as transistor size decreases for a given technology, the observed ∆Vt are much smaller for a commercial 0.225µm technology than for a 0.5 µm research technology.


We have demonstrated that an overlying metallization shield reduces the magnitude of transistor parameter shifts as a result of ion beam exposure, and that both the instantaneous dose rate and area exposed to the ion beam play a role determining the magnitude of the transistor parameter shifts. Electron flood charge neutralization was found to be equally effective at minimizing ∆Vt at 30 and 50 keV. Finally, we have found physical evidence for the occurrence of localized charge buildup and subsequent electrostatic discharge in response to sample charging during FIB irradiation.


All of these findings are consistent with sample charging during FIB exposure as the primary degradation mechanism.


The authors thank the following individuals for their assistance with this work: Pete Czahor, Jim Shea, and Dave Hubanks of IBM Microelectronics; Michael Rye and Alejandro Pimentel of Sandia National Laboratories. The authors also thank Bruce Draper, Ed Cole, Jeremy Walraven, and Rich Anderson of Sandia for their careful review of the manuscript. Sandia is a multiprogram laboratory operated by Sandia Corporation, a Lockheed-Martin Company, for the United States Department of Energy under Contract DE-AC04-94AL85000.


1) A. N. Campbell, K. A. Peterson, D. M. Fleetwood,and J. M. Soden, “Effects of Focused Ion Beam Irradiation on MOS Transistors,” Proc. 35th Annual Internat. Rel. Phys. Symp., p. 72, April 8 –10, 1997


2) J. Benbrik, G. Rolland, P. Perdu, B. Benteo, M.


Casari, R. Desplats, N. Labat, A. Touboul, and Y.


Danto, “Focused Ion Beam Irradiation Induced Damage on CMOS and Bipolar Technologies,”Proc. 24th Internat. Symp. for Testing and Failure Analysis, p. 49, Nov. 15 – 19, 1998


3) D. J. DiMaria, “Temperature Dependence of Trap Creation in SiO2”, J. Appl. Phys. 68, 5234 (1990)


4) Y. Fong, and C. Hu, “The Effects of High Electric Field Transients on Thin Gate Oxide MOSFETs,”EOS/ESD Symp. Proc., p. 252, 1987.


5) G.C. Holmes, ”An Investigation into the Effects of Low-Voltage ESD Transients on MOSFETs,”EOS/ESD Symp. Proc., p. 170-174, 1985 EOS/ESD Symp. Proc., p. 252, 1987. EOS/ESD Symp. Proc., p. 252, 1987.


6) W. D. Greason and K.W.K. Chum,“Characterization of Charge Accumulation and Detrapping Process Related to Latent Failure in CMOS Integrated Circuits,” IEEE Trans. On Industry Applications, 30, 350 (1994)


7) J.C. Reiner, “A Physical Model for the Creation of Latent Gate Oxide Defects by Very Fast Electrostatic Discharges,” Proc. ESREF, p. 467,


1994.


8) R.E. McKeighen, W. Daily, T. Pang, P. Huynh, J.


Wittman, and B. Wiley, “Reversible Charge


Induced Failure Mode of CMOS Matrix Switch,”Electrical Overstress/Electrostatic Discharge


Symp. Proc., p. 69, 1986


9) M.H. Woods and G. Gear, “A New Electrostatic


Discharge Failure Mode,” Proc. 16th Annual


Internat. Rel. Phys. Symp., p. 146, 1978.


10) 10. R. Williams and M.H. Woods, “High Electric Fields in Silicon Dioxide Produced by Corona


Charging,” J. Appl. Phys., 44, 1026 (1973)


Electronic Device Failure Analysis Society, editor, p 285-292


DOI: 10.1361/cp1999istfa285


# Relay Failures Specific to Space Applications


Relay Failures Specific to Space Applications


Alexander Teverovsky


UNISYS/NASA GSFC Operations, Lanham, Maryland


Low-pressure conditions, as experienced in space applications, are considered benign for many electronic components. However, for switching devices the probability of failure may be significantly greater than at normal atmospheric pressure due to arcing-at-break processes. This study was stimulated by a relay failure in a 60-V power bus in a spacecraft module, and it was intended to analyze failure modes and the probability of their occurring under lowpressure conditions. The effects of gas pressure,power bus voltage, and load current on arc duration and probability of arc flashover have been investigated. It was shown that arc duration mostly depends on switching power and gas pressure,significantly increasing when power is rising and pressure is decreasing. Failure analysis indicated two major mechanisms in low-pressure conditions: (1)contact damage (excessive erosion and/or microwelding) and (2) arc flashover to a grounded case and/or grounded coil post. For a relay operating in a vacuum, the effect of leak rate on the time to failure at low-pressure conditions is discussed.


Telemetry data indicated the failure of a 60-V power bus in a spacecraft module. The failure occurred during the first switching of a relay, and it caused a 10-A fuse in the bus power distribution unit to blow open.


One conceivable failure scenario involved the possibility of transient case arcing (arc flashover) in a hermetically sealed relay used in the module. No indication of arc flashover was observed under vacuum and normal pressure conditions during


multiple testing of the module before launch.


However, it is possible that a fine leak in the relay may have decreased internal air pressure while the module was operating in space.


Although failures due to arc flashover in relays are well known since the 1960’s [1], the mechanism of this process is not completely understood. In particular, the effect of low-pressure conditions on relay arcing and the possibility of flashover failures has not been adequately addressed in technical literature. Obviously, this low-pressure condition is of particular interest for space applications.


This work analyzes arc flashover in hermetically sealed latching relays operating in vacuum and estimates effect that a hermetic-seal leak has on this phenomenon. For this purpose, the effects of internal air pressure (ranging from 760 torr to 0.2 torr), power bus voltage (12 V to 60 V) and load current (0.2 A to


3.5 A) on arc-at-break duration and relay failures were investigated.


The setup used to simulate conditions in the bus power distribution unit is shown in Figure 1. A power source was created by combining five car batteries in series, allowing voltage to vary in 12-V increments up to 60 V dc. Standard 10-A/250-V CSA/UL-F fuses were used to detect flashover events. Load current was adjusted from 0.24 A to


3.6 A using 200-W wire-wound resistors.


Inductances of these resistors are listed in Table 1.


Wires of 12 AWG type with lengths of approximately


2.1 m (7 ft) were used to connect the circuitry. A straight wire of this length has an inductance of approximately 1.5 µH. Inductance of the ammeter was 0.23 µH. Total inductance in the circuit


depended primarily on the resistor used, but it was relatively low (≈ 90 µH maximum). The impact of the circuitry inductance is discussed later.


Three hermetically sealed latching relays were used in this study. The contacts in these relays were rated for 12-A resistive load at 28 V dc. According to the manufacturer application note, it is possible to derate the contacts for higher dc voltages provided lower currents are used during switching. At 60 V, the calculated current limit is 3.73 A.


Table 1 Inductances of Resistors Used in the


Experimental Setup


Resistance


Inductance


5 Ω


19 µH


wire-wound


10 Ω


20 µH


0.5 µH


carbon


20 Ω


40 µH


50 Ω


87 µH


The movable relay contacts were connected to the positive battery terminal. Arc duration, θ, was monitored with a current probe and an oscilloscope.


The sample was switched five times at each combination of experimental parameters, and mean values and standard deviations of θ were analyzed.


Small holes were drilled in the relays before installing them in the vacuum chamber to permit pressure equalization.


Figure 1 Block diagram of the test set-up.


Atmospheric Pressure Condition


A typical transient oscillogram measured at contact break under normal conditions in the 60-V/3-A circuit is shown in Figure 2. Duration of the arc for all tests was in the range of 2.2 to 2.7 ms, and it did not vary more than approximately 20% during switching.


Two relays with cases removed were examined under a low-power microscope during operation. Bright arcing was observed for both relays at the moment of contact break. The arcing, which was reproducible,was localized at a certain area between the contacts.


The arcing was visible even when the load resistance was increased, causing the current to decrease from 3 A to 1.7 A, 1.15 A, and even to 0.9A (at 70 Ω). This is consistent with the minimum arcing current of silver contacts which is generally considered to be about 0.4A [2].


Figure 2 Typical transient oscillogram at contact


break (60 V/3 A) at atmospheric pressure.


Low-Pressure Conditions


Preliminary Experiments. The first 60-V/3-A experiment (first contact break), conducted with sample SN 1 (contacts B1-B2) at an internal gas pressure of 1 torr, resulted in a blown fuse, indicating that a flashover event had occurred. The fuse was replaced, and the experiment was repeated with the same result (i.e., the second 10-A fuse was blown open). Following the fuse change, the chamber valve was opened, and testing was conducted at atmospheric air pressure. No fuses blew during multiple switching tests. The transient current oscillograms at contact break and the arc duration were found to be similar to those observed during the initial test, thus indicating that no damage to the relay had occurred during flashover events.


The experiments were continued using the A-side contacts. No failures occurred during multiple switching at low-pressure conditions. Arc behavior was much less stable than at atmospheric pressure,


and θ varied from 15 ms to 1.1 s. Figure 3 shows an example of the transient at contact break in the lowpressure condition.


Figure 3 Transient at break (60 V/3 A) at air pressure of 6 torr, SN 1.


Experiments with contacts B1-B2 were continued,first at normal conditions (atmospheric pressure) and then in the vacuum chamber (6 torr). No failures occurred in the experiments conducted at atmospheric pressure and during the first seventeen switchings at low-pressure conditions.


But the eighteenth switching blew the third 10-A fuse. The flashover event (see Figure 4) occurred approximately 15 ms after arc ignition (θ ≈ 40 ms). After this event, the relay failed open (it was not latching).


Figure 4 “Blowing fuse” event in SN 1 at contact


break (60 V/3 A) in vacuum chamber at 6 torr;


current was measured between case and ground.


Effect of Air Pressure. Two samples were tested at various pressures in the vacuum chamber at the 60-V/3-A condition. Similar to SN 1, arc duration at low-pressure conditions was much longer, less reproducible, and significantly noisier with spikes up to 2 A peak. No fuse blowing occurred during these experiments.


The arc-duration-pressure (θ-p)relationship had an extremum at approximately 10


torr (see Figure 5). Similar extremal behavior of theθ-p dependence was expected. The arc is known to be suppressed at high and low air pressures, and these


effects are used in practical design of vacuum and


high-pressure circuit breakers. However, the range of air pressure that would cause significant increase in θ for the JL type relays was not known. Based on Figure 5 and assuming a 5-times increase in θ(compared to atmospheric pressure) as significant, the low-pressure condition range can be defined between approximately 1 torr and 200 torr.


Sample SN 2 failed (the contacts stuck closed) during experiments at 19 torr after sustaining an arc for about a second.


Figure 5 Arc duration variance with pressure for


60-V/3-A condition.


Effect of Current and Voltage. To avoid possible damage to the contacts by long arc duration at pressures between 1 torr and 200 torr, these experiments were performed first at atmospheric pressure and then at 0.4 torr. Sample SN 3 was switched first at minimal voltage (12 V) while changing load resistors in the sequence 50, 20, 10,and 5 Ω. Then, the voltage was increased in 12-V increments to 60 V. The results of measuring mean θ as a function of the short-circuit current, I, for various power supply voltages are shown in Figure 6. A power function was used to describe θ(I) variance:


= I0θ


where α and θ0 are parameters. Parameter θ0 increases with the power supply voltage, whereas α is relatively independent of current and voltage (above 12 V), but it increases from 0.6 to 0.9 at atmospheric pressure to 3.6 to 5.2 at the internal air pressure of


0.4 torr.


Figure 6 Arc duration at break vs.


short-circuit current.


The flashover event (10-A-fuse blowing) occurred during the second switch at 0.4 torr and the 60-V/3-A condition. The oscillogram of this event was similar to Figure 4. This time, the flashover occurred in 5 ms, whereas the arc duration was 23 ms in length.


Blowing of the fuse coincided with failure of the relay that stuck open.


Effect of Circuitry Inductance. Experiments with the carbon and wire-wound resistors showed that inductance of the 10-Ω resistors did not significantly affect duration of the arc (θcarbon ≈ 940 µs, θwirewound ≈ 900 µs). This suggests that circuit inductance, L, in the range of tens of microhenries can be considered as negligible. On the other hand, it is known [3], that an increase in the load inductance above ≈0.2 mH substantially increases the arc duration (i.e., approximately 10 times). The following approximate calculations facilitate estimation of the condition at which the load can be regarded as resistive.


Energy dissipated during the arcing period θ is:


where Va and Ia are the voltage and current of the arc.


Analysis of the arc oscillograms suggests that arc current and voltage in these experiments can be roughly assumed as constants that are equal to fractions (30%-60%) of the load current and switching voltage. This facilitates estimating Wa ≈kVIθ, where k is an empirical coefficient, k ≈ 0.1-0.4.


Obviously, if the arc energy is much larger than the energy stored in the circuit inductance (WL = 0.5LI2),the inductance effect can be neglected. This gives the following equation for a “negligible” inductance of the circuitry:


<<


kR


I kV


where R is the load resistance.


Typically, arc duration was in the millisecond range at the 60-V/3-A conditions. At these conditions the above estimation gives L<< 4 mH. This means that inductance of the circuitry with any of the resistors used in the experimental setup can be considered as negligibly low. The shortest arcs (in the microsecond range) occurred at low air pressure with minimal load currents (load resistance = 50 Ω). At this condition the negligible inductance should be below 10 µH. As the 50-Ω resistor had L ≈ 90 µH, this circuit inductance should affect arc duration. This most likely explains the higher-than-expected (according to the power law) values of arc duration in the 12-V/50-Ω experiments (see Figure 6b).


Analysis of the low-inductance criterion (Equation 3)shows that arc duration depends on the circuit inductance in the microsecond range of θ. To analyze resistive-load conditions, we will consider results with θ > 100 µs. Besides, this range of θ corresponds to the gaseous phase of arc where the internal air pressure is expected to affect the arcing process [4].


Sample SN 2, which failed without the arc flashover,had a melted movable contact (anode) that was fused to the stationary contact. Appearance of this damage was typical for a contact failure caused by excessive power dissipation (excessive arc duration in our case).


A polymer cap (arc suppressor), which isolated the contact area from the case, had evidence of severe overheating and burning, confirming excessive power dissipation during arcing.


Sample SN 1 had a melted armature which had developed a bump in the area above the post X2.


This post and the welded coil wire were partially melted (see Figure 7). Appearance of the damage suggests that flashover occurred between the armature(connected to the movable contact) and the grounded coil post. The damaged site was approximately 8 mm from the normal location of the arc (between the silver contacts). However, the polymer cap had dark burned spots indicating overheating at the silver contacts, and both (A and B) movable contacts had evidence of excessive erosion. These defects most likely were caused by excessive power dissipation during relay switching under low-pressure conditions.


Internal examination of SN 3 revealed a melted post with a fused spring and melted glass at the periphery of the glass seal around the stationary contact.


Figures 8 and 9 show damaged sites in this relay. The damage appearance suggests a breakdown (arc flashover) between the post connected to the armature and the header. The damaged area is at a distance of approximately 5 mm from the silver contact location.


The polymer cap had a dark burned edge near the stressed contacts.


Figure 7 SN 1 failed at 60-V/3-A circuit break in vacuum chamber at 6 torr due to a flashover between the armature and the grounded coil post.


Figure 8 SN 3 failed at 60-V/3-A circuit break at an air pressure of 0.4 torr due to a flashover between the post connected to armature and the case. The black


area on the case is an arc track. A white arrow


indicates damage to the glass seal (see below).


Figure 9 Close-up view of the melted glass seal


shown above.


It is believed that flashover is caused by the ionized gas diffusing from the between-contacts arc column to the surrounding case or header [1]. This diffusion can initiate a gas breakdown between the contact and the case, and although it may not cause damage to the relay, a failure of the circuit is quite possible. In this sense, a similar event can be considered as a relay failure.


Types of gas molecules and gas pressure significantly affect the arcing process. Data reported by Holm [2]indicate that the arc can be sustained to much wider contact separations at low air pressures (10 torr – 100 torr) and that arc durations may be correspondingly longer than at normal atmospheric conditions. Also,arc behavior changes at low pressures. The arc


column becomes wider, its temperature decreases (at pressures below approximately 10 torr), and the longitudinal potential gradient of the arc in inert gases has a minimum at approximately 2 torr [5].


Our experiments showed that flashover failures occurred within several milliseconds after switching.


This indicates that duration of the arc may have a significant effect on the probability of flashover. Arc duration is governed by a complex processes taking place in the gaseous phase of the plasma.


At relatively low electrical switching levels (I<3 A and V<50 V), the gaseous phase of arcing, which follows the metallic phase, starts after 200-300 µs,when the contact separation reaches approximately 100 µm [4]. The process is controlled by electron emission from the cathode spots which ionizes gas molecules and thus sustains a plasma. The cathode spots are in permanent chaotic movement from site to site along the electrode surface (probably due to the silver oxide decomposition being caused by the hightemperature plasma [6]). This shifting of the cathode spot constitutes a weakening and subsequent restoration (reignition) of the arc [2]. The reignition process is attended by plasma bursts that cause spikes and noise in the arc current. Similar plasma bursts can probably ignite the gas breakdown causing flashover failure provided the cathode spot is in a suitable location and the burst is powerful enough.


Acceleration of the cathode spot motion as gas pressure decreases[6] may also increase the probability of finding a suitable location to initiate this breakdown.


According to this model, an increase in arc duration increases the probability that the plasma burst (which initiates the breakdown) will occur. Correspondingly,the same factors that cause an increase in arc duration are favorable for flashover failures.


It should be noted that an increase in θ increases the energy dissipated in the arc and correspondingly enhances the probability of a “regular” failure event(such as contact erosion and microwelding). This may result in a “regular” failure occurrence before the flashover event.


Arc Duration


Arc duration is mostly considered to be a function of the short-circuit current, I. Two types of arcduration-versus-current laws are usually used to represent θ(I) functions: an exponential law and a polynomial law [7]. Although none of the functions has received the necessary theoretical justification,


the exponential function is mostly used to describe processes in the metallic phase of arcing [4, 8],whereas a power function better describes arcing in the gaseous phase. Our experimental data, which are presented in Figure 6, seem to confirm this conclusion.


An increase in power supply voltage, V, is also known to increase θ, but θ(V) dependencies have not received much consideration. The minimal voltage that is necessary to start acing in relays is about 10 V [2]. This is explained by the fact that to start ionization at contact break, electrons must gain sufficient energy to overcome the energy barrier in the metal electrode and to ionize the metal vapor. As the work function for silver is ϕ = 4.3 eV (for silver oxide, it is less, ≈ 1-1.2 eV) and ionization potential of silver atoms (vapor phase) is Vi = 7.5 V, the minimum voltage necessary to start an arc is Vmin ≈ϕ/e + Vi ≈ 9-12 V. Ionization of the gas atoms and molecules requires more energy, so it, correspondingly, occurs at higher voltages. For example,the Vi values for oxygen and nitrogen molecules are


12.1 V and 15.6 V, respectively. Ionization of helium requires 24.5 V. Several tens of electron-volts are required to strip electrons from internal levels of atoms and molecules. Ben Jemaa and coworkers [4, 8] have proven that the arc voltage in the gaseous phase goes through several stages with voltage plateaus that are specific for various types of gases and that are related to their ionization potentials. This mechanism explains changes in theθ(I) relationship when the power supply voltage was increased from 12 V to 24 V (see Figure 6). The increase in voltage intensifies gas ionization,facilitates the arc-reignition process, and correspondingly increases arc duration.


In the range of currents and voltages used, an increase in both external parameters of the arc, V and I,resulted in a rise of θ, with both parameters having a similarly appreciable effect. This implies that a switching power, P=IV, may be used as a single parameter relating to arc duration. Figure 10 shows the θ(P) variance at atmospheric pressure and at


Figure 10 Arc duration variance with switching


power at various internal pressures in the relays.


It is apparent that θ is relatively independent of load resistance and, correspondingly, of the power supply voltage. At θ > 100 µs, the θ - P relationship can be approximated with the power law:


AP


where A and n are constants.


Calculations gave n = 2.8 for the low-pressure condition and n = 1.4 for the atmospheric-pressure condition. At the low-pressure condition θ increases with power much faster, and above approximately 80 W, arc duration exceeds the corresponding values for the normal-air-pressure condition.


Internal Gas Pressure in Leaking Relays


A decrease in the internal gas pressure with time in a leaking relay can be approximated by an exponential function:


where p0 is the initial (atmospheric) pressure, τ =p0V/L, V is the relay volume (cm3), and L is the standard air leak rate (atm•cm3 /s).


The internal free volume, V, of the relays was estimated at approximately 3.6 cm3. Time dependency for the internal gas pressure in relays with air leak rates in the range from 10-5 to 10-11 atm•cm3/s are shown in Figure 11.


The low-pressure condition (below 200 torr) can be reached in less than 10 years if the leak rate exceeds 10-8 atm•cm3/s of air. The value of 1x10-8 atm•cm3/s of air is used as a rejectable limit for re-lays with internal volume of less than 33 cm3 (2 in3) (per MILR-6106). Although this limit is much more severe(more than two orders of magnitude) than the one that is used for microcircuits, it is justified in the light of the described low-pressure condition failures.


The helium leak test is usually used to confirm the required level of the relay hermeticity. With the standard air leak rate, L, the measured leak rate of the tracer gas (He), R1, can be calculated using the well known formula [see, for example, 9]. Calculations showed that to provide the standard leak rate L =1x10-8 atm•cm3/s of air, the measured leak rate for the part, R1, should be less than 1x10-11 atm•cm3/s of He. This value is near the detection threshold of regular helium leak detectors. Besides, in many instances helium desorption from paint on the relay masks a real leak from the case, thus giving an effective leak rate of more than 1x10-8 atm•cm3/s of He. If the real (from the case) leak rate is approximately 1x10-8 atm•cm3/s of He, then the corresponding standard air leak rate would be 3x10-7 atm•cm3/s, and the low-pressure condition would be reached in a few months.


These estimates show that in real life, use of a leaking relay is quite possible despite stringent screening of parts intended for space applications. Such a relay may cause a circuit failure provided the time of its operation in vacuum is within certain limits such that internal pressure is below ≈200 torr, but above≈0.3 torr. A longer vacuum operation time further decreases air pressure and, thus, reduces the possibility of the arc-related failures.


Figure 11 Calculated gas pressure in a leaking relay in vacuum; Leak rate, L, varied from 10-5 to 10-11 atm•cm3/s of air.


1. A decrease in internal air pressure in relays significantly increases the probability of failures caused by arc flashover and/or contact damage.


Under favorable conditions, a flashover can occur even at the first relay switching (contact break), thus resulting in a single-event catastrophic failure.


2. For the examined relays rated for 12-A/28-V service, flashover failures occurred while breaking a 3-A/60-V resistive-load circuit at pressures between 6 torr and 0.4 torr. The gas breakdown (flashover) occurred 5 to 15 ms after arc ignition. Damage appeared between the armature and grounded coil post or relay header at distances 5 to 8 mm from the contacts.


3. Arc duration significantly increases when internal pressure decreases, reaching a maximum at approximately 10 torr (from 2 to 3 ms at atmospheric pressure to timespans of seconds at low pressure). Excessive arc duration (more than 20 to 30 ms) at low-pressure conditions (between approximately 200 torr and 1 torr) resulted in excessive erosion and/or micro-welding of electrodes and in overheating of polymer caps(arc suppressors).


4. The power supply voltage (in the range 24 V to 60 V) was found to have a similarly significant effect on arc duration as did the short-circuit current (in the range 0.5 A to 3 A). Within these ranges, arc duration mostly depends on switching power, and at P > 10 W, arc duration can be approximated with the power law: θ = APn with the power coefficient n being larger for the lowpressure condition (n = 2.8 at 0.4 torr) than for atmospheric-pressure condition (n = 1.4). Above approximately 80W, arc duration at the lowpressure condition is longer, correspondingly increasing the probability of the relay failure.


5. Increased arc duration and flashover failures


suggest that the internal air pressure range from


0.3 torr to 200 torr can be considered as a highrisk region. Estimates showed that internal


pressure in relays with leaks greater than 1x10-8


atm•cm3/s of He can reach this critical region in


less than a year when operating in vacuum.


The author would like to thank John Slonaker, Scott Hull, Frederick Felt and Steve Esmacher for useful discussion and for review of this manuscript. The reported work was performed at Goddard Space Flight Center Parts Analysis Lab, and it was supported by the Office of Systems Safety and Mission Assurance (OSSMA, code 562).


1) J. Lawrence, Application notes for preferred parts and materials, NASA, GSFC (1965).


2) R. Holm, Electric Contacts Handbook, p. 309,Springer Verlag, (1958).


3) N. Ben Jemaa, L. Nedelec, S. Benhenda, IEEE Trans. on CPMT., part A, v. 19, 82 – 86 (1996).


4) N. Ben Jemaa, J.L. Queffelec, D.Travers, IEEE Trans. on CHMT, v. 14, 113 – 117 (1991).


5) J.M.Somerville, The electric arc, p. 19, John Wiley & Sons Inc., NY (1959).


6) I.G.Kesaev, Cathode process in the mercury arc,p. 49, Consultants Bureau, NY (1964).


7) Handbook of vacuum arc science and technology,edited by R.L.Boxman, D.M.Sanders, P.J.Martin,p. 116, Noyes Publications, New Jersey (1995).


8) N. Ben Jemaa, J.L. Queffelec, R.Haug, J.Phys.


D: Appl.Phys., v.20, 468-475 (1987).


9) Electronic materials handbook, v. 1, p. 1063,Packaging, ASM International (1989).


Electronic Device Failure Analysis Society, editor, p 293-296


DOI: 10.1361/cp1999istfa293


# Failure Analysis of Autoclave-Stressed SRAMs with Aluminum Fuses


Failure Analysis of Autoclave-Stressed SRAMs with Aluminum Fuses


Jamey Moss, Sam Subramanian


Motorola, Austin, Texas


C. M. Chan


Motorola, Kuala Lumpur, Malaysia


Vince Soorholtz, Michael Thomas, Mark Gerber


Several hundred units were subjected to autoclave stress as part of the qualification of a new fast static RAM. Many units failed after autoclave stress, and these parts recovered after conventional depotting using nitric acid and a hot plate. Based on the recovery of the units, the failures were determined to be fuse-related because the nitric acid cleared the fuse cavities during depotting. Chemical analysis after thermally extracting the die from the package revealed an antimony-rich material in failing fuse cavities. Source of the antimony was linked to antimony trioxide added to the plastic package as a fire retardant. However, it was unclear whether the antimony-rich material caused the failure or if it was an artifact of thermal depotting. A new approach that did not thermally or chemically alter the fuse cavities was employed to identify the failing fuses. This approach used a combination of back-side grinding,dimpling, and back-side microprobing.


The antimony-rich material found in the fuse cavity was confirmed using SEM and TEM-based EDS analysis,and it is believed to be a major contributing factor to fuse failures. However, it is unclear whether the short was caused by the antimony-rich material or by a reaction between that material and residual aluminum(oxide) left in the fuse cavity after the laser blows.


As part of the qualification of a plastic-packaged fast static random-access memory (SRAM) with aluminum fuses, several hundred units were subjected to autoclave stress. Autoclave stress is an environmental test to determine the effects of moisture penetration through the package and corrosion on the die. The conditions are 121°C,


100% relative humidity, and 103 kPa (15 psig) for 168 hours. The parts are removed from the oven after a specified period of time and tested, and failures are isolated and sent for failure analysis. Several units failed functional testing for four rows each.


The first step after verifying the failure on a memory tester was to expose the die surface by chemically depotting a few parts using nitric acid and a hot plate.


The depotted units then passed all functional tests.


Two possible explanations for the recovered devices were that the heat from the hot plate affected the defect or the chemicals involved in depotting (nitric acid, acetone) altered the defect. A few failing devices that had not been depotted were baked in an oven for 24 hours at 150°C, but no units recovered,indicating that heat alone was not responsible for the recovered failures.


In most static RAM devices, some manufacturing defects can be repaired using fuses to decode redundant elements in the array of memory cells. The fuses are blown by a laser after probing the wafer to identify the defective regions of the device. It was determined that on each of the depotted recovered units, the four failing rows corresponded with a fuse that had been blown to repair a manufacturing defect.


The above analysis implied that blown open fuses were being shorted during autoclave stress, thereby causing four-row failures. Clearing the shorting material out of the fuse cavities when depotting the die with nitric acid is believed to enable the part to pass functional tests again. However, the mechanism by which the fuses were shorted was unclear.


To facilitate understanding the mechanism, it was necessary to examine the blown fuses without removing the contents of the fuse cavities. Hence, dice from the next batch of failing units were extracted from their packages without using chemicals. To remove the die, the back side of the package was ground away while leaving the top of the package intact. Then, the remaining plastic package was thermally softened using a glass rod heated to several hundred degrees Celsius,and the die was extracted with tweezers. A scanningelectron microscope (SEM) image of fuses on a chemically depotted die is shown in Figure 1(a), as compared with an SEM image of fuses on a unit thermally removed from the package, as shown in Figure 1(b). The blown fuses believed to be causing the four-row failure were microprobed from the top side to identify the shorted fuse. The failing fuse had a resistance of only 17 kΩ, while open fuses had resistances of well over 500kΩ.


Figure 1 (a) Top-down SEM micrograph of clean blown and unblown fuses.


Figure 1 (b) Top-down SEM micrograph of fuses on the thermally decapsulated die with mold compound components in the fuse cavities.


Traditionally, fast static RAM devices have had polysilicon fuses, which have very low electromigration properties compared with aluminum. The main reliability concern of these failures was that the blown aluminum fuses were electromigrating and regrowing during the pressure and temperature stress of the autoclave test. However, SEM and transmission-electron micro-scope (TEM)-based energydispersive spectroscopy (EDS) analysis of the failing fuse showed excessive antimony content and small amounts of mold-compound components, such as phosphorus and bromine, in and around the fuse cavities, but no aluminum. It should be noted that it is difficult or impossible to detect a small quantity of light atomic weight aluminum in a high atomic weight antimony-rich area by EDS analysis. The problem is also complicated by overlapping aluminum and bromine peaks in an EDS spectrum.


The source of antimony was linked to the antimony trioxide added to the plastic package as a fire retardant. A literature search also showed that a previous study by Gallo et al. [1] demonstrated the tendency for antimony trioxide from plastic packages to react with aluminum bond pads during autoclave stresses. A similar reaction between antimony trioxide and aluminum splattered during the fuse blows was suspected. However, microstructure of the antimony-rich material in the fuse cavities, analyzed using a TEM, indicated a nanocrystalline phase embedded in an amorphous matrix as shown in Figure 2. The gap between the antimony-rich material and the walls of the fuse cavities indicated poor adhesion and agglomeration. It was unclear whether the agglomerated state of the material was real or a result of extracting the die from the plastic package by applying excessive heat. The plastic in the package decomposes when heated above the combustion temperature, leaving behind combustion by-products. Since antimony trioxide is added as fire retardant, it is expected to remain as a residue. In such a case, the antimony-rich material observed in the fuse cavities may have been modified during extraction from the package. Hence, it was necessary to develop a new approach to identifying and examining the failing fuses that would ensure integrity of the fuse-cavity content. A combination of conventional front-side microprobing and a novel back-side microprobing approach was developed to resolve this issue.


Figure 2 A cross-sectional TEM micrograph of the shorted fuse in a thermally decapsulated die. The material in the fuse cavity appears to be


agglomerated, and it exhibits poor adhesion to the


walls of the fuse cavity. EDS analysis reveals


antimony-rich material with small amounts of moldcompound components, such as phosphorus and bromine.


Top-Side and Back-Side Microprobing Procedures


In this approach, a small region of the top surface of the die far away from the fuses was chemically exposed, and probe pads were placed on related circuitry using a focused-ion-beam (FIB) system.


The circuitry was microprobed to identify the failing fuse, and the exposed die was backfilled with super glue. The part was then ground from the back side on a grinding wheel to within 30 to 50 µm of the fuses.


To stop the back-side grinding within 30 to 50 µm of the fuses, the part was ground at a slight angle, with the thickest part of the die over the fuse location.


When the thin part of the die was ground down to expose the circuitry, the thickness of silicon over the fuse was estimated based on the grinding angle and the distance to the nearest exposed circuitry.


For the final approach to the fuse bank from the back side, a specific area dimpling technique was used. To create dimples in the silicon, a dimple grinder was used; this tool consists of a rotating grinding disk(30 mm diameter × 2 mm thickness) with an abrasive edge and rotating circular base. Axes of rotation of the grinding disk and base are perpendicular to each other. To create a dimple, the die is glued to the base,which is rotated by a motor. The abrasive edge of the grinding disk is placed in contact with the die, and the perpendicular rotations of the base and the disk result in controlled dimpling and removal of silicon. Such


dimplers are frequently used for TEM sample preparation, and they are commercially available.


Depth of the dimple can be controlled to within±2 µm using these dimple grinders.


In this work, an estimate of the exact thickness of silicon remaining on the back-side-ground die was made by dimpling a region close to the area of interest until the circuitry in that region was exposed.


Using the thickness estimate, another dimple was made in the silicon on the exact location of the fuse bank, stopping about 3 to 5 µm above the fuse. A visible-light image of the fuse bank through the thin transparent silicon is shown in Figure 3.


Figure 3 An optical image of a fuse bank containing


five fuses, one of which is identified. This image shows the fuses as seen through the substrate from the


back side, after back-side grinding and dimpling,


recorded through 2 to 5 µm of silicon.


Using the FIB, probe pads were placed from the back side on both the failing (shorted) fuse and the known good (open) blown fuses. To place the probe pads without shorting through the silicon substrate, a hole was milled to the metal connection of the fuse, then backfilled and oversprayed with an insulator (silicon dioxide). Then, the bottom of the hole was milled opened to expose the fuse connection, and a platinum probe pad was deposited on top of the insulator layer.


The fuses were then microprobed to confirm the failing state of the fuse. Again, the failing fuses had resistances of 17 kΩ to 35 kΩ, while open fuses had resistances of well over 500 kΩ.


Findings


Cross-sectional SEM, TEM-based microstructural,and EDS analyses were performed to analyze contents of the fuse cavities. SEM and TEM micrographs are shown in Figures 4 and 5, respectively. EDS


analysis confirmed excessive antimony in the failing fuse cavity. The source of antimony in the plastic package is antimony trioxide, but it is unknown whether the antimony-rich material found in the fuse cavities is pure antimony or antimony trioxide. The antimony-rich material was found in many fuse cavities that contained blown aluminum fuses, but was not found near unblown fuses. The amount of antimony-rich material in the fuse cavity with the shorted blown fuse was much higher than that found in cavities with open fuses.


Figure 4 A cross-section SEM micrograph of the failing fuse with antimony-rich material filling the fuse cavity.


Figure 5 A cross-section TEM micrograph of a


failing fuse with antimony-rich material partially


filling the fuse cavity. The antimony-rich material was crystalline, and it adhered well to the walls of the fuse cavity.


Fuses are blown open by a laser, and the intense energy of the laser vaporizes the fuse and possibly splatters a coat of aluminum (oxide) around the fuse cavity. However, the laser blow does not leave enough pure aluminum to form a conductive path in the original fuse circuitry. Back-side grinding,microprobing, and cross-sectioning procedures were repeated on several units, with SEM and TEM cross sections both across and along the fuses. No conclusive evidence of residual aluminum “stringers”was found in any of the failing fuse cavities.


Antimony trioxide, which is slightly soluble in water


[1], is believed to leach out of the plastic package during autoclave stress and collect around blown-fuse cavities. Exact nature of the antimony-rich material in the fuse cavity is not known, and it is unclear whether resistance of antimony trioxide is low enough to cause a short of this nature or antimony trioxide reacts with residual aluminum (oxide) to form another compound with lower resistance, thereby causing a short.


After extreme environmental stresses, several devices with aluminum fuses had failures related to shorted blown fuses. Traditional attempts at accessing the die surface to find the root cause of the failure actually eliminated the source of the short, recovering the devices to full functionality. To determine the cause of the short, a new approach was developed, which included functional top-side microprobing, back-side grinding, dimpling, and microprobing on silicon.


Using this technique, failing fuses were identified and cross sectioned for SEM and TEM-based EDS analysis. The root cause of the short in the fuse was linked to a reaction between antimony (trioxide) rich material that leached out of the plastic package. It is unclear whether the short is directly caused by the antimony-rich material or indirectly through a reaction between the antimony (trioxide) and residual aluminum (oxide) left from the blown fuse.


1) Effect of Mold Compound Components on Moisture-Induced Degradation of GoldAluminum Bond Pads in Epoxy Encapsulated Devices, A.A. Gallo, 28th Annual Proceedings,Reliability Physics, p. 244-251, 1990.


Electronic Device Failure Analysis Society, editor, p 297-304


DOI: 10.1361/cp1999istfa297


# Electrostatic-Discharge (ESD) Failures in Thin-Film Resistors


Electrostatic-Discharge (ESD) Failures in Thin-Film Resistors


Scott M. Hull


NASA/ Goddard Space Flight Center, Greenbelt, Maryland


Field failures of nichrome thin-film resistors have been investigated recently for several pieces of spaceflight hardware. These failures have involved resistance shifts ranging from a few percent to complete open circuits. Failure analysis and duplication of these failures have revealed that the failures were caused by electrostatic discharge. The failure characteristics and the circuit conditions necessary for failure have been studied for several types of thin-film resistors, including nichrome and tantalum nitride resistive elements. The effects of latent damage and resistive pattern design will also be discussed.


Failure Analysis Experience1


This investigation into the sensitivity of thin-film resistors to damage from electrostatic discharge


(ESD) began as a result of a failure investigation2. A hybrid electronic module for the Hubble Space Telescope gyro assembly failed during ground-level testing. The failure was isolated to a single 1500-ohm resistor within a thin-film resistor network chip,shown in Figure 1, that had developed an open circuit. This particular resistor had been connected between an isolated pin on the hybrid package and ground, and it was used as a precision reference resistor. Visual examination showed damage in the form of apparent cracks in the resistive film, in this case nichrome. These “cracks” (shown in Figure 2)were perpendicular to the major axis of the resistor and were crowded together in areas where the trace width was a minimum.


At first it was suspected that this damage resulted from some kind of over-power condition experienced during testing. Attempts to simulate this damage on spare resistor chips were unsuccessful, using both constant-power and pulse-power levels relevant to


the application. Even excessively high power levels did not duplicate the observed effects. Test equipment designed to check for ESD sensitivity,however, produced the same kind of transverse,jagged, roughly parallel cracks as in the failed resistor. It was concluded that an ESD event had affected the Hubble hybrid. This was an unusual occurrence (the first of its kind that any of the analysts involved had experienced), so it was decided to investigate further and to determine the risk of further instances of this kind in other flight hardware.


Figure 1 Overall view of the Hubble resistor


network.


Figure 2 Close up vicinal view of the damage to the Hubble resistor.


Background and Literature Review


To facilitate better understanding of this phenomenon, a literature review was undertaken. Twentyfive articles were identified that might be of use in the investigation. Four of these articles were discounted because they dealt with different, but loosely related, subjects (for instance, a study of mechanical stresses induced during laser trimming).


An additional five articles, which could not be located in several technical libraries, may be valuable


to future studies3,4,5,6,7.


A basic three-part tutorial, available over the


internet8, provides a good introduction to the sources,effects, and control of electrostatic discharge.


Several articles were more directly applicable to the study of ESD effects on thin-film resistors. Among


these, Lai9 and Chase10 have most closely duplicated the testing described in this paper. In both cases the authors used multiple ESD pulse sets to test tantalum nitride resistors. Lai tested capacitors and conductors in addition to resistors and described a method for calculating the temperature rise due to the ESD event.


Chase used the Charged-Device Model (CDM), as well as the Human-Body Model (HBM), and confirmed the finding of the present study that a ground path is required for ESD-induced damage to occur.


A similar study by Ebel11 examined the damage induced in cermet thick-film resistors. Several


sources12,13,14 discuss the effects of ESD and electrical overstress (EOS) on programmable readonly memory (PROM) fuses, which are similar to,but smaller than, typical thin-film resistors. A series


of three papers15,16,17 by Wallash describes ESD damage on hard-disk read/record heads with a builtin air gap.


Several papers discuss the related physics and materials effects that occur during an ESD event on a


thin-film resistor. For instance, Hagedorn and Hall18 have quantified the current crowding that occurs at sharp corners in resistive traces. Ramirez-Angulo et


al19,20 have mathematically derived design rules for laser trim placement, size, and shape for highest


resistance stability. Two additional papers21,22 discuss electromigration and vaporization at grain boundaries, which may help to explain the development of apparent cracks due to the ESD event.


It was noted that many of these papers had been published in journals and proceedings typically unfamiliar to the failure-analysis community. For that reason, this study, much of which has been


previously reported1, is being presented here.


Further Characterization Study


Part Description


Parts used in this study were of two basic designs:pre-packaged resistor networks and single resistor chips that were custom packaged for electrical connectivity. These resistor networks were drawn from residual flight inventory to better represent actual parts used in NASA applications. All of the resistor networks contained nichrome patterns ranging from 625 to 25,000 ohms. Most of these patterns were complex serpentine traces, laser trimmed to the desired value. One of the networks was composed of eight rectangular blocks, each laser trimmed to form a simple serpentine pattern. The chip resistors were an assortment of simple blocks and serpentine patterns using either nichrome or tantalum nitride as the resistive material. Chip resistors ranged from 100 to 32,800 ohms.


Test Methods


ESD pulses were induced in the parts using an Oryx Technology System 700 commercial ESD tester.


This tester is capable of delivering pulses from less than 100 to greater than 15,000 volts consistent with the HBM. The HBM, as opposed to the CDM or machine model (MM), is intended to simulate a pulse delivered by an ungrounded person (100 pF)discharging through skin (1500 ohms) into a grounded device. Many of the pulses were witnessed visually by placing the ESD tester under a stereomicroscope to facilitate observing the arcing location on a delidded device. A similar technique was used with an open shutter to photograph arcs in progress.


Visual inspection of the effects of ESD pulses was accomplished using a technique called vicinal illumination (described in more detail at this same


conference). Standard lighting techniques typically fail to reveal ESD damage, or the damage is so subtle that it is difficult to study. Vicinal illumination is accomplished using a standard upright metallurgical microscope by closing the field diaphragm completely and maximizing the light output to produce a small bright spot near the center of the field of view. When that light is directed onto the substrate, it refracts into the substrate material and under the normally opaque resistive trace. If the resistive trace contains ESD damage, the light is reflected through the “cracks” typical of ESD damage.


y = 0.0909x - 0.1111 y = 0.6085x - 0.1084


0 1 2 3 4 5 6 7 8


NUMBER OF ESD PULSES Total % at 1kV


Total % at Max volts


Linear (Total % at 1kV)


Linear (Total % at Max volts)


Figure 5 Pattern ND showed a linear reaction to repeated pulses at fixed voltages of 1kV and at


15.5kV


-1.4-1.2-1.0-0.8-0.6-0.4-0.2


NUMBER OF ESD PULSES AT 1500V


Figure 6 Significant resistance decrease exhibited by tantalum nitride pattern TF.


Figure 4 One pattern with polymer coating over the resistive elements showed this dramatic reaction to critical voltages.


ESD TEST VOLTAGE


5000 2500 1250


Figure 3 Typical reaction to ESD for nichrome


resistors such as these 1250 ohm resistors


4,000


6,000


NH5 NH6 NH9 NH10


Scanning-electron microscope (SEM) inspection was used, but it was found to be totally ineffective for examining ESD damage in nichrome resistors.


Tantalum nitride resistors, on the other hand, were examined quite successfully.


Test Types


The basic test procedure was to measure the resistance of a trace, induce an ESD pulse, remeasure, and repeat with successively higher voltage pulses. The voltage starting point and increment were determined by first testing a sample resistor. It was understood that incremental ESD pulses impose a certain degree of error due to cumulative damage, but this was unavoidable because of the small quantity of parts available. Because of the sometimes subtle variations in the pattern shape or width, it was impossible to accurately estimate the effect of cumulative damage on the resistance measurements. When possible,however, an additional sample of a resistive path was given a single pulse at a voltage well above the damage threshold, and the resistance was measured.


Usually these measurements fell either within the distribution for the sequential measurements or only slightly lower, so it is believed that the cumulativedamage effect was not major.


Another test was used to induce repeated pulses at the same voltage, with resistance measured after each pulse. To determine the effect of latent damage (a non-lethal ESD pulse that might get worse with use),several networks were exposed to various ESD voltages and then burned-in. The burn-in was 1000


hours at 105°C with cycled full rated power (50%duty cycle, 90-minute period). The resistance of each trace was measured at 0, 250, 500, and 1000 hours.


To facilitate better understanding of the ESD damage mechanism, glass slides were cut so that they just covered the resistive traces. Pulses were then imposed on the resistors with the slides in place in an effort to capture any material that might be vaporized by the ESD event and condensed on the cooler slide.


The slides were then examined using an SEM with energy-dispersive spectroscopy (EDS) to determine the presence of evaporated nichrome.


There was a general trend among all samples that the damage threshold was proportional to the resistance of the trace being tested. As a rough rule of thumb,the damage threshold was approximately 1 volt/ohm.


Multiple identical samples exhibited similar behavior, but the response was not perfectly predictable as shown in Figure 3. Initial intent was to measure physical dimensions of the resistor elements and attempt to relate these dimensions to ESD sensitivity. In fact, it was soon found that the simple effects of dimensional variation were overshadowed


by the effects of configuration features in the resistor trace patterns, particularly serpentines and laser trims.


A polymer coating (assumed to be polyimide) on two of the test samples produced some interesting results.


At low ESD voltage, the polymer apparently acted as an insulation blanket, preventing heat flow out of the resistor trace, especially in corners. As a result, these samples exhibited much heavier localized damage,wider cracks in the nichrome traces, and very predictable response as shown in Figure 4. At higher voltages, the coating apparently produced a carbon surface track during arcing events. Development of this stable arcing path protected the resistor from further degradation during repeated high-voltage ESD events.


A few resistors were exposed to repeated ESD pulses at the same voltage, with resistance measurements between pulses. Plots of these data (see Figure 5)show that the resistance increase was basically linear,with a slope proportional to the imposed ESD voltage. Extended pulses eventually resulted in catastrophic failure. Visual inspection between each pulse showed that the corner cracks grew steadily until the resistance of a serpentine trace had increased sufficiently to encourage internal arcing across the serpentine gap. Subsequent pulses produced continued arcing, eventually resulting in an open circuit and, usually, transverse cracks similar to the Hubble failure.


The tantalum nitride resistors tested to date have been simple block designs with “L-cut” laser trims.


During the incremental voltage tests, voltage was ramped from 100 to 15,500 volts in steps ranging from 100 to 1000 volts. In all cases, the resistance decreased after each pulse until approximately 3500 volts, at which point it increased rapidly. The maximum resistance changes measured were approximately 3.8 percent negative and 25 percent positive. Figure 6 shows the typical ESD-induced resistance decrease for a tantalum nitride resistor.


One group of resistors was tested at opposite polarity,with close correlation of the parts within each test condition. Those tested with the high potential connected nearest the laser trim experienced larger resistance shifts (both positive and negative) than the resistors tested with the low potential near the laser trim. It is unclear what importance this may have,and further investigation is planned. Additional testing on tantalum nitride resistors in general is planned for the next phase of this study.


Discussion of Observations1


Slope of the resistance versus imposed ESD voltage curve indicated four basic effects: little or no damage,current crowding, internal arcing, and external arcing.


It should be noted that most of the resistive traces


exhibited some, but rarely all, of these effects. For example, one sample exhibited only the “no effect”and “external arcing” effects due to the close spacing of the substrate bond pads. In another example,several traces in a network experienced no damage until 3000 volts, then exhibited external arcing at all voltages over 4000 volts (after the initial damage,however, the damage threshold decreased significantly).


“Little or No Effect” Region


Some resistors were visually inspected after each ESD pulse to establish a damage threshold below which no damage (typically corner cracking) was visible at 200X using vicinal illumination. The


typical resistance-change (∆R) threshold range for visible damage was 0.2 to 1.3 percent. Above this general range, the effects of current crowding were usually observed. The smallest values measured for


∆R were 0.01 percent.


“Current Crowding” Region


The damage associated with the lowest voltage (and therefore lowest energy) pulses above the damage threshold involved the appearance of “cracks” in the resistive trace at corners and the tips of laser trims.


These features resembled the branches of trees in that they split into numerous smaller paths as they developed at higher voltages. It is believed that these features were not actually cracks in the truest sense of the term because they were most likely thermally generated and not strictly mechanical in nature, but the term “crack” best describes their appearance.


Vicinal-illumination inspection confirmed that the opaque resistive material was missing within these crack features. Their appearance and location suggest that the cracks result from higher current density around corners in the resistive trace (current


crowding). Hagedorn and Hall18 have shown that the maximum current density in a right-angle turn with a radius of 1% of the trace width (a relatively sharp bend) is more than six times the current density in the straight portion of the resistive trace. Figures 7 and 8 show examples of corner-crowding-induced cracks.


In some cases, cracks were observed across the entire width of the resistive trace, but often crack growth was suspended by the transition to internal or external arcing, which shunted the current,preventing it from flowing through the portions of the resistor that exhibited corner cracking. This transition was heavily influenced by the increase in resistance associated with the corner-cracking mechanism.


“Internal Arcing” Region


As the voltage (and therefore energy) of each ESD pulse was increased, eventually arcing would occur within the resistive pattern. Locations of such arcs varied from the base of the laser trim to gaps created by the serpentine pattern to high-potential-difference gaps created when the pattern doubled back on itself.


The arcs tended to occur in as straight a line as possible between the substrate bond pads. In addition to the resistance change evidence, vicinalillumination inspection revealed a distinctive appearance for the damage resulting from internal arcing. The low-potential side of an arc always exhibited a branched crack structure extending into the trace from an edge, and the high-potential side exhibited only a few small chunks of nichrome missing from the edge of the trace. Examples of the damage caused by internal arcing are shown in Figures 9 and 10. During somewhat higher-voltage ESD pulses, arcs were observed directly using a stereomicroscope. Several of these arcs were photographed (see Figure 11), recording locations of the arcs. Internal arcing was often accompanied by the transverse cracks first observed in the Hubble failure (see Figure 12). It is believed that these cracks were the result of increased current density along thin areas of the nichrome, exacerbated by the low effective resistance experienced by the arc,producing higher current flow. At higher ESD voltages, external arcing tended to predominate.


“External Arcing” Region


Many, but not all, resistor networks exhibited some degree of arcing outside the resistive trace. Potential locations of these arcs were between package bond pads, from package bond pads to substrate bond pads,between substrate bond pads, between adjacent resistors, and even between the bond pads and adjacent bond wires. External arcing usually shunted all of the current flow around the resistive element,but in some cases resistance continued to change despite external arcing, indicating that some amount of current flow was causing damage to the remaining resistive material. External arcing was typically easy to observe using the stereomicroscope described above, and it was observed that the location often shifted slightly from one ESD pulse to the next.


Visual inspection at higher magnification revealed that external arcing typically resulted in metal deposition near the low-potential side of the arc and a melted appearance on the surface of the highpotential side of the arc.


Figure 7 Vicinal illumination view of corner


crowding induced damage.


Figure 8 Typical corner crowding damage in a


polymer coated resistor.


Figure 9 Vicinal illumination view of internal arcing damage.


Figure 10 SEM view of ESD damage in a tantalum nitride resistor. Note the internal arcing damage to the left of the laser kerf.


Figure 11 A photograph taken during an ESD


induced arc event. Note the location of the arc on the center resistor.


Figure 12 Vicinal illumination view of


transverse cracking typical of relatively


high voltage ESD damage.


Presence of a direct ground connection at one end of the resistor was required in all cases to produce ESD damage. Several resistors were tested without a ground connection to the subject resistor or an adjacent trace, and in no such case was any damage observed, either electrically or visually. This finding,


confirmed by Chase10, is significant because it helps to explain why ESD failures are not more common in thin-film resistors. Consider, for example, the case of a discrete packaged resistor network; damage to any individual resistor in it would be extremely unlikely given that an ESD pulse would have to be delivered while the pin connected to the other end of the resistor (typically an adjacent lead) was connected to ground potential. This requirement for a ground suggests that thin-film resistors are much more susceptible to ESD damage after being installed into larger assemblies that have their own ground connection. This was the precise situation for the Hubble failure, which was found during board-level testing.


Future Work1


As is so often the case, this investigation seems to have raised more questions than it answered. The surprising result that tantalum nitride resistors can show negative resistance changes in reaction to ESD should be investigated. Is this behavior dependent on the manufacturer’s processing? Does it happen with serpentine as well as block patterns? Plans are in place to procure both block and serpentine pattern tantalum nitride resistors from a different manufacturer in addition to performing further testing on the present samples.


During brief experiments with changes in polarity on tantalum nitride samples, some interesting effects that should be further investigated were observed.


Similar testing should also be performed with nichrome resistors to determine whether the previously noted difference between the two systems extends to polarity sensitivity as well.


From the work described in this paper, it has been postulated that rounding the insides of serpentine bends will reduce current density and thus increase robustness, but this hypothesis was not tested.


Samples with radiused bends will be tested in the next phase of work.


1. Thin-film resistors made from both tantalum nitride and nichrome are ESD sensitive.


2. Locations and shapes of damaged areas can be used as failure-analysis guides for estimating the magnitude and polarity of an ESD insult.


3. Sensitivity levels of the resistor patterns tested in this investigation were influenced by many unexpected factors in addition to, or instead of,simply the width, length, thickness, and resistivity of the resistance trace.


4. Too close spacing of the pads of separate resistors can lead to unexpected damage, caused by the ESD pulse jumping to the adjacent resistor.


5. ESD damage to nichrome resistors can be expected to increase resistance, whereas tantalum nitride resistors may decrease in resistance when subjected to relatively low-voltage pulses.


6. Characteristics of the damage are fairly predictable depending on the form of the resistor trace; serpentine patterns tend to show damage on the inside radii of the bends, laser scribes show arc damage, etc.


7. Dimensions and locations of laser trims can significantly impact ESD sensitivity of thin-film resistors.


8. Some of the ESD damage characteristics are sensitive to the polarity of the applied charge.


9. In practice, ESD damage to thin-film resistors is probably quite rare due to the requirement for a charged surface at one end and a grounded surface at the opposite end of a resistor trace.


10. ESD damage to thin-film nichrome resistors appears to be stable as the part is operated.


The authors wish to thank the following people who supported this work: Andre Pelham and Prashant Patel, the high-school students who performed most of the ESD testing; Doug Macpherson of Electrofilms, Inc. and Fred Castello of Teledyne Electronic Technology, who provided some of the test samples and considerable knowledge and experience, and the management of the National Aeronautics and Space Administration for vital resources and the opportunity to perform the experiment.


1) M.J. Sampson, S. M. Hull, ”Electrostatic Discharge Effects on Thin Film Resistors”,CARTS ’99, pp. 208-217 (1999)


2) J. Slonaker, GSFC Failure Analysis Report Number EV88268 (1998)


3) V.D. Sadkov, D.E. Orlov, “Resistance of a Film Resistor with a Slit of Finite Width”,Radioelectronics and Communications Systems,Vol. 35, Issue 11, pp. 62-64 (1992)


4) R.R. Avanesyan, Yu.P. Lazarev, A.N. Lugin,“Investigation of the Influence of Boundary Effects on the Stability and TCR of Thin-film Resistors”, Measurement Techniques, Vol. 39,Issue 5, pp. 487-490 (1996)


5) J.F. Cain, L. Hart, J.R. McLean, “Failures in Thin Metal Film Resistors – A Case History”,Quality


Reliability


Engineering International, Vol. 8, Issue 2, pp. 99-104 (1992)


6) R. Veyhl, “Temperature Dependence of Thinfilm Resistors”, CARTS-Europe ’91, pp. 110-114 (1991)


7) K.D. Robb, et al, “Analysis of Microstrip Resistors Using the Transmission Line Matrix(TLM) Method”, International Journal for Hybrid Microelectronics, Vol. 14, Issue 2, pp.


62-69 (1991)


8) “Basics of Electrostatic Discharge”, The ESD Association,


http://www.borg.com/~eosesd/cebasics.html


(1996)


9) T.T. Lai, “Electrostatic Discharge (ESD)Sensitivity of Thin-film Hybrid Passive


Components”, Proceedings 39th Electronic Components Conference, IEEE, pp. 229-239(1989)


10) E.W. Chase, “Electrostatic Discharge (ESD)Damage Susceptibility of Thin Film Resistors and Capacitors”, EOS/ESD Proceedings, pp.13-18 (1982)


11) G.H. Ebel, “ESD Induced Failures in Cermet Trim Potentiometers”, ISTFA 1998, pp. 139-142(1998)


12) D.M. Petkovic, “An Irreversible Resistance Transition in Polycrystalline Silicon Thin Film Resistors”, Vacuum, Vol. 40, No.1/2, pp. 213-216 (1990)


13) J. Smith and W. Littau, “Prediction of Thin-film Resistor Burnout”, EOS/ESD Proceedings, pp.


192-197 (1981)


14) R. A. Launer, J. T. May, L. M. Richard, “Interpretation of EOS Damage in NiCr Resistors”,ISTFA 1990, pp. 279-284 (1990)


15) A. J. Wallash, “Electrostatic Modeling and ESD Damage of Magnetoresistive Sensors”, IEEE Transactions on Magnetics, Vol. 32, Issue 1, pp.


49-53 (1996)


16) A.J. Wallash, T. S. Hughbanks, and S. H.


Voldman, “ESD Failure Mechanisms of Inductive and Magnetoresistive Recording Heads”, EOS/ ESD Proceedings, pp. 322-330(1995)


17) A.J. Wallash, M. Honda, “Field-induced Breakdown ESD Damage of Magnetoresistive Recording Heads”, EOS/ESD Symposium ’97,pp. 382-385 (1997)


18) F.B. Hagedorn and P.M. Hall, “Right Angle Bends in Thin Film Strip Conductors”, Journal of Applied Physics, Vol. 34, No. 1, pp. 128-133(1963)


19) J. Ramirez-Angulo, R. Wang, and R. Geiger,“Improvement of Laser Trimmed Film Resistor Stability by Selection of Optimal Trim Paths”,IEEE International Symposium on Circuits and Systems, pp. 2188-2191 (1991)


20) J. Ramirez-Angulo, R.L. Geiger, “New LaserTrimmed Film Resistor Structures for Very High Stability Requirements”, IEEE Transactions on Electron Devices, Vol. 35, No. 4, pp. 516-518(1988)


21) A.J. Patrinos, J.A. Schwarz, “Simulation of Electromigration Based on Resistor Networks”,Journal of Applied Physics, Vol. 75, Issue 11,pp. 7292-7298 (1994)


22) J.H. Linn, et al, “A Reliability Study of Laser Trimmed NiCr Kerfs”, 41st Electronic Components and Technology Conference, IEEE,pp. 883-889 (1991)


Electronic Device Failure Analysis Society, editor, p 305-308


DOI: 10.1361/cp1999istfa305


# Characterization of Gold Embrittlement in Solder Joints


Characterization of Gold Embrittlement in Solder Joints


Carl B. Bunis


AMP M/A-COM, Lowell, Massachusetts


Mechanical strength, integrity, and reliability of solder connections used in the microelectronics industry are important factors in overall quality and reliability of the finished product. In most cases tin(Sn) rich solders are attached to a base metal plated with nickel (Ni) and then with gold (Au). Formation of AuSn4 intermetallics in the solder may result in loss of more than 80% of the initial impact toughness, resulting in loss of reliability of the connection.


Gold (Au) embrittlement is a major concern in tin/lead (Sn/Pb) soldering or any other joining process with Au and Sn as major constituents. Noncompliance to Au plating-thickness specifications by vendors or insufficient Sn wicking of Au surfaces can result in embrittled joints and unreliable parts.


In soldering of microwave microelectronic devices,many of the bond pads are plated with Au because it is a very noble metal that does not corrode or oxidize.


Standard plating under the Au is Ni, which is used as a diffusion barrier and an adhesive layer between Au and copper (Cu). The Au is plated onto the Ni because in the atmosphere the Ni will oxidize, and soldering becomes very difficult and non-wetting will occur.


Diffusivity, time, temperature, and concentration gradient are the major driving forces in formation of intermetallics in solder joints as well as other twometal systems. Temperature, time, and concentration gradient are also the variables that drive diffusion, as shown in the following equations:


RT Q


0e


D is the diffusivity, Do is a constant, Q is the activation energy, R is the gas constant, T is the temperature in K.


Dt


erf


t= time, Cs = surface concentration Cx = concentration at distance x, Co = initial concentration.


dx


dc


J −=


J is the flux, D is the diffusivity, dc dx


is the


concentration gradient .


In the Au/Sn system, formation of intermetallics greatly increases with temperature and time. A mechanically sound joint may degrade over a product’s shelf life depending upon the storage environment. The following is an example of time affecting diffusion in the Au/Sn system.


Example 1


A customer’s specification calls for a plating scheme comprising Ni/Au/Sn over molybdenum (Mo) base metal. The supplier produces the parts and inspects the final thicknesses using X-Ray Fluorescence(XRF). After two months of shelf time, the parts are inspected by the customer before installation, and the plating is out of specification.


Cross-sectional analysis using Energy Dispersive XRay Spectroscopy (EDS) of the plated parts shows diffusion of the Au into the Sn. Here, the initial interface between the Au and Sn has physically moved, so the layer thicknesses have changed, and XRF measurements show that thicknesses are out of specification.


The phenomenon of the interface moving during diffusion is called the Kirkendall Effect, which occurs when metal A and metal B are placed together and metal A diffuses into metal B faster than metal B diffuses into metal A (shown in Figure 1). After time, the interface between the two metals moves toward metal A. If the diffusion of metal A into metal B is faster than atoms of metal A can fill its own vacancies, a void will occur within metal A or at the interface. This is called Kirkendall Voiding.


JA,JB = flux of atoms


JV = flux of vacancies


Figure 1 Illustration showing the Kirkendall Effect.


Figure 2 and Figure 3 are results from an experiment with the same plating scheme as that used on the previously mentioned failed units. Figure 2 is an EDS X-Ray Map of a cross section in the as-received condition. X-Ray maps show qualitative distribution of elements over an area. A particular element can only be compared to itself, where a higher pixel intensity shows an element as rich and a lower pixel


intensity shows it as lean. That is, two elements cannot be compared in the same map. Figure 2 shows clear delineations among the Mo, Ni, Au, and Sn. Figure 3 illustrates a cross section after


5 minutes at 150°C, showing the effect of temperature, where the Au has diffused into the Sn.


Figure 2 EDS X-Ray Map of cross-sectioned


Ni/Au/Sn plating scheme on Mo base metal in asreceived condition (Left to right in top row: SEM image, dot map for Mo, dot map for Sn; left to right


in bottom row: dot map for Ni, dot map for Au).


Figure 3 EDS X-Ray Map of cross-sectioned


Ni/Au/Sn plating scheme on Mo base metal after a


5-minute bake at 150°C (Left to right in top row:SEM image, dot map for Mo, dot map for Sn; left to right in bottom row: dot map for Ni, dot map for Au)


Many of the solders used today are Sn rich with some added Pb. Basic Sn rich solders are 63/37 (eutectic),60/40, and 90/10 Sn/Pb. The eutectic has a lamellar microstructure that is formed when the liquid freezes into two solids. Eutectic, which means “low melting,” designates the lowest-melting-point alloy.


All of the above mentioned solders have some percentage of eutectic with the 63/37 alloy having 100%. Figure 4 is a Scanning Electron Micrograph(SEM) of a eutectic structure. Notice that it is not a solid solution and that the phases can be delineated clearly.


Au and Sn form multiple intermetallics as apparent in Figure 5 which is a vertical section of the phase diagram for the Au/Pb/Sn ternary system between 63Sn/37Pb and Au. The fact that intermetallics are formed does not mean a material is bad or that there is a latent defect. Physical characteristics of the


BV


AV


intermetallics determine how the material properties change. In the case of the Au/Sn system, AuSn4 is a brittle phase that degrades the material properties. As evident in Figure 5, AuSn4 can be formed with an Au weight percentage of approximately 4% to 43%. All of the Au dissolved from 4% to 13% becomes AuSn4. At soldering temperatures ranging from


220°C to 250°C, the dissolution rate of Au into eutectic solder is from 0.13µm/s to 0.26µm/s.


Figure 4 SEM micrographs of eutectic structures;note the clear delineation between phases. The image on the right is Sn/Pb eutectic.


Figure 5 Vertical section of Au/Pb/Sn phase diagram at 63% Sn and 37% Pb [Ref. 1].


Figure 6 is a graph of relative impact toughness versus the percentage of Au in Sn. Impact toughness is related to ductility, yield strength and Ultimate Tensile Strength (UTS). The graph shows the mechanical properties dropping by over 80% when the Au content in Sn reaches approximately 5%. If extrapolated, the impact toughness should reach a


low point at 13% Au, where the most AuSn4 is present, should start increasing over 13% Au, and should reach a maximum again at approximately 45%Au. Although more expensive, many times an Au/Sn eutectic solder (80/20) is used to prevent formation of AuSn4.


Figure 6 Relative impact toughness versus weight percent Au in Sn. [Ref. 2]


Example 2


Typical fractures caused by Au embrittlement have a very brittle appearance, and such fractures are catastrophic (Figure 7). The fracture line follows the intermetallic formation zone. Figure 8 shows the


AuSn4 forming a needle-like structure that can be imaged in Sn rich solder using BackscatteredElectron Imaging (BEI) in the SEM. Contrast in BEI is related to elemental composition, where high average atomic number (Z) materials appear brighter than low average Z materials. In the case AuSn4, the average Z is lower than the atomic numbers of pure Au and Pb and higher than the atomic number of pure Sn. Therefore, AuSn4 appears darker than Au and Pb, but brighter than Sn.


Figure 9 shows an EDS X-Ray map of a cracked solder joint inside a female-to-male connector. In this case, the hole and male connectors were plated with Au, and the solder was 63/37 Sn/Pb eutectic.


The crack is along the interface between AuSn4 and solder. The Au inside the female connector could not be removed by tin wicking because of the small diameter of the hole. Figure 10 shows the intermetallic needle-like structure throughout a solder joint. A layer of Au plating on the bottom soldered surface can still be observed after soldering,indicating inadequate dwell time or insufficient heat.


Figure 7 Crack caused by Au embrittlement inside a soldered female-to-male connector.


Figure 8 BEI SEM micrograph of the needle-like structure formed by the AuSn4 intermetallic.


Figure 9 EDS Map of Figure 7, a cross-sectioned soldered female to male connector (Left to right in top row: SEM image, dot map for Au, dot map for Pb; left to right in bottom row: dot map for Sn, dot map for Ni, dot map for Cu).


Figure 10 EDS Map of Figure 8, the needle-like


structure formed by AuSn4 (Left to right in top row:SEM image, dot map for Au, dot map for Pb; left to right in bottom row: dot map for Sn, dot map for Cu).


Conclusions and Corrective Actions


• Au in excess of 4% in Sn forms a brittle intermetallic AuSn4 that reduces solder-joint mechanical properties by up to 80%.


• Using a standard solder volume, a thickness of approximately 35-40 microinches of Au should prevent formation of AuSn4.


• Common practice with Au thicknesses of greater than 40 microinches is to tin and wick the pad surface before soldering; this procedure consists of melting Sn on the pad surface and using solder wick to remove the Sn and Au from the pad; soldering is performed immediately after wicking.


• Using a eutectic Au/Sn solder will remove the possibility of AuSn4 formation.


1) D. M. Jacobson and G. Humpston, “Gold Coatings for Fluxless Soldering,” Gold Bulletin,22, p. 9, 1989.


2) H.A.H Steen., G. Becker, “The Effect of Impurity Elements on the Soldering Properties of Eutectic and Near-eutectic Solder,” Brazing and Soldering, 1986.


Electronic Device Failure Analysis Society, editor, p 311-316


DOI: 10.1361/cp1999istfa311


# In-situ Dual Beam (FIBSEM) Techniques for Probe Pad Deposition and Dielectric Integrity Inspection in 0.2 µm Technology DRAM Single Cells.


In-situ Dual Beam (FIBSEM) Techniques for Probe Pad Deposition and Dielectric Integrity Inspection in 0.2 µm Technology DRAM


Single Cells.


Gunnar Zimmermann and Richard Chapman


White Oak Semiconductor, Sandston, Virginia


Dual beam FIBSEM systems invite the use of innovative techniques to localize IC fails both electrically and physically. For electrical localization,we present a quick and reliable in-situ FIBSEM technique to deposit probe pads with very low parasitic leakage (Ipara < 4E-11A at 3V). The probe pads were Pt, deposited with ion beam assistance, on top of highly insulating SiOx, deposited with electron beam assistance. The buried plate (n-Band), p-well, wordline and bitline of a failing and a good 0.2 µm technology DRAM single cell were contacted. Both cells shared the same wordline for direct comparison of cell characteristics. Through this technique we electrically isolated the fail to a single cell by detecting leakage between the polysilicon wordline gate and the cell diffusion. For physical localization,we present a completely in-situ FIBSEM technique that combines ion milling, XeF2 staining and SEM imaging. With this technique, the electrically isolated fail was found to be a hole in the gate oxide at the bad cell.


The capabilities of focused ion beam (FIB) systems


[1, 2] to highlight fails in ultra large scale integration(ULSI) semiconductor devices have been enhanced considerably by the recent introduction of dual beam(FIBSEM) systems. In the dual beam systems, the scanning electron microscope (SEM) and FIB can focus on the same spot through eucentric centering.


This allows precise monitoring of the ion beam


assisted milling, deposition[3] and etching[4] procedures with the SEM. Additionally, the SEM can be used to deposit either metal or oxide layers.


Fails in semiconductor devices can often be localized electrically by using sophisticated electrical test


patterns. For the sample under investigation in this article the fail had been electrically localized to a single memory cell of a 64M dynamic random access memory (DRAM) device before starting the FIBSEM analysis. To increase the probability of successfully highlighting the fail in physical failure analysis the leakage path inside the cell had to be investigated further. A well-known technique to access specific parts of electrical devices is to deposit probe pads by means of the ion beam in a FIB system after having removed the upper metal layers that connect the cells or devices. Unfortunately, ion beam assisted silicon


oxide (SiOx) deposition leads to a material with poor insulating properties due to the high amount of


gallium atoms incorporated into the layer [5]. Good insulation between the pads as well as between pad and underlying electrically active areas is necessary to limit the parasitic leakage due to probe pad deposition. In order to measure leakage currents in the range of nanoamperes and below the sample is therefore usually coated outside the FIB using a conventional quartz deposition tool. This leads to a good insulating layer all over the surface and minimizes the parasitic leakage. Quartz layer thickness and homogeneity control over the whole sample is crucial for this process, because a too thin layer increases the conductivity and capacitive coupling whereas a too thick layer can make subsequent imaging of the target area problematic, especially when using the ion beam.


In the first part of this article we present a technique to eliminate the ex-situ oxide deposition without sacrificing the need for a highly insulating material between pad and semiconductor surface by depositing the SiOx pads with electron beam assistance. Lipp et al [5] reported empirical results that show a two order of magnitude higher resistance of electron beam deposited SiOx layers over ion beam deposited layers. Tetraethyl-orthosilicate (TEOS) was used as


precursor for SiOx deposition. The higher resistance is explained by the absence of gallium incorporation into the growing layer during electron beam assisted deposition.


The results of the electrical probing indicated a leakage between the polysilicon gate and the cell junction, which is typically caused by a leaky gateoxide (GOX) of the cell transistor. Holes in thin oxides can be prepared and highlighted by using a two-step process in which a sample first is delayered top-down or cross-sectioned close to the target area and in a second step is stained using a selective silicon etch followed by SEM inspection. All known methods are ex-situ techniques that are not directly applicable in a FIB or SEM-chamber. They often need frequent and time-consuming sample transfers into a SEM chamber for precise monitoring of the progress of delayering and staining. For the staining a selective silicon etch (e.g. potassium-hydroxide,KOH) is used whereas for the sample delayering or cross-sectioning chemical and/or physical delayering methods (e.g. reactive ion etching, selective chemical etching, face lapping) are applied.


In the second part of this article a new technique to highlight holes in thin oxide layers in-situ in the FIBSEM chamber is presented, which allows us to combine all delayering and staining steps in the same chamber and to monitor the process with SEM resolution at any time.


In the “Experimental” section we describe the general layout of the DRAM sample, the initial sample preparation and the tool setup. The section “Results and Discussion” consists of three parts. The first part is dealing with the probe pad deposition technique as well as with the dependence of SiOx growth rate versus deposition parameters. In the second part we discuss the results of electrically probing the single cell. The physical fail localization of pin holes in the GOX is described in the third section. The“Summary” concludes this article.


The sample was a plastic-packaged 0.2 µm technology 64M DRAM manufactured at WhiteOak Semiconductor, which showed a failing single cell after a stress test. The electrical fail address was provided. The single cell consisted of a deep trench capacitor accessed through an n-channel transfer gate, as shown in the schematic drawing in figure 1.


The gate was the wordline (WL) and the data was written or read to the bitline (BL). The cell resided in a p-well (PW). A deep n-doped region (n-band,buried plate, BP) served as electrode for the trench capacitors and isolated the PW from the substrate.


Polysilicon was used to form the BL contact between the tungsten BL bus and the source/drain. The


wordline (WL) consisted of a stack of gate oxide(GOX), polysilicon, tungsten-silicide and siliconnitride. The WL is stitched in regular distances to a ALCu-metal line to reduce the line resistance. Silicon oxide layers served as dielectric isolation between WL and BL as well as between upper AlCumetallization levels. The technology as well as layout and basic functions of a DRAM single cell can be


reviewed in detail elsewhere [6,7].


P-well


N+GOX


N+


Si-Oxide


Si-Nitride W-silicide Poly-Si


Suspected position of GOX hole


bitline (BL)


N-band


Figure 1 schematic representation of the DRAM cell in cross-section. Areas containing SiOx are marked in grey.


The plastic package was totally removed from the die


using hot sulfuric acid at 150°C. All layers above the BL contact were removed using standard delayering techniques involving RIE and wet chemical steps. A FEI XL 830 dual beam system equipped with a gallium source ion column, a field emission scanning electron microscope, and four gas injectors was used for probe pad deposition. The ion beam was at 30 keV with currents between 4 and 350 pA. SEM imaging with a resolution down to 1.5 nm was performed using an immersion lens type ultra high resolution (UHR) field emission SEM at 5 keV and about 100 pA. Secondary electron imaging was used when scanning with the electron as well as with the ion beam. Pt-cyclopentadienyl and tetraethylorthosilane (TEOS) were used for platinum and oxide depositions, respectively. Standard ion beam conditions with beam currents of 4 - 350 pA were applied for Pt deposition and ion milling. SiOx deposition was performed using the electron beam at 3 - 12 keV and beam currents of 0.1 to 15 nA in the UHR mode. Iodine (I2) was used with the ion beam to selectively etch metals, and xenon-difluoride(XeF2) was used without any beam assistance to selectively etch silicon. The TEOS gas injector was aligned to the electron beam, whereas all other injectors were aligned to the ion beam. The distance between needles and sample surface was kept


constant at about 100 µm. Chemical sources were operated at temperatures between 25 and 40°C as recommended by the vendor.


The memory cells were electrically tested using four micromanipulators with T4-10 needles on a Suss PA200 probe station. The electrical signals were captured using a HP 4155B parameter analyzer. All needles were checked for continuity to the probe pads. Residual currents of below 10 – 40 pA were indicating a very high oxide layer quality of the probe pads (see figures 4 and 5). Once the fail was electrically isolated, cross-sectioning of the sample was performed with a Buehler Ecomet polishing table


using diamond lapping foil ranging from 5 µm down to 1 µm. The progress of polishing was monitored using an optical microscope (Leica Polyvar SC). This step was necessary to remove bulk material from one side of the target to be able to perform top-down ion milling after reintroducing the sample into the FIB.


Probe pad deposition


Electron beam conditions were optimized for the maximum deposition rate allowable for adequate image integrity. Image integrity was important for deposition monitoring. The rate of deposition was modulated through beam energy and current adjustments. It is also dependent on the needle alignment with respect to sample surface and electron beam. The SiOx layer thickness was determined from SEM images of in-situ FIB cross-sections. Figure 2 is showing the deposition rate with respect to electron energy for 3 different ranges of beam currents.


According to previous results[5], the deposition rate was found to increase with lower beam energy and higher beam currents. The highest deposition rate of


about 0.5 µm3/min was observed for a 3 keV, 15 nA beam. However, the SEM image resolution was insufficient under these conditions. For the technique of probe pad deposition a 5 keV, 1 nA beam was used because of satisfactory SEM resolution and a sufficiently high deposition rate of about 0.25


µm3/min. It was found that these conditions produced a dielectric film with about a 1 MΩcm resistivity [8],which compared favorably with Lipp’s results [5].


The dielectric for the probe pads took approximately 10 minutes to deposit. The deposited oxide was 100


nm thick and about 5 x 5 µm2. During insulator deposition the layer thickness can be roughly estimated in-situ by taking into account the decreasing SEM resolution through the growing film due to the limited penetration depth of the electron beam and comparing this to deposited films of known thickness. The dielectric was deposited on top of the BL contacts, which remained on the sample after the removal of the bitline. The target contact was identified using the fail address information of the electrical test pattern. Similar pads were deposited on BP and PW contacts outside the memory cell array.


The pad for the WL was deposited on top of the stitch contact.


Figure 2 deposition rate of SiOx using TEOS as


precursor versus electron beam energy for different ranges of beam current.


After forming the probe pad insulator, a 0.3 x 0.3µm2 contact hole was milled into the insulator using a 4 –11 pA ion beam. To position the ion beam, SEM imaging was used to determine the exact location of the target by counting the CB contacts through the SiOx pad. The live ion beam image was used for the end point detection of milling. Before Pt probe pad deposition the contact hole was filled with Pt in a separate step to ensure a low resistive connection to the target contact.


Finally, a 3.5 x 3.5 µm2, 160 nm thick Pt probe pad was deposited using an ion beam of 15 pA. The Pt pad was smaller than the SiOx pad to ensure a good electrical insulation at the pad edges. Iodine gas assisted ion milling was used to remove excessive Pt


electron energy (keV)


0.1-0.3 nA


0.8-1.4 nA 8-15 nA


from the area around the pad. The use of the ion beam was minimized during the whole process to reduce parasitic leakage due to gallium implantation.


The total processing time for one probe pad was approximately 20 minutes. A typical pad is shown in figure 3.


Figure 3 Tilted SEM image of the completed probe pad exhibiting the Pt pad and the underlying isolating SiOx pad. Horizontal lines represent the imprints of the removed bitlines in the sample dielectric.


Electrical fail localization


Pads were deposited to probe the BP, PW, WL-stitch and the BL. Because the sample was delayered to the substrate- and polysilicon-contact levels, contacts were directly accessible with adequate separation of


at least 10µm to allow for individual probe pad deposition. For comparison, the BL contact of a good cell sharing the same WL was also connected. A constant voltage of –1V was maintained for the PW with the BP at +1V while ramping the BL voltage between –2 and 2 V and the WL voltage between –3 and 3V.


Figure 4 shows the WL current for different WL voltages with respect to the BL voltage for the failing cell. The BL contact of the good cell was at 0V. The WL current increases for positive WL voltages and negative BL voltages. It is disappearing for slightly negative WL voltages independent of the BL voltage.


For a WL voltage of –3V the WL current is negative independent of the BL voltage.


The leakage mechanism is primarily controlled by the WL voltage, which defines if the transfer gate is opened or closed. Once the WL voltage is charged positively enough to form the n-channel below the GOX, the leakage mainly depends on the potential difference between BL and WL. Therefore the WL current decreases when increasing the BL voltage up to 2V. The leakage mechanism disappears for negative WL voltages when the gate is closed. It can not be explained by a direct short between the WL and the CB contact, which should only depend on the potential difference between WL and BL and not also on the transistor characteristics.


Figure 4 Wordline (WL) current for different WL voltages with respect to the bitline (BL) voltage for


the failing cell. A WL to BL leakage is detected


which is dependent on the WL voltage.


The results are suggesting a leakage from the WL through the GOX into the PW to which the BL-contact can be connected by switching on the n-channel below the gate. For negative WL voltages the WL-PW diode is forward biased and should show an increasing leakage independent of the BL voltage. The curve for the WL voltage at –3V is indicating the onset of this mechanism. Recall that the p-well is at –1V and the WL-PW diode does not turn on until a WL voltage around –1.7V. Typical causes of failure of the GOX are pin holes or contamination. The fail location must be far enough away from the n-diffusion area of the BL-contact, so that the gate can still control the leakage and is not by-passed. A possible location of the GOX hole is shown in figure 1.


Figure 5 shows the same measurements for the good cell. The BL of the bad cell was held to 0V. No dependence of the WL current on the BL voltage at the good cell is observed. Because both cells share the same WL, the WL current is heavily influenced by the leakage in the bad cell. When changing the WL voltage the WL current is actually tracking the values observed in figure 4 for a BL voltage of 0V at the bad cell (e.g. 0.28pA / +3V and –0.07pA / –3V).


TEOS-Pad


Pt-Pad


SiOx -Pad


-2 -1.6 -1.2 -0.8 -0.4 0 0.4 0.8 1.2 1.6 2


BL voltage of failing cell (volts)


WL= -3V


WL= -1.5V


WL= 0V


WL= 1.5V


WL= 3V


Figure 5 Wordline (WL) current for different WL voltages with respect to the bitline voltage for the good cell. The WL current is not influenced by the BL voltage.


Physical fail localization


Traditionally, physical analysis of holes in the gate oxides involves two steps. First, the sample is delayered top-down into the polysilicon layer of the WL. Second, it is stained using a selective silicon etch (e.g. KOH) followed by SEM inspection. All known methods are ex-situ techniques.


We developed a new in-situ FIBSEM technique to highlight holes in thin oxides (see figure 6). We used ion beam milling for precise material removal in the target area, stopping in the polysilicon layer of the gate stack. Using XeF2, we were able to clear the area above the gate oxide of remaining silicon.


Further-more we etched through the GOX hole into the underlying silicon substrate thus highlighting the hole in the SEM image.


polished surface


stage


GOX-hole


Si etched by XeF2


Si-substrate


Si-oxide


Figure 6 Schematic drawing showing the orientation of the sample with respect to electron and ion beam before applying the technique to highlight holes in thin oxide layers.


First, it was necessary to perform a quick ex-situ polishing step using standard diamond lapping methods to cross-section the sample within about 5


µm of the failing cell. The sample was then mounted in the FIBSEM with the polished surface facing the ion column and the target area milled parallel to the sample surface by a 150 pA ion beam in a fine polishing mode. The SEM was used to monitor the material removal through the different layers of the gate stack. Polishing was stopped as soon as most of the polysilicon of the gate stack was removed and the transfer gate was exposed leaving only a few 10 – 50 nm of silicon above the GOX. Now XeF2 was applied to the surface without any beam assistance and the progress of etching was monitored with the SEM in steps of five seconds, while interrupting the gas flux. Holes in the oxide could then be highlighted by etching into the underlying silicon substrate.


Figure 7 shows the targeted failing cell (X) after topdown polishing and a XeF2 stain of 5 seconds. The top down SEM image is clearly showing the BL contacts (BL) and the corresponding transfer gates(TG) of the cells on either side of the contacts. The imprints of the wordlines in the oxide are still visible as vertical lines in the image. Polysilicon only remains in the areas of the transfer gates and the BL contacts. Their rough surfaces are indications of selective attack by the XeF2 gas. The surrounding oxides are not etched.


Figure 7 SEM-scanned target area viewed from the top. Shown is the failing cell (X) after topdown FIB polishing and 5 minutes XeF2 stain, the BL contact


(BL), the transfer gates (TG) with remaining polysilicon and imprints of the wordline (WL) in the oxide.


After approximately 2 minutes of total exposure time two small pin holes at the upper edge of the transfer gate area of the failing cell became visible (figure 8,arrow). The holes were located a little bit away from the BL contact. This location agreed with the elecX


TG


WL BL


-0.1


BL voltage of good cell (volts)


trical results in that leakage could only be seen as the gate was turned on. Notice that the gate-oxide was not attacked by the XeF2 and shows a very smooth and clean surface. The polysilicon of the BL contact was completely etched away. The dark area around the BL contacts was caused by the removal of silicon from the substrate material under the contact.


Figure 8 SEM-scanned target area viewed from the top. Shown is the failing cell (X) after approximately 2 minutes of etching time using XeF2 stain. Two pin holes in the transfer gate area are visible causing the cell to fail (arrow).


Summary and Conclusion


Two quick and reliable new in-situ FIBSEM methods that can be applied for electrical isolation and physical highlighting of fails in ULSI semiconductor devices are presented. For electrical localization,electron beam assisted SiOx deposition with TEOS as precursor is used to deposit probe pads with very low parasitic leakage. Optimum conditions for SiOx deposition are a beam energy of 5 keV and a beam current of about 1nA, yielding in a SiOx depositon


rate of 0.25 µm3/min. The total time to process one probe pad of (5 x 5) µm2, consisting of 100 nm SiOx and 160 nm Pt is approximately 20 minutes. Using this technique the buried plate (n-Band), p-well,


wordline and bitline of a failing and a good 0.2 µm technology DRAM single cell have been contacted.


Based on the electrical results the fail has been localized to a leakage between the polysilicon wordline gate and the p-well. Currents could be accurately measured down into the range of at least 40 pA at 3V, proving the good isolating characteristics of the SiOx probe pad layer.


Further for physical localization of holes in thin oxide layers, a completely in-situ FIBSEM technique that combines ion milling, XeF2 staining and SEM imaging is presented. Ion milling in a top-down polishing mode parallel to the sample surface is used.


The milling progress is monitored in the SEM and


stopped several tens of nanometers above the gateoxide of the failing cell in the polysilicon layer of the wordline. The remaining silicon is removed by applying XeF2 without beam assistance to the surface. After 2 minutes of total etch time pin holes in the gate oxide of the bad cell were highlighted in a SEM image. A similar technique can also be applied to highlight holes in other insulating layers, which are embedded into silicon, e.g. the node dielectric layer of a trench capacitor. Furthermore the method allows the preparation of top-down transmission electron microscopy (TEM) samples, where the silicon is etched from both sides so that only the oxide layer remains for inspection.


The strength of the dualbeam FIBSEM for applications in the failure analysis of devices with


structures below 0.25 µm is to provide very high precision selective milling and etching procedures combined with the capabilities of a high resolution SEM to monitor these processes in-situ. All ex-situ methods (e.g. using conventional polishing wheels or wet chemistry) suffer from long preparation times caused by frequent sample transfers into a SEM for monitoring. Loss of the target due to overexposure of the sample is a serious risk in all ex-situ methods.


The FIBSEM enables the analyst to perform the quick and high precision sample preparation that is mandatory to succeed in the failure analysis of modern semiconductor technologies.


1) P. Singer, Semiconductor International, 10, 78-82 (1996)


2) K. Gamo, Nuclear instruments & methods in physics research, 1/4, 464ff (1997)


3) R.J. Young and J. Puretz, J. Vac. Sci. Technol. B,13(6), 2576-2579 (1995)


4) L.R. Harriott, Jpn.J. Appl. Phys., 33, 7094-7098(1994)


5) S. Lipp, L. Frey, C. Lehrer, B. Frank, E. Demm,S. Pauthner, H. Ryssel, J. Vac. Sci. Technol. B,14, 3920-3923 (1996)


6) L. Nesbit, J. Alsmeier, B. Chen, J. DeBrosse, P.


Fahey, M. Gall, J. Gambino, S. Gernhardt, H.


Ishiuchi, R. Kleinhenz, J. Mandelman, T. Mii,M. Morikado, A. Nitayama, S. Parke, H. Wong,G. Bronner, IEDM Digest of Techn. Papers,627ff (1993)


7) E. Adler, J. DeBrosse, S. Geissler, S. Holmes,M. Jaffe, J. Johnson, C. Koburger, J. Lasky, B.


Lloyd, G. Miles, J. Nakos, W. Noble, S.


Voldman, M. Armacost, R. Ferguson, J. Res.


Develop., 39 167-187 (1995)


8) M. Ruprecht, DDA Burlington, private communication


Electronic Device Failure Analysis Society, editor, p 317-325


DOI: 10.1361/cp1999istfa317


# Die Backside FIB Preparation for Identification and Characterization of Metal Voids


Die Backside FIB Preparation for Identification and Characterization of Metal Voids


Ann N. Campbell and William F. Filter


Both the increased complexity of integrated circuits,resulting in six or more levels of integration, and the increasing use of flip-chip packaging have driven the development of integrated circuit (IC) failure analysis tools that can be applied to the backside of the chip.


Among these new approaches are focused ion beam(FIB) tools and processes for performing chip edits/repairs from the die backside. This paper describes the use of backside FIB for a failure analysis application rather than for chip repair. Specifically, we used FIB technology to prepare an IC for inspection of voided metal interconnects (“lines”) and vias. Conventional FIB milling was combined with a superenhanced gas assisted milling process that uses XeF2 for rapid removal of large volumes of bulk silicon.


This combined approach allowed removal of the TiW underlayer from a large number of M1 lines simultaneously, enabling rapid localization and plan view imaging of voids in lines and vias with backscattered electron (BSE) imaging in a scanning electron microscope (SEM). Sequential cross sections of individual voided vias enabled us to develop a 3-d reconstruction of these voids. This information clarified how the voids were formed, helping us identify the IC process steps that needed to be changed.


Performing FIB circuit modification from the backside of a chip has become routine for flip-chip packaged ICs, where backside access to the chip is required if electrical operation of the IC is to be preserved in the original package [1-4]. Backside FIB modification is also being considered for making repairs at lower-lying nodes (e.g., M1) in multi-layer non-flip-chip ICs that would otherwise require elaborate circuit modification from the front side. Beyond this, backside FIB sample preparation techniques offer a powerful new capability


which failure analysts are just beginning to exploit.


This paper describes one such failure analysis application: the use of backside FIB milling combined with conventional FIB milling, imaging, and crosssectioning to enable the investigation of voiding and etch defects in a 2-level metal (aluminum) CMOS technology.


The goal of our study was to identify and image voiding at the M1 level and in the M1 to M2 vias without performing any deprocessing steps that would introduce additional voiding or alter existing voids.


Backscattered electron (BSE) imaging performed at the highest primary beam energies (say, 30-40kV) of most scanning electron microscopes (SEMs) can often be used to characterize voiding from the front side of the chip [5], but with limited resolution and only in the uppermost interconnect layers. The resolution of BSE void images suffers even for the top level metal due to the thickness and, for unplanarized technologies, the roughness of the passivation layer covering it.


Obtaining crisp images of voids in vias or deeper levels of metal from the front side is problematic because of the thickness of overlying materials and the nonplanar topography in some IC technologies. In our case, the M1 to M2 vias were formed from aluminum as part of the M2 deposition, resulting in a highly nonplanar topography that produced marked shadowing in the SEM images of the vias. More important, however, the presence of a TiW layer at the bottom of M1 prevented imaging of the voids in M1 and in the vias. The strong backscattered signal from the TiW overwhelms the signal from the aluminum interconnect, obscuring any evidence of voiding. While FIB cross-sections through vias or buried metal layers can be used to image voids,only one location or via can be studied at a time, and this technique obviously cannot be used to locate the voids in the first place. Thus, it was necessary to remove the TiW underlayer in order to successfully perform BSE imaging of the voids in M1 and in the M1


to M2 vias. The backside FIB technique described in this paper exposes long lengths of interconnects and many vias at one time, allowing voids to be located as well as imaged.


In order to remove the TiW underlayer, we first needed to expose the M1 lines from the backside of the chip.


A Micrion 9800FC FIB system, designed for performing chip repair from the back side, was used for this purpose. This FIB system uses super-enhanced gas assisted milling for quick, uniform removal of the silicon substrate and also has an integrated high resolution infrared (IR) microscope to identify the areas of interest from the backside of the chip.


Super-enhanced gas assisted milling of Si uses the same etchant gas, XeF2, that is commonly used for the selective removal of SiO2 and W during “normal” gas assisted milling in a FIB. An important difference between the two processes is the degree of enhancement, which is defined as the increase in material removal during gas assisted milling compared with FIB milling without gas. In the latter case,material removal is accomplished solely by ion sputtering, whereas in the former case a chemical reaction increases the amount of material removed per unit ion dose. The typical enhancement for “normal”gas assisted milling is a factor of 10 – 20. In contrast,the enhancement for super-enhanced gas assisted milling of Si is ~1000x. This super-enhancement leads to very fast processing times; for the samples used in


this study, the silicon (100 – 150  µm thick) was completely removed from areas up to 350  µm x 350 µm in size in less than 30 minutes.


Super-enhancement of Si removal is achieved through


the use of a high current density (20 A/cm2) FIB column combined with a patented gas delivery nozzle for XeF2. As shown in Fig. 1, the ion beam passes through the center of a round nozzle; this nozzle delivers a high XeF2 flux uniformly to the area scanned by the beam, eliminating the directionality effects that are problematic in performing XeF2 backside gas assisted milling with the single needle-shaped gas delivery nozzles that are standard for most FIB systems


[1]. This special gas delivery approach both superenhances the milling process and provides a very smooth milled surface. The nozzle is positioned a few hundred microns above the sample. The system base


pressure (1 x 107 torr range without gas flow) is monitored as the XeF2 gas is introduced and reaches a maximum of ~2 x 10-5 torr. The beam current required for a high rate of silicon removal is about 20nA in a


spot approximately 0.5  µm in diameter.


Figure 1 Special nozzle used for super-enhanced gas assisted milling for backside sample preparation


The high resolution IR microscope integrated into this FIB system detects wavelengths from approximately


0.9 to 1.9  µm. IR imaging was used to locate features of interest from the chip backside, and then localized milling was used to rapidly and completely remove the silicon substrate over the area of interest. The FIB system’s laser interferometer stage enables reliable alignment and registration between the FIB image and the IR microscope image.


The samples used in the study were individual dice


which were first pre-thinned to 100 - 150  µm by mechanical polishing. Pre-polishing the sample quickly removes relatively large amounts of silicon and also facilitates infrared (IR) imaging of the circuitry


100 - 150  µm beneath the surface by reducing the amount of reflection and diffraction at the back surface.


Backside FIB preparation was used in preference to global thinning of the backside of the samples with parallel polishing for several reasons. First, our objective was to expose a number of lines and vias simultaneously with as little thickness variation as possible. Backside thinning accomplished with the polishing wheels used in most FA labs generally cannot achieve the required flatness; the typical thickness variation is a few micrometers over the width of the die. In contrast, the super-enhanced gas assisted milling process permits the complete removal of the Si substrate, exposing the flat back surface of the field and gate oxides. Perhaps more important, globally thinned dice are extremely difficult to handle. Local thinning accomplished with FIB leaves the bulk of the


die thick enough (~ 150  µm) to handle with relative ease. Another advantage of the backside FIB tool for this application is that the IR imaging capability permitted easy identification of the locations of interest for local thinning.


Substrate Special


Nozzle


XeF2


Focused ion beam


Circuit


After loading the sample in the FIB system, the area of interest in the circuit is located with the IR microscope.


For optimum image collection, the optical beam needs to be perpendicular to the sample surface. However,this is also the required angle of incidence for the ion beam, and thus the system was designed with the IR microscope off-axis from the ion beam. The position of the sample is translated back and forth between the FIB and IR microscope with a high degree of accuracy


(0.25  µm) by using the system’s laser interferometer stage. Once registration between the FIB and optical images is established, the area(s) to be milled are defined in the IR mode. The system is then returned to FIB mode, the milling parameters are established, and controlled removal of the bulk silicon begins.


The optical microscope identified areas of interest,which have a high density of M1 lines and M1 to M2 vias. A backside IR image of one such area is shown in Fig. 2. Backside IR images of the same area are shown in Fig. 3 after the removal of about half of the Si


(70  µm remains) and in Fig. 4 following complete removal of the silicon substrate.


Figure 2 A portion of the IC imaged through the


backside of the chip. The Si substrate is approximately


150  µm thick.


Typical rates of removal have been calibrated for specific milling conditions (e.g., beam current density,XeF2 pressure, etc.) and, using the calibrated values,the ion dose necessary for complete removal of the Si was estimated. The actual dose required to completely remove the Si varied with the remaining Si thickness,


and was approximately 0.25 – 0.3 nC/ µm2 for samples with 75 – 100 µm remaining silicon. This is consistent with the expected acceleration of about 1000x for super-enhanced FIB/XeF2. During FIB processing, a


visual endpoint frame was used to determine when the Si had been completely removed from the backside of the sample. The endpoint frame was monitored until the entire area was completely clear of Si, and then the FIB/XeF2 milling was stopped. Because the acceleration of Si removal by FIB/XeF2 is about 100x greater than the removal of SiO2, very little loss of planarity of the surface is introduced by the fact that the milled area has sloped edges that clear last during milling.


Figure 3 IR image through the chip backside following partial removal of the Si substrate. The remaining Si is


approximately 70  µm thick.


Figure 4 IR image of the chip backside following


complete removal of the Si substrate. The M1 lines are horizontal and M2 lines are vertical. Representative M1 to M2 vias are indicated by arrows.


30 µm


Figure 5 (a) R image of an area to be marked, with the


mill box area defined. (b) optical micrograph of


backside-thinned sample. The area of interest has been marked (arrow) by straight sputter milling.


After super-enhanced FIB/XeF2 milling had removed the Si substrate, additional FIB milling was performed in a conventional FIB system. The change of FIB systems was for logistics reasons only; conventional FIB milling can also be performed in the flip-chip FIB.


In fact, before removing the samples from the flip-chip FIB system, straight sputter milling was used to mark the areas of interest so that they could be easily located in our conventional FIB system which lacks an IR


imaging capability. Shallow trenches (about 0.125 µm deep) were milled to mark these areas. Fig. 5a is a backside IR image showing the definition of the mill box. Fig. 5b is an optical micrograph showing the


entire thinned area (350  µm x 350  µm) as well as the marked region, indicated by an arrow. Optical images


such as Fig. 5b are used to assist with navigation on the samples in the conventional FIB system.


Figure 6 shows a “cartoon” cross section of the samples used for this study. The cross section shows the presence of polysilicon “pedestals” beneath the M1 to M2 vias. In many flip-chip FIB applications,“normal” XeF2 gas assisted milling would be used to accelerate the removal of the SiO2-based inter-level dielectric (ILD) while performing FIB-milling to reach a node of interest in a circuit repair application [5,6].


However, our objective was to keep the sample surface as flat as possible so that the M1 lines would be exposed uniformly without overetching or undercutting. Because the selectivity of XeF2 is higher for polysilicon than for SiO2, the polysilicon pedestals


(0.5 µm thick) would be removed much more quickly than the surrounding ILD if “normal” FIB/XeF2 were used, leading to the formation of depressions in the sample surface. During subsequent milling, the backside of M1 would not be exposed uniformly, but instead the backside of the vias would be reached first,and the metal would be undercut in those regions by the time the rest of the M1 backside was exposed. On the other hand, the via regions actually sit slightly further away from the backside of the sample than the surrounding M1, as shown in Fig. 6. With straight sputter milling, the backside of M1 in via regions will be exposed last, but the deviation in surface flatness will be less than if the FIB/XeF2 approach is used. For these reasons, straight-sputter milling was used to remove the layers once the Si substrate had been removed even though this is a much slower process than “normal” XeF2-assisted milling.


Conventional FIB milling was performed in a Micrion 9000 (25 nm/30 keV column) to remove the ILD and expose M1 from the backside. The approximate milling dose required for material removal was calculated from known layer thicknesses. A visual endpoint frame was continuously monitored, and the milling dose adjusted as needed. An ion dose of ~ 4.75


nC/  µm2 was used to remove the ILD and polysilicon pedestals, exposing the backside of M1. As the M1 layer was approached, the milling process was


interrupted frequently (every 0.1  µm or so). Once the M1 lines were exposed, milling was performed in


increments of 0.025 – 0.05  µm until the TiW was removed. Between mills, a high resolution secondary electron mode FIB (SEFIB) image was acquired to monitor removal of the TiW more closely. Figure 7 is one such image showing the early stages of TiW layer removal. The etch rate of the TiW appears to vary with grain orientation, leading to roughening of the layer as it is removed, creating a “speckled” appearance. The TiW at the ends of the lines has not yet been appreciably etched, and thus exhibits more uniform contrast than the lines themselves.


Figure 6 Cartoon cross section of M1 to M2 via in material used for this study. The M1 and M2 lines are parallel to


each other, and run left to right in this field of view.


Figure 7 Secondary electron mode image showing


the backside of several of M1 lines. A moderate


amount of the TiW underlayer remains (areas of dark


contrast along the lines and at the ends).


The die was removed from the FIB and examined in


the field emission SEM (FESEM) at several stages


during removal of the TiW layer. Fig. 8 shows 3 keV


FESEM images of these lines with increasing


amounts of TiW removal. The TiW layer has bright


contrast in the FESEM images compared with darker


contrast in the SEFIB image (Fig 7). Voids are


visible at the ends of several of the M1 lines, which


correspond to the location of M1 to M2 vias. It


should be noted that the large, circular holes in M1


are not voids, but are pitting that likely resulted from


residual polishing debris that remained on the surface


during backside milling.


Figure 8 3 keV FESEM images of several M1 lines.


In (a) the via regions are mostly covered by TiW(bright contrast). In (b), the TiW has been removed almost completely and voiding is visible (arrows).


HBSQ


4.1 µm


passivation


BPSG


polysilicon pedestal


field oxide


silicon substrate


TiAl3


TiW


{


Figure 9 Increased magnification FESEM images of vias. (a) shows a 3 keV image of via 1 from Fig. 8 with no apparent voiding. (b) is a 30 keV BSE image of the same via showing subsurface voiding


(indicated by arrows). (c) is a stress void in a


different via.


The images shown in Figure 9 demonstrate that the voids in Fig. 8 are not an artifact of FIB milling.


These images show a higher magnification view of the M1 via labeled “1” in Fig. 8. Fig. 9a is an FESEM image taken at 3 keV, which shows the


surface structure of the line; no voiding is visible.


Fig. 9b is a 30 keV BSE image of the same location,clearly showing the presence of subsurface voiding.


The subsurface void in Fig. 9b has the same crescent shape as the void that intersects the sample surface in the M1 line labeled “4” in Fig 8. The crescentshaped morphology suggests that these voids lie along the perimeter of the circular via; the images of voids in vias 1 and 4 (Figs. 8 and 9) together suggest that the voiding may occur in both M1 and the via.


Fig. 9c is an image of a void that extends into the via;this void is thought to be a stress void.


In addition to revealing voids in vias, BSE imaging also permits viewing voids in M1 and M2. Figure 10a shows both a number of voids along the edges of the M2 lines and that no appreciable voiding is observed in M1 in this field of view. Figure 10b is the identical field of view, imaged from the front side of the die. The mirror image of the BSE front side image is shown here so that the field of view exactly matches that from the back side. Voiding in the vias and M2 lines is much more visible in the backside images (Fig. 10a).


Figure 10 30 keV BSE images showing voiding at the edges of the M2 lines. (a) BSE image from the


backside of the die and (b) the same field of view


from the frontside. The arrow indicates the same edge void in each image.


M2 M1


Figure 11 Cross section through via 4 showing


voiding in both M1 and M2.


We performed a series of FIB cross sections through several of the vias that exhibited crescent-shaped voids in M1. The following images of the cross sections are all secondary electron mode FIB images.


Fig. 11 is a cross section through via 4 (Fig. 8). This image shows voiding in both M1 (top surface) and M2 (on the face of the cross section), suggesting a possible connection between the two voids. Fig. 12 is a series of images showing the sequential cross sectioning of another via associated with a crescentshaped void in M1. The distance between sequential


cuts is ~ 0.5  µm.


Figure 12 These 5 FIB images shows a series of


cross sections through a voided via. (a) First cut,showing no voiding. (b) Second cut, showing voiding both in M1 and M2. (c) Third cut showing extensive


M2 voiding. (d) Third cut, with image contrast


adjusted to show that the M1 void is connected to the passivation surface. (e) Final cut, showing that voids


in M1 and M2 are physically continuous. All are


secondary electron mode FIB images; Figs. a – d were imaged with the 30 keV, 25 nm ion column, and


Fig. e was imaged with a 50 keV, 5 nm column.


M1 void


voids


M2 void


Passivation notch


M2 void s


Via void


Fig. 12a is the first cut into the via, with no voiding apparent. Fig. 12b is the second cut, showing some voiding (dark areas) in M2 as well as a notch-shaped void in M1. The M1 void, in plan view, is what we refer to as a crescent-shaped void shown in Figs. 8 and 9. The third cut is shown in both Figs. 12c and d.


Fig. 12c is a high contrast, low brightness image


showing extensive M2 voiding. In Fig. 12d, the


brightness was increased to show that the notch void in M1 is connected to the passivation surface through a notch in the passivation caused by a “breadloafing”processing defect. The final cut, shown in Fig. 12e,indicates that the voids in M2 and M1 are physically


connected. This suggests that the void may have nucleated in one metal level and subsequently grew to include both metal levels.


Figure 13 FESEM image of M1 to M2 vias. (a) 5


keV FESEM image showning the misalignment


between M1 and M2. M1 is covered with a biassputtered quartz interlevel dielectric. The M2 lines are not passivated. (b) Cartoon depicting the


intended and actual alignment of M1 and M2. M2 is displaced upward and to the right relative to where it should be.


In addition to the voiding shown in Figs. 8 – 12, we observed significant misalignment between M1 and M2 in this material. Fig. 13 shows the misalignment of M2 relative to M1 in both an FESEM image (Fig.


13a) and in a cartoon representation (Fig 13b). In this field of view, M2 is displaced to the right and upward relative to its intended location.


Figure 14 Illustration of processing defects leading to M1 and M2 voiding. (a) shows the shallow taper of the M1 to M2 via hole etch. (b) shows the


intended M2 patterning. (c) shows the effects of M2 misalignment, overetching of M2, and passivation breadloafing on the structure of this via.


M2 mask


misalignment


M2 free


surface/void


M2 overetch Breadloafing


Passivation


(C)


Asymmetric via-hole etch profile with shallow taper


Intended location of M2 edge


M2 {


Ideal


Actual


Crescent of exposed M1


M1 b


Combining the 3-dimensional understanding of the void morphology derived from the information in Figs. 5 – 12 with the known M2 misalignment (Fig.


13) led to the following understanding of the voiding process in this technology. Fig. 14 illustrates the backend process steps, showing how the M2 misalignment leads to the observed voiding. Fig. 14a shows the shallow taper of the via hole etched through the high bias-sputtered quartz (HBSQ)interlevel dielectric. Fig. 14b shows the blanket M2 film deposited and also indicates where the end of the M2 interconnect is intended to be. Recall that Fig.


13b showed a top view of the misalignment of M2 to the via hole and to M1 after M2 patterning and etching. Fig. 14c shows that mis-alignment causes the M2 edge (and, one can imagine, the side of the M2 line) to coincide with the via hole. When M2 was overetched in this instance, the etch cleared the M2 out of the via in a crescent shape and proceeded to attack M1 as well. Because of the shallow taper of the via hole, the severe topography of the M2 sidewall, and the deposition characteristics of the passivation, the passivation layer does not completely seal the M2, leaving exposed free surfaces which can act as sources of vacancies for the formation of stress voids in M1 and the M2 vias. The fairly “clean”crescent-shaped voids in Fig. 8b are caused by the M2 etch. The irregularly-shaped voids in M2 in Figs.


11 and 12 were determined by other analytical work(not reported here) to be stress voids. Thus, the M2 misalignment and concomitant etch defect create the nucleation point for the larger stress void network that forms in M2. The voids noted at the edges of M2 (Fig. 10) are also stress voids that nucleated from metal sidewall etch defects.


Conventional BSE SEM imaging of the front side of an IC can detect voids in the top metal layer with somewhat limited spatial resolution. Severe topography, materials, and the depth of the layer of interest can prevent the clear detection and characterization of voids in vias and buried metal layers. We have demonstrated that backside thinning in a FIB system can be combined with conventional FIB milling to enable the inspection of voiding at lower lying metallization layers. In particular, we used backside thinning to remove the TiW underlayer from M1 that prevented successful front-side detection of voids with BSE imaging in a SEM. This sample preparation approach allowed us to view the voiding in many vias at once and was crucial in developing an accurate model of how voiding occurred in the vias on this material. BSE imaging from the backside yielded sharper images of voids than is possible from the front side because the amount of material between the void and the surface


is reduced and because the backside preparation eliminates surface roughness.


Backside FIB techniques can be used to expose large areas on a chip; in this study, we used backside FIB processes to remove the silicon substrate from areas up to


350  µm x 350  µm in size. This planar approach permits inspection of a large number of lines and vias relatively quickly and is therefore much more timeeffective than performing cross-sections on a number of individual vias.


The authors thank Bonnie McKenzie, Joe Michael and Alex Pimentel of Sandia National Laboratories for their support of this work, and thank Dennis Kramer, Jeremy Walraven, and Richard Anderson,also of Sandia, for their careful review of the manuscript. Sandia is a multiprogram laboratory operated by Sandia Cor-poration, a Lockheed Martin Company, for the United States Department of Energy under Contract DE-AC04-94AL85000.


1) P. F. Ullmann, C. G. Talbot, R. A. Lee, and C.


Orjuela, Proceedings of the 22nd International Symp. for Testing and Failure Analysis, p. 381,18 – 22 Nov. 1996


2) R. Lee and N. Antoniou, Proceedings of the 24th International Symp. for Testing and Failure Analysis, p. 455, 15 - 19 Nov. 1998


3) N. Antoniou, Solid State Technology, p. 63, Dec.


1998


4) R. H. Livengood and V. R. Rao, Semiconductor International, p. 111, March 1998


5) Scanning Electron Microscopy and X-Ray Microanalysis, 2nd edition, ed. J. I. Goldstein et al, p. 220, Plenum Press, New York, 1992


6) M. Abramo, L. Hahn, and L. Moszkowicz, Proceedings of the 20th International Symp. for Testing and Failure Analysis, p. 439, 13 - 18 Nov.


1994


7) S. X Li, Proceedings of the 24th International Symp. for Testing and Failure Analysis, p. 67, 15


- 19 Nov. 1998


Electronic Device Failure Analysis Society, editor, p 327-331


DOI: 10.1361/cp1999istfa327


# FIB Micromachining and Nano-Structure Fabrication


FIB Micromachining and Nano-Structure Fabrication


Raymond A. Lee and Patrick J. Wolpert


FIB Micromachining has long been an established technique, but until recently it has been overshadowed by the more mainstream semiconductor application of the Focused Ion Beam system. NanoStructure fabrication using the FIB system has become more popular recently due to several factors.


The need for sub-micron structures have grown significantly due to a need for enhanced optical and biological applications. Another reason for the growth in micromachining is the improvement made in the ability of FIB systems to produce geometric shapes with high precision. With the latest high-end FIB systems, it is possible to produce microstructures with tens of nano-meters of precision. Optical lens,AFM tips, and nano-apertures are all part of the growing application for FIB Micromachining. This paper will discuss the ability and limitations of the FIB system and some possible application for FIB Micromachining.


FIB micromachining was the first application developed for the FIB system, but until recently it has only been explored in universities and R&D laboratories. The lack of development in FIB micromachining was due to a deficiency in technology. Until recently the poor milling resolution and speed compounded by limited rastering technology have made FIB a secondary choice compared to other micromachining techniques. (E.g. Electron-beam lithography, RIE, etc.) New developments in FIB column technology and new rastering and scan generation algorithms have given FIB significant new advantages in the world of nano-structure fabrication.


New high resolution and high beam current FIB columns allow for quick removal of bulk materials,


while still allowing for sub-micro precision in mill tolerance and accuracy. New scan generation and rastering hardware allow for complex patterns to be produced with pinpoint accuracy. The combination of the above hardware and software features allows FIB technology to be used in quick prototyping of all kinds of micromachining structures.1-5


AFM


The possible applications for FIB micromachining are limitless. For the purpose of this paper the scope will be limited to the semiconductor industry. The first and major use of the micromachining features of the FIB is to produce and shape AFM tips for ultra high resolution and aspect ratio. Due to the difficulty of manufacturing, AFM tips are traditionally made from single crystal materials like silicon, which are easy to manipulate. The nature of single crystal silicon lends itself to the etching process, which create the sharp tips of the AFM. The usage of silicon also creates several problems. While silicon is a great semiconductor, it lacks the hardness of a material like diamond, which gives it a limited lifetime. It lacks electrical conductivity, which limits its probing capability, and the crystalline structure of silicon also limits the aspect ratios of the tips. Using FIB systems, AMF tips can be made out of any material.


Diamond and other carbide materials can be used to increase the strength and durability of AFM tips.


Conductive materials like tungsten can also be used,which can generate both topographical images and also electrical data.


In order to create an AFM tip from different materials, several parameters need to be determined.


First a suitable pattern needs to be established for the


milling. Most new FIB systems allow for some type of polygonal milling. The milling is normally achieved in two steps. The first step is used to create the rough shape needed for the tip (See Fig. 1).


Figure 1 Coarse milled AFM tip.


A large beam current is used to shape the material into the desired shape and then a fine beam is used to trim the tip to the high aspect ratio and sharpness required (See Fig. 2). With conductive material it is very easy to product a very sharp tip. A fine beam rastered in a circular pattern around a post will generate a very sharp tip because the beam tail will sharpen the unmilled area. With non-conductive material, it is much harder to produce the same sharpness and aspect ratio. Most non-conductive materials will charge up under the positively charged beam and cause drift and vibrations. Extra care must be taken in the sharpening of non-conductive material.


Figure 2 Fine milled AFM tip.


Optical Lens


Another potential usage of FIB micromachining is the formation of optical lenses to increase the resolution limit of light. As semiconductors go to smaller and smaller geometry, light resolution limits are rendering optical inspection, imaging and photolithography systems obsolete. Optical lenses can also be manufactured using FIB systems.


FIB micromachining can quickly create prototype lens configurations to allow experimentation of different lens designs. The most difficult part of lens milling is to create the proper curvature required by the lens.


Until recently the only way to create the curvature of the lens was to use a series of rings with increasing diameters milling at different depths. The more rings used, the more the surface approximates a smooth curve. The difficulty with this setup is that the number of rings needed to achieve a smooth surface is too large to manipulate. Also it is mathematically difficult to translate a curvature into a series of discrete depth measurement. A better way to approximate the curvature needed is to use the bitmap function available on recent model FIB machines.


The curvature of the lens needs to be translated into a gray scale image, where the depth at each location is represented by a different gray scale level. Once the 256 level gray scale image is created, it needs to be reduced to a binary bitmap using the Stucki Error Diffusion (See Fig. 3). Using the above method, a bitmap image can be created where there is an increasing density of dark pixels from the center to the edge of the circle. The rate of increasing density is equal to the curvature of the lens needed. The bitmap is then used as a guide for the FIB rastering control. The dark areas are milled with the beam,


while the white areas are blanked with no milling. A constant milling dose is applied to the entire area,but due to the density of black pixel in the outer areas of the circle, it is milled deeper than the center.


Figure 3 Gray scale image and bitmap conversion.


The depth within the circle is linearly dependent on the density of black pixels, which is dependent on the gray scale of the original image. Using this method,an accurate representation of the curvature of the lens can be created very quickly. It is very easy to experiment with changing the curvature of the lens by varying the gamma scale of the original image.


Figures 4-7 gives examples of bitmaps and the resulting lens curvatures.


Figure 4 Bitmap and FIB milling results.


Figure 5 Bitmap and FIB milling results.


Figure 6 Bitmap and FIB milling results.


Figure 7 Bitmap and FIB milling results.


Nano-apertures


With the high precision of the FIB, it is also possible to create apertures in the 10nm range. These small apertures can be used for a variety of purposes. One of the major problems with creating apertures using the FIB is the aspect ratio limitation imposed by the sputtering characteristic of the Gallium beam. Using straight sputtering, the best aspect ratio that can be achieved using a FIB tool is approximately 5:1. With gas enhancement, this aspect ratio can be increased to between 10-20:1 depending on the materials being milled. This aspect ratio limitation dictates that a FIB aperture must either be very thin or must be done in a reverse pyramid shape. A material with a known thickness must be used. While conductive materials are the best to use, almost any can be used for nanoapertures.


Figure 8 Diagram of FIB machined aperture.


The nano-aperture must be made using decreasing size steps to avoid the aspect ratio limitation (See Fig 8). The aperture material must first be thinned until it is about 500nm at the thinnest point. The coarse thinning process can be achieved using a large beam current and the area can be periodically checked with a laser-scanning micro-scope for accurate depth measurement. Once the desire thickness of 500nm has been achieved then a small beam current (~ 5pA)can than be used to punch a hole through the remaining material at the desire size. An opening of around 10nm can be achieved using this technique.


At this beam current, the physical spot size of the ion beam is around 5nm, but due to ion sputtering interaction, the milling resolution is closer to 10nm.


Therefore, the smallest break through possible given current ion beam technology is around 10nm (See Fig 9).


Figure 9 10nm aperture opening in gold.


One method of ensuring the smallest aperture size possible is to minimize the milling time after breakthrough. At the exact moment the ion beam mill through the material, the opening is very small.


However, due to drift, vibration and other interference, the opening will continue to enlarge in milling is not stopped. A method needs to be found to allow the detection of the moment of breakthrough.


One technique is to rely on the secondary electron endpoint detection. In order to get a secondary electron differential; a material transition is needed in the milling area. The simplest method is to coat the back side of the aperture with a very thin film of material which will give a different level of secondary electron reading which will allow the operator to detect the break-through. To achieve the highest differential in secondary electron, conductive


apertures should be coated with non-conductive material and vice versa. Also, since the film is a sacrificial layer, an easily removable material should be selected to minimal damage or aperture enlargement during the removal process. Copper is a good material for non-conductive apertures and silicon oxide for conductive apertures, since both of these materials have very high selective removal rates.


Other Possible Applications and Future Development


The previously discussed lists of applications are only examples of the possibility of FIB micro-machining.


With improvements in its rastering capability and beam position accuracy, FIB can be expanded to cover a variety of other applications. It can be used to etch masks for both x-ray and photolithography usage (See Fig 10).


Figure 10 FIB micromachined serpentine grid


pattern.


FIB can also be used to etch serial number into samples for identification and security proposes. One of the major limitations of micromachining is the limited rastering generation of most FIB system. As patterns and designs become larger and more complicated, the number of pixels required in each pattern also increases. All current FIB systems have hardware limitation on the maxim number of pixels within each pattern due to memory capacities. In order for FIB to become a true micromachining option, the memory capacity for rastering generation needs to be significantly increased to accommodate a variety of patterns and sizes. Another area for


improvement is the generation of the software pattern for milling. Currently the only way to input data into the FIB is using bitmaps. It would be much easier if the FIB was able to extract layout information from standard formats like GDS2 and other software. This would enable designs to be constructed more precisely and easily altered.


FIB micromachining has only begun to explore the possible ranges of its potential applications. Due to its versatility and adaptability, FIB technology can be applied to all types of machining applications. Its major advantage are the quick turnaround and easy of use. For micromachining, FIB is essentially a direct write method of milling. No physical mask or mold needs to be made for the micromachining. These features make the technique ideal for R&D phases of development where quick turn-around and verification of designs are critical. Variations on designs also can be tried without wasteful retooling costs. The main disadvantage of FIB micromachining is limited etch speed of the ion beam. While FIB is much faster in producing one prototype, it is much slower in producing large quantities of samples, as each sample needs to be done in series as opposed to parallel.


Electron lithography and other mask and etch techniques are still the main source of production level components. However, FIB systems can be made to produce a mold of a desired microstructure that can then be used in production. Since the FIB is only used for the initial mold, the time is reduced.


The mold can then be used to produce the necessary volume of final product. Using the mold method, FIB offers a complete solution from R&D to production in micromachining. With the current advances in technology, FIB dose offers a significant advance in areas of R&D and low level production and prototyping.


1) RK Defreez, et al, SPIE Vol. 1043 Laser Diode Technology and Applications, 25-35 (1989)


2) PG Blauner, et al, J. Vac. Sci. Technol. B 7 (4)609-617 (1989)


3) R Clampit, KL Aitken, and DK Jefferies, J. Vac.


Sci. Technolo. 12, 1208 (1975)


4) Y Mashiko, H Morimoto, H Koyama, S Kawazu, T Kaito, and T Adachi, 25th Annual Reliability Physics, San Diego (April 1987)


5) T. Ishitani and T. Onishi, Jpn. J. Appl. Phys. 28 L320 (1989)


Electronic Device Failure Analysis Society, editor, p 335-341


DOI: 10.1361/cp1999istfa335


# Characterization and Fault Identification of Copper BEOL Sub 0.25µm Six Level Metal Microprocessor Designs


Characterization and Fault Identification of Copper BEOL Sub 0.25µm Six Level Metal Microprocessor Designs


T. Kane, K. DeVries, M. Tenney, A. Patel


IBM Advanced Semiconductor Technology Center, Hopewell Junction, New York


Characterizing and fault localizing sub 0.25µm six level copper BEOL microprocessor RISC designs operating above 450 MHz clock speeds pose significant challenges in functional defect localization and identification. The flip chip designs of these microprocessors with high numbers of I/O outputs can involve backside and frontside fault localization techniques such as emission microscopy,OBIC (Optical Beam Induced Current) using I.R.


laser scanning microscopy, LIVA (Light Induced


Voltage Alteration)[1,2], and PICA (Picosecond Imaging Circuit Analysis)[3,4], to identify the source of functional failures.


Refined backside thinning techniques have been applied to optimize I.R. laser scanning microscopy and PICA localization of functional failures.


In addition, products using highly structured test methods such as LSSD(Level Sensitive Scan Design)lend themselves to a highly software diagnosable category [5,6]. Such software diagnostics (LSSD diagnostics) when combined with image based fault localization has proven highly effective in pinpointing defects causing functional failures.


Examples of electrical and physical characterization of functional logic failures in the six levels electroplated copper BEOL microprocessors will be described. In addition, the electrical characterization of submicron sized SRAM transistor devices using FIB (Focused Ion Beam Microscopy)deposited probe pads [7] will be detailed along with SEM and TEM micrographs of defects identified in this manner.


The six level copper electroplated BEOL microprocessor design featured in this paper involves a


twin-well CMOS design with sub 0.15µm size gates.


A total of seven metal levels (one level- tungsten; six levels- copper) are all CMP (Chemical-Mechanical Polished) planarized using a damascene process. This copper BEOL interconnection design is integrated with a flip chip package design (ceramic ball grid array or CBGA).The applicability of copper BEOL interconnections in such a high speed RISC microprocessor design is self evident. The lower resistance


of copper (<2µ Ω-cm) versus aluminum-copper(>3 µΩ -cm) when filling narrow trenches not only offers improvements in electromigration characteristics but also dramatic reductions in RC (resistance X capacitance) time delay and lower capacitance(since copper lines can be made thinner). It is these thinner, more closely spaced lines that pose added challenges in characterizing and fault localizing functional failures.


FIB Assisted Electrical Probing


The thinner, more closely spaced copper lines offering lower capacitance and higher performance in this copper BEOL microprocessor design present risks in using conventional unlayering methods in physical failure analysis. FIB GAE (Gas Assisted Etch) involving Br2 readily attacks copper unless proper controls are exercised [7]. Using techniques applied to copper, a functional SRAM cell was electrically probed using FIB probe pads.Using FIB milling with straight sputtering and XeF2, the oxide over the copper lands was removed and tungsten metal deposited to protectively cap the exposed


copper lands [7]. Figure 1 is an optical view of the eight FIB deposited pads used to functionally exercise this cell.

