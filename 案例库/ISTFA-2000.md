---
title: "ISTFA-2000.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_bd3f328d26ae59f1c3648128a372091e7295230462135641
file_size: 47314007
---

ISTFA 2000


Proceedings of the


26thInternational Symposium for


Testing and Failure Analysis 12 - 16 November 2000


Meydenbauer Convention Center Bellevue, Washington


Sponsored by


Published by


ASM International


Materials Park, Ohio 44073-0002


Copyright © 2000


by


ASM International®


All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any means, electronic, mechanical, photocopying, recording, or otherwise, without the written permission of the copyright owner.


First printing, October 2000


Great care is taken in the compilation and production of this Volume, but it should be made clear that NO WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN CONNECTION WITH THIS PUBLICATION. Although this information is believed to be accurate by ASM, ASM cannot guarantee that favorable results will be obtained from the use of this publication alone. This publication is intended for use by persons having technical skill, at their sole discretion and risk. Since the conditions of product or material use are outside of ASM's control, ASM assumes no liability or obligation in connection with any use of this information. No claim of any kind, whether as to products or information in this publication, and whether or not based on negligence, shall be greater in amount than the purchase price of this product or publication in respect of which damages are claimed. THE REMEDY HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND SOLE REMEDY OF BUYER, AND IN NO EVENT SHALL EITHER PARTY BE LIABLE FOR SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES WHETHER OR NOT CAUSED BY OR RESULTING FROM THE NEGLIGENCE OF SUCH PARTY. As with any material, evaluation of the material under end-use conditions prior to specification is essential. Therefore,specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or reproduction, in connection with any method, process, apparatus, product, composition, or system,whether or not covered by letters patent, copyright, or trademark, and nothing contained in this book shall be construed as a defense against any alleged infringement of letters patent, copyright, or trademark, or as a defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN: 0-87170-701-2


SAN: 204-7586


Materials Park, OH 44073-0002


Printed in the United States of America


iii


The image on the cover shows one of the latest developments in microelectromechanical systems


(MEMS) at Sandia National Laboratories. The device shown is an electrostatically driven mechanical actuator that operates at less than 20 volts using a simple square wave drive signal. The use of low voltages and simple waveforms to drive MEMS devices is a key issue for the evolution of MEMS-based microsystems. This actuator uses a torsional electrostatic comb drive that is coupled to an external ring gear through a ratcheting system. In this design, the application of a periodic voltage signal causes the inner combs to angularly vibrate about the torsional support springs. These small angular displacements are converted to continuous rotation of the ring gear by the ratchet pawls. Because the actuator produces a discrete displacement output for every applied voltage pulse, it can be used for precise openloop position control.


The image is courtesy of Samuel L. Miller (Manager for Advanced Concepts for MEMS) and Stephen M.


Barnes (Torsional ratcheting actuator designer) from Sandia National Laboratories. For more information,please contact:


Samuel L. Miller


(505) 844-4678


millersl@sandia.gov


or visit the Sandia National Laboratories MEMS web site at http://www.mems.sandia.gov.


iv


The Organizers of the 2000 International Symposium on Testing and Failure Analysis would like to


acknowledge and thank the following people for their assistance in editing this proceedings:


D. Bodoh


Motorola, Inc.


Austin, Texas


V. Chowdhury


Altera Corporation San Jose, California


S. Delgado


Accurel Systems International Sunnyvale, California


I. De Wolf


IMEC


Leuven, Belgium


D. Dylis


IIT Research Institute


Reliability Analysis Center (RAG)Rome, New York


B. Ebersberger


Infineon Technologies AG Munich, Germany


C. Hartfield


Texas Instruments


Dallas, Texas


C. L. Henderson


Sandia National Laboratories Albuquerque, New Mexico


L. G. Henry


ESD/TLP Consultant Fremont, California


K. N. Hooghan


Lucent Technologies Allentown, Pennsylvania


K. M. McCray


Diversified Technologies Resources Colorado Springs, Colorado


J. McDaniel


Lucent Technologies


Orlando, Florida


S. V. Pabbisetty


Texas Instruments Stafford, Texas


J. C. H. Phang


National University of Singapore Singapore


J. D. Plante


Philips Semiconductors Sunnyvale, California


H. S. Silvus, Jr.


Southwest Research Institute San Antonio, Texas


J. Soden


T. Taylor


White Oak Semiconductor Sandston, Virginia


M. Thayer


Advanced Micro Devices Austin, Texas


M. Vanzi


Universita' di Cagliari Cagliari, Italy


K.-W. Yang


Tektronix Oscilloscope Group Beaverton, Oregon


v


ISTFA 2000 Organizing Committee


Daniel L. Barton


General Chair


Richard J. Ross


General Vice Chair


IBM Microelectronics Essex Junction, Vermont


H. Stan Silvus, Jr.


Technical Program Chair


James B. Colvin


Exposition Chair


Consulting Services Newark, California


Thomas M. Moore


Audio Visual Chair


Christopher L. Henderson


Panel Discussion/User Group Chair


Sandra Delgado


Publicity Chair


Christian Boit


Seminar Committee Chair


Jerry M. Soden


Seminar Committee Vice-Chair


EDFAS 2000 - 2001 Board of Directors


Edward I. Cole, Jr.


EDFAS President


Larry Wagner


EDFAS Immediate Past President


EDFAS Vice President


Gary F. Shade


EDFAS Secretary


Visteon Microelectronics Colorado Springs, Colorado


EDFAS Director-At-Large


Infineon Technologies/FA Munich, Germany


James J. Erickson


Hughes Space and Communications Co.


El Segundo, California


Glen Gilfeather


AMD


vi


ISTFA 2000 Committee Members


Expo Committee


Jim Colvin, Chair


Consulting Services, Newark, California


Kathy Renteria


Compaq, Cupertino, California


Efrat Raz


Sela USA, Sunnyvale, California


A/V Committee


Tom Moore, Chair


Texas Instruments, Dallas, Texas


Cheryl Hartfield, Vice-Chair


Anu Barman


Oki Semiconductor, Sunnyvale, California


Chris Henderson


Sandia National Laboratories, Albuquerque, New Mexico


Scott Wills


Texas Instruments, Stafford, Texas


Lee Knauss


Neocera, Beltsville, Maryland


Edward Keyes


Semiconductor Insights, Kanata, Ontario, Canada


Stan Silvus


Southwest Research Institute, San Antonio, Texas


Charles Odegard


Seminar Committee


Christian Boit, Chair


Infineon, Munich, Germany


Dave Burgess


Accelerated Analysis, Halfmoon Bay, California


Tom Moore


Dick Ross


IBM Microelectronics, Essex Junction, Vermont


Dean Tomasi


IBM Microelectronics, East Fishkill, New York


Brent Wahl


Agilent, San Jose, California


Discretes Committee


Massimo Vanzi, Chair


Universita' di Cagliari, Cagliari, Italy


Jim Erickson


Hughes Space & Communications Co., El Segundo, California


Gary Molle


Kaiser Electronics, San Jose, California


Nathalie Labat


IXL – University of Bordeaux, Bordeaux, France


Paolo Malberti


ETH, Zurich, Switzerland


Advanced Techniques Committee


Jacob C. H. Phang, Chair


University of Singapore, Singapore


Ludwig J. Balk


University of Wuppertal, Wuppertal, Germany


Mehrdad Mahanpour


Advanced Micro Devices, Sunnyvale, California


Kiyoshi Nikawa


NEC Corporation, Kanagawa, Japan


Valluri Rao


Intel, Santa Clara, California


Backside Committee


Matt Thayer, Co-Chair


Advanced Micro Devices, Austin, Texas


Dan Bodoh, Co-Chair


Motorola, Austin, Texas


Mark E. Potter


Lucent Technologies, Allentown, Pennsylvania


Dave Vallett


Peter Nguyen


Testing Committee


Jerry M. Soden, Chair


Charles F. Hawkins


University of New Mexico, Albuquerque, New Mexico


vii


ISTFA 2000 Committee Members (continued)


SPM Committee


Bernd Ebersberger, Chair


Infineon Technologies, Munich, Germany


Roland Wiesendanger


University of Hamburg, Hamburg, Germany


Wilfried Vandervorst


IMEC, Leuven, Belgium


Phil Kaszuba


Paiboon Tangyunyong


Nobuyuki Nakagiri


Nikon Corporation, Tokyo, Japan


Techniques Committee


Ingrid DeWolf, Chair


Accurel Systems International, Sunnyvale, California


Jean-Pierre Landesman


Thomson-CSF, Orsay, France


Jennifer McDaniel


Lucent Technologies, Orlando, Florida


Chris Plougonven


IBM, Corbeil Essonnes, France


Case Histories Committee


Jim Plante, Chair


Philips Semiconductors, Sunnyvale, California


Steve Ferrier


SDG Analytic, Inc., Corvallis, Oregon


Christopher Henderson


Stacy Gleixner


San Jose State University, San Jose, California


Makoto Yamazaki


Advantest Corp., Gunma, Japan


Packaging Committee


Kathy McCray, Co-Chair


Diversified Technologies, Colorado Springs, Colorado


Cheryl Hartfield, Co-Chair


Tom Paquette


Insight Analytical Labs, Colorado Springs, Colorado


Deepak Goyal


Intel, Chandler, Arizona


Rajen Dias


Rod Martens


Hewlett-Packard, Fort Collins, Colorado


Military Committee


David Dylis, Chair


Reliability Analysis Center (RAC), Rome, New York


Perry Martin


Martin Engineering, North Highlands, California


George Slenski


US Air Force, Wright Patterson AFB, Ohio


David Johnson


Eddie White


Dale Hart


University of Dayton Institute, US Air Force, Wright Patterson AFB, Ohio


Joe Buben


Defense Supply Center Columbus (DSCC), Columbus, Ohio


FIB Committee


Kultaransingh Hooghan, Chair Lucent Technologies, Allentown, Pennsylvania Alan Street


Integrated Reliability, San Diego, California


William Vanderlinde


Microelectronics Research Laboratory, Columbia, Maryland


Ann Campbell


Rose Ring


Steven Herschbein


IBM Microelectronics, Hopewell Junction, New York


viii


Yield Enhancement Committee


Tom Taylor, Co-Chair


White Oak Semiconductor, Sandston, Virginia Seshu Pabbisetty, Co-Chair Texas Instruments, Stafford, Texas


Swee Yong Khim


United Test and Assembly Center Ltd., Singapore


Mark Ratner


LSI Logic, Fort Collins, Colorado


Luis Andrade


White Oak Semiconductor, Sandston, Virginia


EOS/ESD Committee


Leo G. Henry, Co-Chair


ESD/TLP Consultant, Fremont, California


Vijay Chowdhury, Co-Chair


Altera Corporation, San Jose, California


Advanced Micro Devices, Sunnyvale California


Koen Verhaege


Sarnoff Corporation, Princeton, New Jersey


Mark A. Kelly


Delphi Delco Electronics, Kokomo, Indiana


ix


1999 BEST PAPER AWARD


Detecting Power Shorts from Front and Backside of IC Packages Using Scanning SQUID Microscopy


L. A. Knauss, B. M. Frazier, H. M. Christen, S. D. Silliman, K. S. Harshavardhan


Neocera, Inc.


Beltsville, Maryland


E. F. Fleet, F. C. Wellstood


University of Maryland College Park, Maryland


M. Mahanpour, A. Ghaemmaghami


Advanced Micro Devices, Inc.


Sunnyvale, California


1999 OUTSTANDING PAPER AWARD


Light Emission Spectral Analysis: The Connection


Between the Electric Field and the Spectrum


D. L. Barton, P. Tangyunyong, J. M. Soden, C. L. Henderson, E. I. Cole, Jr.


R. Danz, R. Steiner


Carl Ziess, Inc.


Jena, Germany


Z. Iwinski


Carl Zeiss, Inc.


Thornwood, New York


Future ISTFA Dates


27thInternational Symposium for Testing and Failure Analysis


11 - 15 November 2001


Santa Clara Convention Center


Santa Clara, California


Be sure to put this date on your calendar!


xi


First Announcement And


ISTFA 2001 • Call for Papers


Sponsored by the ASM Electronic Device Failure Analysis Society (EDFAS)


11-15 November 2001 • Santa Clara, California, USA


ISTFA solicits original, previously unpublished papers on a wide range of Testing and Failure


Analysis topics ofpractical value to anyone working to detect, understand and eliminate electronic


device failures. Non-commercial papers from equipment vendors dealing with new or unique tools and methodologies, applications and results are welcome. Papers will be selected for inclusion in the


technical program on the basis of appropriateness and quality of data, technical importance,


novelty/originality, and interpretation of results. Paper acceptance is based entirely on the


information included in the abstract.


We are currently seeking papers on (but not limited to) the following relevant topics:


• Advanced Fault Localization Techniques


• Defect Characterization Methods


• Sample Preparation and Deprocessing Methods • Case Histories


• Discrete/Passive Component Failure Analysis


• Design for Test/Design for Analysis


• Testing and Device Characterization


• Packaging Related Failure Analysis


• Backside and Flip-Chip Analysis Techniques


• Compound Semiconductor Devices


• Micro-Electro Mechanical Systems (MEMS)


• Signature Analysis


ABSTRACT SUBMISSION GUIDELINES


Abstract Preparation:


1. Begin your abstract with the conference name, ISTFA 2001, followed by the title of your paper.


2. Type your abstract (two-page maximum) in English and include significant representative images,


figures, references, etc. All abstracts must adhere to the two-page maximum length to be considered.


Within the two-page maximum, it is highly advisable to include sufficient detail (at least one full page)


to allow for fair evaluation of the work discussed. A full copy of the manuscript in Microsoft Word


format may be submitted in addition to the abstract if desired.


3. At the end of your abstract, describe in 25 words or less, the significance of your work (conclusions


and benefits). Then list three (3) key words from your abstract that can be used for indexing in the


Conference Proceedings, and indicate to which topical area (from the list above, or “other” if


appropriate) your abstract relates.


4. On an additional page(s), provide the following information for the presenting author first, then for all


co-authors of the work: Complete name (including Dr./Mr./Mrs./Ms./Prof. etc.), title, affiliation with


complete mailing address (no P. O. Box numbers), telephone and fax numbers, and e-mail address.


This information must be included with your abstract or it will not be considered for evaluation.


Abstract and Manuscript Deadlines:


1. Abstracts must be submitted by 1 MARCH 2001 to be considered for inclusion in the program.


2. A Conference Proceedings is planned for publication and distribution at the event. A full manuscript in


Microsoft Word format must be submitted for review by 15 JUNE 2001, then in final camera-ready and


electronic formats by 13 JULY 2001.


Abstract Submission Options:


• Please e-mail your abstract as a Microsoft Word file attachment to educatn@po.asm-intl.org. In the“Subject Line,” please enter ISTFA 2001.


• If you absolutely cannot submit your abstract electronically, mail it to arrive before the deadline to:


ISTFA Conference Administrator, ASM International, Materials Park, Ohio 44073-0002 (telephone:


+440.338.5151).


Visit the EDFAS Website frequently at www.edfas.org for updates on this event.


xiii


Preface


The International Symposium for Testing and Failure Analysis, ISTFA, is the premier forum for information on all aspects of microelectronic device failure analysis. The symposium has consistently provided attendees with the latest analysis techniques necessary to obtain accurate and timely information on devicerelated issues for their customers. While the direct corporate financial benefit may be difficult to quantify in some cases, the beneficial impact of failure analysis (FA) on device quality and reliability has proven itself to the community for decades.


This ISTFA marks the beginning of the new millennium.


The state of the art in microelectronics technology greatly exceeds the predictions made just a short time ago. The rapid development of microelectronics has enabled us to reach levels of integration,operating speed, reliability, and even cost that were not imagined a generation ago.


In the FA community, this rapid technology development has forced us to develop advanced techniques. Perhaps the most amazing capabilities are those that allow us to localize faults in deep sub-micron integrated circuits through the silicon substrate. As the ability to test many modern integrated circuits (ICs) is destroyed by removing them from their packages, non-destructive techniques for flipchip technologies are essential.


This ISTFA Proceedings presents readers with a collection of the best in FA research in the industry today. As with past Proceedings, this issue will become the latest addition to the technical libraries of many laboratories and will be used frequently. The nature of the evolution of IC technology presents many of us with similar technologies and their associated problems. This commonality allows us to draw from collective research to help reduce the time and expense associated with FA.


In the future, we should see a more diverse technology base at ISTFA. The current trend is toward high performance silicon-based devices coupled or integrated with compound semiconductor optoelectronic (OE) devices and microelectromechanical systems (MEMS)devices to make integrated micro systems.


Much of this trend has developed from the needs of the internet and the desire to transfer huge amounts of data at blinding speeds.


In the FA industry, the use of OE and MEMS technologies along with silicon ICs will increase the demands for analysts with broader backgrounds and more diverse training. ISTFA has been presenting material on compound semiconductor, OE, and MEMS devices for years but in the background of the larger silicon industry. Future events will see growth in size to allow these technologies the same coverage presently found in silicon. We (the ISTFA Organizing Committee), ASM, and, the members of EDFAS, look forward to the future of failure analysis.


Daniel L. Barton, Ph.D.


Sandia National Laboratories ISTFA 2000 General Chairman bartondl@sandia.gov


xv


Table of Contents


IPFA '99 Best Paper Award Winner


Laser Voltage Probe (LVP): A Novel Optical Probing Technology


for Flip-Chip Packaged Microprocessors .................................................................................................3


W. M. Yee, Intel Technology, Penang, Malaysia; M. Paniccia, T. Eiles, V. Rao, Intel Corporation,Santa Clara, California


Session 1: Advanced Techniques


Scanning Electron Acoustic Microscopy: A Novel Tool for Failure Analysis


and Microcharacterization........................................................................................................................11


W-K Wong, Institute of Materials Research and Engineering, Singapore; J. T. L. Thong, J. C. H.


Phang, National University of Singapore, Singapore; Q. Yin, J. Fang, Shanghai Institute of Ceramics,Shanghai, Peoples Republic of China


Application of Single Contact Optical Beam Induced Currents (SCOBIC)


for Backside Failure Analysis ..................................................................................................................17


M. Palaniappan, J. M. Chin, J. C. H. Phang, D. S. H. Chan, National University of Singapore,


Singapore; C. E. Soh, Advanced Micro Devices Pte., Ltd., Singapore; G. Gilfeather, Advanced Micro Devices, Inc., Austin, Texas


Session 2: Packaging 1


Measurement of Interfacial Adhesion and its Degradation in Multi-Layer Packages, Devices,


and Blanket Films Using the Laser Spallation Technique ....................................................................25


V. Gupta, R. Hernandez, University of California, Los Angeles, California; R. Dias, V. Atluri, G. Raiser,M. Mello, L. Skoglund, P. Zimmerman, Intel Corporation, Chandler, Arizona


New FIB-Supported Approach for Wire-Bondpad Characterization ....................................................35


P. Jacob, EMPA-Swiss Federal Laboratories for Materials Testing and Research, Duebendorf,Switzerland; G. Nicoletti, EM Microelectronic Marin SA, Marin, Switzerland


Failure Analysis of Flip-Chip Bumps After Thermal Stressing.............................................................41


T. K. Hooghan, K. Hooghan, S. Nakahara, R. K. Wolf, R. W. Privette, S. Moyer, Lucent Technologies,Allentown, Pennsylvania


X-Ray Tomography for Electronic Packages..........................................................................................49


D. Goyal, Intel Corporation, Chandler, Arizona


Session 3: Test/Yield


Data Analysis Tools and Methodologies for Quick Yield Learning


in a High Volume Manufacturing Environment ......................................................................................57


L. Andrade, T. Taylor, White Oak Semiconductor, Sandston, Virginia


Failure Analysis of Killer Defects and Yield Enhancement of Flat ROM Devices


in Wafer Fabrication ..................................................................................................................................63


Y. N. Hua, Z. R. Guo, L. H. An, S. Redkar, Chartered Semiconductor Manufacturing, Ltd., Singapore


xvi


Embedded Memory Analysis for Standard Cell ASIC Yield Enhancement .........................................69


C. A. Gloor, LSI Logic Corporation, Fort Collins, Colorado


Yield Enhancement Study: Process Variation and Design Margins Leading


to Timing Issues in the RAM ....................................................................................................................77


S. Perungulam, K. S. Wills, G. Mekras, Texas Instruments, Inc., Stafford, Texas


In-Line Defect to Bitmap Signature Correlation: A Shortcut to Physical FA Results .......................81


J. Segal, A. Sagatelian, B. Hodgkins, T. Ho, HPL, Inc., San Jose, California; B. Chu, T. Singh, H.


Berman, Dominion Semiconductor, Manassas, Virginia


Session 4: Poster Session


Analysis of Leakage Failures in Flash Memory Devices and Root Cause Indentification ................89


J. N. C. de Luna, M. O. del Fierro, J. L. Muñoz, Intel Technology Philippines, Inc., Cavite, Philippines


Passive Voltage Contrast Application on Analysis of Gate Oxide Failure in 0.25 µm Technology..93


S. Zhigang, L. S. Khim, S. Redkar, Chartered Semiconductor Manufacturing, Ltd., Singapore


Forensic Microscopy in the Failure Analysis Laboratory .....................................................................97


W. E. Vanderlinde, Microelectronics Research Lab, Columbia, Maryland; D. A. Stoney, McCrone Research Institute, Chicago, Illinois


Failure Analysis Process Flows and Common Failure Mechanisms


in Flip-Chip Packaged Device ................................................................................................................107


S. Hsiung, V. Chan, LSI Logic Corporation, Fremont, California


A Study on the Yield Loss Due to Al(Cu) Interconnections with Spacing Failure............................117


R. L. Hwang, Y-S Huang, Y-L Wang, M-J Lee, Taiwan Semiconductor Manufacturing Company, HsinChu, Taiwan


Near IR Absorption in Heavily Doped Silicon – An Empirical Approach...........................................121


R. A. Falk, OptoMetrix, Inc., Renton, Washington


Embedded SRAM Bitmapping and Failure Analysis for Manufacturing Yield Improvement ..........129


J-Y Glacet, F. Lee, Motorola, Inc., Chandler, Arizona


LSI Process Diagnosis for High Reliability Usage...............................................................................137


M. Imai, D. Tanaka, K. Hosoda, K. Noda, Oki Engineering Company, Ltd., Minato-ku, Tokyo, Japan; S.


Matsuda, NASDA, Tsukuba-shi, Ibaraki, Japan


Application of KOH Electrochemical Etch and Passive Voltage Contrast Techniques


for Deep Sub-Micron CMOS Leaky Gate Detection .............................................................................141


F. Y. Chang, V. Chan, LSI Logic, Fremont, California


UV Reflectance Spectroscopy of the Copper/Copper Oxide System


for Assessment of Solderability ............................................................................................................147


L. S. Forney, C. Thierolf, B. Toleno, G. Parks, American Competitiveness Institute, Philadelphia,Pennsylvania


xvii


Session 5: Backside 1


Antireflection Coatings for Semiconductor Failure Analysis .............................................................155


B. V. Davis, Advanced Micro Devices, Inc., Austin, Texas; W. Chi, Advanced Micro Devices, Inc.,Sunnyvale, California


Comparative Study of Sample Preparation Techniques for Backside Analysis...............................161


P. Perdu, R. Desplats, F. Beaudoin, Centre National d'Etudes Spatiales, Toulouse, France


A Comparison of Backside Emission Microscopy Systems...............................................................173


B. V. Davis, Advanced Micro Devices, Inc., Austin, Texas


Failure Analysis from the Backside of a Die.........................................................................................177


S. Liebert, Philips Semiconductors, Zurich, Switzerland


Session 6: EOS/ESD


ESD Effects on Electromigration Performance of Aluminum Metallization Systems ......................189


J. E. Vinson, M. J. Dion, Intersil Corporation, Melbourne, Florida


Evaluation of On-Chip ESD Supply Clamp Robustness


by In-Situ Floating Power Bus Monitoring............................................................................................195


M. Fliesler, I. H. Morgan, Advanced Micro Devices, Inc., Sunnyvale, California


Transmission Line Pulse Testing of the ESD Protection Structures in ICs –


A Failure Analyst’s Perspective.............................................................................................................203


L. G. Henry, ESD/TLP Consultant, Fremont, California; J. Barth, J. Richner, Barth Electronics, Inc.,Boulder City, Nevada; K. Verhaege, Sarnoff Corporation, Princeton, New Jersey


Failure Analysis of CDM-ESD Damage in a GaAs RFIC ......................................................................215


A. Poe, S. Brockett, T. Rubalcava, TriQuint Semiconductor, Inc., Hillsboro, Oregon


Session 7: Techniques 1


A Focused Ion Beam Technique to Electrically Contact the Deep Trench Capacitor


of a Single Active Memory Cell in the Sub 0.25µm Technology Regime...........................................225


G. Zimmermann, Infineon Technologies AG, Munich, Germany; M. Johnston, R. Christ, White Oak Semiconductor, Sandston, Virginia


The Use of TMAH to Etch Silicon and Expose Metal Bridging Failures ............................................231


M. L. Morris, J. Mohr, E. Ortiz, S. Englebretson, ON Semiconductor, Phoenix, Arizona


Selective Au Etching in Au/Al Bonds in Current IC Technology........................................................235


M. Vanzi, A. Serpe, E. F. Trogu, P. De Plano, University of Cagliari, Cagliari, Italy; C. Hartfield, W.


Subido, Texas Instruments, Dallas, Texas


A Novel Method to Analyze the Deep Trench Capacitors in DRAM ...................................................241


J. Lee, K-H Huang, J-L Lue, ProMOS Technologies, Inc., Hsinchu, Taiwan


xviii


Session 8: Case Histories 1


Identification and Analysis of Parasitic Depletion Mode Leakage


in a Memory Select Transistor ...............................................................................................................247


J. B. Colvin, A. Roy, WSI, Fremont, California


Thermal Fatigue Induced Voiding in LDMOS Transistors Submitted


to Multiple Energy Discharges...............................................................................................................255


I. Percheron-Garcon, J-M Bosc, C. Levade, M. Cabie, Motorola, Toulouse, France; G. Vanderschaeve,CEMES-CNRS, Toulouse, France


Humidity-Bias Driven Shorts in Multilayer Circuits: A Case Study in Failure Analysis .................263


H. H. Jen, G. D’Urso, H. Andrews, M/A-Com, Inc., Lowell, Massachusetts


Passivation Cracks in a Four-Level Metal Low-K Dielectric Backend Process................................267


M. C. Olewine, J. F. DiGregorio, G. J. Colovos, K. F. Saiz, H. Sun, Philips Semiconductors,Albuquerque, New Mexico


Session 9: Packaging 2


Electronic Package Failure Analysis Using TDR .................................................................................277


D. A. Smolyansky, TDA Systems, Inc., Portland, Oregon


Time Domain Reflectometry as a Device Packaging Level Failure Analysis


and Failure Localization Tool.................................................................................................................285


D. T. Searls, Intel, Hillsboro, Oregon; A. Don, Intel, Penang, Malaysia; E. Dy, Intel, Cavite, Philippines;D. Goyal, Intel, Chandler, Arizona


Contrast Inversions in Scanning Acoustic Microscopy (C-SAM) of Glue Die-Attach......................293


B. Plikat, Infineon Technologies AG, Munich, Germany


Application of Scanning Acoustic Microscopy to Electric and Electronic Parts .............................303


C. Miyasaka, B. R. Tittman, The Pennsylvania State University, University Park, Pennsylvania


Session 10: Case Histories 2


Combining FIB Sequential Cross-Sectioning with TEM for Small Defect Analysis


in SRAM Array .........................................................................................................................................309


N. Wang, R. Fang, Cypress Semiconductor, San Jose, California


Failure Analysis of Tungsten Stud Defect from the CMP Process ....................................................315


K. Takagi, Y. Kohno, ITES Company, Ltd., Yasu-gun, Siga-ken, Japan; S. Nukii, IBM Japan, Ltd.,Yasu-cho, Shiga-ken, Japan


Integrated Circuit SNR Improvement Using Dielectric Altering Compound, Laser Trim


and FIB System........................................................................................................................................323


B. J. Dutt, J. J. Kroutch Jr., K. N. Hooghan, R. J. Jenkins, M. J. Toth, Lucent Technologies, Allentown,Pennsylvania


Characterization and Isolation Techniques in Silicon


on Insulator Technology Microprocessor Designs .............................................................................327


T. Kane, M. Cambra, M. Tenney, P. McGinnis, A. Domenicucci, Y. Wang, D. Falcon, IBM Advanced Semiconductor Technology Center, Hopewell Junction, New York


xix


Session 11: Packaging 3


Failure Analysis of Stacked-Chip Scale Package ................................................................................333


C. C. Flores, Intel Technology Philippines, Inc., Trias, Cavite, Philippines


Reducing Top-of-Die Plastic Delamination by Assuring Pre-Mold Cleanliness


of Die Surfaces ........................................................................................................................................339


R. K. Lowry, J. H. Linn, A. L. Northen, J. R. Zalnoski, H. W. Satterfield, Intersil Corporation,Melbourne, Florida


SMT Ceramic Capacitor Failure Mechanisms, Isolation Tools, Techniques


and Analysis Methods.............................................................................................................................347


R. A. Carbone, D. J. Roche, Hewlett-Packard, Roseville, California


Case Studies of Brittle Interfacial Failures in Area Array Solder Interconnects ..............................355


G. M. Wenger, R. J. Coyle, P. P. Solan, J. K. Dorey, Lucent Technologies, Princeton, New Jersey; C.


V. Dodd, Lucent Technologies, Oklahoma City, Oklahoma; A. Primavera, Universal Instruments


Corporation, Binghamton, New York; R. Erich, Amkor Technology, Chandler, Arizona


Session 12: Case Histories 3


Failure Analysis and Elimination of Galvanic Corrosion on Bondpads During Wafer Sawing.......369


Y. N. Hua, E. C. Low, L. H. An, S. Redkar, Chartered Semiconductor Manufacturing, Ltd., Singapore


High Temperature Solder (Au/Sn) Failures from Nickel Plating Impurities.......................................373


C. B. Bunis, M/A-COM, Inc., Lowell, Massachusetts


Semiconductor Wear Out at Nuclear Power Plants .............................................................................377


J. B. Riddle, Southern California Edison Company, San Clemente, California


UTC Clinic Hospital Network: Description of International Network of Failure Analysis Labs


and Case Studies.....................................................................................................................................385


T. C. Wilkins, Otis Elevator Company, Farmington, Connecticut


Session 13: FIB


Wafer Conserving Full Range Construction Analysis for IC Fabrication and Process Development


Based on FIB/Dual Beam Inline Application.........................................................................................393


R. Weiland, C. Boit, B. Ebersberger, P. Meis, Infineon Technologies AG, Munich, Germany; N. Dawes,A. Dziesiaty, H. Zimmermann, fei Company, Hillsboro, Oregon; E. Demm, A. Hirsch, Infineon


Technologies Corporation, Hopewell Junction, New York; L. Frey, C. Lehrer, Institut für Integrierte


Schaltungen, Erlangen, Germany; S. Geyer, M. Kamolz, H. Rettenmaier, W. Tittes, Infineon Dresden GmbH, Dresden, Germany; H. Lezec, Université Louis Pasteur, Strasbourg, France; R. Treichler,


Siemens AG, Munich, Germany


Focused Ion Beam Analysis of Low-K Dielectrics...............................................................................397


H. J. Bender, R. A. Donaton, IMEC, Leuven, Belgium


Automatic Determination of Optimal FIB Operations for Improved Circuit Probing


and Fast Reconfiguration .......................................................................................................................407


R. Desplats, T. Dargnies, J-C Courrege, P. Perdu, Centre National d'Etudes Spatiales, Toulouse,France; J-L Noullet, AIME, Toulouse, France


Specific Area Planar and Cross-Sectional Lift-Out Techniques: Procedures


and Novel Applications...........................................................................................................................415


R. S. Rai, S. Subramanian, S. Rose, J. Conner, P. Schani, J. Moss, Motorola, Inc., Austin, Texas


xx


Session 14: Discretes


EOS Simulation and Failure Analysis of Metallurgically Bonded Silicon Diodes ............................425


A. Teverovsky, Unisys/Goddard Operations, Lanham, Maryland


Temperature Distributions in III-V and SiC Micro-Wave Power Transistors Using


Spatially Resolved Photoluminescence and Raman-Spectrometry Mapping Respectively ...........435


P. Martin, Escuela Técnica Superior de Ingenieros Industriales, Paseo del Cauce, Valladolid, Spain;R. Bisaro, C. Dua, O. Noblanc, S. L. Delage, D. Floriot, F. Lemaire, P. Galtier, J. P. Landesman, C.


Brylinski, Thomson-CSF, Orsay, France


Failure Analysis of a Transistor Lead ...................................................................................................443


Y. Deguchi, S. Matsuda, J. Aoki, NASDA, Tsukuba-shi, Ibaraki, Japan; T. Tamura, NASDA, Minato-ku,Tokyo, Japan; Y. Iwai, S. Kikui, Oki Engineering Corporation, Minato-ku, Tokyo, Japan


Liquid Metal Embrittlement of Copper Wires .......................................................................................449


L. E. Brown, ITT Aerospace/Communications, Fort Wayne, Indiana


Session 15: Techniques 2


Planar TEM Analysis of Nanoindented Samples Using the


Focused Ion Beam Lift-Out Technique .................................................................................................459


T. L. Shofner, S. R. Brown, B. B. Rossie, M. A. Decker, Y. S. Obeng, F. A. Stevie, Lucent Technologies, Orlando, Florida; J. L. Drown, The Bartech Group, Orlando, Florida


Computerized Quantification of the Dicing Process:


The First Step Toward Related Die Cracking Failure Analysis...........................................................463


D. Glover, J. R. Lynch, I. Huseby, ON Semiconductor, Phoenix, Arizona


Automatic IC Die Positioning in the SEM..............................................................................................469


H. W. Tan, J. C. H. Phang, J. T. L. Thong, National University of Singapore, Singapore


Integrated Circuit Waveform Probing Using Optical Phase Shift Detection .....................................479


K. Wilsher, W. K. Lo, Schlumberger Technologies, San Jose, California; T. M. Eiles, Intel Corporation,Santa Clara, California; G. Xiao, Checkpoint Technologies, San Jose, California


Session 16: Case Histories 4


Failure Analysis of MEMS Using Thermally-Induced Voltage Alteration ..........................................489


J. A. Walraven, E. I. Cole, Jr., P. Tangyunyong, Sandia National Laboratories, Albuquerque, New Mexico


Application of TIVA in Design Debug....................................................................................................497


S. Kolachina, B. Taylor, K. S. Wills, Texas Instruments, Inc., Stafford, Texas; E. I. Cole, Jr., Sandia National Laboratories, Albuquerque, New Mexico


Backside Fault Isolation Using a Magnetic Field Imaging System on SRAMs


with Indirect Shorts .................................................................................................................................503


L. A. Knauss, B. M. Frazier, A. B. Cawthorne, Neocera, Inc., Beltsville, Maryland; E. Budiarto, R.


Crandall, S. Melnik, C. Bennett, Intel Corporation, Hillsboro, Oregon


xxi


Session 17: SPM


Local Electrical Thickness-Mapping of Thin Oxides


with Conducting Atomic Force Microscopy .........................................................................................511


A. Olbrich, B. Ebersberger, C. Boit, Infineon Technologies AG, Munich, Germany


Guidelines for Two-Dimensional Dopant Profiling Using Scanning Capacitance Microscopy ......521


A. Born, R. Wiesendanger, University of Hamburg, Hamburg, Germany


pn Junction Delineation in Si Devices Using Scanning Capacitance Spectroscopy.......................529


H. Edwards, Texas Instruments, Inc., Dallas, Texas


Contactless Voltage and Current Contrast Imaging


with Scanning Force Microscope Based Test Systems......................................................................533


W. Mertin, S-W Bae, U. Behnke, R. Weber, E. Kubalek, Gerhard-Mercator-University of Duisburg,Duisburg, Germany


Session 18: Backside 2


Transparent Heat Spreader for Backside Optical Analysis


of High Power GHz-Scale Microprocessors .........................................................................................547


T. M. Eiles, Intel Corporation, Santa Clara, California; D. Hunt, D. Chi, Schlumberger Probe Systems,San Jose, California


New Laser Ablation Method for Non-Destructive Backside Sample Preparation.............................553


F. Beaudoin, P. Perdu, Centre National d'Etudes Spatiales, Toulouse, France; F. Saviot, ThomsonCSF Laser, Talence, France; D. Lewis, F. Salin, Université Bordeaux 1, Talence, France


Silicon Trenching Using Dry Etch Process for Backside FIB and Probing.......................................559


V. Korchnoi, A. Fenigstein, A. Barger, Intel Israel, Ltd., Haifa, Israel


Application of Near IR, Phase-Contrast Imaging to Backside Failure Isolation and Analysis........567


R. A. Falk, OptoMetrix, Inc., Renton, Washington; E. W. Budiarto, Intel Corporation, Hillsboro, Oregon


Copyright © 2000 ASM International®


p 3-8


All rights reserved.


DOI: 10.1361/cp2000istfa003


www.asminternational.org


Proceeding from the 26thInternational Symposium for Testing and Failure Analysis, 12-16 November, 2000, Bellevue, Washington


Laser Voltage Probe (LVP): A Novel Optical Probing Technology for Flip-Chip Packaged Microprocessors


Wai Mun Yee, Mario Paniccia*, Travis Eiles*, Valluri Rao*


Intel Technology Sdn. Bhd, Malaysia ;


* Intel Corporation, Santa Clara, CA, USA.


Abstract


A novel optical probing technique to measure voltage waveforms from flip-chip packaged complementary metal-oxide-semiconductor (CMOS) integrated circuits (IC) is described. This infrared (IR) laser based technique allows signal waveform acquisition and high frequency timing measurement directly from active PN junctions through the silicon backside substrate on IC’s mounted in flip-chip stand-alone or multi-chip module packages as well as wire-bond packages on which the chip backside is accessible. The technique significantly improves silicon debug & failure analysis(FA) through-put time (TPT) as compared to backside electron-beam (E-beam) probing because of the elimination of backside trenching and probe hole generation operations.


Introduction


As CMOS microprocessor core clock frequencies move beyond 500MHz, there is a growing industry wide interest in the use of flip-chip packaging for these microprocessors. With this migration to flip chip packaging technology, existing techniques for obtaining time resolved waveforms using conventional E-beam probing of metal interconnects from the front side of the chip become obsolete.


With the front-side of the chip inaccessible, electrical measurements of internal nodes can only be obtained from the backside of the chip.


In Ref.[1] a novel method for accessing nodes and measuring signals from the silicon backside is described. This method involves etching trenches and generating precision Focused Ion Beam (FIB) probe holes in the silicon backside substrate to provide direct line-of-sight to metal interconnects for E-beam probing from the backside of the chip. This probe hole generation sample preparation process is timeconsuming and significantly increases the measurement throughput time.


In this paper, we describe a novel infrared (IR)optical probing approach which provides fast and direct access to diffusion (P-N junction) nodes directly through the silicon substrate. Since extrinsic silicon is partially transparent to IR light, an IR laser beam at a wavelength of 1064nm can be focused through the silicon substrate onto a P-N junction in a flip-chip packaged CMOS IC. The small optoelectronic interactions that occur between the focused IR laser beam and the semiconductor P-N junction can be measured stroboscopically to determine the voltage waveform at that internal signal node. The equipment based on this IR probing principle


has been internally named the


Laser Voltage Probe (LVP).


The LVP is a novel IR probing technology that provides a way to measure voltage waveforms directly from P-N junctions through the backside of a silicon substrate. These measurements can be made on flip-chip mounted IC's in stand-alone, multi-chip modules (MCM) or any other package type for which the chip backside is accessible and the silicon substrate can be thinned. This paper discusses the fundamental principles on which the operation of the LVP is based, describes results obtained from an experimental LVP set up and finally conclude with timing waveforms measured from microprocessors operating at full speed during silicon debug and failure analysis, using a production LVP system.


Principles of Operation


The fundamental operation of the LVP is based upon two principles. First, heavily doped silicon is partially transparent to IR light with sub-band-gap photon energies. Second, there are a number of optoelectronic interactions that occur in a semiconductor P-N junction when an optical beam is focused onto the junction. These mechanisms include electroabsorption (also known as the Franz-Keldysh effect),electro-refraction, and free carrier effects including absorption and refractive index changes (plasmaoptical effect) Ref. [2]-[7].


We will first discuss the relationship between photon energy (or wavelength) relative to the silicon band gap energy (~1.1eV). Silicon is completely opaque when light with photon energy greater than the silicon band-gap energy is incident on it. This is due to the fundamental absorption of light (electron-hole pair generation). On the other hand, intrinsic silicon is transparent (non-absorptive) to IR light with photon energy smaller than the silicon band-gap energy. However, when the silicon is heavily doped(as with current advanced CMOS IC fabrication process technologies), free carrier absorption (which is proportional to the square of wavelength, •2) is significant at photon energies below that of the silicon band-gap (Ref.[2]). The combined effects of the fundamental absorption above the band-gap energy and absorption due to free carriers below the band-gap energy give rise to the silicon transmission curves for heavily doped silicon as shown in Fig.1. It is apparent from Fig.1 that thinning the silicon substrate can dramatically increase the transmission(see curves B & C in Fig.1). The result of this partial


inFraction changeal


transmission of IR light through doped silicon allows an IR laser beam to pass directly through a thinned silicon substrate and to be focused onto the active PN junctions (diffusions) of an IC.


A : Intrinsic Si


700μm thick


C : DopedSi, 700μm


B : Doped Si, 200μm


100


0


20 40 60


% Transmission80


1 1.4 1.8 2.2 2.6 3


Wavelength ( μm)A


C B


E =hcλ


Figure 1 Transmission curves for undoped (A) and heavily doped (B & C) P+ silicon substrates as a function of wavelength.


There are a number of opto-electronic processes that occur in a P-N junction in the presence of incident photons. It has been shown (Ref.[2] & [3]) that in the presence of a very high electric field (> 104V/cm),tunnelling states are created in the forbidden energy gap near the edges of the conduction band and the valence band of a semiconductor. These tunnelling states effectively reduce the band-gap energy of the semiconductor. This phenomenon is referred to as the Franz-Keldysh (F-K) effect. The F-K effect causes an increase in the absorption of incident photons with energies near the semiconductor band-gap in the presence of an electric field in a P-N junction. This opto-electronic mechanism is known as the electroabsorption or photon-assisted tunnelling.


In conjunction with electro-absorption, there also exists electro-refraction. Soref and Bennett (Ref.[5])described in detail how through the Kramers-Kronig


relationship, electro-absorption and electro-refraction are related. In addition to the electro-absorption and the electrorefraction phenomena (arising from the presence of an electric field across a depletion region), there are also free carrier effects, which include free carrier absorption and carrier-induced refractive index change. Since all these effects occur simultaneously in a P-N junction, experiments were conducted to determine the relative magnitude of these effects and from the results, develop an optical probing technology that will work with our current CMOS IC processes.


0.0E+00


5.0E-06


1.0E-05


absorption1.5E-05


2.0E-05


2.5E-05


1.035 1.055 1.075 1.095 1.115


Wavelength (μm)


room temp


100 oC


Figure 2 Measured electro-absorption on heavily doped p+ silicon substrate as a function of


wavelength and temperature.


Experimental Results


The Franz-Keldysh effect has been measured experimentally both for intrinsic and slightly doped silicon (Ref. [3,4,5,7]). In order to understand the magnitude of electro-absorption in highly doped P+silicon substrates (as used in today’s CMOS process),measurements were performed on the electroabsorption of highly doped silicon in the presence of a high electric field. Fig.2 shows the measured fractional change in absorption in heavily doped silicon in the presence of an applied electric field of


1.25×105 V/cm at both room temperature and at 100oC. From the figure, we see that the peak electroabsorption occurs at a wavelength of ~1.065μm and the electro-absorption effect resides over a narrow wavelength band of ~50nm. Figure2 also shows that the electro-absorption peak is red-shifted (to longer wavelengths) at higher temperatures. This is as expected because the silicon fundamental band-gap energy decreases with an increase in temperature and this compares well with data presented in Sze (Ref.


[6]).


With the electro-absorption peak determined, a laboratory LVP system was set up to study the feasibility of utilising this mechanism to effect a novel optical probing tool. A simple schematic of the laboratory set up of the LVP is illustrated in Figure 3.


Mode Locked Laser 100MHz, 1.064μm,


~30ps pulse width


Laser sampling pulses


Silicon IC


Collimating


Lens


Faraday Rotator


IR Objective Lens


Polarizing


Beam


Splitter


Photodiodes


To Detection Electronics


Figure 3 Simple schematic diagram of the laboratory LVP set-up.


The LVP is composed of a mode-locked lser that operates at a wavelength of 1064nm and outputs pulses at 100MHz repetition rate. The laser probe beam is focused through the backside of a fully packaged IC and onto the a N+ diffusion, which is nested on a p-well, thus forming a P-N junction. The probe beam passes through the P-N junction region,reflects off the metal contact, travels back out of the silicon surface. The reflected beam is then directed by means of an optical beam splitter onto an optical detection system that converts it into an electrical signal for signal processing. When a time varying signal is applied to the diode so as to reverse-bias the P-N junction alternately, the high electric field across the junction (~105V/cm) causes a small intensity modulation in the reflected laser light due to electroabsorption and free-carrier effects. This optical intensity modulation can then be demodulated and converted into a voltage waveform, which exactly correlates to the input voltage signal applied to the PN junction.


In conjunction with the electro-absorption mechanism, there also exist free carrier effects in the P-N junction, all of which also vary with the applied voltage. The principal free carrier effect that takes place is the free carrier absorption. Experiments were conducted to determine the relative magnitude of electro-absorption and free carrier absorption to assess their contribution in the voltage probing technology. In order to distinguish the two effects,optical absorption modulation measurements were carried out on a reverse-biased P-N junction at low laser power and at two different probing laser wavelengths of 1064nm and 1300nm, respectively.


Results showed that the absorption modulation signal is much smaller (~6X at 2V bias) at 1300nm as compared to 1064nm probing wavelength. As shown previously in Fig.2, electro-absorption is limited to a very narrow wavelength region (~50nm) centred around 1065nm and is very small at 1300nm. In addition, it was also stated in section 2 that free carrier absorption is approximately proportional to λ2.


It should then be expected that the free carrier absorption at 1064nm would be smaller than that at 1300nm. However, since the present measured


absorption signal at 1064nm is larger, it may be concluded that at this wavelength, for the presently considered CMOS process, and at low laser power,the dominant absorption mechanism responsible for the optical modulation signal from a reverse-biased P-N junction is electro-absorption.


Experiments were conducted to measure the magnitude of the optical absorption modulation depth(LVP signal) as a function of the reverse-bias voltage applied to the P-N junction. The result is shown in Fig.4, which shows that the LVP signal is directly proportional to the applied voltage across the P-N junction at various incident powers, for the CMOS IC technology used in this experiment.


0 20 40 60 80 100 120 140 160 180 200


1


1.5


2


2.5


3


Applied Voltage, Vin (Volts)


Pd = 0.25 mW P = 0.50 mW P = 1.0 mW


Figure 4 Measured LVP signal in a P-N junction as a function of applied reverse-bias voltage across the junction for different incident optical power.


Another factor to consider in utilising the LVP for probing internal nodes of an IC is that of cross-talk that may arise when probing two closely spaced diffusions. The full-width-half-maximum (FWHM)beam diameter of the focused laser spot is estimated to be ~0.7μm. A periodic structure of diffusion areas forming a P-N junction as shown in Figure 5 was used to measure the level of cross-talk. This was done by measuring the LVP signal at each incremental spatial distance while the optical probe beam was scanned across the diffusion structure. The resulting spatial variation of the LVP signal along the scanning axis is also showed in Figure 5. Since the LVP signal is only dependent of the opto-electronic interactions that occur at the P-N junction interface,one would expect to obtain LVP signal only when the laser beam is focused onto the junction area. Crosstalk would only be limited to the overlap of the Gaussian beam tail to the neighbouring diffusion.


This is what has been observed in Figure 5 and that cross-talk is minimum as long as the diffusion structures are spaced approximately greater than a distance of a FWHM of the laser spot diameter.


LVP Signal versus Distance along x-axis


0.5)(uV Signal LVP1


1.5 2


2.5 3


3.5 4


4.5 5


0 1 2 3 4 5 6 7 8 9


Distance along x-axis (μm)


n+ diffusion in p-well


p+ diffusion


scanning x-axis


|1-6||||||
|---|---|---|---|---|---|

|||||||

Figure 5 Experiment to determine the level of crosstalk. LVP signal is measured as a function of probe beam position as the laser spot is scanned across the


diffusion fingers of a P-N junction.


Repetitive Waveform (looping)


time


T0


2T0+δT


3T0+2δT 4T0+3δT


t


Laser sampling pulses (Δt=35ps)


Δt


V


Reconstructed waveform


Figure 6 Schematic diagram showing the principles of stroboscopic sampling.


Time Resolved Voltage Measurements


The discussion so far has been focused on the optical mechanisms for sensing voltage variations in a P-N junction and performing measurements in a laboratory LVP set-up. In order in obtain useful timing information, one must incorporate sampling and synchronisation techniques between the tester and the probing equipment. Because the optoelectronic interactions that give rise to the LVP signal (absorption modulation) is very weak(estimated to be in the order of hundreds of parts-permillion), time resolved measurements must be performed stroboscopically as in E-beam probing.


Figure 6 illustrates the principles behind stroboscopic waveform measurement. In order to perform stroboscope sampling, the device under test (DUT) is exercised repetitively by looping the test patterns using a tester. The LVP is synchronised with the tester and the laser sampling pulses are slowly scanned through the waveform at every loop of the test pattern. The benefit of stroboscopic measurements is that a high measurement bandwidth is realised using a short sampling pulse (in this case the laser pulse width). If the pulse width is Δt, then


the measurement bandwidth (BW) is given by~0.36/Δt. The key to achieving very large measurement bandwidths (tens of Gigahertz) is to use very short laser pulses. As stated previously the current LVP uses a mode-locked laser that operates with a repetition rate of 100MHz, has a pulse width of ~35ps and jitter of <10ps. Thus the measurement bandwidth of ~12GHz is obtained using the current mode-locked laser set-up. As IR solid-state laser technology continues to improve, pushing the minimum pulse widths down to sub-picoseconds,future optical probing bandwidth > 50GHz may be achieved.


With the laboratory LVP set-up, clock waveforms were successfully acquired from current advanced CMOS IC’s. With experimental data supporting the feasibility of realising a novel optical probing technology and with all enabling technologies in


Voltager√r


place, a production LVP system was constructed. The production LVP system has been used to acquire time resolved voltage waveforms from internal nodes of advanced CMOS IC’s running at core frequencies greater than 300MHz during silicon debug and failure analysis. We will illustrate some internal signal waveforms obtained with the LVP.


Silicon Debug and FA Waveform Measurements


During the design debug of a new product, waveform measurements from internal nodes of a chip are usually required to aid in the determination of the cause of speed related failures that are caused by circuit or process sensitivities. In IC failure analysis(FA), it is often necessary to probe internal nodes to obtain the logic transitions so as to verify the functionality and to isolate electrical faults of the IC.


The LVP allows backside imaging and voltage waveform measurement from active diffusion areas directly through the silicon backside substrate without the need to open probe holes from the IC silicon backside. The LVP finds numerous debug and FA applications such as electrical node fault isolation, timing delay and rise/fall time measurements.


Figure 7 shows a backside IR image of an advanced CMOS microprocessor acquired through a silicon substrate using the LVP. The ability to image through the silicon substrate eliminates the need to open probe holes and also presents an opportunity for probing any diffusion node, thus improving the signal accessibility coverage for silicon debug and FA applications.


pMOS


transistors


5


nMOS


transistors well tab


div500 ppm/


20 μm


Figure 7 Backside IR image of a CMOS IC showing transistor devices at silicon level. Image acquired using the LVP laser scanning microscope.


Figure 8 shows two waveforms obtained with both the E-beam and the LVP, respectively, at comparable pulse widths and loop lengths. The E-beam pulse width used was 50ps and the waveform was taken from metal interconnects on the front side of the chip.


The LVP system uses a laser pulse width of 35ps and the waveform was acquired through the silicon backside at a P-N junction. As can be seen from Figure 8, both the waveforms from the LVP and the E-Beam are very similar and comparable in terms of S/N ratio.


LVP Waveforms


me(35ps laser sampling pulse)


VM


E-Beam Waveforms


hu(50ps e-beam sampling pulse)


Figure 8 Comparison of LVP and E-Beampp200/divm waveforms for similar probe pulse widths.


Figure 9 shows a set of LVP waveforms acquired


from internal signal nodes of an advanced CMOS


microprocessor at both passing and failing test


conditions. It is noted that signal out[6] exhibited


excessive delay when the sample was exercised in the


failing condition while no such delay was observed in


signal out[0]. It is also noted from Figure 9 that the


out[0] signal has a faster rising edge as compared to


the input signal in[0]. This is because out[0] is a


latched signal that has been regenerated by a driver


while the input signal has been degraded in


propagating along a resistive and capacitive line. We


have thus successfully demonstrated the LVP’s


usefulness in identifying the internal signal node with


the timing related failure (that is signal out[6] in this


example) in a CMOS microprocessors during speed


path debug and failure analysis.


clk passing


clk failing


in[6] passing in[6] failing


out[6] passing out[6] failing


in[0] passing in[0] failing


out[0] passing


out[0] failing


1ns/div


Figure 9 Internal signal waveforms acquired using the LVP from a CMOS IC showing the timing


measurement capability of the LVP.


signal_A


signal_B


signal_C


signal_D


signal_E


10 ns


Figure 10 Additional internal signal waveforms acquired from a flip-chip packaged CMOS


microprocessor using the LVP.


Figure 10 shows additional LVP waveforms taken from a flip-chip packaged advanced microprocessor during FA to isolate the logically faulty node. These acquired logic transition waveforms were compared to simulated results to verify the functionality and to pin-point the electrical faulty node during failure analysis. The LVP has been used successfully in failure analysis to isolate faulty signal nodes in advanced CMOS IC’s.


Summary


We have presented in this paper the basic operation and fundamentals of a novel optical probing technology called the LVP. The LVP can be used to acquire timing waveforms on flip-chip packaged IC’s directly through the silicon backside. The key advantage of the LVP as compared to backside Ebeam probing is the dramatic reduction in debug/FA TPT which ensues due to the elimination of the backside trenching and probe hole generation processes. Time-resolved waveforms acquired from internal signal nodes using the LVP on advanced CMOS microprocessors during FA and silicon debug are also presented. These waveforms demonstrated the ability of the LVP to help in identifying and resolving speed, timing or functionality related failures during silicon debug and FA.


The LVP also has a higher measurement bandwidth(BW~12GHz today) using 35ps pulse width modelocked laser as compared to E-beam probing. This BW can be upgraded to > 50GHz in future allowing the LVP technology to scale with future high frequency (>GHz) microprocessors. The LVP technology is new and will continue to improve as this optical probing technology matures. One additional benefit of the LVP is that it operates in air as opposed to E-beam technology which requires a vacuum system. This feature opens up the possibility of probing fully packaged devices with large form factors such as the multi-chip module.


Acknowledgements


The authors would like to thank Gary Woods and Yi Ding for helpful discussions. Special thanks go to Loren Eyres at Stanford University for making the electro-absorption measurements. Neither expressed nor implied licenses under any intellectual property belonging to Intel Corporation are provided by the contents or publication of this document.


References


1. Livengood et. al., “Focused Ion Beam Techniques for Debug of Flip-Chip Integrated Circuits”, Semiconductor International , March


1998.


2. Jacques I. Pankove, “Optical Processes in Semiconductors”, Dover Publications, Inc. New York, 1971.


3. Marvin Chester and Paul H. Wendland, “ElectroAbsorption Spectrum in Silicon”, Physical Review Lett., Vol.13, pp.193, 1964.


4. G. Koskowich and Mani, “Optical Charge Modulation as an Internal Voltage Probe for CMOS IC’s”, IEEE Journal of Quantum Electronics, Vol.24, pp.1981, 1988.


5. Richard Soref and Brian Bennett, “Electrooptical Effects in Silicon”, IEEE Journal of Quantum Electronics, Vol.QE-23, pp.123, 1987.


6. S.M. Sze, “Physics of Semiconductor Devices”,John Wiley & Sons, 1981.


7. H.K. Heinrich et al, “Measurement of Real Time Digital Signals in a Silicon Bipolar Junction Transistor using a Noninvasive Optical Probe”,Electron Lett. Vol.22, pp. 650.


p 11-16


DOI: 10.1361/cp2000istfa011


Scanning Electron Acoustic Microscopy:


A Novel Tool for Failure Analysis & Microcharacterisation


WK Wong, QR Yin*, JTL Thong+, JCH Phang+, JW Fang*


Institute of Materials Research and Engineering (IMRE), Singapore


*Shanghai Institute of Ceramics Chinese Academy of Sciences (SICCAS), Shanghai, China+Centre for IC Failure Analysis and Reliability (CICFAR) Faculty of Engineering


National University of Singapore


This paper describes Scanning Electron Acoustic Microscopy (SEAM) applications, particularly to samples that are of interest to the microelectronics industry. Several applications of SEAM involving semiconductor and ferroelectric samples are discussed in this paper. The expanding scope of applications for SEAM presents exciting possibilities.


The challenge ahead lies in understanding the contrast mechanisms in SEAM signal formation as well as correlating results to the physical properties of samples.


Historical Background


Since the Scanning Electron Acoustic Microscopy(SEAM) technique was first studied in 1980 (Brandis and Rosencwaig, 1980; Cargill, 1980), numerous work has taken place to study and understand the properties of this technique. Significant work include the exploration of non-linear SEAM operating modes (Balk and Kultscher, 1983a), the use of very short electron pulses which allows timeresolved SEAM imaging with high temporal resolution up to GHz frequencies (Balk and Kultscher, 1984) and depth profiling using phase shift detection (Marty-Dessus and Franceschi, 1993).


Applications studied to date include fields as diverse as defects in metals (Shaw et al., 1994), ferroelectric materials (Liu et al., 1998), ceramics (Liao et al.,1999) and semiconductors such as Si (Domnik and Balk, 1993) and GaAs (Kaufmann, et al., 1994).


SEAM has remained very much a research curiosity until very recently when the first commerciallyviable system was developed, in particular the SEAM 100 system which is used in the current SEAM work at IMRE.


SEAM Theory


SEAM is based on the detection of electron acoustic(EA) signals that are generated as a result of the heating effect of a pulsed electron beam on a sample.


The energy conversion of the high energy electrons from kinetic to thermal energy due to inelastic scattering of the electrons within the sample forms the basis for the thermal wave mechanism proposed to explain SEAM contrast formation (Opsal and Rosencwaig, 1982). The key parameter in this model is the thermal diffusion length μ, which has a frequency dependence described by the following equation:


(


) 2/1


/


ϖ


ρ


μ


C


K


=


(1)where K is the thermal conductivity of the material, ρ is the density of the material, C is the specific heat and ω is the angular modulation frequency.


Examples of μ for some common materials and operating frequencies are given in Table 1.


Table 1 Example of thermal diffusion


lengths for materials


|(μm) Material |Thermal Diffusion length, μ |Thermal Diffusion length, μ |
|---|---|---|

|(μm) Material |@ 50 kHz |@ 1 MHz |

|Silicon |53.7 |12.0 |

|Organic coating |4.5 |1.0 |

|Aluminium |13.4 |3.0 |

Beyond the thermal diffusion length, most of the thermal wave is converted into acoustic energy which propagate through the sample. As the wavelength of the acoustic wave is comparable to the dimension of a typical sample, the acoustic wave itself would only serve as a vector to the SEAM signal and would not contribute any meaningful SEAM contrast to the signal. However, acoustic transmission and reflection effects may introduce changes to the acoustic signal, for example the choice of materials for the SEAM detector housing.


The thermal wave diffusion model described above provides a comprehensive description of SEAM signal behaviour in a sample where only the energy transfer due to inelastic electron-sample scattering mechanism occurs, e.g. in metals such as Al (Ikoma,


et al., 1984). In other classes of samples, other mechanisms may also be present. For example, in semiconductors, excess carrier recombination leading to localised heat generation also contributes to the SEAM signal (Sablikov and Sandomirskii, 1983).


Furthermore, the existence of internally-generated space charges in semiconductors and dielectrics(Sasaki et al., 1986) leads to the additional mechanisms of local piezoelectricity and electrostriction (Kultscher and Balk, 1986). Other mechanisms include magnetostrictive or magnetoelastic interactions in ferromagnetic samples(Koirakh and Preobrazhenskii, 1984) and photostrictive mechanisms (Stearns and Kino, 1985).


Hence, these SEAM signal generation mechanisms must be accounted for in an in-depth analysis of SEAM contrast in semiconducting and ferroelectric samples.


The ideal excitation waveform for SEAM is an electron beam modulated to a perfect square wave.


The spectrum of such a waveform contains only the fundamental and the odd harmonics of the fundamental frequency. Assuming linear behaviour of the EA signal generation, this means that the resultant EA signal would also contain the fundamental and odd harmonics. However, it has been shown that non-linear EA signal generation mechanisms also exist leading to the formation of even harmonics (Balk and Kultscher, 1983b). The even harmonics may originate from hysteretic interaction between the thermal wave and the bulk material. These non-linear SEAM signals can result in images possessing significantly improved spatial resolution and contrast not obtainable in linear SEAM imaging, e.g. in Cu-Zn-Al alloys (Balk et al.,1984).


Experimental Setup


Figure 1 below shows the setup used for Electron Acoustic (EA) detection. The current experimental setup is built around the SEAM 100 system supplied by Scanning Beam Technology. As the EA signal is an ac-coupled signal generation mechanism, frontend excitation is accomplished by a chopped electron beam. High-speed beam chopping performance in the region of MHz frequencies can be achieved using electrostatic blanking with a pair of deflection plates and an aperture (Menzel and Kubalek, 1979). The deflection plates are driven by an analog driver with sufficient capacitive-drive capability. The design of the beam-blanking system is of particular importance in order to achieve a well-defined chopped electron beam with characteristics closely resembling the ideal square wave with only odd harmonics present.


Figure 1 Experimental setup for SEAM detection.


The EA signals propagating through the sample are picked up by a piezoelectric transducer mounted on the base of the sample. Common choices of the piezoelectric transducer include those composed of titanate compounds such as Lead Zirconate Titanate(PZT), Barium Titanate (BaTiO3) and PolyVinyl Dene Fluoride (PVDF). The piezoelectric transducer converts these acoustic signals into electrical signals that are subsequently processed for data acquisition.


However, the piezoelectric transducer may not be the only acoustic to electrical converter in a detection system as mentioned in the previous section. Also,consideration must be given to the mechanical interaction between the sample, transducer and housing in which the detector arrangement is contained.


The output of the piezoelectric transducer for EA detection has a typical amplitude in the order of microvolts even in the best cases. Hence, adequate screening and proper grounding of the system is imperative if reasonable signal quality is to be achieved. Further improvement can be obtained by the use of appropriate pre-amplification to reduce the relative effects of noise before the lock-in amplification stage. The output of the lock-in amplifier undergoes further processing by the SEAM Controller unit before it is relayed to the PC for digital acquisition, processing and storage. The PC also generates the scan signals for the x-y deflection coils of the SEM. The lock-in output is a 2-dimensional vector that is typically represented by the amplitude-phase (R-θ) or rectangular (X-Y) coordinates. The former has the advantage of presenting a phase-invariant derivative of the EA signal.


In the following section, examples of SEAM imaging that is relevant to microelectronics applications are presented.


SEAM Application Examples


(B)


The examples given here were generally obtained using a 25 kV electron beam with a typical current of about 1 μA. Unless explicitly stated, the results that are presented in this paper is of the amplitude-phase(R-θ) representation.


Imaging of Defects in Silicon-on-Insulator (SOI)


The sample is composed of Si and SiO2 layers fused together on a Si substrate. The thickness of the Si,


50 μm


SiO2 and Si substrate layers are approximately


0.6 μm, 0.6 μm and 350 μm respectively. The


(C)


sample was coated with a conductive gold layer to reduce sample charging which may distort the experimental results. The site marked 'a' in the Secondary Electron (SE) image of Figure 2(a) clearly shows a bulge in the topmost Si layer due to a defect in the underlying SiO2 layer. Figure 2(b) shows the cross-section at location x-x’ in Figure 2(a) where a large subsurface pit hole was located. The crosssection cut was performed after the SEAM images of


4


Figure 2(c) to 2(f) were obtained. Figures 2(c)through (f) reveal the contrast due to the subsurface hole as well as the bulge in the Si layer. In addition,


Tood r


the SEAM images reveal additional contrast in the


(D)


regions marked 2, 3 & 4 in Figure 2(c). The origin of the contrast for these areas is probably due to residual stress-strain built up by the sample assembly process as subsequent cross-sectional cuts taken of these zones did not reveal the presence of any subsurface holes or defects. The SEAM signal generation depth can be shown to be about 19, 14, 12 and 10 μm at 78,131, 191 and 236 kHz respectively (Fang and Yin,2000). At the highest frequency (236 kHz), no contrast could be obtained from regions 2, 3 and 4.


This indicates that the stress-strain region only starts from a depth of more than 10 μm from the sample


100 μm


surface. An improvement in the lateral resolution can also be qualitatively observed in the SEAM images


(E)


as the frequency increases, which is commensurate with the reduction in the SEAM signal depth.


(A)


Figure 2 Images of (a) SE image of Silicon-onInsulator (SOI) region; (b) SE image of cross-section containing sub-surface hole marked x-x’; Electron Acoustic (EA) images at (c) 78 kHz; (d) 131 kHz;


(e) 191kHz; (f) 236 kHz


Ferroelectric domains in barium Titanate(BaTiO3)


This example demonstrates the capability of SEAM


in profiling the domain structure in ferroelectric


samples such as BaTiO3. The SE image of a single-100 um crystal BaTiO3 sample in Figure 3(a) shows the usual


surface topography of the sample, while the SEAM


image is able to give information on the ferroelectric


domain orientation within the bulk of the sample as


shown in Figure 3(b). In addition, using different


frequencies can provide information on the


ferroelectric domains at different depths. Figs. 4(a)


and (b) gives an example of the subtle changes in the


ferroelectric domain orientations as the frequency is


increased from 98.9 kHz to 114.7 kHz for a polycrystalline BaTiO3 sample. This feature of SEAM is


particularly relevant to Ferroelectric RAM (FRAM)


metrology.


The sample is a Si test structure where selected


regions have been n-doped. The EA image in Figure


5(b) shows additional information on the doping


-100um


distribution on the sample that is not available in the conventional SE image in Figure 5(a). The primary contrast mechanism is the electrostriction mechanism mentioned previously due to the different doping levels in the Si material.


100μm


100 um


(a)


(b)


Figure 3 Images of Barium Titanate sample: (a)Typical SE image and; (b) EA Image of SingleCrystalline specimen at 210 kHz


--100um


Figure 4 EA images of poly-crystalline barium titanate sample at (a) 98.9 kHz and; (b) 114.7 kHz doped area profiling in silicon (Si) microstructures.


Figure 5 a) Secondary Electron (SE) Image; and (b)Electron Acoustic (EA) Image showing Doped Areas in Dark Contrast.


Imaging of Wirebond Region in IC


Figures 6(a) and (b) show an application of the SEAM technique for the imaging of subsurface layers in silicon-based semiconductor samples. The EA image on the right shows that EA contrast can be obtained from the wire bond and metallisation regions as shown by the high contrast regions in Figure 6(b). Lower-level contrast is also obtained from the subsurface metal 2 layer as shown in the extreme right-hand side of Figure 6(b). This metal 2 layer is not visible in the SE image in Figure 6(a).


Figure 6 (a) SE image; and (b) EA image at f=140 kHz for IC sample showing sublayering information.


Conclusions


The SEAM technique enables thermal-elastic analysis to be performed on relevant samples. This capability allows subsurface defect inspection and analysis to be performed and significantly extends the range of applications on the SEM beyond what is presently available. The recent availability of commercial systems promises broader application of this technique to industrial applications. Significant opportunities presently exist in developing further applications for this technique, particularly in studying and understanding the contrast mechanisms involved in SEAM analysis.


Acknowledgments


The authors would like to acknowledge the support of the staff at the Laboratory of Functional Inorganic Materials at the Shanghai Institute of Ceramics where most of the initial work were performed. We also acknowledge the support of Scanning Beam Technology Pte. Ltd. (http://www.sbtech.com.sg)company for the provision of a SEAM 100 system for the research work at IMRE.


1. E. Brandis and A. Rosencwaig, Appl. Phys.


Lett., 37, 98-100 (1980)


2. G.S. Cargill III, In Scanned Image Microscopy,p 319, Academic Press, New York (1980)


3. L.J. Balk and N. Kultscher, Inst. Phys. Conf.


Ser., 67, 387-392 (1983a)


4. L.J. Balk and N. Kultscher, J. Phys. (Paris),Colloque C2, C2-873-876 (1984)


5. D. Marty-Dessus and J.L. Franceschi, Elec. Lett.,29(10), 843-844 (1993)


6. B.A. Shaw, J.T. Evans and T.F. Page, J. Mat.


Sci. Lett., 13, 1551-1554 (1994)


7. X.X. Liu, L.J. Balk, H.P. Abicht, A. Eckau and Q.R. Yin, Solid State Pheno.,63-64. 361-368(1998)


8. J. Liao, Y. Yang, X.P. Jiang, S.X. Hui and Q.R.


Yin, Materials Letters, 39, 335 (1999)


9. M. Domnik and L.J. Balk, Scan. Micr., 7(1), 37-48 (1993)


10. K. Kaufmann, K. Orsech, M. Domnik and L.J.


Balk, J. Phys. D:Appl. Phys., 27, 2401-2413(1994)


11. J. Opsal and A. Rosencwaig, J. Appl. Phys., 53,4240-4246 (1982)


12. T. Ikoma, M. Murayama and K. Morizuka, Jap.


J. Appl. Phys., 23, Suppl. 23-1, 194-196 (1984)


13. V.A. Sablikov and V.B. Sandomirskii, Sov.


Phys. Semicond., 17, 50-53 (1983)


14. M. Sasaki, H. Negishi and M. Inoue, J. Appl.


Phys., 59, 796-802 (1986)


15. N. Kultscher and L.J. Balk, J. Scanning Elec.


Micros., I, 33-43 (1986)


16. L.A. Koirakh and V.L. Preobrazhenskii, Sov.


Phys. Acoust., 30, 134 (1984)


17. R.G. Stearns and G.S. Kino, Appl. Phys. Lett.,47, 1048-1050 (1985)


18. L.J. Balk and N. Kultscher, Beitr.


Elektronenmikroskop.Direktabb. Oberflacehn.


16, 107 (1983b)


19. L.J. Balk, D.G. Davies and N. Kultscher, Phys.


Stat. Sol., 82(23), 23-33 (1984)


20. E. Menzel and E. Kubalek, Scanning Electron Microscopy, Part I, 305-317 (1979)


21. J.W. Fang and Q.R. Yin, unpublished research(2000)


p 17-21


DOI: 10.1361/cp2000istfa017


Application of Single Contact Optical Beam Induced Currents(SCOBIC) for Backside Failure Analysis


M. Palaniappan1,2, J.M. Chin1,2, J.C.H. Phang2, D.S.H. Chan2, C.E. Soh1, G. Gilfeather31Advanced Micro Devices (Singapore), Singapore 2Centre for Integrated Circuit Failure Analysis and Reliability, Faculty of Engineering,


National University of Singapore, Singapore


3Advanced Micro Devices, Austin, Texas, USA,


The Single Contact Optical Beam Induced Currents(SCOBIC) is a new failure analysis technique, which allows the imaging of junctions by a single connection to the substrate or power pin of an integrated circuit. Modern packaging technologies and multi-layer metallizations has increased the need for backside IC failure analysis. In this paper, the SCOBIC technique is used to image junctions from the die backside. The implementation of backside SCOBIC system is discussed. Application of the SCOBIC technique from both the frontside and backside of CMOS and NMOS devices are presented.


Beam induced current techniques have been successfully used to detect electrical defects in silicon for failure analysis. However the application of conventional beam induced current techniques such as OBIC and EBIC are limited due to the need for two contacts to be connected across the imaging junction. The requirement to electrically connect both sides of the junction under investigation poses a severe limitation on the usefulness of the technique when applied to the failure analysis of VLSI circuits.


The single contact electron beam induced current technique (SCEBIC) [1] was developed to image junctions on an integrated circuit. This technique requires only a single contact such as the substrate pin or the power pin. The main limitation of SCEBIC is that it uses an electron beam that requires the device under test to be in a vacuum chamber. In addition, the penetration distance is dependent on the electron beam energy, typically several microns for 30keV electrons in silicon.


In an earlier paper, the single contact optical beam induced current technique (SCOBIC) [2] was developed using for a 633 nm HeNe laser for frontside analysis.


With the widespread use of flip-chip and lead-onchip packaging with multilevel metallization, there is a need to adapt SCOBIC for backside analysis. In this paper, an IR NeHe laser is used to implement a backside SCOBIC system. Application of the SCOBIC technique from both the fronts3ide and backside of CMOS and NMOS devices are presented.


The phenomena of how a SCOBIC transient is generated can be explained with the help of the equivalent circuit of a p-n junction for this technique as shown in Figure 1 [4]. The physical connection of device is shown in Figure 2.


Figure 1 Equivalent circuit diagram of a junction using the SCOBIC technique.


Figure 2 Physical connection of the device using the SCOBIC technique.


When the laser beam impinges on to the p-n junction,a photocurrent IGis induced due to the generation of electron-hole pairs. This current then flows through the current amplifier and starts charging the parasitic capacitor C1. As a result, the n type region is at a more negative potential with respect to the p type.


This forward biases the p-n junction, causing a diode current IDto flow. A equilibrium is reached between IGand IDat which point no current flows through the current meter and the capacitor is charged to its maximum. When the laser beam impinges at a distance away from the junction, IGis smaller since some of the electron-hole pairs recombine before they reach the junction. Detailed description of the principle of the single contact method is in [5].


Experimental


System Set-up


The system set-up for backside SCOBIC imaging is shown in Figure 3. It consists of a laser scanning microscope (LSM), a near infrared acousto-optical modulator (NIR AOM), a current amplifier, a signal generator and lock-in amplifier as a signal acquisition module.


An infrared HeNe laser with a wavelength of 1152nm and 1mW power was used to generate electron hole pairs. The X and Y movement of the laser is controlled by the scanner card. The laser beam is pulsed by modulating the laser beam using an NIR acousto-optic modulator (AOM). The AOM driver consists of a free-running quartz-crystal carrierfrequency oscillator, a wideband balanced diode ring modulator, a bias level adjustment and a broadband Class-A amplifier.


Figure 3 Schematic diagram of the backside SCOBIC system.


The depth of modulation is determined from the amplitude of the modulating input, which can be controlled by the signal generator. By alternating the modulation between 0% and 100% the laser beam can be pulsed. A jig was built to align the AOM with the IR laser path. The laser beam needs to be pulsed to allow the parasitic capacitor to charge and discharge, producing SCOBIC transients [6]. For SCOBIC the laser is pulsed and raster scanned over the IC in atmosphere.


When the laser beam impinges on the device under test, SCOBIC transients are generated and are amplified by a low noise amplifier. A lock-in amplifier is used as the signal acquisition tool to increase the sensitivity and signal to noise ratio of the collected SCOBIC transient. The output of the lockin amplifier is fed to the imaging acquisition system to generate the complete SCOBIC image for the region being scanned. A signal generator is used to provide the reference signal to the lock-in amplifier as well as control the depth of modulation of the AOM. A common signal generator ensures the synchronization between the laser scanning and the signal acquisition systems. A SCOBIC software program written in C controls the overall operation of the system. This software acquires a 512x512 pixed SCOBIC image in less than three minutes.


Device Description and Sample Preparation


Two test chips, a CMOS device and an NMOS device were used for the analysis. The CMOS device was fabricated using a 0.7 micron two metal layer process and was decapsulated for the frontside analysis. The device used for backside analysis is a short channel large-angle-tilt-implanted-drain(LATID) nMOSFET test structure fabricated using


0.6 μm technology on 6.0-9.0 Ω-cm expitaxial layer on a p-substrate. For backside investigations, the substrate of the nMOSFET was polished down to a thickness of approximately 15 μm using mechanical grinding and polishing. The electrical characteristics


of device were monitored continuously during the sample preparation to ensure that the functional behaviour of the device does not change during the sample preparation.


Figure 4 LSM reflected image of portion of CMOS device.


Figure 5 SCOBIC image of a CMOS device obtained by connecting the VSSterminal to the signal analysis module (50X objective).


Results and Discussion


Frontside Analysis


The frontside SCOBIC imaging was performed on the CMOS device to demonstrate the usefulness of this new technique for failure analysis.


Figure 4 shows the LSM reflected image of a portion of the CMOS IC. The corresponding SCOBIC image obtained by connecting the VSSterminal to the signal analysis module is shown in Figure 5. The bright white line in Figure 5 shows that SCOBIC is able to resolve the well/substrate junction clearly as indicated by the arrows. This ability of SCOBIC in revealing such detailed junction is due to the unconnected junction contrast phenomenon.


Backside Analysis


Figure 6 shows an LSM reflected image of short channel NMOS transistor in a p-well. The corresponding SCOBIC image is shown in Figure 7,which clearly shows the source and drain regions of the transistor as well as the P-well-substrate junction.


Figure 6 LSM reflected image of short channel NMOS transistor in a P-well (magnification 40X).


Figure 7 SCOBIC image of the NMOS device obtained by collecting SCOBIC signals from the substrate pin.


A magnified reflected image of the same transistor is shown in Figure 8 while Figure 9 shows the corresponding SCOBIC image. The SCOBIC image is able to show all the junctions of that transistor including the source/drain-well junctions,source/drain regions and the contacts to the diffusion regions.


Conclusion


It has been demonstrated that SCOBIC technique can be used to image all the junctions in the IC from the silicon substrate including the junctions, which are not directly connected to the external pins.


Implementation of backside SCOBIC has also been discussed in detail.


The authors would like to thank CM Chua, LS Koh and SH Tan of SEMICAPS Pte. Ltd. for their instrumentation advice and support. We would also like to thank Carl Zeiss Singapore (CZS) for the loan of the LSM system.


Figure 8 LSM reflected image of the NMOS at magnification of 200X.


Figure 9 SCOBIC image of figure 8.


1. Phang JCH, Kolachina S, Chan DSH, "Single Contact Electron Beam Induced Current Microscopy for the Failure Analysis of Integrated Circuits", Proc 23rd Int Symp Testing and Failure Analysis, 27-31 Oct 97, Santa Clara,California, USA, pp 215-219, 1997


2. Chin JM, Phang JCH, Chan DSH, Soh CE,Gilfeather G, “Single Contact Optical Beam Induced Currents (SCOBIC) - A New Failure Analysis Technique”, Proc 2000 Int Rel Phys Symp (IRPS 2000), 11-14 Apr 2000, San Jose,USA, pp 420-424, 2000.


3. Ong VKS, Chan DSH, Phang JCH,"Observations of EBIC Contrast of Unconnected Junctions", Proc 4th Int Symp Physical and Failure Analysis of Integrated Circuits, 2-5 Nov 93, Singapore, pp. 45-49, 1993.


4. Kolachina S, Phang JCH, Chan DSH, “Single Contact Electron Beam Induced Currents(SCEBIC) in Semiconductor Junctions. Part I:Quantitative Verification of SCEBIC Model”,Solid State Electronics, Vol. 42, No. 6, pp. 957-962, 1998.


5. Kolachina S, "Single Contact Phenomena in Beam Induced Current Microscopy", PhD Dissertation, National University of Singapore,


6. Ong VKS, Phang JCH, Chan DSH, "Novel EBIC Observation of Unconnected Junctions of Large Area VLSI Circuits", Proc 20th Int Symp Testing and Failure Analysis (ISTFA '94), 14-18 Nov 94,Los Angeles, California, USA, pp. 49-56, 1994.


p 25-33


DOI: 10.1361/cp2000istfa025


Measurement of Interfacial Adhesion and its Degradation in Multi-layer Packages, Devices, and Blanket Films using the Laser Spallation Technique


Vijay Gupta, Robert Hernandez


Department of Mechanical and Aerospace Engineering University of California, Los Angeles, CA, USA


Rajen Dias, Vasudeva Atluri, George Raiser, Mike Mello, Lars Skoglund, and Paul Zimmerman


Intel Corporation, Chandler, AZ, USA


A laser spallation technique to measure the tensile strength of thin film interfaces is introduced. In this technique, a laser-generated stress wave of nanosecond duration in the substrate spalls off(completely removes) a coating deposited on it’s the substrate’s front surface. The threshold laser energy is converted into the tensile stress (strength) at the failure site (usually the interface) by using an optical interferometer. Because of the ultra-short duration of the stress wave loading, all plastic deformation processes that usually accompany the coating decohesion event are suppressed such that the measured value can be regarded as fundamental or intrinsic to the material system (including the defects,if any). Application of this technique to test planar as well geometrically heterogeneous interfaces in IC’s,substrates, and packages is demonstrated. The technique is used to quantify the degrading effects of moisture and in-situ temperature rise on the tensile strength of a polyimide/Si3N4/Si interface system whose strength was systematically degraded by exposing the samples to controlled humidity (50-70%RH) conditions for varying duration (12-96 hrs) and temperatures (30°C-150°C). These measurements of strength degradation can now be used to predict device reliability from a fundamental standpoint in conjunction with simulations capable of predicting time-dependent stress concentrations, moisture accumulation, and temperature rise at critical interfaces during processing and service environment in actual systems.


Multilayer structures composed of metallic,polymeric and ceramic films form an integral part of electronic devices and play a vital role in the microelectronics industry. To carry out their intended electrical functions, avoidance of mechanical failures in the form of coating cracking and delamination during processing and service is of major concern. In addition, due to the large


mismatch in the thermal expansion coefficients of the package (20 ppm/ºC) and silicon (3 ppm/ºC), failures during integration of silicon to package are also observed and include, (a) delamination at the epoxy/passivation interface, (b) deformation and cracking of metal and passivation, (c) delamination and lifting of thin metal lines from silicon, and (d)formation of circular holes, also known as bullet holes, on silicon passivation.


To avoid the above failures, a fundamental understanding of the adhesion between different layers as a function of process (film deposition and surface variables) and service (moisture, temperature,and time) conditions during manufacturing and reliability testing is warranted [1]. This requires development of an adhesion metrology tool that is capable of measuring the fundamental tensile strength of an interface both in blanket and actual device geometries. The fundamental nature of the measurement is emphasized as it would allow a quantitative description of the effects of various process (for optimizing performance) and service (for predicting reliability) variables on interface adhesion.


These measurements of strength degradation with service variables can be used in conjunction with simulations capable of predicting time-dependent stress concentrations, moisture accumulation, and temperature rise at critical interfaces during processing and service environment in actual systems to predict device reliability from a fundamental standpoint.


The aim of this paper is to (a) introduce the laser spallation technique for interface strength measurements, (b) present interface strength data as a function of moisture, temperature and time variables on a blanket polyimide/Si3N4/Si interface system, and


(c) demonstrate the potential of the laser spallation technique in characterizing interface strengths in-situ in C4 plastic substrates and assembled flip chip packages. For the in situ study, C4 bare substrate Cu vias/dielectric layer (on and off bump areas) and Cu line/dielectric layer interfaces were measured. Also,underfill (UF) and bump interfaces to die and


substrate in flip chip packages were studied.


Forthese samples, only qualitative adhesion data in terms of failure loci and critical laser fluences and their reproducibility is presented, as actual


quantification of stresses at heterogeneous interfaces using interferometry is still under investigation.


Figure 1 Schematic of the laser spallation experiment. The arrows on C and T in the lower left inset indicate the direction of the compressive and tensile stress waves.


Sample Preparation


Blanket Samples


Si substrates of <100> orientation were chemically cleaned using acetone and HMDS vapor prime. A 750 nm-thick layer of Si3N4was deposited on these cleaned surfaces using the plasma enhanced chemical vapor deposition process. A polyimide precursor bearing the chemical name polyamic acid of pyromellitic diaanhydride/4,4’-oxydianiline was spin-coated onto the nitride surfaces by operating a Headway spin-coater at 4000 rpm for 40 s. The asspun resin was cured at 135ºC for 2 hrs to convert it into a chemically and structurally stable film. The final thickness of the dielectric films was nominally


2.5 μm. The glass transition temperature for the cured film was reported to be greater than 400ºC.


The samples were divided into four groups. Group I samples were stored in a dessicator immediately after the films were cured. These samples were used to study the effect of in-situ temperature rise on the


tensile strength of interfaces. Samples were tested at 22ºC, 50ºC, 100ºC and 150ºC consistent with typical processing and service temperatures experienced by the devices. These samples were also tested after cooling them to ambient. Group II samples were used to study the effect of relative humidity (50%,60% and 70%) at a fixed time (48 hrs) and temperature (ambient). Group III samples were divided into three categories to study the influence of varying time (24 hrs, 48 hrs, 72 hrs) at a given 60%RH at 38ºC. Finally, the effect of temperature was assessed by exposing samples in a 60%RH environment at different temperatures (30ºC, 35ºC and 40ºC) for a fixed 24 hrs hold time. The choice of different levels of test matrix variables was guided by the current accelerated device testing protocols employed by the industry. All these samples were prepared at UCLA.


↑


中0yPhotodiode Ar Ion laser


Digitizer


M2


M3


M1


Nd:YAG Laser


C C↓


FT


SiO2


Al


Substrate Coating


Geometrically Heterogeneous Samples


For carrying out in situ package measurements, 31 samples of “Substrate plus UF” (with die polished off), 31 samples of “Die plus UF” (with the substrate polished off), and 50 units of bare C4 substrates were obtained from Intel Corporation and tested.


Experimental Procedure


A brief description of the basic laser spallation methodology to measure the tensile strength of a single thin film/substrate interface system is presented before discussing specific procedures adopted for the present study.


The Basic Laser Spallation Technique to


B


Test Interface Strengths at Ambient Temperature


d


In this experiment (Fig. 1), a 2.5 nanosecond (ns)long Nd:YAG laser pulse is made to impinge over a 3 mm-dia area on a 0.3 µm-thick aluminum film which is sandwiched between the back surface of a substrate disc and a 50 to 100 µm thick layer of solid waterglass. The melting-induced expansion of the aluminum film under confinement generates a compressive stress pulse (with 1 nanosecond rise time) directed toward the test coating which is deposited on the substrate’s front surface. The compressive stress wave reflects into a tensile pulse from the coating’s free surface and leads to its spallation (complete removal) at a sufficiently high amplitude. The critical stress at the interface is calculated by measuring the transient displacement history of the coating’s free surface (induced during pulse reflection) by using an optical interferometer with a resolution of only 0.2 ns in the single shot mode. The measured free surface velocity is related to the local interface stress via a wave mechanicsbased simulation. An expanded discussion on why this technique provides a fundamental measure of the interface’s tensile strength, including its correlation with the atomic structure,interfacial chemistry, and independently obtained intrinsic toughness values,can be found elsewhere [2,6].


Measurement of Interface Strength at Elevated Temperatures


The basic mechanics of the laser spallation experiment discussed above remains the same even at elevated temperatures [7]. The sample was supported vertically inside a groove made on a pyrolytic graphite plate that sat inside a quartz tube of an oven capable of heating the sample up to 1000ºC. The two ends of the quartz tube were capped with identical quartz window-stainless steel assembly so as to allow access to the YAG and Argon ion laser beams used for pulse generation and recording, respectively.


A long focal length lens was used to direct the YAG laser beam from the outside to a 3 mm diameter spot on the confined Si surface opposite the polyimide layer. After the sample was left inside the oven long enough (10-15 min) to reach equilibrium conditions,the interface was loaded with single stress pulses of increasing amplitudes at different locations (to avoid fatigue effects) to find the threshold stress pulse causing coating spallation. The quantification of the interface stress corresponding to the latter followed the procedure outlined above.


0 500


1000 S1500 S2000


S


2500 3000 3500 4000


50


150


200


Laser energy (kJ/m2)


Water Glass 40 Microns Water Glass 50 Microns Water Glass 20 Microns Water Glass 10 Microns


Figure 2 Stress wave characterization in silicon.


Specific Procedure used in the Present Study to Test Multilayer Blanket Films


The basic laser spallation methodology as discussed above for a single film/substrate interface system was adopted. While applying the technique to multilayers supported on a Si chip, it was found that sufficient tensile stress for decohering interfaces could be generated without the use of the laser absorbing Al film. So no Al layer was used in the present study.


However, as before, it was still necessary to cover the Si bare surface opposite to that carrying the multilayers with a 40-50 μm-thick layer of waterglass, which previously was showed to optimize the stress wave amplitude. The laser heating diameter(3 mm) to substrate thickness (< 1 mm) always exceeded 3. As discussed in Argon et al. [8], this ensures one-dimensionality of the stress wave over 95% of the stressed interface area.


For the sake of convenience and also for testing multilayer samples, the following three-step procedure was adopted. The critical laser fluence causing coating spallation was recorded first.


Quantification of interface stress followed next by performing measurements of stress pulses as a function of laser fluence on a control sample consisting of a bare Si wafer bearing the same thickness, structure, and orientation, and with the same waterglass layer thickness, as in the actual


multilayered test specimens.. Simultaneous recording of the free surface velocity of the separating film, using interferometry, was not performed in the present work. The procedure used to record and reduce the fringe data to actual stress wave profiles was otherwise similar to that used in


[1] and discussed briefly above. Figure 2 shows such a chart, which


-4.00-3.50-3.00-2.50-2.00


03


0-1.50 0-1.00 s


-0.50 e0.00


0.50


1.00


1.50


9


10


15


20


25


30


Time [ns]


PI/Si3N4


e，


Si3N4/Si


interface 1


interface 2


Si


0.837


0.9420.942


0.44


0.495


-1.81-2.038


Interface stresses


GPa


Figure 3 Interface stress histories as determined from the simulation.


essentially allows the conversion of the laser fluence to stress pulse amplitude inside Si for a given waterglass layer thickness. Finally, a finite elementbased acoustic wave mechanics simulation was developed which calculates the tensile stress histories at any of the interfaces in a given multilayer assembly when loaded normally by the propagating stress wave of a prescribed profile and amplitude from the Si side. Other inputs to the program include thickness and respective elastic properties of each layer, including density, Young’s modulus, and Poisson’s ratio. Only one wave profile was considered in the simulation, as all stress wave profiles at different laser fluences reduced to a single profile when normalized by the peak amplitude.


Thus, it was only necessary to use the peak wave amplitude as the loading parameter, which in turn could be read off from Figure 2 corresponding to the threshold laser fluence.


With the above three-step procedure, it was no longer necessary for the interferometric measurements to be performed during each spallation event. The threshold laser energy for coating spallation was determined (which takes only a few seconds) using visual inspection of the shock-loaded samples, and converted to the peak stress pulse amplitude using Figure 2 for the appropriate waterglass layer thickness. The normalized stress wave profile with this amplitude was used as an input to the program,along with the prescribed multilayer geometry and elastic properties, to calculate the desired tensile stress history of the interface which failed. Figure 3 presents the results of a typical simulation and shows the calculated interface stress histories at the


nitride/polyimide and nitride/oxide interfaces.


Positive values represent tensile stresses. The peak of the interface tensile stress history was taken as the interface strength.


For in-situ high temperature testing, the same threestep procedure was used. The transient displacement history of the free surface of Si was successfully recorded even in the presence of thermal radiation.


Since the reduced velocity profiles from the recorded interferograms were of the same rise times as those obtained under ambient conditions, it was concluded that the strain rate of loading is still way too high to


allow relaxations in Si up to 150ºC. Thus, data in Figure 2 was used to convert the threshold laser fluence for use in the finite element procedure.


Again, because of the high strain rate, both coating and substrate materials were idealized as linear elastic in the wave mechanics simulation. Whether this can be strictly assumed for the polyimide coating deformed at 150ºC under a strain rate in excess of 106s-1needs further confirmation. However, using interferometry, indirect evidence in support of this assumption was provided by recording similar fringe data and associated velocity rise times from the free surface of the polyimide coating under ambient and in-situ 150ºC conditions.


Results


All samples failed at the nitride/polyimide interface,regardless of whether they were tested in-situ at elevated temperatures or subjected to moisture and humidity treatment alone.. Interestingly, because of the transparency of the polyimide film, the threshold laser energy that caused the nucleation of first interface crack or onset of decohesion in an otherwise intact film could be detected by viewing Newton fringes under an optical microscope, even prior to complete removal of the coating from the substrate.


In-situ elevated temperature test results are summarized in Figure 4. All strength values are average of 8 to 10 measurements. The maximum variation was limited to within 7%, and hence the observed strength variations are attributed to the material dfferences. The strength degrades nonlinearly from 304 MPa at 22°C to 245 MPa at 50ºC,beyond which it degrades almost linearly with temperature to 167 MPa at 150ºC. It is interesting to note that only a single heating cycle was sufficient to cause irreversible degradation in the interface strength as evidenced by ambient testing of samples that were heat-treated at 50ºC and 150ºC for 10 min and cooled in air.


0 u50 100 S150 u


0200 u250 d300 350


Temperature (deg C)


In Situ High


◆


Temperature Strength一量Strength Upon


Cooling


好


22,304


50,245


50,167


100,202


150,167


150,141


Figure 4 The effect of in-situ temperature on interface strength.


As Figure 4 shows, the strength of the sample heated


Bump to substrate interface


to 50ºC, then cooled and tested at room temperature,reduced dramatically to 167 MPa compared with 304 MPa for the sample both heated and tested at 50ºC. This effect was even stronger in samples that were heated to 150ºC and then tested at ambient conditions, where the strength reduced to only


Direction of laser shot


141 MPa. A plausible reason for this degrading effect is furnished later.


Interface Strength of Polyimide/Silicon Nitride Interface:Effect of Humidity (Time = 48 hours)


u


205


岁


210 215


d w220 S8225 u


230 41


6


235 240


Epoxy to substrate interface


55


60


65


70


75


Relative Humidity (%)


50,237


60,207


70,205


Figure 5 The effect of relative humidity on the interface strength.


Figure 5 shows the effect of varying relative humidity when the samples were held for 48 hrs at 38ºC. There is a strong degrading effect of moisture between 50% and 60% RH beyond which the effect attains a saturation level. Discovering this saturation effect is of obvious importance in the design and prediction of device reliability.


I


190 nu195 3200


210


215


220 d225


230


40


80


Time (hrs)


Figure 6 The degrading effect of subjecting the samples to increasing durations in a fixed moisture(60% RH) and temperature (38ºC) environment.


The degrading effect of subjecting the samples to


increasing durations in a fixed moisture (60% RH)


n


and temperature (38ºC) environment is shown in


Figure 6. The effect does not appear to follow the typical Arrhenius-type as is usually expected in such studies. Instead, there is almost a linear degradation from 224 MPa at 24 hrs hold to 195 MPa at 72 hrs hold time, beyond which the strength plunges significantly to 140 MPa at times nearing 100 hrs.


Clearly, such points where the data shows a dramatic turn should be critical while designing packages and IC’s using the proposed new reliability strategy.


Figure 7 Substrate+UF sample geometry.


The effect of the temperature (30ºC, 35ºC and 40ºC)at which samples were exposed in a 60% RH environment for a fixed time (24 hrs) was also studied. This matrix of temperatures was chosen since previous in-situ tests (Figure 4) showed the degrading effect to be the most significant in this temperature range. The data showed a steeper decrement of strength with temperature compared with samples that were not exposed to with humidity environment.


Procedure to Test Packages


The initial plan was to characterize the UF/die,


41 U


UF/substrate, bump/die and bump/substrate interfaces by subjecting the fully assembled package units to stress wave loading in the laser spallation setup, and


U


then look for damage using the CSAM technique.


Several loading configurations were tried, but unfortunately, none appeared to cause any interface damage. Apparently we need laser energies higher than 2 J for possibly decohering these interfaces, insitu, in assembled packages.


To circumvent the above difficulties, two sets of samples were prepared. In one set, the substrates were polished off from the packages to leave dies with the UF intact. Such samples were labeled“Die+UF,” (Figure 8) and 31 such units were obtained from Intel Corporation. Similarly, the die was polished off in another set of samples, leaving the substrate with the UF. Such samples were designated “Substrate+UF,” (Figure 7) and 31 such units were acquired from Intel Corporation(Chandler, Arizona). The “Die+UF” samples were:


Die to epoxy interface


Bump to die interface


Figure 8 Die+UF test geometry.


subjected to a laser pulse from the die side without using the waterglass layer as the already existing underfill material served as the constraining material(Figure 8). For the “Substrate+UF” samples, the laser was shot from the substrate side with the covering waterglass layer (Figure 7).


Up to 9 laser shots, with 2 mm-dia focussed spot,were taken on each sample, and the threshold laser energies for interface failure recorded. Specific results on each sample set are discussed next.


As the laser fluence was controllably increased, the first visible damage in the “Die+UF” samples was noted when the underfill from the UF delaminated and spalled off from the die surface while leaving the bumps/die interfaces intact. Figure 9 shows a top view of such damage. The extra dark region is the delaminated die/underfill interface. Note all bumps inside and outside the failed regions remained intact.


The threshold laser energy of 0.095 +/-0.01 J over a 2 mm-dia focussed area was recorded with remarkable


reproducibility for initiation of such a failure. As the laser energy was further increased while keeping the same laser heating spot diameter of 2 mm, individual bumps were found to spall off like “bullets.”Focussing under an optical microscope suggested failure of the bumps from their underlying Al bond pads. This was independently confirmed by analytical tests as well. As the energy was increased to 0.34 J and beyond, the failure was within the bulk Si wafer.


Figure 9 Die+UF sample failure.


Figure 10 A Substrate+UF sample from where the bumps have been spalled.


For the substrate+UF samples, the first damage involved spalling individual Pb-Sn bumps from their underlying Cu vias while the UF remained attached to the plastic substrate (Figure 10). Laser energy in excess of 0.15J over a 2mm-dia area led to 100% of such failures. The failure locus remained consistent in all these failures. As the laser energy was further increased, the underfill was observed to delaminate from the substrate interface. Since the threshold laser energy for the bumps was already exceeded, the failure surface showed the spallation of the bumps as well as the UF from the substrate surface (Figure 11).


The darker region is the delaminated UF/substrate


interface and the spalled bumps bumps in this region are out of focus compared to bumps still attached outside the damaged area. A somewhat large variation in the underfill failure energy, possibly due to bubbles or filler size variation, was observed. But use of laser energy 0.6 J and beyond led to a 100%failure event.


Figure 11 A Substrate+UF sample from where the


bumps and underfill have been spalled.


Testing of Bare Substrates


Several C4 substrates were tested. The Cu layer of the substrate circuitry was used as the laser-absorbing layer, with waterglass as a constraining medium. The stress wave traveled through the BT core and reflected into a tensile wave upon reflection from the surface of the top copper layer. As before, the returning tensile wave pried off the weakest interface at acritical amplitude.


Figure 12 Failure in a bare substrate sample.


For each substrate, two areas, on and off-solder ball,were loaded. This was accomplished by moving the location of the laser heating spot, which in turn was maintained at a diameter of 2 mm. The laser energy was controllably increased, and after each shot, the


sample was observed under an optical microscope to spot any event of crack nucleation.


When the samples were loaded directly underneath the Pb-Sn solder balls, the stress wave completely pried off the solderballs Figure 12 shows a top view of the failed surface from where they have been completely removed. In fact, this picture is from a sample where the damage had just nucleated underneath the surface at the Cu via/dielectric interface. The rings around the failed solder ball areas are reflections of the crack that started at the Cu via/dielectric interface at the 2F/3F level and then grew radically outward and toward the sample’s free surface. When the energy was increased beyond the threshold level, the crack reached the free surface to form a complete material spall and thus left behind a crater on the sample surface. A detailed view of the section through the failed spot at the Cu via showed the local failure to be at the Cu/dielectric interface.


The critical laser energies for accomplishing this failure showed remarkable reproducibility.


For off-solder ball loaded areas, the failure was subsurface and at the interface between the Cu trace and the dielectric material located between the 2F and 3F layers. Since the stressed area was much larger than the via size, occasionally at some failed locations evidence of Cu vias separating from the dielectric layer was seen.


Discussion


The data presented here offers direct testimony of the ability of the laser spallation technique to provide a fundamental measure of an interface’s tensile strength, completely free of plastic effects. In this sense this test differs from the four point bend [9-11],blister [12], double cantilever beam [13], and indentation tests [12], where physics of such tests mandates strong influence of plastic effects on the measured properties. Measurements from these latter tests are of importance in predicting service failures where plastic effects almost always accompany a delamination.


It is generally known that the variables of moisture,temperature and time degrade interfacial adhesion.


This work is the first that quantifies such effects on the fundamental strength of interfaces. Even though a one-on-one correlation of the degraded strength with the corresponding change in the interfacial chemistry and structural relaxations was outside the scope of the present investigation, a plausible mechanism for the observed strength variations is suggested below.


The chemical structure of the as-spun polyimide precursor shows two open carbon rings. During


baking, ring closure occurs on account of dehydrolysis and results in the formation of the stable polyimide molecule. Since nitrogen in Si3N4has a lone pair of electrons, it can form hydrogen bonds at one of the open ring sites of the precursor molecule,if available via direct contact. Since hydrogen bonds are fairly weak they are constantly breaking and reforming even at ambient temperature. Thus, an insitu temperature rise should reduce the number of hydrogen bonds between the Si3N4and polyimide as ring closure through regular dehydrolysis also becomes possible. This mechanism is consistent with the data, which shows a decrement in the interface tensile strength with increasing temperature. Also,this explains the irreversible degrading effect of one heating cycle, as fewer open rings would mean a fewer sites for the nitrogen from nitride to bond to the polyimide precursor. The degrading effect of increasing relative humidity content and hold times is a direct result of the competition between the water molecules that segregate the interfacial region and the nitrogen of the nitride in forming the hydrogen bonds with the polyimide precursor. Whether the observed degradation in the strengths is a direct result of film swelling is a subject of on-going investigation.


Similarly, it is of interest to see if the strength degradation during in-situ temperature testing can be explained by the temperature-dependent relaxation in the film modulus. Such tests are presently in progress.


The data presented here now enable implementation of a fundamental device reliability strategy where the“strength charts” under varying humidity and temperature conditions can be used in conjunction with the already well developed simulation codes that are capable of predicting stress concentrations,moisture accumulation, and temperature rise at any of the interfaces within the package assembly. This will allow predictions for (a) whether the interface will be able to survive processing and system integration cycles during the design phase itself (prior to any IC fabrication and packaging), and (b) the level of interface strength needed at the time of manufacturing to ensure a prescribed service life.


This value can essentially be obtained by first reading off the strength degradation corresponding to the calculated moisture accumulation over the desired service life from the charts, and then adding to it the largest stress concentration at the critical interface under the expected service loads, as calculated from the FEM codes.


It should be mentioned that low-k dielectric films have been successfully tested using the laser spalaltion technique, but the data is not presented here because of space limitations.


The qualitative adhesion data for the UF/die,UF/substrate, bump/die, and bump/substrate interfaces, both in terms of failure loci and the


recorded threshold laser fluence values, shows the potential of the laser spallation technique for in-situ adhesion characterization in fabricated structures, a quality that now separates it from any other adhesion test method that is currently available. Even though a special sample geometry was used, it still preserved the basic interfacial structure and chemistry as in the actual fully assembled packages since the former were prepared by mechanically polishing the latter.


Use of YAG laser with 2J of energy could possibly decohere interfaces in packages, without the need to prepare special samples of die+UF and substrate+UF,as done in this work. The relative adhesion data can and should be converted to actual interface tensile stresses by using interferometry and wave mechanics simulations. Since the stress field is likely to be inhomogeneous, the failure may not occur at the weakest of the interfaces.


One of the limitations of the present technique is in testing very thin films since the net tensile stress is developed upon reflection from the film’s free surface. Experience has suggested that films greater than 0.5•m in thickness can be comfortably tested.


This also applies to individual layer thicknesses in a multilayer assembly.


The commercial version of the laser spallation experiment is presently under development, for use in an industry environment.


The research leading to basic adhesion data on nitride/polyimide system was supported at UCLA through a National Science Foundation Grant No.


9705068, for which we are grateful to Bruce MacDonald of that agency. Vijay Gupta also acknowledges the financial support provided to him by Intel Corporation, along with samples for in-situ testing.


1. Y. Feng, V. R. Raju, and E. Suhir, Structural Analysis in Microelectronics and Fiber Optics,EEP-Vol. 21, ASME, New York, 89-139 (1977).


2. V. Gupta, J. Yuan, and A. N. Pronin, J. Adhes.


Sci. Tech., 8, 6, 713-747 (1994).


3. J. Yuan, and V. Gupta, V., Acta Metallurgica et Materialia, 43, 2, 781-794 (1995).


3. J. Yuan, V. Gupta, and M. Kim, Acta Metallurgica et Materialia, 43, 2, 769-779(1995).


5. V. Gupta, U.S. Patent 5,438,402.


6. A. N. Pronin, and V. Gupta, V., J. Mech. Phys.


Solids, 46, 3, 389-410 (1998).


7. V. Gupta, M. O’Brien, and A. N. Pronin, J. Phys.


IV France, 9, 305-310 (1999).


8. A. S. Argon, J. A. Cornie, V. Gupta, L. Lev, and D. M. Parks, Mat. Sci. and Eng. A237, 224-228(1997).


9. P. G. Charalambides, J. Lund, A. G. Evans, and R. M. McMeeking, J. Appl. Mech., 56, 77(1989).


10. Q. Ma, J. Mater. Res., 12, 840 (1997).


11. S.-Y. Kook, J. M. Snodgrass, A. Kirtikar and R.


H. Dauskardt, J. Electronic Packaging, 120 [4],328-335 (1998).


12. K. L. Mittal, in K. L. Mittal (ed.), Adhesion Measurement of Thin Films, and Bulk Coatings,STP-640. American Society for Testing Materials, Philadelphia, 1978, p.5.


13. V. Gupta, A. S. Argon, and J. A. Cornie, J. Mater.


Sci. 24, 2031.


p 35-40


DOI: 10.1361/cp2000istfa035


New FIB-Supported Approach for Wirebond Characterization


Peter Jacob1, 2and Giovanni Nicoletti1


1EMPA Swiss Federal Institute for Materials Testing and Research, dept. Electronics/Metrology,Reliability Laboratory, Ueberlandstr. Switzerland


2EM Microelectronic Marin SA, Rue des Sors 3, Switzerland


Bond pad characterization is usually performed by mechanical cross-sectioning as well as pull and shear tests. However, since all these methods apply mechanical forces to the bond pad, artifacts may result. Focused Ion Beam (FIB) characterization is a mechanically stress-free characterization method,which allows more accurate conclusions regarding the intermetallic behaviour of the bonding area.


Some new approaches presented here show how to improve the FIB characterization procedure and to combine it with classical characterization methods.


Regarding packaged semiconductor devices, wire bond connections are one of the most important reliability concerns. Therefore, wire bond characterization is usually a scheduled part of process and quality control. However, two problems limit the throughput of bond characterization. First, the statistic relevancy is limited because only a limited number of bonding connections can be examined,and second, the usual tests impose mechanical stress to the bond pad, which may falsify the results. Pull and shear tests provide bond integrity information,but if they point to weak bond strength, no further intermetallic characterization can be done on these destroyed bond pads to characterize the intermetallic zone. If a mechanically polished metallographic cross section has been made, the polishing process will put some mechanical force to the bond pad,which may cause cracks in weak samples or smear the soft metal materials together. FIB characterization provided new approaches to overcome this problem (1).


FIB Cross-sectioning of


Wire-bonded Pads


Together with the leading FIB manufacturers FEI and Micrion, in 1995 we started FIB experiments to completely cross-section wire bonded pads (ball bonds) in order to characterize the intermetallic interface between the gold ball and the Al of the chip


metallization. However, these first experiments lasted an extremely long time due to the low beam currents available on FIB instruments at that time. To cut a complete ball bond at that time, an overnight processing of five and more hours of FIB time was necessary due to the limited capabilities of the FIB tools. Afterwards, intensive FIB polishing work at low current was necessary to allow conclusions about the grain behaviour and the intermetallic phase.


Although lengthy, such a procedure resulted in a clear FIB cross-section of a total bond pad as shown in Figure 1. The image allows a clear conclusion about the grain structures and deformations as well as about the intermetallic zone between the chip metal(Al) and the wire metal (usually gold). Other effects,such as Kirkendahl voids, can be clearly identified at high magnification.


Figure 1 FIB cross-section of a wirebonded pad.


Practical Results


Often classical mechanical polishing of bond pads,combined with information from bond pull and ball shear tests, resulted in conclusions that the bonding process was too weak. These conclusions were based on the presence of micro cracks in the interface region seen in mechanical cross-sections, and on the wire pull test result of bond pads being pulled off from the chip metallization (lifted metal failure),rather than the desired wire break at neck failure.


Aco.V Spot MagnWD Exp-120 μm


10.0kV 3 0 1000x1140Wet1.1 Torr


Figure 2 SEM view of a mechanically polished bond pad (undecorated).


A rough determination of the size of the intermetallic zone can be obtained by optical microscopy of polished cross-sections, but the dimensions of the interface require the better resolution of SEM for a clear understanding of the intermetallic formation.


However, SEM inspection of a traditional mechanically polished sample is unable to provide


新A0XA4


FECLON


Sue


information about the grain behaviour in the absence


of decoration by wet chemistry (grain etch) as shown


in Figure 2. Although this decoration is a standard


procedure in FA labs, it consumes additional time


and includes artifact risks. FIB enables crosssectioning, secondary electron and secondary ion


inspection, and grain size determination, all possible


without taking the sample out of the vacuum chamber


and without wet chemical treatment. Both FIB


imaging modes (secondary ion or secondary electron


imaging) are available in single beam instruments. In


dual beam instruments, secondary electron imaging


with an electron source is also possible. While


secondary electron imaging using an ion source gives


excellent information about ion channelling (grain


boundaries) as well as about potential contrast and


topography, secondary ion imaging produces


material-related contrasts and eliminates


voltage/charge-potential related contrasts and


channelling. Note, however, that the secondaryelectron yield is always better than the secondary ion


yield. This means that higher beam current is needed


in ion mode to obtain a good signal-to-noise ratio


when operating in ion imaging mode. The followingZLEMeps uxx


examples have been made in the secondary electron


imaging mode in order to include the grain boundary


information.


A careful analysis can prevent erroneous conclusions


of poor bonding on wire pull tested samples having


completely lifted bond pads instead of broken wires.


The following examples are taken from a series of


wire bonding-related reliability problems on low


power CMOS devices for automotive applications. A


large gradient of pull force data was measured and


bonds were removed completely by pull testing,


including the Al metallization. In some cases, a first


optical microscope inspection pointed to "bond


cratering", which means that substrate silicon would have been broken out. However, further analysis showed that only the pad Al was affected.


Figure 3a FIB view of the intermetallic phase(arrows) between the bond ball (gold, top) and the


chip metallization (Al, bottom).


Figure 3b A magnified view from Figure 3a shows a Kirkendahl void and to its right, the intermetallic phase. Here, the bond pad Al is entirely consumed.


Only the thin TiW layer on top of the first metallization remains (arrow). On the right side of the image, some Al remained, as should be the case over the whole bonding length of an ideal bond.


Figure 3a shows the intermetallic zone of a portion of a cross-sectioned wire bonded pad prepared by FIB cross-sectioning. The clarity of the FIB image allows


the determination that the intermetallic zone thickness is about three times larger than the original(Al) chip metallization thickness. The aluminum of the chip metallization in some areas has been completely consumed by the gold of the ball bond.


When the pad Al is completely consumed by the intermetallic phase, the bond adhesion on the remaining TiW barrier-sublayer is significantly reduced. A wire pull test of such a sample may result in a lifted metal failure. Lifted metal failures can also occur when bonding parameters are too strong and crack the layers beneath the bond pad. For this particular example, a process correction in the direction of lowering the bond force and energy successfully recovered the manufacturing line. By reducing the bonding pressure and ultrasonic energy,the intermetallic formation resulted in about one third of the chip metallization remaining (Figure 4). In the ideal case, this should be the structure over the whole bonding area. As a rule-of-thumb, the bond can be considered good if more than 60% of the cross section length shows this kind of structure. However,it should be remarked, that it is very difficult to obtain a good homogeneity over the whole bonding area. Even in the small cross section view of Figure 4 this can be seen clearly.


w


Figure 4 Good intermetallic phase, leaving parts of the chip metallization in its original texture.


New Methods


Applying FIB allows better resolution of the intermetallic interface, but still two problems remain.


First, the time needed to obtain a proper cross-section is too long and second, pull tests could not be performed on bond pads after FIB cross-section and examination. Our goal was now to improve this situation by modifying the FIB procedure to allow


both FIB and wire pull on the same bond pad. For the method development, we used samples on hand having no specific problem.


First we experimented with gas-supported etching in order to save milling time. The best results were obtained with iodine gas. Using this in combination with high currents (up to 50nA), process times for complete rough bond pad cross sections could be reduced to less than 1 hour. Additional time can be saved by working with pre-tilted angles: the rough milling can be done at a slightly negative angle,while the fine polish is done at 0 degrees of stage tilting and it is limited to the area of interest (usually the intermetallic zone). In total, the process time can be reduced to less than 1.5 hours.


Next we combined FIB characterization with the pull test. Usually, a bond pad which has been pulled off cannot be characterized further by FIB. Our approach was now both to further reduce process time and to retain FIB examinability. As a first step,we cut the bond pad at approximately a third of its diameter (Figure 5). When defining the cutting window, one must take care of the size of this cut. If the window is too small in the y direction, the material cannot be taken out of the deep trench cut during the milling process. We recommend a minimum width of 5 microns. Another challenge is the center region mills slower than the ends of the ball bond. Thus, the milling window must be resized several times during the milling, decreasing the length and at the same time increasing the milling rate by keeping the beam current high. Note that it is very important to support this process by iodine gas,otherwise the milled material would be backsputtered within the trench (2).


Figure 5 View of the separation cut.


When the cut reaches the bottom of the ball bond with certainty (best determined by a side-angle view as shown in Figure 6), the sample can be removed


chip Al


intermetallic phase


bond wire gold


and a regular pull or shear test can be performed.


When doing a shear test, the shear tool has to be carefully observed and approach the bond-ball so as not to impact the smaller, separated part of the bondball. While the larger section of bond ball itself will be pulled out of the bond pad, the smaller cut portion should remain. Thus it is important to make sure that the milling trench is deep enough so that a safe separation cut has been achieved over the whole length of the bond pad, not just the bond ball. If this is not the case, the wire pull might be successful, but the remaining part would suffer mechanical stress which certainly could falsify the results of the analysis. The cut should not be made too close to the edge of the ball bond, since the outer bond border might not be representative of the bonding quality


Figure 6 Side-angle-view of the separation cut within the whole bond area. On the other hand, the cut should not be too close to the bond center in order to minimize the influence of the bond interface area


deduction when doing pull testing.


Figure 7 shows the appearance after pulling (or shearing) under 0 degrees of tilting. Before starting the FIB operation, it is recommended to verify that the sample really has a problem worthwile exploring further. If, for example, when doing a pull test,always the bond wire is broken while the ball remains on its pad, the ball bond adhesion is good and doesn't require further FIB investigation.


(Of course, FIB characterization may be performed,for example for reference purposes, but then it requires a careful shearing instead of pulling of the main bond ball). In the example of Figure 7, the bond was good and the bondwire broke at the pull test. The remaining bond ball has been sheared, with some material of the bondwire left behind (see also Figures 8 and 9). This indicates effective bonding over most of the bond area.


Since pull and shear tests are not precise measurements but give an "order-of-magnitude"feedback about the pulling/shearing forces and the


remaining bondball footprint, a small bond pad arearelated deviation of 10-20% must be kept in mind when comparing these forces with those measured on uncut bonds. According to our experiences, no significant differences have been observed comparing cut vs. uncut ball bonds of poorly bonded pads within the same device. After completing this mechanical characterization, the sample can be taken back into the FIB. A further fine-milling-step, covering just the area of interest (intermetallic phase), should be performed according to the method described before.


This final milling produces a result which is shown in Figure 8 as an overview and Figure 9 in detail.


Although in our example the bonding is good, two undesirable bond effects can be seen. First, the intermetallic phase is too thick in places and has consumed most of the chip aluminum,and second, we observe an insular


Figure 7 Remaining part of the bond ball after a


shear test of the main bond part.


Figure 8 Overview of the partially polished bond X-section.


bonding (some small areas are not bonded at all). In this area, the original thickness of the chip Al can be clearly seen for comparison.


The slightly round shape of the cut surface makes it easy to reduce the polishing process strictly to the core area of interest, while the outside region remains unpolished (Figures 7, 8 and 9). This final step is not very time consuming and gives a very effective and fast view into the bonding-critical interface.


Figure 9 Detailed view of the zone of interest.


The final phase of polishing should be done without gas support and just using the low current beam.


Comparing this method to the "classical" FIB cut, it should also be mentioned that the amount of material to be milled is much less than in the case of the complete cross-section milling procedure. This reduces the FIB time to about one hour of operation including the local polish step, and, it allows application of pull or shear testing.


Precision milling procedure


While the method described above saves time and keeps other characterization methods available, in some cases, very high resolution imaging of the bond ball and the interface is requested. Mechanical metallography in those cases uses the method of a 45 or more degree sloped cross-section. This can also be accomplished by FIB, as Figure 10 shows. This cross-section has been done over a time frame of about 3 hours without gas support. In this case, the priority was given to a high quality/full area crosssection, so that a longer time was accepted. Since the cross-section was open, no metal-attacking gas support to accelerate milling and to avoid metal redeposition in corners and trenches was necessary.


An important aspect of this image is that the sample was pre-tilted 45 degrees before milling. The image,however, was taken at zero degrees of tilting. This means that the pre- and post-milling tilt procedure is


exactly vice-versa from usual. The advantage of this method is that the cross-section face itself has a 45 degree-angle •, which "increases" the "z-axis" of the zone of interest by a factor of 1/(cos •) (and therefore"magnifies" very thin horizontal layers compared to a traditional cut). Although this factor is of minor


Figure 10 Pre-tilted precision cut of a bondball,without gaz support.


importance regarding the macro structure of a bond,it becomes important when characterizing small micro-cracks or unknown interlayers at the border between the chip and bond ball material. If the FIB instrument allows negative 45 degrees of tilting, it is also possible to have a direct 90-degree-view on the cross section surface.


Summary and Conclusions


FIB methods allow stress-free characterization of wire bonding and can be combined with classical destructive test methods. Especially, FIB crosssections followed by bond pull tests allow an ideal combination: by performing a suitable, iodine gassupported FIB cut along 1/3 of the bond ball's top view and following with the pull-test, one saves not only milling time by reducing the material amount to be milled, but also receives the bond pull-force value,which does not significantly deviate as a result of separating part of the ball.


Sample pre-tilting allows also an improvement for imaging at the zone of interest, comparable to the method of mechanical slope cross sectioning. This is helpful when characterizing small micro-cracks at the ball bond interface.


We would like to express our thanks to the following for their excellent FIB support:


1. Andreas Schertel of FEI Europe GmbH


2. Jochen Meier of Rolling Thunder GmbH


and to:


3. Cheryl Hartfield of Texas Instruments


for her careful reviewing and many helpful remarks on this paper.


1. Volker Hönig, "Zerstörungsfreie Prüfung als Dienstleistung", p. 44-46, Surface Mount Technology, Boeblingen/Germany, April 1999,ISSN 0935-2317


2. FEI Company. "Beam Chemistries", FEI Newsletter 7/1999, FEI ,7451 NW Evergreen Parkway, Hillsboro, Oregon USA 97124-5830


p 41-48


DOI: 10.1361/cp2000istfa041


Failure Analysis of Flip Chip Bumps after Thermal Stressing


Tejpal K. Hooghan, Kultaransingh Hooghan, Sho Nakahara, Robert K. Wolf,Robert W Privette, Ralph S. Moyer


Lucent Technologies, PA, USA


This paper describes a new diagnostic technique for analyzing microstructural changes occurring to flip chip joints after accelerated thermal tests. Flip chip reliability was assessed at high temperatures, with and without the application of electrical bias. A combination of standard metallurgical polishing techniques and the use of a focused ion beam (FIB)lift out technique was employed to make site-specific samples for transmission electron microscopy (TEM)cross-sections. We studied evaporated 95Pb/5Sn bumps, on sputtered Cr/CrCu/Cu/Au as the under bump metallization (UBM). Thermally stressed samples were tested for electrical continuity and evaluated using 50 MHz C-mode scanning acoustic microscopy (C-SAM). Failed samples were crosssectioned and large voids at the UBM were observed optically. TEM specimens taken from the predefined UBM region of degraded flip chip devices provided critical microstructural information, which led to a better understanding of a cause of degradation occurring in the flip chip joints.


Growing use of high-density packaging in the electronic industry is fostering the adaptation of flip chip technology, and the long-term reliability of flip chips has become an important issue. At the same time, increasing use of these flip chip devices is driving development of new and novel diagnostic techniques to analyze failed devices. Failure analysis(FA) of integrated circuit (IC) devices typically involves various destructive/non-destructive procedures such as decapping, physical inspection,imaging, and electrical probing to isolate problems and failures. However, the flip chip device, as the name implies, is mounted on the substrate circuit side down. Contrary to conventional packages, these devices cannot be decapped and inspected. A new modified diagnostic procedure has to be developed.


Flip chip devices were traditionally attached to ceramic substrates, but organic substrates are increasingly being used to keep packaging costs down. Flip chip assembly on organic versus ceramic substrates presents a number of technical challenges.


For example, a melting reflow of the 95%Pb-5%Sn solder cannot be achieved on the organic substrate,because the glass transition temperature of the substrate is usually lower than the melting point(327°C) of the solder. Therefore, a eutectic solder pre-deposit is applied to the substrate to enable wetting at low temperature (220°C) reflow. Another significant challenge occurs because the coefficient of thermal expansion (CTE) of the organic substrate is 4-6 times that of ceramic. There is little CTE mismatch between the ceramic substrate and the silicon die. Conversely, there exists a large mismatch in the coefficient of thermal expansion (CTE)between the organic substrate and the silicon die.


This mismatch is known to cause the formation of a defective solder joint.


During high temperature (150°C) operating bias (5V)reliability aging, intermediate electrical test monitor points at 320 hours yielded no electrical failures.


However, at the 1000-hour test point, the vast majority of the population failed. Failed flip chip devices were screened using C-SAM imaging after subjecting them to reliability tests. A metallographic examination of the flip chip interconnections identified what appeared to be gross voiding in the UBM region. Subsequent SEM and TEM evaluations, however, determined that this region was not voided but was filled with one of the UBM metals which had undergone dramatic microstructural changes.


no issues 21 mm of Cu


BGA Solder Ball


C4 Bump


Figure 7 Low Magnification X-ray radiograph showing current X-ray radiography capability to image C4 bumps and BGA solder balls in a package mounted on a PCB.


Void


Plated


Through Hole


Figure 8 High Magnification x-ray radiograph showing current X-ray radiography capability to image C4 bumps and BGA solder balls in a package mounted on a PCB. Note the presence of voids in the solder bumps. No other features could be resolved.


As shown in these images, the subtle defects as highlighted in Figures 3-6 in C4 bump and/or BGA solder balls can not be resolved by the x-ray radiography technique even at high magnification and good penetration power (~225KV).


Current X-ray Tomography Capability


Currently, the computed tomography (CT) X-ray images are acquired using a “pseudo-laminography”approach where the images are collected by slicing the object horizontally with predetermined slice thickness and extensive image reconstruction. This technique has its limitations particularly in z-direction resolution. Although the technique offers an improved method for measuring the thickness and volume of solder material, it does not adequately detect the defects of interest. A good example of this technique is illustrated in Figures 9 and 10 showing


3-dimensional images of the C4 solder bumps obtained after significant image reconstruction. From these figures it is clear that this technique is good for in-plane defects such as solder voids but not suitable for critical defects such as delamination and cracks.


Also the current resolution is in the range of 10-20 microns and the time to useful images is >30 minutes.


Based on the survey of the several well known vendors in the industry it is concluded that the high resolution CT imaging in acceptable time periods(<10 minutes) on current packages using commercially available sources is impossible. This involves large volumes and small voxels (pixels in cubic volume). Small voxels are necessary for high resolution and large volumes are involved as a result of large samples due to multi-layer interconnects.


This suggests that the CT imaging in reasonable time periods will be possible if the voxel size is increased or volume of the material being imaged is decreased significantly thus restricting the imaging of multilayer samples non-destructively.


Another issue encountered with the current technique


|is imaging and detecting defects in individual layers of interconnects. The typical sample sizes of |is imaging and detecting defects in individual layers of interconnects. The typical sample sizes of |is imaging and detecting defects in individual layers of interconnects. The typical sample sizes of |is imaging and detecting defects in individual layers of interconnects. The typical sample sizes of |is imaging and detecting defects in individual layers of interconnects. The typical sample sizes of |
|---|---|---|---|---|

|100mmx100mmx50mm |with |2-4 |layers |layers |

|interconnects. |||||

packages with the heat sink, etc. is


Figure 9 C4 bump images showing voids in the bumps acquired using “pseudo-laminography”imaging and extensive image reconstruction.


Figure 10 C4 bump images showing voids in the bumps acquired using “pseudo-laminography”imaging and extensive image reconstruction. Same region as Figure 9 showing a different slice of the sample.


Theoretical Study Results


These studies included three different approaches,Fresnel phase zone plate, confocal coded aperture and state of the art computed tomographic imaging. The major issue with each of these was the data collection time for imaging. Image reconstruction would require additional time as well. All these approaches highlighted the need for high anode power and high aspect ratio zone plate construction. The anode power of the currently used sources is approximately 1 watt while the studies suggested that the required power for CT imaging in acceptable time periods would be approximately 100 watts.


Discussions


Critical Breakthroughs Required


Based on the above studies, it is suggested that a nontraditional approach to the CT imaging and system design may be required to achieve the requirements listed in Table 1. It is suggested that there is a need to develop the algorithm (software) and hardware for region of interest (ROI) imaging. This concept is similar to optical imaging where the user can image a sample at low magnification first and then zoom-in to the defect location using higher magnification. The only significant difference is that the higher magnification inspection for x-ray tomography will require significant image reconstruction and thus extensive software development. The critical hardware development required includes very high resolution stage with low vibration and detectors to increase the data collection efficiency and quality of images. Additionally, the anode re-design and improvements are a must to achieve very high x-ray flux necessary for CT imaging in an acceptable time.


CT Imaging of Micro-electronic Package


Figure 11 shows computed tomographic images obtained with an experimental system assembled in a laboratory environment to demonstrate the feasibility and advantages of this technique for microelectronic package failure analysis. Figure 12 is a cross-section scanning electron microscope image of similar region as shown in Figure 11 but on a different sample.


Notice the similarity between the two images. These observations clearly demonstrate the feasibility and the advantage of CT imaging for non-destructively detecting the solder fatigue cracking in a BGA joint.


The time taken for producing the image shown in Figure 11 was >2 hrs.


Figure 11 X-Ray 3-dimensional computed tomography image of BGA solder joints. Notice the presence of a solder void in the left hand side joint and a solder ball crack in the right hand side joint.


Solder fatigue Crack


Figure 12 SEM micrograph of a cross-section of a solder ball from a similar region as shown in Figure


11. Note the similarities between the Figures 11 and 12.


Based on the results presented above, it is concluded that the CT imaging offers significant advantage over the current failure analysis techniques for nondestructively detecting the failures. An example to demonstrate the feasibility of this technique has been presented. The major challenges for effective CT imaging are – sub-micron resolution in x, y and z directions through the multi-layer interconnects and thermal solutions such as heat sinks. In order to hasten the development of such a system for the micro-electronic industry it is suggested that a “one voice” be created to motivate the imaging vendors and also to generate funding for such a development.


There are significant technical developments that will be required for the successful and timely delivery of a CT imaging system. Some of these capabilities include x-ray optics and source development to deliver very high anode power, detector development to decrease time of image acquisition and improved resolution and development of image reconstruction algorithms for region of interest (ROI) imaging capabilities.


The author would like to acknowledge Gay Samuelson for her encouragement during this work,Bruno Clark, Martha Neustadt, Ruth Deacon and Jeff Thomas for their support in data collection. The author would also like to thank following x-ray imaging equipment manufacturers for their assistance in imaging microelectronics samples: Digiray,Nicolet Imaging Systems, Fein Focus USA, CR Technologies, X-Tek Systems Limited and Microphotonics, Inc. Additionally, the author would like to thank Drs. Tommy Thomas, Ken Tobin, Mike Paulus and Jim Hardy of Oak Ridge National Labs for various discussions.


1. Moore, T.M., and Hartfield, C.D., "Package Analysis: Sam and X-Ray", in Failure Analysis of Integrated Circuits: Tools and Techniques, p.


43-54, L C. Wagner (ed.), (Kluwer Academic Publishers, MA) Chapter 3, 1999.


2. S. Bolton, A. Mawer, and E. Mammo,“Influence of Plastic Ball Grid Array Design/Materials upon Solder Joint Reliability”,The International Journal of Microcircuits and Electronic Packaging, Vol. 18, Number 2, P109,1995


3. A. Mawer, S. Bolton and E. Mammo, “Plastic Ball Grid Array Solder Joint Reliability Considerations’, Proceedings of the 1994 Surface Mount International Conference, P239, 1994.


p 57-62


DOI: 10.1361/cp2000istfa057


Data Analysis Tools and Methodologies for Quick Yield Learning in a High Volume Manufacturing Environment


L. Andrade, T. Taylor


White Oak Semiconductor, Sandston, VA, USA


High volume products in manufacturing require fast yield learning, root cause identification, and verification that process or tool problems are fixed.


Yield losses of 1% correspond to very large dollar losses. Therefore, it is important to have sophisticated data analysis tools that handle large volumes of data to drive higher yields. This paper will present our methodology for defining yields,assessing wafer yield signatures, and using data analysis tools to determine tools or processes which drive yield loss. A SAS based data analysis tool will be shown which can identify tool or process related problems causing abnormalities in parametrics and impacting yield. Case studies illustrating the usefulness of the tool are shown for a Synchronous Dynamic Random Access Memory (SDRAM)product from our wafer fab. In the final analysis, it is clear that an efficient data analysis approach utilizes resources most effectively and pinpoints yield problems with minimal cycle time.


In a high volume memory manufacturing environment, small yield losses can result in large dollar losses. A five percent loss for one hundred wafers (for example 500 die per wafer and 25 wafers per lot) would be a loss of 2500 die and $25,000 if the selling price were $10 per die. Most memory manufacturers have thousands of wafers started each day so the loss can quickly multiply on a daily basis.


Clearly, fast analysis turnaround is vitally important to the bottom line.


The traditional failure analysis approach to problem solving has always been to analyze failures having similar signatures on a limited sample of devices.


Detailed analysis requires a lot of failure isolation by liquid crystal, emission microscopy, probing, or other isolation techniques.


To minimize yield and performance losses, it is vital to have highly targeted data and failure analysis for quick feedback to process engineering for root cause


solutions. Data analysis must be based on the volume of the product, and should be directed at the main yield limiting mechanisms (in priority order) for a statistical yield analysis approach. Single chip analyses without a big picture approach are a waste of product engineering and failure analysis resources and main yield limiters remain unresolved or are delayed. Hundreds of wafers may process over a short period of time through a bad tool or be affected by a process marginality while Engineering works on non-relevant or less important issues.


Sometimes the physical failure analysis process is only needed to help develop the root cause solution since action on tool or process related issues can be taken based on the available data (such as shutting a tool down which has low yield). This paper provides details on how an effective data analysis approach can be used to solve problems in a timely manner.


Wafer yield definitions, regional definitions,compressed bitmap data, and various data types will be used to pinpoint causes of failures. Several case studies will show how effective the data analysis can be and how identification of problems from open contacts to misalignment can be resolved.


Yield Definitions and Tool Description


There are a wide variety of tools available for data analysis. Some of the more traditional tools include software packages such as Microsoft Excel and JMP.


Generally, this software is adequate for many analysis tasks; however in a typical manufacturing environment, the amount of data that must be analyzed may exceed 1 million records. Most traditional analysis packages have difficulty handling the large datasets required for volume analysis. As a result, the data analysis tools, which were created at White Oak, are based on a SAS software package.


SAS software is capable of handling large datasets.


Additionally, programs (SAS scripts) may be written to automate many standard analysis tasks, such as yield or parametric analysis by tool. However,before the full advantage of the tool may be realized it is necessary to set up a proper data foundation.


The data components to successful yield analysis are proper definitions for yields, wafer regions, and test fail counts [1]. Proper yield definitions facilitate failure isolation. For example, yield may be divided into various sub yields such as DC, functional, test sequence yield 1, and test sequence yield 2. A test sequence yield bucket consists of a series of similar tests lumped together to produce a product yield. For example, a test sequence yield bucket could consist of a subthreshold leakage test, a retention test, and a signal margin test. Additionally, wafer regions may be used to further partition each yield. Examples of regions include concentric rings, quadrants or wafer halves. Once these categories are created, it is a simple matter to isolate a yield loss mechanism by identifying the sub yield category and wafer region impacted.


Background


The following section presents general background information on trench memory cell technology and product test and characterization of SDRAMs.


Memory Cell Technology


Figure 1 shows a cross sectional view of a trench memory cell. The memory cell consists of an array transistor and a trench capacitor. The array transistor is used to control access to the capacitor, and the charge is stored in the storage node. Critical issues in the yield and performance of the product are cell capacitance and off state leakages. Capacitance is a key factor in cell signal strength and should be as high as possible within limits of the designed chip size. In trench capacitor technology, the depth and critical dimensions of the trench as well as traditional factors such as dielectric material and thickness determine the trench capacitance.


Leakage currents should be as low as possible to maximize cell data retention performance. Retention time is defined as the period a memory cell may hold a charge without requiring a data refresh cycle.


Examples of leakage mechanisms, which influence the retention performance of the cell, are transistor subthreshold leakage, node dielectric leakage, and pn junction leakage.


Every modern semiconductor fabrication line must control subthreshold (sub Vt) leakage mechanisms.


Sub Vt leakage may be defined as the off state leakage current flowing from the capacitor to the bitline [2]. Gate length, oxide thickness, and gate to trench alignment are manufacturing controllable factors that impact sub Vt leakage.


WL


BL


Gate


①


②


③


P-Well


Capacitor


Figure 1 Trench Memory Cell. 1- subthreshold


leakage, 2- pn junction leakage, and


3 node dielectric leakage.


Electrically, all parameters mentioned above enhance leakage current by shifting the threshold voltage to a lower level. Lower gate length, thinner gate oxide and increased misalignment (reduced effective linewidth due to gate to diffusion overlap) result in a shift in the Vt curve (figure 2). A shift from Vt1 to Vt2 has the effect of increasing transistor subthreshold leakage. For a typical memory cell, this enhanced leakage effectively reduces the cell retention time.


Log Ids


Vgs


Vt1


Vt2


Figure 2 Transistor drain current vs. gate voltage characteristics. The arrow at 0 Vgs shows the increase in sub Vt leakage for a shift from Vt1 to Vt2.


Test and Characterization


To prevent leaky chips from reaching the customer,most facilities have developed retention and sub Vt leakage tests to screen out suspect chips. A standard retention test writes a “1” to the cell, waits a specified period of time, and reads the data from the cell to determine if the stored charge has leaked from the cell during the retention pause. A standard sub Vt leakage test works by writing a “1” (high voltage)into the memory cell. The drain voltage is bumped low, placing the maximum source drain voltage across the transistor, and this potential is held for a minimum retention time. The information in the cell is read and compared to an expected value. High sub Vt leakage will cause the data to flip from a “1” to a“0”. If the number of failing cells generated by either of these tests is above the redundancy limit, the device will be rejected as a failure.


Case Studies


Three case studies are presented which illustrate the use of effective data analysis: a) contact opens at the edge of the wafer, b) low trench capacitance on individual trench etch tools, and c) lithography alignment and process sensitivity for good memory array device subthreshold leakage performance.


Contact Opens


Case study 1 highlights the use of regional yield by tool to isolate a DC fail. Low DC yields began lowering the full specification yield. The first step in the analysis was to recognize from the compressed bit maps that many lots showed low DC yields in the


Open contact


edge region of the wafer (figure 3).


M2 to Ml


Figure 3 Compressed Fail Bit Map showing DC


fails at the notch edge of the wafer.


Using the SAS Yield by Trend tool, DC yield in the edge region of the wafer was plotted for various etch process steps. A negative yield trend was observed


on one etch tool at the M2 to M1 contact (C2 contact)etch process (figure 4).


DC Yield by Tool by Process Date


Process Date


Figure 4 Edge region DC yield trend by C2 etch tool trended by process date. The top lines in the chart show the yield for each tool and the lower lines show the number of lots.


Knowing that a possible cause was M2 to M1 contact(C2) opens, random isolated C2 contacts near the edge of the wafer were identified in the layout and immediately cross-sectioned. The C2 opens were verified (figure 5). The analysis was completed in less than one day. Discussions with process engineering indicated that the chamber had received a wet clean on the day of the downtrend. An additional wet clean and focus ring adjustment was performed to correct the problem and the yield recovered on the same day. Follow-ups of process changes are easy to verify by this method.


Figure 5 Open C2 (M2 to M1) contact verified after layout review.


Yields


Number of Lots


Bad trend


After tool fix


Low Trench Capacitance


Case study 2 highlights the use of parametric, and yield by tool to isolate a test sequence yield detractor. Basic daily yield analysis showed lots with test sequence driven yield loss, so a yield analysis by tool was performed. A lower yielding trench etch tool was quickly identified by this method (figure 6).


Test Sequence Yield By Process Tool


Trench Etch Tool


Figure 6 Test sequence yield by trench etch tool.


Low yielding tool is highlighted.


However, lower yield by itself did not prove that the loss was purely capacitance driven; therefore, the next step was to prove that the lower yielding tool was also the tool with the lowest capacitance, so boxplots of the capacitance by tool were generated(figure 7).


Capacitance by Process Tool


Figure 7 Capacitance by trench etch tool. Low yielding tool in figure 6 is also the lowest capacitance tool.


The information found was provided to etch engineering. Investigation into the bad tool showed a small trench critical dimension (CD). As a result, CD specifications were changed.


By trending yield and parametric data by tool, the yield limiting equipment was quickly found. More importantly, the integrated data provided the process engineers with information on good, medium, and bad tools. By facilitating this comparison a good tool optimization program was initiated.


Array Sub threshold leakage.


Case study 3 highlights the use of yield and fail count trends by tool to isolate a test sequence yield detractor. The motivation for the analysis was reduced test sequence yield with high fail counts for the sub Vt test. The first step in the analysis was to run test sequence yield by process tools. A difference between lithography tools was quickly found (figure 8) and confirmed by trending the test sequence yield by process date.


Test Sequence Yield by Litho Tool


Litho Tool


Figure 8 Test sequence yield by litho tool.


To verify that the subthreshold leakage test was driving the yield difference between tools, the compressed bitmap fail count data was trended by tool (figure 9). With the tool information available,wafers from the bad tool were selected for bit fail map analysis (figure 10). Bit fail map analysis showed that the fail density was higher along the edge of the reticle field and that there was an odd or even wordline dependency. This was the first indication of gate to trench misalignment.


Low yielding tool


Capacitance


Lowest


capacitance tool


Fail Count Trend by Process Date


111111111|111111111


Tool Process Date


Figure 9 Fail count trend by litho tool. Upper line is from the bad tool.


Bit Fail Map of Failing Die at Edge of Photo Shot


WL Orientation


Figure 10 Bit fail map showing wordline odd/even signature. Note that the fails are located


at the edge of the photo shot.


Physical failure analysis confirmed the misalignment mechanism (figure 11). The analysis results were fed back to the photolithograhy engineering department.


Failing cell


Gate misalignment to trench


Figure 11 SEM cross section showing gate to trench misalignment.


The data provided, focused engineering on the alignment system differences between tools. As a result of the findings, the process was shifted to the better (newer generation tools) performing tools. The yield and fail count data were tracked over time to insure that the actions taken had correctly addressed the problem.


This paper reviewed several case studies, which illustrate a precise method for quick yield analysis.


Utilization of the software tools developed for high volume data analysis has minimized or detected yield issues for hundreds of tool and process related issues.


Without these data analysis tools, many problems could not have been answered to the root cause. It was also shown that effective yield and wafer regional definitions are important in the resolution of certain types of failures and how choosing the specific yield and region on the wafer is important in the identification of a failure. Additionally, the capability to correlate parametrics, yields, and compressed bitmap fail count data by various dates is critical to understand the nature of the failure and to efficiently direct physical failure analysis activities.


Further, a volume data analysis approach can clearly show that tools or processes are performing incorrectly. Clean data analysis provides the motivation for fast corrective actions since the yield or performance impacts can be clearly demonstrated.


Fail Count


This analysis and corrective action approach results in minimal root cause and corrective action cycle times and minimizes the dollar impact of low yield events.


1. Compressed Bit fail maps for memory fail pattern classification, J. Vollrath, U. Lederer, T.


Hladschik, ETW 2000, Informal Digest, pp 207-112


2. S. Wolf, Silicon Processing for the VLSI Era Volume3 – The Submicron Mosfet, p175, Lattice Press, Sunset Beach, California (1995)


p 63-68


DOI: 10.1361/cp2000istfa063


Failure Analysis of Killer Defects and Yield Enhancement of Flat ROM Devices in Wafer Fabrication


Y. N. Hua, Z. R. Guo, L. H. An and Shailesh Redkar


Chartered Semiconductor Mfg Ltd, Singapore


In this paper, some low yield cases in Flat ROM device (0.45 and 0.6 um) were investigated. To find killer defects and particle contamination, KLA, bitmap and emission microscopy techniques were used in fault isolation. Reactive ion etching (RIE) and chemical delayering, 155 Wright Etch, BN+Etch and scanning electron microscope (SEM) were used for identification and inspection of defects. In addition,energy-dispersive X-ray microanalysis (EDX) was used to determine the composition of the particle or contamination. During failure analysis, seven kinds of killer defects and three killer particles were found in Flat ROM devices. The possible root causes,mechanisms and elimination solutions of these killer defects/particles were also discussed.


In wafer fabrication, line process, yield engineering and failure analysis engineers work together to provide high yield wafers. In this yield enhancement project, some low yield cases for Flat ROM devices have been studied. We not only greatly improved the yield of Flat ROM devices in wafer fab, but also developed and improved failure analysis techniques.


To find killer defects and particle contamination,KLA, bit-map and emission microscopy techniques were used in fault isolation. Reactive ion etching(RIE) and chemical delayering, 155 Wright Etch, 152 Secco Etch and BN+Etch and scanning electron microscope (SEM) were used for identification and inspection of defects. Energy-dispersive X-ray microanalysis (EDX) was used to determine the composition of the particle or contamination. In failure analysis, seven kinds of killer defects were found in Flat ROM devices. They are: silicon crystalline defect on silicon substrate, BN+line breakdown defect, BN+line opening defect, missing contact defect, poly bridging defect, metal bridging


and metal filament defects. We also found three kinds of killer particles, which are referred to as a phosphorous particle, a BPSG/BPTEOS crystal particle and a silicon oxide particle.


In this paper, we will introduce the failure analysis techniques used to identify these killer defects and particles. We will also include the details of failure analysis results. The possible root causes of these killer defects/particles, mechanisms and elimination solutions were also discussed. The failure analysis methods and results reported in this paper will in turn be very good reference materials to other wafer fabrication.


In this study, SEM and EDX analyses were carried out with 5 kV electron beam voltage, spot size 3 and 10 mm working distance using Philips XL 30 FESEM(field emission scanning electron microscope).


A lithium-drifted silicon EDX detector was used. It is mounted at the left rear corner thus resulting in an azimuth angle of 45°. The calibration energy scale of the spectra was performed by using Al/Cu samples at their respective Kα peaks (Al Kα line 1.486 keV and Cu Kα 8.040 keV) with 5000 counts.


Failure Analysis Results of Killer Defects


In this project, some low yield cases in Flat ROM device (0.45 and 0.6 um) were investigated. After performing failure analysis on the low yield wafers,seven kinds of killer defects were found in the Flat ROM devices, which are referred to as silicon crystalline defect, BN+line breakdown defect, BN+line opening defect, missing contact defect, poly bridging defect, and metal filament defect and metal bridging defect. All of these killer defects have resulted in low yield.


This paper describes a technique for preparing TEM samples from failed bumps. The technique is a combination of standard metallurgical polishing and FIB lift out (L/O) techniques for investigating failure mechanisms of flip chip bumps. With this technique,site specific samples were prepared for TEM analysis,which provided an important clue for understanding a cause of the flip chip device failure.


Fabrication Process


Figure 1 A schematic of a solder bump assembly showing various metallization layers in a flip chip


device structure used in this study.


Figure 1 is a schematic view showing the crosssection of a flip chip contact, which is connected through a solder bump and under-bump metallization(UBM) layers. On the silicon wafer side, an 80μmdiameter via-opening was patterned for the Al contact-pad. The multilayer UBM, consisting of chromium (a glue layer to Al), chromium-copper alloy, copper, and a flash of gold (Cr/CrCu/Cu/Au),was then deposited sequentially by sputtering,followed by evaporating the high-Pb solder(95Pb/5Sn) layer. Bumped wafers were fluxed and reflowed at ~340°C to shape the solder bumps. Flux was then chemically removed from the wafers. The wafers were film-frame mounted and diced.


Separated, high density bumped chips were dipped into no-clean tacky flux and placed onto organic bismaleimide triazine (BT) build-up substrates, where the flip chip pads were coated with a eutectic(63Sn/37Pb) pre-deposit solder. The units were reflowed at 220°C in nitrogen ambient to form the flip chip joints. The chip-to-substrate gap was then filled with an underfill epoxy. No heat spreader was used in the construction of these samples.


Samples for Accelerated Reliability Tests


Table 1 Flip chip samples used for stressing tests


|(Å) Hours |Copper Thickness |Copper Thickness |Copper Thickness |Tests |
|---|---|---|---|---|

|(Å) Hours |1.5K |6k |10k |Tests |

|1000 |X |||HTOB |

|0 |X |X |X |HTS |

|300 |X |X |X |HTS |

|600 |X |X |X |HTS |

|900 |X |X |X |HTS |

|1200 |X |X |X |HTS |

A listing of the samples subjected to reliability testing followed by analysis is given in Table I. Two types of accelerated tests were conducted here: (1) hightemperature (150°C) stressing with the operating bias of 5 volts (designated as HTOB) and (2) highSilicon


temperature (150°C) stressing without a bias (HTS).


Passivation


Aluminum (Al)Three Cu thickness values (1.5k, 6k and 10kÅ) in the


Base Metal


Cr/CrCu/CuUBM were used in this study. Samples in Table I had


UBM


5Sn95Pb


Solder Joint


bump heights of 62μm. An additional set of samples Gold (Au)with the same parameters above was studied for


Flip Chip Pad


Nickel (Ni)


Solder Mask


Copper (Cu)100μm height.


Substrate


C-SAM Examination


This investigation begins with failed HTOB samples aged at 150°C with a 5 volt bias for 1000 hours. The Cu thickness was 1.5KÅ. Defective flip chip bumps were identified in C-SAM images. Most of the flip chip bumps in figure 2 are defective, because the white color indicates a loss of acoustic signals penetrating through these bumps. In contrast, a good device, which passed 85°C/85RH @ 5volt bias reliability test, exhibited no change or loss in signal at the bumps. Figure 3 shows a C-SAM image of such a device, where solder bumps are seen as black circles.


Figure 2 CSAM showing loss of signal in bump regions after exposure to 1000 hours of 5 volt bias at 150°C (HTOB).


Figure 3 C-SAM image representative of good bump regions after exposure to 1000 hours of


5 volt bias at 85°C/85%RH (THB).


As assembled, unstressed samples were imaged by CSAM to verify sample integrity. No delaminations such as die/underfill and underfill/substrate were observed. Scanned flip chip bumps appeared very well defined in the images with a very uniform contrast. For this study a 50 MHz transducer in pulse echo mode was used. In another study, a correlation between pulse echo CSAM images and flip chip contact integrity is established [1].


Optical and SEM analysis


Cross-sections of degraded bumps were prepared by potting these samples in a slow curing epoxy.


Standard metallurgical polishing techniques were employed to polish these samples. For this study, the cross-section samples of failed flip chip devices were prepared by cutting through a whole row of solder bumps.


During optical examination, voiding was observed at the UBM region of the bumps correlating to electrical failure. Further investigation with an SEM verified the presence of a dark irregular layer at the UBM interface characteristic of defective solder bumps.


The coverage and thickness of the dark defective layer was not uniform, varying even within one row of solder bumps. Figure 4 (a, b, c) shows SEM images of bumps, with different levels of degradation,from the same row of a HTOB failed sample.


(c)


Figure 4 SEM images from the same row of bumps with varied levels of degradation after HTOB test (a)a good bump (b) partially degraded bump (c)degraded bump.


In support of the idea that the interfacial void was a probable cause for the solder bump failure, it was further speculated that the void was electromigrationinduced, because the devices were tested with the application of the 5-volt electrical bias. Flip chip samples stressed by the unbiased HTS tests, however,also failed after a similar period of time and also contained a dark layer similar to those observed in the HTOB tested samples. From this finding, therefore, it was concluded that the formation of the dark layer present at the solder/UBM interface is not induced by the electromigration process but by the thermal diffusion process. Based on this conclusion, most of the samples were stressed by the HTS test, as seen in Table 1.


More detailed high-resolution SEM examinations of the dark void-like layer, however, revealed that the layer was not voided but was actually filled with an unknown material. In the beginning, it was thought that during sample preparation, polishing debris was deposited into the voids. Energy dispersive X-ray spectroscopy (EDX) analysis was used to determine the chemical composition of the dark layer, and the presence of Cr was verified. When the electron beam is moved from solder regions to degraded regions, the X-ray count rate decreases relatively, which indicated a lower density material.


Figure 5 X-ray mapping from the degraded region of


the UBM showing Cr concentration at


the degraded region.


A two-dimensional elemental x-ray map of Cr also confirmed that Cr atoms were distributed uniformly within the black layer. It is also noted that this Cr layer was unexpectedly thick, ranging from 1 to 3μm.


This is much greater than the thickness of the deposited Cr/co-deposited Cr-Cu layer. The thick Cr layer undoubtedly represents the defective region of the solder bump joint. Without more detailed structural information, however, it was not clear why such a thick Cr layer was formed around the solder/UBM interface. In addition, the exact location of this Cr layer with respect to the UBM layers could not be ascertained by this SEM analysis.


FIB Technique


Microstructural and compositional analysis in SEM is limited by spatial resolution. The thicknesses of degraded regions at the UBM were non-uniform and varied between bumps (Fig. 4) as well as within the same bump. We needed to make a site-specific TEM sample to analyze defective region of the failed bump. Preparation of a TEM sample of a degraded region from a bad bump was a challenge. Crosssection TEM samples used in this study could not have been made by the conventional procedure.


An FEI FIB200 was used to image, mark and make the site-specific TEM samples. A standard lift-out microscope system was used to “pluck” the TEM sample and place it on the TEM grid[2]. FIB imaging(which also mills the surface) exposed the softer material quickly. Figure 6 shows the area scanned for a long period of time using a FIB system.


Metallographically polished cross-section samples were used to identify degraded areas of failed bumps.


10 micron


Pt lines were deposited using the FIB system at the region of interest (Figure 7(a)). The Pt line not only marks the region of interest, it also protects the top surface from being milled away during the sample thinning. Subsequently, lift-out TEM cross-sections were made. Figure 7(a,b,c) shows the sequence of events. A small sample ~10μm x 10μm, was picked up and dropped on a formvar coated Ni grid for TEM analysis.


SOLDER


Voidscanned area


Figure 6 (a) FIB image showing void looking area and the milled area showing the material, and (b)


magnified region showing Cr rich area.


Using the above-mentioned lift-out technique, three types of samples were prepared and analyzed using a Philips CM30 TEM operating at 300 KV.. the samples were as follows: HTOB 1000 hr. failure,6KÅ Cu as assembled (no stress), and 6KÅ Cu 1200 hours @150°C aged sample (HTS). A couple of samples of each of the above types were prepared in order to understand the variations in the thickness of the Cr rich amorphous layer.


TEM sample


Cr rich area


Figure 7 (a) Sample locations are marked with Pt lines (b) One side of the TEM sample is milled (c)Both sides of the sample are milled and the sample is cut and ready to lift out.


TEM Analysis


To further understand the exact location and nature of the thick Cr layer, TEM cross-section samples were prepared from the same defective sample used for the SEM study. A TEM micrograph of a sample prepared from an HTOB failed device is shown in Figure 8. It is clear that the Cr glue layer grown on top of the Al contact pad layer is completely intact without any structural changes. However, there is no evidence of co-deposited Cr-Cu alloy and a Cu layer


above the Cr glue layer. A thick, highly porous amorphous layer is observed between the Cr layer and solders. The chemical composition of this layer essentially verifies the presence of Cr. This amorphous layer is formed at the degraded area and its thickness is consistent with the dark layer observed optically and in the SEM. For this sample, it is clear that the co-deposited Cr-Cu and Cu layers are


amorphous Cr


solder


Cr


Amorphous Cr completely destroyed by the HTOB testing.


Amorphous Cr


Figure 8 TEM bright field image from the degraded region showing broken amorphous Cr layer.


The crack is filled with debris.


Cr-Cu


The SEM image in Figure 9 shows the locations of prepared TEM samples from the 6kÅ Cu sample after 1200 hours of aging. At location 1 the degraded area


is thicker than location 2. Figure 10(a) is a TEM image from location 1 and figure 10(b) is from location 2. An image from sample location 1 (Figure


AI


10(a)) shows only an amorphous Cr layer, similar to the amorphous layer found in the HTOB sample. On the other hand, the image in 10(b) exhibits a codeposited Cr-Cu structure along with the amorphous Cr.


Figure 9 SEM image marked with sample locations.


Crack


or


Figure 10 (a) TEM image from sample location 1


(b) image from sample location 2 from


#2


#1.


SEM image in figure 9.


Formation of Cr Amorphous Layer


Experimental results proved that there is no voiding in the solder and that the UBM / solder interface is obviously degrading and weakening after thermal aging. An amorphous layer between the UBM and solder is the weak interface. During mechanical


grinding and polishing, it is damaged and has a voidlike appearance. TEM results verified that Cr-Cu codeposited and Cu layers are completely destroyed by the HTOB stress test. Copper is known to react readily with Sn at ambient temperatures[3][4]. It is thus reasonable to assume that the Cu atoms diffused out of the Cr-Cu/Cu layers to react with the Sn component of the solder, leaving Cr atoms behind.


Since the diffusivity of Cr atoms at 150°C is extremely small, the Cr atoms will not rearrange to form the crystalline body centered cubic(bcc) Cr phase. As a result, the observed porous [5]amorphous Cr matrix was left behind. Although the amorphous nature of Cr could be reasonably explained by the above argument, it is still unclear how such a thick (1~3μm) Cr layer was formed.


The increased thickness of the amorphous Cr layer is considered to originate from the introduction of high porosity in the layer, especially along the film thickness direction. In other words, the Cr layer has been stretched along the thickness direction by a tensile stress present in the solder bump joint. In our flip chip assembly, one of the main sources for the tensile stress is considered to originate from the CTE mismatch between the Si chip and the organic substrate. Consequently, the solder joint will be always under stress. Thermally stressed bumped silicon samples, before substrate attachment, do not show an amorphous Cr layer at the UBM[5]. It is clear that the internal stress in the joint plays a crucial role in the formation of the amorphous Cr layer. The tensile stress can create excess vacancies as well as voids in the Cr layer, as evidenced by the high porosity in the Cr layer. These excess vacancies and voids will promote the out-diffusion of Cu atoms and serve as a rapid diffusion path, respectively. This stretching was further indicated by a striation formed inside the Cr layer, which was directed along the film thickness direction (see Figure 10).


Effect of Copper Thickness and Solder Bump Height on Degradation


It is important to mention that the thickness of the pure Cu used as part of the UBM layers was found to affect the thickness of the amorphous Cr layer significantly. So far, all the examples were given for the case of the 1.5kÅ thick pure Cu layer of the UBM. Two other Cu thickness values of 6k and 10kÅ were also tested under the same experimental conditions (Table I). In the case of the 6kÅ thick pure Cu sample, which was stressed for 1,200 hours,the sample did show a similar amorphous Cr layer after the 1,200 hour HTS stressing. The thickness of the amorphous Cr layer was, however, much less


(0.1~1μm) than that (2~3μm) of the 1.5kÅ thick Cu sample. In the case of the 10kÅ Cu sample, the amorphous Cr layer was observed but it was discontinuous. The thicker Cu apparently reduced the thickness of the amorphous Cr layer.


The solder bump height was also found to affect the formation of the amorphous Cr layer. An increase in the bump height from 62 to 100μm for the 1.5kÅ thick Cu sample reduced the degradation. This improvement can be attributed to the reduced overall atomic concentration of Sn in the solder, due to the larger volume of the 95Pb/5Sn solder inside the taller bump, attached to the same volume of eutectic solder on the substrate pad.


From the effect of both the Cu thickness and the bump height, it is clear that the extent the amorphous Cr was formed depends on the amount of Sn available for Cu to react. In other words, the relative concentration ratio of Cu to Sn is an important controlling factor that determines the ability to form the amorphous Cr layer at the UBM. The use of thicker Cu in the UBM tends to prolong the life of the flip chip devices during the HTS testing, because excess Cu atoms delay the out-diffusion of the Cu atoms from the Cr-Cu co-deposited layer.


Striations or streaks can be seen in TEM images(Figure 10). Due to the stress this very porous layer gets stretched and an amorphous Cr layer forms. In addition, the Sn concentration is much higher in the studied samples due to the presence of eutectic solder on the substrate contacts. The presence of a porous and amorphous layer at the UBM/solder interface is the weakest link and that is where the interfacial properties degrade and the breaking of the interface starts. Detailed microstructural analysis of the amorphous layer will be discussed in another publication


However, out-diffusion of Cu and formation of the Cr amorphous layer could be typical to the structure we analyzed and could be specific to our process [4].


Also, it is possible that with a different deposition recipe for the Cr-Cu layer, failure mechanisms may be different.


This study has developed a sample preparation technique for the examination of specific failing flip chip bumps by TEM inspection. The use of this technique allows us to make site-specific samples for


TEM study, and the analyzed micro-regions can be correlated t o the overall structure of the sample.


In addition, we studied the reliability of 95Pb/5Sn solder bumps evaporated onto sputtered layers of Cr/CrCu/Cu/Au as the UBM. Electrical continuity of thermally stressed samples was first evaluated using scanning acoustic microscopy. Samples failing the continuity test were then cross-sectioned and examined by both optical and scanning electron microscopes. The failed samples were found to exhibit a thick highly porous amorphous Cr layer at the UBM region, which was thought to be responsible for the continuity failure. The presence of a porous and amorphous Cr layer at the UBM/solder interface is considered to represent the weak link where the interfacial properties degrade and breaking of interface starts.


The authors wish to thank to R. Deshmukh and D.


Werder for their valuable discussions and Debbie Yencho for the SEM analysis. We also appreciate Harry Scholz for his support and encouragement.


1. K. Wolf, T. K. Hooghan, M. K. Bachman, R. J.


Weachock, IEEE/ECTC Proceedings, 50, 633-640 (2000)


2. L. A. Giannuzzi, J. L. Drown, S. R. Brown, R. B.


Irwin, F. A. Steve, Mater. Res. Soc. Symp.Proc.,480, 19, (1997)


3. Alan J Mocker, Peter J. Goodhew and Elizabeth A Logan, Mat. Res. Soc. Symp. Proc., 323, 131-136 (1994)


4. Michael J. Sullivan, Mat. Res. Soc. Symp. Proc.,515, 55-66 (1998)


5. Don Werder, Lucent Technologies, personal communications


p 49-54


DOI: 10.1361/cp2000istfa049


X-Ray Tomography for Electronic Packages


Next generation assembly/package development challenges are primarily increased interconnect complexity and density with ever shorter development time. The results of this trend present some distinct challenges for the analytical tools/techniques to support this technical roadmap.


The key challenge in the analytical tools/techniques is the development of non-destructive imaging for improved time to information. This paper will present the key drivers for the non-destructive imaging, results of literature search and evaluation of key analytical techniques currently available. Based on these studies requirements of a 3D imaging capability will be discussed. Critical breakthroughs required for development of such a capability are also summarized.


The driver in nondestructive imaging is the need for sub-micron (ideally <0.1 micron) resolution of defects in both x/y and z directions for multi-layer polymer/metal boards. Examples of the critical defects driving this capability improvement include printed circuit board dielectric cracking, BGA solder fatigue cracking, underfill delamination and C4 defects such as solder bump defects (bump fracture &fatigue, voids and non-wet bumps) resulting in electrical opens and shorts. In order to address this capability gap it was identified that the standard assembly imaging techniques of x-ray radiography/tomography need to be extended into the next generation. Results of extensive literature and vendor surveys will be presented to discuss the capabilities of the techniques currently used and the capabilities of the other techniques available but not currently used in microelectronic packaging failure analysis.


For x-ray techniques, goals of 1 micron maximum spatial resolution and z-axis resolution with geometric magnifications of >1000X appear to be attainable based on theoretical specifications from several wellknown vendors in the industry. The trade-offs are reduced spatial resolution and poor contrast with increased penetration capability. Examples of current x-ray radiographic capabilities for observation of the defects in the C4 bumps in a BGA package surface mounted to a PC board will be presented. The use of a transmission signal for standard x-ray radiography(2D-imaging) precludes viewing subtle defects such as C4 bump fatigue and BGA solder ball fatigue in the multi-layer interconnect packages. Thus a 3Dimaging capability is a requirement. Moore and Hartfield have concluded that the Scanning Acoustics Microscopy (SAM) technique is better than the 2D x-ray radiography for detection of underfill delamination and open ball joints.* This paper will demonstrate that the use of 3D x-ray tomography imaging technique will offer a distinct advantage over other non-destructive imaging techniques.


The initial evaluation process included investigation of several techniques including techniques that are non-standard in the microelectronics industry. Based on these evaluations, literature surveys and discussions with Oak Ridge National Laboratories(ORNL), 3D X-ray Tomography was identified to show the most promise. Results of these investigations will be presented.


Key Defects in Multi-layer Packages


Typical defects observed in Flip Chip packages and multi-layer organic boards are shown in Figure 1 and 2 and consist of delamination, cracking and voids in interconnects and polymer composites. The analytical challenge is to expeditiously locate and understand the characteristics of these defects with a high success rate.


Some explicit examples of interconnect failures are presented in Figures 3-6. Figure 3 illustrates dielectric


cracking under the metal pad or “pad cratering”, a typical defect of interest in metal defined printed circuit boards (PCBs). There is an inherent propensity to crack from the outer perimeter of corner BGA pads due to distance from neutral point stress effects. The crack can initiate as a result of delamination of the PCB dielectric from the copper pad and propagation occurs into the underlying dielectric layer as seen in Figure 3.


The solder mask defined pad leads to a re-distribution of stress that changes the fail mechanism from cratering to solder joint fatigue.*, *An example of such is provided in Figure 4. Subtleties like the extent of overlap of the solder mask, pad size/opening in the solder mask and ball size contribute to propensity for joint fatigue which is another fail mechanism that needs to be detected as efficiently as possible.


If there are board pad chemistry issues resulting in reduced adhesion, the stresses will manifest themselves as solder ball opens. This is yet a third fail mechanism of interest that is illustrated in Figure 5.


Another failure mechanism most commonly observed is delamination between two metal layers in advanced PCBs. This mechanism is illustrated in Figure 6.


Ideally, we would like to visualize all these defects non-destructively using next generation imaging tools.


DieEpoxy Underfill


Solder Bumps


Solder ball geometry and defects


Organic Substrate Voids in the underfill


Acc.V Spot MagnDet WDom=200 μm


Bump fracture/fatigue Underfill delamination


detection


at each interface


Shorts between bumps


Defects in Flip Chip interconnections


Figure 1 Typical defects in Flip chip interconnections that can be characterized by non- destructive imaging techniques


Defects in Multilayer Organic boards


dielectric


Core(epoxy +glass fibres)


Cu plated through


hole


Adhesion of via


Lands for BGA attach


Defect in the dielectrics solder bond pad


solder resist


cracks through the layers


Delamination at interfaces


Cracks in plated


through hole


Figure 2 Typical defects in the multi-layer organic substrates for which fault isolation and defect characterization techniques are required.


Figure 3 Substrate insulator cracking around BGA land resulting in a crater under the metal pad and subsequent electrical opens.


Figure 4 Solder Ball Fatigue in the solder mask defined land after thermo-mechanical stressing of the


BGA resulting in electrical opens.


Figure 5 Solder ball lift from metal land resulting in electrical opens.


Figure 6 Optical micrograph showing metal to metal delamination in a multi-layer printed circuit board


substrate resulting in electrical opens.


Drivers


The driver for nondestructive imaging is the need for sub-micron (ideally <0.1 micron) resolution of defects in both x/y and z directions for multi-layer polymer/metal boards. The standard assembly imaging techniques of acoustics and x-ray radiography/tomography need to be extended into the next generation. Table 1 presents the current capabilities of the techniques extensively used while Table 2 discusses the capabilities of the other techniques available but not currently used in microelectronic packaging failure analysis. It is clear from these two tables that the capabilities offered by the current techniques do not meet the requirements posed by the drivers identified.


NEC-Niigeta FACR3605-J630 10/7799


BallF21.nonvvet


Current X-ray Radiography Capability


For x-ray techniques, goals of <1 micron spatial resolution and z resolution with geometric magnifications of >1000X appear to be attainable based on theoretical specifications from several wellknown vendors in the industry. The trade-off is between spatial resolution and penetration capability.


Ideally the kV range should be 10-225 or more with maximum possible current to allow penetration through the thermal solutions attendant to high performance packaging. In addition, there should be good contrast resolution; i.e. 256 grey/color scale and complete image manipulation capability such as filtering, density plots, multi-image layout, 2D/3D imaging and rotation. Figures 7 and 8 show current x-ray radiographic capabilities for observation of the defects in the C4 bumps in a BGA package surface


Hilach FACR3807-J67910/4/98 land H4-2B-3B via


mounted to a PC board. From these images it is clear that presence of multi-layer interconnects greatly limits the imaging of defects.


Table 1 Currently used techniques, their capabilities and required capability to meet the imaging needs of the next generation packaging.


|Driver ||Current Capability |Current Capability |Current Capability |Required Capability |
|---|---|---|---|---|---|

|||Acoustics |Optical |X-ray ||

|<1 μm |X/Y |>75 μm |1 μm |8 μm |<1 μm |

|defects |Z |<1 μm |1 μm |? |<1 μm |

|in C4 & |Penetration |Good (?) |Poor |21μm of Cu |Good |

|BGA; |Penetration |Good (?) |Poor |21μm of Cu |Good |

|Multi- |Defect Location |Some |None |None |Good |

|layer |Defect Location |Some |None |None |Good |

|Thick |Defect Location |Some |None |None |Good |

Table 2 Additional techniques and their capabilities as applied to microelectronic next generation packaging.


ities as applied to microelectronic next generation packaging.


||Technique |Available Capability |Available Capability |Available Capability |
|---|---|---|---|---|

|||X/Y |Z |Penetration |

||Laser Ultrasonic |>100 μm |? |PPGA pkg. - |

||X-ray Tomography |8 μm |? |no issues 21 mm of Cu|

||Thermal Imaging |200μm |200μm |Poor |

||Terahertz |100 μm |<100mils |PPGA pkg. - no issues |

||MRI |10μm |10μm |Non-metallic materials |

Table 1 Failure Mode Categories and Attributes


|Group and category |Group and category |Group and category |Types or attributes |
|---|---|---|---|

|DQ Node |DQ Node |DQ Node |Failure due to write or read cycle |

Copyright © 2000, LSI Logic, Corp.


72


Figure 1 Depiction of bit-oriented failure's windowed template.


igure 1 Depiction of bit-oriented failure's windowed template.


|n/a |n/a |n/a |n/a |n/a |n/a |n/a |… |n/a |n/a |n/a |n/a |n/a |n/a |n/a |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

|n/a |n/a |n/a |n/a |n/a |n/a |n/a |Col |n/a |n/a |n/a |n/a |n/a |n/a |n/a |

|n/a |n/a |n/a |Pass |Pass |Pass |Pass |Col |Pass |Pass |Pass |Pass |n/a |n/a |n/a |

|n/a |n/a |n/a |Pass |Pass |Fail |Fail |Fail |Fail |Fail |Pass |Pass |n/a |n/a |n/a |

|… |Row |Row |Row |Row |Fail |Fail |Bit |Fail |Fail |Row |Row |Row |Row |… |

|n/a |n/a |n/a |n/a |n/a |n/a |n/a |… |n/a |n/a |n/a |n/a |n/a |n/a |n/a |

Data Reporting


Perl scripts and cron routines are run on a daily basis to perform the translation operations, recognize and tally the failure modes, and produce trend charts by product and process technology. Reports are linked on the internal web site so everyone can view yield and trend information as needed.


Results & Case Histories


There have been countless examples of successes for this methodology. Often, root cause analysis would have been very difficult to complete using conventional failure analysis approaches for logic chips. Several case histories for systematic failure modes are presented below.


Partial Single Column


Multiple 4Kx8 SRAM memory instances were laid out with 256 rows and 128 columns, and the column span was subdivided into groups of eight. The partial single column failure pattern was seen in the columns at the edges of these groups, particularly at the die near the edges of the reticle field. Photo emission analysis showed sites occurring near the N-well Vdd ties, but no visible defect could be seen at the sites. Scanning Capacitance Microscopy (SCM) was then used which indicated an intrusion of P-well into the N-well region, and a distortion of the N+ active region as show in Figure 2.


After investigation, it is concluded that the metal filaments were possibly due to (a) the narrow space between the two poly lines; (b) high topology and (c)insufficient metal etching. The solution to eliminate this problem is either to increase over etching of L90(metal etching process) from 100% to 135% during the metal etching process, or to increase the space between the two poly lines. However, it will result in


big integration size to increase the space between the two poly lines. Therefore, in this case, we decided to increase over etching of L90 from 100% to 135%.


After using new over etch recipe (over etching 135%), the metal filament was eliminated and the sort yield has been greatly improved.


Figure 8 SEM micrograph showed metal filament defect, which had shorted the metal lines.


Figure 9 EDX result confirmed that the filament was Al filament.


Metal Bridging Defect


Figure 10 SEM micrograph showed the metal bridging defect, which had shorted the metal lines and resulted in low yield.


Some wafers were reported to be of low yield. After depassivation using RIE, metal bridging defects were found (Figure 10). From Figure 10, it can be seen that the defect has shorted two metal lines, resulting in low yield. The defects were caused by micro-mask due to a foreign particle. Cross sectional SEM results also confirmed the particle was silicon oxide, which was being introduced during metal deposition.


Failure Analysis of Killer Particles Found


In failure analysis of Flat ROM devices, besides the above defects, we also found 3 kinds of killer particles, which are referred to as “Phosphorus particle”, “BPSG/BPTEOS crystal particle” and“Silicon oxide particle”.


Phosphorus Particle


A few Lots of wafers were reported to have low yield due to particle issue. Optical and SEM inspections showed the particles found, which had affected 1-2 metal lines (Fig 11). Cross sectional SEM showed that the particle was on BPSG/BPTEOS layer(Fig 12) with clear interface.


Figure 11 SEM micrograph showed the phosphorous particle, which had affected two metal lines.


Figure 12 Cross sectional SEMmicrograph showed that“Phosphorous particle” was on BPSG/BPTEOS layer.


EDX elemental analysis results confirmed the main elements of the particle to be O and P (Fig 13).


Therefore, this kind of particle is referred to as“Phosphorus particle”. Based on fab investigation result, the source of phosphorus element might be from the BPSG/BPTEOS layer. Therefore, it is most likely to be formed by a foreign particle from the chamber of machine during BPSG/BPTEOS densification fab process.


Figure 13 EDX result showed that high P was


detected on the “Phosphorous particle”.


BPSG/BPTEOS Crystal Particle


A few Lots of wafers were reported to be of low yield due to particle issue. Optical and SEM inspections showed the particles (Fig 14). X-SEM showed that the particle was on the BPSG/BPTEOS layer without interface (Figure 15). EDX results confirmed the contents of the particle to be the same as that detected on BPSG/BPTEOS layer. Therefore, we refer to it as“BPSG/BPTEOS crystal particle”.


After further FA and fab investigation, we found that it was formed during BPSG/BPTEOS densification process. The mechanism is that during densification,phosphorus tends to outgas from the BPSG/BPTEOS layer. However, the outgased P may sometimes condense back onto the surface of the BPSG/BPTEOS during the cooling step of densification. The condensed P may absorb moisture,grow bigger and denser during wafer storage. Once the condensed P solidified, it would be difficult to be removed by magasonic clean. It will then and become a micro-mask during BPSG/BPTEOS etch back fab process and thus causes the “BPSG/BPTEOS crystal particle” to form.


To eliminate the BPSG/BPTEOS crystal particle, we deposit a thin undoped silicon glass (USG) layer onto BPSG/BPTEOS layer before densification process. The results showed that the BPSG/BPTEOS crystal


particles were eliminated by depositing a thin USG layer before the BPSG/BPTEOS densification process.


Figure 14 Optical photo showed the


“BPSG/BPTEOS crystal particle”.


Figure 15 Cross sectional SEM result showed the


Silicon Oxide Particle


Figure 16 Cross sectional SEM micrograph showed that the “Silicon oxide particle” lay between


the WSixand poly silicon layers.


A few Lots of wafers were reported to have particle contamination. X-SEM showed that the particle lay between the WSixand poly silicon layers (Fig 16).


EDX results showed the main elements of the particle to be O and Si. After some investigation, we suspected that the particle was due to the implementation of oxide dummy clean at the poly dope sink, which cross-contaminated the production


wafers run at the adjacent bath. After taking appropriate actions, the particle was eliminated and the yield of wafers has been improved.


|0||
|---|---|

|1|洋|

||1|

||工 了|

Some low yield cases in Flat ROM device (0.45 and


0.6 um) were investigated. After performing failure analysis, seven kinds of killer defects (silicon crystalline defect, BN+line breakdown defect, BN+line opening defect, missing contact defect, poly bridging defect, and metal filament defect and metal bridging defect) and three killer particles (which are referred to as Phosphorus particle, BPSG/BPTEOS crystal particle and Si oxide particle) were found. The root causes and elimination solutions have been discussed. FA techniques used in this project such as 155 Wright Etch, BN+Etch, RIE, SEM and EDX were introduced.


The author would like to thank Dr Lau Chi-Kwan, K.


M. Tan, Bob Lee and FA personnel (Fab1 FA group)for providing technical advice and contributions.


1. Y. N. Hua and S. Y. Fong, The proceedings from the 23rdInternational Symposium for Testing and Failure Analysis (ISTFA, 97), Santa Clara Convention Center, Santa Clara, California,USA, 69-78 (1997).


2. Wright Jenkins, J. Electrochem. Soc.: Solid-state Science and Technology, 124, 757 (1977).


3. Rauh, Wacker’s Atlas for Characterization of defects in Silicon, A Part of the Wacker Tutorial Series.


4. Y. N. Hua, Studies of A New Chemical Etching Method – 152 Secco Etch in Failure Analysis of Wafer Fabrication, 1998 IEEE international Conference on Semiconductor Electronics, 24-26 November, Bangi, Malaysia, 20 (1998).


69


p 69-75


DOI: 10.1361/cp2000istfa069


Embedded Memory Analysis for Standard Cell ASIC Yield Enhancement


Cary A. Gloor


LSI Logic Corporation, Ft. Collins, CO, USA


The advances made in process technology along with system-on-a-chip capabilities have made failure analysis ever more difficult and expensive to perform. Quick product time-to-market and the required high fabrication yields demand top quality performance from the failure analysis team. In this paper we present a methodology for embedded memory analysis (EMA) which provides design,layout, and process characterization, and yield and reliability enhancement for standard cell ASIC products. The methodology takes the power of memory testing and failure signature analysis and brings it to the logic chip to accurately predict root cause defects. We also present the application tool that is used to query, bitmap, analyze, and report the data, along with numerous case histories. This process has greatly improved failure analysis hit rates and provided much quicker turn-times for process improvement feedback and customer return root cause analysis.


Memory circuits have long been known for their advantages as process drivers because they push the design, layout, and process technologies to their limits [1]. They are often more sensitive to process variations and generally reveal the yield limiting failure mechanisms. In ASIC designs, which now virtually all contain embedded memory, this methodology provides failure information on all but the back-end of the process flow which uses many layers of routing metalization. Memory failure analysis provides an enormous amount of failure signature information that can be studied to predict root cause mechanisms and evaluate cell library robustness. Both the defect location and probable process layer of the defect can be theorized. Other advantages include the ability to measure defect densities as opposed to modeling them, and even stating them spatially across a wafer. Also, in-line process defect data can be correlated to the bitmap data and killer defects can be studied more effectively.


Objectives


1. Proactive low yield analysis methodology


2. Baseline yield enhancement tool


3. Failure analysis tool for reliability studies and customer returns


4. Characterize new process / library / compiled memory offerings


5. Very high memory fault coverage with a standardized test methodology


Implementation Process


Design-For-Test


Careful planning for controllability and observability of the embedded memory is key to the success of this methodology. Several Design-For-Test (DFT)solutions are available to ensure that a full and accurate bitmap can be produced, namely the traditional through-the-pads (TTP) test vector approach, memory built-in self-test (BIST), or onboard microprocessor controlled testing. This planning is also important because the production testers are logic testers with little or no algorithmic pattern generation capabilities, and limited pattern depth storage space. Test pattern lengths can become quite long and convoluted when many large memory instances exist within the device.


Data Sampling Plans


Typically up to 30 die per wafer are logged for production devices. This gives up to 750 die per 25-wafer lot and provides a good sample size for root cause analysis. The test time overhead is usually only a few added seconds per wafer. This provides a proactive approach to yield enhancement because the data is collected and processed before a problem is even known to exist. Several variables are interactively available through the test program options to customize the data logging for any wafer or lot as needed:


1. “log_disable” is a Boolean to globally turn the logging feature on or off


2. "log_gf_enable" is a Boolean to allow logging even if a die fails a gross functional logic test pattern


3. “log_max_dpw” is an integer used to set an upper limit to the number of die per wafer that are logged


4. “log_interval” is used to control the interval at which a die is considered a candidate for logging


5. “ema_abort” is an integer used to indicate how many vectors will be logged before aborting each test pattern


6. “cassette_slot” is an integer used to further modify which dice are considered candidates.


Special wafers within the lot such as process experiments or wafers with more extensive inline process defect data collected are examples of this.


All of these variables are available as options to be modified without the need to recompile the test program. As the product mix changes over time, the sample options can be changed and tailored to each device.


Data Storage


The test pattern logging routines are custom written for each tester platform. Logging is generally done after the stress test patterns have been applied, during the functional retest application of the vector set. For test chips, thorough sensitivity analysis is also performed which includes logging both before and after stress, and also under various power supply,timing, and temperature conditions. Also, various test pattern algorithms, background data patterns, and address sequences are applied to provide good fault coverage and additional failure signature information.


Test pattern algorithms are chosen to cover a broad range of fault types including those caught by classical March algorithms [2][3] as well as retention faults. The test data is stored in an ASCII file using a custom data format. It is generally defined as follows:


1. ema,1,pattern_name,test_point,vdd


2. ema,2,fail_vector,BCD_I/O


3. ema,3,vector_count,abort_limit


The first record is written at the beginning of each test pattern that is data logged. It contains the test pattern name, a text string indicating the point in the test flow at which the data is collected, and the operating voltage for the device. The next record is repeated for each failing vector that occurs for the


given test pattern up to the vector count abort limit. It contains the failing vector and a 32-bit binary coded decimal (BCD) number representing the set of I/O pins that failed. Multiple 32-bit BCD entries are used if the observable data bus is more than 32 bits or if the logical address bus is presented as in a custom BIST implementation. The last record indicates the actual number of vectors logged and the current setting for the abort limit.


Generating the Bitmap Coordinates


The translation from test pattern to bitmap is a threestep product-specific process. First, the failing vectors and BCD number of failing I/O pins are translated to the logical addresses and data-in/dataout (DQ) nodes of the memory instance via the test pattern description. An algorithm is defined to map vector numbers to test pattern algorithm elements and the logical addresses. Next, it is converted to the physical rows and columns within the compiled memory instance via the logical scramble equations.


Finally, it is converted to memory cell positions in the bitmap via the delineation choices made for viewing multiple memory instances in a mosaic fashion. Products with over one hundred separate embedded memory instances have been bitmapped.


Probability Matrices


Several approaches are used to generate a probability matrix to translate test failure modes into probable root cause mechanisms. This is an important step in the process because of the need to classify the defects in terms of the root cause and not simply the test failure modes. Feedback to the wafer fabrication facilities depends on this information in order to help prioritize yield enhancement efforts. First, a theoretical probability matrix is developed using critical layer information from each mask step. This matrix provides a crude level of probability, usually stated as low, moderate, or high probability that a given failure mode is caused by some physical mechanism. Next, an empirical probability matrix is developed using historical failure analysis results [4].


Finally, a modeled probability matrix is developed using layout simulation tools and in-line process defect data. These three matrices are used in conjunction with each other to predict the root cause.


Application Program


Design


The graphical user interface (GUI) application program was written using C/C++, Motif X windows,and the Xmt toolkit [5], and is installed on a Unix system. It can also be run on any networked PC with an X window terminal emulator. The basic elements


71


are reading the test data file, translating the failing vector information into bitmap coordinates for viewing, and providing automatic failure mode recognition routines. Also, data filtering capabilities,graphical overlays to in-line monitored (ILM)process defect data, and data reporting tools are provided.


Failure Mode Categorization


The failure mode list consists of four groups: bit,row, and column oriented failures, plus logical blocks. The first three are further subdivided into six categories: single, double, triple, quadruple, multiple,and other. One more special category is defined: a probable row to column short. It is derived from the row and column failure modes that graphically overlay, and based upon failing logic states are actually one physical defect instead of two. These cover all of the memory cell array defect categories.


The logical block group, those that alias as errors in the memory cell array, are categorized as address buffer, address decoder, contiguous block, and DQ node failure modes. Each category is further subdivided into types. For example, single columns are divided into full or partial single columns, and address decoder is divided into row and column decoder types. The complete list is shown in Table 1.


Failure Mode Recognition


The application program contains failure mode recognition algorithms to accomplish the categorization task automatically. Various templatematching, matrix manipulation, and scan algorithms have been proposed [6]. The bit algorithm used here is a windowed template-matching scheme as depicted in Figure 1. It uses three regions around the bit in question in which to search for failing bit patterns: a two-cell perimeter fail region, next a two-cell perimeter pass region, and then the entire row and column as related cells. Row and column failure modes are determined by an algorithm that analyzes arrays that tally the fail bit count in the row and column axes. The decoder failure mode is found by searching for repeating patterns at power-of-two intervals or multiples of the number of DQ nodes.


Rules are applied in the algorithms to improve the accuracy of the defect count. For example if single bits fail adjacent to a single column it is considered one defect and classified as a single column with related bits. Many other pieces of information are used to generate the complete failure mode signature such as fail logic state, fault type, logical address,power supply dependence or sensitivity, write vs.


read cycle behavior, defect density and distribution across the wafer, and IDDQvalues.


|Single Bit |Single Bit |Single Bit |(X;Y) is Even/Even, Even/Odd, Odd/Even, or Odd/Odd location |

|Double Bit |Double Bit |Double Bit |Contiguous, alternate, or other spacing. Row, column, or diagonal orientation. |

|Triple|Triple Bit ||“I”, “L”, or other shape |

|Q uad|Quadruple |Bit |“I”, “L”, “T”, or other shape |

|Multiple Bit |Multiple Bit |Multiple Bit |Fail bit count |

|Other Bit |Other Bit |Other Bit |Fail bit count and aspect ratio of failing region |

|Single Column |Single Column |Single Column |Length of full, half, quarter, etc. |

|Double Column |Double Column |Double Column |Length of full, half, quarter, etc. |

|Triple Column |Triple Column |Triple Column |Length of full, half, quarter, etc. |

|Quadruple Column |Quadruple Column |Quadruple Column |Length of full, half, quarter, etc. |

|Multiple Column |Multiple Column |Multiple Column |Length of full, half, quarter, etc. |

|Other Column |Other Column |Other Column |Length of full, half, quarter, etc. |

|Single Row |Single Row |Single Row |Length of full, half, quarter, etc. |

|Double Row |Double Row |Double Row |Length of full, half, quarter, etc. |

|Triple Row |Triple Row |Triple Row |Length of full, half, quarter, etc. |

|Quadruple Row |Quadruple Row |Quadruple Row |Length of full, half, quarter, etc. |

|Multiple Row |Multiple Row |Multiple Row |Length of full, half, quarter, etc. |

|Other Row |Other Row |Other Row |Length of full, half, quarter, etc. |

|Row(s) and Column(s) |Row(s) and Column(s) |Row(s) and Column(s) |Fail logic state at intersection |

|Address Buffer |Address Buffer |Address Buffer |Row, column, or multiplexed buffer |

|Address Decoder |Address Decoder |Address Decoder |Row or column decoder |

|Contiguous Block |Contiguous Block |Contiguous Block |Fail bit count, and fail bit density |

Double Column


A double column failure mode was seen exclusively on even/odd pairs of columns on die near the edge of the wafer as shown in Figure 3. This suggested that the failure mode was not in the memory cell array but probably in the decode or sense circuitry instead. The physical layout of the metal 2 bit lines had a metal 2 Vss bus between them yet electrical microprobing showed a


short between one column's bit line and the neighboring column's bit line. This focused the search on the column decode circuit, and the defect was found to be an active bridge at a minimum space location as shown in Figure 4.


Memory Rings


Another failure mode was dubbed “memory rings”.


This was a bit-oriented failure mode that caused up to a hundred or more bits to fail in a donut shape as shown in Figure 5. Transistor measurements showed elevated threshold voltages on both P-channel and Nchannel transistors in an affected area. Initial SEM cross-sections did not show any problem so Atomic Force Microscopy (AFM) was performed which showed a 50 nm change in film thickness in the ring.


In-line monitored process defect data was then collected at the suspected gate oxide process step and overlaid to the bitmap with excellent correlation as shown in Figure 6.


Partial Single Row


A final example was a Partial Single Row (PSR)failure mode. The failing row was observed to always be at an odd address, and up to 64 bits in length within the row span of 256 bits as shown if Figure 7.


It had a higher failure rate near the center of the affected wafers, was low voltage sensitive, and had a slight sensitivity to die location within the reticle field. The failure mode was theorized to be one specific poly to metal contact in the row decoder circuit, and was the only way the observed failure symptoms could occur. Transmission Electron Microscopy (TEM) cross-sections were done on several of these failures which revealed the defect as shown in Figure 8. Close inspection of the area showed that the edge of the contact was not covered by metal 1 because of a slight misalignment. The post metal etch wet strip process attacked and corroded the metal-contact interface as reported in the literature [7].


73


3 8 8 8


8CO 8


50.0 μM 0


50.0 JUM


Data typeZ range500,0 nm


Z range1.0000u


Height


Data type


dC/du


8881


b6855-2b.22a


b6855-2b.22b


B6855,SCN Run #2, Bottom, AFM ImageB6855, SCM Run #2, Bottow, SCH Image Figure 2 AFM/SCM micrograph showing intrusion and distortion of implanted regions.


YEMA Walermas


Figure 3 Stacked bitmap view showing Double


Column failures for an entire lot.


Figure 4 An active bridge is seen near the top center of the photograph.


TTT Figure 5 A faint dark ring can be seen in this low magnification optical view of the "Memory Ring".


74


LSI Logic Corp.-EMA-dn02599w20


x


File... Setup...Filters...Data... ILM...


Help...


DIE: Vdd(min)=0,000000v Vdd(max>=0,000000v Vdd(combo)=0


Z00M


PROD.:hs112 C


人


△△


LOT:*


MAFER:20:1/1


DIE:*,*;*/10


COND.:*


BIT:(0;0)


COUNT:11/290


TRAVERSAL:


COLOR


NavToolX


<


#V


ORIENT


婪


HUSKER


N☑


CLOSE


Figure 6 "Memory Ring" failure mode with overlaid ILM data


LSI Logic Corp.-EMA-dn05499


File... Setup... Filters... Data... ILM...


DIE: Vdd(nin)=0,000000v Vdd(nax>=0.000000v Vdd(conbo)=0


ZO0M


*


NAFER:13:14/27


XNavToolx


DIE:*.*;*/24


1:1


COND.:


FI


BIT:(0:0)


COUNT:0/4242


WAFER


"


游


RS


08I3N1禁


A


HUSKER N


本18-8凌*


Figure 7 Stacked bitmap view showing PSR failures for an entire wafer


Figure 8 TEM view showing corroded metal-contact interface near the right-center of the micrograph.


Future Plans


Future development includes converting the application to a data base back-end, and moving to a PC Windows based application. Also, more work needs to be done on developing accurate probability matrices, especially using layout simulation tools and in-line process defect data.


This methodology provides powerful and proactive techniques for developing and sustaining standard cell ASIC products in the manufacturing environment using embedded memory analysis. A custom approach was chosen in order to maintain the flexibility needed in an ASIC environment, and to provide a comprehensive methodology. It emphasizes proactive data collection in the production environment and employs logic testers to gather the necessary data to fully bitmap the embedded memory instances. A sophisticated GUI application program was written to query, bitmap, analyze, and report the data. Better failure analysis hit rates, turn-times and smarter capital expenditures for equipment can be realized with this approach.


The author would like to thank Chris Eddelmann,Ron Peercy, Patrick Quinn, Gary Sommers, and David Terry for their physical failure analysis work.


Also, special thanks go to Ken Vest for the test data format specification and his invaluable guidance in Motif programming.


1. B. Prince, “Semiconductor Memories, A Handbook of Design, Manufacture, and Application”, John Wiley & Sons. Ltd.


Chichester, U.K., pg. 15 (1991)


2. A.J. van de Goor, “Testing Semiconductor Memories, Theory and Practice”, John Wiley &Sons. Ltd. Chichester, U.K., pgs. 93-170 (1991)


3. A.J. van de Goor, I.B.S. Tlili, and S. Hamdioui,


0.5um“Converting March Tests for Bit-Oriented Memories into Tests for Word-Oriented Memories”, IEEE International Workshop on Memory Technology, Design and Testing, pgs.


46-52 (1998)


4. J.M. Morrissey, H.C. Chow, R. Devries, and C.


Megivern. “An Approach to Memory Testing,Diagnostics and Analysis”. International Test Conference Digest of Papers, pgs. 56-67 (1981)


5. David Flannagan, “Motif Tools: Streamlined GUI Design and Programming with the XMT Library”, O'Reilly & Associates, Inc. (1994)


6. M. Faucher, “Pattern Recognition of Bit Fail Maps”. International Test Conference Proceedings, pgs. 460-463 (1983)


7. L.T. Koh, K.L. Chok, H.M. Li, S.Y.M. Chooi,"Titanium Corrosion in 0.25μm Metal Interconnects". IEEE International Interconnect Technology Conference, pgs. 47-49 (1999)


p 77-79


DOI: 10.1361/cp2000istfa077


Proceeding from the 26th International Symposium for Testing and Failure Analysis, 12-16 November, 2000, Bellevue, Washington


Yield Enhancement Study: Process Variation and Design Margins Leading to Timing Issues in RAM


Srikanth Perungulam, Scott Wills and Greg Mekras


Texas Instruments Inc, Stafford, TX, USA


This paper illustrates a yield enhancement effort on a Digital Signal Processor (DSP) where random columns in the Static Random Access Memory(SRAM) were found to be failing. In this SRAM circuit, sense amps are designed with a two-stage separation and latch sequence. In the failing devices the bit line and bit_bar line were not separated far enough in voltage before latching got triggered. The design team determined that the sense amp was being turned on too quickly. The final conclusion was that a marginal sense amp design, combined with process deviations, would result in this type of failure. The possible process issues were narrowed to variations of via resistances on the bit and bit_bar lines. Scanning Electron Microscope (SEM)inspection of the the Focused Ion Beam (FIB) cross sections followed by Transmission Electron Microscopy (TEM) showed the presence of contaminants at the bottom of the vias causing resistance variations.


As semiconductor integrated circuits (ICs) grow increasingly complex and minimum feature size migrates to sub 100nm levels, failure analysis is an ever-increasing challenge. The failure analyst is often not familiar with the design and layout details of complex ICs. Hence, failure analysis and yield enhancement efforts often involve a cross-functional team of designers, product engineers and failure analysts. This paper demonstrates the necessity for such a team, as well as the usefulness of failure analysis tools such as the Focused Ion Beam (FIB)and the Transmission Electron Microscope (TEM).


The paper also shows how shrinking design margins,coupled with process variations, can lead to IC failures.


Problem Statement and Failure Isolation


This case study involves failure analysis on an SRAM in a Digital Signal Processor. Sometimes,problem identification in processing complex ICs is easier using the SRAM because the failure can often be narrowed to a single cell, a set of gates, a signal line, or an interconnect. The failures on this particular device were seen across multiple wafer fab lots and got worse during testing at low temperatures and high voltage. By analyzing a failing chip using bench testing with an emulation board, the failures were isolated to columns associated with a single sense amp in the SRAM array.


To fully comprehend the problem, an understanding of the READ cycle of the SRAM is important (1). In these ICs, the READ cycle starts with the precharging of the bit lines and the sense amp by their respective pre-charge circuits. When the SRAM cell is to be read, an address is sent to the MUX circuit. The read process is timed from the address latch signal.


The pre-charged bit lines and the sense amp are allowed to float. An analog signal delayed from the address latch signal turns on the READ select transistor, which connects the SRAM bit lines of the selected cell to the precharged sense amp. At this point, the analog circuit of the sense amp starts to detect the differential voltage between the bit line and the bit_bar line. Some time later, after the READ select signal, the SENSE AMP ENNABLE (ENN)signal, which is also timed from the address latch signal, activates the second stage of the sense amp.


The voltage levels on the bit and bit_bar lines are sufficiently different at this time so that the activation of the second stage will reliably continue the separation of the voltage levels and latch the final state into the output of the sense amp.


During testing of the SRAM, words furthest from the sense amp failed first indicating that the sense amp second stage was turning on too quickly. The sense amp was not reliable in setting up the separation of the bit and bit_bar lines. Adding a delay to the ENN signal would help justify this theory.


To verify the theory, the FIB was used. A useful tool for design edits, the FIB uses a Gallium (Ga) beam(gas- assisted) to mill material (2). There is also provision to deposit conducting material such as Platinum (Pt) or insulation material such as TEOS on most modern FIBs. Using the FIB, the sense amp signal ENN was delayed by the addition of a Pt interconnect on a marginally failing column. The effect of the Pt line was to delay the fall time of the signal but not the start of the signal. The unit showed improvement but not over the complete Voltage/Temperature/ Frequency range. Increasing the resistance on the Pt line by increasing the length showed continuous improvement on multiple columns across multiple units. Simulations suggested that the sense amp design was marginal. SPICE modeling also indicated that process variations were likely to impact the bitline separation significantly.


Armed with this information, the next step was to determine what stage in the process was likely to impact these failures the most. After some investigation, the design team identified a set of metal-to-metal and metal-to-moat contacts (via 2, via 1 and contact) as likely sources of failures. An initial FIB cross section of the suspect vias showed a possible anomaly at the bottom of via 2. An FIB strap around a similar via 2 on another device showed complete recovery from failure. This experiment was repeated on four units with all units healing.


Once the failing via was identified, the next step was to perform a cross section for Transmission Electron Microscopy (TEM), a powerful tool used to obtain high resolution images at high magnifications(>100K) (3). A high energy beam of electrons passing through the electron-transparent sample forms an image on the fluorescent screen below the sample. The interactions between the electron beam and the atoms in the specimen provide the contrast in the TEM image. . This interaction results in transmitted electrons, elastically scattered electrons,inelastically scattered electrons, X- rays, and Auger electrons. The image is formed using the transmitted and elastically scattered electrons. The X-rays are used in the elemental analysis using EDX (Energy Dispersive analysis of X-Rays). The electron diffraction phenomenon in a TEM can be used to obtain information on atomic structure. The TEM work was performed using a 200Kv field emission microscope.


The most popular and efficient method for TEM sample preparation is using the FIB (4). The TEM samples for this study were prepared using the dicing saw to cut a 20um strip around the sample and then thinning it down to < 100nm using the FIB.


The TEM results showed that the Ti/TiN barrier layer is thin at the bottom of the via(Fig. 1-3). Below the thin Ti/TiN, an anomaly was identified to be a material containing (Al, F), possibly aluminum fluoride (Fig. 4), which is not a good conducting material and therefore, can cause increased via resistance. The fluorine from the WF6for tungsten deposition had penetrated through the thin barrier layer and chemically reacted with the aluminum.


Process changes to improve the chemical resistance of the Al during W deposition lead to improved contact performance. The improvements were not considered significant enough to be applied to more modern SRAM designs. A better process margin is required. Subsequent designs included two contacts in the sense amp circuit to guarantee enough conductivity to prevent sense amp marginality. The timing of the ENN signal was also changed in the design by the addition of extra gate delays.


The complexity of the modern DSP designs and the increasing amount of SRAM required in the device are leading to the need to understand the relationship between process and design. This paper clearly shows that no single applied solution is appropriate.


Although a systematic application of ATE testing,physical probing, FIB modification and TEM analysis relieved the contact resistance problem,more improvements were required to make the solution robust. Design changes to the required number of contacts per connection further improved the SRAM process margin.


To eliminate the problem of noise margin in the sense amp, additional delays were added to the design through the increased number of extra gates. This gained the SRAM design better process margin.


Finally, without the complete cooperation of design,product and failure analysis engineering the design/process marginality could not have been resolved.


We would like to acknowledge Lancy Tsung and members of the TI Kilby Center TEM facility for the TEM sample preparation and imaging work. We also acknowledge the support and assistance of Clyde Dunn with the SRAM design debug and Ron Parker for the numerous FIB edits. The authors would also like to ackowledge the contributions of the HDAO lab toward this paper.


1. Weste and Eshraghian, Principles of CMOS VLSI Design, 2nd Edition, 564 (1992).


2. K. S. Wills and S. Pabbisetty, Desk Reference,Microelec. Failure Analysis, 3rd Edition (1997).


3. Reference, Microelec. Failure Analysis, 4th Edition, 315 (1999).


4. Lancy Tsung, Adolfo Anciso, presented at ISTFA ‘98.


TEM results


0.40 μm


90.00 mm


Figure 1 Low magnification TEM image showing the failing via. The area with the anomaly is at the


bottom of the via and is circled.


Ene


Figure 3 TEM image showing the locations of the EDX data.


Figure 2 Higher magnification TEM image at a slightly defocused condition showing the contaminant at the bottom of the via.


Figure 4 EDX results showing the presence of


Fluorine below the barrier layer.


Figure 1


Fig. 3


Fig. 4


1502


ed844


Counts100


ed#


eds#3


eURA2


F


01


100.00nm


W


Fig. 2


p 81-85


DOI: 10.1361/cp2000istfa081


In-line Defect to Bitmap Signature Correlation: A Shortcut to Physical FA Results


Julie Segal, Arman Sagatelian, Bob Hodgkins, Tom Ho


HPL Inc., San Jose, CA, USA


Ben Chu, Tony Singh, Harvey Berman


Dominion Semiconductor, Manassas, VA, USA


Physical failure analysis (FA) of integrated circuit devices that fail electrical test is an important part of the yield improvement process. Unfortunately, the procedures involved are expensive and time consuming. This paper will describe how analysis of existing data from arrayed devices can be used to replace physical FA of some electrical test failures,and increase the value of physical FA results.


In-line defect inspection is performed on semiconductor product wafers at multiple stages in the fabrication process. When used for excursion detection, a spike in defect density can indicate that the previous process step is out of control, and yield may be reduced [1]. However, some defect inspection tools also record the size and location of the defects,and this information can be used in powerful ways to enhance yield diagnosis. This is especially true for memory devices or other regular arrays, either a product or yield diagnosis vehicle, where electrical bitmap results can be correlated directly to in-line defects. The key is to use classified bitmaps, and determine which signature classification correlates to which type of in-line defect. Using this technique,physical failure mechanisms can be determined for large numbers of failures on a scale that would be unfeasible with de-processing and physical FA.


When physical FA results are available, this analysis greatly enhances the value of those results. By formulating a failure mechanism hypothesis ahead of time, only a small sampling of physical FA is required to confirm the hypothesis. Alternately,knowing which signatures correlate or don't correlate to defects can help prioritize the physical FA effort.


This work was performed on Dominion Semiconductor’s state-of-the-art 128Megabit DRAM.


In this article, the discussion is limited to pre-repair results. Though most of the bitmap failures discussed here were subsequently repaired, and do not represent actual yield loss, understanding the failure mechanisms is important for improving overall yield on this and other products running in the same line.


Procedure


The procedure consists of the following steps:


1. Import failing bitmaps generated by the tester into the analysis database.


2. Import in-line defect data into the analysis database.


3. Find defect densities by layer and classification.


4. Translate position of defects into analysis database system coordinates.


5. Classify all bitmaps: identify bitmap signatures automatically.


6. Correlate in-line defects to bitmap failures (find kill ratio).


7. Correlate signatures resulting from bitmap classification to in-line defects (yield diagnosis).


Automatic Signature Classification and In-line Defect Data to Bitmap Correlation


All failing bitmaps are automatically classified according to signature categories such as single bit,single row, double row, partial row, single column,etc., and the results are tabulated. There may be more than one signature per die. The signatures are listed in Table 1. They have been consolidated for clarity in this work. For instance, row pairs, single rows failing 100%, and single rows failing from 30% to 100%have all been combined in the category “Row”.


The classification results on a sample of wafers are shown in Figures 1 and 2. All of the failing bits are accounted for; those failures which don’t fall into any other category are put in the “UNCLASSIFIED” bin.


Figure 1 shows the number of die affected by each signature, and Figure 2 shows the total number of each signature in the sample. Single bit failures stand out more in Figure 2, since some die have hundreds or even thousands of single bit failures.


Table 1 Bitmap classification signatures reported in this paper


|Column |Column fails throughout block |
|---|---|

|Column quad |4 adjacent columns fail |

|Row |Row fails throughout block |

|Column fragment |Fragment of column fails |

|Row fragment |Fragment of row fails |

|2BitCol_EO |Bit pair in a column: Even/odd |

|2BitCol_OE |Bit pair in a column: Odd/even |

|2BitRow_EO |Bit pair in a row: Even/odd |

|2BitRow_OE |Bit pair in a row: Odd/even |

|Single_Bit |Single bit fails surrounded by good bits |

|UNCLASSIFIED |Miscellaneous bit cluster |

b affectednumber of diey signature


Two-way Defect to Bitmap Correlation


Column


Row


In-line defect to bitmap correlation involves physically mapping optically detected defects to


Column fragment


quadColumn


row fragment


2BitCol_EO


2BitCol_OE2BitRow_EO2BitRow_OE


Single_Bit


UNCLASSIFIED


memory bits, which is sometimes referred to as defect overlay. The results of this correlation fall into one of four categories shown in Table 2. Figure 3 illustrates a correlated defect, in this case a row and column cross that correlates to a metal 2 defect.


Table 2 Possible outcomes from correlating optically detected in-line defects with failing bitmaps


The power of this approach comes from performing a


totalf signature occurances o number of


two-way correlation. First, we look at the optically detected defects (A in Table 2) and determine which


□Column


row fragment2BitCol_EO]2BitCol_OE


2BitRow_EO]2BitRow_OE


of these correlate to electrically failing bits. This results in a “kill ratio”, or percentage of the in-line defects which are “killers”. This analysis can be done for each process step, as shown in Table 3. For even more detail, the individual kill ratios can be established by in-line defect classification, as shown for Metal 2 defects in Table 4. In this example, a sample of defects from each layer was classified manually, but ADC results could be used as well.


Silicon Crystalline Defect on Substrate


In wafer fab process, some wafers (0.45 μm and 0.6μm FLAT ROM) were reported to have opposite major flat low yielding pattern. In the production line,similar defect patterns were detected by KLA after L20 CRS (BN+chemical resist strip). The KLA maps showed that very fine particle defects shorted BN+lines and affected approximately 10-20 % of yield.


Particles of size less than 0.3 μm were found to be accumulated near the edges of opposite flat of the wafer or, termed, “Sad-face” (Figure 1-Left side).


These particle defects were first detected after L10 nitride deposition.


In order to identify the root cause of the contamination, wafer orientation (flat up/flat down on SiC boat) experiments at twin well drive fab process were carried out. The interesting result was found that the contamination pattern changed into “Smiling face” particle defects ( Figure 1 –Right side). This result seems to drop a hint that the “Sad face”contamination may be related to SiC materials such as tube, boat and paddles used during twin well drive fab process. Some affected wafers were subjected to 155 Wright Etch, which was developed by us [1]. The procedure of 155 Wright Etch is given below:


Figure 1 “Sad-face” (Left) and “Smiling-face”


(Right) contamination were found.


Figure 2 SEM micrograph showed that the silicon crystalline defect had damaged BN+lines and resulted in low yield.


Figure 3 SEM micrograph showed that the silicon crystalline defect had damaged the BN+lines and resulted in low yield.


Preparing Wright Etch etchant → Sample preparation→ HF (49%) deprocessing for 15 mins → Wright Etch for 5 mins→ Optical and SEM inspections.


Wright Etch etchant was made by following the recipe [2-3]:


60 ml hydrofluoric acid (49%), HF


30 ml nitric acid (69-71%), HNO3


30 ml 5M CrO3(1 g CrO3/2ml H2O)


2 g Cu (NO3)2.3H2O (reagent grade)


60 ml acetic acid (Glacial, CH3COOH 99.7%)60 ml deionized water.


After 155 Wright Etch, no silicon defects were found in the clean area of the affected wafers. However,“Combined” silicon crystalline defects were found on the silicon substrate of the contaminated area of the affected wafers. The silicon crystalline defects were confirmed to be combinations of a few (100) square pits (Figures 2-3). From Figures 2-3, we can see that the defect has damaged BN+lines and resulted in low yield.


After carrying out fab investigation and further failure analysis, it was concluded that the twin-well drive tube was the cause of contamination. The “Sad-face”contamination was directly related to SiC dust contamination from the SiC materials used such as the tube, boat and paddle used for the twin-well drive processing during the diffusion process.


The solution was to use quartz tube and quartz boat or SiC boat pre-coated with a thin film of Si3N4instead of SiC tube and boat, or to use CVD SiC coated tube,boat and paddle. After taking action, the wafer yield has been increased. During this contamination issue,we also developed two new chemical etching methods for identification of the Si defects, which are 155 Wright Etch [1] and 152 Secco Etch [4].


BN+ Line Breakdown Defect


In the wafer fab, buried N+(BN+) lines are used to form the source and drain of a MOS transistor in


0.45 um Flat ROM device. Some wafers were reported to have a low yield problem. It was found that during electrical testing, there was failure on the cell transistor VT and Iread test pattern structure.


Electrical bench analysis results showed that the failure could be due to broken BN+lines on the affected cell transistor. To find out the root cause,failure analysis was carried out on the affected wafer.


To identify BN+defect, we introduced a rapid chemical etching method for the BN+lines, which was termed BN+etch. Its procedure is:


Preparing etchant → Sample preparation → HF(49%) deprocessing for 15 mins (for the completed wafers) or for 20 secs (for the L20 process wafers) →BN+etch for 5 secs→ Optical and SEM inspections.


BN+etch etchant was made in the following ratio:3 HNO3:12 CH3COOH: 1 HF (49%).


Figure 4 SEM micrograph showed that the BN+ lines had been breakdown and resulted in low yield.


After BN


南省苏水


+etch, SEM inspection results showed that


BN+lines on the cell transistor were broken (Fig 4),


which had resulted in low yield. Based on failure93 analysis and fab investigation results, it wasPLD


atrn concluded that the broken BN+lines were due toA120masking problem. After taking actions and0体市 monitoring of L20 process in the wafer fab, the BN+


line broken problem was eliminated and the yield of


wafers has been improved.


BN+ Line Opening Defect


Another kind of defect was found on the low yield wafers, which was termed the BN+ line opening defect. First, bitmap testing was performed on the low yield wafers and the defect site was located. After that, the chemical delayering and BN+etch (refer to


statement in the above section) were performed. It was found that the BN+lines on the cell transistor were opened. From Figure 5, one can see that the defect has resulted in opening of two BN+lines and resulted in low yield. After performing FA and fab investigations, it was concluded that the defects were due to micro-mask or contamination.


Figure 5 SEM micrograph showed the BN+ line opening defect, which had resulted in opening


of two BN+lines and low yield.


Missing-Contact Defect


In this case, some wafers were reported to have low yield. First, bitmap was performed on the wafers to locate the defect site, following which, delayering(using HF for 15 mins) was performed until the substrate. Optical and surface SEM inspection showed that some contacts were missing as shown by the arrow in Figure 6. This killer defect has resulted in yield loss. Missing-contact defect was most likely due to micro-mask or particle contamination.


Figure 6 Optical photo showed the missing-contact


defect, which had resulted in low yield.


Poly Bridging Defect


Some wafers were reported to be of low yield. Failure analysis has confirmed that it was not due to the silicon crystalline defect, BN+ line breakdown/opening defect and missing-contact defect, which have been discussed in the above sections.


After using bitmap to locate the defect sites, the delayering processes using dry (RIE) and chemical etches were done to delayer the wafers down to the poly layer. The poly bridging defect (Fig 7) was found, which has affected three poly lines. After analysis, we believe that it was most likely due to micro-mask or particle contamination before the poly etching processes.


Figure 7 SEM micrograph showed the poly bridging


Metal filament defect


0Ke


In this case, a few Lots of wafers were reported with very low yield. A wafer sample was depassivated using dry (RIE) etching that is made in a plasma etcher system using a mixture of CF4 and O2 gases at a ratio of 9:3. The operation conditions were with 12 mins of etching time, 180 power and 100 m Torr pressure. The main reactions in the RIE etching using CF4 for the removal of passivation are:


CF4 CF4+SiO2→SiF4+CO++ SiO2  SiF4 + CO+ and


CF4 CF4+Si3N」→SiF+CFN+


areA


+ Si3N4 SiF4 + CFN+


1D02003014.0000T00IL.OD


3 parts of O2 are added to CF4 for three reasons: (A).


O2 acts as a catalyst in this reaction; (B). The presence of oxygen avoids polymerization problem associated with gases containing high-to fluorine ratio and (C).


O2 serve as a carrier gas for the products of reaction.


After depassivation, SEM inspection results showed that metal filaments were found at the particular locations, which had resulted in metal bridging(Figure 8). EDX (energy-dispersive X-ray microanalysis) analysis result confirmed that they were Al metal filaments (Figure 9).


Figure 1 Signature classification results: number of die affected by signature


Note that there is significant variation between classifications. Some classifications (class 7) have 0% kill ratio, indicating that these classes represent“nuisance” defects. At the other extreme, there are categories (class 11) with 100% kill ratio.


||Bitmap |No bitmap failure present |
|---|---|---|

||failure |No bitmap failure present |

||Present (B) |No bitmap failure present |

|Optical Defect Detected (A) |Correlated defects |Uncorrelated optical defect |

|No optical Defect Detected |Uncorrelated electrical defect |No defect |

Figure 2 Signature classification results: total number of occurrences of each signature.


C. HPL WaferViewW_GEMINI


回x


Water yiew Rata Pones Synchronizationlools Settings Defects Help


Bx00??aappoma。心恒 Position [um)


2F2 X:


Y:


omelated NA LayerName M2 PLY Code M2_FS FMShor Bitmaps:"CorrelstedSignatures: [Col_100_quad] [Row_quad]


Die


Row:-


ColumrDevice: (none)


Water Die


Die:11:1(GEMINI)M T35RY72MEMARRAY


WTR


Defects7r3_com


all_com


cb_classified


了11_coff13


711


14


713 7m0


7m1


7m2


7cb_con17 7 kv


7kv_com18 7gc_con


7gc


N7m2 comMan


Magn 0.63


Frozen


Magn 16


7 m1_correlated4


12


11


Figure 3 Illustration of in-line defect to bitmap correlation. The center view shows defects at the wafer level, with bitmaps displayed for two of the die. The view on the right is a close-up of one of the die,


with a defect located at the intersection of the cross.


Knowledge of kill ratios is necessary to determine if


a defect level excursion indicates a real threat to


yield. Kill ratio information also contributes to


baseline yield improvement by indicating which type


of defects to reduce for greatest yield impact.


Furthermore, the kill ratios can be used to establish


effective defect densities for in-line yield prediction


[2][3][4].


In previously published correlation work, the area in


the vicinity of the defect is checked for failing bits


with the result being a simple “yes” or “no” [5]. This


is equivalent to the first step of our two-way


correlation. In this work, on the other hand, we


actually determine the type of bitmap signature that


the defect correlates to. We start the second phase of


the correlation by looking at the failing bitmaps


(B in Table 2). Those bitmaps have been classified,


so each failing bitmap is now composed of one or


more signatures. For each signature, we determine if


there was an in-line defect detected, and if so, what


type. Correlation results are shown by number of die


affected in Table 5. The fraction of failures correlated


to optical defects varies from a high of about 70% for


column quad failures to a low of about 10% for


single bit failures. For each signature, correlated


defects are broken down by process step in Table 6.


These results give some insight into the physical


mechanism behind the bitmap signatures, based on


what process step the defect was detected at. In the case of signature classes which rarely correlate to inline defects, this is also informative, since it indicates that a non-visual type of defect, such as oxide leakage, is responsible for the failures. Alternately,uncorrelated bitmap signatures could result from optical defects which are not detected because in-line inspection is not performed at the right step in the process.


Conclusions About


Physical Failure Mechanisms


Inspection of signature correlation results shown in Tables 5 and 6 gives insight into physical failure mechanisms.


Example 1 Column Quad Failure/Metal 2 defects


From 11 wafers, we found that 65 out of a total of 92 quadruple column failures correlated to Metal 2 defects detected in line. Inspection of the layout and circuit confirmed that this is the likely failure mode for metal 2 to metal 2 bridging. The remaining quadruple column failures did not correlate to any optical defect, probably because the defects were outside the sample region for in-line inspection.


Example 2 Row Failure/Metal 1 Defects


Metal 1 defects correlate to row failures, which is to be expected based on the layout.


Example 3 DRAM Capacitor Defects


DRAM capacitor and defects correlate strongly to single bits, bit pairs, and unclassifiable signatures,indicating that they affect only the bits they occur on,which is also expected from the layout.


Example 4 Column Failures


Both types of column failures (complete block and column fragments), which would be expected to correlate to metal 0 based on the layout, correlated more strongly to defects detected at contact mask,and less strongly to metal 0 defects. This could be due to defects which damage the metal 0 level but are detected more easily at contact, or it could be due to defects which cause the metal 0 column line to short to an underlying level through the contact.


Example 5 Contact Open Failures


From the layout, we expect an open contact to result in a bit pair failing in a column. From Figure 1 above,there is little evidence of an open contact failure mode.


All four 2-bit failure modes affect approximately the same number of die (2BitCol_OE, 2BitCol_EO,2BitRow_OE, 2BitRow_EO). If there were many open contacts failures, one of the dual bit columns(2BitCol), either even/odd or odd/even should stand out. The 2BitCol_OE is slightly higher than the others,which suggest that this may be the shared-contact pair.


This is confirmed in Figure 2, which shows the number of individual signatures (as opposed to number of die affected); here the 2BitCol_OE stands out dramatically. These failures occurred at a high rate on some wafers but did not correlate to any in-line defect in Table 6. Therefore, the likely failure mode is contact open due to a systematic process problem that is not optically detectable.


Results from correlation of electrical bitmaps to optically detected in-line defects can provide insight into physical failure mechanisms usually acquired by physical FA. If the bitmaps are classified, two-way correlation can be performed: in-line defect to bitmap failure, as well as bitmap signature to in-line defect.


Results from an advanced DRAM design were analyzed to demonstrate the type of conclusions about failure mechanisms that result from this method. These results also demonstrate the value of analyzing memory devices failures, even those that can be repaired, to gain understanding of defect mechanisms.


1. Julie Segal, Linda Milor, and Yeng-kuang Peng,“Reducing baseline defect density through modeling random defect-limited yield”, MICRO Magazine, January 2000, pp. 61-71.


2. Julie Segal et al., "A Framework for Extracting Defect Density Information for Yield Modeling from In-Line Defect Inspection for Real-time Prediction of Random Defect Limited Yields,"1999 IEEE International Symposium on Semiconductor Manufacturing Conference Proceedings (ISSM), pp. 403-406.


3. Julie Segal et al, “Critical Area Based Yield Prediction Using In-line Defect Classification Information”, to be presented 2000 IEEE/SEMI Advanced Semiconductor Manufacturing Conference


4. A. Gordon, D. Sajoto, A. McCauley, “Inspection Optimization for Excursion and Baseline Defect Monitoring in a Manufacturing Environment”,1999 IEEE International Symposium on Semiconductor Manufacturing Conference Proceedings (ISSM), p 371-374


5. R. Ott et al, “An Effective Method to Estimate Defect Limited Yield Impact on Memory Devices”, Proceedings1999 IEEE/SEMI Advanced Semiconductor Manufacturing Conference, pp. 87-91


Table 3 Average kill ratio for defects at various masking levels.


le 3 Average kill ratio for defects at various masking levels.


|Dram cap |active |Contact |poly |M0 |M1 |M2 |Average |
|---|---|---|---|---|---|---|---|

|48.1% |61.5% |18.7% |41.5% |56.6% |16.4% |53.3% |38.8% |

Table 4 Kill ratios for Metal 2 in-line defects by classification.


e 4 Kill ratios for Metal 2 in-line defects by classification.


||Class 1 |Class 2 |Class 3 |Class 4 |Class 5 |Class 6 |Class 7 |Class 8 |Class 9 |Class 10 |Class 11 |Class 12 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|

|# defects in sample |12 |50 |18 |90 |14 |2 |36 |1 |1 |1 |3 |1 |

|Kill ratio |66.67% |2.00% |38.89% |58.89% |57.14% |0.00% |0.00% |100% |0.00% |100% |100% |0.00% |

Table 5 Bitmap correlation results showing number of die with each signature present (there may be more than one occurrence in a die), and how many of those die showed no correlation, full correlation, of partial correlation on each signature


on, full correlation, of partial correlation on each signature


|Bitmap Signature |# die with signature |# die with no correlation |# die with full correlation |# die with partial correlation |# die with partial correlation |
|---|---|---|---|---|---|

|Column (block) |172 |117 |46 |9 |9 |

|Column quad |92 |23 |68 |1 |1 |

|2BITCOL_EO |286 |231 |44 |11 |11 |

|2BITCOL_OE |359 |317 |27 |15 |15 |

|2BITROW_EO |271 |226 |39 |6 |6 |

|2BITROW_OE |261 |209 |42 |10 |10 |

|Row (block) |431 |290 |119 |22|22 |

|Single_Bit |1942 |1606 |75 |261 ||

|UNCLASSIFIABLE |1249 |950 |148 |151 |151 |

|Column (partial block) |2405 |1828 |352 |225 |225 |

|Row (partial block) |1620 |1141 |291 |188 |188 |

Table 6 In-line defect correlation results showing the number of in-line defects


at each mask layer which correlated to each signature.


|Bitmap Signature |DRAM Cap mask |Active mask |Poly mask |Contact mask |M0 mask |M1 mask |M2 mask |
|---|---|---|---|---|---|---|---|

|Column (block) |2 |5 |20 |24 |9 |12 |9 |

|Column quad |2 |0 |0 |4 |0 |4 |65 |

|2BITCOL_EO |27 |21 |15 |10 |2 |2 |0 |

|2BITCOL_OE |10 |10 |17 |12 |6 |4 |0 |

|2BITROW_EO |15 |15 |20 |15 |0 |1 |0 |

|2BITROW_OE |16 |11 |19 |26 |1 |3 |0 |

|Row (block) |1 |4 |9 |16 |4 |95 |31 |

|Single_Bit |109 |90 |150 |128 |10 |17 |0 |

|UNCLASSIFIABLE |97 |107 |139 |109 |27 |7 |0 |

|Column (partial block) |30 |130 |210 |345 |82 |36 |25 |

|Row (partial block) |24 |160 |341 |269 |26 |43 |9 |

p 89-91


DOI: 10.1361/cp2000istfa089


Analysis of Leakage Failures in Flash Memory Devices and Root Cause Identification


N. De Luna, M. Del Fierro, and J. Muñoz


Intel Technology Philippines, Inc., General Trias, Cavite, Philippines


An advanced flash bootblock device was exceeding current leakage specifications on certain pins.


Physical analysis showed pinholes on the gate oxide of the n-channel transistor at the input buffer circuit of the affected pins. The fallout contributed ∼1% to factory yield loss and was suspected to be caused by electrostatic discharge or ESD somewhere in the assembly and test process. Root cause investigation narrowed down the source to a charged core picker inside the automated test equipment handlers. By using an electromagnetic interference (EMI) locator,we were able to observe in real-time the high amplitude electromagnetic pulse created by this ESD event. Installing air ionizers inside the testers solved the problem.


Electrostatic discharge or ESD damage to components, devices and equipment continue to be a problem for the electronics, semiconductor and hard drive industries [1,2]. The ESD problems are aggravated by the technology trend to smaller device geometry, faster operating speeds, and increased circuit density. It is very likely that ESD will be a continuing threat to the industry with increasing severity if not properly addressed.


Charged device model (CDM) ESD failures are still widespread in assembly and test sites. In a recent issue, assembled 8Mb, 16Mb, and 32Mb flash devices were found to be exceeding current leakage specifications at test. Fallout was coming from several sources: electrical internal trouble reports,product qualification, manufacturing validation and class testing. This translated to a yield loss ranging from 0.07% to 0.98%. The failures were caused by ESD occurring somewhere in the assembly and test flow.


An ESD event happens very fast, typically in 100 nanoseconds or less and often intermittent. Therefore it is very difficult to trace or pinpoint. Furthermore,the many process steps in the assembly and test line just adds to the complexity in isolating the source.


Oftentimes, corrective actions such as proper grounding, elimination of triboelectric charging and stray fields, and installation of ionizers are done blindly in hopes of eliminating ESD problems.


There are however, ways to detect occurrences. When an ESD event happens, a burst of energy is created in its immediate vicinity in the form of electromagnetic radiation also known as electromagnetic interference or EMI. The radiated EMI is typically in the 10MHz2GHz range and can be detected with an EMI locator. This device consists of an antenna that detects the EMI pulse and a high speed, digitizing oscilloscope that displays it. In our case, this device proved to be very helpful in identifying the ESD source in the line that was causing the leakage failures. This paper presents the electrical characterization of the failure, the physical failure analysis techniques used in the case and the usefulness of the EMI locator in identifying root cause.


Failure Analysis Results


Electrical validation showed that failing devices exceeded current leakage specifications on specific clock pins called OEB (output enable pin) and WEB(write enable pin). Emission microscope analysis detected a photoemission spot at the nmos transistors of the input buffer circuit of the affected pins. This is shown in Figure 1.


Figure 1 Photoemission spot at the input buffer circuit of the OEB pin.


A schematic and layout of the input buffer circuit is shown in Figure 2. The nmos forms part of an inverter in the input buffer. All affected devices had photoemission in the same location. The nmos source is connected to Vss, the drain to signal (SP3) and the polysilicon gate connected to the pin (OEB).


A2/T91.0 kV x11.0K 2.23mm


A2/T91.0 kV x1lKoK 2.72μm


Figure 2 Schematic of the input buffer circuit.


Physical FA results hinted at ESD as the possible root cause but the failure mechanism was not well understood, nor easily visualized. Units that were dipped in hydrofluoric acid (HF) did not consistently show damage at the affected nmos when imaged in a field emission scanning electron microscope (FESEM). Figure 3 shows a FESEM image of an etched unit. This sample has some damage seen that on the nmos gate but is neither readily evident nor conclusive. A 20 second Wright-Jenkins decoration


etch helps in visualizing the defect clearly as shown in Figure 4. Several pinholes on the oxide are seen and are concentrated near the source side of the gate.


03#


The failure mechanism is gate oxide breakdown. The high electric field created by the ESD event exceeded the oxide breakdown field strength. The schematic in Figure 2 shows that the discharge


VSS


current created a leakage path from gate to the grounded source.


InputFigure 3 FESEM image of the nmos after HF etch.Buffer Ciruit


SHHSO


OEBM


SP3


Leaky nmos


ESD Protection Cimit


Vss


Figure 4 FESEM image of the nmos after 20s


Wright-Jenkins decoration.


Root Cause Identification


Efforts to contain the problem focused on looking at device sensitivity to ESD and checking ESD protection at the line (grounding, ionizers, handling,etc.). These efforts did not reduce the fallout.


These bootblock devices were known to have lower ESD tolerance than previous generations and this was initially attributed as the reason for the high leakage fallout. However, with the introduction of a new, high capacity tester and handler in the line, we observed zero device leakage fallout. This means that the leakage failure was being induced at test and not solely due to device sensitivity to ESD.


With the aid of an electromagnetic interference (EMI)locator, the high amplitude EM pulse created by the ESD event was detected when the picker was about to socket a unit under test. Failure analysis on these units showed leakage failures. Air ionizers were installed inside the test chamber in order to neutralize the accumulating charge. When this was done, the EMI locator confirmed that the ESD event was no longer occurring and the leakage fallout disappeared.


Investigation showed that high static fields are present at the retriever boat and core picker which are shown in Figure 5. Both make contact with the device, hence causing the device to charge up and then discharge upon socketing. With an electrostatic fieldmeter, we found that the core picker and the boat that makes direct contact with the device is made of a high perfomance plastic that easily gains high static charge. We theorized that the device gains charge from contact with these materials and discharged as the balls make contact with the tester pogo pins.


Figure 5 (A) Core picker and (B) retriever boat With regards to the ESD tolerance margin of the device, it was low enough to the point that the ESD voltage levels generated inside the tester was able to induce damage. Earlier generation devices did not require the installation of ionizers inside the old testers.


Summary and Conclusion


Failure analysis of leakage failures in flash memory devices showed gate oxide breakdown at the nmos transistors of the input buffer circuit caused by an ESD event. The failures were induced in the line.


Using an EMI locator, we were able to observe in real-time the high amplitude EM pulse when a device was about to be socketed into the tester. The retriever boat and core picker in the test handler are made of a high performance plastic which is prone to static charge gain. Both come into contact with the device,causing the device to charge up and discharge upon socketing. The EMI locator was helpful in solving our ESD problem.


1. L. Levit and A. Steinman., “It’s the Hardware.


No, Software. No, It’s ESD!”, Solid State Technology, May 1999, Pennwell Publishing Company.


2. J.Munoz, C. Adriano, J. Tan and E. Roldan,“Detecting ESD Events Using a Loop Antenna”to be published in the 2000 EOS/ESD Symposium proceedings.


p 93-95


DOI: 10.1361/cp2000istfa093


Passive Voltage Contrast Application on Analysis


of Gate Oxide Failure in 0.25 μm Technology


Song Zhigang, Loh Sock Khim and Shailesh Redkar


Failure Analysis Group, QRA, Chartered Semiconductor Manufacturing Limited, Singapore


With further miniaturization of MOS devices, the thickness of gate oxides becomes thinner and thus more sensitive to damage. Emission microscopy has shown its capability in analysis of these failures.


However, emission site is not always the exact location of the physical defect. High-density devices with multi-metal layers make the situation worse. But when it is combined with Passive Voltage Contrast(PVC) technique, the success rate of isolating such failures can be greatly increased. In a case study, a unit of 1M bits Static Random Access Memory(SRAM), fabricated by 0.25 μm technology with 5 metal layers, failed after 500 hours burn-in. We successfully isolated the leaky poly and subsequently found gate oxide pinholes with the combination of PVC technique and emission analysis.


With continuous scaling down of ULSI devices,CMOS devices tend to be of smaller feature size,higher density and more layers. Meanwhile, the thickness of gate oxides becomes thinner and thus more sensitive to damage. Of which, plasma-induced damage is believed to be a very common one and has been extensively studied [1, 2] because of the wide application of high-density plasma processes in semiconductor manufacturing. It is generally accepted that plasma-induced damage to gate oxides can not only impact yields of devices but also affect their reliability.


In the past, emission microscopy has shown its capability in analysis of gate oxide failures [3, 4].


However, emission site is not always the exact location of the physical defect. Recently, highdensity devices with multi-metal layers make the situation worse. But when it is combined with Passive Voltage Contrast (PVC) technique [5], the success rate of isolating such failures can be greatly increased. In this paper, we demonstrate a method to identify the leaky poly in a burn-in failed unit by the combination of emission analysis and PVC


technique, and subsequently find the gate oxide defects, which are believed to be due to plasmainduced damage.


Passive Voltage Contrast Description


As a failure analysis technique for semiconductor devices, PVC was first published by Colvin in 1990


[5]. The technique is passive because voltage contrast in a sample is due to charge-up by the electron beam,not from an external power supply. When a sample is inspected in Scanning Electron Microscope (SEM),different structures such as floating and grounded structures on the sample will be at different potentials because of electron charge-up, leading to different secondary electron emission yield and an image contrast between the structures. Figure 1 shows a general secondary electron emission yield curve vs.


beam energy, where EIand EIIare the two cross-over energies at which the secondary electron emission yield is equal to 1 [6]. Usually, in PVC experiment,the electron-beam energy E is between the two crossover energies. Such electron beam makes the floating structure be charged positively because the secondary electron emission yield is more than 1. The net positive charge makes the floating structure at a positive potential, which will further accelerate the incident electron beam and so increase the effective beam energy until EII[7, 8]. Therefore, the secondary electron emission yield from the floating structure decreases. In addition, since the secondary electron energy is low, only 0-50eV [6], they will be recalled by the positive potential and recombined with the net positive charge. So the floating structure is dark in SEM image. For grounded structure, the net positive charge will drain off to substrate and so no potential is built-up. Thus, the secondary electron emission yield remains high for grounded structure. So the grounded structure is brighter than the floating structure in SEM image. Tilting the sample to certain degree will enhance the contrast. Similarly, PVC has also been observed in ion-beam-based microscope [9]and applied in failure analysis of integrated circuits[10]. In ion-beam induced PVC, voltage contrast is due to charge-up by an ion beam, analogous to that by an electron beam.


Figure 1a general secondary electron emission


yield curve vs. beam energy.


Case Study


1M bit Static Random Access Memory (SRAM) was fabricated by 0.25 μm technology with 5 metal layers


on BearnDet WD Exp10.0KVCEM 16.5 1WKEX42A10μm


and 1 poly layer. It was comprised of 16 sub-RAM blocks and connected in such a way that all 1M bits can be addressed separately. One unit failed because its IDDQ value was higher than a normal unit after 500 hours burn-in. Emission analysis revealed an emission site in the block decoder as pointed by arrow in Figure 2, when the unit was powered-up in such a way that all Vcc pins are tied together to 2.7V and the rest pins are grounded. For good unit, no emission was found at the same power-up conditions.


So the emission was confirmed to be valid.


Figure 2 Emission site in the block decoder detected by emission microscope.


Acc. V Spot MagnDet WD Exp5.00kV 3.0 28100x TLD 46 1


After emission site was found, the unit was deprocessed layer by layer until metal 1 with the combination of Reactive Ion Etch (RIE) for dielectrics and parallel lapping for metal layers. No anomaly was found. Therefore, the leakage was likely due to gate oxide defect. The unit was further parallel lapped to expose poly. Although emission


analysis found an emission site in the block decoder,it is still difficult to tell the exact leakage location. In order to identify which poly is leaky, PVC experiment was performed around the emission site by ion beam in FEI Dual Beam 820 FIB/SEM Station and the obtained PVC photo is shown in Figure 3.


From Figure 3, it is clearly seen that three poly sites(2 N-channel and 1 P-channel) are much brighter than the others. This means that these three poly sites are leaking to substrate and thus grounded.


Figure 3 PVC photo showing three leaky poly sites.


After identifying three leaky poly sites by PVC, the unit was further deprocessed to remove poly by polyetchant. SEM observations revealed three pinholes,which are correlated with the corresponding three leaky poly sites (see Figures 4 - 6). The root cause for these pinholes is believed to be plasma-induced damage. One probable scenario is that plasmainduced charging caused latent damage to the gate oxide but the unit still passed the test before burn-in.


During burn-in, the latent damage got worse by stress and eventually gate oxide totally break down after 500 hours burn-in, leading to IDDQ failure.


Figure 4 Pinhole was observed at the gate-oxide


layer at 1stleaky poly site (S1).


Beam Energy E(keV)


EI EII


Secondary electron emission yield δ


δ=1


E


Figure 5 Pinhole was observed at the gate oxide


layer at 2ndleaky poly site (S2).


Figure 6 Pinhole was observed at the gate oxide


layer at 3rdleaky poly site (S3).


In summary, Passive Voltage Contrast technique,combined with emission anlysis was demonstrated to greatly enhance the analysis success rate of gate oxide failures. In this case study, emission analysis found an emission site at the block decoder of the failed unit and PVC further identified three leaky poly sites around the emission site. Finally it was found that the leaky poly sites were due to pinholes in gate oxide. The root cause for these pinholes are likely due to plasma-induced damage.


Acknowledgment


The authors would like to thank Gan Chock Khing and Phoong Boom Fue for providing samples and invalable discussion.


1. Y. H. Lee, K. Wu, G. Sery, N. Mielke and W.


Lin, P2ID, 38 (1998).


2. K. P. Cheung, Q. Lu, N. A. Ciampa, C. T. Liu,C. P. Chang, J. I. Colonell, W. Y. C. Lai, R. Liu,J. F. Miner, H. Vaidya, C. S. Pai and J. T.


Clemens, P2ID, 137 (1999).


3. C. L. Chiang and N. Khurana, IEEE International Electron Devices Meeting, 672(1986).


4. B. Bossmann, P. Baurschmidt, K. Hussey and E.


Black, ISTFA Proceedings 351 (1992).


5. J. Colvin, ISTFA Proceedings, 331 (1990).


6. H. Seiler, J. Appl. Phys., 54(11), R1 (1983).


7. H. von Seggern, IEEE Trans. Nucl. Sci., NS-32,1503 (1985).


8. Z. G. Song, C. K. Ong and H. Gong, J. Appl.


Phys., 79 (9), 7123 (1996).


9. E. C. G. Kirk, J. R. A. Cleaver and H. Ahmed,Electronics Letters, 23, 585 (1987).


10. H. Yamashita, H. Nanatsue, Y. Hata and S.


Mayuml, IPFA Proceedings, 50 (1991).


p 97-105


DOI: 10.1361/cp2000istfa097


Forensic Microscopy in the Failure Analysis Laboratory


William E. Vanderlinde


Microelectronics Research Laboratory Columbia, MD, USA


David A. Stoney


McCrone Research Institute Chicago, IL, USA


100 microns


p 107-115


DOI: 10.1361/cp2000istfa107


Failure Analysis Process Flow and Common Failure Mechanisms in Flip-chip Packaged Devices


Steve Hsiung, Victer Chan


LSI Logic Corporation, Fremont, California


Flip Chip BGA


With the increasing complexity of packaging


Highest Performance Package


technology, especially Flip-chip, package failure analysts face challenges to identify failure root cause.


Due to the complex construction of Flip-chip


Silicon Die


packages, the conventional failure analysis process


Theninal Epoxy


flow needs to be enhanced. Thus, generating a bench


Spreader Copper Heat


marked failure analysis process flow specifically for Flip-chip packaged devices becomes necessary.


In this paper, the failure analysis process flow for


Mobraye


Drganic or Ceramic Substrate


Solder Bumps on Die


Flip-chip package devices along with different failure


Power and Gro Hsh Demity


Eus Arom RnAp


mechanisms will be discussed and demonstrated. For


Solder Balls


instance, even in a simple continuity-open failure,


500fa1509


instead of cross-sectioning the device as the initial fault identification step, the process flow details how to start from non-destructive C-SAM, TDR, to destructive die removal, polishing and finally crosssectioning.


Flip-chip is an interconnect technology that uses small solder bumps on the active surface of the die for connection to the substrate. It has three main sites: the die, the solder bumps and the substrate.


The die is flipped upside down, and bumps are soldered in between bond pads and substrate. In this way, connections can be made with very short trace lengths, and core power connected directly to the core of the die (Figure 1).


The utilization of Flip-chip technology has significantly increased in the semiconductor industry,largely because of its higher lead count, thermal and electrical performances and low cost. LSI Logic, for instance, uses Flip-chip Ball Grid Array (FC-BGA)package technology that can support lead counts in excess of 1700, and offers excellent electrical and thermal performance.


Figure 1 Cross-sectional view for Flip-chip BGA Construction.


However, the complex construction in Flip-chip packaged devices compared with wire-bond devices makes failure localization and failure identification much more difficult. The conventional failure analysis process flow may not work for the new Flipchip packaged devices.


Considering a continuity-open failure case as an example, the defect could occur in any one of the three sites. Therefore, questions often arise on how to locate the failing site and when the failing site is isolated, whether cross-section is the best approach to identify the defect without damaging the device, etc.


Therefore, it is necessary that a bench marked failure analysis process flow for Flip-chip packaged devices be generated.


Failure Analysis Process Flow and


Common Failure Mechanisms


From a failure analysis standpoint, failure localization is critical for defect identification and the process is interactive. To isolate the failure to one of the three sites, the process flow should be done in order, because some steps are irreversible. The failure analysis process flow for Flip-chip packaged devices


starts from non-destructive to destructive methods based on their unique construction. In the following process, case examples of common failure mechanisms will be discussed. The process flow includes:


1. Verification


2. Heat Spreader Removal


3. Optical Inspection


4. C-mode Scanning Acoustic Microscopy


5. Time Domain Reflectometry


6. Real-time X-ray Inspection


7. Stiffener Removal


8. Die Backside Thinning


9. Backside Emission Microscopy and Liquid Crystal


10. Die and Substrate Separation


11. De-processing


12. Cross–sectioning


13. Scanning Electron Microscope and Energy Dispersive X-ray


Verification


Whether for Flip-chip packaged devices or for wirebond devices, failure verification is the first step once a failing device is obtained. Failure verification can save the analyst valuable time. For example, poor contact during electrical test could result in false failure. During verification, such conditions as testing parameters, stress tests, etc should be considered.


Case No. 1: A failing device was recovered at room temperature during failure verification. Testing history showed the failure happened after temperature cycling test. The failure was confirmed later when the device was heated up. That demonstrates the failure mechanism was temperaturesensitive.


Heat Spreader Removal


Unlike wire-bond devices, Flip-chip packaged devices have a heat spreader that gives the best thermal dissipation without a heat sink. Removing it makes optical inspection, C-SAM, X-ray etc possible.


The technique begins at each corner of the package.


Wedge a razor blade between the heat spreader and the stiffener, slide the razor through the epoxy material and work around the package (Figure 2).


Figure 2 Optical image of separated heat


spreader from package.


Optical Inspection


Some failure mechanisms are so obvious that they are detectable by optical inspection. This saves time for the analyst and makes analysis more effective.


Usually optical inspection of a device is performed under microscope at low and high magnification.


Case No. 2


A failing device was found missing solder balls of the signal pins by optical inspection (Figure 3). The Solder Ball Shear Testing was then done to determine whether it was assembly or handling related problem.


Figure 3 Optical image of missing solder balls.


Case No 3


The die crack was found in a failing device, where a power short between Vdd and Vss occurred


(Figure 4).


Figure 4 Optical image of a die crack.


C-mode Scanning Acoustic Microscopy


The C-mode Scanning Acoustic Microscopy(C-SAM) analysis is effective in detection of cracks or separations in solid materials. In Flip-chip packaged devices, C-SAM analysis is used to find delamination at any of the two interfaces: the die underfill epoxy interface and the underfill epoxy substrate interface (Figure 5).


Figure 5 Illustration of concerned interfaces for CSAM analysis: (1)die-underfill epoxy; (2)underfill epoxy-substrate.


Case No. 4


A mass delamination at die-underfill epoxy interface was revealed by C-SAM in a failing device where there were multiple open signal pins (Figure 6).


Figure 6 C-SAM image of delaminated (red) area.


Time Domain Reflectometry


One of the fast and nondestructive methods for failure localization is Time Domain Reflectometry(TDR) analysis. The fundamentals of TDR are simple: a digital sampling oscilloscope with a TDR module sends a fast rise-time voltage edge to the signal pin, and then records the voltage edge reflections. The time delay between the incident and reflected electrical signals is analyzed and compared


to characterize the electrical signal path of the signal


Underfill epoxy


pin.


Used in Flip-chip packaged devices with four Substratemeasurements, TDR can provide instant indication of the failing site, whether it is in the die, the solder bumps or in the substrate. Signal pins are measured


Solder Ball


in the failing device, the standard device and the


Solder Bump


unassembled substrate (bare substrate) as correlation,along with one measurement with no device (open device). By comparing the waveform from the failing device with those from the bare substrate, the standard device and open device, the analyst can easily identify the failing site.


Not only can TDR waveforms tell where the failure is in one of three sites, but they can also pinpoint the precise location. For example, depending on how far the waveform from signal pin is away from the waveform from bare substrate, TDR can show if the failure is near solder balls or near substrate pads.


That will help the analysts decide which destructive technique should be carried out.


Case No. 5


TDR analysis was performed in a failing device indicating that the failing site was in the substrate(Figure 7). That was confirmed later by cross-section technique.


Figure 7 TDR waveforms of signal pins showing that the open is in the substrate: a) from open device; b)from the failing device; c) from the bare substrate; d)from the standard device.


Real-time X-ray Inspection


Due to its high sensitivity, broad field of view, high spatial resolution, flexible sample orientation and sophisticated post-acquisition image processing,Real-time X-ray (RTX) inspection is widely used for locating hidden elements without damaging the device in Flip-chip packages, especially for locating solder bridges.


Case No. 6


Figure 8 RTX image of solder bump bridging.


A solder bridging between solder bumps was found by RTX inspection in a failing device where a power short between Vdd and Vss occurred (Figure 8).


Stiffener Removal


Nothing can be done to de-process the substrate in Flip-chip packaged devices without removing the stiffener. The procedure for removing a stiffener is similar to that of removing a heat spreader, except wedging a razor blade between the stiffener and the substrate (Figure 9). During the stiffener removal,one should be careful not to damage the solder mask and the substrate underneath.


Figure 9 Optical image of removed Stiffener.


Die Backside Thinning


Because the die in Flip-chip package is flipped and faced downward, traditional localization techniques such as Emission Microscopy (EMMI), Liquid Crystal(LC), mechanical and e-beam probing are impossible.


In order to perform backside analysis, a milling machine is used to thin the die by mechanical grinding.


Typically the die is thinned to 200μm (Figure 10).


Figure 10 Backside image of die surface after the die was thinned.


Backside Emission Microscopy and Liquid Crystal


After the die is thinned, Backside EMMI and LC techniques can be used at die level without affecting the devices’ electrical functionality.


Case No. 7


The failing site in a failing device was pinpointed to the die. The die was thinned first. Then an emission site was found by backside EMMI (Figure 11).


Figure 11 A backside image showing an emission


site detected by EMMI technique.


If emission sites or hot spots are detected by backside EMMI or LC techniques, the failure analysis will target the die. Otherwise the failure analysis will continue with the substrate as the target.


Die and Substrate Separation


Once the die or the substrate is determined to be the target, they must be separated from each other. The simplest way is to put the device in a heater block for five minutes at around 350oC until the die attach material begins to soften. A razor blade is then used to remove the die attach material and to slowly lift the die upward (Figure 12). This method tries to preserves the die and the substrate for further failure analysis.


Figure 12 Optical image of removed


die from substrate.


Unfortunately, with this technique, sometimes the die, the substrate or both can be damaged, which will end the failure analysis effort pre-maturely. In order to improve the success rate of preserving the integrity of the target, one of the elements can be sacrificed with the following de-process technique.


De-processing


The de-processing technique used for Flip-Chip packaged device refers to grinding or lapping the die or the substrate.


By grinding the substrate, the die is preserved. The surface of the die can now be made visible with reactive ion etching (RIE), which removes the remaining underfill epoxy material.


By grinding the die, the substrate is preserved. This allows the analyst to confirm the substrate failure by making measurements from the substrate bond pads to the related solder balls.


Case No. 8


Continuing analysis from Case No. 7, after grinding the substrate, optical inspection in the location of an emission site on the die surface found EOS damage(Figure 13).


Figure 13 Optical image of EOS


damage on the top metal.


Case No. 9


A failing device was found to be a pin-to-pin short in the solder bump. However, the defect could not be located by using RTX inspection. After grinding the die, optical inspection revealed solder bridging(Figure 14).


Figure 14 Optical image of solder bridging.


If no defects can be found with surface visual inspection, continue with die or substrate parallel lapping. Lapping the die to review root cause of failure from Flip-chip packaged devices is no


different than wire-bond devices. The more important application is lapping the substrate. It is crucial,through parallel lapping, each layer of the substrate is made accessible, and failure mechanisms in any layer can be identified.


Case No. 10


The open location was pinpointed to the substrate in a failing device. Lapping the solder mask material after removing the stiffener revealed a crack in the first layer of the substrate (Figure 15). Then this layer was again lapped to expose second layer where broken signal metal traces were identified (Figure 16 and Figure 17).


Figure 15 Optical image of a crack in the first layer of the substrate.


Figure 16 Optical image of broken metal traces in


the second layer of the substrate.


Figure 17 Optical image at high magnification shows


broken metal traces in Figure 16.


Case No. 11


A failing device was found to be pin-to-pin short in the substrate. Lapping the substrate down to signal layer showed metal migration between metal traces in the same layer of the substrate (Figure 18).


Figure 18 Optical image of metal migration.


Case No. 12


After an open was found in the substrate, sequentially lapping the substrate shows misaligned via(Figure 19).


Figure 19 Optical image of a misaligned via.


Cross-sectioning


The cross-sectioning technique is primarily used to evaluate the integrity of solder bumps and substrate in Flip-chip packaged device.


When examining the solder bumps, the target bump is identified with the solder bump schematic. The device is next sawed on the side opposite the target and put in a mounting cup (Figure 20). Next, the two-part epoxy is poured into the cup and cured. The encapsulated device is then polished by first grinding to the target and then polishing it using a polishing cloth and polishing wheels. When the target row of solder bumps is reached, both bump/die pad interface and bump/substrate pad need to be inspected.


Figure 20 ptical image of an encapsulated device for polishing.


Case No. 13


An open pin in a failing device was found in the solder bump. Cross-sectioning the target showed a detached solder bump from the die pad caused by delamination at die-underfill interface (Figure 21).


Figure 21 SEM image of detached solder bump from die pad.


Case No. 14


A short between a signal pin and a power pin in a failing device was traced down to the substrate. The location was cross-sectioned. Optical inspection in dark field revealed metal migration in different layers in the substrate (Figure 22).


Figure 22 ptical image of a metal migration in


different layers in the substrate.


Case No. 15


An open signal pin in a failing device was found in the substrate. Cross-sectioning the substrate layer sequentially found an open via (Figure 23).


Figure 23 Optical image of an open substrate via.


Scanning Electron Microscopy and Energy Dispersive X-ray


In Flip-chip packaged devices, Scanning Electron Microscopy (SEM) analysis is used on a routine basis to evaluate the solder bumps after cross-sectioning.


Such SEM analysis requires high magnification to enable visual identification, especially in cases where there are sub-micron cracks at the interfaces of the bump and the pads that are impossible to detect by optical inspection.


Accompanying the SEM, Energy Dispersive X-ray(EDX) analysis is a quick and useful analysis tool.


By interpreting the spectra one can identify the chemical compositions in the interested location.


Case No. 16


In order to confirm that metal migration came from different layers in Case No. 14, the element was analyzed by EDX (Figure 24). The EDX spectrum indicated that the elements were Ni-Cu (Figure 25).


Figure 24 SEM image of an element ready for EDX.


Figure 25 EDX spectrum indicating the


elements Ni-Cu present in Figure 24.


Flip-chip packaged devices are different from wirebond devices in their construction. The traditional failure analysis process flow is not sufficient to ensure high success rate in defect localization and defect identification. The new process flow for Flipchip packaged device, starting from non-destructive approaches, provides a quick, easy and effective way to localize and identify different failure mechanisms.


Case studies have proved the merit of the flow.


Acknowledge


The authors would like to thank their colleagues in New Technology Engineering Department, Package Reliability Department, Package Development Department and Analytical Service Department at LSI Logic for their support in failure analysis.


1. LSI Logic Flip-chip Ball Grid Array (FC-BGA)Package Technology Datasheet, October 1997.


2. Charles Odegard, Craig Lambert, Comparative TDR Analysis as a Packaging FA Tool, ISTFA proceeding (1999), 49-55.


3. John H. Lau, Flip Chip Technologies, MCGrawHill.


10Mm


20KUX3,700 12mm4. David L. Burgess, O.D. Trapp, Failure & YieldAnalysis Handbook.


5. Lawrence C. Wagner, etc., Failure Analysis of Integrated Circuits, Tools and Techniques,


Aqcixition ampbtd


Kluwer Academic Publishers.


Derdrise


Nroat 20Me


比


QMM licesoric:tcl ordireFer 200


0n 10 6400


secsicn


" res Iive


him san rae


The (ws)120


birectury ]tttrm-y atx


Castar frakents anas


This ciple


10.0


15.0


kev


p 117-120


DOI: 10.1361/cp2000istfa117


A Study on the Yield Loss Due to Al (Cu)Interconnections with Spacing Failure


Ruey Lian Hwang , Yung-Sheng Huang ,Ying-Lang Wang , Ming-Jer Lee


Taiwan Semiconductor Manufacturing Company, Taiwan


As ULSI dimensions continue to shrink, the production requirements become more stringent. For the 0.25um process and its sequential generations,metal line width approaches 0.3um or less and the pitch is less than 0.35um. Therefore, it is a challenge to etch the metal lines. Yield loss analysis of 0.25um and 0.18um products showed only TiN residues.


These were from the barrier layer of the TiN/Al(Cu)/TiN layered metal structure, and caused an electrical short and resulted in a low yield. The study focuses on the diagnosis of failure mechanism based on the SEM views of the sites having electrical shorts. Based on the topography of the leakage sites,we propose that excess Cu migrated to the bottom of the the Al(Cu)/TiN interface. Large 0-Al2Cu precipitatesAl(Cu)/TiN interface. Large -Al2Cu precipitates grew and obstructed the general etching process, and formed TiN residues.  In addition thel-precipitatesIn addition the-precipitates were lifted off in the subsequent PR wet stripping process. Meanwhile, Al voids were also formed at the side side wall of metal lines neighboring the -precipitateswall of metal lines neighboring the -precipitates during the processes. We examined the short/openyield-structure (a pattern of Wafer Accept Test) after metal patterning but before PR wet stripping. The etching residue was detected by SEM and analyzed with EDS. The residue contained Cu and was most likely the well-known theta phase Al2Cu. An optimized recipe for interconnections formation was devised and thermal treatments were implemented following the metal depositing process to improve the yield.


With SEM observation, we revealed the failure mechanism of Al (Cu) interconnects with spacing failure induced by[-Al2Cuby-Al2Cu precipitates and significantly contributed to the sequential correction actions.


The stacked TiN/Al (Cu)/TiN layers are used as interconnections in the ULSI process. In the metal configuration, the top TiN layer is an ARC (anti reflective coating), Al (Cu) is the main conductor and the bottom TiN layer is a diffusion barrier and Al<111> texture promoter. A small amount of Cu(0.5% ~ 2% by weight) is alloyed into the aluminum interconnections since Cu is known as an inhibitor for Al electromigration. However, some shortcomings still remain. As the ULSI dimensions continue to shrinkage, the Cu concentration in the Al (Cu) films strongly influences the RIE etch ability [1]. If the Cu is gathered into Al2Cu during the metal film depositing process, the larger the size of the Al2Cu precipitate, the poorer the ability of the RIE to etch small spaces between the Al (Cu) lines.


In this study, the Al (Cu) films contained 0.5wt% Cu as-deposited. A low yield analysis of the product manufactured with the 0.25μm process was performed. The major yield killer was a short in the metal 1 (M1) layer. TiN-residue was found between the metal lines with minimum spacing, 0.32um.


Based on the topographical observation performed on the failed sites using SEM, the failure mechanism was identified and approved by in-line inspection on short-loop wafers.


Experiment


Analysis on the Wafer Posing with Low Yield


The wafers which were manufactured with the CL025 process suffered from scan failure (Bin2 fail)and resulted in low yield. The failed dies were distributed like a donut around the wafers. Liquid crystal technique was applied to localize the failed sites and the overhead SEM (Hitachi S4500)observation at 15KeV on the failed sites was carried out after the stripping of the wafer layer by layer. FEI 820 FIB was used to expose the cross section of a failed site, and X-section SEM images were taken.


Analysis of the Test Patterns of the Wafers with


Metal Spacing Failures Occurring in M1


According to the Wafer Acceptance Test (WAT)results, some wafers suffered from M1 spacing failures and the distribution of failed patterns


VD9


DE


corresponded to the failed dies. The schematic diagram of the test pattern (metal 1 continuity and spacing yield structure) is shown in Figure 1. SEM was also used to inspect the test patterns with M1


metal void


metal 1lines


failed site


spacing failure after the removal of overlayers of M1.


narrow metal line width: 0.32um and metal space: 0.32um


bridging site


Figure 1 The schematic diagram of the test pattern.


In-line and Off-line Examination of a Sample


o


Wafer Manufactured after M1 Patterning


The observation of the short-loop wafer fabricated after the of M1 patterning and before the PR removal was done by an automated electron-beam inspector(KLA/ SEMSpec system). The defective site was subjected to SEM observation and element analysis by EDX. The SEM and EDX examinations were carried out at 15KeV and 5 KeV electron beam voltages respectively, using an Hitachi S-4500 with an attached NORAN lithium-drifted silicon EDX


detector. The calibration of the energy scale of the spectra was performed using Cu samples at their respective L(0.928eV) and K(8.047eV) respective L(0.928eV) and K(8.047eV) peaks.peaks.


Results and Discussions


J58V14.4x83.8 SEC) 11/2/190829:19 35m


Low Yield Analysis


The failed site of the defective die with the scan failure was isolated using LC. According to the LC image, the removal of layers from the passivation layer down to M1 layer and SEM inspection on the failed site were carried out layer by layer. In Figure 2,SEM images of the failed M1 site are reported.


Obviously, only TiN-residue from the barrier layer of the TiN/Al (Cu)/TiN layered metal structure was detected. FIB was used to expose the X-section of


another failed site also located with LC. The SEM image of the failed site is shown in Figure 3;moreover, TiN residue is revealed in the image.


TSMCOR15.0kVx35.ak 85Znm


pad


Figure 2 SEM images at two magnifications of the failed M1 site resulting in the low yield.


Figure 3 The X-section SEM images at two


magnifications of the bridge site of


another failed die.


Analysis on Failed M1_spa


PR


Pattern (WAT pattern)


AI-Cu


The distribution of the failed pattern was consistent


etching


with the low yield die profile on the wafers. LC was


TU4


PRCutch byproduct


applied to isolate the leakage sites again, and the


0.3 um


SEM images of the failed sites are shown in Figure 4.


Noticeably, only the TiN-residue was detected again.


(Higher ion bombardment /etching rate)etchingOpen eara


The root cause of the M1 spacing failure was similar


PR 4


Flching lmkto loading etiecetching rate)


to that which incurred the low yield.


▼PR removal


CuA12 induced Al void during the metal etching and subsequent PR wet strippin


Te


人<CuAt2 induced Ai pitting during PR wet atripping


Figure 4 SEM image of the failed site in WAT test pattern.


Discussions on the Proposed Failure Mechanism


Firstly, the low yield issue could not be fixed by increasing the etching time of the bottom ARC in the M1 etching recipe. That meant the TiN-residue was not attributed to under etching and there were unexpected materials existing and blocking the metal etching. Secondly, Younan [2] revealed a phenomenon that the Al2Cu-precipitate was surrounded by holes on Al pads. Those holes surrounding a -phase nucleus on Al pads surrounding a -phase nucleus on Al pads werewere caused by galvanic corrosion during wafer sawing at assembly. Thirdly, P. Dehaven et al. [1] reported that a high level of Cu concentration segregated at the bottom Al (Cu) /TiN interface. Finally, we took a closer look at SEM images of failed sites shown above, the metal (AlCu) sidewall voiding around the TiN-residue was obvious. Combining these reports and the features of the bridging sites shown above,we presumed that excess Cu migrated to the bottom Al Al (Cu)/TiN interface and large [-phase precipitates(Cu)/TiN interface and large -phase precipitates grew and obstructed metal etching. The holes surrounding the nuclei were formed during the metal etching and subsequent PR wet stripping, and etching and subsequent PR wet stripping, and the-thephase precipitates were lifted off during the PR wet stripping. In addition, it is getting worse in the advanced technology with smaller metal line width and spacing due to lower ion bombardment of metal etching for thinner PR. The schematic diagram of the mechanism of the M1 spacing failure is indicated in Figure 5.


Figure 5 The schematic diagram of the failure mechanism of the M1 spacing failure.


Verify the Failure Mechanism by Inspection on


the Test Structures of the Wafer Processed


between Metal Patterning and


PR Wet Stripping


The wafer processed after metal patterning but before PR wet stripping was examined by SEMSpec system to find out hidden defects. [3] The defective structure was inspected again with off-line SEM. In Figure 6,TiN-residue between metal lines and an expected particle left over the residue were noticed. EDX spectrum of the particle is shown in Figure 7.


Comparing to the EDX spectrum from metal line regions shown in Figure 8, the spectrum of the particle implied that the particle was a Cu-rich precipitate and most likely to be the well-known Al2Cu -phase precipitate. The assumed Al2Cu 0-phase precipitate. The assumed failurefailure mechanism was approved. The yield loss due to Al(Cu) interconnections with spacing failure was caused by large -Al2Cu precipitates blocking caused by large [-Al2Cu precipitates blocking thethe general metal etching and resulting in residues remained.


Figure 6 TiN-reside between metal lines and an expected particle left over the residue.


Figure 7 EDX spectrum of the particle shown in Figure 6.


Figure 8 EDX spectrum from metal line.


The failure mechanism of Al (Cu) interconnects with spacing failures were investigated. The feature of the leakage sites was detailedly analyzed with SEM observation and EDX. We discovered the failure was caused by-phase Al2Cu precipitates obstructing metal etch. In fact, the Al2Cu precipitation formation and dissolution were strongly related with the thermal treatments after metal deposition [4]. An optimized recipe for interconnections formation was devised


and thermal treatments were implemented following the metal depositing process to improve the yield.


Optical microscopy techniques used by forensic analysts are shown to have application to failure analysis problems. Proper set up of the optical microscope is reviewed, including the correct use of the field diaphragm and the aperture diaphragm.


Polarized light microscopy, bright and dark field methods, refractive index liquids, and a particle reference atlas are used to identify contamination found on semiconductor products.


Methods used by forensic scientists such as polarized light microscopy have a variety of applications to microelectronics failure analysis. Process induced particles and foreign materials causing defects on wafers must be analyzed for composition and origin.


Field failures may contain a broader range of foreign material contamination. Furthermore, failure analysis personnel are generally considered the “company experts” in microanalysis and are sometimes called upon to analyze unusual particles or contamination found in a variety of different situations. Therefore it is useful for the failure analyst to have a basic understanding of the methods of forensic microscopy,particularly the polarized light optical microscope.


A survey of the microelectronics failure analysis literature finds very few publications [1,2] on optical microscopy. International Reliability Physics Symposium (IRPS) Proceedings and Tutorials from 1988 to 2000 and International Symposium on Testing and Failure Analysis (ISTFA) proceedings from 1983 to 1999 contain almost no material specifically on optical microscopy. Some failure analysis engineers are poorly trained in optical microscopy and do not take full advantage of all the features of their microscopes. Optical microscopes are often under rated, perhaps because they are not expensive or “high tech”. However, a simple and inexpensive technique such as polarized light microscopy can quickly and non-destructively identify particles that in some cases are difficult to identify by other methods. Furthermore, polarized


light microscopy is excellently suited to compare contaminant particles with alternative sources of the contamination.


The Art of Microscopy


Microscopy is the interpretive use of microscopes to provide specific information about a sample. [3] A basic understanding of microscope operation is necessary to achieve a good image, but the microscopist must also know how to use the instrument to display the particular features of interest in a given sample. There is not necessarily a“best” illumination, magnification, focus, or diaphragm setting for a given sample, it depends on what feature of the sample the microscopist wishes to emphasize.


Optical microscopes can be used in either transmission or reflection mode, i.e. the illumination can be from below and proceed through the specimen, or it can be from above and reflect off the specimen. Forensic microscopists typically use transmitted light to examine particles and fibers,while microelectronics failure analysts typically use reflected light to examine particles adhering to wafers or electronic components. However, in both modes the optical path will proceed through similar optical elements and techniques such as polarized light, dark field, and immersion lenses can be used. For this investigation, samples were examined with a Reichert Zetopan equipped for polarized light examination in transmitted, reflected, or mixed illumination mode.


Some samples were also examined using a Leitz Ergolux without polarizers. The basic design of optical microscopes is discussed in many references[4,5] and will not be reviewed here.


Diaphragm Settings


Optical microscopes (in either reflection or transmission mode) will typically have at least two diaphragms in the optical path. The field diaphragm is placed in a conjugal focal plane, and thus produces


a visible, sharply focused shadow on the image when it is closed down, see Figure 1. If the field diaphragm edges are not in sharp focus, the microscope is not set up properly and the evenness of illumination will suffer dramatically. To correct this condition in transmission mode, the substage condenser must be focused. The condenser is mounted below the microscope stage and has its own separate focusing knob, allowing it to be raised or lowered relative to the stage. With the field diaphragm closed down the condenser focus is adjusted to bring the field diaphragm edges sharply into the same plane of focus as the specimen. Depending on microscope design, it may or may not be necessary to adjust the opening of the field diaphragm as magnification is changed. The field diaphragm should always be adjusted so it is just outside the field of view of the image. If the field diaphragm is further open than necessary, the result is increased glare that will reduce image quality,particularly when taking photographs.


Figure 1 Optical reflection image showing the field diaphragm closed so that it casts a shadow on the image. Magnification is 500x.


The aperture diaphragm, also called the condenser


diaphragm, is not in a conjugal focal plane and thus0.does not produce a visible shadow on the image.


Closing down the aperture diaphragm will result in


an overall reduction in the brightness of the image.


However, if one wishes to reduce the brightness of


the image the best way to do that is by reducing the


illumination lamp voltage, because closing the


aperture diaphragm will have other important effects


such as decreasing the numerical aperture. The


numerical aperture (NA) is a measure of the light


gathering and resolving power of a lens, and it is


related to the angle of the light entering the lens


according to the formula:


NA = n sin (AA/2)


(1)where n = refractive index of the medium (typically n = 1.0 for air when using a dry lens) and


AA = angular aperture of the lens. As the aperture diaphragm is closed, the angle of light entering the lens is decreased, and the numerical aperture is decreased accordingly. As the NA decreases, the resolution and brightness of the image will decrease,but the depth of field and contrast of the image will increase, see Figures 2 and 3. The aperture diaphragm thus provides an important tradeoff between image brightness, resolution, contrast, and depth of field somewhat analogous to adjusting the condenser lens and final aperture in an electron microscope. Each sample will have its own optimum aperture diaphragm setting, depending on the features that one wishes to emphasize. For the aperture diaphragm to control the numerical aperture, as discussed above, it must be focused properly on the specimen as indicated by the in-focus field diaphragm discussed earlier and shown in Figure 1.


Figure 2 Optical reflection image with aperture diaphragm set to open position, with resulting large


NA and high brightness and resolution.


Magnification is 500x.


Figure 3 Optical reflection image with aperture diaphragm set partially closed, with resulting large depth of field and high contrast. Magnification is 500x.


50 microns 50 microns


50 microns


Optical Sectioning


Optical microscopes have a very limited depth of field, particularly at high magnification and open aperture diaphragm settings. When viewing transparent objects, it is possible to take advantage of the narrow depth of field to view horizontal planes within the object. By raising and lowering the focus one can get a good idea of the shape of the object in different horizontal places. Many microscopes have calibration marks on the fine focus knob that allow the user to measure the vertical height distances. This technique is particularly valuable with integrated circuits where the interconnect layers are extremely planar and are located within a transparent dielectric.


Semiconductor defects caused by mis-processing are generally much more planar than defects caused by contamination, and this planarity is easily characterized by optical sectioning.


Particle Refraction: Contrast and Becke lines


Refraction and Contrast


When light passes into and out of transparent particles its direction changes abruptly, which is known as refraction. Refraction at the edges of particles, as seen in the microscope, is responsible for the darkness or contrast that is present. The more refraction that occurs, the darker will be the particle borders. Figures 4, 5, and 6 show fibers with high,medium, and low contrast. The amount of refraction,and thus the amount of contrast, depends strongly on the difference between the particle’s refractive index and the surrounding medium. All particles will show high contrast when the surrounding medium is air,since air has a much lower refractive index than all solids.


For critical microscopy particles are usually mounted in liquids or resins of known refractive index. This allows the particles to be more carefully studied because the refraction at the particle’s edge is not so strong as to detract from the particle’s structure.


Furthermore, the particle’s refractive index can now be qualitatively compared to the refractive index of the mounting medium. Thus in Figures 4, 5, and 6 we could observe respectively that the mounting medium’s refractive index is far away, closer, and very close to that of the fiber. In the extreme case where the particle matches the refractive index of the mounting medium there is minimal contrast and the particle “disappears.” By consistently using a selected mounting medium, analysts are able to rapidly distinguish among particles based on differences in contrast.


Figure 4 A fiber with high contrast to the surrounding medium. The fiber is kevlar with


n = 2.35 along the fiber axis mounted in“Meltmount” with n = 1.662. Magnification is 256x.


Transmission mode was used.


Figure 5 A fiber with medium contrast to the surrounding medium. The fiber is nylon with n = 1.52 perpendicular to the fiber axis mounted in“Meltmount” with n = 1.662. Magnification is 256x.


100 microns 100 microns


Figure 6 A fiber with low contrast to the surrounding


media. The fiber is kevlar with n = 1.64 perpendicular to the fiber axis mounted in“Meltmount” with n = 1.662. Magnification is 256x.


Transmission mode was used. The edge of the fiber,as indicated by the arrow, is very difficult to see in this image due to the close match in refractive indices.


Becke Lines


In addition to contrast differences, particles can be observed to be of either higher or lower refractive index than the mounting medium. Particles that are of higher refractive index will focus light towards their centers, whereas particles of lower refractive index will focus light away from their centers, towards the mounting medium. These effects can be seen by slightly de-focusing the microscope. Moving from sharp focus on the particle to a position of focus just above the particle, light will be seen to move either toward the particle, indicating that the particle is of higher refractive index than the mounting medium, or move toward the mounting medium, indicating that the mounting medium is of higher refractive index than the particle. In general, when one is focused just above a particle, the light is seen to move toward the higher refractive index. Often the light is seen as a bright halo around the particle, referred to as the Becke line. Figure 7 shows a nylon fiber mounted in a medium of higher refractive index and with the microscope focused just above the fiber. The bright Becke line is outside the fiber, demonstrating that the mounting medium is of higher refractive index than the particle. Figure 8 shows the reverse. Here the nylon fiber is mounted in a medium of lower refractive index and when the microscope is focused just above the fiber, the Becke line goes into the fiber.


By using a set of standard oils of known refractive indices, analysts can systematically determine the refractive index of particles by observing particle contrast and the movement of the Becke line in one


liquid and choosing liquids that are successively closer to the refractive index of the particle until the matching liquid is found.


Figure 7 Optical transmission image of a nylon fiber


with the Becke line “out”. np< nm.


Magnification is 256x.


Figure 8 Optical transmission image of a nylon fiber


with the Becke line “in”. np> nm.


Immersion Lenses


Certain lenses are designed to be used with a drop of oil filling the space in between the lens and the sample. This oil acts to increase the effective numerical aperture of the lens by a factor equal to the ratio of the refractive index of the oil (n ~ 1.5) to the refractive index of air (n ~ 1.0), per equation 1. For very fine features at high magnification, the improved resolution is quite noticeable, see Figures 9 and 10. The oil can later be removed from the sample with solvents.


Becke lines


Becke line


Figure 9 Optical image in reflection mode of a three


附


level metal integrated circuit imaged using a dry lens.


Magnification is 1,000x.


求


Figure 10 Optical image in reflection mode of a three level metal integrated circuit imaged using an immersion lens, n = 1.515. Magnification is 1,000x.


Lens oil can also be used for a “trick” to decrease light scattering from passivation while using dry objectives. When integrated circuits are fabricated,the final layer of insulation is known as the passivation, and will typically be a layer of silicon dioxide followed by silicon nitride. The passivation is normally deposited in a conformal fashion, i.e. the surface of the passivation conforms to the topography of the top layer of metal interconnect. The rounded edges of the passivation cause light scattering that significantly degrades an optical image of the circuit.


Some failure analysts use a plasma etcher to remove the passivation and thus improve the image. An alternative is to place a drop of immersion oil on the sample and then spray it with an air jet to spread the oil into a thin layer. [6] Since the oil closely matches the refractive index of the glass, the passivation reflections will be eliminated and the image


improved, see Figures 11 and 12. Note that the presence of oil on the chip surface would also affect the image in Figure 10, so for Figures 9 and 10 the microscope was focused on a lower level of metal(M2) for which the dielectric is planarized.


Figure 11 Integrated circuit imaged with dry lens,magnification = 1,000x. Top metal lines appear enlarged due to reflections from passivation.


Figure 12 An integrated circuit imaged with a dry lens, but with the sample surface coated with lens oil.


Magnification is 1,000x. Reflections from the passivation are reduced, resulting in better resolution.


Dark Field


In bright field illumination the control of the aperture angle is by means of a diaphragm which eliminates the most highly scattered rays and allows the nonscattered (in transmission mode) and specularly reflected (in reflection mode) rays to appear bright. If the angular aperture is replaced with a diaphragm with an opaque central disk, the reverse will be true and some but not all of the direct rays will be blocked, resulting in a “dark field”. [7] In dark field mode any light that was scattered from an uneven


25 microns


feature such as a defect will appear bright against a dark background. Dark field optical microscopy is often ideal for finding defects since irregular particles will show up bright against the dark background of a flat wafer, see Figure 13.


Figure 13 Dark field reflected image of the same defect crystals as shown in Figs. 1-3. Light scattering objects show up well against the dark background.


Dark field illumination can also be used to distinguish materials that merely scatter light from those that absorb it. For example, uncontrolled fluorine reactive ion etching can produce a very rough surface in silicon. Bright field optical microscopy of this rough surface will show a very dark appearance, leading to requests for analysis of the “black layer” for composition. However, if the same area is viewed in dark field, the etched regions will now look bright instead of dark, indicating that the black color seen using bright field was due to scattering, not absorption. [2]


Polarized Light Microscopy


Some particles have consistent optical properties in all directions and are said to be isotropic. These particles show very simple optical behavior and have only one refractive index. Most crystalline particles,however, have different optical properties in different directions and are said to be anisotropic. These particles have more than one refractive index, arising from differences in the atomic and molecular composition along different crystallographic directions. Many artificial fibers consist of polymer chains oriented along the length of the fiber, so they have one refractive index along the fiber axis and a different refractive index perpendicular to the fiber axis. Polarized light microscopy provides a means to distinguish between isotropic and anisotropic particles and to investigate the behavior of light in anisotropic particles. [8]


Ordinary unpolarized light consists of rays having a common propagation direction but randomly oriented planes of vibration. In polarized light the rays all vibrate in the same plane. In a polarized light microscope a polarizer is placed below the condenser, resulting in light that vibrates in only one direction in the image. By convention the polarization direction is oriented horizontally in the field of view. A rotating microscope stage then allows the particle to be oriented with respect to the polarized light. Anisotropic particles, because of their different refractive indices in different directions, can show differences in contrast, color, and in their Becke line behavior as they are rotated in polarized light. Consider Figures 4 and 6 where the same kevlar fiber is viewed with the fiber axis parallel to the microscope polarizer (Figure 4), and then perpendicular to the polarizer (Figure 6). Kevlar has an unusually large refractive index difference between the axial (n = 2.35) and perpendicular(n = 1.64) directions, resulting in a large contrast change on rotation when the fiber is mounted in a Cargille Meltmount medium with n = 1.662.


Additional, highly discriminating properties are seen in these crystals when they are placed between crossed polars. This is achieved by introducing a second polarizing filter, called the analyzer, between the microscope’s objective and eyepiece. The analyzer is oriented so that it is crossed with respect to the polarizer. That is, it polarizes light vertically.


In crossed polarized light one sees a dark background. This is because the polarizer only transmits light that vibrates horizontally and the analyzer only transmits light that vibrates vertically.


All light is therefore blocked.


Isotropic particles, viewed between crossed polars are also dark and will not be seen. Isotropic particles include amorphous materials such as glass, and also crystals of the cubic crystallographic system. Some isotropic materials become anisotropic when placed under stress, and this property is used by mechanical engineers use to study stress concentrations in model structures.


Anisotropic particles viewed between crossed polars will appear bright and often show colors that arise from interference phenomena. This property is known as birefringence and results from the rotation of polarized light that occurs when light passes through anisotropic crystals. The amount of interference that occurs is qualitatively related to the particle’s thickness and the refractive index difference that the anisotropic particle exhibits.


Quantitative measurements of this sort, or qualitative comparisons, can be extremely useful for particle identification. Isotropic particles, that have the same refractive index in all directions, cannot show a refractive index difference, and this accounts for their lack of interference colors.


When anisotropic particles are rotated while viewed under crossed polars, interesting and characteristic effects are seen. Most particles will be observed to disappear (become black) four times during one complete rotation of the circular stage. These positions are called extinction positions and occur 90 degrees apart. The extinction positions reveal the directions in the crystal where the light from the polarizer encounters just one refractive index. In these positions there is no rotation of polarized light and therefore no interference phenomena. The orientation of the extinction positions relative to the shape of the particle is important for particle characterization. Polycrystalline materials may not show any extinction, or they may show irregular or undulating extinction depending on the orientation of the crystallites. Starches and many plant fibers are examples.


Polarized light microscopy (PLM) is an excellent way to distinguish crystal structures rapidly and inexpensively without resorting to TEM and electron or x-ray diffraction. A large fraction of common dust,fibers, and even hairs are microscopically crystalline,and about 85% of crystals show unique birefringence properties under polarized light. Crossed polarizers can be used to study birefringence properties in reflection mode on opaque objects (such as a silicon wafer) although forensic microscopists usually use polarized light in transmission mode.


Applications of PLM


Polarized light microscopy is particularly useful for identifying crystal types and for distinguishing crystalline materials from amorphous materials that have similar composition.


Example 1 - Quartz and Glass Particles


Quartz is frequently used in clean room equipment such as diffusion tubes, vacuum windows, and high temperature glassware. Quartz fragments generally do not fracture along crystal planes and appear microscopically similar to ordinary glass. Quartz is of course chemically identical to un-doped SiO2glass and cannot be distinguished using common analytical techniques such as energy dispersive x-ray spectroscopy (EDS), Auger electron spectroscopy(AES), or secondary ion mass spectrometry (SIMS).


Electron or x-ray diffraction will distinguish glass from quartz, but these techniques are less commonly available and are expensive and time consuming. A simple test to identify the crystallinity of an SiO2 particle is to view the particle using crossed polarizers. The SiO2glass fragments will appear dark,whereas the quartz fragments will appear bright and will exhibit complete extinction upon rotation. See Figures 14 and 15.


Figure 14 Quartz particles observed in transmission with crossed polarizers. Magnification is 176x. The crystalline quartz exhibits birefringence which rotates the light’s polarization vector so that some light is transmitted through the analyzing polarizer.


Figure 15 Ground glass particle observed in transmission. Polarizers were slightly un-crossed to improve visibility. Magnification is 176x.


Example 2 - BPSG Precipitates


Boron and phosphorus doped silicate glass (BPSG)was widely used to achieve planar dielectric layers prior to the development of chemical mechanical planarization (CMP). During BPSG deposition, it is important to maintain tight control over the amount of boron and phosphorus incorporated in the films,otherwise particles will precipitate on the surface of the film during re-flow resulting in a serious yield impact. Typical particles are hexagonal as shown in Figure 16 (Figures 1, 2, 3, and 13 also show these particles.)


Figure 16 BPO4particles imaged by scanning electron microscopy. Magnification is 5,000x.


Energy dispersive x-ray spectroscopy (EDS) analysis of these particles shows silicon, oxygen, and phosphorus, but not boron due to the poor sensitivity of EDS for light elements. Electron diffraction in a transmission electron microscope (TEM) identified a pattern matching JCPDS card number 34-132, which is tetragonal BPO4. [9] Ideally, one should have a quicker and less expensive way to identify these particles. Using crossed polarizers in an optical microscope, the particles exhibits birefringence with a few crystals showing complete extinction upon rotation, see Figure 17.


Figure 17 BPO4particles observed in reflected light


with slightly un-crossed polarizers.


Magnification is 176x.


Example 3: Fabric Fibers


Clean room garments are typically constructed in a herringbone weave from man-made polyester fibers combined with a carbon yarn which improves the conductivity of the material. An example is shown in Figure 18. Polyester fibers have an index of refraction of 1.70 parallel to the fiber axis, and 1.54 perpendicular to the fiber axis. When placed in a


mounting medium with n = 1.55, the fiber will show different Becke line behavior depend on its orientation with respect to the polarization of light.


Most microscopes have horizontal polarization, so when the particle is horizontal then n = 1.70 and the Becke line will be inward with high contrast, but when the fiber is vertical then n = 1.54 and the Becke line will be outward but with low contrast. With crossed polarizers, the polyester fibers exhibit birefringence with complete extinction parallel and perpendicular to the fiber axis.


Figure 18 “Integrity 2000” fabric fibers from Precision Fabrics Group, Inc., imaged in transmission with crossed polarizers. Magnification is 176x. Note the strong optical extinction where the polyester fibers run horizontal or vertical to the image orientation.


For comparison, most street clothes consist of cotton or a blend of cotton and artificial fibers. Cotton fibers show a much more irregular appearance, see Figure 19. Under cross polarizers the cotton displays birefringence with no extinction, because the cotton consists of many small crystals of random orientation. If clean room garments are worn improperly, street cloths worn underneath the clean room garments may represent a potential source of contamination. Properly maintained clean room garments should not be a source of contamination unless cut or frayed.


100 microns 5 microns


Figure 19 Typical cotton fiber from street clothes,transmitted light with crossed polarizers.


Magnification is 176x. Cotton fibers are flat twisted


ribbons and show no extinction.


Particle Reference Atlas


Semiconductor process yield is enhanced by identifying and eliminating defects caused by particles on wafers. [10] Many fabrication lines have developed a gallery of frequently observed defect particles. For unknown particles it is convenient to refer to a computerized particle reference atlas on CD-ROM [11]. This atlas contains more than 1,000 common particles and fibers and includes optical and SEM images, energy dispersive x-ray spectroscopy composition data, and optical properties such as refractive index, birefringence, and extinction. The particle atlas can be searched using key-words, or by the elemental composition and optical properties of an unknown particle.


Inexperienced failure analysts are often impressed by the high magnification of scanning electron microscopes (SEM) and the element analysis capability of energy dispersive x-ray spectroscopy(EDS), and they will perform little or no optical microscopy before putting a sample into an SEM/EDS system. However, the optical microscope has many advantages such as: fast sample loading(since vacuum is not required), rapid surveying of the sample surface in real-time, and the ability to observe colors and high contrast which are lacking in an SEM. Furthermore, techniques such as dark field,optical sectioning, and polarized light microscopy provide valuable information about the location,planarity, and composition of defects. Improved understanding of optical microscopy methods will


enhance the failure analyst’s ability to located and analyze defects.


1. L.C. Wagner, in Failure analysis Desk Reference, 4thEdition, ASM, 1999, p. 271.


2. L.C. Wagner, Microelectronics Failure Analysis,Klewer, 1999, p. 180.


3. T. Rochow and P. Tucker, Introduction to Microscopy by Means of Light, Electrons, X Rays or Acoustics, Second Edition, Plenum,New York 1994, p. 23.


4. Ibid., p. 49.


5. W.C. McCrone, L.B. McCrone, and J.G. Delly,Polarized Light Microscopy, McCrone Research Institute, Chicago, 1984, p. 15.


6. Group discussion at the Failure Analysis Workshop, IRPS, 1995.


7. T. Rochow and P. Tucker, Introduction to Microscopy by Means of Light, Electrons, X Rays or Acoustics, Second Edition, Plenum,New York 1994, p. 201.


8. W.C. McCrone, L.B. McCrone, and J.G. Delly,Polarized Light Microscopy, McCrone Research Institute, Chicago, 1984, p. 49.


9. Private communication, Joseph T. McGinn,David Sarnoff Research Center, Princeton, NJ.


10. E. Bruls, in Integrated Circuit Manufacturability,edited by J.P. de Gyvez and D.K. Pradhan, IEEE Press, New York, 1999, p. 24.


11. W.C. McCrone, The Particle Atlas, McCrone Research Institute, Chicago, 1992


1. L.A. Clevebger, M. Honda, R. Ravikumar and G.


Stojakovic, “Al Deposition Temperature Process Window for 0.20um Al RIE Interconnections,”IEEE International Interconnect Technology Conference, 29-31 (1999)


2. Hua Younan, “A Study on Discolored Bondpads and Galvanic Corrosion,” Proceedings from the 24thInternational Symposium for Testing and Failure Analysis, 15 – 19 Nov. 1998, Dallas,Texas.


3. Jeff Hamilton and Arum Chatterjee, “E-beam Inspection Detects Hidden Defects,” Solid State Technology Supplement 41 (Sept. 1998).


4. Matthew A. Marcus and J. Eric Bower,“Precipitation of Al2Cu in Blanket Al-Cu Films,”Journal of Applied Physics 82, 3821-3827 (15 October 1997).


p 121-123


DOI: 10.1361/cp2000istfa121


Near IR Absorption in Heavily Doped Silicon – An Empirical Approach


R. Aaron Falk


OptoMetrix, Inc., Renton, WA, USA


Backside failure analysis techniques rely heavily on transmission of near infrared (IR) radiation through the silicon substrate. This statement applies both to emission techniques and active laser probing. Heavy doping of substrates causes them to become highly absorptive in the near IR due to band gap shifts,which effects phonon-assisted absorption, and to free-carrier absorption. Substrate thinning is often required to allow adequate optical transmission. This paper describes an empirical approach to determining the absorption coefficient in a heavily doped substrate and use of the coefficient in determining the amount of substrate thinning required.


Absorption coefficients versus wavelength and carrier density are necessary to determine the amount of thinning required for a particular measurement.


First principle analysis of absorption in doped silicon has been performed using complex computer models


[1]. Use of these models by the “on-the-line” failure analysis engineer is not generally tractable, however.


This paper presents results from an empirical approach to modeling optical absorption in heavily doped silicon. The model uses known scaling laws and parameter fitting to experimental data. The derived absorption curves fit the available experimental data within 10%. The empirical model has been placed into a simple spreadsheet, which calculates thinning requirements and displays absorption curves.


Experimental Data


An empirical model utilizes known scaling laws as its foundation. These scaling laws will have a set of unknown coefficients, which must then be fit to experimental data. The measurements of S. E. Aw, et al. [2] form the basis for our model. Their paper appears to be the most recent experimental results of optical absorption in doped silicon. The description of the experimental procedures and the comparison of


results to other data [3-5] indicate that this data is fairly reliable.


One area of uncertainty is the reliability of Aw et al.’s method for determining the dopant density. They indicate that these dopant concentrations were determined from the resistivities as measured by the“standard four-point probe technique”. Neither an uncertainty, nor potential for an offset bias in this measurement is given by Aw et al.


One typographical error is noted in Aw et al. In their Figure 1, a dopant density of 1.6x1017is listed.


However, their Table 1 and Figure 4 both indicate a dopant density of 1.6x1018. Analysis of the free carrier absorption portion of their absorption curve(see below) indicates that the second value must be correct. The value listed in Figure 1 is assumed to be a misprint, being off by a factor of 10.


Empirical Model


Phonon-Assisted Absorption


The two main optical absorption effects for doped silicon in the near IR are phonon-assisted absorption and free carrier absorption. As silicon is not a direct band-gap material, direct promotion of an electron from the valence to the conduction band can only occur with the aid of a phonon. Aw et al. present a theoretical framework for the phonon-assisted absorption, which coupled with their experimental results, yields the semi-empirical formula


)


(E


k ph0pa


2 1pa


Δ


−


α


for


) 0


E ph0


>


,


(1)


else 0=α ,


where αpais the phonon-assisted absorption, kpais a constant, Ephis the photon energy, E0is a constant,and ΔE(ρ) is an energy shift dependent on the dopant density, ρ. The constant, kpais determined empirically from Figure 3 of Aw et al. to be 58 (1/eV*cm1/2). E0is primarily the bandgap energy, however, other


contributions include the longitudinal acoustic phonon energy. It has an empirical value of 1.09 (eV)The shift in band-gap, ΔE(ρ), was found by Aw et al.


to fit the empirical formula


k


ρ , (2)where kρ has a value of -1.0x10-8(eV*cm) for both n and p doping. No theoretical foundation for this scaling law is given, however, Figure 4 of Aw et al.


shows that the fit is very good for their data and in reasonable agreement with other experimental results. Figures 1 and 2 show plots of Eqs. 1 and 2 respectively.


Free Carrier Absorption


In addition to phonon-assisted absorption, photons can be absorbed by the free carriers in the semiconductor substrate. This effect is simply plasma absorption and is characterized by the Drude equation


h


,e


e fc


e Nk λ=


, (3)where kfcis a constant dependent on the free carrier effective mass and mobility, λ is the optical wavelength, and N is the free carrier density. The superscripts, e and h, stand for electrons and holes respectively. In the case of a substrate with no carrier depletion effects and moderate to high dopant density, the free carrier density is essentially equal to the dopant density. In this case, Eq. 3 can be rewritten as


p


,n


n fc


,nk


λ


. (4)At wavelengths longer than ~ 1.5 micron, the absorption coefficients plotted in Figures 1 and 2 of Aw et al. are essentially all due to free carrier absorption. The wavelength squared and linear density scaling given in Eq. 4 fits the data very well in this wavelength region. Again, kfccan be empirically extracted from the data and is found to be


3.3x10-18(cm2/μm2) for p doping and 3.5x10-18(cm2/μm2) for n doping.


Total Absorption


The total absorption is the sum of the two effects,phonon-assisted absorption and free carrier absorption. The above equations with the empirically derived coefficients were incorporated into an Excel spread sheet with the results shown in Figures 3-5. A conversion factor of 1.243 (um/eV) is used to convert from photon energy to wavelength.


Figure 3 shows the relative contribution of each of the two absorption effects for a carrier density of 1x1019(1/cm3). As can be seen, free carrier absorption begins to dominate the absorption at wavelengths longer than 1.030 micron. This crossover point moves to shorter wavelengths as the carrier density is increased.


Figures 4 and 5 show the total absorption coefficient for a range of p and n dopant densities. The agreement between this empirical formalism and the data is generally better than 10% as shown in the example in Figure 6. An exception is for the lower p dopant values and wavelengths around 1.2 micron. A dip occurs in the experimental data at this point that cannot be explained by the two absorption effects. In this limited region, the empirical result will over estimate the absorption coefficient.


In all cases care should be used in applying these results to a depletion region. The free carrier and dopant densities are not necessarily proportional in such a region.


An Example


Many laser based backside-imaging tools utilize YAG lasers, which operate at a wavelength of 1.064 micron. Figures 7 and 8 show the empirically derived absorption coefficient at this wavelength versus n and p dopant levels respectively. To use these coefficients to determine the transmission through substrate, the formula


( )


exp


R


T2


(5)is applied, where R is the surface reflectivity, d is the substrate thickness in centimeters. The factor of two in the exponential accounts for the double pass through the substrate. Use of an anti-reflection coating to reduce R to less than 0.01 is common.


A nominal wafer thickness of 0.1 centimeter with a p dopant level of 1x1019and a negligible surface reflectance is assumed. For this case Eq. 5 combined with absorption coefficient in Figure 8 indicate a transmission of ~ 6x10-7! Clearly some thinning of the substrate would be required in this example. In most optical instruments a certain fraction, f, of the input illumination must be returned. The thinned thickness required in order to achieve this fractional transmission is given by


α−


≤2R1fln


. (6)


Continuing our example, if f needs to be 10%, then the substrate must be thinned to less than 160 microns.


An empirical model for determining the absorption in doped silicon is presented. The model utilizes simple closed form expressions and four parameters that are derived from experimental data. The model can be readily put into an spreadsheet and utilized to determine thinning requirements for backside analysis of heavily doped substrates.


The author wishes to acknowledge the technical discussions on this 民topic with Dr. Paiboon Tangyunyong and Dr. Daniel L. Barton.


1. P. Tangyunyong and D. Barton, Sandia National Laboratories, private communication.


2. S.E. Aw, H.S. Tan, and C.K. Ong, “Optical Absorption Measurements of Band-Gap Shrinkage in Moderately and Heavily Doped Silicon,” J. Phys. Condensed Matter 3, 8213-23(1991)


3. J. Wagner, “Photoluminescence and Excitation Spectroscopy in Heavily Doped n- and p-type Silicon,” Phys. Rev. B 29, 2002-9 (1984)


4. A. Borgheshi, Chen Chen-Jai, G. Guizzetti, F.


Marabelli, L. Nosenzo, E. Regussoni, A. Stella,and P. Ostoja, “Infra-Red Properties of Bulk Heavily Doped Silicon,” Il Nuovo Cimento 5D,292-303 (1985)


5. G. e. Jellison, Jr. F. A. Modine, C. W. White, R.


F. Wood, and R. T. Young, “ Optical Properties of Heavily Doped Silicon between 1.5 and 4.1 eV,” Phys. Rev. Letters 46, 1414-7 (1981)


1.0E-03


1.0E-02


Magnitude of Band Gap Shift (ev)1.0E-01


1.0E+00


1.0E+17


1.0E+18


1.0E+19


1.0E+20


Dopant Density (1/cm3)


Figure 1 Graph of magnitude of band-gap shift versus n or p dopant density.


0.0


2.0


84.0


6.0


2)(1/cm1/


8.0


12.0


14.0


16.0


1.05


1.10


1.15


1.20


1.25


1.30


Photon Energy (eV)


1.00E+17


1.00E+18一△1.00E+19*-1.00E+20


Figure 2 Graph of square root of absorption coefficient versus photon energy for phonon-assisted absorption.


1.0


100.0


α (1/cm)


1000.0


|||||+|+||Free Carrier |
|---|---|---|---|---|---|---|---|

|||||、|、||Free Carrier |

|||||、 k|、 k||Free Carrier |

||||||||Total |

|||||1|1||Total |

|||||、|、|||

|.9 |1.0 |1.1 |1.2 1.3 ||1.4 |1.5 |1. |

||||Wavelength |(μm) ||||

Phonon


Figure 3 Absorption coefficient versus wavelength as derived from empirical formulas for a p dopant density of 1x1019(1/cm3).


0.1


1.0α (1/cm)10.0


|||||||||X||
|---|---|---|---|---|---|---|---|---|---|

||00|D0|MAAAA44|MAAAA44||X8RX|*XXXx8|||

||||||||||--|

||||||||通|1|1|

|||||||量 晋 路||||

||1.00E+17 1.00E+18 |1.00E+17 1.00E+18 |1.00E+17 1.00E+18 |||||||

||1.00E+17 1.00E+18 |1.00E+17 1.00E+18 |1.00E+17 1.00E+18 |1.00E+19 1.00E+20 |1.00E+19 1.00E+20 |1.00E+19 1.00E+20 ||||

0.9


1.1


1.2


1.3


1.4


1.6


Figure 4 Absorption coefficient versus wavelength with p dopant level as a parameter.


α (1/cm)10.0


||||||||
|---|---|---|---|---|---|---|

||||||*> 288||

|||||公公(*|||

||||||-1||

||||H 鲁|D H 播|||

|1.00E+17 1.00E+18 1.00E+19 1.00E+20 |1.00E+17 1.00E+18 1.00E+19 1.00E+20 ||||||

Figure 5 Absorption coefficient versus wavelength with n dopant level as a parameter.


fficient versus wavelength with n dopant level as a parameter.


|||||Model Aw et al. - 7.3E18 |Model Aw et al. - 7.3E18 |Model Aw et al. - 7.3E18 ||
|---|---|---|---|---|---|---|---|

|9 |1.0 |1.0 |1.1 |1.1 |Model Aw et al. - 7.3E18 |Model Aw et al. - 7.3E18 |1.2 |

||||||Model Aw et al. - 7.3E18 |Model Aw et al. - 7.3E18 |Wavelength |

10α (1/cm)100 1000


0.


.6


Figure 6 Example fit to Aw et al.


(α1/cm)10.0


Figure 7 Absorption coefficient versus p dopant density for a wavelength of ~1.064 μm.


Figure 8 Absorption coefficient versus n dopant density for a wavelength of ~1.064 μm.


p 129-135


DOI: 10.1361/cp2000istfa129


Embedded SRAM Bitmapping and Failure Analysis for Manufacturing Yield Improvement


Jean-Yves Glacet and Fourmun Lee


Motorola Inc., Chandler, Arizona


SRAM bitmapping and failure analysis have been


used as a driver for continuous yield improvementMotorola's MPC555 during pre-qualification manufacturing of a microPowerPC Microcontroller


controller. The combination of the embedded SRAM electrical failure data and failure analysis results was used to generate a pareto of failure modes and failure mechanisms and establish a correlation between the


N V 00 ad O1 1


DPTRAM1。dVna0


8V09


0IOLM00nW


SV0 N光


two. Bitmap trend charts can be used as a manufacturing line monitoring tool to supplement traditional in-line inspection. Identification of manufacturing issues can be obtained from bit failure information


SRAM


and compared with in-line inspection results to


192Kth299X


10K


quickly identify which specific process module is


FLASHFLASH


responsible for a significant yield loss.


16K


L2U BBC


PPC CORE


USIU


SRAM memories have been used frequently as drivers for process yield improvement [1-2]. The benefits are that memories are highly dense and therefore very sensitive to manufacturing defects. Memory arrays can be bitmapped during electrical test in order to precisely identify a failure location. This is a very significant advantage for failure analysis which is a key tool for determination of process issues and to facilitate yield enhancement.


We applied this methodology for continuous yield improvement of a microcontroller using its embedded SRAM. The device is a 32-bit PowerPCTMmicrocontroller with 448Kbyte Flash EEPROM and 26Kbyte SRAM embedded memory. It is manufactured using a triple metal double poly technology. Figure 1 shows a picture of the die layout with the location of the SRAM module. It is composed of a 16 Kbyte SRAM and a 10 Kbyte SRAM. Each array is made of 2 Kbyte blocks. The whole SRAM represents 12% of the die area.


This paper describes the implementation of the embedded SRAM bitmapping and the results obtained during production. It presents the failure analysis methodology and the correlation obtained between


the failure modes observed at bitmapping and the defects responsible for failure. It concludes with the application to yield monitoring.


Figure 1 Microcontroller die layout showing location of the embedded SRAM.


SRAM Bitmapping Tools


Figure 2 represents the SRAM bitmapping sequence and the associated tools. Bitmapping is performed after the production electrical test at wafer probe.


SRAM failing dice are tested with a bitmapping program which generates a bitmap file for each 2K block of each memory array. These files can be displayed with a typical tester platform bitmap viewer in order to extract column and row address of failing cells.


However, this procedure is very time consuming since it is done manually, and is not practical and compatible with a production environment. A device specific translator was written to automatically process the bitmap files from a given wafer after probe and generate two new files. The first one is a text


formatted summary file which contains several pieces of data: die X,Y probe coordinates on the wafer,failing SRAM block number, failure mode class, column and row numbers, and physical X,Y coordinates of failure site on the wafer. The failure modes are classified as follows: block, multiple column, multiple row, single column, single row, partial column,partial row, double bit column, double bit row, and single bit. All the data is sorted in order to obtain a table with a description summary of all the failures for each die.


The second file is created in a standard defect file format (klarf file) and contains all the SRAM failure site information such as the wafer map shown in Figure 3. It can be loaded and processed in any kind of software which is compatible with the klarf format.


We used this file with the Yield Management System and Maskview applications.


The Yield Management software can be used for various types of analysis based on the wafer map and the characteristics of the SRAM failures in the same way as a regular defect file. For example, it can display paretos of SRAM failure modes per wafer and overlay SRAM failure sites with defect sites found during in-line inspection.


Figure 2 SRAM bitmapping sequence and associated tools.


Figure 3 Wafer map of SRAM failure sites obtained from translation of bitmap files into a defect file.


We used the Maskview software to display SRAM failure sites on the die layout (see Figure 4) and for CAD navigation during failure analysis. With this feature, it was possible to automatically drive the failure analysis equipment stage (optical microscope,SEM, FIB) to a specific SRAM failure site.


Figure 4 Overlay of SRAM single bit failure site on die layout.


The implementation of the bitmapping was done with a new product. It was therefore necessary to validate the embedded SRAM bitmap test program of the microcontroller, and the failure sites characteristics given by the bitmap file translator, before application during production probe. This was achieved by performing failure analysis on low yielding wafers to confirm that the defect sites responsible for the failures were in accordance (failure mode, block number,column and row numbers, physical location on wafer) with the results generated by the translator.


Failure Analysis Methodology


The SRAM failure analysis was based on investigating the results provided by the bitmap translator summary and defect files, study of the in-line inspection data when available, use of a whole 8" inch wafer deprocessing technique associated with an inspection method driven by CAD navigation, and some other failure analysis techniques (see Figure 5).


SRAM failure wafer maps and pareto diagrams of failure modes per wafer were obtained using the bitmap defect file with the Yield Management application. It quickly provided an overview of the different failure types. By superimposing the SRAM failures wafer map and the in-line inspection defect map,it was possible to identify a potential in-line defect responsible for a failure.


Analysis of the SRAM failure summary file was necessary to get a better understanding of the failure modes. The results provided by the bitmap test program required in some cases an interpretation of the data: a single defect may cause several failure modes,there may be several defects on the same die with different failure modes, a typical failure mode may not fall into one of the predefined categories or may show a specific pattern (number or repetition of multiple columns), or a failure mode may not appear in a simple form of classification (many adjacent singles bits instead of a partial or single column). Overall,the summary file was helpful in providing a detailed signature of the type of failure.


Once this analysis was done, the wafer was inspected using an optical microscope and navigation with the bitmap defect file and Maskview. With this technique, each failing die on the entire wafer can be inspected very quickly. The ability to zoom in the die layout and overlay the SRAM failure site provides the ability to check the exact location of a visible defect. For cases such as column/row/block failures which may occur in many different locations, additional techniques were employed during the analysis.


SRAM leakage was checked by electrical microprobing and located using liquid crystal or light emission microscopy techniques. FIB contrast imaging was also employed to identify opens and shorts.


However, most of the remaining failure analysis was handled by selective chemical deprocessing of the whole 8" wafer and optical or SEM inspection of the different layers at each failure site with the help of navigation. As a result, many sites could be inspected at each deprocessing step performed on two wafers simultaneously. The number of sites to be checked decreases with the progression of the analysis after some defects have been found in previous layers. The type of failure mode and the in-line inspection data provide additional information to where the defects maybe be located reducing some of the inspection steps. Overall, this approach appeared to be more productive than breaking the wafer followed by a deprocessing of each individual die especially when there was a large number of dice to be analyzed.


SRAM failure summary file


SRAM failure


defect file


Electrical microprobing Liquid crystal microscopy Light emission microscopy FIB contrast imaging


Whole wafer step by step chemical deprocessing Navigation driven Optical and SEM


Inspection


In-line inspection


file


Figure 5 SRAM failure analysis methodology.


Pareto of Failure Modes and Mechanisms – Correlation


SRAM bitmapping and failure analysis was implemented as part of a continuous yield improvement program during pre-production debug of the microntroller. Samples were submitted regularly and results based on failure modes and failure mechanisms were stored in a simple data base. The goal was to accumulate enough data in order to determine the main issues impacting yield on the technology and to obtain sufficient historical data in order to rapidly identify a process problem after bitmapping.


Figure 6 shows a pareto diagram of failure modes determined by SRAM bitmapping on a series of lots.


It gives a visualization of the bitmap failure trend and the contribution of each failure mode to the overall SRAM yield loss.


Figure 7 represents a second pareto diagram obtained from failure analysis of the same wafers. For simplification of the results, the layers where the defect responsible for a SRAM failure occurred are indicated. The defective layers have been grouped by category, when applicable (metal, via), that gives a trend regarding which process modules impact most significantly manufacturing yield. A detailed pareto of failure mechanisms for each wafer analyzed was provided as a feedback to manufacturing.


The combination of these results and in-line inspection data was used to identify process issues and prioritize corrective actions. From these two figures, one can see that the most significant failure modes were single/multiple columns failures as well as single bits, and that a majority of defects were located at metal and poly 2 levels.


In order to establish a more accurate relationship between failure modes and failure location, a systematic correlation was performed for each wafer analyzed. The results are summarized in Figure 8. The upper diagram represents the relative contribution of each layer, where the failure site was found, to a given failure mode. It shows that some individual layers are highly related to specific failure modes and that, in other cases, it is a combination of several layers. This is due partly to the design of the SRAM, the location of the failure site with respect to the memory array, and the manufacturing process. For example,the location of a poly defect inside the array or at the periphery will produce a different type of failure.


Metal 3, which is used for column bitlines, will impact significantly column failures in case of a manufacturing issue, but other defective layers may contribute as well. The lower diagram in Figure 8, which represents the same correlation but in absolute value,is helpful in assessing the real contribution of a given defect to a specific failure mode. A high percentage may not be as significant as it appears on a relative scale if it was found on a very small number of dice.


To complete these results, a summary of the typical failure modes with the corresponding failure mechanisms and failure location based on SRAM bitmapping and failure analysis is shown in Table 1. "Array"indicates that the failure occurred in the memory cells, and "periphery" means that is was located in the external logic of the SRAM (column and row decoders, sense amplifier, circuitry accessing the SRAM).


Base on the experiment result, HCL / HF molarity ratio of 1.5:1 at 45 degree C for 5 minutes can remove both nitride liner and cobalt silicide effectively without loosing the integrity of STI and spacer. For KOH ECW etch optimization, the result shows at 65 degree C, 10M agitated KOH solution with bias of 4.5V, 1.5A and keeping the sample to platinum cathod separation within 1 to 2 inches will obtain the best result for removing 0.18um dualdoped poly gate.


De-process Flow


The recommended de-process flow for leaky gate identification in deep sub-micron CMOS device:


1. Remove inter dielectric layer and metal layer above metal 1 by parallel lapping


2. Perform M1 level PVC by checking with circuit layout.


3. Polish to remove M1 then submerge sample into pad etch for 3 mins to strip PSG layer, metal etch to remove tungsten contact and local interconnect.


4. Inspect sample with SEM to check for anomaly at contact regions (non-silicided, contact spiking,misalignment etc.)


5. Submerge sample into silicide and nitride removal etch (1.5M HCl plus 1M HF at 45 deg C).


6. Perform SEM or optical inspection to make sure silicide and nitride has been removed successfully.


7. Apply KOH ECW etch analysis for 6 mins at 65C with described setup.


8. SEM to identify the leaky gate.


Due to the high SiO2 to SiN selectivity in pad etchant, nitride liner covering poly and diffusion area will be preserved after pad etch. The followed-up metal etch will let analyst inspect particles or junction related damage before checking any gate related failures (refer to Figure 5). Since SiO2 dielectric layer will be removed by pad etch but cells are still protected by nitride liner, larger inspection area can be achieved for defect identification without


co-planarity issues during parallel lap.


Figure 5 SiN liner still covered on top of sample after pad etch.


Figure 6 After HF/HCl chemical dip, silicide and nitride liner has been successfully removed.


A 168 hours dynamic burn-in (150C/2V/1MHz)failure with static Iddq leakage ~ 350μA was submitted for failure analysis. Dynamic emission microscopy analysis located four suspected emission spots on the failing unit. Since traditional Si based CCD spectrum was incapable of detecting black body radiation, metal bridging related failure was excluded. After the rejected unit was parallel lapped down to Metal 1, passive voltage contrast was performed for identifying the leaky poly gate. By analyzing the circuit layout, one of the M1 connecting two poly gates which was supposed to be floating was observed shorting to substrate under SEM inspection, i.e. the pointed M1 should be brighter, but showed darker under M1 PVC analysis(refer to Figure 7 and Figure 8).


Figure 7 Circuit layout showed the highlighted M1


only connecting to two poly gates.


Figure 8 The gate shorted to substrate was identified


by performing M1 level passive


voltage contrast.


Figure 9 Two leaky gates were identified by KOH ECW etch analysis.


By applying KOH ECW etch, both gates tied to M1 was confirmed shorting to substrate. The finding of KOH etch agree with the interpretation of the M1 PVC analysis. Further de-processing proved the physical damage at silicon under the gate.


For another suspected location, M1 PVC analysis did not observe any contrast anomaly by checking with the circuit layout. The leaky gate cannot be observed due to M1 was tied to P+ body contact; therefore,KOH ECW etch was performed to identify the leaky gate. By applying KOH ECW etch at 4.5V, 1.5A at 65C for 6 mins, the leaky poly gate was located under SEM. The physical damage at substrate was clearly shown after stripping the oxide layer (refer to Figure


10 and Figure 11).


Figure 10 Area view of the failing location: the leaky poly gate was preserved by KOH electrolyte etch analysis.


Figure 11a Close-up of the leaky gate.


Figure 11b AFM image of the defect


under poly gate.


With this case study, by combining KOH ECW etch and M1 PVC techniques, all four gate leakage locations from a burn-in rejected unit with Iddq = 350μA has been identified.


We have proved the newly developed etch recipe (1M HF plus 1.5 M of HCl at 50C for 5 mins) can efficiently remove silicide and nitride liner. This made the KOH electrochemical method for leaky gate identification possible for the 0.18um deep submicron CMOS logic device. The proposed deprocess flow also help reduce de-process rework and improve overall successful rate for leaky gate detection.


In addition to KOH electrochemical etch, passive voltage contrast at metal 1 was also purposed for localizing defective poly gates. Case study confirmed the 0.18μm CMOS leaky poly gate can be successfully localized by incorporation passive voltage contrast and KOH electrolyte etch.


1. N. Ohtani and T. Katayama: Detection of Gate Oxide Defects Using Electrochemical Wet Etching in KOH:H2O Solution; 279-283, Proc.


of the ISTFA (1997)


2. D.S. Patrick and L.C. Wagner et al.: ATE Failure Isolation Methodologies for Failure Analysis,Design Debug and Yield Enhancement; 235-244,Proc. of the ISTFA, (1998)


3. Akira Nishikawa el al.: An application of Passive Voltage Contrast (PVC) to Failure Analysis of CMOS LSI IC Using Secondary Electron Collection; 239-244, Proc. Of the ISTFA, (1999)


4. Jim Schlueter: CMP and Shallow Trench Isolation; 123-130, Semiconductor International(October, 1999)


5. N. Borghol and T. Haddock: Locating Defective Gates Using SEM Charge Contrast With Parallel Polishing; 213, Proc. of the ISTFA (1993)


6. M. R. Baklanov and I.A. Badmaeva el al.:Kinetics and Mechanism of the Etching of CoSi2 in HF-based Solutions; J. Electrochemical Society, 3245-3251, Vol 143 No.10 (1996)


7. M. R. Baklanov and E. Kondoh el al.: Limitation of HF-Based Chemistry for Deep-Submicron Contact Hole Cleaning on Silicide; J.


Electrochemical Society, 3240-3246, Vol 145 No 9 (1998)


8. Lai-Cheng Chen and Minjan Chen el al.: The Band Model and the Etching Mechanism of Silicon in Aqueous KOH; J. Electrochemical Society, 170-176, Vol. 142, No 1 (1995)


9. Genichi Taguchiel al: Robust Engineering,McGraw-Hill Inc. (1999)


p 147-151


DOI: 10.1361/cp2000istfa147


UV Reflectance Spectroscopy of the Copper/Copper Oxide System for Assessment of Solderability


L. Forney, C. Thierolf, B. Toleno, G. Parks


American Competitiveness Institute, Philadelphia, PA, USA


Surface changes of copper and copper coupons coated with organic solderability preservative (OSP)after accelerated aging were measured using UV Differential Reflectance Spectroscopy. A chemometric method has been developed that allows correlation of the spectroscopic results with independent measurements of the solderability of the copper and copper/OSP coupons using a wetting balance or sequential electrochemical reduction analysis (SERA). Based on the results of this study,a versatile instrument for the assessment of the solderability of printed wiring boards has been demonstrated. The instrument is currently in beta testing at several locations.


Copper readily oxidizes in air, forming a surface layer of mixed cuprous and cupric oxides. The resultant alteration in surface chemistry is directly observable as a visible change in the appearance of the copper surface. It has also been shown that the surface formation of copper oxides on a copper surface alters the ultraviolet (UV) reflectance spectra through an optical interference phenomena. The resultant interference spectrum combines the reflectance from the surface of the oxide layer with the reflectance from the surface of the underlying copper, and allows direct calculation of the thickness of the oxide layer.


The surface oxide layer also impacts the functional properties of copper metal, including the wetting contact angle of molten solder (eutectic tin/lead alloy) on the copper surface. This solder wetting property is of paramount importance in the formation of a strong reliable solder joint. Accordingly, the electronics industry has developed a standardized test method based on the copper/solder contact angle in order to assess the “solderability” of electronic components.


The copper for soldered connections is usually protected against oxidation by prior application of a protective, solderable material to retard or prevent copper oxidation. Common protective materials include a precoat of hot air-leveled solder (HASL),immersion silver (IAg), electroless nickel over immersion gold (ENiG), or an organic solderability preservative (OSP). Commercially available OSP,usually a substituted benzimidazole compound,adheres to the copper surface by complexing with copper ions to form a stable organometallic structure.


When heated in the presence of a suitable solder flux,the copper-benzimidazole complex is displaced,exposing the copper surface for solder wetting and bonding.


Unfortunately, the OSP coating on copper is transparent, so that a simple visual observation is not adequate to assess the extent of OSP surface coverage or coating uniformity. Furthermore, OSP has an indeterminate lifetime that varies according to environmental storage conditions, usually in the range of 6 to 18 months. Because of the nature of the chemometric method utilized, it is not certain whether the derived relative absorbance value is an expression of the copper-copper oxide system or the OSP system (i.e., yellowing, polymerization,carmelization, etc).


For these reasons, we explored the application of UV reflectance spectroscopy to the study of the OSPcopper/copper oxide system. The goal of the study was to determine the origin of the spectral changes in this system and correlate these changes to solderability.


Materials and Methods


UV-Visible reflectance spectra were obtained using a Pentium processor to control an Ocean Optics SD2000 dual fiber spectrometer and DT-1000S tungsten-deuterium light source impinging a 5.3mm2 area normal to the target through a fiber optic probe,with automatic referencing to a Labsphere diffuse white reference standard. The probe placement is monitored using a 7mm Elmo-QN42HL micro


camera with a 4mm lens mounted in the probe holder a 45° angle to the target. Internal background intensity calibration utilizes the constant silicontungsten absorbance peak at 655nm.


OSP studies utilized standard 1” x 2” x .027” test coupons, coated with Entek Plus CU-106A(a benzimidazole derivative) by Raytheon Systems Company with an OSP thickness of 0.21μm. Bare copper samples were cut from 1” x 0.022” industrial copper foil and pickled with 10% H2SO4 to remove oxides and passivating agents. Commercial OSP-coated PCB’s were utilized for some reflow studies. All samples were stored under nitrogen when not actively undergoing aging or analysis.


Accelerated aging methods included a (1) dry air(convection oven) at 150 ± 1°C, (2) humidity chamber set to 85°C at 85% relative humidity, and


(3) repeated passes through an Omniflo7 Electrovert Convection Reflow Oven using a time/temperature profile typical for PCB reflow operations, with a maximum temperature zone of 240°C for 42 seconds,in air.


Solderability was assessed by measuring the solder wetting and electrochemical reduction potential of the test piece. A Multicore Must-II wetting balance was used with 63/37 Sn/Pb solder at 245°C and immersion speed of 10mm/sec to a 5mm depth, with an immersion time of 10sec. Unless noted, the flux was Multicore ACTIEC-5, which contains 5% halide activators. The criteria for wetting is the time in seconds to achieve a 90° contact angle following sample immersion. Sequential electrochemical reduction analysis (SERA) was performed using an ECI Technology QC-100 chronopotentiometer with a de-aerated, pH 8.4 solution of borate buffer at a current density of 50μA/cm2. In appropriate systems the plateau voltage reflects the nature of a metal oxide, the charge passed is a measure of the amount of oxide present and, for OSP coated copper, the final voltage is a measure of the integrity of the OSP coating.


Bare Copper (Cu°)


The reflectance spectra of bare copper (Cu°) rapidly undergoes marked changes in the UV-Visible region upon heating. This is consistent with the visible color changes of copper that are readily apparent to the naked eye upon ambient aging or heating. The various colors which develop on copper during oxidation have been assigned to specific thicknesses of a growing oxide layer. The UV-Visible spectrum of Cu° is characterized initially by formation of an absorbance peak at 420nm after 5 minutes at 150°C,as shown in Figure 2. This is not a fixed absorbance


however, and with additional time the peak intensity increases and the peak maximum shifts to higher wavelength, reaching a maximum intensity at approximately 500nm in 12 minutes. The absorbance at 500nm is consistent with the yellow color of copper as it oxidizes under these conditions. At longer heating times, the peak maximum decreases in intensity and continues to shift to higher wavelengths until, after 25 minutes at 150°C, the peak is found at 640nm.


340 390 440 490 540 590 640


Wavelength(nm)


0 5 10 15 20 25


Figure 2 Cu° aged at 150°C. The predominant feature in the reflectance spectra of Cu° changes in intensity and shifts to higher wavelength with increasing time at 150°C. (baselines corrected for diffusion and slope, and zero points shifted for comparison purposes)


The shift in the wavelength of the major feature of the Cu°-Cu oxide spectra overwhelms the spectral features that can be ascribed to specific chemical species and even the strong diffuse absorption band at 300-550nm, at least in the time period of interest for the determination of solderability parameters. As a result, a straightforward analysis of the oxidation process can be constructed from the shift in the wavelength of the major feature against time, as shown in Figure 3. It is not necessary to rely on relationships between relative intensities at given wavelengths ascribable to specific chemical groups.


This spectral pattern of wavelength shift suggests that the primary observed process is related to interference phenomena, where the spectral response is determined by the thickness of an optically transparent or translucent layer such as copper oxide.


minutes


Interference patterns in the Cu°-Cu oxide system were first studied by Hummel in 1975.


Subsequently, Urban et al demonstrated that the longest wavelength peak of the interference spectrum can be calculated from the expression:


λ ≅ 5nd


where:


λ = the wavelength of the major spectral feature


n = the index of refraction of the oxide (reported as


1.6 for copper oxides, per Urban, although other workers report this value variously, up to 2.7)d = the thickness of the oxide layer (nm)


Inserting an index value of 1.6 into this expression with the major interference peak absorbance ranging from 350 to 600nm region, the oxide thickness is calculated to increase from 37 to 75nm. Using an index value of 2.7, the calculation indicates an oxide thickness of 22 to 44nm. Independent thickness calculations derived from the measured reduction potential (SERA) are in reasonable agreement with these numbers, indicating a maximum oxide thickness of 200nm from the same aged samples.


300 350 400 450 500 550 600


Minutes at 150C


Figure 3 Cu° aged at 150°C


Plot of the wavelength of the major spectral feature against time


OSP-Copper


The oxidation of Cu° provides invaluable insight for the spectral interpretation of the Cu°-Cu oxide system, but is of limited direct practical value to the PCB manufacturer who is concerned about the solderability of copper that has been coated to retard or prevent oxidation. For this reason, our studies mainly concentrated on the interpretation of the spectra of OSP-coated copper.


Analysis of the reflectance spectra of OSP-coated copper is more complex than that of Cu°. A corresponding shift of wavelengths through the 350-600nm region is found to occur with aging, and


this strongly suggests that optical interference phenomena are an important feature of this system also. However, the intensity of the observed peaks are reduced to about 10% of that observed with bare copper. As a result there is much more interference from the background diffusion band of copper and there is no major spectral feature which can be clearly followed as it shifts across the measurement range. The problem is illustrated by comparison of the strong features of the Cu° system (Figure 2) with the weaker peaks of the OSP-Cu samples shown in Figure 4.


350 400 450 500 550 600 650


Wavelength (nm)


0 30 45 75 120 180


Figure 4 OSP-Cu aged at 150°C


Changes in the reflectance spectra of OSP-Cu upon oxidation at 150°C are complex, and features are less pronounced than are observed with Cu°. (baselines corrected for diffusion and slope, and zero points shifted for clarity)


Analytical Method


The analysis of the OSP-coated Cu spectra is derived from the interpretation of the interference spectrum.


It utilizes two reference wavelengths to follow the aging process in the oxide region (350-600nm). The absorption at 450nm is taken as a measure of initial oxidation processes, and the absorption at 540nm is taken as a measure of later oxidation processes. For the analysis, the raw spectra are corrected for baseline shift and slope, and then the absorption at 540nm is subtracted from the absorption at 450nm to yield a relative absorbance. The relative absorbance,which may be either positive or negative due to the baseline correction and peak intensity ratios, is quite sensitive to the spectral disturbance caused by residual copper oxide interference phenomena.


Benzimidazole exhibits a diagnostic peak at 270nm, a wavelength that is transparent to the other species in the system and is itself free from interference patterns. The decrease in absorption at 270nm upon heat aging of benzimidazole coatings is consistent with the “deterioration or reorganization” that has


been inferred from the increasing final voltage found in prior SERA aging studies. Such OSP aging processes may include the slow volatilization of the benzimidazole under the heating conditions,polymerization, or chemical changes that alter the energy state of the benzimidazole or its copper complex. When held at 150°C for ≥50 hours, the benzimidazole absorbance at 270nm disappears entirely.


Data for coupons with a 0.21μm layer of benzimidazole, aged at 150°C, are shown in Figure 5.


The unusual shape of the curve plotted against time reflects the interference pattern which overlays the discrete wavelength absorbances of the copper oxides. At even longer time periods the relative absorbance value exhibits a cyclic pattern, typical of interference spectra. Fortunately, in the coppercopper oxide system it is the first cycle that is diagnostic for solderability.


-0.04-0.02


0.02


0.04


0 30 60 90 120 150 180


Minutesat150C


Figure 5 OSP-Cu Aged at 150°C


The Relative Absorbance provides a diagnostic measure of surface changes related to solderability.


To calibrate the relative absorbance value against solderability, the same 150°C aged coupons were analyzed by their reduction potential (SERA), and solder wetting. Both these measurements of solderability are highly dependent on the substrate and the experimental parameters chosen for the test.


The most effective utilization of these tests, therefore,utilizes conditions under which the maximum rate of change against time occurs at the boundary between good and poor solderability. As shown by Figure 6,it can be seen that the maximum rate of change in both the reduction potential and solder wetting occurs at approximately 40 minutes at 150°C. The spectral data are at their most sensitive (most rapid change with aging) in the same spectral region, suggesting that wetting balance, SERA, and spectral


measurements are indeed responding to similar changes in the OSP-copper substrate.


30 60 90 120 150 180Minutes


SERA


Wetting Method I Method II


Figure 6 OSP-Cu Aged at 150°C: Comparison of Solder Wetting, Reduction Potential and Spectral Intensity. For clarity, the measured values are scaled to the %-age of their maximum value during the time period of interest


Analysis of test coupons and commercial PCBs passed through a reflow oven from one to ten times gave similar results: Compare the relative absorbance of coupons heated at a steady 150°C for 75 minutes (Figure 5) with the corresponding relative absorbance that occurs after 6-7 reflow passes(Figure 7). In both cases spectral analysis exhibits a similar discontinuous spectral curve, and the regions of greatest sensitivity (maximum change of values with unit aging time) of all these methods overlap.


0 1 2 3 4 5 6 7 8 9 10


Reflows


SERA Vf WET sec Method I Method II


Figure 7 OSP-Cu Aged by Successive Reflow:Comparison of Solder Wetting, Reduction Potential and Spectral Intensity. For clarity, the measured values are scaled to the %-age of their maximum


value during the time period of interest.


Coupons aged at 85°C and 85% relative humidity exhibited a lower rate of oxidative change, as shown in Figure 8. A similar spectral pattern is again seen for all three techniques, in that the spectral values increase in accord with the SERA and wetting balance values. This is true even though the spectral


intensity values are shifted to higher values in the high humidity system (not apparent in Figure 8, as a consequence of normalizing the data).


50 100 150 200 250 300


Hours


SERA Vf Wet (sec)Method I Method II


Figure 8 OSP-Cu Aged at 85°C, 85% Rel. Hum:Comparison of Solder Wetting, Reduction Potential and Spectral Intensity. For clarity, the measured values are scaled to the %-age of their maximum


Based on this and earlier studies, a versatile instrument for the assessment of the solderability of printed wiring boards has been developed. The instrument is currently in beta testing.


Significance of the Work:Conclusions and Benefits


An affordable, rapid, portable, nondestructive technique for the assessment of printed circuit board solderability has been demonstrated and is in field trials.


Keywords (3)


Solderability


Copper oxides


UV Reflectance Spectroscopy


Topical Area


Testing and Device Characterization


1. R.E. Hummel, E.D. Verink, Jr. and C.W.


Shanley, Proc. 6th Int. Congr. Metallic Corrosion,Melbourne, Australia (1975).


2. F.K. Urban III, Dissertation, University of Florida (1981).


3. IPC/ANSI J-Std-003, Section 4.3.1 (1992).


4. J.L. Parker, Jr., Solderability Treatments,Electronic Materials Handbook, vol.1,Packaging, p563, ASM International, Materials Park, OH, 1989.


5. George M. Wenger, Immersion Silver Surface Finish: Usage Requirement Test Results and Production Experience, IPC 3rd Annual National Conference: A Summit on Surface Finishes and PWB Solderability, Proceedings v.1, p.51, 1999,Irvine CA.


6. D. Hillman et al, A Comparison of Immersion Gold/Electroless Nickel, Hot Air Solder Leveled,and Organic Solderability Preservative Surface Finishes, IPC 3rd Annual National Conference: A Summit on Surface Finishes and PWB Solderability, Proceedings v.2, p.21, 1999, Irvine CA.


7. J.D. DeBiase, The Emergence of Substituted Bezimidazole OSP’s, Surface Mount Technology, February 1997.


8. J. B. Cotton, Second Int. Congr. On Metallic Corrosion., New York (1963) p. 590 .


9. R. E. Hummel, E. D. Verink, Jr. and C. W.


10. F. K. Urban III, R. E. Hummel and E. D. Verink,Jr., Differential Reflectometry of Thin Film Metal Oxides on Copper, Tungsten,Molybdenum and Chromium, Corrosion Sci. 22,647 (1982).


11. F. K. Urban III, Dissertation, University of Florida (1981).


12. P. C. Ladelfe, A. W. Czanderna and J. R.


Biegen, Optical Constants of Cupric Oxide from 450 to 800mμ, Thin Solid Films, 10, 403 (1972).


13. F. K. Urban III, Dissertation, University of Florida (1981).


14. P. Bratin, M. Pavlov, G. Chalyt, and R.


Gluzman, New Application of the SERA Method– Assessment of the Protective Effectiveness of Organic Solderability Preservatives, SurFin ’95,Proceedings of Technical Conference, p. 583-589 (June 1995).


p 155-160


DOI: 10.1361/cp2000istfa155


Antireflection Coatings for Semiconductor Failure Analysis


Brennan Davis


Advanced Micro Devices, Austin, TX, USA


Wilson Chi


Advanced Micro Devices, Sunnyvale, CA, USA


Figures 9-13 show some examples of defects responsible for SRAM failures.


SRAM Failure Mode


0%10%20%30%40%50%60%70%80%90%100%


D


Lot


other


sing le b it d oub le b it p artia l row row


multi row p artia l c ol c ol


multi c ol b loc k


Figure 6 Pareto of SRAM failure modes.


SRAM Defect Location


Undetermined


Other


Ac tive


Poly2


ILD0


Via 2/ Via 1/ Conta c t M3/ M2/ M1


Figure 7 Pareto of SRAM defect location.


SRAM Defect Location/Failure Mode Correlation


block multi col col partial col


multi row


row partial row


double


bit


single bit


Failure Mode


Undetermined Other


Active


Contact


Via1


Via2


SRAMDefect Location/Failure Mode Correlation


0.2


0.4


0.6


0.8


block multi col


col partial col


double bit


Figure 8 Correlation between SRAM failure mode and defect location.


Failure mode Failure mechanism Failure location Block M3 pattern


M2 pattern


periphery periphery


Multi column M3 pattern M3 pattern M1 pattern missing Contact Poly2 pattern Active pattern Active pattern


array periphery periphery periphery periphery periphery array


Partial column missing plug at Via2 missing Via2 open Via2


missing Contact


array array array array


Single column M3 pattern M2 pattern Poly2 pattern Poly2 pattern Active pattern


array array periphery array periphery


Multi row ILD2 cmp Poly2 pattern


Partial row missing Via2 missing Via1 missing Contact


array array array


Single row M2 pattern M2 particle Poly2 pattern


array array periphery


Double bit open Via2 missing Via1 M1 pattern missing Contact Poly2 pattern Active pattern


array array array array array array


Single bit ILD0 particle missing Contact Poly2 pattern Active pattern Active implant


array array array array array Table 1 SRAM failure modes, failure mechanisms and failure location obtained from bitmapping and failure analysis.


Figure 9 Metal 3 pattern defect


(multiple column failure).


Figure 10 Missing Via 2 (partial row failure).


Figure 11 Metal 2 pattern defect (row failure).


Figure 12 Missing Contacts (double column failure).


Figure 13 Poly 2 pattern defect (single bit failure).


Application to Yield Monitoring


The purpose of establishing a close correlation between SRAM failure modes and failure mechanisms is to help in finding the origin of yield issues by monitoring bitmap results once sufficient historical data has been obtained. This methodology has the advantage of providing a fast feedback for yield enhancement without performing time consuming failure analysis. It is also complementary to conventional in-line inspection that is becoming limited as smaller and more complex technologies appear.


Estimation of potential defects from a production bitmap trend chart requires knowledge of how much each known failure mechanism is likely to cause a specific failure mode. This information can be deduced from the correlation results shown in figure 8.


To be valid, there must be enough confidence in the results obtained from failure analysis. It means that a large amount of the failure analysis should be successful (70% to 80% in the present case, see Figure 7) in order to obtain some data representative of the current wafer manufacturing. There should also be enough confidence in the correlation results in order


to use the data. For example the SRAM block failure mode indicates 70% of undetermined cause for failure (see Figure 8) because it was the most difficult analysis to perform. Although Metal 3 was a major contributor to block failure, there may be another physical mechanism more relevant. In some cases,the amount of data may be too small to be taken into consideration.


Table 2 represents the most significant failure modes,defect locations, and occurrence (% of total quantity of die analyzed) based on the correlation results. It shows that defectivity at Metal 3 is most likely to produce multiple and single column failures, Metal 2 defects will induce single row failures, Via and Contact defects will produce partial col/row failures, and Poly 2 defectivity will generate single and double bit failures. These are the most likely defect locations to generate a specific failure mode and it confirms what was expected from the SRAM array design. However, we can see that Metal 3, Poly 2, Via 1, Contact and Active defects will impact significantly other failure modes as well.


Analysis of a typical SRAM bitmap trend chart as shown in Figure 14 involves using the bitmapping failure analysis correlation results and the current inline inspection data. If the two are in agreement, the data can pinpoint what impacts the manufacturing yield without doing any failure analysis. In case of a difference or in the absence of in-line inspection data,additional investigations may be performed for confirmation if necessary.


Failure mode


Defect location Occurrence


Block Metal3 21 %Multiple column Metal3


30 %10 %10 %


Single column Metal3 Poly2 Active


53 %18 %18 %


Single Row Metal2 Poly2


50 %37%


Partial column +Partial row


Vias + Contact 100 %Double bit Poly2


25 %10 %10 %10 %


Single bit Poly2 Active Contact


69 %10 %6 %Table 2 Summary of principal failure modes and most likely defect location obtained from bitmapping/failure analysis correlation.


SRAM bitmap trend chart


0 2 4 6 8 10 12


G


b loc k


multi c ol c ol


row


sing le b it doub le b it


Figure 14 SRAM bitmapping trend chart showing variation of failure modes across several wafer lots.


Bitmapping and failure analysis have been performed on the embedded SRAM of a microcontroller product as a driver for yield improvement. The implementation of SRAM bitmapping in production associated with a device specific bitmap file translator was used to automatically extract SRAM electrical failure information and generate a standard defect file of bitmap failures. This data was employed extensively during failure analysis and a correlation between failure mode and failure mechanisms was made. Based on the historical results, SRAM bitmap failure data in combination with in-line inspection data can reveal major issues impacting manufacturing yield.


1. E. Hall, D. DiMarco, P. Berndt, and A. Zandi,“A Structured Approach for Failure Analysis of a 256K BiCMOS SRAM”, Proceedings ISTFA 1989, pp 167-176.


2. F. T. Agricola and K.F. Anderten, “Failure Mode Analysis Methodology on High Density CMOS SRAMS”, Proceedings ISTFA 1989, pp 389-398.


p 137-140


DOI: 10.1361/cp2000istfa137


LSI Process Diagnosis for Device Users


Miki Imai, Daiki Tanaka, Katsuhiko Hosoda, Katsuhumi Noda


Reliability Engineering Department, Oki engineering Co., Ltd., Tokyo, Japan


Sumio Matsuda


Office of Research and Development, NASDA, Japan


Conventional reliability test using accelerated test is not suitable for selection of high-reliability LSI device, because it needs high cost and long testing time. Then observation methods such as construction analysis have been used in a part of the test.


Construction analysis can detect faults on leads,packages wires and chip surfaces. However, recent LSI device structures have multilayers one, and most part of faults exist in inner layers. The faults are due to LSI wafer process imperfection such as inaccurate process design or device structural defects.


LSI process diagnosis has been developed for the quality and reliability evaluation with the observation of device structures. It consists of fault detection and estimation of risk that the faults cause to fail more than one of devices through many manufacturing lots.


Typically, cross sectional SEM for observation and data base or theory of reliability for risk estimation are used in this method.


We device users are enforcing the reliability evaluation test at the device selection/acceptance to secure the reliability in the field. But, this evaluation test needs a long time and the enormous cost.


Furthermore, these evaluation tests have been getting difficult realistically at present which has been improving the quality of devices caused by the performance improvement such as a manufacture device. So, we examine the LSI process diagnosis as the one method of evaluating the quality of devices.


This is a method that evaluates devices by observing the inside of devices. That has an advantage which the defective element can be evaluated in few samples, in a short time, while there is a problem that the proof of the reliability is poor. Examination had made about the method of the LSI process diagnosis,and the possibility of the realization and the validity is described in this paper.


Method of the LSI process diagnosis


It is a part of broad sense-like DPA, and evaluate the quality of devices as the LSI process diagnosis by observing the fault which exists inside devices which is good devices electrically, and the problem in device structure. The LSI process diagnosis is executed in the steps below, the decision of the evaluation item,the observation, the process of the analysis of the data, the diagnosis.


The decision of the evaluation item


The evaluation item is decided from the factor and so on which relates to LSI devices development, the problem in the manufacture, the trouble and the structure.


Observation


The main ways of observing it are the chip surface observation and the devices structure (chip cross section) observation. Optical Microscope (OM) and Scanning Electron Microscope (SEM) are used chiefly for the observation. Transmission Microscope(TEM) and Focused Ion Beam (FIB) were used, if necessary.


The analysis of the data


Examination is made about faults, devices structure,process flow, and so on from the observed result.


And, the data base is being made based on the data that it was accumulated by the failure analytic data,the DPA data, literature, and so on.


Diagnosis


It is estimated that the occurrence source of the fault and risk which reaches the trouble from the data base,literature, and so on, and a fault. The quality of devices are evaluated as a result. As for the data base,it was collected about the thickness of each devices structure, the layer, a fault, and so on. It can get the typical information because the data on many


manufacturers are contained. The devices structure is set up by device manufacturer took the reliability into consideration. The devices which came off greatly from the data base have the possibility that the problem is contained in device structure. And, the danger due to the kind and the size of the fault can be evaluated by making the data base about a fault.


Figure 1 shows an example of the data base. It is the histogram of the thickness of the metallization layer of the 0.6m scale devices. The thickness of the metallization layer in this histogram are distributed around about 0.7m.


When the metallization thickness gets thin,electromigration is easy to occur. Therefore, the thickness of the metallization layer is an important factor. We consider that it is possible to evaluate devices by using the data base like this.


The possibility of the realization of the LSI process diagnosis


The possibility of the realization of the LSI process diagnosis was examined from executing the quality evaluation which the LSI process diagnosis was used for by using devices put on the market.


The fault of the devices structure


The faults observed inside the devices structure in the analysis we had made are shown in the table 1.


The faults in the column of “good” devices in the table were detected in the electrically good sample.


The faults in the column of “failed” samples were detected as trouble factor in the failure analysis. Many faults inhere in good devices as well like this. And,most of the faults observed with good devices are detected as a failed factor. Usually, because it is fully small, these faults don't influence the character of devices and the life. But, it is considered having the possibility that it reaches the trouble when a fault becomes big due to the dispersion in manufacture and so on.


LSI process diagnosis result.


The result of the LSI process diagnosis about devices on the market was shown in the table 2. The observation was carried out about devices of 24 kind.


About 1-3 faults were observed in devices of 13 kind.


These faults aren't so serious as it is connected with the trouble directly. But, it is contained the risk that reaches the trouble due to the dispersion of the manufacture and so on.


There are some devices in which no fault observed.


Therefore, it is possible that the quality of devices is classified by this method.


However, the structure of devices varies in the design,and considered to have the unique structure of the manufacturer. Therefore, the comparison with the information from the devices manufacturer and the discussion with the manufacturer are important.


The validity of the LSI process diagnosis


Both the cost and the time become enormous when the reliability test is enforced in all the samples when 1 kind is chosen from a certain several pieces kinds of devices. Therefore, the LSI process diagnosis is carried out in all the kinds, and the reduction of the cost which the reliability test costs by limiting the kind, a saving of the time become possible.


The problem of the manufacture wafer process of devices was given, and the risk that reaches the trouble, and the possibility of the process diagnosis were collected in the table 3. As for the metallization layer formation which relates to the trouble specially and easily, the insulation layer formation process, and so on, it is understood that it can be observed from here. Therefore, it is the effective method of evaluating it in the metallization layer, the insulation layer. And, the lot evaluation in the reception is possible, too.


On the other hand, devices all can't be observed as for the LSI process diagnosis because it is the method which the SEM observation of the section, the surface is used as for the master. Therefore, it is limited as follows.


1. The fault which exists unanimously, and the fault in structure.


2. The fault which has the size that can be observed.


The LSI process diagnosis is one technique of the method to evaluate the quality of devices, and it can be applied as the selection test in the devices acceptance and the lot evaluation in the reception.


Reference


1. M.Imai, T.Ajioka, K.Noda, D.Tanaka, K.Oka,”Developed of process diagnosis” TECHNICAL REPORTOF IEICE.R97-8(1997-09)


2. M.Imai T.Ajioka, K.Noda, D.Tanaka, K.Oka, ”A Fault analysis for LSI device with a Data base”THE 1998 IEICE GENERAL CONFERENCE SC-11-2(1998-03)


Table1 Faults in good or failed devices


area


Fault


good


failed


Wafer


crystal defect


✓


gate


deformation


reacted layer


coverage


configuration


contact


plug void


interlayer


void


via


grain size


corrosion


nodule


interconnection


hillock


uniformity


planerization


insulator


over etching


lithography alignment


Table 2 Faults observed in the process diagnosis


Sample No.


kind


1 2 3 4 5 6 7 8 9 10 11 12


Contact/via


F F


Inter-connection


foreign material void


13 14 15 16 17 18 19 20 21 22 23 24


foreign material F


The thickness of metallization


0 2 4 6 8 10 12 14 16 18 20


0 0.2 0.4 0.6 0.8 1 1.2 1.4


thickness( μ m )


E M


Figure 1 An example of the data base


Figure 2


Figure 3


Figure 4


Figure 5


Table3 Faults due to wafer process


Manufacturing


Process


Failure Observation


wafer


dispersion, crystal defect, contamination, crack


lithography


alignment, foreign material, contamination


over, shortage, foreign material, contamination


diffusion


abnormal, crystal defect


Inter-connection crack, void, deformation, uniformity, adhesion, contamination,electromigration


crack, pinhole, uniformity, coverage


A B C D


Relation to failure


much --------- little


easy ------ difficult


p 141-146


DOI: 10.1361/cp2000istfa141


Application of KOH Electrochemical Etch and Passive Voltage


Contrast Techniques to Identify Leaky Gate in Deep Submicron CMOS


Fred Y. Chang, Victer Chan


LSI Logic, Fremont, CA, USA


This paper describes a novel de-process flow by combining cobalt silicide / nitride wet etch with KOH electrochemical wet etch (ECW) to identify leaky gate in silicided deep sub-micron process technology.


Traditionally, leaky gate identification requires direct confirmation by gate level electrical or emission detection technique. Ohtani [1] used KOH electrochemical etch application to identify nonsilicided leaky gate capacitor in DRAM without using the above confirmation. The result of the case study demonstrates the expanded application of ECW etch to both silicided 0.18um logic and SRAM devices. Voltage contrast at metal 1 to assist leaky gate localization is also proposed. By combining both techniques, the possibility for isolating gate related defects are greatly enhanced.


Case studies also show the advantages of the proposed technique over conventional poly level voltage contrast in leaky gate identification especially with devices that use local interconnect and nitride liner process.


Since high pin count, high varieties of package types and shorter turn around time are required to deal with today’s ASIC business, most of the failure analysis cases were done by executing dynamic test patterns on testers instead of bench verification for reducing the FA cycle time [2]. However, with advance process technology, emission attenuated by multiple layers of metal, continuous scaling of cell size combine with the vibration from testing environment, making it very difficult to pin point the exact defect location.


The typical structure for modern deep sub-micron CMOS logic device comes with shallow trench isolation (STI) to eliminate field oxide encroachment created by conventional LOCOS structure, nitride linear plus local interconnect (LI) to increase cell density, and nitride spacer to overcome SiO2 spacer over-etch issues. However, adding STI and LI process technologies created problems during die deprocessing. Electron charging at top of the LI can


confuse the analysts in localizing a defective gate.


Due to STI replacement on traditional LOCOS process, dummy poly on field oxide is no longer a good parallel lap reference for performing passive voltage contrast. Both problems have increased the difficulty to pin point the defective poly gate. Figure 1 and Table 1 show the cross section for modern deep sub-micron CMOS device and process flow.


The passive voltage technique sometime can create misleading information if planar surface cannot be achieved by parallel lapping. In addition, if no gate oxide related defect was found after poly removal, the follow-up wet etch for junction checking can also remove the spacer, gate oxide, particles or poly stringer. This could potentially remove the root cause of the problem.


The KOH electrochemical etch application to identify leaky gate capacitor in DRAM was introduced by Ohtani [1]. However, the disadvantage of using KOH electrolyte method is the necessarily of removing silicide on top of poly gate, which made this technique difficult to be applied on logic and SRAM devices with salicide process. Furthermore, without removing the nitride liner covering the top of poly,the limited poly contact exposed area did not give the analyst good SEM visibility to localize the leaky gate when performing KOH ECW analysis.


Figure 1a Cross section of a CMOS device with integration of shallow trench isolation (STI), nitride


spacer and liner, and local interconnect.


Table 1 The summary of 0.18um CMOS process flow.


1. Shallow Trench Isolation: mask, etch and trench fill


2. Well Formation: N/P well masks amd implants, Vt implants


3. Gate Oxide formation ~ 35A


4. Poly Deposition


5. Poly mask and etch


6. LDD Formation


7. Spacer deposition and etch (1000A SiN + 200A liner oxide)


8. Source and Drain formation


9. Cobalt Silicide formation


10. LI SiN etch stop layer deposition: 600A SiN


11. ILD1 PSG deposition and CMP: 6500A


12. LI mask and etch


13. W fill and W CMP


14. ILD2 TEOS deposition 4500A


15. Metal 1 deposition 5000A


Techniques Concepts


M1 Passive voltage contrast (PVC) inspection


Nishikawa et al. have demonstrated the combination of secondary and backscattered electrons in between 1 to 2.5keV will generate the positive charges on top of metal surface [3]. By inspecting Metal 1 layer under SEM at 2 to 2.5 KeV, gates tying together or connecting to n+ junction through M1 will shows metal 1 (M1) charge contrast difference when comparing with those gates having M1 connection to P+ junction. (Whether a leaky gate shows darker or brighter under the SEM is determined by the system setup. In the case we presented, if leaky gate does not link to p+ junction via M1, it will show darker contrast under our SEM system.) As a result, this kind of leaky gate will be easily identified at M1 stage by checking the sample with layout files.


KOH electrochemical etch (ECW)


It was known that by applying positive potential on Si substrate, a thin anodic oxide will grown on the silicon surface in KOH: H2O electrolyte [2]. The KOH electrochemical reaction for forming anodic oxide layer can be described by listed equation:


| |


- Si - Si - + OH- + h+ → - Si – O – Si - + ½ H2 (1)


A leaky poly gate, which is electrically conductive to substrate, will be preserved and covered with thin oxide layer. Non-defective gates insulate from the substrate will be removed by KOH electrolyte. For


0.35um and 0.25μm logic and SRAM devices using traditional LOCOS process, KOH ECW method can successfully identified the leaky poly if the defective location can be parallel lapped to remove the poly silicide.


Figure 2 A leaky p-channel gate in 0.35um SRAM using traditional LOCOS process was identified by KOH ECW analysis.


However, after LOCOS field oxide was replaced by STI process, poly on trench oxide and active gates are all located at the same plane. It eliminates the poly on top of trench oxide as a good reference for checking the remaining dielectric thickness while performing parallel lapping [4, 5]. As Figure 3 shows, the electron charge at local interconnect also raised the difficulty for finding the defective gate as well. Since the analyst may not be able to lap the sample evenly with consistency, the chance to reveal the defective gate will be diminished substantially when the suspected location cannot be clearly defined.


Figure 3 The electron charge on top of local interconnects made it difficult for analyst to identify the defective gate.


KOH ECW method will be the alternative for localizing the gate related defect if silicide and nitride liner can be efficiently removed. Wet etch method is considered as the better solution for removing silicide and nitride liner because during dry etch, the plasma build-up potential in RIE etcher is likely to damage the non-defective gates and creating leaky gate. Thus,in order to apply KOH ECW with modern deep submicron CMOS process, a new wet etch recipe for removing silicide and nitride liner needs to be developed.


Experimental Design


The HF based solution has been known for titanium and cobalt silicide removal. However, cobalt silicide etch rate is much slower than Ti silicide [6]. The chemical reaction to removal cobalt silicide in HF based solution can be expressed as:


CoSi2 + 12HF→ CoSiF6 + H2SiF6 (2)Since hydrogen ion and protonated fluorides (HF and HF2-) are the main active species in the process of the


LI Poly


silica dissolution, adding HCl could maintain a higher level of H+ within the solution [7]. If nitride liner can also be effectively removed, the leaky gate can be located by KOH ECW etch. This will completely remove poly silicide rather than the limited poly silicide within contact area (refer to


Figure 4). Optimizing the cobalt silicide and nitride linear removal etch recipe will increase KOH ECW etch analysis sensitivity for identifying leaky gate and preventing over-etch of STI / SiN spacer as well.


Run # Agitation


Degree C Concen.


Voltage


Current


Electrodes Etch Thickness


M


Amp


Inch


No


45


237


7.5


611


4.5


0.5


942


548


607


1523


7


955


8


1752


1348


Yes


367


494


902


13


705


1460


1093


16


1249


17


976


18


1835


Table 2 Experimental setting and etch result for KOH electrolyte etch optimization. (Etch thickness was measured by atomic force microscope.)


HF strength


Temp HCl/HF ratio


Result of 0.18um


Run lot


a


b


c


STI


Integrity Spacer Integrity Etch %


3.5 mins


5 mins 3.5 mins 5mins


5 mins


1M


90


1.5M


85


1,5M


3.5


2M


95


98


Table 3 Experiment Design and Results for silicide / nitride liner etch optimization. * The scales of STI and Spacer integrity are evaluated by range from 1(better) to 5 (worse).


1M = 1 molarity.


Fig 4a


Fig 4b


Figure 4a Without removing nitride liner, the limited poly contact region (.25μm by .35μm) is too small for the analyst evaluating KOH ECW etch result under SEM.


Figure 4b Nitride liner and cobalt silicide can be removed efficiently by optimizing HF + HCl solution.


The success of KOH ECW etch depends on the competition between anodic etching and passivation process [8]. In order to promote oxidation process for forming anodic oxide growth layer on leaky poly gate, high concentration of holes in bulk Si need to be thermally excited and released to the Si/KOH interface. Temperature of the electrolyte, the voltage being applied, the concentration of KOH and the distance between the sample and platinum cathode,all need to be considered.


L18 (21X 37) and L9 (34) Taguchi orthogonal array methodology was used to optimize the factors for KOH ECW and silicide / nitride removal recipe respectively [9]. The L18 orthogonal array was set up with 2 levels of agitation and 3 different etch parameters for ECW optimization as illustrated in


Table 2. Table 3 listed the L9 array experimental setup for optimizing silicide / nitride etch recipe. By reducing variability and adjusting the mean from experiment design, an optimum silicide / nitride etch recipe has been developed and KOH ECW was optimized for removing dual-doped


(N and P type) poly.


The use of an antireflection coating for backside semiconductor failure analysis is discussed. The process of selecting an appropriate coating is described. Several known coatings are also described in regards to imaging quality, material properties, and the benefits to device analysis applications.


The advent of flip chip technology and the increase in backside failure analysis applications have created the need for innovations in the methods used to prepare samples for analysis. Many backside FA techniques such as photoemission microscopy and laser based techniques have experienced a decrease in sensitivity due to the refractive index mismatch at the silicon to air interface. The use of an antireflection(AR) coating to decrease reflections and thus increase transmission has been widely used in optical sciences. The applications of AR coatings for semiconductor FA have not been widely publicized.


This paper will describe the pertinent factors behind selecting an AR coating and discuss some of the advantages and disadvantages of several materials that are commercially available.


AR coatings have been widely used to coat lenses for telescopes, eyeglasses, and the metal layers in integrated circuits. New backside semiconductor FA techniques have created a need to utilize antireflection coatings. Many of these techniques require the maximum transmission of incident light in both directions across the air-silicon interface. The incident light may consist of a laser beam transmitted from an air ambient through the silicon substrate to the active device circuitry. The intensity of the laser light that reaches the circuit must be maximized to create the desired analytical effects. On the return,modulated reflected light or photoemission is at a low level and so any loss of signal decreases the chance of detection. The maximum transmission through a silicon substrate with a beam at normal incidence


through air depends on the reflection at the silicon-air interface, as shown by Equation 1,


T −=


(1)where T equals the percentage of incident light transmitted, and R equals the percentage of light reflected. The reflection can be found from Equation 2.


+−


air


sub


(2)


The refractive index of the typical silicon substrate is nsub=3.5, and the refractive index of air is nair=1.0.


Combining Equations 1 and 2 with these refractive index values gives the maximum transmission through a silicon substrate,


%1.


)1


5.3(


T


Since the refractive index of silicon increases with doping concentration, the transmitted intensity decreases with the high doping levels typical of modern integrated circuits.


The addition of an AR coating can increase the transmitted intensity. By choosing a coating with the correct refractive index and thickness, reflections from the front and back surface of the coating will cancel out by interference, thus reducing the amount of reflection. To achieve destructive interference, the front surface and back surface reflections must be equal in amplitude and 180 degrees out of phase at the front surface. From optics, the correct refractive index for equal amplitude reflections is


coating


n *= (3)


For the refractive indices of air and silicon,Equation 3 gives,


87.1


.3


ncoating


The correct thickness of the AR coating layer can be determined from Equation 4, where d is the coating thickness and λ is the wavelength of the light at normal incidence.


d∗=4λ


(4)


This thickness assures that the interfering waves are of the correct phase for cancellation by interference.


For ncoating = 1.87 and a typical laser scanning microscope wavelength of 1064 nm, the coating thickness should be


nm


.


142


87


1064 =


Using this method results in a calculated transmission of 100%. However, because of the substrate doping,the refractive index of the substrate will not be 3.5.


After the correct substrate refractive index is determined, which can be done using ellipsometry techniques, Equations 3 and 4 can be used to find a suitable AR coating. Although 100% transmission may not be actually achievable, figures in excess of 90% are realistic even considering factors such as film imperfections and thickness variations which will reduce the actual transmission that is possible.


Figure 1 shows the calculated transmission versus index of refraction for the case of silicon with nsub = 3.5.


60.00


70.00


80.00


90.00


100.00


1.75


2.25


Figure 1 Transmission vs. coating refractive index.


Coating Materials


Several materials are good candidates as AR coatings for silicon based on their refractive index. Some of these materials include Lead Fluoride, Aluminum Oxide (Sapphire), Silicon Monoxide, and Zirconium Oxide. These materials, along with their chemical formulas, refractive indices, and calculated transmission percentages are described in Table 1.


As seen in the table, all of these coatings can provide a significant improvement over the 69.1%transmission that would result from having no coating.


Table 1 Coating Materials


Common Name Formula n %T(calc)Lead Fluoride PbF2 1.74 99.48 Alumina/Sapphire Al2O3 1.77 99.69 Silicon Monoxide SiO 1.90 99.98 Zirconium Oxide ZrO2 2.09 98.78


Coating Process


All of the coatings mentioned are currently available commercially. Several companies will apply coatings on a contract basis with a fee per coating run. Usually, several samples can be coated in a single run, depending on the size and geometry of the tool chamber. Additionally, there are companies that can manufacture systems that are suited for a failure analysis laboratory environment. For these commercial systems, silicon monoxide seems to be the most common material that is used.


In most cases, the samples are coated using a bent beam evaporation method. A magnetic field bends the beam from an electron gun so that the beam is incident on the AR material. The beam evaporates the crystalline solids, creating a cloud of material that coats the sample.


Another commonly used method for deposition of AR materials is sputtering, during which energetic ions (typically Ar+) bombard a target composed of the coating material. Collisions at the surface of the target result in the displacement of atoms of the AR material that fill the chamber and coat the sample.


For best results, the sample is often rotated about a planetary substrate holder to obtain an even coating thickness. The rate at which the material is deposited, referred to as the growth rate (G), is given by Equation 5


r


m


πρ


(5)


where r0 is the radial distance of the sample to the center of the circular rotation, ρ is the density in(g/cm3) and m is the mass evaporation rate (g/sec) of the starting material. The optical quality of coatings deposited using either of these two methods is quite suitable for typical backside FA techniques including photoemission microscopy, laser voltage probing and basic backside imaging.


The thickness of the coating can be accurately controlled so that consistent films can be produced across multiple runs. A crystal quartz oscillator is commonly used to monitor the coating thickness. As the crystal is coated, the oscillating frequency changes. A film thickness monitor converts the changing frequency into a thickness value, based on coating material parameters and the crystal location.


The accuracy of the applied film can be controlled to well within 10% repeatedly. As the crystal monitor acquires more coating, the frequency shift becomes nonlinear. Periodic replacement and recalibration of the oscillators is necessary.


During the coating process, the entire inside of the chamber is coated along with all internal parts.


These parts must be periodically cleaned to maintain the efficiency of the tool. This can be a dangerous process, especially with a coating such as Lead Fluoride, due to the lead content, which is a known health hazard. This can be a factor in choosing a coating depending on local safety regulations. As a minimum the cleaning process can add to the general overhead of operating this type of tool.


Imaging


One of the basic characteristics of an effective coating is the quality of the image that can be obtained. All of the coatings from Table 1 provided satisfactory images. Figure 2 shows a backside image of a sample with no AR coating, taken with a confocal laser scanning microscope at 20X magnification.


Figure 2 Image with no AR coating.


The substrate was thinned and polished to an optical quality finish using a 1 micron film prior to imaging.


The thinning was needed due to substrate doping levels and is not necessarily needed for all devices.


The interference fringes in the image result from a slight tilt of the sample surface with respect to the incident beam. The tilt results from an uneven polish or uneven mounting of the sample in device fixture of the microscope. These fringes can be seen even on a coated sample, if the sample coating parameters are not correct.


Figure 3 shows the dramatic increase in image quality after application of an AR coating. The fringing from the previous image is gone and even the effect of the scratch in the lower right corner is minimized.


Figure 3 Image with AR coating applied.


Figures 4 - 7 show images taken with a laser scanning microscope at 20X. The lead fluoride and the silicon monoxide samples were thinned to approximately 100 microns and were coated in house. The other two samples were thinned to approximately 50 microns and were coated by a commercial vendor. As seen from the images, all four coating materials result in quality images, although some fringing can be seen. From the images, it appears that the lead fluoride coating provided the best image quality.


Figure 4 Lead Fluoride coating.


Figure 5 Aluminum Oxide coating.


Figure 6 Silicon Monoxide coating.


Figure 7 Zirconium Oxide coating.


Material Properties


For device analysis applications, imaging is often the most important factor when considering different AR coating materials. Often overlooked are some of the material properties of the coatings themselves. For instance, lead fluoride is very commonly used as an AR coating, despite its toxic nature. Also, lead fluoride coatings are very soft and easy to scratch.


Excessive handling may affect the use of backside FA tools. Thus, it is important to take these types of properties into consideration when selecting an AR coating.


Studies were performed to assess the durability of different antireflective coatings. Micro Scratch Testing was performed on four samples to determine the adhesion properties of the coatings. Each sample was coated with a different type of AR material, with the results summarized in Table 3. The left column indicates the AR material used to coat the respective samples. The middle column shows the average critical force (in mN) to start coating damage. The right column shows the average force to completely penetrate the coating. Please note that four measurements were performed on each sample. The coating thicknesses were determined by Equation 4 and were not optimized for mechanical properties.


The data demonstrates that lead fluoride is the least adhesive coating of the four tested.


Table 3 Adhesion Test Results


AR Material


1st Defect (mN)Average


Complete Delamination(mN) Average PbF2 11 (Std dev 1) 369 (Std dev 120)SiO 16 (Std dev 5) 1087 (Std dev 118)Al2O3 14 (Std dev 5) 1305 (Std dev 41)ZrO2 25 (Std dev 14) 1303 (Std dev 69)Additional testing using a nano hardness tester(NHT) determined the relative hardness of each type of coating. The NHT places a weighted tip on the film surface and measures the maximum load that can be applied without deforming the film. The hardness is calculated from the pressure per area and is measured in Vickers. The hardness values are tabulated in Table 4.


Table 4 Hardness Test Results


Coating Material


Hardness (Vickers)


PbF2


244


SiO


425


Al2O3


629


ZrO2


372


Photoemission Microscopy


Photoemission microscopy is one of the most common FA techniques. The benefits of an AR coating are quite obvious when comparing the intensity of emissions before and after the deposition of an AR coating. Table 2 shows emission intensity data from two diode structures both before and after the application of a lead fluoride coating. In this case, the coating was optimized as before. However,photoemission results in a range of wavelengths.


Even so, with the coating optimized at 1064nm, there is less than 5% reflection in the range from 0.9 to 1.3 microns. Since most common defects emit strongly within this range, there is still a considerable gain in sensitivity after the application of an AR coating.


Assuming the initial intensity readings as 69.1% of the theoretical maximum, the increase in intensity results in a transmission percentage of around 90%.


Table 2 Photoemission Data


Sample Bias


Counts/sec


Increase


No ARC ARC


Diode 1 Forward 282 369 31%Diode 2 Forward 480 644 34%Diode 1 Reverse 22 28 27%


Diodes 1 and 2 were both N+ diodes on a P substrate.


The diodes were identical, although diode 1 was four times larger by area than diode 2. Both diodes were on a sample with the substrate thinned to 200 microns. Emissions were taken with a 30-second acquisition time using a laser scanning microscope with a cooled silicon CCD detector.


The gain in intensity results in two benefits. One benefit is the ability to detect lower level signals.


This fact is especially important as supply voltages and device currents are scaled down. The other benefit is shorter exposure times; so more data can be obtained in less time. This allows the failure analysis engineer to simulate many different device situations in less time and get a better picture of the device characteristics.


Laser Based Applications


Since AR coatings increase the transmission through the substrate, they are also well suited for use in many of the modern FA techniques using lasers as the incident light source. Techniques such as LIVA,TIVA, and laser voltage probing all benefit from the use of an AR coating.


As discussed earlier, many tests can be done to see how efficient an AR coating performs. Light transmission and reflectance tests using a spectrometer are the most basic experiments that can be done to test how well a coating performs.


However, the best way to gauge how well an AR coating performs is to see how well it works with typical laser based applications.


Studies were performed using a Laser Voltage Probe(LVP) tool on samples with different AR coating materials. The samples were working flip-chip microprocessor units, and were driven with the appropriate signals and power. For each device, an internal clock signal was acquired from the same coordinates on each device using the same LVP system. The LVP measures the photons absorbed within a junction area. The AR coatings served to maximize the amount of laser light being transmitted through the silicon, and thus maximize the absorption in the junction area. The results of the study are condensed into Table 5, with the left column showing the type of AR coating material used to coat each sample. The right column shows the average amount of absorption in ppm (parts-per-million). The higher the ppm level, the better the tool is able to determine signal quantities such as rise and fall times.


Table 5 LVP Data


AR Material Average PPM Level


PbF2 3000ppm


SiO 2800ppm


Al2O3 2800ppm


ZrO2 1500ppm


As the data shows, PbF2 on average does perform better than the other three coatings for LVP signal acquisition. However, it does not perform substantially better than SiO and Al2O3.


Due to the increase in the need for backside failure analysis applications, the absorption of light in the substrate has caused a need for antireflection coatings to improve the efficiency of many FA techniques,both old and new. The selection of an appropriate AR coating is not difficult, but there are many factors to consider including selecting a coating with the correct refractive index, considering material properties such as adhesion and hardness, and determining whether or not to purchase a tool or have parts coated by an vendor.


The authors would like to thank the following people for their help during the development of the data in this paper: Rama Goruganthu, Mike Bruce, and Danny Stone from AMD, Alan Berginc of Cressington Scientific Instruments, Pierre Leroux of Micro Photonics Inc., Bill Atwood of UVIRA, and Alex Jacobson of CVI Laser Optics.


1. Jurgen R. Meyer-Arendt, Introduction to Classical and Modern Optics, Prentice Hall, New Jersey (1995)


2. http://www.luxpop.com/ (Web based calculation tool.)


3. Michael Bass, editor, Handbook of Optics,McGraw-Hill, Inc, New York (1995)


4. Richard C. Jaeger, Introduction to Microelectronic Fabrication, Volume V,Addison-Wesley Publishing Co. (1993)


p 161-171


DOI: 10.1361/cp2000istfa161


Comparative Study of Sample Preparation Techniques for Backside Analysis


Philippe Perdu, Romain Desplats, Felix Beaudoin


Toulouse, France


This paper presents a comparative study of backside sample preparation techniques with applicability to conventional as well as flip chip package types. We will cover mechanical (grinding and milling tools),chemical (wet and dry chemistries) and other approaches such as laser ablation. Backside sample preparation is very challenging.


The preparation process flow starts with decapsulation of the ceramic or plastic package,continues with the die paddle removal, silicon thinning and finishes with silicon polishing.


The techniques involved include mechanical,chemical and other novel approaches for ceramic and plastic package. Today, only CNC milling can cover the whole process for almost any kind of packages.


Nevertheless, photo ablation is a rising technology for package decapsulation. In addition, chemical wet etch can be used to perform silicon thinning and polishing.


We will illustrate the complexity of the process through examples. The first one is a ceramic package where the main issue is the hardness of ceramic. The second one is a TSOP package where the main challenge is the chip scaled package. Both will be observed through the IR emission microscope to demonstrate the efficiency of the preparation.


The analysis of integrated circuits often requires access to the chip without disturbing the device functionality. To do this, several sample preparation techniques have been successfully developed to expose the front side of the device. However, new technological trends [1] in packaging such as flipchip, lead-on-chip, the constant increase in the number of metallic layers in integrated circuits and the generalization of top metal layer filling require access through the substrate to the heart of the circuit.


Failure analysts in the space-related field, encounter many different plastic or ceramic packages, usually one-of-a-kind failing samples.. To ensure accurate results, we investigated backside sample preparation issues. After a short review of the backside sample preparation challenges, we will describe every step of the preparation process flow: decapsulation, silicon thinning and polishing. For each technique we will focus on its capabilities and we will explain the improvements we have done. Conventional wirebonded packages are being discussed as well as flip chip packages


Our goal is to share our experience on different tools in order to help other users in their sample preparation and in the development of new techniques.


Backside Sample


Preparation Challenges


If we consider the systems available for backside analysis, there are only a few such as SQUID(Superconducting QUantum Interference Device) [2]that directly allow short circuits localization inside the die without package removal. The backside analysis techniques are mainly based on optical tools


[3] such as LIVA (Light Induced Alteration Voltage)


[4], OBIRCH (Optical Beam Induced Resistance Change) [5], SEI (Seebeck Effect Imaging) [6], TIVA(Thermally Induced Voltage Alteration) [6] and laser voltage probing [8]. All these techniques need a complex sample preparation process.


The first challenge is to decapsulate the package to access the backside of the die without jeopardizing the electrical properties of the device. Then the silicon has to be thinned down to 80-300 µm and polished. The thickness of the remaining silicon has to be determined according to the wavelength used by the optical beam based testing system and the substrate doping. We can use Johnston’s results [9]about absorption coefficient in silicon (see Figure 1)


to calculate the allowed maximum thickness according to the observation conditions.


Figure 1 Absorption coefficient in silicon [9].


After silicon thinning, the silicon surface roughness can cause light distortion, which can cause optical losses that can jeopardize the backside analysis. To avoid the distortions, we have to polish the backside surface to obtain a near optical finish.


Furthermore, the device has to be mounted in a way such that it can be inserted under short working distance (W. D.) high magnification optical lenses used for backside optical beam imaging and optical beam testing of the ICs. For instance, Table 1 shows working distances for various 100 X magnification objective. Obviously, the short distance between the sample and the optics imposes geometrical limits on the remaining part of the package, pins, socket or IC support and DUT board. Moreover, in some cases, it is impossible to access the backside without deprocessing the package (see Figure 2) the die must be ported to an engineering package.


Manufacturer


System


W. D.


Zeiss


Optical microscopy 1 mm


LSM


3 mm Mitutoyo (ULWD) Optical microscopy 20 mm Mitutoyo (NIR) Emission microscopy 12 mm Table 1 Working distances for 100 X magnification objective


Figure 2 Example of BGA package that cannot be


prepared with our process flow.


We will present only backside sample preparation techniques that follow process flow composed of decapsulation, die paddle removal, die attach removal, silicon thinning and silicon polishing.


Decapsulation


Chemical and mechanical decapsulation techniques based on wet etch, micro sand blaster and other techniques were reviewed by Lee [10]. In our lab, we have access to chemical etching (wet and dry),grinding and polishing wheels (diamond and carbide),milling tools and a laser micro-machining system for backside sample preparation. For ceramic cavity packages, the first step in backside sample preparation is front side decapsulation and cavity filling. The filling material is usually an epoxy that can be removed with panasolve (or dynasolve). We also used a wax that can be removed more easily by heating.


Chemical Decapsulation


We have a Nextral 80 plasma RIE dry etcher. It can remove any kind of material with a good selectivity by an accurate choice of Radio Frequency, gases and pressure. A screening shield can mask areas that we do not want to etch. We encounter three problems with this method: redeposition of species, etcher contamination and time-consuming etches for ceramic packages. For these reasons we do not use RIE for package decapsulation.


Wet Etch


In our lab, we process plastic package by jet etch(NSC PA103) with nitric acid. For those packages that require hot sulfuric acid, we use the dropper method.


Wet etch does have its disadvantages. Wet etch does not work with ceramic packages. With plastic packages, the acid can damage the lead frame and the bonding. It could be very difficult to keep the functionality of IC with CSP (Chip Scale Package).


More generally, wet etch works well if the size of the die is quite small compared to the package size. Wet etch gives us an isotropic etch and a high etch rate.


Figure 3 Over wet etch and under wet etch in a


plastic package caused by etching


window misalignment.


During the wet etch process, a shield window usually defines the area of the package to open. This window is manually positioned and we encounter some slight misalignment that can induce over etch in some parts and under etch in other parts (see Figure 3). The hazardous nature of the acid and the changes in package material and bond wires make wet etch a process of continuous experimentation.


Mechanical Decapsulation


Mechanical decapsulation can be applied to every kind of package material. It usually works in a Z plane. The device has to be perfectly horizontal.


Figure 4 Plastic DIL package processed with a grinding wheel after 180° vertical pin rotation.


Grinding Wheel


The grinding wheel works only with devices that have the lead frame higher than the backside of the die. If not, the wheel will damage the lead frame during package removal or silicon thinning. The grinding wheel works well for flip chip devices. It removes a constant thickness on the whole package backside surface. This process is a well-known technique with no specific issues. For DIP plastic packages, we can bend the pin to expose the backside of the die (see Figure 4). Before the grinding operation the device is put on a socket to avoid lead frame lift off.


Milling


We use Chip Unzip (see Figure 5) from Hypervision for the whole process of backside sample preparation.


Figure 5 Chip Unzip system.


The Chip Unzip is a three-axes milling tool. This CNC (Computer Numerical Control) with diamond or carbide milling drill is software driven and the process is simulated with SmartCAM Production Milling, from SDRC. The main advantage of this kind of system for package decapsulation is the ability to remove material in a controlled area, right above or below the die. In addition the drilling tools are very


long (5 cm) and thin (diameter from 0.793 mm to 6.4 mm). Therefore the tool allows processing of the center of packages with surrounding vertical pins. It can process ceramic packages with a high speed air spindle and diamond drill or plastic packages with a low speed spindle and metal endmill drill (see Figure 6). We maintain the chip functionality even for chip scaled packages, because we can open a window that preserves the lead frame. The device is held by wax inside an aluminum fixture. After the whole process of decapsulation, die paddle removal, silicon thinning and polishing, this wax is heated to recover the sample.


Figure 6 Chip Unzip spindle, high speed (left), low speed (right).


Other Lapping Tools


There are many other lapping tools such as the Beaps from South Bay Technology. The Beaps can decapsulate either plastic packages or ceramic packages. It can also perform the whole process of backside sample preparation. The Beaps’s only limitation is the 5 cm diameter of the tool. It cannot process parts of packages surrounded by vertical pins like PGA’s. (see Figure 7)


Figure 7 Device that cannot be processed by some tools because the vertical pins limit machine access.


Laser Decapsulation


Femtosecond ablation has several advantages compared with the other mechanical and chemical approaches used for backside sample preparation: it is contact-less and non-thermal, the ablated volume is constant and all types of materials present in IC packaging can be ablated.


The trials were done on an Alpha-1000 laser(Thomson CSF 800 nm laser) producing 100 fs pulses with energy of 0.8 mJ at a 1 kHz repetition rate [11].


The etch is anisotropic and follows the light path.


The process removes a constant thickness at each laser pulse.


Figure 8 above shows a backside opening of a 64 Meg DRAM device in a TSOP package. It took only 32 minutes to open a 9 mm by 19 mm surface in the 230 µm thick plastic package. The tool also processes ceramic packages, although the etching rate drops from 20 106 µm3/s (plastic packages) to 1.4 106 µm3(ceramic packages). Like Chip Unzip, we can process the center of packages with surrounding vertical pins.


However, this technique is still in development and it is not reliable yet.


Figure 8 Package opening by photo ablation (left)


and the same after polishing (right) .


Figure 9 Constant Z removal initial position (top)and final position (middle) compare with the improved Z(x,y) milling process (bottom) .


We have only two processes, milling and laser ablation, which are able to remove material on any kind of packages (ceramic and plastic). Only milling tools are commercially available. Our milling system basically removes material in a xy plane. At each step, the milling drills remove all the material (plastic or ceramic) from a position Z0 to a position Z1 in the removal window (see Figure 9).


This process is called the constant Z removal process.


Unfortunately, this process needs to have a pe1111rfectly horizontal device. If not, milling tools can either over etch a side of the package or induce device damages on ceramic packages (see Figure 10).


To avoid this issue we have developed software macros for Chip Unzip. This macro allows a variable Z(x,y) milling. The milling drill moves now in a plane parallel to the surface of the package even if this package is tilted. The first step is the precise measurement of the Z reference and the tilt, which are


the two basic parameters for this new macro. To do this, we use a 3D sensor (see Figure 11). To get the exact difference between this sensor and the spindle we use a tool-adjustment metrology system (see Figure 12).


Figure 10 Tilted ceramic package broken during milling.


Figure 11 3D sensor for accurate Z measurements.


The program was also modified to allow the gradual increase and decrease in the removal depth per step to limit package stress (5 µm, 20 µm,, 20 µm, 50 µm,… ,50 µm, 20 µm, 20 µm, 5 µm). With these extensions,Chip Unzip gives us accurate results for all kind of packages.


Figure 12 Tool adjustment metrology system.


Die Paddle and Die Attach Removal


When stuck on the die backside, the die paddle and the die attach has to be removed. This operation can be done either with a razor blade (see Figure 13) or milling tool. We often observe die paddle lift off during decapsulation.


Figure 13 Die paddle and die attach removed by razor blade.


Silicon Thinning


Chemical Thinning Dry Etch


Because of the large amount of material to remove,we run into the same limitations as decapsulation.


Therefore, we do not use this tool for silicon thinning.


Nevertheless, some trials were done with SF6 (25


cc/mn), O2 (10 cc/mn), 50W RF. We obtained a 2.5µm/min etch rate. The surface roughness could be observed with the naked eye and we observed unwanted side effects such as overetching of the cavity edges.


Silicon wet etch was reviewed by T.W. Lee [12]. At the present time, we have used two kind of chemical etchers: Pyrocatechol based and HF-HD NO3 mixture. Both have the great advantage of high etch rates. Because wet etch is difficult in deep cavities,we experimented with a thick package containing a small die. The cavity opening was 8mm by 8 mm by 2 mm depth. The die size was 5 mm by 5 mm and the 400 µm silicon thick substrate was N doped(1015 at/cm3).


We used a mixture of 4.5 g of Pyrocatechol(C6H6O2), 25 cm3 EDA (Ethylenediamine),and 25 cm3 deionised water. The process took 10 mn to remove 100 µm of silicon at 80°C. The main advantage of this mixture is its high selectivity for silicon. Without any other polishing process, we tried then to observe the die with an IR emission microscope (Phemos 1000 from Hamamatsu) The surface seemed quite smooth but under a 5 X magnification with visible light, we observed an uneven etched surface (see Figure 14 left). Using near infrared light with the same magnification we can guess metal lines (see Figure 14 middle). A difference image obtained by subtracting the visible light image from the infrared image is shown in Figure 14 right.


We can clearly see that the metal lines are enhanced.


Figure 14 Pyrocatechol, 5 X magnification, visible(left), IR (middle) and difference (right).


This device emits light when direct biased at 2 mA.


The obtained emission image is shown in Figure 15 left. The localization of the emission spot was done by superposition of this emission image with the I.R.


reflected image (see Figure 15 middle). Once again we can improve the image using the difference image instead of the reflected one (see Figure 15 right). At higher magnification (20 X) we can get a better


picture of metal lines with slight distortions caused by the border of small etched areas (see Figure 16).


Figure 15 Pyrocatechol, 5 X magnification, light emission (left), superimposition with reflected image


(middle) and previous difference (right).


We also experimented with a HF-HNO3 mixture.


The nitric acid in this mixture oxides the silicon, and the hydrofluoric acid dissolves the resulting silicon dioxide. With more nitric acid than HF, the etch rate is controlled by the oxidation. With more HF than nitric, the etch rate is controlled by the silicon dioxide removal. Water and/ or acetic acid will extend the range of oxidation power of HNO3. We used different solutions for isotropic silicon etching according to etch rate, isotropic effect and chemical polishing properties (see Table 2). The pins and exposed parts of lead frame are protected by wax.


Figure 16 Pyrocatechol, 20 X magnification, visible(left), IR (right).


Using the dropper method, with solution 1 from Table 2 created a convex silicon surface (see Figure 17 left).


With the immersion method, the silicon looked more uniform but we observed a poor surface state under the microscope (see Figure 17 right). The same method was applied with solution 2. The etch rate decreases strongly but the results seem better.


However, in both cases, we could not get an accurate image of these devices at low (5 X), medium (20 X)and high (100 X) magnification inside our IR emission microscope.


Nevertheless, we are still trying wet chemical etching of silicon because it can potentially be used to obtain accurate chemical polishing [13].


So. Composition Tried Etch rateµm / mn 1 HF (60%)


HNO3 (30%)


Yes 470


2 HF (5%)


HNO3 (90%)


CH3COOH (5%)


Yes 5


3 C6H6O2 (33 %)


EDA (33%)


H2O (33%)


4 Hydrazine (40%)


H2O (60%)


No 0.6


5 KOH + propanol +H2O


No 1


6 Choline


Hydroxyde


Not yet 1


Table 2 Solutions for silicon thinning


Figure 17 State surface with solution 1, dropper method at low magnification, immersion method a


medium magnification (right).


Mechanical Thinning


We can use the same tools as for package removal with the same limitations (grinding wheels and other lapping tools).


We use a Struers grinding wheel with SiC paper (800 to 1200 grit) for devices that can be processed that way.


For any kind of device, we use a high-speed air spindle of Chip Unzip with a diamond drill (400 grit).


We correct the total tilt (die attach, package,fixturing) using our software tilt correction. In fact we find that on big die (more than 1 cm2), there can be a total tilt that induces a Z difference of more than 100µm between two corners. In addition, the process is cooled to allow low stress milling.


Laser Thinning


It should be possible to use photo ablation for silicon thinning according to first trials but this technique is still in development.


Other Thinning Tools


Focused Ion Beam (FIB) can etch silicon. Revise proposes also a Laser MicroChemical (LMC) tool for silicon etching but in both cases, these techniques are dedicated to local device microsurgery. They are not adapted to remove a large amount of material.


The main issues of silicon thinning are thickness uniformity, low stress process and surface roughness compatible with polishing process. At the present time, only Chip Unzip and wet etch can work inside boxes opened in packages. Good silicon thinning is also linked to decapsulation for ceramic packages.


For these packages, epoxy filling is a key issues. In some cases, we encountered die cracking, broken bonding wire and even die lift off. All these issues are related to the epoxy hardness and adherence. The filling process is also involved. We chose citofixdurofix epoxy from Struers and a polymerization process under a pressure of two atmospheres to avoid these problems.


Silicon Polishing


Mechanical Polishing


We can use both the Dremel, polishing wheel (1 µm or below) or other lapping tools with diamond paste or colloidal silicon. Dremel is a well-known small drill brand that can be used with a cotton bob, 1 µm polycrystalline diamond compound, with ethanol to get a lower viscosity. In all cases, the results are quite good.


Chemical Polishing


Chemical silicon polishing can be carried out with the same solution as silicon thinning. HF (5%)+HNO3(90%)+CH3COOH (5%) solution gave us the best result but not good enough.


CMP


CMP (Chemical Mechanical Polishing) is widely used for wafer polishing. CMP employs both a chemical and a mechanical component. The chemical


solution (colloidal silica in NaOH, KOH, deionized water and citric acid) reacts with the surface silicon to create a hydrated silicate layer. The mechanical component, and endmill at high speed, drains the silica particles that ablate this layer. Then the process can carry on the next silicon layer. At the end of the process, the sample is water rinsed. To achieve the process, we use replication material (cellulose acetate sheet from Agar) with acetone to remove small remaining particles. Then we dry the sample with dry nitrogen.


All


packages


Silicon Polishing Dry etch No Possible No Wet etch No Yes Yes Grinding Wheel No Possible Possible CNC Milling Yes Yes Yes Other lapping


tools


No Possible Possible Photo ablation Yes Possible No Table 3 Comparison of preparation techniques


As mentioned in Table 3, only CNC milling is able to follow the process flow of backside sample preparation for all kinds of packages. Other mechanical tools can be efficient with some limitations regarding the packaging.


For package decapsulation, photo ablation seems to be an interesting technique and it could be completed by wet etch silicon thinning and polishing.


Sample Preparation Examples


Ceramic Package DIL 24


We chose a DIL 24 ceramic-package device with a small die. The first step is to decapsulate the side brazed package with a razor blade. Then we fill the cavity with epoxy. After polymerization in a controlled atmosphere to avoid epoxy expansion and bubbles, the epoxy is polished with a polishing wheel.


After that, we open a 1cm by 1cm box in the package backside with Chip Unzip (high-speed air spindle and 80 grit diamond drill). We thin the silicon to a thickness of 200 µm in a 5 mm by 5 mm box with Chip Unzip (high speed air spindle and 400 grit diamond milling drill). The epoxy must be very hard to withstand the high pressure on the die during silicon thinning. If the epoxy is somewhat weak or


elastic it can mechanically deform and break the bonding. Due to the small surface area of the die, we polish it by hand with a Dremel. At the end of the process, the sample is water rinsed. To finish the process, we used a replication material with acetone to remove small remaining particles. Then we dry the sample with dry nitrogen.


Figure 18 Front side view of the die and the epoxy


filled cavity (ceramic package).


The epoxy is transparent and we observed the front side of the die through it (see Figure 18). The bonding wires were enclosed in the epoxy and the silicon was only held by epoxy (see Figure 19). With this kind of package we cannot bend the pins. To follow working distance limitations, we cut the pins and put the device inside a DIL test support which allows us to test the device (see Figure 20). The device functionality was kept afterthe full backside preparation process.


Figure 19 Backside view of the prepared sample(ceramic package).


Figure 20 Sample preparation of .ceramic DIL package.


Figure 21 Backside view through silicon at 100 X


magnification (ceramic package).


The efficiency of the sample preparation was checked under an IR emission microscope at 100 X magnification (see Figure 21).


TSOP Package:


We chose a plastic TSOP package that is very representative of sample backside preparation. The die (9mm by 17 mm) is almost as large as the package!


After fixturing, the package is widely opened with Chip Unzip (low speed spindle and metal drill). There is only 0.5mm of the remaining package near the pins. We thin the silicon to 200 µm with Chip Unzip(high-speed air spindle and 400 grit diamond drill).


The final polishing is done on Chip Unzip with CMP.


The prepared device is then placed in a socket to ensure electrical contact (see Figure 22). After one day, the functionality of the device was lost due to some discontinuities between the socket and the device. In fact there is a combination of constraint relaxation and humidity that induced device bending(see Figure 23).


Figure 22 TSOP package inside a test support.


Figure 23 Bent TSOP package after 24 h.


Figure 24 Sample preparation of TSOP package.


To avoid this effect, we processed a new device after soldering it onto a PCB adapter. This also makes it easier to test because of the DIL adaptation (see Figure 24). The efficiency of the sample preparation


was checked under IR emission microscope at 100 X magnification (see Figure 25).


Figure 25 Backside view through silicon at 100 X


magnification (plastic package).


We tried five sample preparation techniques: two mechanical (polishing wheel and milling), two wet chemical (etch by pyrocatecol and HF-HNO3 mixture) and one laser (photo ablation).


We also slightly reviewed other techniques like dry chemical etching (plasma RIE), FIB and Laser assisted dry chemical etching. Only Chip Unzip can satisfy all our needs for backside sample preparation.


Currently, we have solved the planarity problem with software development and added instrumentation. We are still working to improve its processes. We have to take care also of extrinsic issues like optical working distance (observation of the prepared sample) and deformation of thin packages. For CSP and more generally CMS, it is important to solder the reverse side device on a PCB to reinforce it.


We showed the efficiency of the Chip Unzip system with two challenging samples. These samples were observed under IR emission microscope to check the preparation quality.


Finally, according to our preliminary experiments, we believe that photo ablation is a very promising technique for backside preparation when coupled with chemical wet etching for silicon thinning and polishing.


Thanks to Michael Ribiere (Chip Unzip optimization), Frederic Courtade (Plasma RIE),Gerald Guibaud (Chemical silicon etching), Alain Wislez (Mechanical polishing), Frederic Saviot(Photo ablation) and Guy Perez for his helpful advice.


1. International Technology Roadmap for Semiconductor (1999).


2. L. A. Knauss, B. M. Frazier, H. M. Christen, S.


D. Silliman, K. S. Harshavardhan, E. Fleet, F. C.


Wellstood, M. Mahanpour and A.


Ghaemmaghami, “Detecting Power Shorts From Front and Backside of IC Packages Using Scanning SQUID”, 25nd ISTFA, , 11-18 (1999)


3. K. Bernhard-Höfer, E. Cole and D. Barton.,“Flip-chip and “backside” techniques”,Microelectronic Failure Analysis, Desk Reference, 4th edition, 487-503 (1999)


4. E. Cole, “Novel Failure Analysis Techniques Using Photon Probing With a Scanning Optical Microscope», IRPS , 388-398 1994.


5. K. Nikawa and S. Inoue, “New capabilities of OBIRCH Method for Fault localization and Defect Detection”, 6th Asian Test Symposium,219-229 (1997).


6. E. Cole, “Backside Localization of Open and Shorted IC Interconnections”, IRPS, 129-136(1998)


7. J. A. Kash, J. C. Tsang, D. R. Knebel.and D. P.


Valett, “Non-Invasive Backside Failure Analysis of Integrated Circuits by Time-Dependent Light Emission: Picosecond Imaging Circuit Analysis”,Microelectronic Failure Analysis, Desk Reference, 4th edition, 505-510 (1999)


8. T. Eiles, G. Woods and V. Rao, “Optical Probing of VLSI Ics From the Silicon Backside”, 25th ISTFA, 27-34 (1999).


9. A.H .Johnston, “Charge collection in p-n junctions excited with pulsed infrared lasers”,IEEE transaction on Nuclear Sciences, 40, 6,1694-1702 (1993).


10. T. W. Lee, “Mechanical and chemical decapsulation”, Microelectronic Failure Analysis, Desk reference, Third Edition, 61-71(1997).


11. F. Beaudoin, P. Perdu, F. Saviot, D. Lewis.and F.


Salin, “New Laser Ablation Method for NonDestructive Backside Sample Preparation”, 26th ISTFA (2000).


12. T. W. Lee, “A Review of Wet Etch Formulas for Silicon Semiconductor Failure Analysis”, 22nd ISTFA, 319-330 (1997).


13. Y. Chew, K. H. Siek, W. M. Yee, “Novel Backside Sample Preparation for Advanced CMOS Integrated Circuits Failure Analysis”, 7th IPFA, 119-122 (1999)


p 173-176


DOI: 10.1361/cp2000istfa173


A Comparison of Backside Emission Microscopy Systems


Advanced Micro Devices, Austin, Texas, USA


The need for failure analysis from the backside of the die has introduced new challenges in device analysis applications. Standard silicon based detectors are no longer as efficient due to the absorption of emission signals by the silicon substrate, which is now in the optical path between the device and the detector. The emergence of infrared detectors has offered a solution since emissions in this regime are not attenuated.


This paper will describe a comparison made between a silicon detector and two of the most common IR detector materials.


Photoemission microscopy is often one of the first lines of defense for a failure analysis laboratory.


Many types of common defects can be located using this technique. The characteristics of photoemission from each defect class have been well documented.[1,2] Early studies showed that the emission spectrum from many defect classes began to tail off at wavelengths near one micron when in fact this was due to the upper limit of detection for silicon based systems.[3,4] This upper limit corresponds roughly to the bandgap of silicon at approximately


1.1 micron with many systems not able to detect emissions higher than 0.9 micron. This was bad news since many devices now utilize flip chip technology.


The presence of the silicon substrate in the optical path serves to greatly attenuate signals with wavelengths less than 1.1 micron. These signals have enough energy to create electron hole pairs and become absorbed in the substrate. The absorption problem is even further aggravated as substrate doping levels increase. These factors limit the effectiveness of silicon based detectors since the majority of emissions (> 1.1 •m) that can be transmitted through the silicon without significant attenuation fall outside the detection limits of the detector.


More recent data shows that these typical defect emissions extend past the silicon bandgap and into the near infrared (NIR) regime. [5] Due to this fact,


an infrared detector is well suited for backside photoemission microscopy. Many IR detectors have spectral response ranges that take advantage of these emissions, which can have strong responses in the area of 1.2 to 1.5 microns. This gives IR detectors an advantage over standard silicon detectors, which can only detect emissions that have been greatly attenuated by the substrate.


Systems


An evaluation was conducted to compare the performance of several photoemission systems. The three systems that were used were the ZEISS Laser Scanning Microscope (LSM), the Infrared Laboratories Infrared Emission Microscope (IREM),and a prototype system, which used a Sensors Unlimited camera. The key parameters from each detector are summarized in Table 1.


Table 1 Detectors


System LSM IREM SUI


Detector Si MCT InGaAs Range (μm) <1.1 1 - 2.5 0.9 – 1.7 Array Size 512X512 256X256 320X240 Pixel size (μm) 24 40 40 LSM: The Zeiss LSM uses a Photometrics CH250 camera with a silicon detector that is cooled using an enclosed ethylene glycol coolant system. The detector is a 512X512 array with 24 μm pixels. The system utilizes a standard Axiotron microscope base that includes a motorized xyz stage. All controls are accessed through a GUI system. The system is no longer being manufactured or supported by Zeiss. It was selected as a typical silicon based detector system to provide a common baseline for comparison with the newer IR detectors. The photoemission intensity data was taken using the LSM measurement software.


IREM: The IREM uses a Mercury Cadmium Telluride (MCT) detector cooled with liquid nitrogen.


The coolant must be replenished every 12 hours. If the detector reaches room temperature, the camera


Dewar must be evacuated for 12 hours to remove contamination. The detector itself is a 256X256 array with 40 μm pixels. The system components include a high precision 3-axis stage with CAD overlay. All controls are located in a GUI system.


Intensity data was taken using the IREM data analysis software. The IREM was the first commercially available photoemission system developed specifically for backside analysis. The extended detection range of the detector also allows for some thermal analysis capabilities.


Prototype system: The prototype system consisted of an Indium Gallium Arsenide (InGaAs) cooled camera by Sensors Unlimited Inc. (SUI). The detector is a 320X240 array with 40 •m pixels and requires no external cooling. The camera was mounted on a microscope head with IR optimized objectives, which was in turn mounted on a standard microprobe station in a dark box. Intensity data was taken using a Hamamatsu Argus-20 image processor. This processor only uses the lower 8 bits of the 12 bit output by the camera. This resulted in saturation of the intensity values for high intensity emissions, but was not a factor for lower intensity emissions resulting from lower bias voltages. The camera had only one acquisition time of 16 milliseconds. For the purposes of this comparison, adding successive frames together simulated longer times. Future revisions of the camera will have the capability to select multiple acquisition times. Illuminated images were taken using a 12-bit image acquisition board.


Samples


The samples used for the evaluation results presented here were integrated N+ diode structures from a C4 backside testchip. The sample was thinned and polished to 100 microns of remaining silicon. No AR coating was applied for this study. (The addition of an AR coating can increase transmission intensities on the order of 20 to 30 percent. [6]) Data was taken for both forward and reverse bias cases. This particular diode was chosen since it provided a large area of photoemission that was easily compared to the background with no other active devices. This enabled an easy way to determine signal to noise parameters. An illuminated image taken with the LSM of the diode is shown in Figure 1.


Figure 1 Diode structure used for evaluation.


Emission Intensity


The sample was biased using a constant current source and emission images were collected using each instrument. All data was taken using a 20X objective for each system. This allowed the structure to fill approximately half of the screen, with the other half used to determine noise parameters. In all cases the emission intensity figures were determined by taking the average pixel value over the center of the emission area as the signal quantity. The noise values were likewise determined by taking the intensity outside of the emission area. The sample had only one structure powered during the experiment, so there were no stray emissions from devices other than the one of interest. Table 2 shows the minimum current detected under forward bias for each system. These numbers were determined as the lowest current detected that resulted in a signal to noise ratio of 2:1 or greater. Since the acquisition times varied widely for the minimum current levels,the minimum current detectable in 1 second was also measured to obtain a more direct comparison of detector capabilities. This data is also shown in Table 2.


Table 2 Minimum Current Level Detected


System Min. Current Time


Min. Current(1 second)LSM 100μA 60s 500μA IREM 750nA 50s 10μA SUI 10μA 1s 10μA This data illustrates the performance increase of an IR detector over a standard silicon detector when used for backside photoemission. While the silicon was able to detect similar current levels, it did so with a much longer time required to capture the signal.


For reference, a 750nA figure relates to a power level of approximately 0.4μW while a 100μA current relates to approximately 60μW power.


Figure 2 shows the forward bias emission data at low current levels for each tool. The data was taken using a one-second acquisition time and normalized to the intensity at the 1mA forward bias current for each tool. This was done to enable a comparison of intensity counts from three systems with varying ranges of data.


0.3


0 0.1 0.2 0.3


Current (mA) Si


MCT


InGaAs


Figure 2 Fwd Bias Emission Intensities.


The signal to noise parameters were also tracked for each measurement. The diode was forward biased and the data was taken as previously noted. The S/N data for the lower level current measurements is shown in Figure 3.


10 20 30 40 50


0 0.05 0.1 0.15 0.2 0.25


Current (mA)


MCT InGaAs


Figure 3 S/N for forward biased diode.


The detectable current levels, along with the signal to noise data show that the IR detectors provide a significant improvement over silicon detectors when used for backside photoemission. This is especially evident at lower signal levels.


General illuminated light imaging performance was also compared. The image quality of the LSM is well documented. [7-9] Both of the IR detector systems were lacking in image quality when compared to the LSM. In fact, image quality seems to be the best area for improvement for the IR detectors in general. For low level magnifications it is possible to resolve large structures well enough to do rough navigation. For high magnifications it is difficult to determine exactly what feature is being imaged.


Figures 4 and 5 show images from the IREM and SUI system respectively. Both of these images cannot match the quality of contrast and the image sharpness that can be seen on images taken with the LSM such as Figure 1. Additionally, the best possible resolution is limited by the wavelength of the incident light source so performance may be in jeopardy as line widths continue shrinking to submicron dimensions.


The IREM system uses a CAD overlay to overcome the resolution problem. Using this feature, emission sites can be directly overlaid onto the device layout.


The precision xyz stage along with specially developed software results in the ability to locate the centroid of an emission site with 0.1 micron accuracy once the CAD overlay is aligned to the actual device image using a 3 point alignment procedure.


Figure 4 IREM image.


Figure 5 SUI image.


All three of the systems detailed have strengths and weaknesses.


1. For standard frontside analysis techniques,although the Zeiss LSM is no longer available in a device analysis platform, in general, silicon based systems are the most commercially available and have been heavily used for device analysis for many years.


2. If backside analysis capability is needed, either due to flip chip processing, or due to the density of metal interconnects, then one of the IR systems might be a better choice.


3. For both IR systems, sensitivity is greatly increased for backside photoemission; however,imaging is the major drawback.


4. The IREM provides a complete system that is currently available commercially.


5. The Sensor’s Unlimited camera is more versatile and can be integrated into a complete photoemission system for significantly less than either of the other options.


The author would like to thank the following individuals.


Mark Aguilar-Aasted of Sensor’s Unlimited Inc.


Olivier Durney of Infrared Laboratories Inc.


1. C.F. Hawkins, J.M. Soden, E.I. Cole, E.S.


Snyder, International Symposium for Testing and Failure Analysis (ISTFA), pp. 55-67, 1990


2. T. Wallinger, ISTFA, pp. 325-334, 1991


3. G. Shade, ISTFA, pp. 121-128, 1990


4. J.S. Seo, S.S. Lee, C.S. Choe, S. Daniel, K.D.


Hong, C.K. Yoon, ISTFA, pp. 73-78, 1995


5. D.L. Barton, P. Tangyunyong, J.M. Soden, A.Y.


Liang, F.J. Low, A.N. Zaplatin, K. Shivanandan,G. Donohoe, ISTFA, pp. 9-17, 1996


6. B. Davis, this conference


7. K. Hussey, S. Selesky, ISTFA, pp.259-265, 1990


8. T.W. Joseph, A.L. Berry, B. Bossmann, ISTFA,pp. 1-7, 1992


9. B. Bossmann, P. Baurschmidt, K. Hussey, E.


Black, ISTFA, pp.351-361, 1992


p 177-185


DOI: 10.1361/cp2000istfa177


Proceedings from the 26th International Symposium for Testing and Failure Analysis, 15-19 November 2000, Bellevue, Washington


Failure Analysis from the Back Side of a Die


Silke Liebert


Philips Semiconductors, Zurich, Switzerland


A back side failure analysis flow has been developed in order to enable failure analysis of flip-chip, leadon-chip dies and within multi-metal-level dies. A combination with frontside failure analysis methods is possible too. The back side flow consists of stepwise bulk silicon removal, electrical and physical failure analysis methods. Four different methods for bulk silicon thinning in order to localize electrical defects using PEM are compared. A method to remove the bulk silicon after PEM analysis to expose the gate oxide level of a die has been developed. Different back side applications like physical analysis of gate oxide defects, passive voltage contrast and microprobing with an AFM tip for detection of interrupts within conductive interconnects are described.


The development of reproducible back side sample preparation and failure analysis methods becomes more and more important because of the increasing number of metal levels within a semiconductor device and the ongoing transition to new packages like flipchip or lead-on-chip. Quite often defects are located within the lowest chip levels which make electrical defect localization from the frontside very difficult.


Otherwise electrical defect localization in flip-chip and lead-on-chip devices is only possible from the back side of the die. To enable successful failure analysis for these die types we have developed a failure analysis flow which contains back side and frontside failure analysis methods. This flow is shown in Figure 1. It consists of back side photoemission microscopy after bulk silicon thinning and electrical recontacting of the die for electrical defect localization. Due to the type of stress test, test results and fault location, the defect type quite often can be deduced. With junction leakage, latch up or aluminum spiking, the die should be prepared for frontside analysis because during further back side preparation the whole active area of the die will be removed. Gate


oxide defects, particles and interrupted conductive interconnects can be analyzed from the front as well as from the back side of the die. Due to the fragility of the die after bulk silicon thinning for electrical defect localization the preparation of defects becomes much easier from the back


Defective multi-metal, flip-chip,lead-on-chip die


Bulk silicon thinning


Electrical recontacting


Back side photoemission microscopy


Bulk silicon


Frontside


removal


analysis


Visual inspection


SEM


Optical


Passive Electrical Analysis Microscopy Voltage probingContrast with AFM


Figure 1 Back side failure analysis flow for multimetal-level, flip-chip and lead-on-chip devices.


side. After bulk silicon removal, optical inspection is possible. Particles or, for example, damage caused by electrostatic overstress might be visible. Gate oxide defects are analyzable by SEM and interrupted conductive interconnects are detectable using Passive Voltage Contrast or electrical probing with AFM.


Electrical Defect Localization using Photoemission Microscopy


Basics


The photoemission microscope (PEM) is a tool for localization of defect sites within integrated circuits.


The PEM analysis is based on the detection of weak electroluminescent radiation that is emitted from defects in integrated circuits as visible and infrared (IR)light. Most defect types emit wavelengths between 500 and 1300 nm. Because of the transparency of silicon in the near IR it is possible to detect failures from the back side of the device. There are several parameters that attenuate the IR light passing through the silicon (Figure 2). The light attenuation is described by the Lambert Beer Absorption Law (Equation 1):


It/Io= (1-RSi)2 exp (-α(λ) ΔSi) (1)It is the transmitted light intensity, Io is the incident light intensity, RSi is the reflection coefficient of silicon, α(λ) is the wavelength dependent absorption coefficient of silicon and ΔSi is the silicon thickness.


The transmission of the light decreases exponential-ly with the thickness and with the absorption coeffiFigure 2 Attenuation of IR light which incidents on parameters bulk silicon.


cient of the silicon. Thinner silicon leads to better light tranmission and a better image during PEM analysis. The absorption coefficient of the silicon is a function of the band gap and the free carrier absorption of the silicon and thus, of the doping concentration and the wavelength. At a given wavelength, the absorption coefficient increases with the doping concentration of the substrate [1]. Finally, the transmission of the silicon is also dependent on the reflection at the silicion surface. During the transition of the emitted light from the optically dense silicon (refractive index nSi ≈ 3.5) to the air (refractive index nair = )


a large amount of the emitted light intensity is lost due to total internal reflection. Moreover, the contrast of the back side image is deteriorated by the high reflectivity of the bulk silicon. The application of an anti-reflective coating (ARC) to the back side silicon minimizes this problem [2]. Defects in bulk silicon as well as surface roughness cause diffuse reflections and attenuate the light emission too.


Bulk Silicon Thinning


Under consideration of the attenuation parameters mentioned above we can deduce the key issues for bulk silicon thinning (Table 1) which enables maximum NIR light transmission during PEM analysis.


Table 1 Key issues for bulk silicon thinning.


NIR attenuating


Parameters


Consequences for sample preparation


Si thickness


Thinning down to 50 -


Bulk silicon doping Highly doped silicon:


thinning down to 50 μm Lightly doped silicon:


thinning down to 100 μm Bulk silicon defects Thinning down to 50 μm Surface roughness Polished surface, resulting surface roughness <5nm


Total reflection


Anti-reflective coating


Using a CCD camera with a wavelength width of 250 to 1100nm, bulk silicon thinning becomes very important. To maintain the mechanical stability of the device, achieve good NIR image quality and retain electrical functionality, 50-100 μm of silicon should remain.. The silicon thickness ΔSi of the polished sample can be determined (Equation 2) by the focal distance ΔF from the polished back surface to the metallization multiplied by the refractive index of the remaining silicon nSi at a given wavelength [3]:ΔSi = ΔF* nSi (λ)


(2)The doping concentration can be taken into consideration by large thinning of highly doped and less thinning of lightly doped silicon. The mechanical stability has to be retained. Influences by defects in the bulk can be minimized by thinning down to 50 μm too. The surface roughness should be as small as possible to avoid geometric distortions of the image and non-uniform illumination during PEM analysis.


Scratches and digs obscure parts of the image. A final surface roughness of 5nm after bulk silicon thinning is recommended [4]. An anti-reflective coating is


Io


It


ΔSi


Si, nSi≈3.5 Air, nAir=1


defects,doping


RSi


helpful due to the optical impedance mismatch between air and silicon. The lateral resolution of backside imaging is reduced because of working with NIR wavelengths [5].


Before silicon thinning, the molding compound located above the back side of the die, the die pad and the die attach adhesive have to be removed. This can be accomplished by using a precise milling tool or by parallel lapping. Because in our case the die pad is located near and at the same depth as the leadframe, the die pad and the die attach adhesive can only be removed within the small region above the die in order to retain electrical functionality. Otherwise the bond wires are cut and have to be reconnected to a new leadframe. Heat slugs, which are sometimes mounted on flip-chip dies, can be heated and mechanically removed. In the following sections, four different thinning methods using a multi-metal-level die embedded in a QFP package are described.


Thinning by Precise Milling


The first thinning method is precise milling. The silicon thinning is accomplished with a diamond milling head at 3000 rpm. Figure 3 shows that the chip corFigure 3 IR image, 200x, of a milled device. Chip


corners are still coated with bulk silicon.


ners are still coated with bulk silicon due to the large diameter of the milling head (3mm). The final polish step is achieved using a hand held drill and diamond pastes. This step causes a wavy surface which results in a non-uniform illumination image in the chip center. After coating the sample with anti-reflective Si3N4 the illumination becomes uniform. Now structure details in the center of the chip are observable(Figure 4), but the die corners are still obscured.


Figure 4 IR image, 200x, of a milled device. After sample coating with anti-reflective Si3N4 a uniform illumination and structure details in the chip center are observable.


Thinning by Anisotropic Plasma Etching


The second thinning method is anisotropic plasma etching in a Nextral NE 860 with Ar and SF6 at a pressure of 60 mT and a UHF power of 1750W. Figure 5 shows distortions of the IR-PEM image caused


Figure 5 IR image, 200x, of an anisotropic plasma etched device, coated with ARC. Surface roughness causes image distortions.


by preferentially etched silicon. The electrical functionality of the die is retained.


Thinning by Wet Chemical Etching


The third thinning method is wet chemical etching with Tetra-methyl-ammonium-hydroxide (TMAH) in an aqueous solution. We use TMAH because the Si:SiO2 selectivity is greater than 4000:1; in comparison, KOH has a Si:SiO2 selectivity of 500:1. The TMAH is a quaternary amine which is totally dissociated in tetra-methyl-ammonium and hydroxide ions in


its aqueous solution. During the reaction between TMAH and Si a silicate is generated (Equation3):2(CH3)4NOH +Si +H2O⇔ ((CH3)4N)2SiO3+2H2↑ (3)The etch rate of silicon at 105°C using 25% TMAH is approximately 10 μm/min. The TMAH boiling point is 109°C. Our bulk silicon etch system shown in Figure 6 consists of a heating system with temperature control unit and stirring option to reach


Figure 6 Construction of a bulk silicon etch system.


a homogenous distribution of the alkaline in the etch solution, a two-necked bottle, a thermometer, a backflow cooler to enable a constant concentration during the etch process, a platinum basket to carry the sample and a lamp to observe the reaction.


The single crystal silicon is preferentially etched against [111] [6]. Figure 7 shows a strong surface


Figure 7 IR image, 200x, of a TMAH-thinned die,coated with ARC. The strong surface roughness causes large image distortions. Roughness caused by etching along the crystallographic planes with the lowest atomic density. After anti-reflective coating,coarse structure details are visible but a precise failure localization in the PEM becomes very difficult.


The electrical functionality of the die is retained. Epoxy packages are resistant in the TMAH solution at parameters described above.


Thinning by Parallel Lapping


The best results were obtained by parallel lapping.


The sample is mounted on a parallel lapping tool consisting of a brass cylinder with a micrometer screw and diaphragm which enables an optimum fit between the sample surface and the polishing plate. The sample rotates around its own axis. Using diamond foils with grain sizes from 15 to 0.1 μm, a planar-parallel polishing is possible. The last step is chemical mechanical polishing (CMP) using colloidal silicon on a polyurethan foil. This foil optimizes the planarity of the surface and avoids edge rounding. After coating with Si3N4 all structure details are visible in the chip center as well as in the chip corners (Figure 8). The PEM image is


Figure 8 IR image, 200x, of a parallel lapped die,coated with ARC. Structure details in the chip corner are visible.


uniformly illuminated and distortions do not exist.


The only disadvantage of the parallel lapping method is that the bond wires are cut during the lapping of the die pad and die attach adhesive. Thus, a reconnection of the die with a new leadframe becomes necessary.


Recontacting of the Die


After bulk silicon thinning by parallel lapping, the chip has to be electrically recontacted. One method is to attach the thinned packaged die to a new leadframe and to create electrical connections between the die and the new leadframe by wire bonding (Figure 9).


Another method is to use mechanical probes to contact the embedded wires. In this case the number of pins is a limiting factor.


Backflow cooler


Lamp


Thermometer


Two-necked


bottle


Platinic basket


with chip


Heating system with temperature control and stirring option


Figure 9 Wire bonded back side thinned device.


Back side PEM Analysis and Corresponding Frontside Preparation


Back side PEM in a spectral range up to 1100 nm allows detection of gate oxide breakdown, junction leakage, aluminum spiking, ESD damage, latch up and more. Further failure analysis can be done from the back as well as from the frontside of the die.


In the following examples, the electrical defect localization within multi-metal-level dies has been performed using back side PEM analysis because during frontside PEM no emission spot could be detected.


Figure 10 shows an ESD stressed sample. A bright emission spot is visible in the contact region. After


Figure 10 IR-PEM back side image, 500x. An emission spot near a contact is observable.


wet chemical preparation from the front side of the die a small hole in the substrate in the contact area is revealed (Figure 11). The metal of the die had covered the photoemission during frontside PEM.


Figure 11 SEM frontside image from the emitting defect in Figure 10. A small hole in the


substrate is visible.


The second example (Figure 12) shows an emission spot during back side PEM in the region of interest of an ESD protection structure. After front side sample preparation, the corresponding defect is visible in the SEM (Figure 13).


Figure 12 IR-PEM back side image, 1000x,of an ESD stressed device.


Figure 13 SEM frontside image of the ESD defect located during back side PEM (Figure 12).


Cut bond wire of the die


New bond wire


to leadframe


Bulk Silicon Removal, Visual


Inspection and SEM Investigations


If there is a suspicion of a gate oxide defect, physical failure analysis can be done from the back side of the die. After pulling the bond wires and removing the ARC by plasma etching or parallel lapping, the SiSiO2-interface can be selectively exposed by TMAH which has been described above. The etch result can be monitored by visual inspection. To find the PEM localized defect site in the SEM it is helpful to use CAD navigation software with a layout flip option for back side investigations of dies. Back side analysis makes the handling of the die much easier because the device is very fragile after bulk silicon thinning,but some problems can occur:


Within ball-bonded devices sometimes an underetching in the pad area caused by microcracks occurs(Figure 14). The reason is the large force during the


Figure 14 Optical microscope image of a bondpad from the back side, 600x. The cracked pad area is visible.


bonding process which results in a weakness of the Si-SiO2 interface in the pad area. The TMAH penetrates through the microcracks and causes an underetch of this chip area. Thus, ESD defects located in the neighborhood of the pad area are destroyed. This problem can be solved by only exposing the chip edges during wet chemical etching because then the etch time is much smaller. Chips with bumps show no problem.


After exposing of the Si-SiO2-interface, ultrasonic cleaning should be avoided because the thin gate oxide layer can be destroyed within the defect region.


Figure 15 shows emission spots during back side PEM caused by gate oxide defects after a CDM stress.


Figure 15 IR-PEM image from the back side with


emission spots in the gate area, 1000x.


In Figure 16 the defect area is shown after back side preparation. The TMAH has penetrated through the gate oxide defect hole and has etched the polysilicon while the gate oxide has not been attacked. After ultrasonic cleaning the thin gate oxide is broken.


Figure 16 SEM image after bulk silicon removal and ultrasonic cleaning. The polysilicon has been etched through the defect hole and the gate oxide is broken.


Thus, the defect hole isn’t visible anymore. The lower gate oxide is broken too. The defect which has been located within this lower gate oxide has not been detectable in the form of an emission spot du-ring PEM analysis. A possible reason for this effect can be that the defect is located between gate and drain which both posses the same doping type. Thus, no recombination is possible which would generate an emission spot during PEM analysis.


Figure 17 shows another example of a gate oxide defect which has been detected after bulk silicon removal. Ultrasonic cleaning has been avoided.


Figure 17 SEM image of a gate oxide defect after bulk silicon removal.


The aluminum contacts as well as the gate oxide of the transistor are visible. In the left bottom corner a gate oxide defect in form of a small pin hole is visible. The TMAH has penetrated through this hole and etched the polysilicon below the gate oxide. Thus, the gate oxide seems to be wavy. This gate oxide defect matched the hot spot of the PEM analysis.


Optical Microscopy from the Back Side


If no gate oxide defect can be found after bulk silicon removal or if other defect types are suspected, optical microscopy at high magnification can be helpful again (Figure 18). Particles or EOS damages may be visible from the back side of the die.


Figure 18 Optical microscope image (500x) from the back side. Transistors, metal connections etc. are visible.


If no defect is found, Passive Voltage Contrast or microprobing using an AFM tip can help to detect interrupted interconnects from the back side of the die.


Passive Voltage Contrast with FIB


After bulk silicon removal, Passive Voltage Contrast is a helpful method to identify floating interconnects.


FIB is the better tool for this voltage contrast analysis because some sample preparations are necessary to get access to the interconnects which can only be achieved with a FIB. A FIB usually works with positive gallium ions Ga+. When a sample is exposed to the ion beam, sputter erosion occurs and secondary electrons (SE), ions and neutrals are emitted from the surface. At the same time Ga+ ions are implanted into the sample surface. Because the yield of secondary electrons is ten times greater than that of secondary ions or neutrals, a net positive charge results on insulating surfaces. The SE emitted from the sample surface are accelerated toward the detector. Using the SE image mode of the FIB (Figure 19), dielectric materials appear dark because the dielectrics are charged by Ga+ ions which recapture SE.


Figure 19 Scheme of back side voltage contrast.


Thus, the SE yield is very small. Grounded conductors like metal or polysilicon lines appear light because the positive charge due to the Ga+ ions can flow off. The SE yield of grounded conductors is much higher than that of insulators. If a part of a conductor is electrically floating it will also charge positively and have no contrast.


Analysis of Floating Polysilicon


To detect a floating polysilicon line, first the sample has to be sputtered in a sputter tool with a gold layer of 50 nm thickness. Now, the interconnects of the device are shorted via active area contacts which are exposed after bulk silicon removal. An orientation on the chip is only possible using a CAD navigation tool with a flip option for back side inspection. To enable the alignment between chip and layout the chip corSiO2


ners have to be exposed. After navigation to the defect site, a small window has to be etched into the gold layer using a FIB with 10 pA beam current at 30 keV. To get better access to the polysilicon lines, the gate oxide should be removed too. It is recommended to practice this opening operation on an unimportant chip site before making the real experiment. During slow scan mode, the sample becomes charged. Figure 20 shows an example of


Figure 20 Passive Voltage Contrast from the back side of a die using FIB, 6000x.


floating polysilicon. The gold layer as well as the small window over the interesting defect region are visible. The floating polysilicon line appears dark,consistent with the theory above.


AFM Back Side Investigation


To detect shorts or opens within the conductive interconnect of the device an atomic force microscope(AFM) used as an electrical prober is helpful. A standard probe station can be utilized with a conductive atomic force microscope tip with a final diameter of less than 10 nm. The AFM senses interatomic forces between probe tip and sample. During the imaging mode the probe tip is lowered onto the sample surface with a computer monitoring the cantilever deflection.


After establishing the contact between the probe tip and the sample surface, the tip is lifted up some nm and moved across the sample surface in a scanning pattern, while the vertical position of the cantilever is monitored. Variation in substrate heights cause the cantilever to deflect up or down. Cantilever displacements of less than 0.1nm can be measured. During the electrical probing mode, a conductive AFM tip enables an electrical contact to conductors like metal or polysilicon interconnects or via plugs with dimensions down to 0.18 μm.


Microprobing of Conductive Interconnects


In Figure 21 the active-area-contacts are exposed by bulk silicon removal. Gate and field oxide, TiSi2 and tungsten plugs are visible. Electrical probing with a microprober is possible. The disadvantage of using one AFM tip and one standard probe needle is that the smallest possible probing distance between two structures is 2 μm.


Figure 21 SEM image of a back side etched device.


The gate and field oxides as well as the TiSi2-layer and the W- plugs are visible. Microprobing between W-plugs is possible.


Figure 22 shows an AFM image of polysilicon lines and a tungsten plug which have been exposed by bulk silicon removal. After sample coating with gold,


Figure 22 AFM image of polysilicon lines and a tungsten plug exposed by bulk silicon removal.


a small window has been opened above the interesting chip area with a FIB. The FIB window size and AFM tip scanning area should be matched. The probe needle establishes the contact to the gold layer which shorted the active-area-contacts and thus the interconnects. The AFM tip can contact a via plug as well as a polysilicon line. By measuring the I/V curve, interrupts within the interconnects can be detected.


Having the layout of the device is very helpful.


To improve the AFM image, the sample can be etched with BHF for some seconds to reach a better topography. This makes precise positioning of the AFM tip easier. Using a curve tracer, a diode characteristic will be measured caused by a Schottky diode which is built up by the outside electrical interconnects.


I would like to thank Martin Herrmann for his active cooperation concerning passive voltage contrast from the back side of a die and Kurt Mayer for his critical comments and the constructive discussions concerning this paper. Otherwise I would like to acknowledge the support of Albert Maurer concerning the wire-to-wire-bonding, of Thomas Keller and Peter Bönsch for the emission imaging and of Hannes Gut for frontside preparations. Not the least, I would like to thank Bert Otterloo for managing the antireflective coating of our samples in Eindhoven and for valuable physical discussions.


1. R.A.Soref, B.R. Bennett, IEEE J. Quant. Electron., 23, 123, (1987)


2. S. Seidel, V.R. Rao, A.N. Zaplatin, F.J. Low,ISTFA Proc., p. 471-476, (1999)


3. J. Colvin, ISTFA Proc., p. 365-375, (1999)


4. D.L.Barton, K.Bernhard-Höfer, E.I. Cole Jr., Microelectronics Reliability, 39, 721-30 (1999)


5. C. Boit, Microelectronic Failure Analysis, 4th edition, 213-229, Materials Park (1999)


6. C. Lue, H.G. Hughes, United States Patent, No.


5,207,866, (1993)


7. K. Krieg, R. Qi, D. Thomson, G. Bridges, ISTFA Proc., p.39-45, (1999)


p 189-194


DOI: 10.1361/cp2000istfa189


ESD Effects on Electromigration Performance of Aluminum Metallization System


J. E. Vinson and M. J. Dion


Intersil Corporation, Palm Bay, FL, USA


The semiconductor industry continues to challenge designer’s ability to provide adequate protection for ESD by scaling to ever-smaller geometries. The metal lines used to connect these circuit elements are also scaled. The effect of non-destructive ESD events on aluminum metal lines is investigated showing a reduction in electromigration lifetime for ESD events close to the failure threshold of the metal. The mechanism contributing to the reduction is a change in the microstructure of the metal resulting in void formation similar to traditional electromigration damage rather than melting and crystallization into smaller grains.


ESD (electrostatic discharge) events are produced by every day actions such as removing a sweater during the winter or walking across a carpeted floor and touching a doorknob. ESD is a charge driven mechanism. It follows four stages: charge generation,charge transfer, charge conduction, and chargeinduced damage. [1] The charge transfer events are modeled by 3 electrical configurations known as Human Body Model (HBM), Machine Model (MM),and Charge Device Model (CDM). Large peak currents can result from each of these models. As an example, the HBM as defined in Specification ESD STM5.1-1998 Sensitivity Testing – Human Body Model (HBM) – Component Level from the ESD Association, produces a peak current of 2.4 amps with the capacitor charged to 4000 volts. This large current travel through the metallization used to interconnect circuit elements (transistors, resistors, capacitors, and inductors) on an integrated circuit. Even though copper is becoming more important in the growth of the semiconductor industry, aluminum based metallization system are used in the majority of all circuits produced.


Using a back side failure analysis flow, it is possible to get access to defects within multi-metal, flip-chip and lead-on-chip dies. Gate oxide defects, ESD/ EOS damage, particles, interrupted polysilicon lines and metal interconnects are detectable using methods like SEM, Optical Microscopy, FIB, Passive Voltage Contrast and AFM. A combination of back and frontside failure analysis methods is possible. Quite often defects which couldn’t be detected during frontside PEM, like defects after CDM stress, can now be precisely located from the back side of the die. A preparation method for back side PEM has been developed consisting of parallel lapping down to 50 – 100 um, sample coating with ARC and electrical recontacting by wire-to-wire bonding. If there is a suspicion of gate oxide defects, these faults can be detected by SEM after bulk silicon removal. The problem concerning the under-etching of the chip edge area within ball-bonded devices during bulk silicon removal can be solved by minimizing the etch time by selectively exposing the chip edges. Ultrasonic cleaning should be avoided. If no defect can be detected with SEM, the sample can be further analyzed using optical microscopy, Passive Voltage Contrast or AFM. Many other methods like FIB cross sections through defects from the back side or EBeam back side failure analysis can complete the failure analysis flow for back side investigations.


As technology scales these metal lines become smaller in cross sectional area, thus lowering their capability to handle the large currents produced by ESD.[2] The sources of ESD are not scaling like the lines and the customer expectation is that newer generations of circuits will be more robust to ESD damage. These factors combine to make it important to understand the effect ESD can have on aluminum interconnect. The currents induced by ESD events produce three potential effects: 1) no change, 2)reduced electromigration lifetime, or 3) fusing damage. Fusing damage is detectable by electrical testing. The circuit would not pass functional testing or it would have increased leakage. A model for predicting fusing damage was previously developed.


[3 , 4] The area of most concern is in the degradation of electromigration performance. This reliability parameter is not measurable on an individual unit but could cause failures in the field several years after the original ESD event took place. This paper presents a study on Aluminum-Silicon-Copper metallization evaluating the effects of ESD on the electromigration lifetime of the metal and looking at the physical changes that take place as a result of these ESD events.


Thermal-Electrical Model


Vinson and Liou in [3, 4] developed a model based on the adiabatic heating and temperature dependent material properties of aluminum. The model is based on finite element analysis of an arbitrary geometry and input waveform. Circuit models for HBM, MM,and CDM were developed. Good agreement between the HBM and MM were shown. The non-socketed model for CDM did not include arc resistance for the higher voltage levels so a divergence between the predicted and actual failure voltage levels was observed. Inclusion of the arc resistance in the discharge path corrected the divergence. Figure 1


shows the agreement between the modeled and measured data.


Figure 1 Agreement between Model and Test Results.


Aluminum Characteristics


Aluminum is a metal with a relatively low melting point. Aluminum melts at 933K and vaporizes at 2720K. Each gram of aluminum requires 9.4•J of energy to take it from room temperature to its boiling point. The heat of fusion for aluminum is 1.35μJ/g and the heat of vaporization is 37.2μJ/g. A parameter defined as enthalpy determines the heat content of a mass of aluminum at a defined temperature. Figure 2 shows the enthalpy of aluminum. The largest energy increase is during the vaporization of aluminum.


Another important parameter of aluminum is the resistivity. Figure 3 shows the resistivity of aluminum as a function of temperature. An important characteristic of the resistivity is the discontinuity at the melting point. Aluminum is more resistive in its liquid form than in its solid form. The sudden change in resistivity produces a sudden change in voltage drop along the line during an ESD event. The voltage increase caused by a resistance increase can damage oxide in a circuit.


Figure 2 Enthalpy (heat content) of aluminum.


Figure 3 Resistivity of Aluminum.


Samples and Stress Conditions


The metal lines chosen were designed similar as NIST electromigration structures with a nominal thickness of 1 μm, length of 800 μm and widths of 2,4, 6, and 8 μm. A single wafer fabrication lot was used in the experiment and samples of each wafer were cross-sectioned to determine the metal width and thickness. The metal lines consist of an alloy of


0.7 weight percent silicon and 0.4 weight percent copper. No refractory metal layers were used in the experiment. The metal layer chosen for evaluation was the 2nd level of a 2 layer metal process. The 8000 angstroms thick overcoat is composed of a layered composite of undoped-doped-undoped silicon dioxide. Phosphorus is used as the doping material.


The structures included extrusion monitors along each side that provided both optical loading during manufacturing and an electrical monitor for any metal whisker growth during EM stressing.


The fusing model described above allows prediction of the internal temperature rise in an aluminum conductor under the influence of an external EOS(electrical overstress) event. Events that do not change the physical structure do not have significant influence on the electromigration performance. The most interesting events are the ones that apply enough energy to melt the line and just less than the energy necessary to vaporize (fuse) the line. The EOS event selected was the Machine Model ESD. The equipment used was a KeyTek ZapMaster System 7/6. Machine model testing was selected because it provided the greater range of energies to deposit into all line widths. The other two models did not have sufficient energy to fuse all metal widths. The selected voltage is determined by the dimensions of the aluminum line under investigation and the model in [3]. Two peak line temperatures were chosen in this experiment: 1000K, just above melting and 2000K, below fusing point. Table 1 shows the voltages needed for the metal lines chosen in this experiment to raise the line temperature to the values shown in the left most column.


Table 1 Stress Matrix for MM Testing.


Peak-T 2μm 4μm 6μm 8μm 1000K 325V 475V 575V 675V 2000K 400V 650V 825V 975V


Data Collection


The resistance before and after the ESD event was measured for all structures tested. This allows predictions of the amount of damage done to the metal line. It was expected that the melting of the lines would cause one of two events: freezing into one large grain or freezing into many smaller grains. The former would cause a lowering in the resistance while the latter would cause an increase in resistance. The number of grain boundaries to overcome is proportional to the resistance. All resistances were measured using a 4-wire measurement technique to maintain the highest measurement accuracy.


An even more sensitive measurement of microstructure damage is found in the thermal coefficient of resistance (TCR). TCR is a fundamental characteristic of the metallization and is dependent only on the residual resistivity of the metal which is determined by differences in the structural order of a pure, bulk metal, that contribute to electron scattering.[5] A well ordered metal system will have


a high TCR, while a poorly ordered system, with structural variation will have a lower TCR. TCR was measured using JEDEC Standard JESD33A on virgin(unstressed) metal lines. Following the measurement,samples were stressed and the measurement repeated.


Sample lifetime was the major portion of the experiment performed. Electromigration stressing was performed with a current density of 1E6 A/cm2 at an ambient temperature of 250°C. Failure was defined as a resistance change of 20%; although many of the structures failed to an open circuit before reaching 20% change. Failure distributions were statistically analyzed assuming a log-normal distribution following JEDEC standard JESD37,including 95% confidence limits on the failure time median’s (t50) and sigma.


The last area of data collection was physical observations of the metal lines. The surrounding passivation was removed chemically and the metal lines inspected optically and with a scanning electron microscope (SEM). Special attention was paid to looking at the grain structure of the metal lines to note the change of state.


Resistance Measurements


Figure 4 shows the resistance values for the 2 and 6 micron line widths prior to stressing. The 2 micron line showed more variability most likely due to the variability in the etch process. The larger width lines were more consist in their line widths. After stressing the variability increased, as did the resistance values.


Figure 4 Resistance Values prior to stressing.


Thermal Coefficient of Resistance


Figure 5 shows the results of the TCR measurements for all 4 line widths. Each line width shows a virgin group of lines along with lines stressed to 1000 and 2000K. It is clear that the ESD event had little effect on the lines stressed to 1000K but the 2000K stresses had significant effect. The TCR values were significantly lower on the 2000K samples over all line widths indicating a significant increase in structural variation along the line. The 1000K pulses added only slight structural variation to the metal lines.


Electromigration Results


The EM failure distributions for the 2 μm and 4 μm structures are shown in Figures 6 and 7 respectively.


Both the 2 and 4μm lines subjected to 2000K temperatures fail earliest. The sigma’s are very large indicating much variability in failure time when compared to the non-stressed structures. The 1000K stressed lines show a slightly lower median lifetime with an increased sigma. The unstressed line lasted the longest and was terminated prior to reaching 50%cumulative failure. The effect of ESD damage on the 4um line was not as drastic. The 2000K lines had the shortest median life time but the 1000K and virgin lines were statistically the same. The difference in life times between the 1000 and 2000K lines was not as much.


Figure 5 TCR values for 25°C.


Figure 6 2μm electromigration results.


Joule heating of the 2 μm and 4 μm lines was 5°C and 12°C respectively. Adjustments of the lifetimes for a direct comparison due to the temperature difference does not substantially change any attributes but is shown in Figure 8 for completeness. For direct comparison of the 2 and 4 μm data, the 4μm failure times were normalized to 255°C (528K), the stress temperature of the 2μm line. The normalization constant used followed the Arrhenius relationship with a thermal activation of 0.6eV.


Figure 7 4μm electromigration results.


Figure 8 Normalized electromigration results.


Optical and SEM Inspection


Samples of each metal line width were investigated using optical and SEM microscopes both before and after the MM ESD stress. Figure 9 shows a 6-micron line with no-stress. The silicon dioxide was removed using wet chemistry. A technique known as a “Flash HF” was employed. With this technique a drop of concentrated hydrofluoric acid is placed on the die surface and the sample is immediately placed in a rinse tank of deionized water. The “Flash HF”technique minimizes the attack on the aluminum metal that can occur with buffered HF. Figure 10 shows a 1000K stressed line. The grain structure of the two lines is similar. There is no evidence of melting in the 1000K line even though there was sufficient energy pumped into the structure for the entire length of the line to melt. This result was common for all of the 1000K lines. No 1000K stress line showed evidence of melting (no change in grain structure) even though TCR measurements show that damage to the microstructure did occur. It is believed that the damage occurred along the grain boundaries.


The energy placed into the system went into mass movement rather than joule heating. This observation is more evident from the 2000K stressed lines.


Figure 11 and 12 show two lines that were stressed to 2000K. The obvious factors observed are the voids that have formed. These voids are in the shape of grains or along grain boundaries. It appears that a rapid electromigration has occurred because of the ESD energy. The ESD pulse duration is on the order of 1 microsecond. Areas away from the void do not show evidence of melting even though far more energy was applied to these lines than is required to


cause melting. It is hypothesized that most of the energy went into mass movement of the aluminum to create the voids.


Figure 9 SEM view of unstressed metal -note grain structure.


Figure 10 M view of 1000K stressed line -


little difference from unstressed line.


Samples were ESD stressed with the overcoat removed to determine if the oxide was influencing the physical observation in the metal. The “Flash HF”removal technique was employed to remove the overcoat. Without the overcoat, the metal lines melted and became liquid. An ESD event is an adiabatic event – no heat loss is realized into the surrounding oxide. Given this, the oxide surrounding the aluminum must confine the aluminum into its given form not allowing the surface or volume to change.


The adhesion of the oxide to the aluminum is believed to play a part in this process also. The constriction allows the energy from the event to be converted into


kinetic energy of the aluminum atoms rather than joule heating of the mass.


Figure 11 SEM view of 2000K stressed line -grains are missing.


Figure 12 EM view of 2000K stressed line -


grains are missing and slit void forming.


This study showed that ESD events can degrade the electromigration performance of aluminum interconnects. ESD has more influence on the smaller lines than on the larger lines. The larger thermal mass and larger cross section allow the line to absorb more energy without degradation. The degradation mechanism present as a result of ESD damage is not melting and recrystallization into smaller grains as originally believed. For encapsulated aluminum systems, much of the energy in an ESD event is converted into mass movement of the aluminum via


the grain boundaries similar to what would be experienced over a longer period of time during traditional electromigration method. The difference is this time frame for electromigration occurs over a very small time scale (< 1μs).


The authors would like to thank the support of Ray Wurzbacher for his assistance conducting the experiments and taking the data on metal thickness and width.


1. J. E. Vinson and J. J. Liou, “Electrostatic Discharge in Semiconductor Devices: An Overview,” Proceedings of the IEEE, Vol. 86,No. 2, Feb. 1998, pp. 339 – 418.


2. Ameraskera and C. Duvvury, “The Impact of Technology Scaling on ESD Robustness and Protection Circuit Design,” Proceedings of the EOS/ESD Symposium, VOL. EOS-16, 1994, pp.


237 – 245.


3. J. E. Vinson, “Aluminum Interconnect Response to Electrical Overstress,” International Symposium for Testing and Failure Analysis,Dallas Texas, Nov. 1998.


4. J. E. Vinson and J.J. Liou, “A New Model for Aluminum Interconnect Fusing caused by ESD,”3rd IEEE International Caracas Conference on Devices, Circuits and Systems, Cancun, Mexico,March 2000.


5. N. F. Mott, and H. Jones, “The Theory of the Properties of Metals and Alloys,” Dover Publications, Inc. New York, p. 286, 1958.


p 195-201


DOI: 10.1361/cp2000istfa195


Evaluation of On-Chip ESD Supply Clamp Robustness by In-situ Floating Power Bus Monitoring


Michael Fliesler and Ian Morgan


Continuous improvements over time to a CMOS Flash Memory technology resulted in significant improvement in Human Body Model (HBM) ESD immunity for “I/O’s” to Vcc power supply and Vss ground pins. Remaining low level failure modes in the die core included elevated standby current that in some cases could not be localized even with extensive chip de-processing. In addition an apparent functional failure upon post stress ATE test was isolated for certain part revisions.


Routine separation of Vss/Vcc supply pin combinations from “all other pins” during HBM ESD test allowed identification of the several failures occurring in the die core. Failure analysis and corrective action is described. Additional diagnostic testing using separate polarity HBM pulses aided in tracing the conduction path causing the apparent functional failure and prompted investigation of HBM tester dynamic properties. It was determined that the magnitude of the “second” HBM pulse in certain testers was sufficient to cause a false powerup condition which results in apparent functional failure upon subsequent ATE test.


In-situ monitoring of the Floating Power Bus response (in this case Vss) during application of HBM stress to the Input-pad to Vcc-pin combination revealed a transient caused by the “second” pulse that allowed such apparent failures to be invalidated.


Further more, monitoring the in-situ floating Vss bus response to the HBM allowed conclusions to be drawn as to the utility of different power bus and Vss/Vcc supply clamp layouts, thereby allowing improvements to die layout to be implemented.


Significant improvement in basic HBM* immunity for “I/O’s” to supply and ground were obtained for a sub-μm CMOS Flash Memory technology as a result of continuous improvements introduced over time with process scaling and die revision. The improvement in shunt protection also resulted in enhanced Charged Device Model[1] (CDM)


immunity. However, remaining low level failuremodes included some cases of elevated standby current that could not be localized even with use of emission microscopy* and extensive chip deprocessing. Determination of the root cause of ESD damage internal to die core became very difficult.


Analysis of full die CMOS I/C response to humanbody model (HBM) stress is complicated by many factors including: chip layout (pads, power-supply bussing, supply clamps), package type, and tester parasitic elements; e.g., see*. Measurement techniques such as transmission-line pulse (TLP)testing do not measure node behavior deep internal to the die when an Input or I/O pad is stressed.


However, diagnostic separation of ESD polarity,rather that the standard (positive, then negative)stress application to each “pin pair” *, suggested that on-chip power supply protection circuits had different robustness to each stress polarity.


Significant tester-to-tester variations depending upon construction were observed in the magnitude of the HBM waveform “second pulse” aberration due to the model discharge relay. We found that internal node behavior could be inferred by monitoring the die transient response to this “second pulse” via the floating power bus. This measurement technique was used to determine root cause of the unusual functional failure found after ESD stress and allowed this apparent failure to be ruled invalid. In–situ monitoring the transient voltage on the floating power bus during HBM excitation while stressing an Input (or I/O pad) to the Vcc supply pin allowed conclusions to be drawn as to the utility of different power bus and supply clamp layouts.


ESD Protection Scheme


Since a diode between pad and Vcc is not allowed due to possible signal over-shoot the Input-only ESD protection schemes in AMD CMOS Flash technologies rely on parasitic bipolar action from a gate coupled N-MOSFET to both Vss and Vcc supplies. Dynamic gate control is provided using a dummy driving buffer; a compact model for such gate coupling in the gc-NMOS has recently become


available . The equivalent circuit for an Input-only pin is shown in Figure 1 with key parasitic elements indicated. Pins used in initial test modes are similar,but use an integrated pair of NMOS in cascode configuration similar to the high voltage Vpp protection used in earlier EPROM’s.


Figure 1 FLASH input-only protection using dual


gc-NMOS and showing dummy buffer for dynamic gate control.


The I/O pins use an NMOS pull-down transistor to Vss and a PMOS pull-up to Vcc as shown in Figure


2. The parasitic p-n diode to Vcc resulting from the n-Well of the PMOS pull-up transistor plays a major role in ESD protection.


Figure 2 Self protective CMOS I/O.


Note that gate coupling for the I/O and Input-only is achieved from the pre-drivers and dummy driver such that the parasitic bipolar mode is entered without passing through the localized snapback region. Power supply clamps between Vcc and Vss utilize a large Weff gc-NMOS with explicit capacitive gate coupling to provide a sufficient time constant so that again the snapback region is avoided.


Conduction Mechanism & Path


Depending on the HBM stress polarity and pin combination under test, the conduction path shown in Table 1, involves a forward biased diode, parasitic bipolar transistor conduction, or both. When an Input


pin is stressed negative with respect to Vcc the discharge conduction path also involves the on-chip power-supply clamps shown in Figure 3.


Table 1 Conduction Paths for “Input-Only” Stress


GND PIN


POLARITY


CONDUCTION PATH


Vss (+) Lateral BJT: gc-NMOS


Vss (−) Forward Diode – Drain to subs


Vcc (+) Lateral BJT: gc-NMOS


Vcc (−) Lateral BJT plus Vss/VccClamp


The conduction path for the I/O stressed negative to Vcc requires similar action of the Vss to Vcc power supply clamp, as shown in Figure 4.


Figure 3 Conduction path for input pin stressed negative with respect to vcc.


It is common practice to reduce the effect of output switching noise in the case of large die, or when memory organization requires many I/O’s, to use isolated Vcc supplies; (i.e., separating power supply pins) and using a split ground as shown in Figure 5.


Figure 4 Conduction path for I/O stressed negative


with respect to vcc, showing action


of vss/acc supply clamp.


In this case the die core supply pair is shown as Vss/Vcc and the “quiet” I/O supplies as VssQ/VccQ.


Some primary conduction paths during discharge are listed in Table 2 It is noted that more than one“device” in series is required for some discharge paths.


Figure 5 Self protective CMOS I/O with isolated vcc power pins and split ground showing required power supply clamps.


If a power clamp does not trigger properly for any of the examples discussed then damage may occur at the pad or at internal die nodes, even though protection may be adequate for other types of ESD stress.


Table 2 Conduction Path for “I/O” Pin Stress, with


Separated Vss and Vcc Power Supplies


VssQ (+) Lateral BJT: gc-NMOS


VssQ (−) Forward Diode: Drain to Subs


Vss (+) Lateral BJT + Vss-VssQ Clamp


Vss (−) Forward Diode: Drain to Subs VccQ (+) Forward Diode: Drain to Vcc


VccQ (−) Lateral BJT: gc-NMOS


Vcc (+) Forward Diode + Vcc Clamp


Vcc (−) Lateral BJT + VccQ/Vcc Clamp


Improper power clamp operation can occur as a result of inadequate electrical width, too high a trigger voltage, or high resistance due to excessive bus resistance between the clamps and die core or between clamp and power pin.


ESD Test Methodology


HBM stress is routinely applied to each pin (pair)combination using three positive (3+) zaps followed by (3-) negative zaps. Separate samples are used for each stress level/pin combination to facilitate batch ATE pre/post stress. ATE test is required to ensure


functionality of “passing” parts and to examine for parametric shift since some (other) product use pullup/down terminations at “I/O”.


Pin Combination Super-Set


AMD standard practice, as disclosed * to ESDA Device Level Working Group 5.1 has been to use a superset of the pin combinations defined in MIL STD-883, method 3015* as shown below in Table 3.


Table 3 Separation of Supply Pins from “I/O” Pins


CONNECT INDIVIDUALLY IN TURN TO EXCITED TERMINAL A.


COMMON COMBINATION TO GROUND TERMINAL B


I. All “I/O” pins.


( All Input’s, Output’s Only)


VSS1, to VSSX


II. All “I/O” pins.


VCC1 to VCCY


III. Each “I/O” pin.


All other I/O’s


IV. Each Named Supply Pin in Turn.


Each Remaining Named Supply Pin or Pin set.


Full pass/fail diagnostics are achieved for one test pass by separating all Vss and Vcc power pins from the “all pins” to named supply set pin combinations.


provides a peak current that compares to the peak HBM current that also fails the device under test.


When HBM is used for its primary purpose of qualification testing it stresses both the ESD protection circuit and protected core of the IC. When TLP is used in its primarily function as a design tool,it has the additional analysis advantage that allows testing each element used in protection structures to determine their individual pulse current capability and dynamic I-V characteristics. This provides the designer with knowledge on how each will perform in the final circuit assembly. Knowing the current path a stress pulse takes through an ESD protection structure and its dynamic impedance at I and V values allows the optimum design of each element.


Each diode, transistor, resistor and metal interconnection can be individually TLP stress tested to provide a library of component size, layout, and optimum construction to be used in a complete ESD protection circuit. It can provide clear electrical failure analysis data on the voltage-current characteristics of each component. When the length of the test pulse is included, the energy capability of the elements is available.


A TLP pulse curve tracer (TLP-CTR) is an excellent electrical analysis tool because it uses rectangular pulses with a flat top [29]. This allows accurate measurements of both the voltage across the device and the current through the device by averaging the digitized data for some length of time near the end of the pulse. Testing the complete IC using the TLP pulse curve tracer provides an I-V characteristic curve which identifies the electrical behavior of the tested pin relative to a grounded pin


We made measurements using a constant impedance TLP system, which we define as TLP-50 (Figure 1).


We define this because it uses a constant impedance of 50 ohms throughout the system up to the pads of the Device Under Test (DUT).


One of the advantages of maintaining a 50 ohm constant impedance for the pulse traveling through the system is that the pulse rise time and flat top of the TLP pulse is passed through constant impedance connections and is not degraded. Using the circuit arrangement of Figure 1, allows the DUT to be momentarily disconnected from the pulse source after each pulse with a coax switch so that DUT can be connected to a DC voltage source and pico ammeter.


During this time a DC leakage measurement at the selected DC voltage (usually Vdd +/- 10%) is made after every test pulse with the DUT in situ. The leakage current measurement is then plotted with the I-V plot, against the measured pulse current (that is,the current through the DUT). The constant impedance system allows both the DUT response and DUT leakage measurements to be made when testing


either socketed devices or when TLP stress testing on wafers.


Figure 1 TLP-50: a constant impedance 50 ohm TLP system.


Some researchers have published data on the use of the traditional Curve Tracer (CTR) to stress test the ESD protect structures [ 30 ]. However, since the CTR uses extremely long pulses (μsec rise time and pulse width), it causes additional joule heating and EOS type failures. These longer pulse currents cause the ESD structures to fail at lower currents than that caused by the much shorter length ESD pulses. The CTR pulses are much longer (μsec) than HBM 150 nsec ESD pulses or the 100 nsec TLP pulses. TLP has typically used 100 ns long rectangular pulses to produces failures at the same peak currents as HBM.


Damages seen from CTR failures are immediately visible after de-capsulation and occurs on the top surface of the device [31]. These are EOS failures compared to ESD failures which occur in the subsurface of the IC [ 32 ] and which require deprocessing down to the silicon level to see the physical failures.


Calibration and Verification


Short and Zero ohms


At any point along the transmission line, there exists a source impedance of 50 ohms and a load impedance of 50 ohms. To be certain that measured TLP data is accurate, a TLP test systems must be calibrated and then verified that the pulse calibration factors are correct. TLP systems lend themselves to easy calibration by making a series of tests using a short(zero ohm) and an open (infinity ohms). Another low value resistor can be used that has a similar slope to the slope of the dynamic resistance of protection structures when in their high current conduction mode. A common value we use is 5 ohms.


Zero Ohm (short) Load Impedance


The figure 2 below shows that the transmission line is terminated with a load impedance of 0.00 ohms.


Theoretically, the maximum current in the 0.00 ohms load is (500v/50 ohms) equal to 10 amps. This 10 amp maximum is achieved by the TLP-50 system.


The voltage pulse is reflected back to the source with opposite polarity and the correct I-V curve is a vertical current line with “zero” voltage as shown in figure 3 . Hence the ideal TLP system shou ld not add any “unwanted” voltage to the measurements.


Figure 2 Basic calibration with short circuit (zero ohm).


Figure 3 Typical short circuit calibration Plot.


Infinity Ohm (Open) Load Impedance


The figure 4 below shows a transmission line terminated with a load impedance of infinity ohms(open circuit). Theoretically (500 V/ ∞ Ω) there will be no current flowing in the circuit. Here the voltage pulse is reflected back to the source with the same polarity and the resulting I-V curve is a horizontal line shown in figure 5.


Figure 4 Calibration with open circuit.


Figure 5 Typical open circuit calibration Plot.


5 Ohm Load Impedance


The figure 6 below shows a transmission line terminated with a load impedance of 5 ohms (device on impedance). Theoretically (500 V/ 55 Ω) there will be 9.0 amps in the calibration circuitry and the curve (diagonal line) is as shown in figure 7. Note that for a 50 ohm load impedance, the maximum current in the circuit is 5.0 amps, and a similar diagonal line is obtained if the transmission line is terminated with a 50 ohm impedance.


Figure 6 Calibration with 5 ohm load.


Figure 7 Typical 5 ohm calibration Plot.


Since the perfect short circuit (zero ohm) will have a perfectly vertical straight line with no voltage variations, the amount of the voltage variation is a measure of the short circuit measurement error [ 33 ].


This applies also to the open circuit measurement which results in the horizontal line. Further details are to be found in references [29] and [33].


The Gaussian Waveform


The broad tolerance of 2-10 nsec range in rise time as specified in the HBM standard adds to the correlation problems. The risetime variation and added ringing of the HBM tester is avoided in the TLP-50 by using controlled 0.2 nS, 2.0 nS, and 10.0 nS Gaussian shape risetime pulses. Controlled Gaussian rise time test pulses with no overshoot or ringing as shown in Figure 8. These Gaussian waveforms are used because they transition gradually as do most “reallife” HBM threat pulses. The Gaussian waveforms are obtained with special filters that can produce the initial rise in a gradually increasing and controlled manner. High voltage pulses in nature are usually produced this way, so being able to repeat the shape of the initial rise provides an inherent simulation of naturally occurring threats. Such risetime information could also provide data for the fundamentals of a TLP standard test method or standard practice.


Figure 8 displays the 0.2 nsec, 2.0 nsec, and 10.0 nsec Gaussian rise times without any ripples.


The TLP Load Lines


The use of the load line concept to define the pulse current and voltage capabilities of any TLP system is shown below in figure 9. The first load line represents the 50 ohm load line at the maximum test pulse amplitude of 500 volts and the second is at half maximum amplitude. The figure 9 shows that the TLP-50 has a maximum pulse current of 10 Amps into a short circuit and a maximum pulse voltage of 500 Volts into an open circuit or infinity ohms. The different slopes of constant resistance plotted with the TLP system are all shown starting at the origin, and are labelled characteristic lines. The open (infinity ohm) circuit horizontal line and the short (zero ohm)circuit vertical line are obvious in figure 9. Note however that the “playing field” area for designers is much smaller than the 500 volts indicated in figure 9.


We can attribute this to the fact that designers deal with single protection structures and not packaged ICs where other circuit interactions come into play.


Vss/Vcc power supply pins are then tested as an additional pin combination. This allows failures that occur purely due to stress between Vss and Vcc to be readily distinguished from those due to stressing an“I/O” pin to a supply pad. Additionally in this investigation we examined the effect of polarity separation.


Failure Analysis


Analysis of the tested superset of pin combinations showed that the sporadic elevated Icc failures only occurred following stress between Vss and Vcc.


Some of these failures were not readily located by emission microscopy. However, two types of failure signature [9] internal to the die core were readily identified.


Failures in Die Core


The first type of failure was due to inadvertent thick oxide bipolar clamp action between adjacent N+regions connected across Vss and Vcc internal to the die core. This particular failure signature * shown in Figure 6 was easily suppressed by improved layout design rules. Placing a P+ guard-bar/substrate tie between the adjacent N+ regions tied to the source of the “pull-down” prevented triggering the bipolar due to source-to-substrate bounce and killed the base of the parasitic bipolar.


The second failure type is shown in Figure 7. This shows local failure between N+ source and drain regions in a large internal NMOS clock driver. Based on previous work it was concluded that this large minimum channel length transistor also acted as a clamp to protect the die core by triggering before the power supply clamp/s became active. This failure type required improvements in power supply clamp placement and ensuring that the minimum clamp Weff was at least as great as that in the Input.


Figure 6 Failure due to un-intended clamp action at


far-internal parasitic NPN directly


Across vcc and vss Supplies.


Figure 7 Local failure in a large


internal NMOS driver.


Apparent Post Stress Functional Failure


In addition, a mysterious low level functional failure occurred at ATE post ESD stress for certain die revisions. This failure was hard to explain and much harder to solve. While we initially suspected I/O pin interaction, it was discovered to occur only for a negative stress applied to Input pins to Vcc. Thus the discharge path involved the Vss/Vcc power supply clamp. The further observation that failure most often occurred for parts in which multiple Vss and Vcc supplies were used to isolate the “noisy” I/O from the“quiet” internal logic and die core caused further concern for power supply clamp design.


The frequency of this failure, if it occurred, appeared to depend on the number of part address pins. We showed further however that this failure could indeed be induced on some parts by repeatedly zapping an


arbitrary selected address pin many times. This led us to more carefully examine the dynamic behavior of the HBM tester, particularly for the case of negative stressing product input to Vcc.


Dynamic Behavior of HBM Tester


Commercial HBM testers are available from several manufacturers but actually differ in their construction and associated parasitic elements.


The “Second” Pulse


A surprising artifact was re-discovered during the detailed re-evaluation of tester behavior. A “second”HBM-like pulse occurs at around 20-25 μs after the initial HBM discharge as shown in Figure 8.


Figure 8 The HBM “Second” pulse aberration


showing delay after initial discharge.


While EIA/JEDEC Test Method A114-A is not cognizant of the existence of a spurious second pulse,the ESDA Standard Test Method STM-5.1 requires verification that “any (additional) spurious pulse is less than 15% of the magnitude of the main pulse”.


The second pulse aberration has the same polarity as the initial pulse and very similar wave-shape, as shown in Figure 9, but is of much lower amplitude. A delayed trigger is required to display the correct amplitude for the second pulse as indicated.


Figure 9 The HBM “Second” Pulse Aberration has Remarkably Similar Wave-Shape to Initial Discharge.


The Discharge Relay


The “bounce-less” mercury-wetted relay used as the HBM discharge switch is the recognized as the source of this second pulse. Such relay’s are intended to eliminate the possibility of “bounce” when making contact and eliminate arcing when breaking contact.


Bounce does not occur in these relays since each contact is wetted with mercury. The metal contacts still tend to bounce (as in a traditional dry relay);however, the mercury maintains a physical connection between the contacts due to surface tension. The mercury forms stringers between the two contacts as they bounce off each other. Since there is no break in electrical continuity any possibility of multiple discharges due to bounce should be eliminated. When breaking a powered circuit the Hg arc is quenched. This is of particular importance since arcing (as in a dirty relay) can readily generate electrical fast transients, (EFT) *.


The model capacitor is pre-charged to a high voltage in the HBM; hence, the initial discharge occurs through a Hg arc before any physical connection (i.e.,before any metal to metal contact). During the initial discharge the voltage on the capacitor drops and at some point, the voltage becomes too low to sustain the arc. The discharge therefore ceases but some residual charge remains on the capacitor.


Approximately 20-25 μs after the initial arc conduction, the relay contacts make physical connection; the low resistance path created then allows the remaining charge on the capacitor to be discharged by direct injection. This is manifested as the second pulse.


Tester Differences


HBM testers from two different vendor’s were characterized and compared. The amplitude of the second pulse for one brand of tester examined was only about 5% but for another used here the amplitude was as large as 10%. In the former case with a pulse magnitude of only 5% we did not find any evidence of the post-test functional failure. In the latter case (used here) the second pulse amplitude of 10% was approximately the same for several testers having pin count capability of 256 and 512 pins. This appears to be due to discharge relays of different construction used by the two vendors.


In-Situ Pin Monitoring


We found that when an Input or I/O pin DUT pin is stressed to the Vcc supply pin the consequent transient voltage of the floating Vss power bus can be usefully monitored as illustrated in Figure 10 by using an oscilloscope and a high impedance probe.


The figure also shows the use (a) of a current probe to record the HBM short circuit waveform and detect the second pulse.


Response of Address Pin


Figure 11 shows little response from a nearby address pin (A12) upon negative zapping Input (A5) to Vcc.


Figure 10 Scheme for in Situ Monitoring Response


of a Floating Pin during HBM Zap.


However the very large negative excursion of ~ 6.6 V upon monitoring the pin of the floating Vss power bus suggests that the response depends upon the Vss/Vcc power supply clamp action across the die core capacitance.


Figure 11 Response of an Address Pin (A12) and the Floating Vss Pin when Zapping Address Pin (A5).


Note large Voltage Excursion for Vss.


On this particular die the Vss and Vcc pins were located at the same end of the die with a single power supply clamp, as shown in Figure 12. There was no clamp at the die end remote from the power pin location; in addition the Vss and Vcc buss’s between the Inputs and I/O’s located at the die ends were narrow.


Floating Power Bus Monitoring


For comparison the transient response of the floating Vss bus for a part, without apparent functional failure and with known good layout practice, displays a very limited negative excursion of only 240 mV, as is shown next in Figure 13.


Figure 12 Die Layout with Incorrect Power Pad Placement, High Bus Resistance and Inadequate Power Supply Clamps.


The layout for this known good die is shown in Figure 14. Note that it has a similar height to the previous example but has twice the die area.


Figure 13 A Part With Known Good Clamp and Die Bus Layout Showing Vss Excursion of Only 240 mV.


The Vss and Vcc busses between the die ends are almost twice as wide, there are Vss and Vcc pins at both ends of the die and power supply clamps are distributed around the die periphery.


Figure 14 Layout for the Good Die a Showing Multiple Supply Clamps.


The Second HBM Pulse


The second pulse was largely forgotten by early workers and may be unknown to more recent users of HBM testers. The reason for examination for spurious pulses in the ESDA STM-5.1 is not described in the document. We re-discovered this aberration causing an apparent functional failure in FLASH memory post HBM stress when using one brand of tester, but have since found it a useful tool in device analysis.


Effect of Substrate Transients


Flash memories have extremely low (<500 nA)standby current, thus any substantial substrate voltage transient will only be discharged by diode leakage current. If the transient Vss/substrate-to-Vcc bias is in the -3V range (nominal operating +3V Vcc) for a duration of several micro-seconds, a false power-up condition can occur. Brief but un-predictable operation may then result in apparent functional failure upon subsequent ATE test. But if the second pulse is high enough in amplitude to trigger the clamp, and if the power supply clamp and metal routing are well designed; then the voltage across the background capacitance between the Vcc and Vss buss’s is limited.


Power Bus Supply Clamps


In 1984 one of the authors described Vss and Vcc power supply clamps to provide safe discharge path’s between remote I/O’s and for use between multiple isolated power supplies. Russ et al have recently shown that the “background“ capacitance, consisting of the core capacitance and that of the other floating pins, must be included in a model to predict in-situ failure during HBM stress. Our observations can be simply explained by the simple example in Figure 15.


Figure 15 Effect of Bus Resistance and Power Clamp Design on Transient Voltage Across the Die


Core when an “I/O” is Stressed to Vcc.


Transient voltage stress will occur across the die core capacitance unless limited by supply clamp action between the supplies with suitably low trigger voltage. Dynamic resistance and parasitic metal bus resistance must be small enough to provide a rapid decay time to minimize the duration of stress across minimal features in the die interior.


The magnitude of the “second” pulse aberration on certain HBM testers is sufficient to cause a false power-up condition in FLASH memory parts that can result in apparent functional failure upon ATE test.


Thus the product appeared to fail using one brand of HBM tester, but not when using another brand. Such apparent failures were invalidated following in-situ monitoring during HBM stress, which revealed a significant transient voltage on suspect parts.


When applying stress to the Input-Only pad-to-Vcc supply pin combination we noted large differences in magnitude for the in-situ transient response of the Floating Power Bus (in this case Vss),


We concluded that such differences were due to differences in power supply clamp operation and indicated the varying utility of power bus and supply clamp layouts. These conclusions thereby allowed improvements to die layout and metal routing to be implemented.


The authors thank C.Hatchard for early assistance with the monitoring scheme and S. Beebe for technical discussion. We are especially grateful to S.Johnson for access to the HBM testers and continued support in the ESD Laboratory.


1. ESD Association Standard Test Method, STM5.1, “Electrostatic Discharge (ESD) Sensitivity Testing: Human Body Model (HBM)


- Component Level”.


2. ESD Association Standard, S-5.3, “Electrostatic Discharge (ESD) Sensitivity Testing – Charged Device Model (CDM) - Component Level”.


3. Ed., Wagner, “Failure Analysis of I/C’s - Tools and Techniques“, L.A., Klweuer Academic,Boston, 1999.


4. S.G. Beebe, “Methodology for Layout Design and Optimization of ESD Protection Transistors,” Proc. 18th EOS/ESD Symp., 1996,pp. 265-275.


5. See reference #1.


6. H. Wolf., H. Gieser, W.Stadler, “Bipolar Model Extension for MOS Transistors considering Gate Coupling Effects in the HBM Domain”, Proc.


20th EOS/ESD Symp., 1998, pp. 271-280.


7. I.H.Morgan, AMD, Disclosure to ESDA Standards Committee, 5.0-Device Level,February, 1997.


8. MIL-STD 883, Method 3015, “Electrostatic Discharge Sensitivity Classification”.


9. I.H. Morgan, “Identifying EOS and ESD Failure Signatures”, Proceedings 3rd ESD-Forum,Eibsee, Bundesrepublic Deutschland, Dec.,


1993.


10. I.H. Morgan, “EOS & ESD Failures in CMOS I/C’s”, in “Microelectronics Failure Analysis”,National Technical University, Course NTU-I 535, University of New Mexico, 1999.


11. EIA/JEDEC Test Method – A114A, “Electrostatic Discharge (ESD) Sensitivity Testing:Human Body Model (HBM)”.


12. See reference #1.


13. H.W Ott, “Noise Reduction Techniques in Electronic Systems”, Wiley, New York, 1988


14. I.H. Morgan, “General Recommendations for an Architectural ESD Methodology giving Enhanced ESD Immunity for all AMD Products”, AMD Technical Report #272, 1984.


15. C Russ, H. Gieser, P. Egger, P. Kropf and K.Verhaege “Compact Electro-Thermal Simulation of ESD-Protective Elements’,Proceedings ESREF, 1993.


p 203-213


DOI: 10.1361/cp2000istfa203


Transmission Line Pulse Testing of the ESD Protection Structures of ICs.- A Failure Analysts Perspective.


Leo G. Henry


ESD/TLP Consultant, Fremont, CA, USA


Jon Barth, John Richner,


Barth Electronics Inc., Boulder City, NV, USA


(3) Sarnoff Corporation, Princeton, NJ, USA


The IC industry continues to find ways to improve the ability to correlate the electrical failure signature of devices with the physical failure location using different techniques. The purpose of this work is to show that improved transmission line pulse (TLP)testing technique of ESD (ElectroStatic Discharge)protection structures can provide accurate identification of leakage current to better identify where ESD stress testing should stop and failure analysis should begin. Besides the traditional current and voltage measurements at the Device Under Test(DUT), this new TLP testing technique includes the ability to correct for the measurement system losses for improved accuracy. The pulse width of the TLP is chosen to provide the same current amplitude damage level (electrical) as is found in the Human Body Model (HBM) ESD stress testing. This allows a one to one correlation between the two methods and hence the means to correlate the electrical damage of the device and the physical location of the failure site. An SCR (Silicon Controlled Rectifier) device is used as an example.


The use of failure analysis to confirm the physical location of a failure site in a device damaged by ESD stress testing is well established [1 ]. Fifteen years ago the Transmission Line Pulse (TLP) testing technique was introduced by Maloney and Khurana[2, 3 ] as a new electrical analysis tool. The tool employed a rectangular pulse with energy similar to that utilized in HBM testing to provide an equivalent energy threat to the ESD protection structures of ICs.


TLP is a very short pulse measurement system which has evolved into a very useful tool to provide both electrical operating analysis, and electrical damage signatures (EDS). By using a flat top pulse, both the current through the device under test (DUT) and the voltage across the DUT can be accurately measured to provide its Current-Voltage (I-V) characteristics.


During this same time, we saw the sporadic use of failure analysis to confirm the physical location of the failure sites due to TLP testing [4-7 ]. HBM testers were built to simulate real life HBM in qualifying ICs to specified immunity levels [8, 9 ].


Initially, HBM stress testing was used for analysis of ESD designs to determine if they met the desired level of immunity. As TLP became available to more IC manufacturers, it quickly replaced HBM for design work.


Home made TLP test equipment systems has been used for many years [2, 3 10 ] but undefined measurement errors required considerable expertise to interpret the data from each different system.


However, it was the only method that could provide the dynamic electrical characteristics of each ESD protection design at high pulse currents. As ESD designers provided data showing fairly good relationships between TLP and HBM testing, it became more widely used and its test data became more accepted as an effective design analysis tool.


With the use of Failure Analysis tools, they were able to show that TLP can correlate to HBM peak current amplitude failures and also to the failure sites located.


This correlation has been remarkable because the HBM ESD event uses a double exponential and the TLP ESD pulse uses a square or rectangular pulse.


HBM pulses with an exponential decay (1/e) time of 150 nsec should theoretically require a rectangular pulse of 75 nsec to provide an equivalent energy at the same peak currents [ 10 ]. Traditional HBM ESD testing for qualification [ 8 ] requires the use of a discharge circuit of a 1500 ohm resistor and 100 pF capacitor connected in series. The resulting stress pulse is a double decaying exponential waveform with most standards specifying a rise time of 2-10 nsec.


ESD designers have been using TLP systems with rectangular pulse widths of 75-200 nsec with unspecified rise times that have probably ranged between 1 nsec and 40 nsec. When attempting to compare failure from TLP pulses to HBM pulses, the rise times of both systems must be considered in


addition to the pulse widths. The rise time of either threat pulse however, can cause significant differences in device failures because of dV/dt effects in the layout and arrangement of components in the ESD protection circuit.


Most designers however, fail to provide evidence of physical failures for both types of testing in the same paper [ 11-17 ]. Those who do, have not addressed the critically relevant issue of risetime of both the TLP and HBM pulse [ 18-20 ]. This is probably because of the difficulty of controlling this parameter. Those who do consider the rise time do not provide any physical (FA) pictures [ 21-26 ].


Correlation between the rectangular TLP pulse and the double exponential HBM test pulse can be remarkably close if the test pulse risetimes are comparable [27]. The ESDA standard risetime specification for the HBM test pulse has been 2 to 10 ns for many years, but most HBM testers built for testing 256 pins or more have a 9-10 ns risetime pulse [28].


HBM testers can only provide simple go/no-go test data, but the simplest TLP systems can provide Current-Voltage (I-V) data of ESD protection circuits and can be displayed on the tester or plotted on the computer screen with a software plotting program.


This is a significant improvement for ESD design because it provides an analysis tool unavailable with HBM. Moreover, TLP also has the ability to measure and display the DC leakage current evolution of the device under test, that is, leakage measurement after each pulse instead of at the beginning of the stress test and at the end of the stress test. Adding a DC leakage current measurement of the DUT after each test pulse allows additional insight into minute changes of damage to the protection or core circuits,which is unavailable without this measurement. The DC leakage current data combined with the I-V data provides electrical indications of where damage begins, and how rapidly it can evolve from soft to hard failures. We define this I-V and leakage data on a device as the electrical damage signature (EDS).


TLP Basics


TLP is defined as the application of a narrow(75-200 nsec) rectangular pulse, usually generated by discharging a transmission line, to an ESD protection structure connected to the pins of an IC [23]. When the DUT voltage and current are measured it becomes a Pulse Curve Tracer [29] that has an energy content similar to that used in HBM ESD stress testing. With an ordinary curve tracer, the much higher amounts of energy associated with the longer pulse widths (usecs) dissipated in the ESD protection circuit, limits the current trace to a small fraction of what the same circuit is capable of with shorter ESD pulses. TLP Pulse stress testing to failure levels


Figure 9 The Load line of the TLP 50 at the maximum test pulse amplitude and at half of the maximum pulse amplitude.


The Device Negative Resistance


The 50 ohm operating load line for the TLP-50 identifies how the system operates in the negative resistance portion of a device with snap-back. When the test pulse amplitude is in the negative resistance region of a DUT, it can only plot out the actual I-V data if the absolute value of the negative resistance portion of the DUT is lower than the source impedance of the TLP. In the case shown in Figure 10, the slope of the TLP system load line is lower [50 ohms] than that of the DUT negative resistance line [ 125 ohms].


The TLP will be able to accurately identify the peak voltage immediately before snap-back (trigger voltage,Vt1); but when it increases above the snap-back point(at the far right in figure 10), it will immediately snap to a current and voltage on the positive resistance portion above the holding current. [ 33 ]. The details are covered in reference [33].


Figure 10 The TLP 50 Load line crossing the I-V plot of a typical DUT.


Stress Testing ESD Structures


It is important to distinguish between single element ESD structure stress testing and full IC (chip) stress testing. Based on the data in the literature, most TLP stress testing is used for single element stress testing during design and HBM stress testing is used for IC qualification testing [ 8 ]. However HBM and TLP correlation is necessary to extrapolate the TLP ESD results to full chip HBM stress testing. TLP stress testing was probably never intended as a direct replacement of HBM; however its simplicity and accuracy is leading toward its use as a calibrated and more universal and quantifiable reference. The HBM stress testing is relatively good because it represents a go/no-go stress test (pass or fail), but it provides very limited data. On the other hand, TLP stress testing of single structure elements gives the detailed data that is needed by the designer. Whereas TLP can be regarded as an engineering tool, the HBM stress test is a qualification tool which provides levels of threshold failures, that is, classes like 1, 2, 3 etc which are related to the increase in voltage failure levels.


Stress testing single structures (diodes, resistors,capacitors, transistors, metal stripes etc) will provide direct insight into the single protection structures.


This is done either on a wafer or packaged as test chips or test devices before qualification. At qualification , the fully packaged IC (ESD structure +core) is stressed tested. The electrical I-V characteristics may be somewhat different but the physical failure location is the same – inside the protect structure.


The most common way to stress test the single protection structures is to use wafers level stress testing. For the diode, there is junction failure which is localized for the reverse breakdown and spread nicely along entire width of the structure for the forward breakdown. Three types of failures occur for a transistor: the failure at the gate-drain junction(avalanching junction); the second failure type is the failure at silicide block edge in the drain [ 36 ]; the third is the gate oxide failure which has been reported by H Gieser [ 37 ].


What Is Stress Tested


In general, for the MOS devices, the drain (collector)is stress tested while the gate , the source (emitter)and the substrate are tied to ground. This is an example of a single element structure.


Figure 11 Schematic showing the protection structure is stress tested.


The wafer level can be used to test a single element structure or a combination of several structures.


Figure 12 shows the path of the current through the protection structure and the resulting I-V characteristic curve is on the right (pin 1 to Vss).


Figure 12 The protection structure on a wafer with


the first protected core element.


The packaged test chip is a packaged single structure or several structures for design development testing.


Each structure (resistor, diode or transistor etc) on the test chip has its own set of contact pads, bond wires to a lead frame and pins that can be contacted for testing. This figure 13 shows the resulting I-V curve for each structure.


Figure 13 The layout of typical elements on a test


chip for testing individual components.


The fully packaged IC is a combination of one or more of the single protection structures plus the core all connected by the usual metal stripes and interconnects of various widths. This figure 14 shows the different current paths and the interactions.


In general, the I-V characteristic curve is the same with some variations due to interactions with the other elements on the IC.


Packaged IC


Figure 14 The layout of the fully packaged IC(protection + core).


Basic I-V and


Leakage Evolution Plots


The following three figures represent the characteristic responses from a typical nMOS device.


There are two curves. In figure 15, the plot with the dots represent the I-V characteristic curve using the bottom x-axis (voltage) and the vertical y-axis(device current). The second plot with the crosses is a leakage evolution plot. After the collection of each IV data point, a simple DC leakage measurement is done on the device under test. This DC leakage value(top x-axis) is obtained for a specified DC bias (e.g Vdd+10%) and is then plotted as a function of the stress parameter, the TLP pulse current ( y-axis). In this figure, the structure shows no sign of a problem based on the I-V curve. However, the leakage evolution continues to change from pico amps to nano amps which is three orders of magnitude.


Something has changed in the device and it is safe to say that the structure is damaged. Such electrical signatures are usually termed soft failures.


Figure 15 Soft Failure from TLP I-V plot.


In the figure 16, the I-V plot (dots) indicates an It2 point at 2.2 amps. The figure also shows that the leakage changes from 10E-10 amps to 10E-6 amps which is 4 orders of magnitude. This electrical data indicates a failure which appears to be catastrophic.


Figure 16 Hard Failure plot showing


For figure 17 below, a soft failure mechanism at 4.0 amps (vertical scale) appears before the hard failure at 8.6 amps. The leakage evolution allows the analyst to stop the stress at the soft failure point to perform physical failure analysis. This will allow identification of the physical location of the start (weakest point) to the failure if multiple failed locations are possible/expected.


Figure 17 Soft failure followed by a hard Failure


Stress Testing the SCR Structure


We stressed several SCRs (silicon controlled rectifiers) type structures (figure 18). We made the measurements using a constant impedance TLP system, which we defined earlier as TLP-50 (figure 1). The basic SCR is a two terminal device made up of two transistors (G2 is pnp and G1 is npn), and the on-resistance typically ranges from 1-3 ohms. This is a low powered dissipating device so it is generally regarded as a good device for ESD protection. The designated anode pins (22 and 23), were each stress tested relative to the ground pin which is the Cathode in the structure.


Figure 18 The schematic and I-V


for a typical SCR structure.


The I-V characteristic of an SCR type structure (also called pnpn type structure or thyristor) is shown in figure 19 below. The I-V curve (dots) shows a trigger voltage(Vt1) of 6.4 volts, the typical snap-back region and a constant leakage evolution (vertical line-x’s) of approximately 2.5 nanoamperes (2E10-5amps), the top horizontal scale. At approximately 3 amps (vertical yaxis scale), the structure appears to fail catastrophically with a leakage change of at least three orders of magnitude (10E-9  10E-6). The figure 19 I-V curve shows that this corresponded to the Vt2 of about 7.1 volts and a corresponding It2 of 3amps. For both the HBM and the TLP Step stressing, there was no leakage change until after catastrophic failure point at 3.0 amps.


The snap-back or holding voltage, Vh (extrapolation of snap-back/resistance line) is approximately 1.60 volts and the on resistance is approximately 1.46 ohms.


Figure 19 The I-V characteristic curve.


and leakage evolution for the SCR.


These SCRs, which are single element pnpn transistor structures, were electrically tested using the Curve Tracer (CTR) and were found to exhibit the short-type electrical failures. Both anode designated pins (22 and 23) were tested to the designated ground pin- the cathode. After decapsulation and deprocessing, the physical failures could be seen as pits and deep“cuts” in the structure. The figure 20 shows the positive anode on the left side and the negative cathode anode on the right side of the figure.


For pin 23, the TLP low magnification 5KX SEM picture (figure 20 ) shows soft-failure sites (anode area) and the catastrophic or hard failure across the structure (anode to cathode).


Figure 20 SEM photo of the TLP failure of the SCR protection structure for the anode pin 23.


The Figure 21 below shows the high magnification TLP failure from figure 20. The catastrophic failures across the structure from the anode to the cathode is quite evident. These 0.18um CMOS test structures failed at 3.6 KV for the HBM stress testing and 2.3 amps for TLP stress testing. The ratio (3.6/2.3) is 1.6 and is termed the correlation factor. The possible explanation for the multiple damage sites in the TLP pictures is that the high leakage started before the It2 point is reached, where the catastrophic failure frequently occurs.


Figure 21 Higher magnification of the SEM photo of the TLP failure for pin 23 shown in figure 20.


For the same pin 23, the 14Kx magnification HBM picture below (figure 22 ) shows a much more severe and localized catastrophic failure but the failure location for this TLP failure is generally in the same anode area as the TLP failure site (figures 20 and 21).


Figure 22 SEM photo of the HBM failure of the SCR protection structure for the same anode pin 23.


For pin 22, the low magnification HBM picture below (figure 23 ) also shows severe/catastrophic failure and the failure location is in the same anode area as the TLP and HBM failure sites for pin 23.


The second (figure 24 ) and third pictures (figure 25)show the higher magnifications for pin 22. The pictures show “pits” and “cuts” not only in the anode area but across the structure from anode (left) to cathode (right). These 0.18μm CMOS test structures failed at 4.2 KV for the HBM stress testing and 2.75 amps for TLP stress testing. The ratio (4.2/2.75)provides a correlation factor of 1.5, which is similar to that (1.6) obtained for pin 23. We have therefore shown that both the TLP and HBM data exhibit failure location and failure type/signature correlation.


Figure 23 Low magnification SEM photo of the HBM failure of the SCR protection structure for the anode pin 22.


Figure 24 High magnification SEM photo of the


HBM failure of the SCR shown in figure 23 for pin 22.


Figure 25 High magnification SEM photo of the


HBM failure of the SCR shown


in figure 24 for pin 22.


This paper describes an improved measurement technique to demonstrate the ability to correlate electrical failure signatures with the physical failure locations. This improved transmission line pulse(TLP) testing technique was used to show that the electrical failure signature and the physical location for an SCR structure correlated with that of HBM ESD stress testing. The paper demonstrated that the new techniques accurately tracks the leakage current evolution. This leads to better identification of where ESD stress testing should stop and failure analysis begin. Besides the traditional current and voltage measurements at the DUT, this new TLP testing technique included a correction for improved accuracy of the I-V characteristics using a simple short and open for the calibration. The pulse width and rise times of the TLP was chosen to provide the same current amplitude damage level (electrical) as is found in the Human Body Model ESD stress testing.


A one to one correlation between the two methods was established which lead to correlation between the electrical damage and the physical location of the failure .


The authors would like to thank the following engineers and super techs for their support :Christian Russ for the many valuable technical discussions and Phil Jozwiak for the failure analysis data collecting.


1. L. G. Henry. “Differentiating between EOS and ESD Failures for ICs”. Microelectronic Failure Analysis Desk Reference, 4th Edition, pp421-436.


ASM, Materials Park, Ohio, (1999).


2. T. Maloney and N. Khurana, "Transmission Line Pulsing Techniques for Circuit Modeling of ESD Phenomena" EOS/ESD Symposium Proceedings, EOS-7. 1985 pp. 49-54.


3. N. Khurana, T. Maloney and W. Yeh. “ESD on CHMOS Devices – Equivalent Circuits, Physical Models and Failure mechanisms…1985 IEEE IRPS, p212.


4. G. Notermans "On the Use of N Well Resistors for Uniform Triggering of ESD Protection Elements", EOS/ESD Symposium, EOS-19,1997, p222.


5. S. Kiefer, R. Milburn and K. Rackley: “EOS induced polysilicon migration in VLSI Gate Arrays”. EOS/ESD Symposium, EOS-15. 1993,p123-127.


6. W.A. Andersen and D.B. Krakauer. “ESD Protection for Mixed –Voltage I/O Using nMOS Transistors Stacked in a Cascade configuration”.


EOS/ESD Symposium, EOS-20. 1998, p54-62.


7. G. Notermans, P. de Jong and Fred Kuper.


“Pitfalls when correlating TLP, HBM and MM testing”. EOS/ESD Symposium, EOS-20, 1998,p170- 176.


8. ESD Association Standard for ESD Sensitivity Testing (Human Body Model).


ANSI/EOS/ESD-S5.1-1999.


9. K. Verhaege, P. Roussel, G. Groeseneken, H. E.


Maes, H. Gieser, C. Russ, P.Egger, X.


Guggenemos and F.G. Kuper. “Analysis of HBM Testers and Specifications Using A 4th Order Lumped Element Model”. EOS/ESD Symposium, EOS-15. 1993, p129- 137.


10. S. G. Beebe. Ph.D Thesis, “Characterization,Modeling, and Design of ESD Protection Circuits”. 1994. Tech.Report No.ICL94-038,Stanford Univ, Stanford, CA.


11. 11. A. Amerasekera, L. van Roozendaal, J.


Abderhalden, J. Bruines, L. Sevat. “An Analysis of Low Voltage ESD Damage in Advanced CMOS Processes”. EOS/ESD Symposium. EOS–12. 1990, p143-150.


12. J.C. Smith. “A Substrate Triggered Lateral Bipolar Circuit for High Voltage Tolerant ESD Protection Applications”. EOS/ESD Symposium. EOS–20. 1998, p 63-171.


13. H.U. Schroder, G. van Stenwijk and G.


Noterman. “High Voltage resistant ESD protection circuitry for 0.5um CMOS OTP/EPROM programming pin”. EOS/ESD Symposium. EOS–20. 1998, p 96-103.


14. D. Krakauer and K. Mistry. “ESD Protection in a 3.3V Sub-Micron Silicided CMOS Technology”. EOS/ESD Symposium. EOS–14.


1992, p 250-257.


15. N. K. Clark. “ Melt Filaments in n+pn+ Lateral Bipolar ESD Protection Devices”. EOS/ESD Symposium. EOS–17. 1995, p295-303.


16. J. Z. Chen, A. Amerasekera and C. Duvvury. “Design Methodology for Optimizing Gate Driven ESD Protection Circuits in Submicron CMOS Processes.” EOS/ESD Symposium.


EOS–19. 1997, p230- 239.


17. J. C. Smith. “An Anti-Snapback Circuit Technique for Inhibiting Parasitic Bipolar Conduction During EOS/ESD Events”. EOS/ESD Symposium. EOS–


21. 1999, p 62-69.


18. A. Bridgewood and Y. Fu. “A Comparison of Threshold Damage Processses in Thick Field Oxide Protection Devices following Square Pulse and Human Body Model Injection”. EOS/ESD Symposium, EOS-10, 1988 page 129.


19. W. Stadler , X. Guggenmos, P. Egger, H. Gieser, C.


Musshoff. “Does The ESD-failure Current Obtained by Transmission Line Pulsing always correlate to Human Body Model tests?” EOS/ESD Symposium,EOS-19, 1997. Page 366-372.


20. K. Bock, B. Keppens, V. De Heyn, G. Groesenken,L.Y. Ching and A. Naem. “ Influence of Gate Length on ESD-Performance for Deep sub micron CMOS Technology”. EOS/ESD Symposium. EOS–


21. 1999, p 95-104.


21. H. Gossner, T. Muller-Lynch, K. Esmark and M.


Stecher. “Wide Range Control of the Sustaining Voltage of ESD Proptection Elements Realized in a Smart Power Technology”. EOS/ESD Symposium,EOS-21, 1999, p19-27.


22. H. Wolf, H. Gieser and W. Wilkening. “ Analyzing the Switching Behaviour of ESD- Protection Transistors by Very Fast Transmission Line Pulsing”.


EOS/ESD Symposium, EOS-21, 1999, p28- 37.


23. K. P. Cheung. “Plasma-Charging Damage and ESD help each other”. EOS/ESD Symposium, EOS-21,1999, p38 – 42.


24. M. Mergens, W. Wilkengang, S. Mettler, H. Wolf,A, Stricker and W. Fichtner. “ Analysis and Compact Modeling of Lateral DMOS Power Devices Under ESD Stress Conditions”. EOS/ESD Symposium, EOS–21, 1999, page 1-10.


25. C. Russ, K. Bock, M. Rasras, I. DeWolf. G.


Groeseneken, H.E. Maes, "Non-Uniform Triggernig of ggNMOSt Investigated by Combined Emision Microscopy and Transmission Line Pulsing",EOS/ESD symposium, EOS-20, 1998, pp177-186.


26. Richier 1997 EOS 19 1997 EMMI only. C.


Richier, N. Maene, G. Mabboux and R. Bellens. “Study of ESD behaviour of different clamp configurations in a 0.35 um CMOS technology”.


EOS/ESD Symposium, EOS-19, 1997, page 240-245.


27. Barth Electronics TLP Application note #3. “TLP to HBM Rise Time Correlation, 1999, Publisher, B.E.


Inc, Nevada. www.barthelectronics.com.


28. Leo .G. Henry. Disclosures to the ESDA HBM Working Group (WG–5.2) in 1998 and 1999.


“Comparisons between the ESDA and the JEDEC HBM standards”.


29. J. Barth, K. Verhaege, Leo G. Henry and John Richner. “TLP Calibrations, Correlation, Standards and New Techniques”. Paper accepted by the EOS/ESD Symposium for presentation at the 2000 EOS-22 to be held in Anaheim, CA.


30. H. Ishizuka, K. Okuyama and K, Kubota. “Photo Emission Study of ESD Protection Devices Under Second Breakdown Conditions”. The 32nd Annual IRPS, 1994, p286-291.


31. Leo G. Henry, and J.H Mazur. Basic Physics in Color-Coded EOS Metallization FailuresDifferentiating between EOS and ESD”. The 24th Annual ISTFA, 1998, page 143-150.


32 Leo G. Henry, I. Morgan, M. Merhanpour, T.


Raymond. “ EOS and ESD Laboratory Simulation and Signature Analysis of a CMOS Programmable Logic Product”. The 20th Annual ISTFA, 1994,page117-126 .


33 Barth Electronics TLP Application note #2.


“Calibrating TLP Systems”, 1999, Publisher, B.E.


34. A. Amerasekera and C. Duvvury. ESD in Silicon Integrated Circuits. Publ. John Wiley and Sons,


1995.


35. S. Dabral and T.J. Maloney. Basic ESD and I/O Design. Publ. John Wiley and Sons, 1998.


36. C. Russ, K Verhaege, J. Roussel, G. Groeseneken,and H.E. Maes. "Compact Model for the groundedgate nMOS transistor behavior under CDM ESD stress", IEEE Transactions on Electron Devices, Vol.


44-11, 1997, pp 1972-1980. And EOS/ESD Symposium, EOS-18, 1996, page 302-315.


37. H. Gieser. “Very-Fast Transmission Line Pulsing of Integrated Structures and the charged Device Model”.


EOS/ESD Symposium, EOS-18, 1996, page 85-94.


p 215-221


DOI: 10.1361/cp2000istfa215


Failure Analysis of CDM ESD Damage in a GaAs RFIC


Amy Poe, Steve Brockett, and Tony Rubalcava


TriQuint Semiconductor, Inc., Hillsboro, OR, USA


The intent of this work is to demonstrate the importance of charged device model (CDM) ESD testing and characterization by presenting a case study of a situation in which CDM testing proved invaluable in establishing the reliability of a GaAs radio frequency integrated circuit (RFIC). The problem originated when a sample of passing devices was retested to the final production test. Nine of the 200 sampled devices failed the retest, thus placing the reliability of all of the devices in question. The subsequent failure analysis indicated that the devices failed due to a short on one of two capacitors,bringing into question the reliability of the dielectric.


Previous ESD characterization of the part had shown that a certain resistor was likely to fail at thresholds well below the level at which any capacitors were damaged. This paper will discuss the failure analysis techniques which were used and the testing performed to verify the failures were actually due to ESD, and not caused by weak capacitors.


There are three industry standard models for ESD:Human Body Model (HBM), Machine Model (MM)and Charged Device Model (CDM). Schematics of each of these models can be seen in Figure 1. 1,2,3 HBM is the oldest and most widely recognized ESD model. This model was developed when most ESD damage was the result of people touching parts without proper grounding. The actual capacitance and impedance of the human body varies widely so a somewhat arbitrary set of values was chosen to facilitate comparative testing (100pF and 1.5Kohms).


This model is still applicable whenever devices are manually handled and should be performed on all new device designs. This is also the most widely published and requested ESD data. Devices damaged by HBM ESD are generally found to have thermall damaged junctions, melted metal lines, or other similar damage caused by high peak current and a


Human Body Model


Machine Model Charged Device Model


JESD22-A1141


JESD22-A1152 JESD22-C1013


Peak Current < 0.75A Peak Current < 8A Peak Current 5-15Ampsτc = 150nS


τc < 5nS


τc < 1nS


Voltage Source


DUT


Source


1500 Ohms


10 0 pF


20 0 pF


C 1 Ohm


Figure 1 Schematics of ESD models.


large amount of charge dissipated over the period of several hundred nanoseconds. The JEDEC standard JESD22-A114-B classifies devices according to the following failure thresholds:


Class 0: < 250 V


Class 1A: 250 V to 500V


Class 1B: 500 V to 1000V


Class 1C: 1000 V to 2000V


Class 2: 2000 V to 4000V


Class 3A: 4000 V to 8000V


Class 3B: ≥ 8000V.


MM is an older model primarily used in Japan and Europe. Originally developed as a “worst-case”HBM ESD model, machine model accurately replicated the new failure modes caused by automated pick and place machines used for assembling circuit boards. The model simulates a machine with moderately high capacitance (200pf)and very low impedance discharging through a device, and can create significant damage at relatively low voltages. The JEDEC standard JESD22-A115-A classifies devices according to the following failure thresholds:


Class A: < 200 V


Class B: 200 V to 400 V


Class C: ≥ 400 V.


CDM is the newest ESD model with industry work starting about 15 to 20 years ago. This model best reflects real world ESD damage that occurs in small,plastic-packaged devices. As a packaged device slides on a surface, the device will accumulate charge through triboelectric action between the plastic body and the contacted surface. It is important to keep in mind the device picks up charge, which results in a potential. This is different from applying a known potential that results in an acquired charge. If the device is acquiring a triboelectric charge of a given value, the resulting potential is dependent on the bulk capacitance of the device. Therefore, with smaller devices, the potential can be surprisingly high6.


However, when simulating a CDM event, the device is charged to a fixed potential and discharged3. This is why some of the fail voltages seem so much higher than the equivalent HBM fail voltages. The JEDEC standard JESD22-C101-A classifies devices according to the following failure thresholds3:


Class I: < 200 V


Class II: 200 V to 500 V


Class III: 500 V to 1000 V


Class IV: ≥ 1000 V.


The popularity of CDM testing is increasing as more companies realize the importance of protecting circuits against damage due to CDM ESD. The JEDEC committee JC14.3 is in the process of


revising the JEDEC Stress Driven Qualification Spec(JESD-47) to require CDM testing over MM.


After determining that the parts failed the production retest, the first step was to do DC testing of each pin to check for shorted or opened paths. This DC analysis revealed a decrease in the resistance in either the positive or negative direction. This can be seen as a bend in the curve trace in Photo 1. The most direct path from the RF input to ground is through the resistor, R1 (see Figure 2). If either capacitor C1 or C2 is shorted, there is another path to ground through a FET gate diode, F1 or F2. If C1 is shorted, there will be a decrease in the negative resistance (negative bend), whereas if C2 is shorted there will be a decrease in the positive resistance (positive bend)See Photo 1. Out of the nine parts which failed, 8 had the signature of a C1 short, while only 1 had the signature of a C2 short.


Photo 1 Curve trace of RF Input to ground:A) Good part,


B) Part with C1 short


C) Part with C2 short.


Figure 2 Circuit schematic.


After decapping the parts, the Temptronic liquid crystal LC2 ZZ04050, with a transition temperature of 47.5C, was used to determine the defect location on the parts with a negative bend in the curve trace(signature of a C1 short). Because the shortest path to ground was through the resistor R1, the heat from the resistor made fault isolation difficult. Thus, to locate the hot spot due to the short, it was necessary to remove R1 from the circuit being probed. This was accomplished by applying +2.5V to the RF input on the parts with a negative bend in the curve trace.


This voltage was sufficient to open the input resistor(Photo 2).


Photo 2 Open resistor, R1. Mag: 4000 X After removing R1 from the circuit, liquid crystal analysis indicated that there were hot spots in C1 on all parts probed. This proved that the capacitor was shorted. On one device there was also a visible spot on capacitor C1, at the location of the hot spot(Photo 3). This spot looked similar to spots seen on capacitors on other parts, which were known to have been blown by ESD (Photo 4).


In order to determine what the nature of the spot was a particle, a hole or a bump, it was necessary to


deprocess down to the top plate of the capacitor.


However, it was known from previous experience that a plasma etch of the dielectric would leave the surface covered with an RIE grass8, so a wet etch method was developed which left only a thin, clean layer of silicon nitride on top of the capacitor. Since the capacitor in question was covered by successive dielectric layers of silicon nitride and a low-k dielectric (see Figure 3b), it was possible to use the particular wet etch characteristics of the low-k dielectric, along with a laser, to remove the layers.


Photo 3 Optical photo of spot on capacitor of failing device. Circle indicates hot spot identified with liquid crystal analysis.


Photo 4 Optical photo of known ESD on a capacitor on a sample device. This is the


same device as in photos 5, 6, 7 and 8.


The laser was used to cut a square trench around the capacitor on both a failing device and a device with a known ESD zap. This trench was cut deep enough to allow the etchant to reach the lowest layer of the lowk dielectric (Figure 3a). Photos 5 and 6 show optical and SEM photos respectively after the laser cuts were made on the device with the known ESD. After cutting the trench, a sulfuric acid etch was used to


preferentially etch the low-k dielectric. A quick ultrasonic clean lifted away the nitride layers which were now detached, allowing a view of the top plate through the last thin layer of nitride (Figure 3b and


Photos 7 and 8). A protrusion was visible in the same location as the previously identified spot. This bump, shown in photos 9 and 10, is very similar to the bump seen on the capacitor on the device which was known to have been blown by ESD (photo 8).


Figure 3a Trench cut around capacitor C1.


Figure 3b View of capacitor C1 after the etch and ultrasonic clean. The layers of silicon nitride and low-k dielectric are clearly visible in the sidewalls.


Photo 5 Optical photo of sample device after laser cuts were made around the capacitor. Arrow indicates known ESD spot. This is the same device as in photos 4, 6, 7 and 8.


Photo 6 SEM photo of sample device after laser cuts were made around the capacitor. Arrow indicates location of known ESD spot. This is the same device as in photos 4, 5, 7 and 8.


Photo 7 Optical photo of sample device after deprocessing . Arrow indicates known ESD spot.


This is the same device as in photos 4, 5, 6 and 8.


Photo 8 Protrusion on capacitor from known ESD event. This is the same device as in photos 4, 5, 6 and 7.


Photo 9 Optical photo of spot on failing device after deprocessing.


Photo 10 SEM photo of protrusion on capacitor of failing device.


ESD Testing and Analysis


Because the protrusion looked remarkably similar to damage we had seen which we knew was ESDinduced, an experiment was devised to see if the failure mechanism could be reproduced. Since previous testing with Human Body Model (HBM)and Machine Model (MM) had always caused the resistor to blow open rather than shorting the capacitor, the experiment was designed to include HBM, MM and also CDM simulations. Forty-five parts were pulled for testing – fifteen for each ESD model. The result of the testing was that HBM and MM consistently yielded an open or a high resistance on the RF input, while CDM yielded a positive or negative bend in the curve trace just like those of the failures in question (see Table 1). An internal visual inspection verified that the HBM and MM testing had overstressed the resistor, thus causing the high resistance. The failures generated by the CDM simulation were analyzed using liquid crystal and found to have the same shorted capacitors as seen in the original failures. These devices were then deprocessed using the same technique described above, and protrusions similar to the original failures were found. One of these spots can be seen in photos 11 and 12.


Photo 11 SEM photo of protrusion in C1 on device zapped with CDM ESD.


Photo 12 Optical photo of protrusion in C1


on device zapped with CDM ESD.


It is important to note that from the HBM and MM values listed in Table 1, this device would be classified as a class 0 and class A device according to the JEDEC HBM and MM standards respectively.


These are the lowest classifications for each of those standards. However, none of the failures seen on the test floor failed due to an overstressed resistor, which is the signature of an HBM or MM event. The values in Table 1 indicate that this device would be classified as at least a class II device according to the JEDEC CDM standard. Nevertheless, even though the device has a higher ESD classification for CDM than for either the HBM or MM models, the devices on the test floor actually failed due to a shorted capacitor, the same failure mode found with CDM ESD testing. This proves the idea that the CDM ESD model is more representative of the ESD which occurs in this type of device on the modern test floor,and underlines the importance of testing and characterizing the CDM ESD performance of a device, along with the HBM and MM testing and characterization.


Table 1 Results of ESD Testing.


Part #


HBM


Fail voltage


Fail Mechanism


1 +250 V open resistor 2 +250 V open resistor 3 +250 V open resistor 4 +250 V open resistor 5 +250 V open resistor 6 -250 V open resistor 7 -250 V open resistor 8 -250 V open resistor 9 -250 V open resistor 10 -250 V open resistor 11 +/- 250 V open resistor 12 +/- 250 V open resistor 13 +/- 250 V open resistor 14 +/- 250 V open resistor 15 +/- 250 V open resistor


MM


16 +25 V high resistance 17 +25 V high resistance 18 +25 V high resistance 19 +25 V high resistance 20 +25 V high resistance 21 -20 V open resistor 22 -15 V high resistance 23 -20 V high resistance 24 -20 V high resistance 25 -15V open resistor 26 +/- 20 V open resistor 27 +/- 25 V open resistor 28 +/- 20 V open resistor 29 +/- 25 V open resistor 30 +/- 20 V open resistor


CDM


31 +850 V C2 short 32 +1000 V C2 short 33 +1050 V C2 short 34 +450 V C1 short 35 +850V C2 short 36 -650 V C1 short 37 -450 V C1 short 38 -650 V C1 short 39 -700 V C1 short 40 -650 V C1 short 41 +/- 1050 V C1 short 42 +/- 1050 V C1 short 43 +/- 1000 V C2 short 44 +/- 1000 V C2 short 45 +/- 1000 V C2 short


After parts were found failing at retest on the test floor, failure analysis determined that the failures were due to a shorted capacitor. CDM ESD simulations were able to replicate the failure mode


and were successful in proving that the devices were failing due to ESD. HBM and MM simulations were also performed, but although the devices failed at relatively low threshold for HBM and MM, these models did not duplicate the failures which were found on the test floor. The importance of CDM


ESD testing is thus reiterated, as a major investigation into the integrity and reliability of the parts was averted by proving the failures were caused by CDM ESD events.


1. EIA/JEDEC Standard, Electrostatic Discharge(ESD) Sensitivity Testing Human Body Model(HBM). EIA/JESD22-A114-B, June 2000.


2. EIA/JEDEC Standard, Electrostatic Discharge(ESD) Sensitivity Testing Machine Model(MM). EIA/JESD22-A115-A, October 1997.


3. JEDEC Standard, Field-Induced Charge-Device Model Test Method for Electrostatic Discharge Withstand Thresholds of Microelectronic Components. JESD22-C101-A, June 2000.


4. V. Soorholtz, A. Bormann, R. Wheelus, N. Herr,and M Phillips, Conference Proceedings from the 17th International Symposium For Testing and Failure Analysis, 297-303, (1991).


5. The ESD Association, Part Five – Device Sensitivity and Testing from Compliance Engineering, September/October, 1998.


6. Steve Brockett, Internal Publication, TriQuint Semiconductor, 2300 NE Brookwood Pkwy,Hillsboro, OR 97124.


7. JEDEC committee JC14.3, Minutes of meeting


# 36, January 27-28, 2000.


8. A. Crockett and W. Vanderlin, Microelectronic Failure Analysis Desk Reference, 4th Edition,pp. 243-252, ASM, Materials Park, Ohio, (1999).


p 225-230


DOI: 10.1361/cp2000istfa225


A Focused Ion Beam Technique to Electrically Contact the Deep Trench Capacitor of a Single Active Memory Cell in the Sub 0.25μm Technology Regime.


Gunnar Zimmermann


Mark Johnston and Rolf Christ


White Oak Semiconductor, Sandston, U.S.A.


Focused ion beam (FIB) techniques are continuously improved to meet the demands of shrinking device dimensions and new technologies. We developed a simultaneous milling and deposition FIB technique to provide electrical contact to small buried targets in semiconductors. This method is applied to directly connect the deep trench (DT) capacitor of a DRAM single cell in deep submicron technology. By carefully adjusting the deposition parameters(scanned area < (0.3 μm)2, beam current < 20 pA) we are able to influence diameter, depth and Pt fill properties of the hole to meet the very restricted requirements for successful DT connection (hole diameter < 200 nm at DT level). Electrical measurements are performed on DRAM single cells after connecting buried plate (n-band), p-well,wordline, bitline and DT. The probe pads were Pt,deposited with ion beam assistance, on top of highly insulating SiOx, deposited with electron beam assistance by using a dualbeam FIB. The read and write conditions of an active memory cell are studied.


The presented method increases the capabilities to localize and characterize trench related failure mechanisms.


The characteristics of transfer gates (transistors) in an electrical circuit are important parameters to define the function and performance of semiconductor devices. Focused ion beam (FIB) techniques can be used to deposit probe pads and modify electrical circuits with the purpose to access source and drain of individual transistors for electrical probing [1,2].


However, shrinking dimensions and the increasing complexity of modern IC technologies are making this task more and more difficult to achieve.


Especially challenging is the electrical sensing of the transistor drain of a single memory cell in dynamic random access memory (DRAM) devices in deep trench (DT) technology. Modern DT technologies are using a buried strap design. Here, the capacitor which resides in the silicon substrate, is directly connected to the drain diffusion of the transistor. As a


consequence there is no access site above substrate level to extract the drain-side signal. Obviously this design and the small dimensions of the cell makes it a very difficult task to directly contact to the DT without destroying or unintentionally modifying the cell, rendering electrical measurements meaningless.


Existing techniques to electrically probe single memory cells in sub 0.35 μm DT technology are accessing only the transistor source, which is the bitline (BL) contact. After removing all upper metal layers including the BL, probe pads are deposited on top of the contacts of n- and p-well as well as the appropriate wordline (WL) and BL contacts. The technique has already been successfully applied to the failure analysis of DRAM single cells [3,4].


Although time-consuming, this method offers the advantage of being able to apply a large variety of test conditions (e.g. voltages and temperature, access and retention times) directly to the suspicious cell.


Failure modes and leakage paths can be studied in more detail and with little or no influence of neighboring cells as compared to the routinely used full functional testing of the product during manufacturing.


Many tests of the cell functions do not need a separate electrical connection to the transistor drain.


This applies of course to all leakage mechanisms related to the transistor source or the gate. But also capacitor-related failures, like node dielectric leakage can be studied in many cases without connecting the drain. It requires however to turn on the WL and extract the drain-side signal via the BL contact.


Therefore the signal from the capacitor is mixed with possible leakages from WL or p-well. To distinguish these leakage paths an additional drain contact is needed. Node-side gate-induced drain leakage(GIDL) or junction leakage of the buried strap to pwell diode can only be studied with a separate drain contact. Another application would be the direct measurement of the transistor parameters, especially the threshold voltage, which in turn could be beneficial for fine-tuning the transistor performance during process development.


This article describes a modified single cell probing technique for sub 0.35 μm DT technologies (buried strap design), where an additional electrical contact to the drain (the capacitor trench) is included. In the“Experimental” section the general layout, the initial sample preparation and the tool setup is illustrated.


The section “Results and Discussion” consists of two parts. The first part is dealing with the FIB-technique for successful trench connection. In the second part we discuss an example of electrical measurements on a fully connected single cell. The “Summary”concludes this article.


Samples were 0.2 and 0.19 μm technology 64M DRAM devices manufactured at WhiteOak Semiconductor. Pass devices as well as parts which failed electrical testing due to single cell failures were investigated. In this article electrical measurements on a pass device will be discussed. A schematic representation of a single memory cell in buried strap design is shown in figure 1.


deep


trench (DT)capacitor


BLcontact


P-well (PW)


N+(drain)


GOX


wordline(WL)


N+(source)


Si-oxide


bitline (BL)


N-well (NW)


passing wordline(pWL)


buried strap node dielectric


Figure 1 schematic representation of a DRAM cell in cross-section (not to scale). Areas containing SiOx are marked in grey. The black arrow is indicating the location of device modification for DT connection.


A typical single cell consisted of a deep trench capacitor accessed through an n-channel transfer gate, which was the WL. The data was written or read to the BL via the BL-contact. Source and drain of the transistor were n+-doped regions. The poly Sifill of the DT was directly connected to the drain diffusion at substrate level via a recess in the node dielectric (buried strap design). The cell resided in a p-well (PW). A deep n-doped region (n-well, NW)served as electrode for the trench capacitors and isolated the PW from the p--doped substrate. The WL consisted of a stack of gate oxide (GOX), polysilicon,tungsten-silicide and silicon-nitride. The WL was stitched in regular distances to an AlCu-metal line to reduce the line resistance. The passing wordline


(pWL), which was completely covering the area above the DT was accessing the neighboring row of cells. Note, that the neighboring cell itself is off the plane of cross-section and can not be represented in figure 1. A thick oxide (shallow trench isolation, STI)was separating the pWL from the deep trench. Silicon oxide layers served as dielectric isolation between WL and BL as well as between upper AlCu metallization levels. The technology as well as layout and basic functions of a DRAM single cell can be reviewed in detail elsewhere [4,5].


Before introducing the sample into the FIB chamber all layers above the BL contact were removed using standard delayering techniques involving reactive ion etching (RIE) and wet chemical steps. The contacts of BL, WL, PW and NW were then exposed at the surface. Probe pads were realized by using electron beam assisted SiOx deposition, ion milling and ion beam assisted Pt deposition, as described in detail elsewhere [6]. The BL contacts were the only remaining landmarks at the sample surface in the cell array area and could be used for the localization of specific cells based on the physical cell addresses.


The additional contact to the DT can be realized by accessing either the drain implant region or the polySi fill of the DT. We decided to take advantage of the cell design and to mill in two steps directly through the stack of SiOx, pWL and STI with a total thickness of about 1 μm into the DT, as indicated by the black arrow in figure 1. End point detection was less critical here because of the vertical structure of the DT, while it would have been very difficult to avoid shorting to the PW due to overmilling, when trying to contact the drain implant area. There was also a larger distance to the electrically active WL when milling into the DT instead of into the drain implant,which reduced the risk of unintentional shorting to the WL. Finally this method would allow to extract the DT signal via the stitch contact of the pWL,because the DT would be automatically shorted to the pWL after Pt fill of the hole. All five probe pads were then widely separated from each other and easy to access by probe needles. The contacts for WL and DT (pWL) were located at different stitch rows, the contacts for PW and NW could be accessed outside the cell array and the BL contact remained the only contact at the cell position. It has to be noted however, that all possible leakage paths from pWL through STI into the DT can no longer be studied when using this technique. For current technologies though, this failure mode has no importance for yield detraction and can be neglected.


A number of challenges had to be faced to realize a Pt plug into the DT. A correct alignment of the initial hole with respect to the DT was absolutely necessary.


The DT is covering an ellipsoidal area of only about 300 nm along the long axis and 225 nm along the short axis at substrate level. To precisely locate the


center of the DT under the pWL we used the dense pattern of BL contacts as landmarks, spaced at around 400 nm around the target.


Due to the small DT dimensions, the diameter of the opening should have been well below 200 nm.


Misalignments from the center of the DT of around 25 nm could then be allowed without risking to hit the node dielectric and to create shorts to PW or NW.


Equally important was to ensure a sufficient Pt filling of this narrow opening to reduce the electrical resistance of the plug. Successful shorting of the pWL was indicated by voltage contrast at the stitch contact of the pWL.


The FIB system used for DT connection and probe pad deposition was a FEI XL 830 dual beam system equipped with a gallium source ion column, an ultra high resolution immersion-lens type field emission scanning electron microscope and four gas injectors.


Secondary electron imaging was used when scanning with the electron as well as with the ion beam. Ptcyclopentadienyl and tetraethylortho-silane (TEOS)were used for platinum and oxide depositions,respectively. Standard ion beam conditions with beam currents of 4 - 150 pA were applied for Pt deposition and ion milling. For the deposition of highly insulating SiOx layers the use of the ion beam was avoided to prevent Ga implantation. Instead, the technique of electron-beam assisted TEOS deposition


[7] was applied using an electron beam of 5 keV with a beam current of 1 nA in the UHR mode. This technique was already proven to yield in very high quality insulating SiOx layers [6]. Iodine (I2) was used with the ion beam to clean the probe pads from Pt overspray to reduce parasitic leakage. The TEOS gas injector was aligned to the electron beam, whereas all other injectors were aligned to the ion beam. The distance between needles and sample surface was kept constant at about 100 μm. Chemical sources were operated at temperatures between 25 and 40oC as recommended by the vendor.


The memory cells were electrically tested using micromanipulators with T4-10 needles on a Suss PA200 probe station. Electrical signals were captured with a HP 4155B parameter analyzer. All needles were checked for continuity to the probe pads.


Results and Discussion Deep trench connection


To fulfill the demanding requirements for successful DT connection as defined in the previous chapter the following procedure was developed:


To navigate to the target cell only the electron beam was used in order to avoid any Ga implantation due to ion beam scanning. Then a (4x4) μm2 and 70-100 nm thick layer of TEOS was deposited using the electron beam on top of the target area. The purpose of this layer was to isolate all electrically active areas at the surface around the target and to help minimizing the use of the ion beam in subsequent cleaning steps for Pt overspray.


An approach of directly milling into the DT in one step and subsequently filling the hole using ionbeam-assisted deposition could not be successfully implemented due to poor reproducibility. The retrieved information from the small scanned area during milling (0.04 μm2) was insufficient for end point det ection. The hole formation was therefore only based on a predefined milling time. A homogeneous Pt fill from the bottom of the hole to the top was very often immediately blocked by Pt overgrowth at the top of the hole leaving a void with unpredictable electrical conductivity between DT and pWL. We therefore had to modify this procedure.


Instead of directly milling into the DT in one step, the hole formation was stopped after a predefined time at poly-Si level of the pWL. Then the Pt needle was introduced and a stable Pt precursor flow to the sample surface was established. By reducing the scanned area down to only (0.01) μm2 we observed,that not only Pt deposition, but also a substantial amount of milling took place, which depended on the ion beam density. This simultaneous milling and deposition mechanism resulted in the formation of a deep needle-like Pt plug into the DT with much improved reproducibility. It also provided – although usually forming a void in the center of the plug - an excellent Pt coverage from the edges of the hole. Pt plug depth, diameter and void formation were increasing with increasing beam current density. For our purpose a beam current of 4 pA gave the best results. In combination with a milling box size of(0.01) μm2, a 300 – 400 nm deep Pt plug with a diameter of typically less than 180 nm at substrate level was formed in 6 seconds of milling/deposition time.


SEM images of FIB cross-sections through a DRAM single cell after Pt plug formation are shown in figure 2 perpendicular (a) and parallel (b) to the pWL. Figure 2a can be compared to the schematic of figure 1. It reveals the importance of a needle-like Pt contact in order to have acceptable tolerances for misalignment. Figure 2b is showing the efficient shorting between DT and pWL via the Pt plug. Both images were taken before completion of the probe pad for the BL contact, which would have covered the whole sample surface shown in figure 2. Leakage between the Pt plug and the FIB pad of the BL contact was avoided by a Pt overspray cleaning step


and the electron beam assisted deposition of a SiOx layer on top of the Pt plug before realizing the pad for the BL.


Figure 2 SEM images of a cross-sectioned DRAM single cell perpendicular (a) and parallel (b) to the pWL after completion of the Pt plug into the DT.


To explain the simultaneous milling and deposition behavior we took into account the well-known dependence of growth rate vs. current density for ion beam assisted deposition from the gas phase(figure 3). This deposition efficiency curve combines the two concurrent processes of milling due to ion bombardment and deposition based on the interaction of the ion beam with a precursor at the surface. While deposition is dominant in the low range of current densities, the milling component becomes dominant for sufficiently high current densities (negative growth rate in figure 3). In figure 4 we assumed a simple gaussian current density profile for the ion beam and estimated the resulting net growth rate at a given location at the beam from the growth efficiency relation of figure 3. If the density in the beam center is sufficient for dominant milling, a hole will be milled in areas scanned by the beam center. But deposition will still occur in the areas covered by the beam tails due to the decreased beam density. When scanning the beam in a predefined region, the outer areas of this region will be mostly covered by the beam tails, explaining the dense Pt coverage at the edges of the hole, that we observed under various conditions. By increasing the beam density the milling component becomes more dominant in accordance to the experimental result of larger and deeper void formation under these conditions.


Deposition efficiency


-1.0-0.5


Current density (a.u.)


0.4 0.8 1.2 1.6


deposition


milling


Figure 3 Deposition efficiency for ion beam assisted


deposition from the gas phase.


Current density profile


0 1 2 3 4 5


Location (a.u.)


Figure 4 Assumed gaussian beam density profile of the ion beam.


Figure 5 shows first results of electrical measurements for a single memory cell in 0.2 μm technology after DT connection. The currents for BL(IBL, open squares), DT (IDT, filled squares), WL(IWL, open circles) and PW (IPW, filled circles) are shown for three different WL voltages VWL of 1.5, 3 and 4.5 V while ramping the BL voltage VBL between 0 and 2 V. The voltage of DT (VDT) and BP (VBP) was kept constant at 1 V and the voltage of the PW (VPW)was at –1V.


If VWL is at 1.5 V or below, the transfer gate is turned off and IWL is around 0 nA. IBL and IPW (on the negative scale) are slightly increasing by 8 nA, when increasing VBL from 0 to 2V. This small current is the leakage across the reversed biased diode between BL and PW below the BL contact. IPW and IDT show an additional bias independently of UBL of around 8 nA.


This is the current across the reversed biased buried strap diode at the transistor drain between DT and PW. Both diodes show a comparable leakage behavior and it can be concluded, that the buried strap diode was not affected by the ion beam manipulations to form the nearby Pt plug.


For UWL = 3V the gate starts to open and an increased current out of the DT into the BL can be detected for BL voltages below the DT voltage of 1V. IWL and IPW are not showing a dependence on the WL voltage up


to UWL = 3 V. At UWL = 4.5 V the n-channel below the gate is fully developed. For UBL below 1 V the current is flowing from the cell into the BL, which simulates the read procedure. Source and drain are switched for BL voltages above 1V and the current is flowing into the DT, comparable to the write condition of the cell.


At 1 V the potential at the BL is equal to the potential at the DT and the resulting current under the gate is


0. The current for the read condition is higher than for the write condition at comparable potential differences between DT and BL. This effect is also observed in operating DRAM cells (source-follower effect) and is caused by switching from an input to the output characteristic of the gate when increasing UBL over 1V.


-100-75-50-25


0 25 50 75 100


BL voltage (V)


UDT= 1V UBP= 1V UPW= -1V UWL=1.5V


UWL=3V


UWL=4.5V


2 0


Figure 5 Currents for BL (open squares),DT (filled squares), WL (open circles) and


PW (filled circles) in dependence of the


BL voltage (UBL) for three different


WL voltages (UWL) of 1.5, 3 and 4.5 V.


The IV-curves are qualitatively in good agreement with the expectations for the read- and writeconditions of an operating DRAM cell. However further improvements are needed to apply the technique also for the quantitative characterization of cell properties, e.g. the threshold voltage. The measured values for IBL and IDT are differing by some orders of magnitude from the expected values in the range of μA. We also expect the gate already to be turned on at a gate voltage of UWL=3V, which is not the case in figure 5.


Both effects of decreased transistor currents and an increase of the threshold voltage have been reported in the literature for ion beam irradiated MOS structures [8,9]. Ion beam exposure results in our study from the milling and Pt deposition steps, while navigation and oxide deposition was performed using the electron beam. Campbell et al [8] explain the shift in transistor parameters by sample charging. They reported that the parameter shift can be reduced by using electron flood gun neutralization during ion beam exposure and that an optimized annealing procedure can lead to a full recovery of parameter


shifts. Further investigations are planned to prove the validity of this concept for the current study and to evaluate if the proposed countermeasures are applicable to allow quantitative statements from electrical measurements after direct DT connection.


A FIB technique to directly access the deep trench(DT) capacitor of a DRAM single cell in deep submicron technology is presented. The method is creating a Pt-filled hole into the poly-Si fill of the DT, which connects the DT to the passing wordline of the cell. The very restricted requirements for successful DT connection (hole diameter < 200 nm at substrate level) were fulfilled by optimizing the beam density in the scanned area during Pt deposition. For a scanned area of only (0.1 μm)2 and a beam current of 4 pA a 300 – 400 nm deep hole with a diameter of around 180 nm at substrate level is milled. Platinum is deposited simultaneously from the edges of the hole during milling, providing a reliable electrical connection even for very small holes. The effect of simultaneous milling and deposition is explained by taking into account the deposition efficiency relation of the ion beam and by assuming a gaussian current density profile of the beam. For sufficiently high current densities in the center of the beam we can distinguish the two areas of dominant milling in the center of the beam, responsible for the hole formation and dominant deposition in areas covered by the beam tails, which leads to the Pt deposition around the center of the hole.


The probe pads for n-well (NW), p-well (PW),wordline (WL), passing wordline (DT) and bitline(BL) were Pt, deposited with ion beam assistance, on top of highly insulating SiOx, deposited with electron beam assistance by using a dualbeam FIB. Electrical measurements for the read and write conditions of a fully connected DRAM single cell in 0.2 μm technology were presented. The IV curves show the typical dependencies for the input and output characteristic of the gate and represent qualitatively the read and write conditions of the connected DRAM single cell. However, the absolute values for the currents and the threshold voltage are differing significantly from expected values, which is probably caused by sample charging effects due to ion beam exposure. Without appropriate countermeasures to reduce the sample charging and its effects, e.g. the use of an electron flood gun and an optimized sample annealing procedure, quantitative statements are difficult to be retrieved from electrical measurements using the described DT connection method.


Even without these improvements, the method can already be applied to the localization of trenchrelated failure mechanisms, like node-dielectric,


buried strap junction and gate-induced drain leakage,where the results can be compared to a similarly prepared pass device. The FIB technique of creating a small needle-like conductive plug can generally be applied for the connection of small buried targets in semiconductors.


Acknowledgement


The authors wish to acknowledge R. Chapman and J.


Vollrath of WhiteOak Semiconductor and H.


Schneider of Infineon Technologies for insightful discussions and their valuable contributions to this work.


1. K. Van Doorselaer, R. Young and N. Dawes,Proc. Int. Symp. Test and Failure Analysis, 27(1996)


2. K. Gamo, Nuclear instruments & methods in physics research, 1/4, 464ff (1997)


3. G. Benstetter, G. Bomberger, P. Coutu, R.


Danyew, R. Douse, Proc. Int. Symp. Test and Failure Analysis, 401 (1996)


4. L. Nesbit, J. Alsmeier, B. Chen, J. DeBrosse, P.


Fahey, M. Gall, J. Gambino, S. Gernhardt, H.


Ishiuchi, R. Kleinhenz, J. Mandelman, T. Mii,M. Morikado, A. Nitayama, S. Parke, H. Wong,G. Bronner, IEDM Digest of Techn. Papers,627ff (1993)


5. E. Adler, J. DeBrosse, S. Geissler, S. Holmes,M. Jaffe, J. Johnson, C. Koburger, J. Lasky, B.


Lloyd, G. Miles, J. Nakos, W. Noble, S.


Voldman, M. Armacost, R. Ferguson, J. Res.


Develop., 39 167-187 (1995)


6. G. Zimmermann and R. Chapman, Proc. Int.


Symp. Test and Failure Analysis, 311 (1999)


7. S. Lipp, L. Frey, C. Lehrer, B. Frank, E. Demm,S. Pauthner, H. Ryssel, J. Vac. Sci. Technol. B,14, 3920-3923 (1996)


8. A.N. Campbell, P. Tangyunyong, J.R. Jessing,C.E. Hembree, D.M. Fleetwood, S.E. Swanson,J.M. Soden, N. Antoniou, W.E. Vanderlinde,M.T. Abramo, Proc. Int. Symp. Test and Failure Analysis, 273 (1999)


9. J. Benbrik, G. Rolland, P. Perdu, B. Benteo, M.


Casari, R. Desplats, M. Labat, A. Touboul, Y.


Danto, Proc. Int. Symp. Test and Failure Analysis, 49 (1998)


p 231-234


DOI: 10.1361/cp2000istfa231


The Use of TMAH to Etch Silicon and Expose Metal Bridging Failures


Mark Morris, James Mohr, Esteban Ortiz, and Steven Englebretson


ON Semiconductor


Determination of metal bridging failures on plastic encapsulated devices is difficult due to the metal etching effects that occur while removing many of the plastic mold compounds. Typically, the acids used to remove the encapsulation are corrosive to the metals that are found within the device. Thus, decapsulation can result in removal of the failure mechanism.


Mechanical techniques are often not successful due to damage that results in destruction of the die and failure mechanism. This paper discusses a novel approach to these types of failures using a silicon etch and a backside evaluation.


The desirable characteristics of the technique would be to remove the silicon and leave typical device metals unaffected. It would also be preferable that the device passivation and oxides not be etched so that the failure location is not disturbed. The use of Tetramethylammonium Hydroxide (TMAH), was found to fit these prerequisites. The technique was tested on clip attached Schottky diodes that exhibited resistive shorting. The use of the TMAH technique was successful at exposing thin solder bridges that extruded over the edge of the die resulting in failure.


In a recent incidence, customer exposed Schottky diodes, in large surface mount packages, to excessive temperatures during a double wave solder process.


During subsequent power cycling the device would fail. Electrical characterization found devices exhibited intermittent anode to cathode shorting.


After chemically removing the mold compound on several samples, it was found that the devices recovered with no anomalies present. It was speculated that the failure mechanism was solder that had re-flowed and bridged the oxide gap between the anode and cathode at the edge of the die.


In order to verify the re-flowed solder theory, several devices were mechanically separated. This technique was developed based on a previous technique [1].


When this technique was attempted, the evidence of


the failure mechanism was lost due to the large amounts of stress of this mechanical process. It was obvious that the mechanical method, although possibly suitable for times when many samples are available, was not suitable for the typical failure analysis case in which there are a limited number of samples. A new technique was needed.


Technique definition


One possible solution to the problem would be to come in from the backside of the device and dissolve the silicon with minimal affect to the mold compound, surface oxides or bridging metal.


In previous experiments during analysis of devices with trench structures, TMAH etch was found to be highly preferential to etching silicon over both silicon dioxide and aluminum, see section on TMAH etch results. Having some inside information of the device structure, a possible technique for uncovering solder bridging using the TMAH was designed. The process would involve polishing the device so as to expose the cathode or backside of the die. The polish should thin the silicon but stop short of damaging the surface of the die. This technique would leave the backside of the die exposed with the die still imbedded in the mold compound. The TMAH etch could then be used to etch the silicon back and leave the solder and surface oxides intact. This would leave the suspected solder bridge sandwiched between the mold compound and the surface oxide. It was felt important not to etch the surface oxide. In this way the oxide would act to preserve the metal bridge helping to protect it from being washed away during rinsing of the device following the chemical deprocessing.


In order to verify the etch technique, devices suspected to have solder bridges would be required.


In the previous paper [1] it was found that the internal die temperature of devices in large and standard surface mount (SMB and SMC) packages could be raised above the re-flow temperature of the internal solder. Applying a short duration high power pulse


had this effect. Because these devices were in relatively large packages, 160x130 mils, the analyst could use the technique of mechanically separate and inspect the die to verify the failure mechanism.


Although successful, it did take many samples to be able to break the devices without loosing the solder bridge in the process.


Figure 1 Cross-section of the device.


Shortly after the initial technique was tested, a reliability test was being run in order to determine the maximum power pulse that a Schottky diode in a Powermite® package could safely be subjected to.


Several devices failed the midrange and highest power tests. Electrical characterization of the devices found them to exhibit unstable anode to cathode shorting. Solder bridging was suspected. Due to the small dimensions of the device, 69x69 mils,mechanical decapsulation would be difficult. This appeared to be the ideal case to further develop the TMAH technique.


The first step was to expose the backside of the die,see figure 1. The backside material was ground off using a polishing wheel. A x-ray system was used to determine the thickness of the die remaining in the package. In order to prevent any damage to the surface of the die, approximately 8 mils of die material was left in the package.


The devices were next placed in a 10% TMAH to DI water solution (see section on TMAH etch results for concentrations) maintained at 100 °C. The temperature was maintained by using a double boiler technique in which the TMAH beaker was placed inside of a beaker of boiling water. The devices were monitored every 30 minutes. Once the edges of the oxide were exposed the devices were monitored every 15 minutes until the area of interest was exposed.


Generally, this took in excess of two hours for the process.


As the etch exposed the top edges, a cavity was left in the mold compound where the die had been as well as a pyramid of silicon in the center of the device, see figure 2. The TMAH etch being isotropic etched in from the sides as well as the surface, creating the silicon yramid. The edges of the devices were the areas of interest, so once the edges were cleared the etching was terminated. Optical inspection of the edges revealed the suspected solder bridges, see figure 3.


Figure 2 An SEM image of the device after 3 hours in TMAH. Note the pyramid shaped silicon chunk that remains.


TMAH etch experiment


TMAH was used to for the backside technique. This section explains the methodology behind the decision.


Although there are many well-known etchants used for silicon removal, this application required a high etch rate for both n+ and p+ silicon with little or no attack of silicon dioxide, aluminum, and solders (Sn -Pb). The most common silicon etchants, nitric:HF mixtures, have high n+ and p+ silicon etch rate, but have poor selectivity against silicon dioxide and most metals. Hydrazine [2] and the ethylenediamine -pyrocatechol [3] based etchants were not considered due to safety concerns in our lab. Potassium hydroxide (KOH) -water [4] and tetramethylammonium hydroxide (TMAH) - water


[5] mixtures are well known to have very high oxide selectivity for n-type silicon but little is discussed about p+ silicon etch rate in the literature. Despite the problem that KOH has a very high aluminum etch rate, KOH and TMAH were selected to do further experiments and determine their p-type silicon and silicon dioxide etch rate.


Figure 3 Optical inspection of the backside of the die clearly shows the solder extrusion extending over the edges of the top metal. The bottom image also shows that not all of the silicon was cleared from the metal.


In these cases it was not necessary.


Silicon etch rate was determined by weight loss measurements. Silicon substrates were cleaved into 1x3cm strips, etched in 1:1 (HF:water) to remove a 3000A backside oxide, rinsed, then baked for 2 hours at 125 °C to remove any residual surface moisture and weighed to 0.1mg. Before etching, the strips were dipped in 1:1 (HF:water) to remove the native oxide. The strips were etched for 60 minutes at 100+/- 5 °C, rinsed, then weighed again. Covering the beakers with watch glasses reduced evaporation. The silicon thickness removed can be determined using the silicon density and area. We ignored the slight error caused by not accounting for the strip edges because they amount to only 2 to 4% of the total surface area. Silicon etch rates were determined for a variety of KOH-water and TMAH-water dilutions using boron doped, (100) substrate orientation with 2 x 1015, 3 x 1018, and 3 x 1019 boron atoms/cm3. Silicon dioxide etch rates for a 400 Å (dry+HCl) gate oxide and 10 kÅ plasma enhanced TEOS (PETEOS) films were determined by etching the films simultaneously with the substrates and measuring the film thickness change using a Nanospec AFT with <10 Å error.


The results are shown in figure 4, with each data point being the average of 3 to 5 runs. Interestingly,the peak etch rate for both KOH and TMAH was at 10 wt% dilution with water. The PETEOS film had 3 to 5 times greater etch rate than the gate oxide.


Silicon/silicon dioxide selectivity for the gate oxide


and PETEOS film was roughly parallel and peaked at 20 wt% TMAH and 10 wt% KOH (figure 5).


KOH etch rate of Boron doped samples


1.8


35


wt % KOH


2ee15 3ee18 3ee19


TMAH etch rate of Boron doped samples


0.7


wt % TMAH


Figure 4 Silicon etch rates (μm/min.) for Boron doped substrates verses wt % of etchant. Top graph shows KOH, bottom TMAH. Both appear to peak close to 10%.


KOH Silicon to Silicon Dioxide etch


0 50 100 150 200 250 300


2ee15/GOX


3ee19/GOX


2ee15/PETOS 3ee19/PETEOS


TMAH Silicon to Silicon Dioxide etch ratio


0 1000 2000 3000 4000 5000 6000 7000 8000


2ee15/PETEOS 3ee19/PETEOS


Figure 5 Ratio of Silicon to Silicon dioxide etch rates for gate oxide (GOX) and Plasma Enhanced TEOS(PE/TEOS) verses wt % of


etchant. Top graph shows


KOH, bottom TMAH.


Based on this data we selected 10 wt% TMAH in water at 100 °C for experiments with real devices.


There is no discernible oxide etching and minor aluminum attack. Schnakenberg et.al. [5] discusses a method to reduce TMAH attack on aluminum by predissolving silicon in the etch solution but we could achieve a similar result and currently accept minor aluminum attack.


TMAH, as a silicon etchant, used to reveal solder bridges was demonstrated on several different samples. In many cases this may be the only reliable method for the analysis. The etch data given was obtained for p-type substrate material. Although the etch rates may vary, similar results are anticipated for n-type substrates. Subsequent to the solder analysis a successful attempt, on a different analysis, was also made to uncover copper dendrites on a single sample.


1. J. Di Silvestro, Simon Keeton, Kent Kime, Ruth Ruiz, Chuck Reed, Gene Thome,“Mechanical/Plasma Decapsulation Method and Thermal Finite-Element Analysis Provide Explanation for SMB Zener Failures“ 24th International Symposium for Testing and Failure Analysis pp. 353-358 (1998)


2. M.J. Declercq, L. Gerzberg, and J.D. Meindl,“Optimization of the hydrazine-water solution for anisotropic etching of silicon in integrated circuit technology,” J. Electrochem. Soc., vol.122, no.4,pp.545 (1975).


3. R.M. Finne and D.L. Klein, “A water-aminecomplexing agent system for etching silicon,” J.


Electrochem. Soc., vol.114, no.9, pp.965 (1967).


4. J.B. Price, “Anisotropic etching of silicon with KOH-H2O-isopropyl alcohol,” in Semiconductor Silicon, publ. Electrochemical Society, pp.339(1973).


5. U. Schnakenberg, W. Benecke, and P. Lange,“TMAHW etchants for silicon micromachining,”Proc. of IEEE Transducers ‘91, pp.815 (1991).


p 235-239


DOI: 10.1361/cp2000istfa235


Selective Au Etching in Au/Al Bonds in Current IC Technology


University of Cagliari, DUIEE-INFM, Cagliari, Italy


A. Serpe, E.F. Trogu, P. Deplano


University of Cagliari, Dip. Chimica e Tecnologie Inorganiche e Metallorganiche, Cagliari, Italy


C. Hartfield, W. Subido


Texas Instruments, Dallas, TX, USA


A new Au etch, recently developed for selective Au etching on Ti/Pt/Au metallization of optoelectronic devices, has been tested on Au wires bonded on Al films. Contrary to theoretical expectations, Au wires are removed without Al damage, except for a very localized area around the bond interface. The role of the native Al oxide is discussed in preserving Al and allowing Au lift off.


New selective Au etching has been recently proposed for compound semiconductor technology and specifically demonstrated for GaAs-based laser diodes where selective Au dissolution was required on Ti/Pt/Au triple metal systems [1]. In that case,although the oxidation potentials of the two noble metals were similar, with Au having slightly higher oxidation potential than Pt, selective dissolution of a 1μm thick Au layer from the top of a similarly thick Pt layer was achieved without damaging the Pt layer(Figure 1).


The etch is based on the bis-diiodine adduct of N,N’-dimethylperhydrodiazepine-2,3-dithione (from here forward abbreviated as D.2I2, where D stands for the eptamethyl (Epta-Me) donor). It uses dilute tetrahydrofurane (THF) or acetone as a solvent. This greatly helps in cleaning the specimen surfaces after environmental test.


The success of the etch for the reported applications led to its experimentation on silicon technology for removal of Au wire bonds from bonded devices to facilitate failure analysis for optimization of probing and bonding parameters during packaging development and assembly. Lack of good intermetallic formation between the Al bond pad and Au wire, from either surface contamination, probe


damage, or improper bond parameters, will result in lifted ball bonds. Too much force during the bonding process will cause mechanical damage which may not be immediately apparent (interlevel dielectric (ILD)microcracks beneath the bondpad surface), or may result in immediate gross failure (lifted metal failures). The microcracks are a reliability concern due to their role as being an initiation site for subcritical crack growth and also due to concerns of leakage. The ability to identify interconnect defects beneath bond pads rapidly and reliably during learning cycles is critical for successful implementation of low-k dielectric materials.


Figure 1 View from the top of a InGaAs/AlGaAs laser diode after etching the Au. The exposed


Pt layer has been completely preserved.


One method commonly used for identification of microcracks beneath a wire-bonded pad is the use of an etch to remove the ball bond, allowing visual access to the layers beneath the pad. The use of etches are preferable to cross-sectioning as they are faster techniques, and there is greater chance to catch the defect since pre-knowledge of the fail site is generally not required. In addition, some etches allow determination of % intermetallic formation.


Under the best conditions, the etches will provide access to the entire pad area for all pads on a device


in a short period of time (minutes to hours).


However, many etches do not work well on devices with very strong intermetallic formation, or on devices that are aged by time and/or temperature. In addition, shrinking geometries and changing material sets are creating a need for new etches which are less


aggressive to the Al and underlying materials. Thus,it is desireable to develop an etch that could remove a ball bond from an Al pad while retaining the impression of the probe mark for site-directed FIB inspection for microcracks.


Figure 2 Etch results on unpatterned Al film. a) as received b) after 4 minutes.


Figure 3 Etched specimen at three different steps: a) as received b) 2 min etch c) 4 min etch d) 9 min etch.


The outlined area marks the Al etch boundary after the first etching step, indicating by reference in c and d the small increase of Al dissolution. In d) the wire has lifted off.


Experiments


Both theory and first experiments on pure metal powders were discouraging: due to the oxidation potentials of Al and Au, it was expected that Al should be etched much more quickly than Au. This happened, indeed, as soon as pure Al powder was added to the etch. However, when the experiment was performed on a suitable simple test pattern (a wafer of CVD deposited blanket Al bonded with a few dozen Au wire bonds closely aligned), the result in Figure 2 was obtained. Here, an irregular area is etched into the Al layer, around the complete circumference of the Au bond. Away from the bond itself, aluminum survives.


Figure 3 documents the etch progress when carried out in steps, with multiple cycles over a 10 minute time span of dipping, rinsing and drying for microscopic observation. The last step shows the wire removed not by complete Au dissolution, but by simple lift off after etching Al from the contact area.


The most peculiar phenomenon is the shape of the boundary of the Al dissolution. It is not evenly increasing at each new etching step, but merely adding new “lobes” at some places, and in many cases simply remaining the same as after the very first step. Some Al-rich rings (revealed by EDS)remain in the etched area (Figure 4), surviving any further chemical action.


Figure 4 After etching, under the lifted Au bond an Al-rich ridge survives.


When a patterned sample was etched (Figure 5), the same effect leading to final wire detachment resulted.


Where Au wires were bonded to some of the many available bond pads, Al etched only from a limited area at and around the Au bonds. The unbonded pads remained perfectly intact even after the last etching step.


Figure 5 Optical images of an unpassivated die with bonded and non-bonded pads (top, as received).


After the etch (bottom), as the wires start to detach,unoxidized Al is revealed and etched at the bonded pads, while the unbonded Al pads survived.


Interpretation


The results are puzzling under many points of view and call for more complex kinetics for the Au/Al/Epta-Me2I2 interaction on actual structures than on pure elements. The first question is why Al is not etched away from the great majority of the wafer surface. Second, why should this rather surprising effect disappear near the massive gold bonds? Third, why does the etching of Al under and around the Au bonds display such an irregular behavior, documented in Figures. 3 and 4?


The hypothesis of a much slower etch speed for Al than Au is contrary to both theoretical expectations and experimental observations on Al powders. But this could also be defended, provided a mechanism is proposed for enhanced Al etch reactivity near the bond areas. In this case, early wire bond removal by lift off simply shortens the etch time enough to avoid complete metal dissolution from the whole surface.


Such a mechanism could potentially be influenced by intermetallics or electro-chemical properties.


In the case of Au/Al intermetallics formed during wire bonding, it is expected that any Au-rich phase should be etched faster. Unfortunately, neither industry experience in wire bonding nor local measurements on actual devices indicate any significant intermetallics extending out of the metallurgical interface to an extent comparable with the size of the observed Al removal. Considering an electro-chemical effect, the relationship of the Al/Au oxidation potentials does not clearly state that aluminum should act as the sacrificial element of a cell. Moreover, the boundary of the etched Al should be a sort of smoothed wave front evenly propagated from the original boundary of the Al/Au interface,which is not the observed case.


The Role of the Native Oxide


A reasonable explanation for all observed phenomena is achieved by considering a native Al oxide. First of all, such a native oxide is formed rapidly on exposed Al and may even create a possible problem for proper Au bonding on aged devices. Second, this oxide is known to be extremely thin, tenacious and brittle. In this way, with a few monolayers, it passivates the bare Al from further oxidation and is resistant to many of the most aggressive etches, yet allows ohmic bonding by breaking under the mechanical action of bonding. The observed phenomenon of Al preservation under Epta-Me-2I2 etch is quite compatible with the passivation role of the native Al oxide.


Figure 6 Etching sequence. a) a gold layer on a thin Al film deposited on a bulk substrate; b) under Au etch, gold thins and exposes unoxidized Al, reacting with the etch solution; c) the etch completely cuts the Al film and continues laterally. At this point the sample is removed, rinsed and dried, and an Al oxide covers the newly exposed Al; d) starting a new etch step, the process is repeated, leaving unetched the oxidized surfaces; e) the only reacting Al is under the gold layer; f) the residual Al under gold is dissolved,gold lifts off.


As the process is considered in more detail (Fig. 6) it clearly supports the hypothesis that Al oxide exists only at the exposed Al surface, while at the Au/Al interface the electrical continuity of the contact ensures that the oxide, if present, has been extensively fractured and dispersed. During the very first etch exposure of a wirebonded Al pad, initially only Au dissolves, decreasing the remaining bonded area and leaving some non-oxidized Al exposed to the etch.


The etch itself does not include free oxygen that would be available to oxidize the Al.


Thus, the etch dissolves the unoxidized Al and penetrates entirely through the film thickness. The chemical reaction continues laterally, both inward under the Au bond and outwards. The etch efficiency is here limited by the very narrow reacting surface that is only the cross section of the Al film, and preferential directions may be displayed, depending on the Al texture. As soon as the etch is stopped for microscopy purposes, the rinsed and dried specimen once again meets the room atmosphere. The native oxide may now form at the exposed transverse Al surfaces, passivating them.


Once exposed to the etch again, the outer Al film has no more available entrances for the etch, apart from possible local pinpoints (dust, edges, etc.). Under the Au bond, on the other hand, the process could continue, because Au is further dissolved and new pure Al surface is exposed. It is interesting to observe tracks of the previous oxidized Al boundary must survive, giving rise to the observed “rift”. The process continues until the wire bond lifts off due to complete dissolution of the underlying Al.


Discussion and Conclusions


The proposed role of the native Al oxide accounts for the observed puzzling behavior of the Au etch when it is applied to Au wire bonded patterned devices and bonded blanket Al films. It is interesting to notice how the chemical process deviates from theory due to the unique features of the relationship between Al top metal and Au wire bonds in IC technology. From the failure analysis point of view, the result is the ability to remove Au bonds from Al without damaging the Al surface away from bonded areas. However, it is desired to minimize the Al damage at the bonded areas as well.


A possible development will be varying the solvents for the Epta-Me-2I2, including possibly adding oxygen, perhaps in the form of hydrogen peroxide or even simple water. In that case, the oxidation of Al


by the iodine ions of the solution should be substituted with oxidation by oxygen atoms to form Al oxide. This should preventing Al dissolution when unoxidized Al becomes exposed to the etch.


This work has been partially supported by Regione Autonoma della Sardegna – Consorzio21.


1. M.Vanzi, A.Bonfiglio, P.Salaris, P.Deplano, E.F.


Trogu, A.Serpe : “Selective Au-Etching on aged GaAs-based Devices” ISTFA99, p.233


p 241-244


DOI: 10.1361/cp2000istfa241


A Novel Method to Analyze the Deep Trench Capacitors in DRAM


Jack Lee, Kuo-Hui Huang and Jen-Lang Lue


ProMOS Technologies Inc., Hsinchu, Taiwan


A novel method has been developed to reveal the entire three dimensional (3D) deep trench (DT)capacitors for inspection in DRAM, especially NO capacitor dielectrics, ASG residues at corners,morphology etc., for process evaluation and failure analysis. It offers an alternative to conventional cross-section polishing, top down polishing or FIB milling methods. A DRAM chip was ground and polished down to a certain level from the chip backside. An etching solution was then applied to enhance the DTs appearance. 3D DTs can be inspected in scanning electron microscopy (SEM).


The entire DTs or specific DT also can be lifted out for detailed investigation in transmission electron microscopy (TEM). The innovation of this technique is to provide a quick 3D observation in SEM, and much more flexibility to an entire DT inspection in TEM, which were not presented before.


Introduction and Background


The deep trench (DT) capacitor has played an important role in submicron technology for high density DRAM due to its large storage capacitance [1-3]. The analysis in electron microscopy for the trench node, especially NO capacitor dielectrics, ASG(arsensilicate glass) residues at corners, morphology etc., is always very important for process evaluation and failure analysis. As feature size becomes smaller,the DT analysis will become more difficult and challenging to the conventional methods, the plain view and cross-section view [4-6]. The plain view and cross-section view have been very useful and common methods for physical failure analysis and process evaluation in the trench node as shown in Figure 1 and Figure 2, respectively. However, there are some limitations to perform detailed information due to the uncertainty of the sectioning planes to


0.1μm thin film during sample preparation. During the sample preparation step, the areas containing defects may not be covered with the 0.1μm thin film for TEM observation as shown in Figure 3. Most of the feature and information will be polished away due to the process of sample preparation. In order to complement the disadvantage of plain view and cross-section view,


the observation of an entire 3D DT will be introduced in this paper. 3D DTs can be revealed by chemical solution and lifted out for further investigation in electron microscopy. The innovation of this technique is to provide a quick 3D observation in SEM, and much more flexibility to an entire DT inspection in TEM, which were not presented before.


Figure 1 TEM image showing the plain view of trench capacitor.


A chip was prepared from a Si (100) 64M/128M DRAM wafer. The chip front side was mounted onto a glass slide by wax. The backside of the chip was then pre-thinned to about 50μm thick by mechanical polishing with diamond films. The final polish for the chip backside was done by colloidal silica suspension to obtain a smooth surface. Later, the chip was removed by placing the glass slide onto a hot plate,and then cleaned with acetone and alcohol.


An etching solution of KOH with about 16% KOH by weight and 84% distilled water by weight was applied to the pre-thinned chip to etch away Si substrate for 3D DTs appearance. The KOH solution was preheated to about 80 degrees Centigrade. In order to handle easily


the pre-thinned chip into the etching solution and observation for optical microscopy and SEM, the prethinned chip of front side was mounted onto a smooth and flat substrate by epoxy. The Si substrate remaining of backside chip can be controlled at certain levels depending on the etching time. After removal from etching solution, the specimen was cleaned with distilled water or alcohol, and then dried it very fast.


Drying after alcohol cleaning had better DT appearance than distilled water cleaning. The overview for the 3D DT appearance can be viewed in optical microscopy (OM) and SEM.


Figure 2 TEM image showing the cross-section view of deep trench capacitors.


Figure 3 Schematic of 3D trench containing defects shows the 0.1μm thin film may not cover defects during sample preparation for TEM observation.


For the failure analysis, the DTs needed to be lifted out using a micro-manipulating system with a probe.


After DTs was lifted out, the DTs will be placed onto a carbon film grid for further SEM and TEM observation. Detailed information for DT’s lifting out from a micro-manipulating system with a probe will not be described in this paper.


Some applications using the techniques developed here will now be discussed.


Incomplete DT Formation


Figure 4 shows a SEM image with 3D appearance for incomplete DTs formation after KOH chemical etching. It is obvious that there were some incomplete formations for deep trench capacitors during manufacturing process. Figure 4 is also a typical image for 3D DTs appearance at complete DTs regions. Before inspected in SEM, OM inspection showed an incomplete region over the chip as indicated in Figure 5. The incomplete region was further identified to be the DTs missing by SEM as shown in Figure 4. This 3D DTs appearance provides a very quick way to check failures.


Figure 4 A SEM image showing 3D structure for incomplete DTs formation.


Figure 5 OM image showing the incomplete region.


ASG residues


The following images are some results after DTs were lifted out. Microstructures for entire DT inspection at trench node area were inspected for process evaluation and failure analysis. ASG residue after out-diffusion into Si substrate to form buried plate [1-2] was not etched away before NO dielectric formation as shown in Figure 6. Tilted angles must be considered for detailed inspection during TEM examination. A supplemental Energy Dispersive Spectroscopy (EDS) analysis in Figure 7 applying to the gray area as indicated a circle in Figure 4 confirmed that it contained ASG. Figure 8 and 9


show the typical images of plain view and cross section view for ASG residues at trench node.


However, due to the discontinuity of ASG residues on the outer surface this technique provides more reliable information for process evaluation compared with conventional methods. With conventional methods the information of ASG residue may not be found as discussed in Figure 3 because the areas containing residue will be missed during sample preparation or interfered with by Si substrate during TEM examination. For the purpose of ASG residue examination, the method developed here will be suggested to use for analysis.


Figure 6 A TEM image after DT was lifted out


shows ASG residues remained.


Figure 7 EDS results shows As was


detected at ASG. region.


NO Dielectrics and Polysilicon Seam


NO dielectrics were easily observed as shown in Figure 10. NO capacitor dielectrics can be investigated and measured to the entire trench node,which will be very helpful for process evaluation.


With conventional cross-section method, it is difficult and extremely time-consuming to perform this kind


of inspection at entire trench node area, especially trench bottom as described earlier. Meanwhile,polysilicon seams were also observed as shown in Figure 10.


Figure 8 A typical TEM image of plain view


showing ASG residues at trench node.


Figure 9 A typical TEM image of cross section view


Deformed DT


A bump due to DT deformation was found after examining the entire DT by TEM as shown in Figure


11. Through the technique from manipulating system the DT can also be turned 90 degrees under OM for TEM observation. This deformed DT was also found in SEM observation as shown in Figure 12.


Figure 10 A typical TEM image after DT was lifted out shows the trench profile at trench bottom.


Figure 11 TEM image indicates a bump at trench node after DT was lifted out; the sharp corner may


produce a current leakage path.


In this paper a novel method has been developed to reveal the entire 3D deep trench (DT) capacitors for inspection in DRAM for process evaluation and failure analysis, instead of conventional cross-section polishing, top down polishing and FIB milling methods. A DRAM chip was ground and polished down to a certain level from the chip backside. A KOH etching solution was then applied for the DTs appearance. 3D DTs can be inspected in SEM. The entire DTs or specific DT also can be lifted out for detailed investigation in TEM. This method was well implemented into some applications as discussed in the results. The approach of this method provides a quick 3-D observation in SEM, and much more


flexibility to an entire DT inspection in TEM. As feature size becomes small, this method will become one of the important choices for failure analysis and process evaluation in the future.


Figure 12 SEM image also indicates a bump and


deformed surface at trench node.


The authors would like to present our thanks to the colleagues at Department of Physical Failure Analysis at ProMOS for their insightful discussion and support.


1. P Kucher, H. Aochi, J. Gambino, T. Licata, T.


Matsuda, S. Nguyen, M. Okazaki, H. Palm, and M. Ronay, Applied Surface Science, 91, 359-366(1995)


2. E. Adler, J. K. DeBrosse, S. F. Geissier, S. J.


Holmes, M. D. Jaffe, J. B. Johnson, C. W.


Koburger III, J. B. Lasky, B. Uoyd, G. L. Miles,J. S. Nakos, W. P. Noble, Jr., S. H. Voldman, M.


Armacost, and R. Ferguson, IBM J. Res.


Develop. Vol. 39, No.1/2, January/March , 167-187 (1995)


3. Clarence W. Teng, Yasuhiro Okumoto, Jiann Liu,Ih-Chin Chen, Katsuo Yuhara, and Yoshinobu Yoneoka, VLSITSA, 366-370 (1991)


4. T.T. Sheng and C. C. Chang, IEEE Transactions on Electron Devices, ED-23, 531 (1976)


5. R. B. Marcus and T.T. Sheng, Transmission Electron Microscopy of Silicon VLSI Circuits and Structures, John Wiley and Sons (1983).


6. T.T Sheng, Instruments Today, V15 No. 4, 51(1994)


p 247-249


DOI: 10.1361/cp2000istfa247


Identification and Analysis of Parasitic Depletion Mode Leakage in a Memory Select Transistor


Jim Colvin and Anirban Roy


WSI, Fremont, CA, USA


Low yield was reported for a non-volatile embedded memory array. This memory array is constructed of cells with two transistors per cell. The cell is comprised of a non-volatile transistor in series with a special n-channel (select) transistor. This select transistor is comprised of n+ with an LDD (LightlyDoped Drain) spacer on the source side and a DDD(Doubly Diffused Drain) n+ junction on the drain side. In one case, this n-channel transistor was observed to exhibit single bit OFF leakage in a 32K array. In another case, there was general leakage(many cells in the array) observed between drain junctions of neighboring transistors, even though these were isolated by field oxide. The objective of the failure analysis described in this paper was to characterize the electrical behavior of the leakage and determine the exact location and cause of the leakage.


Sample Identification


Appropriate dice for analysis were determined based on wafersort rejects and extensive memory pattern write and read operations on the Credence memory test platform (Model BTMA2001). The details of the electrical analysis on the Credence are beyond the scope of this paper. Leakage measurements were performed on the suspected select transistor by direct memory access of the leaky cell. The leakage current by the direct memory access technique was compared to the leakage current measurement obtained after physical isolation of the leaky cell with the FIB(Focused Ion Beam).


Traditional Approach


Selected dice were exercised on the Credence tester in programming mode to help generate enough photons for effective emission microscopy.


Location(s) of the leakage was identified on the Emission Microscopy System (FA1000) with a 50X objective, but the resolution of the image was not enough to provide localized information within the failing cell. Leakage measurement with direct memory access lacked the control required to isolate the electrical behavior of the leakage source further.


Deprocessing of the sample down to bare silicon did


not reveal any defects or abnormalities in the cell(s)in question. We were forced by circumstances to try new techniques.


New Approach


Direct contact and control of the terminals of the select transistor(s) under investigation was obtained by polishing the samples down to the contact plugs(removal of metal 1 from the array was necessary to lay down FIB traces). The FIB was used to make contact with the DDD n+ junctions, select transistor gate and LDD-N+ source junction. The FIB also provided micropads for microprobing to obtain the I-V behavior of the leakage.


Microprobing of the select transistor drain to source leakage (case #1) and select transistor drain-neighbor select transistor drain leakage (case #2) both exhibited a depletion mode (JFET) like I-V behavior suggesting presence of shallow n-type dopant impurities in the path of the leakage.


Determining the exact location of the leakage source within the cell(s) in question was obtained by combining the microprobing and photoemission techniques. To obtain higher magnification, a metallurgical microscope (Zeiss Axiotron) was utilized in conjunction with the photoemission camera and modified microprobes. A spatial resolution on the order of three hundred nanometers was achieved and thus helped to identify the exact location of the leakage source.


Case #1 Select Leakage


Several dice were identified with the bitline leakage problem in the memory cell. Figure 1 shows schematically the path across the select transistor.


Emission microscopy was used in conjunction with decoding to identify the exact location of the failing cell as shown in figures 2 and 3. The failing cell creates a leakage on the bitline, which can be eliminated by programming the failing cell. Once programmed, the leakage is gone due to the fact that the NVM (Non Volatile Memory) transistor is in series with the select transistor. This electrical information points to the select transistor as the source of the leakage. A test mode known as DMA


(Direct Memory Access) was used to measure the leakage current at the failing cell. Leakage on the order of 18 μA was found at 1.4 volts applied between the source line and bitline. Note: The cell is unprogrammed for this measurement.


The identified failure was deprocessed by stripping to substrate with HF and staining with Wright etch to delineate the junctions. No anomalies were observed as seen in figure 4. Another die was prepared in a similar fashion as above except Sirtl etch was used as the final delineation step.* No stress related or dislocation related anomalies were observed with the failing cell.


The next step was to eliminate any possible gate involvement associated with the word line over the failing cell using Passive Voltage Contrast (PVC).*PVC uses the electron beam of a conventional SEM to charge the surface at low accelerating energies to an equilibrium level. Any conductors, which have a path to ground, will not charge to equilibrium and appear bright. The sensitivity of measurement for the technique typically extends into the femtoamp range and is dependent on the beam current as well as scan area/scan time. No gate related leakage was observed.


The DMA current was recorded at 18.9 μA on another select failure and analyzed further. The part was surface polished to remove metal 2 and metal 1,leaving behind the tungsten plugs. Laser marks were placed equidistant from the failing cell to simplify navigation and the FIB (Focused Ion Beam) was used to connect the source line, drain and word line to allow the leakage behavior to be characterized. Figure 5 shows the location of the deposited platinum traces and probe points. The drain contact was created to allow direct electrical access to the select transistor. Figure 6 is a family of curves generated by stepping the Vgs (gate to source voltage) negative in 0.5 volt increments with a vertical scale of 5 μA/div. The curve at Vgs=0.0 with 1.4 volts drain force is 18 to 19 μA. This data point matches the previously measured DMA value of 18.9 μA prior to deprocessing. Note the depletion mode behavior of the transistor with a pinchoff of –4 volts. Figure 7 is the family of curves obtained for positive gate drive values from 0 to 1.5 volts in 0.5 volt steps and 10 μA/div. The saturated depletion mode characteristic transitions to an enhancement mode characteristic.


In order to perform emission microscopy with adequate spatial resolution the sample needs to be planar with minimal refracting oxide and under a high numeric aperture lens. The FIB preparation was done on the sample with all the metal interlayer dielectric removed by surface lapping. This allowed greatly improved spatial resolution of the poly word


lines. A temporary probe station to take advantage of this was put together using an aluminum plate and 3 vacuum probes as shown in figure 8. The probe tips were configured on a low entry angle as shown in figure 9 to allow biasing of the select transistor. Figure 10 clearly shows the location of the photoemission on the poly wordline associated with the left edge of the select. The drain to substrate breakdown was checked and found to be normal. The exact depletion site was triangulated with a sized overlay to the drawn layers. Dopant concentration control by modifying masking layers resulted in elimination of the problem in subsequent lots of silicon.


Case #2 Drain to Drain Leakage


Similar analytical methods were used to identify and analyze the drain to drain leakage. Extensive test patterns were used to pin down the relationship of the leakage path. The failure pattern was a “bull’seye” pattern on the wafer. Figure 11 shows schematically the drain to drain leakage across a field oxide isolation. A long integration photoemission image (1-hour) taken during programming revealed a leakage along the memory row in figure 12. Note the diminishing leakage away from the cell being programmed. As was done in case study 1, FIB probe points (figure 13) were created directly to the adjacent drain regions. Figure 14 is a curve of the leakage between adjacent drain structures that revealed a depletion characteristic of 30 μA at 4 volts. To confirm the series nature of the leakage,probing was performed on each side of a drain structure. The curve of the leakage in series across an isolated drain structure gave a depletion mode characteristic of 13 μA at 4 volts as shown in figure 15. Photoemission performed with an AC bias revealed the location of the leakage as shown in figure 16. DC bias will generate one or the other of the two sites based on polarity. A failing die from the center of the wafer was decorated using the Wright etch and compared to an edge die which was passing the electrical tests. No differences or anomalies to explain the failure were observed(Figure 17). Note: The drain area is labeled “D”.


Additional analysis was performed to map the nature of the depleted region by using Scanning Capacitance Microscopy.* This technique allows dopant concentration as well as polarity to be mapped on a properly prepared sample. In order to prepare the sample it is first stripped to substrate using 49% HF. The sample is then swabbed lightly with blue colloidal silica and a cotton swab. Organic soap and a foam swab are then used to clean the surface. The sample is baked at 200C for 5 minutes and exposed to 254nm UV light prior to the scan to dissipate surface charge. Figure 18 is a capacitive scan from the edge of the wafer corresponding to a good die. Figures 19 and 20 are capacitive scans


from the center of the wafer corresponding to a bad die. Note the n-type-depleted slot crossing the ptype region associated with every other row. The Wright etched sample from figure 17 was examined with the AFM in 3D topographical mode as seen in figure 21. The Wright etch enhanced defect stands a mere 50 angstroms in height but is visible and corresponds in location to the capacitive scan.


Corrective Action


The first case study involved dopant concentration optimization at the drain of the select transistor by modifying mask layers and good results were obtained in subsequent lots of silicon.


The second case study also involved a cell layout change to remove a parasitic n-type implantation from the FOX isolation region


Two elusive leakage problems were identified,analyzed and eliminated from the process using multiple analytical techniques. The FIB was used to make electrical contact to drain regions, which lacked a contact for microprobing. Once the electrical parameters were obtained, photoemission analysis was performed with modified probes for higher spatial resolution to pinpoint the leakage path.


Finally, scanning capacitance microscopy methods were used to prove the presence of the n-type depletion path.


The theory of a parasitic n-type dopant creating leakage was based on the I-V curves for the select transistor in the first case. In the second case the sample was stripped down to bare silicon with HF 49% and a high-resolution capacitance probe technique was used to image the silicon surface.


Very clear and positive confirmation of the presence of the parasitic n-type dopant was confirmed.


Cuong Trinh and Lucas Wong from the technology development group for suggestions and experimental results on the two case studies.


1. Margaret Wright Jenkins, “A new preferential etch for defects in silicon crystals,” Journal of the Electrochemical Society, vol. 131(5), pp.


757-762,1977.


2. Thomas W. Lee,”A Review of Wet Etch Formulas for Silicon Semiconductor Failure Analysis”, Microelectronic Failure Analysis Desk Reference, Fourth Edition, EDFAS ASM.


P. 598.


3. Jim Colvin, ”A New Technique to Rapidly Identify Gate Oxide Leakage in Field Effect Semiconductors Using a Scanning Electron Microscope”, Proceedings of the International Symposium for Testing and Failure Analysis,(Los Angeles, CA), October 1990, pp. 331-336.


4. Y. Strausser, J. Colvin,”Atomic Force Microscopy: Modes and Analytical Techniques with the Scanning Probe Microscope”,Microelectronics Failure Analysis Desk Reference, Fourth Edition, EDFAS ASM. Pp.


337-339.


Figure 1 Schematic view identifying the leakage


path across the select transistor.


Figure 2 Emission image of the failing cell during program of word line 00 (Bright spot above). The


failing cell leaks during program


sufficiently to be detected.


Figure 3 Close up emission image of the failing cell during program of word line 00 (Defective select).


During programming the expected emission is shown adjacent to the select failure.


Figure 4 SEM view of the failing cell after Wright etch enhancement. No defects were observed.


Figure 5 Optical image of the region after FIB connection. The pads allow probing of the defective select transistor to obtain a family of curves as well as emission information.


Figure 6 Family of curves for gate voltage values from 0 volts to –4 volts. Note the depletion style behavior of the transistor.


Figure 7 Family of curves for positive values of Vgs. The transistor acts as a saturated depletion in parallel with the expected enhancement characteristics.


Figure 8 Setup necessary to allow probing in conjunction with emission microscopy at high spatial resolution.


Figure 9 Close up view of the setup used to probe


with emission. The objective used


is .75NA 100X.


Figure 10 Photoemission image of select leakage


with 6 volts drain to source and 0


volts gate to source.


Figure 11 Schematic view identifying the leakage


path across adjacent drain regions.


Figure 12 Photoemission image of the adjacent drain leakage during programming. Note the diminishing leakage away from the cell being programmed.


Figure 13 FIB deposited probe points for adjacent


drain leakage measurements.


Figure 14 Curve of the leakage between adjacent drain structures. Depletion characteristic of 30 μA at 4 volts.


Figure 15 Curve of the leakage in series across an isolated drain structure. Depletion characteristic of 13 μA at 4 volts.


Figure 16 Photoemission image of the adjacent drain leakage with ac bias applied via the probe pads. DC


bias will generate one or the other site based on polarity.


Figure 17 SEM photo of the adjacent drain leakage after Wright etch enhancement. No defects were observed. Note: Orientation is 90 degrees from the previous images.


Figure 18 Capacitance probe image of a normal die at the edge of the wafer. Note that the light blue region indicates n+ type and dark blue indicates n–type dopants. The red regions are the p– areas.


Figure 19 Capacitance probe image of a failing die due to adjacent drain leakage from the center of the wafer. The arrows illustrate one of 8 leakage paths across. Note that the light blue region indicates n+type and dark blue indicates n– type dopants. The red regions are the p– areas.


Figure 20 Capacitance probe image from figure 19 displayed in 3D format.


Figure 21 3D AFM topographical image of the area from figure 17. The Wright etch enhanced defect


stands a mere 50 angstroms in height.


p 255-262


DOI: 10.1361/cp2000istfa255


Thermal Fatigue Induced Voiding in LDMOS Transistors Submitted to Multiple Energy Discharges


I. Garcon1, J.M. Bosc1, C. Levade2, 3, M. Cabié3, G. Vanderschaeve2, 3


1 Motorola Toulouse, Le Mirail - B.P. 1029, 31023 Toulouse Cedex France 2 CEMES-CNRS, BP4347, 31055 Toulouse Cedex France


3 INSA, Département de Génie Physique, 31077 Toulouse Cedex France


The repetitive energy discharge test (power cycling)is an accelerated stress test (AST) that can be used to characterize the long-term behavior of power transistors taking into account stress on customer final application. This paper describes the application of this test to an LDMOS transistor in order to optimize both design and size while preserving final reliability of the product.


We will detail this reliability characterization program, emphasizing the power cycling tests performed in extreme conditions in order to reach and study physical limit of LDMOS devices.


Analysis of LDMOS devices under these extreme conditions indicated evidence of metal voiding: the conditions of formation of these thermal fatigue induced voids will be discussed.


The effect of major parameters like power cycling energy, ambient temperature will also be discussed.


Electrical characterization of stressed devices will be presented. Finally, the results of the Transmission Electron Microscopy characterization of the metal microstructure will be discussed.


Developing Accelerated Stress Testing in order to predict both the long-term behavior and reliability of a device is key in the semiconductor industry where time to market becomes a key success factor. In most of automotive applications (ABS, Injection systems,etc…), the Integrated Circuit (IC) power driver stages are composed of integrated LDMOS transistors with a clamp connected between drain and gate. These transistors are generally connected to inductive charges (valve solenoids, etc...). In such applications,the components are submitted to repetitive energy discharges, which induce a drastic temperature rise in the silicon. This temperature rise can cause evolutionary degradation due to thermal fatigue resulting from temperature cycles applied on the device. When such devices are excited by short


duration discharges (<2ms), the temperature rise is located within the die. The device package, even with an additional heat spreader does not play a major role[1]. So the situation during transient operation must be handled at silicon die level.


The output stages of power ICs take usually a significant area of the die and the temperature rise within the device during the power discharge depends on output transistor size. In such applications, the limiting factor in power device designs is the energy capability of the transistors submitted to inductive discharges.


Test vehicle


A specific test structure (Figure 1) has been designed in order to perform AST on insulated LDMOS structures. These dice were mounted on engineering packages with direct wire connections from drain and source pads to external leads.


All the results presented in this work were obtained on medium size LDMOS (third LDMOS from the left on figure 1).


Previous work [2] showed that for a same ambient temperature and a same delta T (applied energy to reach a same delta T depends on LDMOS size), life time of LDMOS device was not size-dependent.


Figure 1 Test vehicle overview.


Figure 2 is a schematic overview of LDMOS structure. Passivation was made of a 0.7μm thick bilayer of oxide and nitride. Metal 2 lines consisted of large plates of 2 μm thick aluminum-copper stacked with Ti and TiN layers.


The interlevel dielectric thickness was ~1.5 μm.


Metal 1 lines were 0.6μm thick.


Figure 2 Schematic overview of LDMOS top layers.


Accelerating Stress Test Circuit


In order to evaluate the temperature rise inside the device when an energy pulse is applied, a characterization circuit based on a 68HC11 microcontroller was set up. This circuit is able to apply energy pulses on the device under test (DUT), then to measure the temperature inside it [3].


It is composed of three modules: an application card based on a 68HC11 micro-controller, an interconnection card and a card dedicated to support the device under test.


This circuit is able to run with an inductive or a resistive load, which corresponds to apply a triangle or square shaped energy pulse. In this study, we have chosen to use a resistive load which corresponds to a square shaped pulse (figure 3).


1 ms


1s


P(W)


Figure 3 Short-pulse sequence


Figure 4 summarizes the main elements of the AST :


- Delta T: maximum temperature increment.


Delta T = Tmax- Tamb


with Tamb the ambient temperature of the stress test.


Tamb can vary from –40°C to 155°C.


- ton : energy pulse duration.


- toff the duration between two energy pulse.


The delta T and the pulse duration ton depend on the application conditions. However, in order to find the shortest toff allowing the shortest cycle duration, we have analyzed the cooling curves of the tested structures. Indeed, we wanted to avoid thermal runaway. For these tests we have chosen a ton of 1ms and a toff of 1 s. Using these test conditions, we are able, for specific applications, to simulate 3 years of aging with a test that takes only a few days.


Figure 4 Accelerated Stress Test Parameters.


Aged devices analysis and failure mechanism


Optical inspection of extreme conditions stressed devices before failure, revealed a specific evolution within LDMOS structures. A surface bulging could be evidenced as illustrated on Figure 5.


As shown on the Focused Ion Beam (FIB) section(Figure 6), this surface bulging effect was consecutive to void generation and propagation within metal 2 line, inducing a volume increase of the line.


These features worsened when the number of power cycles increased. Another FIB cross-section across the LDMOS drain-source spacer clearly evidenced that power cycling could induce, in extreme stress conditions, metal 2 lateral extrusion across passivation layer (Figure 7). Increasing power cycling at this stage will enhance metal voiding and extrusion. As a consequence, the probability that source metal extrudes and comes in contact with drain metal will become critical and device failure will immediately follow.


Figure 5 a-Optical micrograph of bulging effect on LDMOS surface.


b- Surface profile along arrow drawn on figure 5a :bulging amplitude of 1.6 •m can be evidenced on stressed LDMOS.


Figure 6 Relation between surface bulging and metal voiding.


Figure 7 Metal 2 lateral extrusion


through passivation


Thermal fatigue voiding origin


The voiding phenomenon within metal lines is a well known mechanism and has yet been studied in detail


[4][5][6].


This phenomenon can be the result of either mechanical stress (S-voids) or electromigration(E-voids)[7][8]. In our case, current densities are too low (much lower than 106A/cm2) to induce E-voids.


Thermal fatigue induced voids are then a consequence of mechanical stress generated by passivation layer on top of metal line. Indeed, when the device is heated up to a temperature higher than 200°C, the passivation expands less than the metal and compresses the underlying layers.


The void growth mechanism is related to vacancy diffusion from tensile areas towards compressive areas along grain boundaries (See figure 8).


Vacancies


Aluminum grain 1


Atoms


Aluminum grain 3


Aluminum grain 2


Figure 8 Schematic view of vacancy diffusion along grain boundaries.


In early reports, stress induced voiding occurred either during wafer processing (passivation deposition process) or during device temperature storage. Many studies were performed in order to eliminate voids occurrence induced by these two main thermal treatments [9][10][11].


Metal extrusion


Metal 2 voiding


Bulged surface


Passivation crack


Metal voiding


5a


5b


1.6 μm


Unstressed LDMOS


Stressed LDMOS


Recently, K. Banerjee [12] reported voiding within interconnect metal lines which were induced by peak current (current density ~ 107A/cm2) and electrostatic discharge (ESD) event.


Now, it is the first time that stress induced voiding has been reported subsequently to energy stress testing. Moreover, analysis of the stress-voiding effect on power device characteristics has been rarely studied.


Formation of thermal fatigue induced voids


Study of conditions of formation of thermal fatigue induced voids as a function of AST parameters such as ambient temperature, delta T, or cycles number,required to quantify voids occurrence within the stressed structure. Usually, the interconnect metal line resistance is used to estimate void propagation


[13][14]. In our case, we did not have direct and inline access to metal 2 plate resistance. Moreover,metal voids could only be visualized by local destructive techniques as FIB.


As a consequence, we decided to evaluate void evolution thanks to the measurement of surface bulging amplitude.


For all performed experiments, bulging amplitude increased with number of power cycling. As a matter of fact, it is well representative of device thermal fatigue.


Figure 9 shows the evolution of bulging amplitude as a function of number of power cycling for different applied delta T. This graph clearly shows that device thermal fatigue is directly correlated to energy supply: the higher delta T, the more pronounced bulging.


0.8 1


250


Number of power cycling (kcycles)


delta T=205°C delta T=225°C delta T=243°C


Figure 9 Bulging amplitude as a function of number


of power cycling for different delta T( Tamb =25 °C).


0 0,2 0,4 0,6 0,8 1 1,2 1,4 1,6 1,8 2


200 400


600 800 1000 1200 1400 1600


Tamb=118°C / delta T= 150°C


Tamb=155°C/ d elta T=113°C


Tamb=25°C/ delta T= 243°C


Figure 10 Bulging amplitude as a function of number of power cycling for different Tamb and delta T.


The three curves presented on figure 10 were obtained for different ambient temperature and delta T with a common Tmax temperature (Tamb + deltaT)equal to 268°C. Two areas can be drawn on this figure. Indeed for short power cycling sequences(about a hundred kcycles), the same trend than the one presented on figure 9 was observed : the higher delta T, the more pronounced bulging is,independantly of the ambient temperature.


For long power cycling sequences (about a one million cycles), effect of delta T became less important than ambient temperature : indeed, units stressed at higher Tamb but lower delta T shows more bulging amplitude (see square and lozenge curves of figure 10).


In conclusion, delta T has large impact on device thermal fatigue during the early stage of power cycling while ambient temperature becomes the most stressing parameter for long power cycling sequences.


Some stages on the two square and lozenge curves of figure 10 can be noticed. No comment will be made on this specific curve profile. The way surface bulging amplitude measurement was performed(maximum amplitude found along profile across stressed LDMOS) is not accurate enough to be sure these curve steps are significant.


Electrical characterization of thermal fatigue induced voiding


For a complete electrical characterization of stressed LDMOS structures, three electrical parameters were measured on samples stressed in different conditions(see table 1).


Area 1


Area 2


Table 1 List of analysed units


Unit number


Bulging amplitude(μm)


Analysis performed#R 0 R + RDSon +TEM


# 1 0.24 R + RDSon+TEM


# 2 0.35 R


# 3 1.15 R + RDSon


# 4 1.6 R + TEM


# 5 0.25 R


# 6 1.75 R


# 7 0.35 R


Drain-Source Breakdown Voltage (BVDSS)measurement was first performed on several stressed units: no shift could be observed whatever stress test conditions. Power cycling test did not affect at all LDMOS characteristics at silicon junctions level.


In order to characterize impact of power cycling on the metal layers of the LDMOS structures, metal 2 lines resistance and RDSon measurements were undertaken. Results are presented in the following section.


Metal 2 line resistance measurement.


Four probes measurement technique was chosen for metal 2 lines resistance measurement as illustrated on figure 11. Two probe contacts were taken on aluminum pads for P2 and P4. The two other contacts were taken on metal 2 plate after opening a window through passivation layer thanks to Laser cut.


Validity of measurement technique was checked by comparing experimental results with theoretical results based on sheet resistance of metal 2 lines and LDMOS surface. Obtained results fit within an error bar of 8 % to theoretical values.


Structure LDMOS


Aluminum pads


P2 P4


P1 P3


Figure 11 Four probes resistance measurement technique.


Experimental results are presented on table 2: variation of metal 2 line resistance, due to power cycling, could be observed on two units only: #4 and


# 6. Those units present respectively, 1.6 and 1.75 •m of bulging deformation. Their metal 2 line resistance increased by about 65%.


For bulging amplitude lower than 1 •m, no effect of power cycling on resistance could be observed.


#1 #2


#3


#4 #5 #6 #7


Bulging amplitude


(•m)


0.24 0.35 1.15 1.6 0.25 1.75 0.35


(Rs-Rr) /Rr 0 0 1.90% 67% 0 66% 0


Table 2 Metal 2 lines resistance variation due to power cycling test.


Rs is the resistance value of stressed unit.


Rr is the resistance value of unstressed unit.


RDSon measurement.


The RDSon parameter is one of the most critical electrical characteristics to take into account when designing a power transistor. RDSon measurements were made to evaluate the impact of power cycling test on this parameter.


This measurement was performed thanks to curve tracer with Vgs=10V and Id=1A.


The experimental results are presented on table 3: measurement was successful for two units only, #1 and #3. Indeed, no gate pad was available on vehicle test die: gate contact was then taken after opening a window above metal 1 line.


Nevertheless, these two measurements lend evidence that RDSon parameter is much more sensitive to power cycling test than metal 2 line resistance.


Indeed RDSon variation of 8% could be observed for a sample with bulging amplitude of 0.24•m only. For a deformation amplitude of 1.15μm, RDSon parameter increases by 16%.


Ref unit


#1


#3 Bulging amplitude (•m) 0 0.24 1.15 RDSon*S – RDSon*Sref /


RDSon*Sref


8%


16%


Table 3 RDSon variation due to power cycling test.


RDson*S is the measured value of stressed unit.


RDson*Sref is the measured value of unstressed unit.


As a conclusion, electrical characterization of power cycling stressed units showed that this reliability test did not affect silicon but metallization layers and more specifically top metal layers : this stress slightly impacts metal line resistance, but drastically increases RDSon value.


Structural characterization by TEM analysis


The TEM analysis was a preliminary study of the microstructure of metal 2 lines especially the presence of voids as a function of the number of power cycling. Three types of specimen have been studied: reference piece #R not submitted to power cycling and LDMOS stressed at different stages of thermal fatigue tests: samples #1 and #4 with surface bulging of respectively 0.25 μm and 1.6 μm.


TEM observations were performed at 200 kV. Crosssections were first mechanically ground and finally argon ion milled to electron transparency. As the milling rate is higher for silicon than for metal, this procedure resulted in an inhomogeneous TEM sample with a thin and very brittle metal strip.


In all the observed samples the grain size is rather heterogeneous with no evidence of a significant grain size variation with power cycling. The largest grains reach 1 μm in size which is consistent with SEM observations (figure 12). Electron diffraction analysis did not show evidence of a texture in observed areas.


Figure 12 Metal 2 line SEM micrograph after


chemical etching of the cut surface.


Figure 13 is a bright field micrograph of the reference piece #R. It shows small and large grains and a grain boundary which crosses from part to part the metal line. No feature (small cavities, grain boundary decohesion…) which could be interpreted as void nuclei was observed in this sample.


Figure 13 Bright field TEM micrograph of the metal


2 line in the reference piece #R showing heterogeneous grain size.


The microstructure of sample #1 is very similar to the reference piece #R with no evidence of void nucleation.


For samples with a strong surface bulging, the most reliable observations have been made on sample #4.


Figure 14 is a bright field micrograph where voids are indicated by arrows. Their shape is comparable with those observed by SEM on FIB cut (figure 8)and their size is probably slightly enlarged by ion bombardment.


In our sample, voids were randomly distributed in the metal layer (figure 7): there was no evidence of any concentration at the passivation interface and vias. In the present Accelerated Stress Test, the nucleation seemed to be independent of topography and edge


1 μm


Grain boundary


location, at variance with what is reported in


[7][15][16][17]. However, the line thickness (2 •m) is here an important parameter which makes difficult the comparison with previous works generally done on thin layers (less than 1 •m); indeed, for a similar grain size such thin layers have a bamboo structure.


The voids observed in figure 14 seem to take more or less the shape of grain boundaries. Then, at this stage of the observations, we think that grain boundary diffusion could be predominant. Two facts should support this statement : i) Copper concentration in Al-Cu(0.5 wt%) lines is higher than the solubility limit and according to [16], copper atoms dissolved in Al grains are bonded to excess vacancies and suppress lattice diffusion ; ii) At temperatures lower than 400 °C - which is the case of the mean and peak temperatures in the AST described in this paper -grain boundary diffusion always dominates [18].


In conclusion, we have demonstrated that metal voiding could be generated by power cycling Accelerated Stress Test. Based on numerous test results, we could show that, at the early stage of the stress test, device fatigue is very sensitive to temperature increase (delta T) because of repetitive energy pulses. On the other hand, for long sequence tests of about a million cycles, the parameter which mostly affects device is ambient temperature.


Electrical characterization was performed on aged devices: RDSon parameter was proven to be very sensitive to this multiple energy discharges test.


Using TEM and SEM analysis, we demonstrated that thermal fatigue induced voids did not nucleate and grow in the same way than previously reported.


Finally, this study points out the LDMOS device physical limits during multiple energy discharge accelerated stress test. It can be used to optimize design and size of LDMOS while preserving its final reliability within the application.


The authors would like to acknowledge Cathy Julian and Jacques Crestou from TEM sample preparation laboratory of CEMES for their help. Special thanks also go to Daniel Berail and Jean Paul Caillaba from Motorola engineering assembly laboratory.


Figure 14 Bright field TEM micrograph of highly stressed sample #4.


1. P.Dupuy, PhD Thesis, Institut National des Sciences Appliquées de Toulouse, France, 1998


2. J.M. Bosc, I. Garcon, E.Huynh, P. Lance, I.


Pages, J.M. Dorkel, G. Sarrabayrouse, 12th International Symposium on Power Semiconductor Devices & ICs, Toulouse, p165-168, 2000


3. J.M. Bosc, P.Dupuy, J.Gil, J.M.Dorkel,G.Sarrabayrouse, Therminic Proceedings Rome,Italy, 1999


4. J. Curry, 22nd Annu. Proc. Reliability Physics 1984, Las Vegas , (IEEE, New York), p6, 1984


5. N. Owada, Proc. VLSI Multi-level Interconnect Conference, (IEEE, New York), p173, 1985


6. J.T. Yue, 23rd Annu. Proc. Reliability Physics 1985, Orlando (IEEE, New York), p126, 1985


7. T. Marieb, P.Flinn, J.C. Bravman, D. Gardner and M. Madden, J. Appl. Phys. 78 (2), July,p1026-1032, 1995


8. J.D’Haen, P. Cosemans, J.V. Manca, G. Lekens,T. Martens, W. De Ceuninck, M.D’Olieslaeger,L. De Schepper, K. Maex, Microelectronics reliability 39, p1617-1630, 1999


9. T. Hosoda, H. Yagi, and H. Tsuchikawa,International Reliability Physics Symposium,p202-206, 1989


10. K. Tokunaga and K. Sugawara, J. Electrochem.


Soc., Vol. 38, No. 1, January , p 176-180, 1991


11. S. K. Groothuis and W. H. Schroen,International Reliability Physics Symposium, p1-8, 1987.


12. K Banerjee, D.Y. Kim, A. Amerasekera, C. Hu,S.S. Wong, K.E. Goodson, 38th International Reliability Physics Symposium, San Jose, p283-288, 2000


13. J. C. Doan, J.C. Bravman, P.A. Flinn, T.M.


Marieb, 37th Annual international reliability physics symposium, IEEE, p206-212, 1999.


14. S. Foley, L. Floyd, A. Mathewson,Microelectronics reliability 40, p87-97 (2000)


15. S. Domae, H. Masuda, K. Tateiwa, Y. Kato, M.


Fujimoto, 36th Annual International Reliability Symposium, IEEE, p318-323,1998


16. S. Mayumi, T. Umemoto, M. Shishino, H.


Nanatsue, S. Ueda and M. Inoue, International Reliability Physics Symposium, IEEE , p15-21,1987


17. A. Tanikawa, H. Okabayashi, H. Mori,H.Okabayashi, International Reliability Physics Symposium, IEEE, p209-215, 1990


18. T.D. Sullivan, Appl. Phys. Lett., 55, p 2399-2401, 1989


p 263-266


DOI: 10.1361/cp2000istfa263


Humidity-Bias Driven Shorts in Multilayer Circuits:A Case Study in Failure Analysis


Hei-Ruey Harry Jen, Gerald S. D’Urso, and Harold Andrews


Engineering & Technology, M/A-COM Inc., Lowell, MA, USA


When a failure analysis (FA) involves a multiple layer structure separated by a polymeric material such as Benzocyclobutene (BCB), in a plastic package, it becomes a very challenging task to find out where the failure site is and how it failed. This is due to the fact that the chemical de-processing procedure removes BCB as well as the plastic molding compound. This paper outlines the studies carried out to determine the failure site and the root cause of the failure mechanism in a multilayer circuit and the steps taken to fix the problems. The methodology and results of this study are applicable to many other types of circuits.


The role of a Failure Analysis group varies, from primarily analyzing field failures to analyzing reliability test and qualification test failures. New parts, as they are being developed, go through various stress tests to validate their design and processes.


The objective of the failure analysis is to improve the design and/or process after failures are reported. By identifying the failure mode, failure mechanism, and reporting the corrective action, an FA can benefit the entire engineering community starting from design to manufacturing. The M/A-COM Engineering and Technology Department has developed an eight step FA process to facilitate the flow of the analyses.


They are: 1) Define problem statement, 2) Collect data, 3) Establish analysis plan, 4) Execute analysis plan, 5) Determine why, 6) Determine corrective and preventive actions, 7) Document and database, and 8)Celebrate. These eight steps have been proven to be a very helpful guidelines to increase analysis efficiency and reduce turnaround time. At the same time, a high quality output is maintained.


The circuit in this case study was a plastic packaged multilayer transformer which structure is comprised of four layers of gold (Au) separated by one layer of silicon nitride (SiN) and two layers of BCB polymer(Figures 1 and 2).


Figure 1 Plan view of the device.


Figure 2 Cross sectional view of the


multi-layer BCB structure.


Both plastic and ceramic packaged transformer parts were put through environmental tests. After temperature (85°C), humidity (85%RH) and bias(20V) testing for 72 hours, these devices exhibited“soft” (reversible) and “hard” failures. A tensile nitride layer was used to isolate the first and the second Au layers at a cross-over.


Visual inspection was performed using a compound optical microscope with a high resolution CCD camera attached. Mechanical polishing was done by various grades of sandpaper both in the cross sectional and planar view. A micro radiography xray machine was used to view, non-destructively, the device layout through the plastic package. A nitric etcher was used to chemically open the plastic package and expose the device and wire bond inside.


Both conventional scanning electron microscope(SEM) with a thermionic LaB6 filament, and field emission SEM (FESEM) with a thermally assisted tungsten field emission filament were used for electron microscopy imaging. A focused ion beam(FIB)/FESEM system was used to obtain cross sectional views at the precise location. An electrical probe station was used to probe the device for electrical failures. When combined with the liquid crystal technique and a precision laser cutting attachment, this probe station could be used to identify the hot spot (electrical short) location on the die.


As we follow the eight step failure analysis process,the first step is to define the problem statement. It is clear for this problem: why do we develop an electrical short after humidity, temperature, and bias environmental stress test? With this question in mind, we started to collect the data about this device,the process condition, the environmental test condition, etc. We learned that this device, when experiencing “soft” failure, recovered (electrically)after removing out of the environmental chamber and leaving it in ambient for an hour. Also, this device did not fail when it was tested in a ceramic package with open lid.


With the problem statement and enough data in hand,a strategy on how to analyze the part was developed.


It is always a good practice to start the failure analysis using non-destructive techniques. It is also always a good practice to start from the simplest technique.


When executing the analysis plan (step 4), all the steps and analysis should be recorded no matter whether it has signs of a problem or not. After performing several techniques, it has been beneficial to go back to re-examine the results obtained from the earlier analyses. Visual inspection and x-ray microradiography techniques were done to record any external and internal information without opening the package. There were no abnormalities observed. Electrical probing was also used to confirm the electrical short (Figure 3).


Figure 3 Electrical probe plot showing the short circuit response.


Figure 4 Auger Electron Spectroscopy spectrum shows residual Ti on the BCB surface.


There were possibilities that this short might be either through the BCB from one layer of metal to the other layer, or short within the same layer of BCB. To confirm whether there was any leakage path between inductor lines, surface analysis techniques were used.


Auger Electron Spectroscopy (AES) and Time-ofFlight Secondary Ion Mass Spectroscopy (TOF-SIMS)were used to examine devices that were intentionally removed from the wafer processing with two of the three BCB layers defined. AES result showed residual Ti left on the BCB surface between the inductor metal turns even after 1 minute of plasma cleaning (Figure 4). Because of the serious surface charging problem,TOF-SIMS was used to confirm and measure the residual Ti layer thickness. However, these experiments did not seem to relate to the failure of the devices but were helpful to improve the process and to prevent possible long term reliability issues.


It was time now to move onto the destructive techniques. First the chemical and mechanical deprocess. In this study, however, chemical deprocessing with nitric acid jet spray (to etch off the plastic molding compound) did not work because of the same etching rate between BCB and plastic molding compound. Once the plastic molding compound was removed, BCB was also removed and the entire multilayer inductor structure collapsed.


Mechanical polishing was carried out very carefully,layer by layer, to remove the BCB/inductor structure.


After removing each BCB/inductor layer, electrical testing was done using the probe station. It was this tedious process which confirmed that the electrical short happened at the first level of the device. After removing the top two layers of the BCB/inductor structure, the device was still electrically short.


A liquid crystal technique was used on the probe station to reveal the hot spot (electrical short)location. It was located at the first and the second metal cross-over. The hot spot location was further confirmed after isolating the area with a precision laser cutting tool. At this point, the failure site was physically located, however, still unanswered questions were how the device failed and what the failure mechanism was.


An FIB cross section through the failure site and subsequent FESEM examination revealed very clearly that at the first and second metal cross-over,the silicon nitride layer, used for electrical isolation,had a crack. Inside the crack was a chunk of gold connecting between the first and second metal(Figure 5). To confirm that this was not an isolated problem, several more devices were de-capped and the second layer of Au was etched. Optical microscopy showed the same location, where liquid crystal technique identified the failure, indeed had a crack so that the Au etching solution was able to get through nitride layer and etched away part of the first Au metal (Figure 6). FESEM inspection looking at the step of the cross-over on several devices also confirmed the crack (Figure 7).


One other piece of information was that the analysis done on the control part which never went through the stress test, did not reveal any nitride layer crack at the cross-over.


Figure 5 FESEM image of a FIB cross section showing crack in nitride and Au metal in the crack to


short the first and second Au metal.


Figure 6 Optical image after the second gold layer was removed. The over etch into the first gold layer


indicated a cracked nitride layer.


Figure 7 FESEM image showing the crack nitride as shown in Figure 6.


At this point, the analysis was stopped and a conclusion based on the results from all the analyses was finalized. This is step five in the analysis flow chart.


Failures only occurred under bias in a humid environment. The cause of the failure was the short between the first and second Au metal at a very specific cross-over site under two layers of BCB/inductor structure. The nitride layer was under tensile stress instead of preferred compressive stress.


Unstressed device did not have any nitride crack at the same cross-over location. The failure mechanism was very clear at this point, a nitride stress cracking followed by gold migration.


The next step, step six, was to determine the corrective and preventive action. Two suggestions were made: 1) replace the dielectric cross-over with air-bridge, and 2) replace the tensile nitride layer with a compressive nitride layer. The results were documented and a final report was written and archived in the Reliability Database completing step seven.


As far as the step eight goes, we have to wait for the test of the new design to be completed, before we can really carry out that step.


Similar tests carried out on a nitride plus BCB coated GaAs LNA (Low Noise Amplifier) did not show this failure. This was important data because increasing numbers of circuits fabricated at M/A-COM are being encapsulated in this manner. The problem in the multi-layer transformer was probably from the additional stresses caused by the stacking of multiple BCB layers.


A step by step failure analysis was carried out based on the eight step process developed in M/A-COM Reliability Laboratory. The failed part was a multilayer transformer after environmental stress(85%RH, 85°C, 20V bias for 72 hours). The failure site was at a metal cross-over beneath the BCB/inductor multi-layer structure. The failure mechanism was the stress cracking at the nitride layer followed by gold migration under bias and humid environment. An air-bridge design was proposed and implemented to replace the metal line cross-over.


Compressive nitride was also proposed to replace the tensile nitride.


Authors wish to thank Keith Novaris for his help on liquid crystal and laser cutting experiments, and Elisa Truong for her effort to coordinate the analyses. We are also grateful to Dana Crowe for his encouragement and support to make this analysis and presentation possible.


p 267-277


DOI: 10.1361/cp2000istfa267


Passivation Cracks in a Four-Level Metal Low-k Dielectric Backend Process


Michael C. Olewine, John F. DiGregorio, Gus J. Colovos, Kevin F. Saiz, and Hongjiang Sun


Philips Semiconductors, Albuquerque, NM, USA


Mechanical stress problems in integrated circuit devices are becoming more severe as the number of metal interconnect levels increases and new materials such as low-k dielectrics are introduced. We studied dielectric cracking in a four-level Al-Cu interconnect structure that uses hydrogen silsesquioxane (HSQ), a low dielectric constant (low-k) material. The cracks extended down through the passivation layers to the HSQ layer. For the first time we report on passivation dielectric cracks directly related to the level of residual fluorine in a plasma enhanced chemical vapor deposition (PECVD) reactor. It is shown that a silicon nitride pre-coat deposition removes fluorine (F)from the reactor ambient and prevents the dielectric cracks.


PECVD amorphous silicon nitride films have been used as integrated circuit passivation layers for nearly 20 years. The motivation for using nitride films was the advent of plastic packaging and the need for passivation films impervious to water.


Previous work examined the effects of stress on interconnect reliability in terms of Al hillock formation [1], stress induced voids of Al interconnects [2], and Al intermetallic induced cracks


[3]. The stress of passivation layers is a major contributor to Al stress voids [4]. The primary cause of mechanical stress in interconnect structures is differences in the coefficient of thermal expansion(CTE) [5]. The stress due to thermal expansion differences is given below:


ν


σ


Dep o


T T


Sub


Film


Film Film


TH


dT)


Stress


Where E is the Young’s Modulus, ν is Poisson’s ratio, and α is the coefficient of thermal expansion.


Both E and ν are assumed independent of temperature. The term,E1−υ, is the biaxial modulus.


The temperature difference is between the temperature of deposition and the temperature of testing. The CTE is 24 and 0.3 ppm/ºC. for aluminum(Al) and silicon nitride respectively.


Most work with PECVD silicon nitride films for integrated circuit passivation has centered on reduction of the Si-H bonded hydrogen [6] that can cause traps in the gate oxide, and hot carrier degradation


[7].


The work by Claassen and colleagues at Philips [8]showed the relationship between the deposition conditions of PECVD nitride films and intrinsic film stress. To achieve compressive films low frequency ion bombardment is used. A similar effect can be observed by adding neutral gas species to the plasma such as helium (He) [9]. Jo et al. [10] concluded that more tensile films are susceptible to crack induced failure. More recent work by Ibok et al. at AMD [11]show that silicon nitride films with high hydrogen content were more susceptible to fracture. The addition of oxygen to the films lowered the tendency to fracture. Loboda et al. [12] confirmed the results of other researchers that increasing N-H bond content correlates to increasing compressive nitride film stress. Further they showed that the biaxial modulus was inversely proportional to the total bonded hydrogen content. The highest hydrogen levels produced the lowest biaxial modulus values. A passivation dielectric stack of a phosphosilicate glass(PSG) layer followed by a silicon nitride film had superior resistance to passivation crack failures during thermal cycling of packaged parts [13].


The present work occurred during the development of a four-level metal interconnect strategy designed to meet the demands of an advanced 0.5-µm BiCMOS technology for mixed-signal applications [14], [15].


A key feature of the backend dielectric stack was use of HSQ [16]. HSQ has excellent gap-fill capability and does not require etch-back processing [17].


The prevention of dielectric film cracks was a major concern during process development since a key feature of the HSQ film was superior crack resistance as compared to older siloxane based materials. HSQ produces crack-free films of up to about one micron in thickness [18]. HSQ has a CTE of approximately


20 ppm/ºC. [19]. The intrinsic stress of HSQ is approximately 65 MPa tensile [20]. The use of a PECVD liner deposition (in our case a high refractive index or silicon-rich oxide) prior to the HSQ spincoat was shown to prevent cracking. However, Texas Instruments [21] reported bond pad damage for interconnects incorporating HSQ. They suggested alternative bond pad designs to eliminate bond pad delamination during wire bonding.


Defect Description


Cracking was first noticed on square shaped bond pads that consisted of a stack of M1 to M4 levels of metal. These M1 to M4 bond pads were not allowed by design rules and were only used in special engineering test structures. Later, however, cracking was also observed on design-rule bond pads composed of only two levels of metal, e.g. M2 and M3 or M3 and M4. Cracks were observed only after the alloy process. Bond pad cracking was found on approximately four wafers per lot on about one third of the lots processed. The problem was localized to about one third of the wafer area located opposite the major flat (150 mm diameter substrates).


Figure 1 Decorated Bond Pad Cracks.


Products with up to three levels of metal did not have any cracking. Products that used a thicker three micron (3 μm) interconnect at M4 had more extensive cracks on up to ten wafers per lot. The cracks appeared to originate from the corners of the bond pad. A top down view of bond pad cracks decorated with copper sulfate (Cu2SO4) is shown in Figure 1. The bond pads are approximately 100 µm in size. In some cases only the square-shaped bond pads had cracks. Nevertheless, bond pads with octagonal or hexagonal shapes also cracked. A scanning electron micrograph (SEM) showed that the cracks extended from the passivation films down to the


interface of HSQ and the high refractive index oxide liner (Figure 2).


The outside edge of an M4 to M3 bond pad has a vertical crack about halfway between the metal edge and the right side of the image. The crack extends through the silicon nitride and PSG passivation layers. The M3 dielectric stack has a 400 nm PECVD HRI liner (Refractive Index =1.55) followed by 700 nm of HSQ.


Figure 2 SEM Cross-section of Bond Pad Crack.


The HSQ shown in Figure 2 coats just slightly above the M3 layer HRI liner and is capped by a 500 nm TEOS-based PECVD oxide film. The notch in the TEOS cap glass is caused by the over etch of the M4 etch. The SEM was decorated by an HF dip to highlight the various layers. A 150 nm tungsten (W)CVD layer beneath the Al-Cu metal distinguishes the M3 layer. More complete details of the interconnect system are discussed elsewhere [15].


First Experiments


The cross section SEM data stimulated a series of experiments to determine the extent of cracking.


These included changing the HSQ film thickness, the liner material from HRI to TEOS-based oxide, and thickness of PSG in the passivation stack. None of these experiments produced useful information since the control wafers failed to show any signs of cracking.


Since the cracks appeared only after the alloy process, splits were done on the alloy process itself.


Different temperature ramp rates and a lower alloy temperature were compared to the standard alloy process. The lower alloy temperature eliminated the cracks. However, this solution was not acceptable since the alloy process required a 50º C. higher temperature than the passivation deposition to obtain specific device characteristics.


Passivation Nitride Film Stress


Experiments were done with the nitride film in the passivation film stack. Extreme values of the film stress were produced by changing the level of lowfrequency RF (230 kHz) power during the deposition.


The total RF power (LF and HF) was kept constant.


Since tensile films tend to crack, a more compressive film may be more immune to cracking. The passivation nitride recipe was modified so the proportion of LF RF increased from 25% to 85%. This doubled the compressive stress from 2 to 4X109 dynes/cm2.


Although it was expected that this process change would make the nitride less susceptible to cracks just the opposite occurred (Figure 3). Other wafers processed with tensile stress nitride cracked as expected(Figure 4).


Figure 3 High Compressive Stress


Nitride film Cracks.


The interference fringes in Figures 3 and 4 indicate that the film peeled up from the surface. These wafers had cracking across the entire wafer. Furthermore the unpatterned test wafer ran with the tensile nitride delaminated. Although these wafers had catastrophic cracks, they were clearly not related to the bond pad crack phenomena.


Defect Source Isolation


Examination of processing equipment used for lots with and without cracking showed no single tool linked with cracks. Post alloy inspections revealed that the cracked wafers with were in consecutive order in the cassette. For example the wafer I.D.


numbers were often 24, 01, 02, 03 and 04 corresponding to slots 1 through 5 in the cassette.


Careful investigation revealed that the wafer handling on the passivation tool required that each cassette must have a wafer in the first slot (next the “H” bar).


All wafers were flat aligned in the cassette before processing.


The reactor used for the passivation deposition was a commercially available PECVD system [22]. A key feature of this tool is that the depositions are carried out in multiple steps that generate six interfaces in a stack of seven layers.


Figure 4 Tensile stress Nitride film cracks.


The benefits of this approach are superior film thickness uniformity, elimination of pinholes and higher system throughput.


Our passivation process consisted of two layers deposited as part of the following sequence:


1. Pre-coat PSG deposition for 60 seconds


2. PSG deposition of 300 nm (3 wt.% P)


3. Undercoat of 240 seconds USG


4. Pre-coat nitride deposition 60 seconds


5. Nitride deposition 800 nm.


The purpose of layers 1 and 4 is to lower particulate contamination. Layer 3 prevents process degradation from surface roughening of the showerheads caused by the reactor clean (aluminum fluoride formation)[23]. Only depositions 2 and 5 were deposited sequentially on the wafers. The passivation deposition of PSG and nitride films was performed sequentially without a break in vacuum.


Products with the 3 μm M4 showed a maximum of four cracked wafers per lot. Therefore, a product lot of 24 wafers was split into six groups of four wafers each to perform experiments during the passivation deposition. It was discovered that cracked wafers occurred only when the PSG/Nitride followed a run of thick PSG (2.1 µm). When a PSG/Nitride run was done following another PSG/Nitride run there were no bond pad cracks. This explains why the equipment dependence for bond pad cracking was so difficult to determine – it depended on the previous process run on the tool. The reactor clean from as few as 11 wafers of PSG (2.1 µm) run prior to the PSG/nitride deposition caused passivation cracks. The PSG


process specification allowed as many as fifty (50)PSG wafers to be processed at a time.


The passivation tool was confirmed as the cause of cracking by running the wafers with both flats up and flats down in the cassette. Wafers run with flats up had cracking at the crown whereas wafers run with flats down had cracking near the wafer flat. This conclusively showed that the passivation tool was the source of the bond pad cracks.


Defect Elimination


Since the first wafers processed through the passivation tool had cracks (in the worst case ten wafers for product with 3 μm M4), a set of ten dummy wafers was deposited prior to running the production lot. A full lot of 24 wafers was deposited with 2.1 µm of PSG prior to the experiment. All product wafers following the ten dummy wafer deposition were free from cracks. A control group without the dummy wafers deposition had cracking on the first four wafers processed through passivation. A final test of the containment procedure was performed on products with 3 μm thick M4. All wafers were free of cracks.


Next, the pre-coat deposition times for the PSG and nitride depositions were changed to duplicate the effect of running ten dummy wafers prior to production lots. The nitride pre-coat time was increased from 60 to 400 seconds so the pre-coat time equaled the total deposition time for ten wafers. This was independently tested for the pre-coat of the PSG and the nitride deposition. Only an increase in the nitride film pre-coat time eliminated the bond pad cracking.


Reactor Cleans


The last step in the deposition process is a reactor clean using Zyron®-116 (C2F6) and oxygen (O2). A possible chemical reaction during the reactor clean is:


NF


SiF3


24


N


CO


O


+


→


The reactor uses an endpoint detection system based on optical emission of fluorine, F, to terminate the reactor clean. When the F level increases the reactor clean is terminated following an over etch period.


The tool programming is restricted to using only a percentage of the total etch time as an over etch. In this particular case a ten percent over etch was used.


The reactor clean removes material from both showerheads and a large heater block beneath them that holds the wafers during deposition. The endpoint occurs when the thickness deposited in the


load/unload region of the heater block is removed.


The 2.1 µm PSG process is by far the thickest deposition process run on the passivation tool. A typical end point trace for the reactor fluorine intensity at 704 nm is given in Figure 5.


Time in Seconds


Figure 5 Relative intensity of 704 nm End point


Trace following a Reactor Clean [24].


The intensity drop in the fluorine emission following endpoint is due to changes in the overall plasma intensity as dielectric films are removed from reactor.


Silicon Nitride Cracking Mechanism


A possible explanation for bond pad cracking is the level of fluorine in the reactor following the reactor clean. It is interesting to note that there is a commercially available high density plasma (HDP) tool with a large ceramic surface area that employs hydrogen(H2) plasma to lower the residual fluorine following the reactor clean [25].


The fluorine atoms tend to segregate at film interfaces [26] or at grain boundaries of polycrystalline materials [27]. Williams and Woods [28] demonstrated that fluorine is very mobile at room temperature in silicon dioxide. Fluorine has been shown to diffuse much faster in silicon oxide (3½ times) than in silicon nitride [29]. Kim and Steinbruchel [30]report that F can diffuse through Al in contact with fluorosilicate glass (FSG) at room temperature.


Other researchers studied the effects of fluorine on silicon nitride [31]-[34]. The primary interest of this work was to reduce the hydrogen level in the films.


Other applications include bottom anti-reflective coatings (BARC’s) and ultra-violet (UV) transparent films. However, these investigations were done in single substrate PECVD reactors that produce single layer films unlike the multilayer films used in the present work.


We postulate that cracks originate in the silicon nitride passivation caused by fluorine contamination at the nitride film interfaces during the first depositions following a long chamber clean. For films deposited in these multilayer deposition reactors, the fluorine detected by SIMS analysis [35] is typically on the order 1X1019 atoms/cm3.


Cracks occur on the wafer area opposite the major flat since that portion of the reactor (at the center of the heater block) is in close proximity to alumina(Al2O3) parts used for wafer handling. The porous alumina surface acts as a source of fluorine following the reactor clean. A longer pre-coat of nitride film prior to deposition lowers the partial pressure of the contaminant fluorine to prevent cracking. Figure 6.0 shows the configuration of the reactor hardware in relation to the wafer position. The top-plate and showerhead assembly has been raised for a better view of the wafer position. The tool in Figure 6 is configured for 200 mm substrates.


Figure 6 PECVD reactor from Novellus Systems, Inc.


A question is why the 240 second undercoat deposition of USG does not remove the fluorine from the reactor before the nitride deposition. The reactants used in the nitride deposition are silane(SiH4) and excess ammonia (NH3). Nitrogen is added to improve deposition uniformity but does not participate in the reaction. Ammonia acts as a source of hydrogen to form hydrofluoric acid (HF) that is then pumped out of the reactor. The USG deposition uses SiH4 and an excess of nitrous oxide (N2O). Thus there is a much lower partial pressure of hydrogen present during the USG deposition. This would explain why only an increase in the nitride precoat step could eliminate fluorine in the reactor.


An explanation for how the fluorine causes cracking comes from work done with F-doped grain boundaries of polycrystalline ceramics of silicon nitride and silicon carbide. Pezzotti et al. [36],showed that fluorine-doped Si3N4 composites “had creep rates several orders of magnitude higher compared to the undoped sample. Noticeable variations of both elastic modulus and fracture energy of the composite were detected upon F addition, that were related to a spontaneous process of phaseboundary microcracking upon cooling.” Other work by Park et al. [37] using SiF4 as a fluorine source


produced nitride films more tensile with increasing SiF4 flow rate during the deposition.


Evidence of Fluorine Contamination


The refractive index of the films was measured using a Thermawave Optiprobe® model 5240 on the first through tenth wafers processed through the PSG/nitride deposition following the long reactor clean cycle. The film thickness and refractive index for each film was measured. Figure 7 shows the refractive index data for the first ten wafers process following the long reactor clean.


1.92


1.94


1.96


1.98


2.02


1 2 3 4 5 6 7 8 9 10 Sequential Wafers after a Reactor Clean


Figure 7 Silicon Nitride Refractive Index Trend following a long reactor clean.


The data show an increase in the minimum refractive index while the mean refractive index stays nearly constant. These data were taken from 121 point polar maps with a 3mm edge exclusion. Outlier data from near the wafer flat was excluded from the data set.


Researchers reported a lower refractive index for films with increasing fluorine content [38]. Figures 8 and 9 show contour maps of the silicon nitride refractive index for the first and tenth wafers processed through the passivation respectively. The contour interval is 0.5% or a value of 0.0099. These maps show that the minimum refractive index occurs in the region where bond pad cracks were observed.


Figure 8 Refractive index contour map for the first silicon nitride deposition following an extended reactor clean.


Figure 9 Refractive index contour map for the tenth


silicon nitride deposition following an


extended reactor clean.


A summary of the refractive index data from the contour maps is given in Table 1.


Table 1 Data Summary for Passivation Silicon Nitride film Refractive Index.


MEAN Minimum Maximum First Wafer 1.9840 1.9010 2.0346 Tenth Wafer 1.9898 1.9556 2.0334 Between the first to the tenth wafer not only is the within-wafer uniformity of the refractive index much improved, but also the minimum refractive index in the region opposite the flat has increased. The film stress was calculated from silicon wafer bow measurements using a Tencor Flexus® model FLX2320. The stress for the PSG/nitride passivation film stack following a long reactor clean is presented in Figure 10. The film stress of the first two wafers is more tensile than the subsequent films.


34 36 38 40 42 44 46 48


9 10 Sequential Wafers Following a Reactor Clean


Figure 10 Film stress for PSG/nitride passivation


after an extended reactor clean.


It has been shown that a contaminant (suspected to be fluorine) present in a PECVD following a reactor clean can cause cracks in subsequently deposited silicon nitride films. We believe that this phenomenon has not been reported previously since HSQ makes the BEOL film stack more susceptible to cracking. Furthermore, previous work with fluorinated PECVD silicon nitride films has not used a multi-layer structure. A plasma containing hydrogen following the reactor clean eliminates cracks by lowering the fluorine content of the silicon nitride films.


We wish to gratefully acknowledge the contributions of the engineers, technicians and operators of the Philips Albuquerque FAB organization. The authors particularly wish to thank Steve Smith, Joe Perry, and Steve Nelson for their useful discussions.


1. D.S. Herman, M.A. Schuster, and R.M. Gerber,“Hillock Growth on Vacuum Deposited Aluminum films,” Journal of Vacuum Science and Technology, Vol. 9, No. 1, 1972, pp. 515-519.


2. J. Curry, G. Fitzgibbon, Y. Guan, R. Muollo, G.


Nelson, and A. Thomas, “New Failure Mechanisms in Sputtered Aluminum-Silicon Films,” Proc. IEEE IRPS, 1984, p. 6.


3. R. Shohji, M. Uda, T. Nakamura, T. Yoda, and Y. Itoh, “High-Reliability Tungsten-Stacked Via Process with Fully Converted TiAl3 Formation Annealing,” IEEE Transactions on Semiconductor Manufacturing Vol. 12, No. 3,August 1999, p. 302.


4. K. Tokunaga, and K. Sugawara, “The influence of plasma silicon-nitride passivation film quality on aluminum void formation,” Journal of the Electrochemical Society, Vol. 138, No. 1, 1991,pp. 176-180.


5. B. Greenbaum, A.I. Sauter, P.A. Flinn, and W.D.


Nix, “Stress in metal lines under passivation:Comparison of experiment with finite-element calculations,” Applied Physics Letters, Vol. 58,No. 17, 1991, pp. 1845-1847.


6. A.J. Lowe, M.J. Powell, and S.R. Elliott, “The electronic properties of plasma-deposited films of hydrogenated amorphous SiNX (0 ≤ x ≤


1.2),”Journal of Applied Physics, Vol. 59, 1986,p. 1251.


7. W.H. Stinebaugh, A. Harrus, and W.R. Knolle,“Correlation of Gm Degradation of submicrometer MOSFET’s with Refractive Index and Mechanical stress of encapsulation materials,” IEEE Transactions on electron devices, Vol. 36, No. 3, March 1989, pp. 542-547.


8. W.A.P. Claassen, “Ion Bombardment-Induced Mechanical Stress in Plasma-Enhanced Deposited Silicon Nitride and Silicon Oxynitride Films,” Plasma Chemistry and Plasma Processing, Vol. 7, No. 1, 1987, p. 109.


9. G.N. Parsons, J.H. Souk, and J.Bately, “Low hydrogen content stiochiometric silicon-nitride films deposited by plasma-enhanced chemical vapor-deposition,” Journal of Applied Physics,Vol. 70, No. 3, 1991, pp. 1553-1560.


10. M.-Ch. Jo, S.-K. Park, and S.-J. Park, “Study on resistance of PECVD silicon nitride thin film to thermal stress-induced cracking,” Applied Surface Science, Vol. 140, No. 1-2, February 1999, pp. 12-18.


11. E. Ibok, S. Garg, B. Ogle, T.M. Besmann, M.D.


Allendorf, D. McRobinson, and R.K. Ulrich,“Material, fractural, and optical properties of PECVD silicon nitride and oxynitride film,” 13th International Conference on Chemical Vapor Deposition, 5-10 May, 1996, pp. 470-477.


12. M.J. Loboda, and J.A. Seifferly, “Chemical influence of inert gas on the thin film stress in plasma-enhanced chemical vapor deposited aSiN: H films,” Journal of Materials Research,Vol. 11, 2 February 1996, pp. 391-398.


13. S.-M. Lee and K.-W. Lee, “Optimization of passivation layout structure for reliability improvement of memory devices,” Japanese Journal of Applied Physics, Part1: Regular Papers, Short Notes & Review Papers, Vol. 35,No. 10, 10 October 1996, pp. 5462-5465.


14. A. Pruijmboom, D. Szmyd, R. Brock, R. Wall,N. Morris, K. Fong, and F. Jovenin, “QUBiC3:A 0.5 µm BiCMOS production Technology,” in Proc. IEEE BCTM, 1998, p. 120.


15. R.N. Wall, M.C. Olewine, R. Augur, J.


DiGregorio, and G.J. Colovos, “A New FourLevel Metal Interconnect System Tailored to an Advanced 0.5-µm BiCMOS Technology,” IEEE Transactions on Semiconductor Manufacturing,Vol. 11, No. 4, November 1998, p. 624.


16. FOx®-25 Dow-Corning, Corp., Midland, MI.


17. B.Y. Ahlburn, G.A. Brown, T.R. Seha, and T.F.


Zoes, “Hydrogen Silsesquioxane-based Flowable Oxide as an Element in the Interlevel Dielectric of 0.5 Micron ULSI Circuits,” Proc. 1st DUMIC 1995, p. 36.


18. [18] M.K. Jain, S. Nag, G.A. Dixit, J.D. Luttmer,and R.H. Havemann, “Homogeneous and Multilayer Low-k Interlevel Dielectric Architectures for Capacitance Reduction,” Proc.


of Advanced Metalization & Interconnect Systems for ULSI Applications, 1996, p. 70.


19. H.-C. Liou, and J. Pretzer, “Effect of curing temperature on the mechanical properties of hydrogen silsesquioxane thin films,” Thin Solid Films, Vol. 335, 1998, pp. 186-191.


20. M. Olewine, R. Wall, and G. Colovos,“Integration of Hydrogen Silsesquioxane into an advanced BiCMOS process,” Proceedings SPIE,Vol. 3508, pp. 29-38.


21. M. Saran, R. Cox, C. Martin, G. Ryan, T.


Kudoh, M. Kanasugi, J. Hortaleza, H.


Ibnadeljalil, M. Murtuza, D. Capistrano, R.


Roderos, and R. Macaraeg, “Elimination of Bond-pad Damage Through Structural Reinforcement of Intermetal Dielectrics,” Proc.


IRPS 1998, p. 225-231.


22. E.P. van de Ven , I.W. Connick and, A.S.


Harrus, “Advantages of Dual Frequency PECVD for Deposition of ILD and Passivation Films,”Proc.7th IEEE VMIC Conference, June 1990, pp.


194-201.


23. “Oxide undercoat implementation for SiN and SiON Processes,” Novellus Applications Note,August 1995.


24. “Reactor Clean Characterization for Concept One,” Novellus Applications Note, 1991.


25. Novellus Concept Two SPEED HDP Dielectric Deposition High Density Plasma Process Guide,15-May-98, p. 3-11.


26. Y. Ono, M. Tabe, and Y. Sakaibara,“Segregation and defect termination of fluorine at SiO2/Si interfaces,” Applied Physics Letters,Vol. 64, No. 4, Jan 25, 1993, pp. 375-377.


27. H.J. Kleebe, “Structure and chemistry of interfaces in Si3N4 ceramics studied by transmission electron-microscopy,” Journal of the Ceramic Society of Japan, Vol. 105, No. 6,June 1997, pp. 453-475.


28. R. Williams and R.H. Woods, “Mobile fluoride ions in SiO2”, Journal of Applied Physics, Vol.


46, No. 2, February 1975, pp. 695-698.


29. W. Li and W. Catabay, “ Thermal Stability study of the interconnect system with fluorinated silicate glass as IMD layers,” Materials Research Society Symposium Proceedings, Vol. 476, April 1-4, 1997, p. 261-266.


30. S.E. Kim, and Ch. Steinbruchel,“Metal/fluorinated-dielectric interactions in microelectronic interconnections: Rapid diffusion of fluorine through aluminum,”Applied Physics Letters, Vol. 74, No. 13, 27 September 1999, pp. 1902-1904.


31. C.-P. Chang, D.L. Flamm, D.E. Ibbotson, and J.A. Mucha, “Fluorinated chemistry for highquality, low hydrogen plasma-deposited silicon nitride films,” Journal of Applied Physics, Vol.


62, No. 4, 15 August 1987, pp. 1408-1414.


32. R.E. Livengood, M.A. Petrich, D.W. Hess, and J.A. Reimer, “Structure and optical properties of plasma-deposited fluorinated silicon nitride thin films,” Journal of Applied Physics,Vol. 63, No.


8, 15 April 1988, pp. 2651-2659.


33. N. Watanabe, M. Yoshida, Y.-C. Jiang, T.


7. Searls, D., C. Schuring, W. Hayashida, C.H.


Tan, R. Hardin. “Time Domain Reflectometry as a Component Package Level Damage Detection Tool.” InterPack’99 Proceedings.


June 1999.


8. Odegard, C., C. Lambert. “Comparative TDR Analysis as a Packaging FA Tool.” ISTFA Proceedings. November 1999.


9. Strickland, J. Time-Domain Reflectometry Measurements. Tektronix, Inc. Beaverton,Oregon. (1970).


10. H.W. Johnson and Martin Graham, High-Speed Digital Design, Prentice-Hall Inc. Upper Saddle River, New Jersey (1993).


p 293-302


DOI: 10.1361/cp2000istfa293


Contrast Inversions in Scanning Acoustic Microscopy (C-SAM) of Glue Die Attach


Boris Plikat


Infineon Technologies AG, FA 3 (Failure Analysis), Munich, Germany


The quality of the die attach is crucial for almost all power devices, as in most cases thermal and electrical transport is vertical through the die and its backside.


For glue inspection, C-SAM through the lead frame is widely used. Ordinarily, one of the three following states of delamination is found: (A) no delamination,(B) delamination at the die, or (C) delamination at the lead frame. A general rule for the assignment of the brightness in C-SAM amplitude images to these states of delamination cannot be given. This is evidenced by contrast inversions observed with frequency variation of the applied ultrasound or variation of the glue thickness. Contrast inversions at images through the lead frame occur between areas of states (A) and (B).


The calculation of ultrasonic echoes for a three-layer model (copper, glue, silicon) shows that the contrast inversions are connected to the first resonance of the glue in state (B). Here complicated shapes of the echoes are found in experiments and calculations,which helps to correctly assign brightness levels to delamination states.


Additionally a flow for reliable glue investigation with the use of through-transmission SAM inspection is proposed.


Principle of C-SAM


C-SAM is a pulse-echo method. An electronic pulser excites a piezo-electric element inside a transducer.


Typical center frequencies of the pulses for the investigation of microelectronic packages are 10 to 300 MHz [1]. To record an image, the transducer is scanned across the specimen. At each position, the ultrasonic pulse propagates via a spherical lens into the water couplant and further into the specimen.


Parts of the ultrasonic pulse are reflected at interfaces where the acoustic impedance Z changes. Within the


depth of focus, the reflection at a single interface takes place according to Equation 1 valid for plane waves [2], where R is the reflection coefficient.


Z


The echoes are received by the same transducer and amplified. The time-of-flight into the specimen and back to the transducer depends on the depths of the reflecting interface. Hence echoes from different interfaces are separated in time. A certain interface is selected by gating the echo electronically. The amplitude of the echo inside the gate with the highest absolute value will determine the brightness or colour in the image.


The sign of the echo may or may not be useful for image interpretation depending on the investigated interface. If the acoustic impedance increases at the interface e.g. from mold compound to a lead frame,the reflected echo of a positive incident pulse will also be positive (R > 0). At points of delamination the impedance decreases and the reflected amplitude is negative (Z2 << Z1, R ≈ -1). Hence the echoes from areas of adhesion and delamination are positive and negative respectively. In the case of a decrease of the acoustic impedance at the interface, the echo will be negative regardless of whether there is delamination.


Nevertheless the absolute value of the reflection coefficient in Equation 1 will be higher in delaminated areas. In an amplitude image,delaminated areas will appear brighter than areas of good attachment.


The selection of an interface by gating electronically as described above will only work if the echoes from adjacent interfaces are sufficiently separated from each other. This is not the case for the C-SAM images of glue presented in this paper.


Interpretation of C-SAM Images of Glue Die Attach Recorded through the Lead Frame


G. Pfannschmidt [3] presents C-SAM images of die attach which are thoroughly cross checked with transmission measurements and destructive methods.


She finds three steps of amplitudes in the C-SAM image of the glue. The brightest areas (highest reflected amplitudes) correspond to delaminations of the glue at the lead frame; the areas of intermediate brightness correspond to delaminations on the chip side. The areas of lowest reflected amplitude represent a good attach on both glue interfaces. Latest results show that this interpretation of the reflected amplitudes is not generally applicable. Variations of the frequency of the applied ultrasound or variations of the thickness of the glue may create an inversion of the contrast between the areas of delamination on the chip side and of areas without delamination.


These results show that the direct interpretation of brightness levels in C-SAM images of glue die attach might be a pitfall.


glue


lead frame


die


Figure 1 Schematic cross-section of a package where the mold compound is ground off for the C-SAM investigation of the glue. The scanned incident ultrasonic wave is indicated by the blue triangle.


Grinding and Sealing


With many packages like the SOT223 prepared for this paper, the lead frame is covered with mold compound at its bottom as shown schematically in Figure 1. The attempt to investigate the die attach material through the mold compound and the lead frame usually yields poor or uninterpretable results because of scattering in the mold compound and at the interfaces water - mold compound and mold compound - lead frame. Grinding off the mold


compound greatly improves resolution. The mold compound is removed with silicon carbide paper.


To prevent water from entering the package at the CSAM investigation, the lead frame is sealed. Water would bridge delaminations for the ultrasound and mask delaminations. Ordinary nail polish is used for sealing. A sealed SOT223 package is shown in Figure 2.


Figure 2 A SOT223 package ground


off and sealed with nail polish.


Contrast Inversions and Echo Forms


Silver epoxy glue Epinal 4095 R was used for the die bonding of the investigated parts. Its thickness as determined from a mechanical cross section is 14 μm.


The lead frame thickness after grinding is 150 μm.


C-SAM images were taken with the transducer center frequencies 50 MHz, 75 MHz, 100 MHz and 230 MHz (cf. Figure 3). In the glue images mainly two areas are visible. They are named according to the states of delamination described in the abstract. In the larger area (A) the glue is not delaminated while in area (B) the glue is delaminated at the die. Around the glue the interface between mold compound and lead frame is imaged showing no delaminations.


Looking at the contrast between areas A and B, we find that in the 50 MHz and the 75 MHz image area,B appears darker than area A. In the 100 MHz image the contrast is weak, while in the 230 MHz image the contrast is inverted as compared to the 50 MHz and 75 MHz images.


Below each C-SAM image the echoes (A-scans)corresponding to both areas are given in Figure 4.


The first echo comes from the water - lead frame interface.


Figure 3 C-SAM images of glue through the lead frame taken at transducer frequencies of 50, 75, 100 and 230 MHz.


With increasing frequency a contrast inversion occurs between the area without delamination (A) and the area with delamination at the die (B). The specific location from which all A-scans were taken for Fig. 4 is indicated by a “+”.


TDR uses a low voltage, low current, and very short rise time voltage pulse to determine the impedance of a signal trace as a function of time. With a waveform of trace impedance versus time, not only can the presence of a failure be detected, but the distance along the trace to the anomaly can also be quickly determined.


This paper presents TDR as a useful tool for package level failure analysis labs. The paper proposes one set of solutions for enabling effective TDR analysis(e.g., TDR test fixturing), and discusses some TDR methodologies for detecting and locating anomalies.


The methodologies will be illustrated using three example cases that reflect some commonly used packaging technologies: Flip-Chip Organic Land Grid Array (FC-OLGA), Flip-Chip Pin Grid Array(FC-PGA), and Plastic Land Grid Array (PLGA).


Time domain reflectometry (TDR) is a method for measuring the impedance of an electrical trace as a


function of time. Through these measurements,fundamental information about a trace’s condition can be collected in detail. The technique is already used as a package characterization and design validation tool [1-5]. Only recently have labs begun to use this tool for failure analysis [6], [7]. One benefit of TDR in FA is it can detect a failure and help determine its location within the package. This is in contrast to more common equipment for checking package signal line continuity. Such equipment can usually only detect the presence of a failure. TDR can also detect more subtle failures such as parasitic impedance and capacitance. In addition, TDR testing is entirely non-destructive.


These features make TDR an effective and efficient tool for locating the sources of many failures in component packaging. For more information on the principles behind TDR, see [7], [8].


TDR Setup for FA


Figure 1 is a schematic of a TDR testing system. The two fundamental components are a TDR sampling head, and a digital-sampling oscilloscope. The TDR sampling head generates a low amplitude current pulse, and the oscilloscope measures the reflections from the trace being tested. From these reflections,impedance information can be gathered. The waveform output gives impedance versus time.


Beyond the basic components, excellent fixturing is required to help ensure accurate and reproducible results. The main considerations for proper TDR fixturing include impedance control from the probe tip to the device under test (DUT), good grounding for the DUT, and avoidance of ground loops. Proper consideration of these issues will help avoid unnecessary attenuation of signal energy entering the DUT, ensure proper impedance within the DUT, and allow for stable, accurate and reproducible results.


The fixture should also have a simple user interface in order to minimize the potential for user dependant results. Figure 2 is a schematic for one solution to meet these requirements. In this design, a Land Grid Array type DUT is placed upside down in a formfitting metal cavity, and a grounding plate is placed over top. This plate has holes corresponding to all the DUT’s lands. The package’s ground and power


pads are then grounded to the plate via pogo pins.


Figure 3 is a schematic of the concept for DUT grounding. Figure 3 also illustrates the concept for probing. A coaxial probe is brought into contact with the signal pad of interest through the grounding plate.


The grounding plate thus helps to control the impedance at the probe tip. This simple probe/DUT interfacing method also makes the solution easy to use and ensures consistent probing regardless of the system user. Also, the potential for ground loops is minimized since the large grounding plate will provide the current return path from the DUT to the probe outer conductor.


Digital Sampling Oscilloscope


PC running signal analysis software


Grounding plate


Component fixture


Device under test


TDR test lead


Test lead support TDR sampling head


Figure 1 Schematic of a TDR probing station.


Probe Grounding Plug


Grounding Plate


DUT Holding Plate


Figure 2 Schematic of TDR fixturing solution.


Grounding Plug TDR Coax probe


Device Under Tes


Vss or Vcc Pad Signal Pad


Figure 3 Schematic of a fixturing solution for LGA type packages.


The solution for Pin Grid Array type packages is similar to that of LGA type packages. The main difference is that additional care must be taken to provide impedance control along the pins of the package so that the pin’s impedance matches that of the probe and DUT as closely as possible. Figure 4 gives an example of one solution. An additional plate fits over the package’s pins providing the pin impedance control. This configuration makes the pin-plate interface like that of a coaxial cable with air acting as the dielectric. As such, Equation 1 can be used for determining the proper plate hole diameter:


1 2


r d d


ln


e 60


Z =


Where er is the relative dielectric constant (~1 for air), d2 is the diameter of the plate hole, and d1 is the diameter of the package pins. More information on ground loops,impedance control and other aspects of high frequency signal measurement can be found in [9].


Grounding PlugTDR Coax probe


Device Under Test


Vss or Vcc Pin Signal Pin


Pin Impedance Control Plate


Figure 4 Schematic of a fixturing solution


for PGA type packages.


Figure 5 gives an example of the differences typically seen between this paper’s fixturing solution and a common probe solution. The common probe solution consisted of a coaxial probe with a copper strip connecting the probe’s outer conductor to the DUT ground. The DUT was a PGA package and Equation 1 was used to design the impedance control plate. In Figure 5, the common probe solution shows a 68.6Ω impedance jump at the probe-tip and package pin, and only minor impedance variation within the package. On the other hand, the fixtured trace shows only a 3.5Ω impedance discontinuity at the probe-tip and pin. In addition, the smoothed out humps in the earlier trace show up as more clearly resolved features in the fixtured case. It has also been observed that ground loops caused by the copper strip make reproducibility an issue for the common probe case. This can make analysis(especially automated analysis) more cumbersome.


Open probe


A) Typical probe solution B) Fixtured solution


Figure 5 Comparison between this paper’s fixturing solution and a typical generic probe solution.


Example Cases


During failure analysis, the system will be used to locate continuity problems in a component package.


Failing signal traces will be scanned and their waveforms compared to the corresponding waveforms of a good part. The divergence of the failing wave from the reference indicates the existence of a trace continuity problem. The divergence’s location along the waveform indicates the location of the package damage. Signal velocity is used to estimate the distance along the trace to the problem. Then the location within the product is estimated with the help of relevant layouts. The failure location can also be estimated using comparisons to standards with failures placed at


known locations. Other tools such as crosssectioning can then be employed to determine the root cause of the continuity problem. Without this technique, locating continuity problems can be much more time consuming.


Example 1 – OLGA


The first example illustrates TDR analysis on a C4-OLGA package. The unit was failing for opens on a production line test. The failure analysis engineers were given data indicating which signal lines were failing. TDR was used to isolate the location of the open by comparing the response of the TDR trace to the response of “standard” OLGA packages. One sample was a die-less OLGA substrate, while the other sample had a known open in the trace at the top-most layer. For all cases, the samples were fixtured and the TDR responses obtained for the same trace. Figure 6 gives an example of the results obtained. The figure shows the TDR response for a failing OLGA trace, and for the corresponding standard traces. The data shows the fail occurring soon after the open in the bare package. Therefore the failing location is just after the substrate and may occur in the solder bump or die. The next step was to use the data gained from the TDR analysis as input for physical FA. Cross-sectioning revealed that the source of the open is a missing solder ball (Figure 7).


Good bare package


Failing unit


Standard sample 3F Opens


Figure 6 TDR response for the failing OLGA and the test standards.


Figure 7 Physical FA showing a missing solder ball in the failing trace.


Example 2 – FC-PGA


In this case, the FC-PGA was failing for opens after temperature cycling stress. In the same way as the C4-OLGA example, the failing sample was fixtured and TDR probed. Subsequently, a set of standards were fixtured and probed. The set of acquired TDR waveforms was then compared. The FA engineer used the fail location relative to the standards as shown in Figure 8 to estimate where the open is occurring. Figure 8 gives the results of this FA procedure. Trace (a) comes from a FC-PGA standard with the trace opened in the 1C layer. Trace (b)corresponds to a standard with the trace opened in the 2C layer. Trace (c) belongs to the actual failing sample. The results concluded that the fail occurred between 1C and 2C layers. Armed with this data,physical FA was performed by cross-sectioning at the 1C-2C via. Figure 9 gives the results showing a via crack.


(a) 1C Open


(b) 2C Open


(c) failing sample


Figure 8 TDR response for the failing FC-PGA and the test standards.


Figure 9 Physical FA showing a via crack in the failing trace.


Example 3 – PLGA


The PLGA was failing at functional testing at elevated temperatures (100oC or above). The fail signature was erroneous data on one or more signal lines. Using the tester data, TDR was used to determine if the functional failures were occurring due to package damage. The system was also used to gain insight into why the failures occurred only at elevated temperatures.


The following methodology was employed for the experiment:


1. Fixture a known-good sample and obtain its TDR response for the signal line corresponding to the failing line on the failing sample. This will be the reference trace to which subsequent traces are compared.


2. Using a thermal stream, heat the known good sample to the failing temperature of the test samples. Take a TDR trace of the signal at the elevated temperature. This data point will show how a functional PLGA would respond at the failing temperature.


3. Fixture a failing sample and obtain the TDR response for the failing signal line.


4. Using a thermal stream, heat the failing sample to the failing temperature and take its TDR response.


5. Compare the response of the failing traces to that of the known-good traces and note any deviations.


6. Repeat this procedure as necessary for additional failing signal lines.


7. If anomalies are found, determine where in the package they are located using signal time of flight measurements.


8. Verify the results using whatever appropriate technique (e.g. cross-sectioning, deencapsulating, etc.)


Figure 10 gives the typical response of the known good PLGA at room and 100°C. The image also gives a TDR trace for a probe inserted into an empty fixture. The third trace thus gives the location in time of the probe tip, and is used to locate where the DUT data begins. One can observe some differences between the first two traces, however no gross discontinuities appear. The differences are attributed to changes in material properties in the trace and substrate as the temperature increases. When heating is disengaged, the signal returns to its original state.


Figure 10 Known good unit’s TDR response at


room and elevated temperatures.


Figure 11 gives the typical response of a failing trace at temperatures ranging from room to 100°C. At room temperature, no appreciable differences are observed between the failing and known good trace.


This response does not contradict the functional tester’s data showing that the failing samples functioned at room temperature. However at


elevated temperatures, Figure 11 clearly shows behavior that diverges from a known good sample.


The series of TDR traces show that beyond a point within the package, the impedance gradually shifts upwards with increasing temperature. Eventually, at the failing temperature, the TDR response shows an open signal line. After disengaging the thermal stream, the signal was observed to return to the room temperature state. This data explains the failure signature given from the functional tester. With the TDR system, one can observe in real time how heat affected the signal line and eventually created an open signal at sufficiently high temperatures.


Figure 11 Failing unit’s TDR response at


temperatures varying from room


temperature to 100°C.


Figure 12 gives a schematic of what the TDR data is likely describing at elevated temperatures for this example. The TDR signal enters the package from the probe tip, propagates to a wirebond break and is reflected back. The time difference between the probe tip and the package open is measured as 163±10ps. Using a prior measurement of the signal velocity in the package as 2.02±0.01E8m/s, the distance into the package to the open is measured to be 1.65±0.20cm. Package design data gives the signal length as 1.53±0.0.01cm. Therefore, the area near the package-side wirebond bondpad was


identified as the probable location of the package damage.


Wirebond Break


Signal trace


Distance back to pad


= trace length = 1.53cm TDR Probe


Figure 12 Schematic of failing device trace.


Armed with the above data, the failing package was de-encapsulated and the area around the package-side bondpad inspected. Figure 13 gives the result of the analysis of the bondpad corresponding to the failing signal. The scanning electron microscopic image clearly shows a wirebond break at the package-side bondpad. This data confirms the conclusion reached by the TDR analysis.


Figure 13 Scanning electron microscopic image


confirming damage at the bond pad.


In this example, the FA engineers went from functional failure data to isolating the location of package damage in one quick experiment. Is should also be noted that at the start of the experiment,package damage was only one of numerous possible causes for the functional failure. However using TDR, package damage was quickly found to be the cause. In addition, this example hints at the potential for TDR to be use din detecting anomalies more subtle than straightforward opens or shorts.


Figure 11 shows a TDR response that varies


continuously with temperature between closed and open. One can imagine a case where TDR would be very helpful in finding the failure in a marginally failing unit.


TDR can be a very effective tool for failure analysis at the package level. The tool can quickly provide accurate information to detect and locate package damage. Also, the testing is entirely inevasive, so regardless of the TDR results, the sample is intact for further tests. If TDR does detect a package failure,the data it provides can also be used to locate the damage and direct the focus of further analysis.


These features can in many cases eliminate many steps in the FA process with one quick experiment.


This in turn allows for improved efficiency and much quicker turn around time. In some cases, a series of FA procedures totaling more than two hours can be reduced to minutes.


To make TDR effective as a FA tool, consideration must be placed into system design. Major system design factors focus on the accuracy and reproducibility of results. In addition, gains in FA throughput time should be enhanced as much as possible through the implementation of an easy to use interface. Much of these considerations can be accounted for through thoughtful design of device fixtures. For example, data reproducibility can be accomplished through a fixture that adequately grounds the DUT and carefully controls impedance throughout the probing assembly. Also, ease of use can be greatly promoted through a system with a short setup time, and simple probe to DUT interface.


The examples also suggest avenues for further TDR development. For example, a TDR based system can be envisioned which would augment or replace typical board testers which employ a simple scheme such as forcing current and measuring voltage to test for continuity. Current board testers do not provide location information and can have difficulty finding marginally bad traces. One can imagine an automated TDR system that scans all traces and notes significant deviations from its library of accepted standards. Then, using time of flight data, the location of the anomaly can be measured and displayed graphically on a CAD drawing for the device. Such a system would require robust fixturing to ensure the accuracy and reproducibility needed for automation. These and other possible improvements may further enhance TDR as an effective and time saving FA technique for locating failures in electronic packages.


1. S. Pannala, A. Haridass, M. Swaminathan,“Parameter Extraction and Electrical Characterization of High Density Connector Using Time Domain Measurements”, IEEE Transactions On Advanced Packaging, Vol. 22,No. 1, February 1999


2. Guideline for Measurement of Electronic Package Inductance and Capacitance Model Parameters, JEDEC Publication #123, JC-15 Committee, October 1995


3. M.D. Tilden, “Measuring Controlled-Impedance Boards with TDR,” Printer Circuit Fabrication,February 1992


4. J.M. Jong, B. Jako, V.K. Tripathi, “TimeDomain Characterization and Circuit Modelling of a Multilayer Ceramic Package,” IEEE Transactions of CPMT, Part B, Vol. 19, No. 1,February 1996, pp48-55


5. “TDR tools in Modeling Interconnects and Packages,” – Tektronix Application Note, 1993


6. Dascher, D. “Measuring Parasitic Capacitance and Inductance Using TDR.” Hewlett Packard Journal, April 1996, pp.83-96.


Nomoto, and I. Abiko, “Preparation of Plasma Chemical Vapor Deposition Silicon Nitride Films from SiH2F2 and NH3 Source Gases,”Japanese Journal of Applied Physics Part 2-Letters, Vol. 30, No. 4A, 1991, pp. L619-L621.


34. O. Sanchez, C. Gomezaleixandre, and C.


Palacio, “Role of fluorine-atoms in the oxidation-hydrolysis process of plasma assisted chemical vapor-deposition of fluorinated siliconnitride film,” Journal of Vacuum Science and Technology B, Vol. 11, No. 1, Jan-Feb 1993, pp.


66-69.


35. Unpublished data, T. Mountiser, Novellus Systems, Inc., 81 Vista Montana, San Jose, CA.


36. G. Pezzotti, T. Nishida, H.J. Kleebe, K. Ota, N.


Muraki, and V. Sergo, “Effect of interface chemistry on the mechanical properties of Si3N4-matrix composites,” Journal of Materials Science, Vol. 34, No. 7, April 1, 1999, pp. 1667-1680.


37. Park, Y.-B., S. Rhee, J.-H. Choi, C.-W. Kim, and J.H. Suok, “Fluorinated silicon nitride film deposited at low temperatures from SiH4-SiF4-NH3,” Materials Research Society Proceedings,Vol. 507, April 14-17 1998, pp. 471-476.


38. B.H. Jun, J.S. Lee, D.W. Kim, T.H. Sung, B.S.


Bae, and K. No, “Composition, oxidation and optical properties of fluorinated silicon nitride film by inductively coupled plasma enhanced chemical vapor deposition,” Journal of Materials Research, Vol. 14, No. 3, March 1999, pp. 995-1001.


p 277-283


DOI: 10.1361/cp2000istfa277


Electronic Package Failure Analysis Using TDR


Dima A. Smolyansky


TDA Systems, Inc., Portland, OR, USA


Time Domain Reflectometry (TDR) measurement methodology is increasing in importance as a nondestructive method for fault location in electronic packages [1]. The visual nature of TDR makes it a very natural technology that can assist with fault location in BGA packages, which typically have complex interweaving layouts that make standard failure analysis techniques, such as acoustic imaging and X-ray [2], less effective and more difficult to utilize.


In this paper, I will discuss the use of TDR for package failure analysis work. I will analyze in detail the TDR impedance deconvolution algorithm as applicable to electronic packaging fault location work, focusing on the opportunities that impedance deconvolution and the resulting true impedance profile opens up for such work.


TDR Fundamentals


TDR was initially developed for fault location of long electrical systems, whereas, optical TDR(O-TDR) primarily applies to fault location in optical fiber.


TDR is very similar to X-ray and acoustic imaging techniques in that it sends the signal to the device under test (DUT) and looks at the reflection to obtain the information about the DUT. The difference between X-ray or acoustic imaging and TDR is in the type of signal and the type of propagation media for the signal. X-ray and acoustic imaging use X-ray and acoustic stimuli correspondingly, propagating through the free space and acoustic coupling media to the DUT, whereas TDR uses fast-electrical-step stimulus, delivered to each trace in the DUT via electrical cables, probes, and fixtures. A direct electrical contact between the TDR instrument and the DUT is required to perform the measurement. In addition, not only the signal, but also the ground contact must be provided in order for the TDR signal to provide meaningful information about the DUT


(Figure 1). Without a good ground contact, the TDR path, and the TDR picture will be extremely hard to interpret. signal will not have a good current ground return


Figure 1 TDR oscilloscope measurement setup. Both signal and ground connections are necessary in order for the TDR signal to provide meaningful information about the DUT.


A typical TDR oscilloscope block diagram is shown in Figure 2.


The fast-step-stimulus waveform is delivered to the DUT via electrical cable, probe, and fixture interconnects. The waveform reflected from the DUT is delayed by two electrical lengths of the interconnect between the DUT to the TDR oscilloscope, and superimposed with the incident waveform at the TDR sampling head Figure 2. The incident waveform amplitude at the DUT is typically half the original stimulus amplitude (V) at the TDR source. The smaller DUT incident waveform amplitude is due to the resistive divider effect between the 50 Ω resistance of the source and 50 Ω impedance of the coaxial cables connecting the TDR sampling head and the DUT.


Ztermination


Cable: Z0, td


Rsource


Rsource= 50 Ω Z0= 50Ωthen Vincident= ½V Vincident


Vreflected


DUT: ZDUT


Figure 1 TDR oscilloscope equivalent circuit.


TDR


Instrument


TDR probe with signal and ground


connections


Cable


As the reflected signal is observed in the TDR, one can choose a voltage, reflection coefficient, or impedance mode on the TDR oscilloscope. Either one of these outputs represents the signature of the DUT.


TDR does not provide an optical image of the package, but rather an electrical signature of the trace in the package. Because of the nature of the information that TDR provides, it is important to be aware of typical TDR signatures that correspond to simple package failures, such as a short or an open connection (Figure 3).


½ V


TDR Open


TDR Short


2•tcable


>1000


Impedance


Short


Open


Figure 2 Open and short connection TDR and impedance profile signatures. V is the full voltage amplitude of the TDR step source; tcable is the


electrical length of the cable and probe interconnecting the TDR oscilloscope and the DUT.


TDR measurements always display the round trip electrical delay for the cables, fixtures, and DUTs,which is why Figure 3 displays twice the delay of the cable interconnecting the TDR instrument to the DUT.


The faster the rise time that the TDR interconnect can deliver to the package under test, the smaller the size of the discontinuities that can be resolved with a TDR oscilloscope. Available TDR instrumentation provides very fast rise times; reflected signal rise times of the order of 25-35 ps can be observed at the TDR oscilloscope. However, poor quality cabling and fixturing can quickly degrade the TDR instrumentation rise time and decrease the instrument resolution. I will discuss the TDR measurement accuracy issues in further detail in the section entitled TDR Accuracy Considerations. Additional information about TDR measurement technology and TDR oscilloscopes can be found in references [3]and [4].


TDR Multiple Reflection Effects and the True Impedance Profile


One of the limitations of TDR is the effect of multiple reflections, which is present in multisegment interconnect structures, such as an electrical package. The accuracy of the DUT signature observed at the TDR oscilloscope is dependent on the assumption that at each point in the DUT, the incident signal amplitude equals the original signal amplitude at the probe-to-DUT interface. In reality,however, at each impedance discontinuity, a portion of the TDR incident signal propagating through the DUT is reflected back, and only a portion of this signal is transmitted to the next discontinuity in the DUT. In addition, the signal reflected back to the scope may re-reflect and again arrive at the next discontinuity at the DUT. These so called “ghost”reflections are illustrated on the lattice diagram in Figure 4.


Z0 Z1 Z2 Z3 Z4


Vincident1(1)


Vtransmitted1(1)


Vreflected1(1) Vreflected2(1)


t0 Vreflected1(2)


Vreflected1(3)


Time Direction of forward propagation


Figure 3 Lattice diagram of TDR waveform propagating through a DUT with multiple impedance discontinuities.


As a result of these re-reflections, the signature of the DUT becomes less clear, and additional processing is required using the impedance deconvolution algorithm ([5] and [6]), which is currently not available in TDR oscilloscopes. The impedance deconvolution algorithm deconvolves the multiple reflections from the TDR waveform and provides the true impedance profile for the DUT, significantly improving the clarity of the DUT signature and simplifying further analysis of the TDR data.


For example, in Figure 5 the DUT waveform(dut.wfm) is the TDR waveform of a board trace,going through several impedance discontinuities. The Zline waveform (Zline.wfm) is the true impedance profile waveform computed from the TDR data. It is obvious from the true impedance profile waveform that it is open-ended at the far end, because its impedance goes to infinity at about 2.75 ns. The TDR waveform, on the other hand, appears to continue re-


reflecting back and forth at that time, which in effect is an artifact of multiple reflections. The true impedance profile provides an exact location of the open in the DUT, whereas the TDR waveform by itself provides confusing information about the location of this open. Therefore, the impedance profile provides more accurate impedance readouts and more precise information about the position of possible short and open failures.


The waveform (step.wfm) is the reference short waveform, acquired by disconnecting the TDR probe from the DUT and shorting the signal tip of the probe to ground on a simple conductive metal plate (short reference) or leaving the probe open in the air for the measurement (open reference). Such reference information is required in order to compute the true impedance profile using the impedance deconvolution algorithm, and to properly define the DUT measurement reference plane.


Figure 4 True impedance profile (Zline.wfm) vs. raw TDR data (dut.wfm). Waveforms are offset for display purposes.


Similarly, if a failure analyst technician were looking for an open failure in an electrical package, TDR data by themselves would probably not have been sufficient to locate the position of the failure (Figure 6). In addition, the impedance profile, being an exact signature of the DUT, is relatively easy to correlate to different layers in a BGA package. Such correlation is practically impossible with a TDR waveform alone.


Figure 5 True impedance profile vs. the raw TDR waveform for a BGA package. The true impedance profile provides much more accurate information about the failure location.


An additional advantage that the true impedance profile provides is that it is very easy to evaluate capacitance or inductance of an impedance profile segment using the following equations:


⋅


=2


dt


Z 1


2 1


=2 1


dt)


L


The type of discontinuity (inductive or capacitive)that we observe in the impedance profile, can also be easily identified ⎯ “dips” in the impedance profile correspond to the capacitive discontinuity, and“peaks” correspond to inductive discontinuity. Being able to estimate the value of capacitance or inductance for any given segment can be a significant help in understanding which package segment is being analyzed and in locating the failure more accurately.


TDR Accuracy Considerations


Before discussing package failure analysis techniques using TDR in further detail, it is imperative to note the importance of obtaining a good quality TDR measurement and a clean impedance profile.


Without a good TDR measurement for the DUT and the reference, the true impedance profile is likely to be computed incorrectly, and both TDR data for the DUT and the true impedance profile will provide a confusing picture.


TDR is delivered to the DUT via electrical cable,probe, and fixture interconnects. The quality of these interconnects is the key to obtaining a good measurement. As noted before, poor quality cabling and probes can degrade the TDR rise time and decrease the resolution of the instrument. In addition,when computing the impedance profile, it is necessary to have a clean reference short or open


Zline dut


Step


Zline


waveform; without a good reference, we are not likely to get a clear signature of the DUT. Because of these factors, good quality microwave probes and cables are required to obtain a good quality TDR measurement.


Fixtures, probes, and probing stations for package failure analysis work are available from various manufacturers. A full-featured failure analysis probing station can provide easy viewing and access to the package with a probe, and enable a failure analyst to perform at-temperature analysis of the package failures.


Failure Analysis Goals and Methods


The goal and the task of the failure analyst is to determine whether there is a possible connection failure in the given package trace, and what the exact position was when the failure occurred. Once the position of the failure is determined, further analysis can be performed to determine the physical cause and the nature of the failure, possibly with destructive analysis methods.


Typical approaches that can be used to determine whether there is a failure present are signature analysis, where the package trace true impedance profile data are analyzed for known failure signatures, and comparative analysis, where the package trace data are compared to the data of a trace in a known good package. Both approaches will be applied to the true impedance profile data obtained from the TDR using the impedance deconvolution algorithm.


The true impedance profile provides a much clearer picture of the failure type, and also enables the user to easily determine the exact position of the failure in an electrical sense, i.e., in terms of electrical length of the interconnect in picoseconds. Additional analysis must be performed to determine the physical location(in millimeters or milli-inches) of the failure with the goal of locating the package element that is failing.


The true impedance profile provides the user with a way to correlate the TDR data to the specific layers in the package, as well as provide an estimate of a constant that would allow the user to convert the electrical length in picoseconds into physical lengths in milli inches.


Signature Analysis


In the true impedance profile, open and short failures can be easily identified as 0 Ohm impedance readout for the short and very high (1000 Ohms or more)impedance readout for the open (Figure 3). The exact electrical position of a short or an open can be easily


identified in the true impedance profile, even in the presence of multiple reflections, as previously described.


In the following example (Figure 7), the known good BGA package (ZlineGood.wfm) was analyzed alongside a suspect package (ZlineBad.wfm). The fixture-impedance-profile (ZlineFixture.wfm) is shown for reference. The known good package impedance profile ends with a large capacitive dip,corresponding to the input package capacitance. An open failure is clearly observed in the BGA package at about 80 ps inside the package (160 ps roundtrip delay).


Figure 6 Signature analysis of a BGA package


failure using the true impedance profile.


So called “soft” failures, i.e., partly shorted or partly open leads, can also be identified using the signature analysis, but their impedance profile and TDR signatures must be identified beforehand. The only alternative to knowing the soft failure signature beforehand is to observe the changes in capacitance of the known good device compared to the failing device.


TDR has specific signatures for the open and short connections, as shown in Figure 3, and can also be used for identifying the failures. However, in multisegment structures, such as BGA packages, the exact location of the failure can be difficult to determine because of the multiple reflection effects.


Comparative Analysis


Comparative package failure analysis, as the name implies, relies on comparison of the known good waveform to the suspect waveform. Even though some discrepancy between different measurements may still be observed due to measurement repeatability, the comparative analysis utilizing the true impedance profile waveforms yields very quick and intuitive results.


ZlineBad


ZlineGood


ZlineFixture


Consider the following example. In Figure 7, the package failure is identified as an open failure. In Figure 8, the analysis is continued by comparing the failed waveform to the package substrate waveform only, without connection to the die. The challenge is to determine what package component is failing based on this comparative analysis. Because the failed impedance profile waveform overlays directly over the substrate waveform, it is easy to deduce that the likely failure source is the broken connection between the package and the die. Again, the large capacitive dip is due to the input capacitance of the die.


Figure 7 Comparative analysis for a BGA package.


The bad impedance profile waveform clearly indicates an open failure signature. Comparing it to the package substrate waveform only without connection to the die, allows pinpointing the likely failure source – a broken connection to the die.


Based on this analysis, a failure analyst can focus on the connection to the die area, and use additional failure analysis techniques to determine the physics of the failure.


An important issue when performing comparative analysis is measurement repeatability. Following good general measurement practices, such as:


1. maintaining TDR instrument calibration


2. keeping the instrument well-warmed in a lab with constant ambient temperature


3. maintaining the probe or cable position and spacing between the probe signal and ground during the measurement


will enable the analyst to minimize any nonrepeatability errors. However, a failure analyst must be aware that small differences between different impedance profiles may actually result from measurement non-repeatability, rather than failures in the package under test.


For example, because of the differences between the good package impedance profile (ZlineGood.wfm)and bad package impedance profile (ZlineBad.wfm)in the outlined region of Figure 9, a failure analyst may view the differences between the good and bad waveforms in the selected region as the cause for the failure observed in the later portion of the impedance profile. However, because we are working with the impedance profile and not the TDR waveform, any effect of the reflections in the selected region on the rest of the impedance profile waveform is minimal.


With that in mind, the differences between the two impedance profiles are too small to be viewed as the cause of the failure. And, one can comfortably conclude that the failure occurred in the later portion of the package (in this case, again, it is a failure of the package-to-die connection.)


Figure 8 Measurement repeatability considerations.


The TDR waveform comparative analysis may also yield sufficiently accurate results. However,pinpointing the exact location of the failure may prove to be difficult. For example, see Figure 6.


Additional Considerations for


Package Failure Analysis


The true impedance profile is very powerful because it opens up other interesting venues for FA on electronic packages. For example, because the true impedance profile represents an exact signature of the DUT, one can now analyze the package impedance profile and quite easily correlate it to the physical layers in the BGA package, which can be observed in the package layout or drawing.


Consider the following two package samples with the following simplified trace layouts in Figure 10. The two packages are quite similar, except that the trace leading to the via connecting the package trace to the die is significantly longer for package 1. Both of these packages were analyzed with a TDR instrument


ZlineFixture ZlineSubstrateZlineBad overlays directly over


Zline1Good


and a computed true impedance profile. In both cases a good package sample and a sample with a failure of the connection between the package trace and the die has been analyzed.


Simplified package 1 trace geometry Ball


Trace on


layer 1


Via to die


Simplified package 2 trace geometry Ball


layer 2


Figure 9 Sample package trace geometries used for


correlation to the impedance profiles.


The impedance profile enables a simple correlation to the package geometry (Figure 10 and 11). In package 1, the known good waveform (Zline1good.wfm)shows a segment with inductive behavior (estimated to be about 2nH in inductance), correlating to the long package trace, then a short segment correlating to the via, and then a segment correlating to the input capacitance of the die. When the connection to the die is broken, the corresponding waveform(Zline1bad.wfm) still shows the long trace in the package, but does not go into the capacitance of the die (estimated to be 800fF). Finally, the shorter second package trace correlates to the shorter section in the impedance profile waveform(Zline2good.wfm), whereas for the failed trace in package 2, the impedance profile goes up to high impedance at a much earlier point. The estimates for the inductance of the trace and input capacitance of the die match the expected numbers well, which provides further confirmation for the accuracy of the analysis of the failure type and location.


Once the correlation from the physical package structure to the impedance profile waveform has been determined, the location of the fault in the package can be found easily.


Figure 10 Layer correlation and distance analysis on the impedance profiles of two packages with similar layouts.


In addition, since the overall physical length of the package trace can be quickly found from the package layout, and the impedance profile provides exact information about the electrical length of the package trace, this correspondence can provide a reasonably good estimate of the physical location of the failure.


For example, if the package layout software gives a reading for the overall package trace length of ltotal meters, and the true impedance profile shows that the package length is td total seconds, then the average relative velocity of propagation through the package can be estimated as


total


average


prop


V 1


t l


2)


where VC is the speed of light. For example, the difference between the length of the traces in package 1 and package 2 is 45 ps (90 ps roundtrip). Based on the layout file data, the corresponding physical length is 10 mm, which provides an estimated relative velocity of propagation of 4.5 ps/mm, or 0.74 the speed of light.


In addition, if a correlation between an electrical position in seconds to the physical position in meters needs to be estimated, it can be done using the following equation


d t


l


(3)


Using equation (3), one can estimate the relative poison of the failure within a layer, if it is suspected that the failure actually occurred within a layer.


Clearly, equations 2) and (3) are only estimates. The propagation velocity will vary through


Zline1Good Zline2Good


Zline1Bad Zline2Bad ZlineFixture


the different layers in the package. To get a more accurate value for the propagation velocity one needs to do extensive characterization of the package substrate material, as well as other characteristics.


Such characterization is very time consuming and requires that special test structures be laid out on the material under test. Because of such complexity, the exact data about the velocity of propagation through the separate package layers are rarely available to a failure analyst. A much easier approach is to correlate the layers in the package to the segments in the true impedance profile and use equation 2) to estimate the propagation velocity in each layer.


However, sufficient resolution of the TDR instrument is required to resolve the layers, which can be on the order of 10 ps or less.


An attractive approach for a failure analyst could be to model the package under test, and then attempt to predict the TDR waveform of the package trace via SPICE or full-wave circuit simulations. The problem with this approach is, again, that the properties of the package material must be known with a reasonably high level of accuracy in order to ensure that the simulation predicts the TDR waveform correctly,unless the package model has been directly extracted from TDR measurement.


In this paper, TDR measurement technology is discussed as it applies to the failure analysis of electronic packaging. The impedance deconvolution algorithm is analyzed, and the advantages are demonstrated that the true impedance profile(resulting from applying this algorithm to the TDR data) provides for a package failure analyst over a simple TDR data set, for both signature and comparative package failure analysis. Additional analyses were presented, which can be performed on the true impedance profile, and that can further simplify the location of the failures in electronic packaging.


The author would like to thank Dr. Anil Pannikkat and Mr. Roy Wei-Guang Wu of Altera Corporation for providing package samples, and valuable assistance in performing measurement and data analysis.


1. C. Odegard and C. Lambert, “Comparative TDR Analysis as a Packaging FA Tool,”—ISTFA Proceedings 1999


2. P. Viswanadham, P. Singh, “Failure Modes and Mechanisms in electronic packages,”—Chapman and Hall, 1998


3. M.D. Tilden, “Measuring Controlled-Impedance Boards with TDR,”—Printed Circuit Fabrication,February 1992


4. Time Domain Reflectometry Theory,—Hewlett Packard Application Note 1304-2, May 1988


5. L.A. Hayden, V.K. Tripathi, "Characterization and modeling of multiple line interconnections from TDR measurements,"—IEEE Transactions on Microwave Theory and Techniques, Vol. 42,September 1994, pp.1737-1743


6. D.A. Smolyansky, S.D. Corey, “PCB Interconnect Characterization from TDR Measurements” — TDA Systems Application Note PCBD-0699-02, published in Printed Circuit Design Magazine, May 1999


7. D.A. Rudy, J.P. Mendelsohn, P.J. Muniz,“Measurement of RF Dielectric Properties with Series Resonant Microstrip Elements,” —Microwave Journal, March 1998, pp. 22-39


8. D. I. Amey, S.J. Horowitz, “Tests Characterize High-Frequency Material Properties,”—Microwaves and RF, August 1997


p 285-291


DOI: 10.1361/cp2000istfa285


Time Domain Reflectometry as a Device Packaging Level Failure Analysis and Failure Localization Tool


Damion Searls, Anura Don, Emilie Dy, and Deepak Goyal


Intel Corporation, Hillsboro, OR, USA


Detecting failure in electrical connectivity at the component packaging level is a major expenditure of the industry’s failure analysis (FA) resources. These package failures can result from material/manufacturing excursions, stress tests,and/or customer returns. However, many of the methods employed currently (such as X-ray or crosssectioning) can fall short in terms of throughput time,or success rate. Moreover, many FA techniques can be destructive and therefore leave the sample useless for subsequent tests. On the other hand, time domain reflectometry (TDR) can be used as a component packaging level FA tool which meets the needs of quickly, precisely, and non-destructively locating electrical connectivity problems in signal traces.


Once the failure location has been pin pointed, other FA methods (X-ray, cross-section, etc.) can be used more easily to determine why the failure occurred.


Since TDR testing involves no physical preparation,the sample will be completely intact for subsequent tests.


0,00 0,05 0,10 0,15


50 MHz


t [μs]


75 MHz


100 MHz A


230 MHz A


Figure 4 Echoes (A-scans) from the C-SAM images shown in Figure 3 recorded at transducer frequencies 50, 75, 100 and 230 MHz. The A-scans in the top row stem from area A (without delamination) and the A-scans in the bottom row are taken in area B (with delamination at the die). The corresponding transducer positions valid for all frequencies are indicated in the 230 MHz image in Figure 3. The first echo is the surface echo. The glue echo is plotted in red.


The echo of interest is the second echo, which stems


from the die attach. This echo was in the gate when


the images were recorded (red in Figure 4). Besides


the contrast inversion in the images, we can make the


following observation concerning the form of the


echoes: in the area of no delamination, the glue echo has the shape of a negative echo for all four frequencies, although two glue interfaces are involved. Where the glue is delaminated at the die(area B) a broader echo consisting of four prominent


maxima is found for 50 MHz, 75 MHz and 100 MHz.


Going from low to high frequencies the second maximum increases.


The experimental findings can be summarized as follows: when imaging the die attach layer through the lead frame (die pad), a contrast inversion occurs as the transducer frequency increases. In the area of good die attach, the glue echo looks like a single negative echo, while in the area of delamination at the die, a complicated echo consisting of four maxima is observed. Its shape changes with frequency.*


lead frame (1)


glue (2)


die (3)


β1


β2


β3= 0


α1


α2


α3


Z1


Z2


Z3


d2


Figure 5 Three-layer model with amplitudes αj of the plane waves propagating in positive x-direction and amplitudes βj of those propagating in negative x-direction. The Zj represent the acoustic impedances of the layers. d2 is the thickness of the glue.


Calculations


The Model


As shown in Figure 5 calculations are made for a three-layer model consisting of the lead frame, the glue and the die. Only plane longitudinal waves are taken into account. The wave equation for isotropic media is solved by plane waves.


f


i


j


e


π


β


* Note that the time between the surface echo and the glue echo is shorter in the A-scans of region B than in those of region A. The reason for this is a thickness variation of the lead frame induced by nonparallel grinding.


The coefficients αj and βj are complex amplitudes of plane waves in layer j propagating in positive and negative x-direction respectively. cj describes the corresponding velocities of sound. f is the frequency of the ultrasonic wave. For plane waves the acoustic impedance Zj is given by ρjcj, where ρj is the mass density of layer j. The amplitudes in the lead frameα1 and β1 are those incident from the transducer and reflected back to the transducer. The transfer function or frequency dependent reflection coefficient R of the glue given in Equation 3 describes the phase shift and the attenuation of a plane wave by the interaction with the glue and its interfaces.


)(


1 1


...


ξ


ξπ


αβ


where


= f d2 2


(4)In Equation 4, d2 is the thickness of the glue. The three layers lead frame, glue and die have the acoustic impedances Z1, Z2 and Z3. A delamination at the die is taken into account by letting Z3 be zero. For a delamination at the lead frame additionally the glue thickness is assumed to be zero.


Because R is frequency dependent, and the glue thickness and the mass density of the glue at constant Z2 are frequency independent, resonance curves will be discussed as a function of ξ.


0,0


0,5


1,0


1,5


2,0


2,5


0,0 0,2 0,4 0,6 0,8 1,0


no delam.


delam. @ die


delam. @ lead frame


m = 2d2/λ2 = 2ξ/Re{Z2} [ ]


Figure 6 Resonance curves for three states of delamination, no damping inside glue, Z2= 107 kg/(m2s).


Resonance Curves


If no damping is considered (i.e. if impedances are real for monochromatic plane waves) no contrast inversions with variation of ξ are expected. As shown in Figure 6, with a delamination at any of the glue interfaces the whole amplitude is reflected. In the case of no delamination, losses because of transmission take place. These are maximum if m is an integer in the resonance condition Equation 5.


{ }2


Re 2


Here λ2 is the wavelength in the glue.


Figure 7 Resonance curves for three states of


delamination, with damping inside glue,Z2= (107 + i106 kg/(m2s).


Since the ultrasound is incident from the lead frame,it does not enter the glue if the delamination is on the lead frame side. Therefore the plane wave is reflected without losses even if damping inside the glue is taken into account. As shown in Figure 7, the contrast inversions with variation of ξ occur between areas of good attachment at both glue interfaces and areas where the glue is delaminated on the chip side only. In both cases a part of the plane wave enters the glue. At the backside of the glue (i.e. at the interface to the chip or at the delamination) it is reflected without or with phase inversion respectively. This is why resonances are found at different conditions for these two cases (m integer or m odd multiple of 0.5 in Equation 5). At resonances reflected amplitudes are small due to damping in the glue and transmission into the die or due to damping in the glue only.


In conclusion, for monochromatic plane waves contrast inversions can only be understood if damping inside the glue is considered. In the next section it is shown that for ultrasonic pulses, contrast inversions can be explained without damping inside the glue.


Calculation of Echo Forms


Since C-SAM does not work with monochromatic waves but with pulses of ultrasound, their spectra have certain widths. In the following, pulses with a Gaussian envelope according to Equation 6 are assumed.


τ


cos


(6)


Here f0 is the center frequency of the pulse, and τ a time constant which determines the pulse length. The reflected pulse forms are calculated by multiplication of the Fourier transform of the pulse in Equation 6 with the transfer function of the glue in Equation 3 and subsequent numerical inverse Fourier transformation.


-1 0 1


incident


Figure 8 Calculated pulse forms for τf0 = 0.5, Z2 =107 kg/(m2s) at the first resonance of the glue if delaminated at the die (m = 2d2/λ2 = 1/2).


Like with the discussion of the resonance curves, in the following, ξ0 = f0d2ρ2 will be used instead of f0, d2 or ρ2 separately. The pulse width can be expressed in terms of the period 1/f0 by τf0. For the pulse forms shown, τf0 = 0.5 is chosen. On the very left of Fig. 8 the incident positive pulse is plotted. On the opposite side the echo from a delamination at the lead frame(C) is shown which simply is the incident pulse inverted. These pulses are the same for all parameters of the glue since the glue is not involved. In the center of Fig. 8 the echoes in the case of no delamination (A) and in the case of a delamination at the die (B) are represented. These echoes will change with variation of the impedance, Z2 , of the glue and of ξ0 = f0d2ρ2 as can be seen in Figure 9.


From top to bottom in Figure 9, ξ0 increases corresponding to an increase of the frequency f0 as in the experiment. Throughout the whole interval of ξ0,the first minimum in the echo is predominant if the glue is not delaminated. For a delamination at the


die, the first minimum dominates at small ξ0. In the first resonance of the glue with a delamination at the die where d2 = λ2/4 or m = 0.5, a broader echo consisting of about four predominant maxima appears. Here the highest amplitude in the echo is small. With increasing ξ0 the second maximum grows. At d2 = λ2/2 or m = 1 two minima are separated by this maximum. Although a direct comparison with the experiment will be tried later in this paper we can state at this point that the above findings are consistent with the experimental data shown in Figure 4.


-7,2-6,0-4,8-3,6-2,4-1,2 0,0


delamination @ die


d=7λ/16


d=λ/2


d=3λ/8 d=5λ/16 d=λ/4


d=3λ/16 d=λ/8


no delamination


Figure 9 Calculated pulse forms for τf0 = 0.5, Z2 =107 kg/(m2s) for the case of no delamination (A) and of delamination at the die (B). From top to bottom ξ0 increases. The red and blue arrows indicate the time and sign of single interface echoes from multiple reflections inside the glue whose superposition is the complete echo.


The pulse forms in Figure 9 can be understood as the superposition of multiple reflections inside the glue.


At each reflection the single pulse changes its sign or not as determined by the reflection coefficient in Equation 1. This leads to a sequence of positive and negative echoes represented by blue and red arrows in Figure 9 with decreasing amplitudes. Looking at the right column we see that for small ξ0, the first two negative echoes from the interface lead frame - glue and the delamination at the die side interfere constructively while the later echoes of alternating sign interfere destructively. This leads to a strong


minimum at the beginning of the superimposed echo.


At the first resonance (d2 = λ2/4 or m= 0.5) this order is inverted in the sense that the two negative echoes at the beginning interfere destructively, while the later echoes reinforce each other as expected for a resonance. As a consequence, a broad echo with small amplitudes at the front occurs. At even higherξ0, with d2 = λ2/2 or m = 1, the two negative single pulses start to separate. A similar analysis can be made for the left column.


-0,2 0,0 0,2 0,4


Impedances Z2 [106 kg/(m2s)]:4


ξ0 [106 kg/(m2s)]


Figure 10 Amplitude contrast from calculated echoes for different impedances Z2 of the glue. The arrows indicate the first resonance of the glue with


delamination at the die (m = 0.5).


Calculated Amplitude Contrast


C-SAM images of the die attach recorded through the lead frame are amplitude images. The brightness in the image is assigned according to the highest absolute value in the gated part of the echo (A-scan)as described in the introduction. With amax and bmax being these values for delamination states A and B respectively, the amplitude contrast is calculated corresponding to Equation 7.


max


(7)


In Figure 10 the amplitude contrasts for three different impedances of the glue are plotted as a function of ξ0. In the vicinity of the first resonance of the glue (m = 0.5), the amplitude contrast k is negative, which is plausible with the considerations of the previous section. Around m = 1 it becomes positive again. Here the first pulses from the front and the backside of the glue begin to separate.


Because they still interfere constructively in the case of a delamination at the die and destructively in the case of no delamination, the amplitude contrast is positive. With even higher values of ξ0, the interference of the echoes from single interfaces vanishes and with it the amplitude contrast. If a


broader incident pulse (e.g. with τf0 = 0.75) is used for calculations, this interference vanishes at higherξ0, and a second contrast inversion at m = 1.5 occurs.


If the interference of subsequent single interface echoes can be neglected, these echoes can be gated separately and be interpreted in the standard way again.


Comparison of Calculated and Experimental Echoes


Characteristic Echo Forms and Contrast Inversion


The discussion of the calculated pulse forms on the basis of Figure 9 confirmed that the experimental CSAM images in Figure 3 are recorded in the vicinity of the first resonance of the glue (m = 0.5) and at higher frequencies. Like in the simulation, with good attachment on both glue interfaces the glue echo consists of one dominant minimum. With a delamination at the die, a broader echo consisting of about four maxima is found where the second maximum increases with frequency. The calculation also reproduces the contrast inversion near the first resonance of the glue.


For direct comparison of experimental and calculated echoes, values of the impedance Z2 of the glue and ofξ0 where both echoes seem to fit best were sought. Z2 is varied in steps of 106 kg/(m2s) and ξ0 in steps of 105 kg/(m2s). For τf0 0.5, 0.75 and 1.0 are used. In Figure 11 the calculated echoes assigned to the experimental “by eye“ are plotted. On the very left the center frequencies of the applied transducers are indicated. The echoes on the right hand side are calculated with the same parameters as those in Figure. 9 (τf0 = 0.5, Z2 = 107 kg/(m2s)) but for different values of ξ0. Since the calculations are not made for distinct frequencies but for certain values ofξ0 = d2ρ2f0, the time base in terms of the period of the pulse is fixed.


Already in the experiment the echo from a delamination at the die is not exactly a symmetric inverted Gaussian pulse with the same width as in the calculation. Hence a very close similarity of experimental and simulated echoes cannot be expected. Even with the use of the correct incident pulse form, factors such as mode conversions and interface roughness will introduce deviations between experiment and calculation.


0,05 0,10 0,15


-768-512-256


0 256


Calculation


230 100 75 50


-4,8-3,2-1,6 0,0


f0tr


[MHz]


4,4 3,8 2,8 2,7


ξ0[106 kg/(m2s)]


Figure 11 Direct comparison of experimental echoes taken in the area of delamination at the die with calculated echoes.


Frequency Down Shift and Its Implication on Calculations


If for the experiment the center frequency of the transducer f0tr was the same as in the recorded echoes(A-scans), f0tr and ξ0 = d2ρ2f0 should be directly proportional to each other, because d2ρ2 is constant throughout the experimental frequency variation. As can be seen in Fig. 11, a direct proportionality is not observed. This is due to the frequency down shift induced by the frequency dependent damping of the ultrasound in the water couplant and in the specimen itself [1]. For the given experiment, damping in the water is dominant where the absorption coefficient increases with the square of the frequency. The down shift of the center frequency of the ultrasonic pulse is the stronger the bigger the focal length of the transducer, the narrower the original pulse, and the higher its center frequency. In a realistic case a pulse emitted at 100 MHz can be received as a 30 MHz pulse. The center frequency of the pulse at the specimen will be somewhere in-between. With frequency also the shape of the pulse will change.


Also, if the received echo is very different from the one actually interacting with the glue, the above calculations make sense. As long as all modifications of the spectral components of the echo reflected by the


glue are independent of their amplitude, they can be described with a transfer function T(f). The product T(f)R(f), with the transfer function R(f) of the glue as given in Equation 3, will give the overall transfer function for the pulse with the spectrum η(f) incident on the glue. The received echo will correspond to T(f)R(f)η(f). All considerations remain correct if we assume T(f)η(f) to be the spectrum of the pulse incident on the glue, which is then only modified by the transfer function R(f) of the glue. The echo received from a delamination at the lead frame corresponds to -T(f)η(f) since in this case R = -1.


As a consequence of the frequency down shift one can not move through the resonances of the glue by simply shifting the transducer frequency by the same relative amount as the desired change of m in Equation 5.


Practical Work


Investigation of Glue Die Attach Through the Lead Frame and Contrast Inversions


As discussed in the above sections, a direct assignment of brightness levels in an amplitude image to states A (no delamination) and B (delamination at the die side) is not possible a priori. According to simulations, an area delaminated at the lead frame(state C) will not have a lower brightness than any of the other two states, regardless of frequency.


Broad echoes in A-scans in dark areas of the image hint at glue that sticks to the lead frame but is open at its backside, i.e. delaminated at the die or fractured.


Also, if almost no contrast is visible the broader echo will point at an open backside of the glue. This corresponds to the situation in the C-SAM image in Figure 3 taken with the 100 MHz transducer.


Occasionally, the contrast inversion even occurs in an image because of the wedge shape of the glue. In both cases a change of the transducer might produce better contrasts. If the thickness of the lead frame is sufficiently homogeneous, also gating the tail of the glue echo will work and give a bright contrast only in the area of a delamination at the die.


reflection from top


reflection from bottom


transmission


Figure 12 Glue investigation by a transmission


measurement before grinding.


Complementary SAM-Methods


Two major problems arise in connection with investigating the die attach through the lead frame.


One is the difficulty of unambiguously interpreting the observed contrasts, especially if the whole image is homogeneous, which frustrates the attempt to learn from comparisons. The second is the risk of introducing additional delaminations during preparation. This will mainly happen if the glue is already largely delaminated before preparation.


For packages similar to the one outlined in Figure 12,transmission measurements are frequently helpful in this situation if the chip topside and the lead frame bottom both have a good attachment to the mold compound. Then the transmission measurement carried out before grinding can already give a low resolution image of the die attach, since then the ultrasound will only be blocked on its way from top to bottom through the package if there is a delamination at the die bond. At these areas the transmission image appears dark. A reflection image recorded simultaneously with the transmission image will help to assign positions to the different areas of the low-resolution transmission image. It turns out that the transmission images are of sufficient quality only if a small diameter unfocussed transducer, or a focussed transducer, is used as the receiver [5]. If the low resolution of the transmission image is satisfactory and (in the case of delaminations) the information about the delaminated glue interface is of no interest, analysis can be stopped at this point. The three images necessary for this first part of the glue investigation are shown schematically in Fig. 12.


These include a reflection image from the bottom and one from the top, to check the attachment between mold compound and the bottom of the lead frame and between the mold compound and the topside of the die respectively. The third is the transmission image.


For a P-DSO-8-6 package these images are presented in Figure 13 and Figure 14. In Figure 13 both images are taken with a 75 MHz transducer. Positive echoes are represented in blue and negative echoes in red corresponding to an attachment and a delamination.


The top of the die as well as the bottom of the lead frame show a good attachment to the mold compound. Note that dimples in the lead frame disturb the image from the bottom. The left image in Figure 14 is a transmission image of the same package. The contrast in the area of the die indicates that more than half of the die bond shows good transmission (bright) corresponding to attachment. In the reflection image on the right hand side the red colour in the area of the die is not due to a delamination on top of the die. It is caused by interference of the echo from the top of the die with the echo from the delamination of the die attach.


Figure 13 Left: C-SAM image of the interface between mold compound and lead frame bottom.


Right: C-SAM image of the interfaces between mold


compound and die or lead frame.


Figure 14 Transmission image (left) of the package in Figure 13 (30 MHz transducer). The blue rectangle indicates the position of the die as measured in the reflection image on the right taken simultaneously.


Since at transmission images the ultrasound has to cross the whole specimen and a long path in the water couplant, absorption is comparatively high. This is compensated for with the use of lower frequency transducers, e.g. 30 MHz. As a consequence, in the simultaneously acquired reflection image shown in Figure 14, the positive echo from the top of the die interferes with the negative echo from its bottom. In this example the negative part from the bottom of the die overbalances the positive from its top in the area


of the glue delamination. The occurrence of this effect depends on and is very sensitive to focussing and other parameters such as the thickness of the die.


Hence it can serve as a hint on a delamination of the glue but might also not appear even if the glue is delaminated completely.


For the second part of the glue investigation the device is prepared as described in the experimental section. To check for preparation-induced delaminations of the glue, the transmission measurement shown in Figure 14 is repeated.


Figure 15 Reflection image of the glue


(75 MHz transducer) recorded through the lead frame for the same specimen as shown in Figures 13 and 14 The bright fringes at the edges of the image stem from the sealing of the lead frame. Also shadows caused by the dimples in the lead frame bottom are visible.


Then a reflection image of the glue is recorded through the lead frame as shown schematically in Figure 1. The experimental example is shown in Figure 15. This image has better resolution than the transmission image. The border of the glue is visible as a thin line. Additionally we can decide which delamination states are present by combination of different images.


As known from the reflection image from the top in Figure 13 and Figure 14 the interface between mold compound and lead frame is delaminate on the right hand side in Figure 15. In the reflection image through the lead frame, the echo has the same form and amplitude at this delamination outside the area of the die and in the bright area within the die. We can assume that the delamination at the lead frame reaches into the glue die bond.


In the dark area within the borders of the die in Figure 15 the glue is not delaminated. This is evidenced by the transmission image. Consistently no broadened echo is found.


* For the reflection image in Fig. 15 the part has been turned upside down. Left and right sides have changed.


Further Methods


Also X-ray images and physical destructive methods like mechanical cross sections and a lead frame lift off are useful in the investigation of the die attach.


Voids in the glue are indistinguishable from delaminations at the lead frame in C-SAM images through the lead frame. In X-ray images voids in the glue are visible while delaminations are not.


The thermal coupling between the die and the lead frame correlates with the degree of delamination of the glue [4]. It can be measured via the shift of the source drain voltage at the inverse biased diode of the power MOS-FET before and after electrical heating.


Another measurement uses the shift of the gate source voltage necessary to maintain a certain drain source current while the device is heating up.


To investigate glue die attach, C-SAM through the lead frame is widely used. Contrast inversions with frequency variation are observed between areas with no delamination and areas with a delamination at the die. Hence an a priori assignment of brightness levels to delamination states of the glue is not possible.


With contrast inversion typical changes of the echo form arise in areas of delamination at the die.


Assuming a symmetric incident pulse with a Gaussian envelope, reflected echoes are calculated on the basis of a three-layer model (copper lead frame, glue,silicon die) for three states of delamination. These are(A) no delamination, (B) delamination at the die and(C) delamination at the lead frame. The contrast inversion as well as the forms of the echoes observed with the inversion are reproduced. The contrast between areas of states A and B is inverted in the vicinity of the resonances of the glue in state B. Only the first of these where the thickness of the glue is a fourth of the ultrasonic wavelength is of practical relevance. Here a broadened echo consisting of four maxima occurs. The second maximum increases with frequency. A delamination at the lead frame will never appear darker than the other two states.


Although the observation of typical echo forms helps in many cases to interpret C-SAM images of glue die attach through the lead frame, in others the contrasts will still be a puzzle. A second problem with this method of glue investigation is the introduction of additional delaminations through preparation. Often these two problems can be overcome by the combination of different C-SAM methods.


For the investigation of the die attach, transmission images might help to check for preparation-induced artefacts by measurements before and after preparation and to assign brightness levels at a reflection image of the glue through the lead frame to delamination states. A requirement for the usefulness of transmission images is that all interfaces underneath or above the glue do not block the ultrasound. If a delamination extends from the area around the die, as will be known from a comparison with the reflection image from the top, identical brightness and echo forms in both areas are consistent with a delamination of the glue at the lead frame.


Additionally, the knowledge of the resonance properties of the glue as discussed above can be used to understand the state of the glue. To enhance image contrast and reliability of contrast interpretation, the first glue resonance can be sought by suitable change of the transducer. In general the comparative investigation of a device with known properties is recommended.


I very much appreciate the fruitful discussions with my C-SAM teacher Gaby Pfannschmidt at Infineon Technologies. Also many thanks to Sonoscan for their expedient help with the through-scan-arm.


1. S. Canumalla, IEEE Transactions on Components and Packaging Technology, 22(4),1999, 582-592.


2. J. Krautkrämer, H. Krautkrämer,Werkstoffprüfung mit Ultraschall, Springer Verlag, Berlin etc., 1986.


3. G. Pfannschmidt, Proceedings of IAMIS(International Acoustic Micro Imaging Symposium), International Acoustic Micro Imaging Society, San Diego 1996, without page numbers.


4. G. Pfannschmidt, Quality and Reliability Engineering International, 8(3), 1992, 243-246.


5. T. M. Moore, C. D. Hartfield, Proceedings 23rd Int. Symposium for Testing and Failure Analysis,1997, 197-204.


p 303-306


DOI: 10.1361/cp2000istfa303


Application of Scanning Acoustic Microscopy to Electric and Electronic Parts


C. Miyasaka and B. R. Tittmann


Department of Engineering Science and Mechanics, Pennsylvania State University, PA, USA


Figure 1 Schematic of Input.


Electrical Characterization


I/O Leakage Measurement from Pad


Electrical characterization at pad level was done to verify the I/O leakage failures. Figure 2 shows the I/O leakage for the same conditions as the LSI tester measurements. The conditions are shown in Table 1.


The leakage value was same as measured with the LSI tester.


Figure 3 shows the characteristics of pad-GND,which is normal and figure 4 shows the characteristic of pad-V1, which has a short.


From these results, the following modes were considered most likely as the cause of the input leakage:


1. A short between an input pad and V1


2. A leakage path from input pad to V1 through a PFET of one of the protective devices


Table 1 I/O leakage measurement.


Figure 2 I/O leakage at pad.


Figure 4 Pad – V1 characteristic VP = -3.5V to 3.5V (sweep)


Planar Polishing and Internal Probing


Optical observations with planar polishing made clear that M4, M3, M2 and M1 were normal. There was no short between the input line and the V1 line. The cause of the failure was suspected to be leakage through a P-FET of one of the protective devices. The connections of the input circuit were analyzed.


Figures 5 and 6 show the M1 level optical image of the input circuits. Figure 7 shows the optical image of the P-FET after M1 was removed. Figure 8 is the schematic of input circuit that was composed of M1 and a poly-Si gate. At the M1 level, the common source of the P-FETs can be divided into several sources, and most of the P-FETs are connected in parallel in pairs except at each end.


Figure 5 Optical image of Input after M2 removal.


Figure 6 Optical image of Input after M2 removal(higher magnification).


The static characteristics of each P-FET pair were measured one by one with internal probing. Figures 9, 10 and 11 show the measurement results. The conditions of the measurements are shown in Table 2.


Current through a good P-FET pair is shown in Figure 9. It is twice as much as from a single P-FET,which is shown in Figure 10. However, for a bad PFET pair, as shown in Figure 11, the current flow is only half the current of a good P-FET pair. To sum it


up, the current of the failed P-FET pair is equal to a single P-FET. This result reveals that one gate of the bad P-FET pair did not turn 'on'.


Figure 7 Optical image of P-FET after M1 removal.


This indicated that a floating gate caused the input leakage failure, and it was suspected that the cause of the floating gate was an open W stud defect, where the stud connects M1 to the gate.


Figure 8 Schematic of Input at M1 level.


Table 2 Static characteristic of P-FET


Figure 9 Static characteristic of good P-FET pair.


Figure 10 Static Characteristic of single P-FET.


Figure 11 Static characteristic of fail P-FET pair.


Cross-sectional Observation (SEM)


A cross-sectional SEM image of the suspicious contacts was made to confirm the open defect. The sample was prepared by mechanical polishing.


Figure 12 shows the result. It was found that there was a space between the bottom of M1 and the top of the W stud. Part of the space was filled with FM,


which from its contrast seems to be an organic material. This result made it clear that one of the suspicious contacts was open and this caused the gate to float, but it was unclear whether the FM was originally inside the space or if it was debris from the mechanical polishing.


Figure 12 Cross sectional SEM observation.


Detailed Cross-sectional Observation(TEM)


Another open stud was isolated using the same method. This time a TEM specimen was prepared by using FIB to examine a cross-section without artifacts from mechanical polishing. Figure 13 shows the image of a gap. There was a gap at the interface between the Ti liner of M1 and the W stud, and the FM was clearly observed inside the space. The Aluminum (Al) grains and Al3Ti grains appeared normal. From these results, it seemed that the open was traceable to the W CMP process.


Figure 13 Cross sectional TEM observation.


W CMP Process Description


Following are the process steps of the W CMP process. Figure 14 shows a schematic view of each step in W-CMP.


Figure 14 Schematic of cross sectional W-studs explaining W-CMP process.


1. W polishing: Polishing W by CMP (Chemical Mechanical Polishing).


2. Rough brush cleaning: Cleaning with an organic brush after W polishing.


3. Oxide touch up: Polishing only oxide adhering to W studs.


4. Final brush cleaning: Final cleaning with organic brush.


FE-AES Analysis of Cross-section Using FIB Preparation


FE-AES analysis was performed with an FIB crosssectional preparation to clarify the composition of the FM. FE-AES can do elemental analysis and detects changes in chemical composition with high spatial resolution [(x,y,d); (20 nm, 20 nm, 20 •)]. Another open stud was isolated using the same methods as before. A fresh cross-section of the gap was necessary for accurate chemical analysis. For accuracy, it is also important to detect sufficient


numbers of Auger electrons from a sample.


Therefore, a large cross-section including the open stud was prepared by FIB milling. The crosssectional SEM image made using FE-AES is shown in Figure 15. The specimen was tilted at fifty degrees.


An Auger survey spectra was obtained from the cross sectional surface of the FM after Ar sputter cleaning.


The survey spectrum is shown in Figure 16. Oxygen(O), carbon (C), phosphorus (P), silicon (Si), Al, Ti and W were detected.


Figure 15 Cross sectional SEM Image of the open


stud by FE-AES (tilted at 50 degrees).


Note A allow indicates the FE-AES analysis point.


Figure 16 FES-AES survery spectra at the surface of the FM.


Considering the high spatial resolution of FE-AES,there was little likelihood of detecting Auger electrons that were generated from elements located far from the analysis point. However, Al, Ti, W can be ignored, because they are the materials of the metal lines themselves. Therefore, O, C, P, and Si were considered to be the elements making up the FM.


FE-AES Analysis at the Interfaces Using FIB Flat Milling Preparation


It was necessary to perform an FE-AES survey analysis at the interfaces to verify the result of the cross sectional FE-AES analysis. Therefore, another open stud was isolated in the same way as before. M2 was polished off and the surface of the specimen was an interlayer of dielectric film on M1. If argon (Ar)sputtering with FE-AES is applied for a long time to mill the dielectric film down to the M1 interface, the sputtered surface becomes rough, and the Auger spectra at the interface loses its clearness and accuracy. In that condition, it is also impossible to analyze very small areas. To avoid these problems,FIB’s flat and wide milling technique was used down to the middle of M1.


Figure 17 shows the SEM image obtained by FEAES after FIB milling. Stud #1 shows at higher contrast than Stud #2. It seemed that Stud #1 was observed through M1 and the gap.


Figure 17 SEM image by FE-AES. Note: Arrows


indicate the FE-AES analysis point.


Figure 18 Schematic of cross section at Stud #1.


Note: line A,B,C indicates the analyzed Interfaces.


The analyzed interfaces are shown in Figure 18.


Figures 19, 20, and 21 show the Auger survey spectra as each interface was exposed through Ar sputtering.


Checking the spectra against structure of the metal line (M1), it was clear that the Al and Ti peaks were taken from the material of the metal line. When the Ti peak began to decrease, O, C, P, Si, and W peaks began to appear, and in particular the O peak was very strong. These elements must not exist in the interfaces. The Auger chemical analysis also showed a shift of the Al peak at this time. It was clear that Al oxide, O, C, P, and Si surely existed at the interface between the Ti liner and the space above the W stud.


This result agreed with the cross-sectional FE-AES analysis result. The FM was composed of organic material, aluminum oxide, phosphorus compound,and Silicon compounds. These materials seemed to be traceable to the slurry and brushes used in the W CMP process.


Figure 19 Auger survey spectra at interface A.


Figure 20 Auger survey spectra at interface B.


Figure 21 Auger survey spectra at interface C.


Reproduction Experiments on W-CMP Process


Problem reproduction experiments and inspections were performed on the W CMP process in the manufacturing line after the failure analysis results had been fed back into the process. It was determined that the unexpected chemical reactants were adhered to the raised edge between the W studs and PSG during the oxide touch up process. It was also found that when the oxide touch up step took more time,more reactants were stuck to the wafer. An SEM image of the excess reactant chemical is shown in Figure 22. An FE-AES spectrum of the reactant is shown in Figure 23. Although the electrical chargeup process disturbed the obtained Auger spectra, O and C were certainly detected from the surface of the reactant. This confirmed that the reactant consisted of organic materials, in agreement with the earlier failure analysis results.


Figure 22 SEM image of the reactant.


Figure 23 FE-AES spectra at the surface of the reactant.


The I/O leakage failures were caused by floating gates, specifically by open W studs. Cross-sectional SEM and TEM observations showed gaps between the M1 Ti liner and the W studs. FM was found inside the gap. The FIB process was used for sample preparation, so that cross-sectional and planar FE-ES analyses could be used to identify the elements of the FM. Problem reproduction and inspection in the WCMP process confirmed that chemical reactants containing organic matters were stuck around contacts during the oxide touch up process.


These results revealed that the W-stud open faults were traceable to the chemical reactants that stuck to uneven edge between the W studs and the PSG film during the oxide touch up process. The composition of the reactants was identified to be slurry, PSG debris, and organic materials such as brush fibers.


The root cause of the stud open failures had been identified.


The mechanism producing the open W studs was to postulated to be as follows: Leftover reactants remained on the uneven edge between the W stud and the PSG during the W CMP process. Gas was generated from condensation and degeneration of the reactants during subsequent thermal processes. The M1 layer was pushed up by the gas, forming the gaps that caused the stud to be disconnected.


The analysis results were fed back into the W CMP sector. As a result ,the material of the cleaning brushes was changed from nylon to PVA (polyvinyl acetate), and the oxide removal quantity was reduced.


The process yield had been improved by these actions, showing that the open stud defects were the main cause of the low yield.


I/O leakage analysis using various analytical instruments was able to reveal the root cause of yield problems, which turned out to be in the W CMP process for this component. The failure mechanism was discovered using of FE-AES on samples prepared using FIB to achieve high accuracy of elemental analysis in microscopic areas.


The authors would like to thank the following people for their important contributions:


Nobuhito Miura, Akira Nishikawa, Naoko Katoh,Ryuji Kanehara, and Masumi Miyaki.


p 323-326


DOI: 10.1361/cp2000istfa323


Integrated Circuit SNR improvement using Dielectric


Altering Compound, Laser Trim, and FIB system.


B.J. Dutt, J.J. Kroutch, Jr., K.N. Hooghan, R.J. Jenkins, M.J. Toth


Lucent Technologies, Allentown, PA, U.S.A.


Communication Signal Processors (CSP) did not have the Signal-to-noise ratio (SNR) performance expected. Significant differences were noticed between SNR values at wafer level and package testing.


The analog section of the chip was suspected to be the culprit as the problem existed at the analog to digital conversion level. A Dielectric Altering Compound (DiAC) was chosen to simulate the packaged environment in decapsulated parts1. The DiAC was applied in and around the analog section,after application in other areas did not show the SNR degradation.


The sampling capacitors in the A to D Converter section (ADC) were selectively coated with DiAC and laser trimmed to identify the offending circuit element. A signal trace running adjacent to the sampling caps, was isolated and suspected of coupling noise to the sampling caps.


A FIB system was used to deposit a grounded metal shield that covered the suspect runner on a packaged part - subsequent testing showed no degradation.


The above procedure was successful in isolating,verifying, and rectifying the SNR degradation. The SNR degradation was found on more than one code.


The same procedure was used repeatedly on subsequent errant codes. Finally, a mask level fix on silicon achieved the desired SNR performance for all the codes.


A mixed signal, Communication Signal Processor(CSP), was not exhibiting the expected SNR in the Analog to Digital Converter (ADC) section. The 13 bit ADC has a theoretical SNR of approximately 80dB. Significant differences (about 6dB) were observed between SNR values at the wafer level and package part tests.


An experiment was planned to identify the source of degradation. The plan was to take some packaged devices, test their noise performance, decapsulate them and retest again to compare differences. The 6dB difference (typical) between packaged and decapped parts were evident on all tested parts. In addition, significant differences in total harmonic distortion (THD) and noise floor in general were also observed (refer to Graphs 1 and 2 below and Table 1 summary). The 6dB SNR difference was further verified by bench testing. This proved that the package material was causing the noise degradation by altering the dielectric constant in the vicinity of some sensitive circuits. Therefore, isolating the sensitive areas became the next diagnostic step.


Graph 1 Packaged device showing degraded SNR and noise floor.


Graph 2 Decapped device showing expected SNR and noise floor.


Table 1 Test results


Parameter


Packaged Parts or with DiAC


Decapped parts without DiAC SNR 58.911 dB 66.419 dB THD 67.834 dB 74.727 dB Noise Floor 70.462 dB 77.357 dB


Isolation


Based on previous experience, we decided to use a Dielectric Altering Compound (DiAC) and apply it systematically to sections of the chip in order to isolate which part of the circuit was sensitive to packaging. The Dielectric constant of the packaging material was 3.7. In order to simulate the effects of plastic packaging, a DiAC with a dielectric constant greater than 3.7 would have to be used. The DiAC used was a common heat sink grease, with a dielectric constant of 4. This compound has been used previously to simulate plastic package encapsulation by adding parasitic capacitance to the underlying circuitry.


To start diagnostics, the entire chip was initially covered with DiAC to see if its SNR would degrade.


A 6dB degradation was observed with this treatment.


Next, since the ADC SNR was degraded, the DiAC was applied to only half of the chip where the analog circuitry was located (Figure 1). Again, SNR degradation was observed. The digital section of the chip was then coated with the same DiAC and this time, no degradation was observed. This confirmed our speculation that the analog section of the chip was the one that suffered from the packaging degradation effect. Using one strand of a fine artist brush, the DiAC was applied to smaller and smaller areas, (Fig. 2, 3) eventually concentrating around the sampling capacitors of the ADC circuitry. Initially, it was thought that there was noise coupling between some digital control circuitry and the sampling capacitors of the ADC section. Applications of DiAC to these areas however, failed to show SNR degradation. The evidence, however, continued to indicate that the sampling caps and their surrounding areas were the sources of the SNR degradation problem. Pinning down the exact offending circuit element, however, became more of a challenge. An innovative approach was required to precisely apply and trim the DiAC to the ADC elements and their surrounding section(s).


Figure 1 Analog section covered.


Figure 2 Example of DiAC application.


Figure 3 Higher magnification image of the sampling caps in the DAC section.


Figure 4 Example of Laser Trimming


Figure 5 Final Isolation DiAC cover.


Figure 6 Suspect Trace.


Figure 7 Unsuccessful FIB re-route


Figure 8 Successful FIB Shield.


A method of applying the DiAC in the general troubled area and laser trimming the DiAC away was suggested, discussed, and implemented. A New Wave laser, model LCSIII Tri-Lite, was used in the UV mode (355nm) to trim away the DiAC. With this wavelength, it was possible to remove the selected DiAC (Figure 4) without damaging any underlying circuitry. DiAC was applied, device tested, DiAC laser trimmed, and device re-tested. Using this method, we were able to more accurately pinpoint the offending circuit elements.


Several techniques were used to apply the DiAC compound. The best results were obtained by dipping a mechanical probe in the compound and then apply it using a low power microscope. With practice, a section of circuitry could be covered and spread over the targeted area. Laser trimming accomplished further isolation on specific circuit elements.


After application of the DiAC, devices were re-tested and characterized. Additional DiAC application or trimming was done after testing or, at times, the device was cleaned in acetone and a fresh application was applied in a new area. This process was repeated


until there was confidence that the sensitive area was identified. One final application of DiAC surrounding the suspect area (Figure 5) showed no degradation until after the isolated circuitry was covered. A metal three line, which ran adjacent to the ADC sampling caps, appeared to be the point at which noise was coupled into the ADC section(Figure 6). The last step was to verify the finding.


Verification and Fixes


Discussion with the design and layout engineers, led to a suggestion to disconnect the offending line and reroute it. A FEI FIB Model 200 was used to disconnect and reroute the offending runner(Figure 7). This however degraded the performance further even without the presence of any DiAC,perhaps because of the higher resistance of the rerouted line.


Further discussions led to the idea of using a grounded metal shield over the offending circuit element2. Again, using a FIB system, a metal shield was placed over the offending runner and tied to ground (Figure 8). DiAC was then applied to the suspected area. This time the noise degradation phenomenon was gone.


Knowing the offending trace, a metal mask fix was now proposed. The runner was routed away from the sampling capacitors and moved to an underlying metal level. This mask solution was successful and was then applied to circuits associated with two other codes that had used the same codec design.


Communication Signal Processors (CSP) did not have the Signal-to-noise ratio (SNR) performance expected in packaged form. A Dielectric Altering Compound (DiAC) was chosen to simulate the packaged configuration in decapsulated parts. The DiAC was selectively and iteratively applied to the chip in order to simulate the package caused noise degradation. Laser trimming of the DiAC helped to isolate the exact offending circuit elements that had contributed to the SNR degradation.


Next, a FIB system was used to verify that a metal trace was coupling noise to the adjacent sampling capacitors in the ADC section. This was verified by putting a ground shield over the offending metal line and resulted in recovery of the SNR performance.


Thus, by using a combination of DiAC, laser trimming (of DiAC), and FIB modification, we were able to isolate, verify, and rectify a SNR degradation problem. With this technique, we have come up with


a permanent solution of using just one mask change and effectively recovered all of the packaging induced SNR loss in a communication IC.


1. Lucent Technologies, Technical Memorandum


# 52211-860912-01M, “Capacitive effects on circuits due to passivation and packaging materials on the chip surface”, Davar, V, Lucent Technologies Proprietary (1986)


2. K.N. Hooghan, K.S.Wills, P.A. Rodriguez, S.


O’Connell, “IC Device Repair using FIB System, Tips, Tricks, and Strategies”,proceedings of ISTFA 1999, pp 247-254


Ever since the invention of the scanning acoustic microscope (SAM), a key objective has been the enhancement of the resolution in an interior image.


Thus, an acoustic lens that can form an interior image with a shear wave has been designed. The use of this lens gives benefits such as an increase of lateral resolution in the interior image, a reduction in background noise caused by surface roughness, and a reduction of spherical aberration.


Significantly, with the current trend towards microminiaturization of microelectronic packages, acoustic microscopy with higher resolution and removal of surface roughness can play an important role in diagnostic examinations and failure analysis. In this paper, applications for the lens in microelectronic IC packages will be summarized.


Increasing Subsurface Resolution


The scanning acoustic microscope (SAM) [1] has become a useful tool of nondestructive evaluation in the field of microelectronic integrated circuits (IC).


It can provide cross-sectional images to visualize details of defects located within an IC package. One of the issues of acoustic imaging in these fields is how to increase a resolution of its interior crosssectional image for detecting defects causing failures to the microelectronic IC systems.


The resolution of a surface image (Δr) of a specimen formed by the SAM is expressed by the following equation [2]


Δr = Fλ = F(Vc/f)


(1)where λ is a wavelength, F is a constant related to the lens geometry, Vc is a velocity of the coupling medium, and f is the frequency.


Three approaches can be considered to pursue the above objective from Equation 1. One approach is to raise the acoustic frequency [3]. By means of this


approach, B. Hadimiooglu et al. achieved a resolution of 0.2 micron by operating at about 4.4 GHz with the specimen in boiling water in order to minimize the attenuation of the coupling medium [4]. The second approach is to use low velocity coupling media such as super-fluid liquid helium [5]. Using the second approach, J. S. Foster et al. were able to obtain a resolution of 20 nano-meters using super-fluid liquid helium as coupling medium at a temperature of 0.2°K


[6]. These approaches are excellent for increasing resolution on the surface of a specimen, but not necessarily in its interior.


In the first approach, the ultrasonic wave is attenuated in proportion to the square of its frequency; therefore, when the high frequency ultrasonic wave is used as a probe, the wave may not penetrate the inside of the specimen, and the internal information may not be obtained. In the second approach, also referred to as cryogenic microscopy,the acoustic impedance between the coupler and the specimen are forced to be very different. In this way,most of the ultrasonic waves are reflected at the interface between the coupler and the specimen, and it is unlikely that an image from any significant depth may be obtained. Hence, acoustic microscopy’s most important and unique feature; namely obtaining subsurface information, may not be realized by these two approaches.


The third approach is to design a new acoustic lens.


By means of this approach, C-H Chou et al. proposed an acoustic lens with a transducer generating polarized waves to image anisotropy of materials [7].


D. A. Davids et al. proposed an acoustic lens with a restricted aperture for only generating the Rayleigh waves [8]. A. Atalar et al. proposed an acoustic lens with non-spherical aperture for generating the Lamb waves [9], and slit aperture for pseudo line focusing to image anisotropy of materials [10]. However,although these lenses give improvement of obtaining sub-surface information, the resolution at deep penetration depths is not improved.


Practical Shear Wave Lens


It is well known that resolution may be enhanced by using shear waves rather than longitudinal waves,since the wavelength of a shear wave is much shorter than that of the corresponding longitudinal wave at the same frequency. Most acoustic lenses, for low frequency application commercially available today,are limited to using only longitudinal waves.


Therefore, the acoustic lenses are designed with a low aperture angle (i.e., below 30°), by considering a penetration depth and a beam spot size. We call such lenses “conventional lenses”.


When a longitudinal wave traveling in a liquid is incident at a certain range of angles onto the surface of a solid, both longitudinal and shear waves are transmitted into the solid. The relative power of the component of the shear wave is zero when the incident wave from liquid to solid is vertical (θ is 0°).


As θ is increased, the component of the shear wave appears and increases. When θ exceeds the critical angle of the longitudinal wave, only the shear wave component is present. As can be appreciated, the critical angles for the longitudinal and shear waves depend on the properties of the materials used.


The description above can be applied to the case of an ultrasonic source in the shape of a lens sending longitudinal waves through a liquid into a solid. The considerations above lead to the existence of two separate focal points, one for longitudinal waves and the other for the shear waves. Furthermore, the relative ultrasonic power level at each focal point depends on the critical angles of the material. In particular, in order to excite a shear wave strong enough to form an acoustic image of the sample interior, the aperture angle of the lens portion of the acoustic lens must be large enough so that acoustic waves can be incident at angles exceeding the critical angle of the longitudinal wave. The shear wave can be excited in most of the materials when the full aperture angle is designed to be 100° or more at a frequency 30 MHz.


An acoustic lens having such a large aperture for pulse wave mode is called a high numerical aperture(hereinafter called simply “high N. A. lens”) [12]. A feature of the high N. A. lens is a large aperture angle for generating not only a longitudinal wave, but also a shear and a surface wave in the specimen in order to increase the interior resolution. The high N. A.


lens is designed for using the pulse wave so that longitudinal, shear and surface waves reflected from the specimen can be substantially separated by an electronic gate.


Figures 1(a) and 1(b) show images obtained by the conventional and high numerical aperture acoustic lenses, respectively. Both lenses operate at a


frequency of 30 MHz. These images are from a standard aluminum calibration specimen used for measuring the resolution of the scanning acoustic microscope in C-scan mode using the pulsed waves.


The resolution measuring patterns are arranged on the front surface. The width of the pattern is made to be 35 μm and 45 μm corresponding to the numbers indicated, with the thickness of the specimen at 3 mm. The pattern for measuring resolution is imaged by the longitudinal and shear waves incident from the back surface of the specimen to be focused on the front surface. Clearly, the high numerical aperture acoustic lens using the shear wave forms a better image in the interior.


Figure 1 Acoustic images obtained by focusing on back surface using (a) conventional and (b) High N.


A. lenses (frequency: 30MHz).


The aperture angle of the lens might not be large enough to generate shear waves within a soft material such as a polymer. In that case, an interior image can only be formed by a longitudinal wave reflected from the material. However, the resolution of the image is


increased because the lens geometry reduces spherical aberration. Figs. 2(a), 2(b), 2(c) and 2(d)show images of internal structures of a plastic mold IC package, wherein the images were formed by the conventional lenses with frequencies at 30, 50, 75 and 110 MHz, respectively. As can be seen the images are resolved better due to the frequency increase. The frequency cannot be increased beyond 110 MHz because of the high attenuation of the plastic. Fig. 3 shows an image of internal structures of the same plastic mold IC package, wherein the image was formed by the high N. A. lens with a frequency at 30 MHz. The resolution in Figure 3 is seen to be considerably better than that in Figure 2(d).


Frequency f = 30 MHz,


Scanning size 12.0 mm x 9.0 mm


Frequency f = 50 MHz,


Frequency f = 75 MHz,


Frequency f = 110 MHz,


Figure 2 Acoustic images of internal structures of a plastic mold IC package using conventional lenses.


Figure 3 Acoustic image of internal structures of the same plastic mold IC package using the high N. A.


lens with a frequency at 30 MHz.


It is generally well known that an internal acoustic image is strongly affected by surface features, such as machining marks, insignia, corrosion pits, or generally surface roughness. When this surface roughness is excessive, its superposition on the internal image leads to complications in image analysis. Thus, it is desirable to minimize this influence.


The point-spread function (PSF) of the high numerical acoustic lens has a significantly wider distribution in the horizontal plane. Considering the final output at the transducer, the reflected acoustic field is integrated over a larger surface area leading to a “washing out” of surface roughness details. This is a key issue for the reduction of superimposed surface roughness. Figs. 4 (a) and 4(b) show images formed by a conventional and a high N. A. lens at a frequency of 30 MHz. Fig. 4(a) is an interior image showing an IC chip included in the package, wherein the surface image (i.e., marks) was superimposed onto the interior image. Fig. 4(b) is an interior image showing the same IC chip, but the surface image was not superimposed.


Figure 4 Acoustic images obtained by focusing on back surface using (a) conventional and (b) High N.


A. lenses (frequency: 30MHz), wherein the images are from the IC chip internally located in the IC package. Clearly visible are the improvement in resolution and reduction in surface features for the high N. A. lens.


The use of a high N. A. lens (i.e., one of practical shear wave lenses) has at least three benefits for visualizing interior portions of a mold IC package.


One may select the shear waves for the imaging process and achieve about 50% or higher resolution.


The effects of surface roughness of a specimen on an interior image are reduced.


A spherical aberration is reduced when an interior image is formed by a reflected longitudinal wave.


1. R. A. Lemons and C. F. Quate: “Acoustic microscope-scanning version”, Appl. Phys. Lett.,24, pp. 163 - 165, (1974)


2. G. S. Kino: “Fundamentals of scanning systems.


In Scanned image microscopy (ed. E. A. Ash),pp. 1 – 21. Academic Press, London (1980)


3. V. B. Jipson and C. F. Quate: “Acoustic microscopy at optical wavelength”, Appl. Phys,Lett., 32, pp. 789 - 791, (1978)


4. B. Hadimioglu and C. F. Quate: “Water acoustic microscopy at suboptical waterlengths”, Appl.


Phys. Lett., 43, pp. 1006 - 1007, (1983)


5. J. Heiserman, D. Rugar and C. F. Quate:“Cryogenic acoustic microscopy”, J. Acoust.


Soc. Am., 67, pp. 1629 - 1637, (1980)


6. G. T. Saumer and D. Rugar: “High resolution acoustic microscopy in superfluid helium”, Appl.


Phys. Lett., 42, pp. 869 - 871, (1983)


7. B. T. Kuri-Yakub and C-H Chou: “Acoustic microscope lenses with shear wave transducers”,IEEE 1986 Ultrasonic Symposium, pp.741 - 744,IEEE, New York, (1986)


8. D. A. Davids and P. Y. We and D. Chizhik:“Restricted aperture acoustic microscope lens for Rayleigh wave imaging”, Appl. Phys., Lett.,54(17), pp. 1639 - 1641, (1989)


9. Atalar, H. Koymen, and L. Degertekin:“Characterization of layered materials by the Lamb wave lens,” in Proc. of IEEE 1990 Ultrasonics Symposium, pp. 359 - 362, (1990)


10. Atalar, I. Ishikawa, Y. Ogura and K. Tomita:“Anisotropy sensitivity of an acoustic lens with slit aperture,” in Proc. of IEEE 1993 Ultrasonics Symposium, pp. 613 - 616, (1993)


11. D. A. Hutchins and D. W. Schindel: “Advances in non-contact and air-coupled transducer”, in Proc. of IEEE 1994 Ultrasonics Symposium, pp.


1245 - 1254, (1994)


12. C. Miyasaka, B. R. Tittmann, and M. Ohno:“Practical shear wave lens design for improved resolution with acoustic microscope”, Res Nondestr Eval, 11, pp. 97 –116, (1999)


p 309-313


DOI: 10.1361/cp2000istfa309


Combining FIB sequential cross-sectioning with TEM for small Defect Analysis in SRAM array


Nathan Wang and Rei Fang


Cypress Semiconductor Corp., San Jose, California, USA


To find defects and their root cause in semiconductor devices has become more and more difficult as chip size dramatically drops. A novel method combining FIB sequential cross-sectioning and TEM is described in this paper. This combination has provided a powerful tool for defect mechanism analysis. FIB slicing through a failed cell can be controlled to a precision of 0.1 micron. Passive voltage contrast imaging with FIB enhances defect detection. After a defect is found, in-situ TEM sample is prepared with FIB milling. By putting together the series FIB images along side with the TEM images and its associated high resolution EDS data, the detailed defect formation mechanism was discovered and feedback to process engineering for process improvement.


The shrinking geometry in VLSI manufacturing has made failure analysis more difficult because of more subtle and smaller defects[1]. Physical visualization of a defect is crucial for understanding defect formation mechanism. Capital equipment, such as SEM, FIB and Transmission Electron Microscope(TEM) has become essential tool for this task. How to use the equipment to take advantage of its capability is the key for high success rate of failure analysis. Therefore the methodology of applying the equipment plays a key role in the FA field.


It is well known that Focused Ion Beam has the following capabilities:


1. Modify circuitry to isolate defects.


2. Make precise cross-section at short turn around time without mechanical damage.


3. Its unique passive voltage contrast can pin-point very small defects.


4. The ability of making In-Situ TEM sample, so TEM high resolution can also be applied.


Many defects in SRAM main array can be isolated into a small cell location by means of automatic test equipment (ATE). A major challenge for FA engineer is how to physically expose the defect in the small volume. FIB’s sequentially cross-sectioning proves useful for bit related defect.*


When combining this technique with TEM’s high resolution and precise EDS analysis capability, the power to identify small defects compounds. This paper introduces such an example to find a small defect in an SRAM array.


Materials


The failure device used in this study is a 1M SRAM device fabricated with a 0.35 μm technology which uses a 5 Volt power supply. It failed after 80 hours burn-in stress at 5.5 volt and 150 °C.


Electrical Analysis


The electrical test is the first step to identify defect characteristics and physical locations. The electrical signature also provides information for analytical strategy decision.


The sample was tested with MosAid. The unit failed a single column. Whole column failed for one polarity except one bit failed for opposite polarity.


The result is shown in Figure 1. The gray bar represents failed bits stuck at low, while the black one stuck at high. The electrical signature indicates that the column failed due to reverse polarity failing bit. This is a typical bit-line to memory cell leakage signature. Now we have defect navigation information not only the location in the X-Y plane on die surface but also at the Z direction in stacking layers. The bit line is metal 1 layer where the memory cell is connected to it by the W local interconnect layer below. This type of defect is very difficult to visualize using traditional Top-Down deprocess failure analysis.


Figure 1 MosAid result showing defect signature.


FIB analysis


FIB slicing was performed at this location. Figure 2 represents the top-down SRAM cell shape and relative FIB cut location. A series of In-Situ FIB cross-section images are shown in Figure 3. A feature of immediate interest is the number of bright and dark contrast features, which anomalous appear right under the tungsten local interconnect (LI) layer. The dark ones look like cavities while the shining ones should be conductive material and connected to the substrate according to FIB passive voltage contrast.


Figure 2 Top-down SRAM cell structure schematically showing FIB cut position. The box


shows the failing cell boundary.


a. FIB Cross-section # 1.


b. FIB Cross-section # 2.


c. FIB Cross-section # 3.


d. FIB Cross-section # 4.


d. FIB cross-section # 5.


Figure 3 FIB images of a series of cross sectioning.


TEM and EDS analysis


To see the detailed image and determine the composition of the conductive material, in-situ TEM sample was made.


The sample was mechanically polished into a block and mounted on a grid. The grid was put into FIB machine for final cutting.[4,5,6] Figure 4 shows schematically how the sample was finally cut with FIB machine.


Figure 4 TEM sample preparation with FIB system.


Figure 5 is the TEM image that shows the short-lineshape defects. The short white lines are cavities that correspond to the short black ones in FIB images.


Electrons will be readily transmitted through these low density areas and therefore the signal intensity is much higher, i.e. bright contrast. The short black lines are the heavy metal lines that are shining in FIB images. EDS analysis was carried out to find the


composition of the filled material in the cracks. The location of the EDS is circled in Figure 6 and the EDS spectrum was shown in Figure 7. The result indicates that it is tungsten.


TEM result also allows us to clearly tell where is the origin of the short lines. It is very hard with FIB image because of its limited resolution. All the lines start at the boundary of BPSG layer and cap TEOS layer.


These short lines are the defects that caused the failure. The next thing we need to know is how it occurred so our FAB can eliminate it.


Figure 5 A TEM image showing the defects.


Figure 6 A high magnification TEM image showing the defects. The circle is the location of EDS.


Figure 7 EDS spectrum showing that tungsten filled into the cracks.


Focused Ion Beam technology proved useful for such purpose because it provides the ability to do the sequential cross-sectioning and in-situ observation. In other words, most defects within a single memory cell can be hit, if the FIB slices through the cell with small enough steps. Since FIB cutting steps are controllable and can be as small as 0.1 micron, many defects in this size can be seen from FIB image.


Besides, this operation produced a series of FIB images, which can be transferred into threedimension information, so that defect shape,distribution and size can be unveiled. Based on this model we linked the short lines in each FIB image of our sample, we composed the Figure 8a which shows the shape of these lines top-down. It revealed that the failure mechanism is the shorting between two tungsten plugs because of the lines filled with tungsten formed a path. Figure 8b show the scratch marks at failing cell from top-down physical analysis of another failed unit.


Figure 9 shows the defect in the electrical circuitry.


The metal stringer shorted the bit-line pass gate. The leaky pass gate makes the cell fail when writing a zero. In other words, it is equivalent to stuck at "1"on bit map. The bit -line and bit-line bar are charged up prior to the read operation. The leaky pass gate would pull down the pre-charge on bit-line.


Therefore whole column failed "1" read operation. It shows stuck at "0" on bit map.


Figure 8 A top-down schematic showing defect shape and distribution.


Figure 8b A top view showing the scratch marks


from top-down physical analysis.


Figure 9 The schematic circuitry of the memory cell


showing the failure mechanism.


It was noticed that the lines that formed the shorting path are always shining in FIB images and they look larger than the rest of dark cracks. It is the FIB unique voltage contrast technique that exaggerates the defect size. Such effect is good to be used to identify open-short defect,[7] but it mislead about the actual defect size and where it started. In our example, FIB image shows the defect started at bottom of the local interconnection layers. But TEM observation clearly reveals that the defects are below cap TEOS layer.


According to this result we can deduce that the defect occurred before the cap TEOS layer deposition but after bottom BPSG formed. The defect shape in Figure 8 shows the chatter mark shape. The chatter mark is a typical mechanical scratch signature.[8] Size of the scratch is so small that it is not likely from wafer handling. After checking the FAB process, the only possible step that can cause such scratch is the Chemical Mechanical Planarization.


Now we can figure out the whole sequence of the defect formation: First, the CMP caused the scratching on the surface of BPSG layer; and then the layer was covered by the cap TEOS. Some of the cracks cross over the positions of two contacts so during the following-up etching of plug-hole, both ends of these cracks reached the contact holes and


formed a tunnel between the two contact holes. They filled with tungsten during the subsequent tungsten CVD and formed butterfly shape stringers. They are fat at both ends attached to tungsten plugs and fine in the center. The tungsten path between the two contacts is very fragile and easy to be broken during the Top-Down de-layering process, since this metal stringer is not a designed feature. It is not necessary to be a good conducting channel nor to fail at time zero. After burn in stress at higher Vcc and elevated temperature, the conducting passage could be created by either the primitive oxidation layer break down or metal grains re-growth.


FIB sequential cross-sectioning is a good method to analyze the defect in a small volume, such as single bit failure. This is because of the FIB's voltage contrast can identify tiny defects; provide 3-D images to see the distribution of defects. Combined with insitu TEM, high resolution and EDS analysis, detail can be seen and composition can be determined. It enhances the capability of analyzing small defect.


It is worth of mentioning that for analyzing such defect between layers, FIB is the best tool. Top-down layer by layer deprocessing using chemical etching will wash the tiny defect. The mechanical polishing can easily by-pass the small defects between steps and missed them altogether.


1. L. Wagner et al., Failure Analysis of Integrated Circuits, Klumer Academic Publishers, 1999, P.


241.


2. A. N. Campbell, Fault Localization with the Focused Ion Beam System, ISTFA’97 Workshop, 1997, P. 180.


3. D. Luo, X. Song, Proceedings of ISTAFA’97.


4. S. Tsuji et al., The Solid Films, 281-282(1996)


562.


5. A. Yamaguchi, M. Shibata, J. Vac. Sci. Technol.


B 11(6), Nov/Dec 1993.


6. S. Morris et al., Proceedings of ISTFA’91, P.


417.


7. K. J. Giewont et al., J. Vac. Sci. Technol. B 15(4), Jul/Aug 1997, P.916.


8. ASM committee, Metals Handbook, American Society for metals, 8.3, 1983, P.259.


p 315-321


DOI: 10.1361/cp2000istfa315


Failure Analysis of Tungsten Stud Defects from the CMP Process


K. Takagi, Y. Kohno


ITES Co., Ltd. Shiga, Japan


S. Nukii


IBM Japan, Ltd.


This paper describes a failure analysis that effectively combined multiple analytic techniques to find the cause of I/O leakage in a flawed chip produced for an OEM (Original Equipment Manufacturer) product.


Internal probing was initially used for defect isolation and a Tungsten (W) stud open circuit flaw was isolated by electrical characterization with internal probing. SEM (Scanning Electron Microscopy), TEM(Transmission Electron Microscopy, and FE-AES(Field Emission Auger Electron Spectroscopy)analysis with FIB (Focused Ion Beam) preparation were used for physical analysis. Cross-sectional SEM and TEM observations showed a gap with foreign material (FM) between the bottom of the metal line and the top of the W stud, possibly from the W CMP(chemical mechanical polish) process. FE-AES is effective for the analysis of light materials and their chemical composition, so a flat milling FIB process was used to prepare a cross-section for FE-AES analysis of the FM and the interfaces of the open defect. The spectra showed that the FM was traceable to the W CMP process. From these analytical results and problem reproduction experiments in the W CMP process on the manufacturing line, the failure mechanism was identified.


Failure analysis is very important to improve and maintain production yield in manufacturing lines,because low yield wastes production resources and decreases business profits. Quick and accurate feedback from analysis to manufacturing lines is necessary in order to take corrective actions. Failure analysis generally involves two steps.


The first step is to localize a defect. Electrical analysis such as electrical diagnosis, EMS (emission microscopy), OBIC (optical beam induced current)technique, LCT (liquid crystal technique), internal probing and so on are used for defect localization.


The second step is physical analysis of the defect.


SEM, TEM, FE-AES, FIB, and SIMS (secondary ion


mass spectroscopy) are used for physical analysis.


The mentioned analytical techniques are useful by themselves, but when they are combined, they become more effective.


One of the most important goals of failure analysis is to determine the root cause of failure. This paper describes the effectiveness of these combined analysis techniques to analyze the I/O leakage failure of the OEM product, leading to the correct conclusion.


Failure Description


The problem was low yield of the OEM product. The main features were 0.5 um design rules, single poly-Si with W silicide and 4 layers of metallurgy. Also CMP technology was used for each interconnect layer.


According to electrical diagnostic result from an LSI tester, the detected failures showed up in the following categories: Functional failures, IDD (power supply current) leakage failures, and I/O leakage failures.


It was necessary to perform failure analysis, and feedback to the manufacturing line was desired as soon as possible. However, analysis of the functional failure or IDD leakage failure might be very difficult,because there was a lot of process information but relatively little design information. Since it seemed that the same root cause led to all three failures, we tried to analyze the I/O leakage failure, because the I/O circuits were simpler than the others.


Defect Isolation


There are three types of I/O that can be performed(Input, Output and Common input/output). We decided to analyze the input circuit, because this circuit is simpler than the output or common input/output circuits. Figure 1 is the schematic of the input circuit. It has two VDD (power supply voltage)inputs labeled V1 and V2. V1 is a power supply for the protective devices, and V2 is for the receiver circuits and internal LSI logic. An input line from the pad is connected to the gates of a receiver circuit through protective devices.

