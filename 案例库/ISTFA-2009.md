---
title: "ISTFA-2009.pdf"
source: IMA知识库/IC失效分析/
media_id: pdf_f27e1b7ab86c953bd98a56bed90e29a1_e7e42cfbcb68317815f5ad5ee54a9de57295230462135641
file_size: 41909048
---

ISTFA  2009TM


Conference Proceedings from the  35th International Symposium  for Testing and Failure Analysis


November 14–19, 2009


San Jose McEnery Convention Center  San Jose, California, USA


Sponsored by


EDFAS


Electronic Device Failure Analysis Society


An Affiliate Society of ASM International®


ASMNATIONALEverything®Material.


ISIFA/2009


The Materials


Information Society


www.asminternational.org/istfa


www.asminternational.org


Published by  ASM International®


Materials Park, Ohio 44073-0002


Copyright  © 2009


by


ASM International®


All rights reserved


No part of this book may be reproduced, stored in a retrieval system, or transmitted, in any form or by any  means, electronic, mechanical, photocopying, recording, or otherwise, without the written permission of  the copyright owner.


First printing, November 2009


Great care is taken in the compilation and production of this Volume, but it should be made clear that NO  WARRANTIES, EXPRESS OR IMPLIED, INCLUDING, WITHOUT LIMITATION, WARRANTIES  OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE, ARE GIVEN IN  CONNECTION WITH THIS PUBLICATION. Although this information is believed to be accurate by  ASM, ASM cannot guarantee that favorable results will be obtained from the use of this publication alone. This publication is intended for use by persons having technical skill, at their sole discretion and risk. Since  the conditions of product or material use are outside of ASM's control, ASM assumes no liability or  obligation in connection with any use of this information. No claim of any kind, whether as to products or  information in this publication, and whether or not based on negligence, shall be greater in amount than the  purchase price of this product or publication in respect of which damages are claimed. THE REMEDY  HEREBY PROVIDED SHALL BE THE EXCLUSIVE AND SOLE REMEDY OF BUYER, AND IN NO  EVENT SHALL EITHER PARTY BE LIABLE FOR SPECIAL, INDIRECT OR CONSEQUENTIAL  DAMAGES WHETHER OR NOT CAUSED BY OR RESULTING FROM THE NEGLIGENCE OF  SUCH PARTY. As with any material, evaluation of the material under end-use conditions prior to  specification is essential. Therefore, specific testing under actual conditions is recommended.


Nothing contained in this book shall be construed as a grant of any right of manufacture, sale, use, or  reproduction, in connection with any method, process, apparatus, product, composition, or system, whether  or not covered by letters patent, copyright, or trademark, and nothing contained in this book shall be  construed as a defense against any alleged infringement of letters patent, copyright, or trademark, or as a  defense against liability for such infringement.


Comments, criticisms, and suggestions are invited, and should be forwarded to ASM International.


ISBN-13:978-1-61503-008-8


ISBN-10: 0-61503-008-5


SAN: 204-7586


Materials Park, OH 44073-0002


Printed in the United States of America


Multiple copy reprints of individual articles available from Technical Department, ASM International.


EDFAS 2009-2010 BOARD OF DIRECTORS


EDFAS President                                                EDFAS Vice President


Mr. Tracy D. Myers                                                 Dr. Thomas Moore


ON Semiconductor                                                       OmniProbe


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

|Mr. Thomas Zanon |Education Chair |PDF Solutions Inc. |

|Mr. William E. Vanderlinde |Events Chair |IARPA |

|Dr. Aaron Falk |Journal Chair |Quantum Focus Instruments Corp. |

|Mr. John West |Membership Chair |Texas Instruments |

|Mr. Gary Shade |Nominating Chair |Insight Analytical Labs |

|Mr. Jeremy Walraven |Website Chair |Sandia National Laboratories |

iii


ISIF4/2009


ORGANIZING COMMITTEE


r


|Nicholas Antoniou |William E. Vanderlinde |Jeremy Walraven |Dan Bodoh |James Demarest |
|---|---|---|---|---|

|General Chair |Vice General Chair |Technical Program Chair |Tutorial Chair |Tutorial Vice Chai |

|Harvard University |IARPA Sandia |National Laboratories |Freescale Semiconductor |IBM |

David P. Vallett


Immediate Past General Chair


IBM Systems & Technology Group


||Activities Chairs |Activities Chairs |Activities Chairs |
|---|---|---|---|

|Martin Keim ||Ed Keyes |Philippe Perdu |

|Panel Chair ||Exposition Chair |User’s Group Chai |

|Mentor Graphics |Corp. |Semiconductor Insights |CNES |

|Efrat |Raz-Moyal |Dave Vallett |Zhiyong Wang |

|Publicity/Local |Arrangements |EDFAS Liaison |Audio/Visual Chai |

|Chair ||IBM Systems & Technology Group |Intel Corporation |

|Omniprobe, |Inc. |Inc. |Inc. |

iv


ISTFA 2009 TUTORIAL COMMITTEE


ISTFA 2009


Tutorial Program Chair


Dan Bodoh


Freescale Semiconductor


|Tutorial Committee Chair |Topic |Affiliation |
|---|---|---|

|Dan Bodoh |Fault Isolation, Lab Management, Technology Specific FA, The Periphery of FA |Freescale Semiconductor |

|James Demarest (vice-chair) |Fault Isolation, Microscopy |IBM |

|Susan Li |Fault Isolation, Microscopy |Spansion |

|Chris Richardson |Focused Ion Beam (FIB), |LSI Logic |

|Chris Richardson |Microscopy, |LSI Logic |

|Chris Richardson |Technology Specific FA |LSI Logic |

|Chad Rue |Die and Defect Access, Technology Specific FA |FEI Company |

|Sam Subramanian |Die and Defect Access, Technology Specific FA, The Periphery of FA |Freescale Semiconductor, Inc |

|Jeremy A. Walraven |Technology Specific FA |Sandia National Laboratories |

v


ISTFA 2009 SYMPOSIUM COMMITTEE


Technical Program Chair


Jeremy A. Walraven


Sandia National Laboratories


Advanced Metrology & System  Level FA


SAM SUBRAMANIAN (CHAIR),


Freescale Semiconductor, Inc.


JAMES DEMAREST (CO-CHAIR), IBM


Jiann Min Chin, AMD


Ted Kolasa, Freescale Semiconductor, Inc. Eckhard Langer, Global Foundries


Srikanth Perungulam, Texas Instruments


|APEK MULAY (CHAIR), |JIM COLVIN (CHAIR), |STEVE IPPOLITO (CHAIR), IBM |
|---|---|---|

||FA Instruments|AARON FALK (CO-CHAIR), |

|Texas Instruments|Dave Burgess, Accelerated Analysis |QFI/Optometrix |

|DAVID L. BURGESS (CO-CHAIR), |Vijay Chowdhury, Evans Analytical Group |Christof Brillert, Infineon Technologies |

|Accelerated Analysis |Carl Nail, Independent Consultant |Tohru Koyama, Renesas |

|Syed Ali, Volt Technical Resources |Rose Ring, SMSC |Hirotoshi Terada, Hamamatsu |

|Carlos Arroyave, Skyworks Inc. ||Winfield Scott, MEFAS |

|Phil Kaszuba, IBM |||

|Bhanu Sood, University of Maryland |Nanoprobing |Posters |

||TAYLOR CAVANAH (CHAIR), |Posters|

|Alternative Energy |Zyvex Instruments |SCOTT WILLS (CHAIR), |

|CHRISTIAN BOIT (CHAIR), |PETER HARRIS (CO-CHAIR), |Independent Consultant David Paul , Texas Instruments |

|University of Berlin |Multiprobe Inc. |Phu Thy Do, Texas Instruments |

|Stefan Gall, Berlin Helmholtz Center |Larry Liu, Texas Instruments |Phu Thy Do, Texas Instruments|

|Sarah Kurtz, NREL |Terry Kane, IBM ||

|Jef Poortmans, IMEC |Randy Mulder, Freescale Semiconductor, Inc. |Sample Preparation |

||Andy Saxonis, Analog Devices |BECKY HOLDFORD (CHAIR), |

|Circuit Edit ||Texas Instruments |

|TED LUNDQUIST (CHAIR), |Packaging/Assembly Level FA |ROBERT CHAMPAIGN (CO-CHAIR |

|DCG Systems |JAMES DEMAREST (CHAIR), IBM |Raytheon |

||Carol Boye, IBM |Jake Klein, Texas Instruments |

|RYAN ROSS (CO-CHAIR), |Ted Levin, IBM |David Su, TSMC |

|Freescale Semiconductor, Inc. |Andrew Mawer, Freescale Semiconductor, Inc. |Bryan Tracy, Spansion |

|Marsha Abramo, Independent Consultant |Jessica Tucker, Aerospace Corporation ||

|Yuval Greenzweig, Intel |||

|Mike Phaneuf, Fibics Incorporated |||

Texas Instruments


Chris Richardson, LSI


Emerging Concepts


MIKE BRUCE (CHAIR),


Independent Consultant


DAN BODOH (CO-CHAIR),


George Lange, Freescale Semiconductor, Inc. Susan Li, Spansion


Failure Analysis Process  FA Instruments


Photon Beam Based Techs.  1


FELIX BEUDOIN (CHAIR), IBM


PHILIPPE PERDU (CO-CHAIR), CNES  Franco Stellari, IBM


Herve Deslandes, DCG Systems


Jerome Touzel, Infineon Technologies


Frank Zacchariasse, NXP


Photon Beam Based Techs. 2


),


vi


Be part of ISTFATM 2010.


Think Big.


November 14-18, 2010 Intercontinental Hotel Dallas, Texas USA


Calling all experts!


Share your experiences and advance the


industry at ISTFA 2010, the premier event for  the electronics failure analysis community.


The high technology industry has been one of  the fastest growing industries in the world, in  the US, in the state of Texas and in the


Dallas/Fort Worth area.


EDFAS9639 Kinsman Road Electronic Device Failure Analysis SocietyMaterials Park, Ohio 44073-0002 An Afflate Society of ASM Interrational+


800.336.5152


We invite you to submit  your work for publication


ISTFA/2010


and to present to the industry in Dallas, Texas for  the 36th year of ISTFA. Advance the industry.


Present and be a part of ISTFA 2010.


Submit your abstract today.


Abstract Submission Deadline: April 2, 2010 Go to www.istfa.org.


EDFAS 2009 Photo Contest Winner,First Place Color: An image of an EOS site after decapsulation of a power


device. It looks like a smiley face.


Deborah Romero


International Rectifier Corporation


ix


Contents


IPFA 09 Best Paper


# Contents


An Advanced Reliability Improvement and Failure Analysis Approach to


Thermal Stress Issues in IC Packages ..................................................................................1


Michael Hertl1, Diane Weidmann1, and Alex Ngai2


(1) Insidix, Grenoble/Seyssins, France;


(2) Teltec Semiconductor Pacific Ltd., Hong Kong


Session 1: Emerging Concepts


Gradient Thermal Analysis by Induced Stimulus .................................................................6


Jim Colvin


FA Instruments, Inc., San Jose, CA USA


Measurement of Bit Leakages in a Functional SRAM ........................................................16


Xiaowei Deng, Wah Kit Loh, Beena Pious, Jayesh Raval, Bashar Khan,  Larry Liu, Taylor Lowry, DB Yoon, Theodore W. Houston, Randy McKee,  Abha Singh Kasper, and Dan Corum


Texas Instruments Inc., Dallas, TX, USA


Extended Circuit Edit, Analysis and Trimming Capabilities Based on the


Backside Focused Ion Beam Created Ultra Thin Silicon Platform ....................................21


Rudolf Schlangen1, Rainer Leihkauf1, Uwe Kerst1, Christian Boit1,  Peter Egger2, and Ted Lundquist3


(1) Berlin University of Technology, Berlin, Germany;


(2) Infineon Technologies AG, Munich, Germany;


(3) DCG Systems Inc., Fremont, CA, USA


Subsurface Imaging of Multi-Level Integrated Circuits Using


Scanning Electron Acoustic Microscopy ............................................................................27


L. Meng1, A.G. Street2, and J.C.H. Phang1


(1) National University of Singapore;


(2) Qualcomm CDMA Technologies, San Diego, CA, USA


Laser Timing Probe with Frequency Mapping for


Locating Signal Maxima ........................................................................................................33


L.S. Koh1, H. Marks2, L.K. Ross1, C.M. Chua1, and J.C.H. Phang1, 3


(1) SEMICAPS Pte Ltd, Singapore;


(2) NVIDIA Corporation, Santa Clara, CA, USA;


(3) National University of Singapore


x


Session 2: Photon Beam Based Techniques – 1


Pseudo-Soft Defect Localization ..........................................................................................38


Paiboon Tangyunyong, Rick McFarland, and Richard S. Flores,  Sean Pearson, and Marco O. Sanchez


Sandia National Laboratories, Albuquerque, NM, USA


Software Enhanced Time Resolved Laser Assisted Device Alteration with a


Non-Pulsed Laser Source .....................................................................................................43


Kent Erington, John Asquith, and Dan Bodoh  Freescale Semiconductor, Austin, TX, USA


From Static to Full Dynamic Laser Stimulation ..................................................................52


A. Deyine1, K. Sanchez1, P. Perdu1, F. Battistella1,  H. Deslandes2, and D. Lewis3


(1) Thales & CNES Laboratory, Toulouse, France;


(2) DCG System, Fremont, CA, USA;


(3) IMS Laboratory, Talence, France


Annular Illumination and Collection in Solid Immersion ...................................................60


Stephen Bradley Ippolito1 and Hirotoshi Terada2


(1) IBM Semiconductor Research & Development Center, Hopewell Junction, NY, USA;


(2) Hamamatsu Photonics, Hamamatsu City, Japan


Backside IR Raman Temperature Measurements ...............................................................65


R. Aaron Falk1, Tram Pham1, and Grant Albright2


(1) Quantum Focus Instruments Corp., Tukwila, WA, USA;


(2) Quantum Focus Instruments Corp., Vista, CA, USA


Session 3: Nanoprobing


Nanoprobe Capacitance-Voltage Spectroscopy (NCVS) Localization of


32nm SOI SRAM Array Failure .............................................................................................73


Terence Kane and Michael P. Tenney


IBM Systems and Technology Group, Hopewell Junction, NY, USA


The SRAM Soft Failure Analysis with SNM & TR Characterization by


Nanoprobing in Sub 45nm ....................................................................................................76


Jakyung Hong, S.J. Cho, Y.W. Han, H.S. Choi,


T.E. Kim, S.J. Son, H.S. Kim, S.D. Kwon, and Y.S. Oh  Samsung Electronics Co., Korea


Electrical Characterization of Different Failure Modes in


Sub-100 nm Devices Using Nanoprobing Technique .........................................................81


E. Hendarto, S.L. Toh, J. Sudijono, P.K. Tan, H. Tan, Y.W. Goh,  L. Zhu, Q. Deng, H.B. Lin, R. He, H.L. Li, Z.H. Mai, and J. Lam  Chartered Semiconductor Manufacturing Ltd, Singapore


xi


Electrical Signature Verification of a Lightly Doped Drain Profile Abnormality in a


65nm Device via Nano-Probing and Junction Stain TEM ...................................................88


Jie Su, Sanan Liang, Yoyo Wen, May Yang, Linfeng Wu,


Chorng Niou, Xianfeng Chen, and Gary Zhao


Semiconductor Manufacturing International Corporation, Beijing, P.R. China


FAMOS Fail Bit Verification /Characterization via NanoProbe ..........................................93


Mark Dexter1, Richard Stallcup II2, and Sarma Gunturi1


(1) Texas Instruments, Inc. Dallas, TX;


(2) Zyvex Corp., Richardson, TX


Session 4: Circuit-Edit


Methodologies for Quantifying FIB “Milling Acuity” ..........................................................97


Chad Rue


FEI Company, Hillsboro, OR, USA


Novel Dielectric Etch Chemistry for the Next Generation of Circuit Edit:


Delicate to Low-k Dielectrics and Silicon ..........................................................................106


Vladimir V. Makarov1, Leo Krasnobayev1, and Sabina F. Misquitta2


(1) Tiza Lab, LLC, Milpitas, CA, USA;


(2) Advanced Circuit Engineers, LLC, Milpitas, CA, USA


Global Die Ultra-Thin Silicon for Backside Diagnostics and Circuit Edit .......................110


Dane Scott1, Erin O’Donnell1, Tahir Malik2, and Rajesh Jain2


(1) Intel Corporation, Folsom, CA, USA;


(2) DCG Systems, Inc., Fremont, CA, USA


A Versatile Design of Solid Immersion Lenses in Bulk Silicon Using


Focused Ion Beam Techniques ..........................................................................................119


P. Scholz1, U. Kerst1, C. Boit1, C.-C. Tsao2, and T. Lundquist2


(2) DCG Systems, Fremont, CA, USA


Session 5: Sample Preparation


Localized Epoxy Layer Formation on Surface Defect Using a


Micro-Brush in a Plucking System .....................................................................................126


Kun-Lin Lin, Jian-Shing Luo, Hsiu-Ting Lee, and Jeremy D. Russell  Inotera Memories Inc., Taoyuan, Taiwan


Deterministic Polishing Applications in Failure Analysis ................................................130


Mark Kimball


Maxim Integrated Products, Hillsboro, OR, USA


Near-Infrared Microscopy in Semiconductor Failure Analysis Applications .................135


Thomas B. Davis, Robert Reagan, Yangyang Sun, and Tom Jiang  Micron Technology Inc., Boise, ID, USA


xii


Low Temperature O2 Plasma Process for


Scanning Capacitance Sample Preparation ......................................................................140


Donald W. Schulte, Terry McMahon, David D. Hall, Mark Johnson, William Stickle,  Craig Sanders, Greg Long, Gary DeHaan, and Ruhua Cai


Hewlett Packard Company, Corvallis, OR, USA


Non-Destructive Failure Analysis in Organic Thin-Film Transistors ..............................144


Shih-Ting Liu1, Tao-Chi Liu1, Ming-Lun Chang1, King-Ting Chiang1,  Su-Ping Chiu1, Jandel Lin1, Po-Yuan Lo2, and Pei-Wen Li2


(1) Integrated Service Technology Inc., Hsin-chu, Taiwan (R.O.C.);


(2) National Central University, Taoyuan, Taiwan (R.O.C.)


Session 6: Alternative Energy


Comparative Failure Analysis of Photovoltaic Devices ...................................................149


FA Instruments, Inc., San Jose, CA, USA


Analysis of Poly-Si Thin Film Solar Cells by IR-LBIC .......................................................157


M. Boostandoost1, H.-P. Lin1, U. Kerst1, C. Boit1, and S. Gall2


(2) Helmholtz-Zentrum Berlin für Materialien und Energie, Berlin, Germany


Failure Analysis of Breakdown Sites in Silicon Solar Cells .............................................162


Otwin Breitenstein1, Jan Bauer1, Jan-Martin Wagner1, Horst Blumtritt1,  Nikolai Zakharov1, and Andriy Lotnyk2


(1) Max Planck Institute of Microstructure Physics, Halle, Germany;


(2) Christian-Albrecht-University, Kiel, Germany


Approaches to Photovoltaic Systems Reliability .............................................................166


Jennifer E. Granata, Elmer Collins, and Mike Mundt,  N. Robert Sorensen and Michael A. Quintana


Session 7: Posters


Writing Better Research Reports .......................................................................................171


Thomas B. Davis


Micron Technology, Inc., USA


A New Failure Analysis Flow of Gate Oxide Integrity Failure in


Wafer Fabrication ................................................................................................................177


Hua Younan, Chu Susan, Gui Dong, Mo Zhiqiang, Xing Zhenxiang, Liu Binghai, Ng Adrian, and Tsai Tony


Chartered Semiconductor Manufacturing Ltd, Singapore, Singapore


Instrumental Discrepancy and Relation of Stress Condition between


ESD Association and JEDEC Standards on ESD CDM Test ............................................182


Yuparwadee Satirakul, Tanawat Butngam, and Surapol Phunyapinuant  Spansion (Thailand) Limited, Nonthaburi, Thailand


xiii


Doping Profile Inspected by SEM Dopant Contrast, Wet Stain and SCM .......................189


Po Fu Chou and Chun Yen Chen


United Microelectronics Corporation, Ltd., Taiwan, R.O.C.


Case Study: Failure Analysis of Functional Shmoo Hole with


Laser Voltage Probing .........................................................................................................193


S.H. Lee1, Y.W. Lee1, K.T. Lee1, C.Y. Choi1, H.W. Shin2,  Yin S. Ng3, and T.R. Lundquist3


(1) Samsung Electronics Co. Ltd., Ki-hung, South Korea;


(2) NEOSEM Inc., Su-won, South Korea;


(3) DCG Systems, Inc., Fremont, CA, USA


In Situ Removal of Polyimide Layer Using Modified Decapsulator .................................198


C. Ramachandra1, B.M. Sweety1, U.G. Chandan1, D. Jaypal1,  Sarat Kumar Dash2, M. Ravindra2, and A.M. Khan3


(1) Tessolve Services Pvt. Ltd., Bangalore, India;


(2) ISRO Satellite Centre, Bangalore, India;


(3) Mangalore University, Karnataka, India


Surface Effect on SEM Voltage Contrast and Dopant Contrast ......................................202


Lai Li-Lung1, Huimin Gao2, and Hong Xiao3


(1) Semiconductor Manufacturing International Corp.;


(2) WuHan Xinxin Semiconductor Manufacturing Corp. WuHan, HuBei, China;


(3) Hermes Microvision, Inc., San Jose, CA, USA


Back-End-of-Line Quadrature-Clocked Voltage-Dependent


Capacitance Measurements ...............................................................................................208


Stas Polonsky1, Paul Solomon1, Mark Ketchen1, Ernesto Shiling2,


Laertis Economikos2, and Manjul Bhushan2


(1) IBM Research, Yorktown Heights, NY, USA;


(2) IBM Systems and Technology Group, Hopewell Junction, NY, USA


The Novel TEM Sample Preparation Approach for Targeted via with


Barrier/Cu Seed Layer Inspection ......................................................................................214


Wen-Fei Hsieh, Shih-Hsiang Tseng, and Bo Min She,


United Microelectronics Corporation, Tainai, Taiwan, R.O.C.


Decapsulation Techniques for Cu Wire Bonding Package ..............................................217


Dongmei Meng, Joe Rupley, and Chris McMahon  LSI Corporation, Fort Collins, CO, USA


Evaluation Trial of MEMs Devices by LSI Process Diagnostics ......................................222


Wataru Shimizu, Hidehisa Kubota, Daisuke Murahara, Noriko Nakamura,  Hirokazu Kamiyama, Tamiko Oda, and Kazuhiro Yabe


Oki Engineering Co., Ltd., Japan


A Novel Technique of Device Measurement after


Cross-Sectional FIB in Failure Analysis ............................................................................230


Chih-Chung Chang, Jian-Chang Lin, Wen-Sheng Wu,


Chih-Ying Tasi , and Ching-Lin Chang


United Microelectronics Corporation, Tainan, Taiwan, ROC


xiv


Effectiveness of Nanoprober in Detecting Single/Multiple


Bit Flash Data Gain & Data Loss Failures .........................................................................234


Rajesh Medikonduri


Texas Instruments Incorporated, Stafford, TX, USA


The Method for Retaining an Intermittent Electrical Failure Signature during the


Interconnect Immobilization Process throughout Failure Analysis ................................242


Julie Schuchman and Julie Willis


Intel Corporation, Hillsboro, OR, USA


Effectiveness of Non Destructive Physical Analysis Method Using


X-ray CT Imaging .................................................................................................................247


Akira Mizoguchi and Koichiro Takeuchi


Mitsubishi Electric Corporation, Kanagawa, Japan


Production Yield Enhancement through Failure Analysis Investigation ........................254


Fail Mechanisms Causing Single Bit Flash Data Gain in Flash Memory ........................261


easily calculate the CTE value for the component in x-direction,  Fig. 6 shows the same in-plane deformation analysis for the area           of the PCB where the component will be soldered to, for the same temperature increase. The experimentally obtained x-direction expansion of the PCB on the solder area is about 12 um, which          allows to calculate the CTE value of the PCB to be about 10x106


The solderability and the reliability of the solder joints during           product life time of components with bottom side solder ball arrays is among others determined by the amount of (out-of-plane)  warpage of the component before, during, and after the solder        height of each single solder ball.


Fig.8 shows the bottom side of a Flip Chip on Chip component


with 8 lines of solder balls. The warpage of the ball array has been


In terms of solderability, the annoying result is that along the


(quite short) length of one single line of solder balls, the height Fig. 9 shows the bottom side topography of the component at room temperature, with a height scale adapted to visualize the     topography of the mould compound. The bottom side of the          component has a concave topography, with an amplitude between


component center and the borders of typically 60-120 um.


We then applied to the component a typical lead free JEDEC


solder profile, with a top temperature of about 255C, and acquired a similar topography as the one shown in fig. 9 at 215C  in the cooling cycle, i.e. at the temperature where the solder will


solidify. The respective profiles on the mould compound and


along the solder ball line as shown in fig. 9 is shown in fig. 11.


Both profiles perfectly flattened out. The solder balls on the line  are perfectly aligned at solder solidification temperature. From       this topography we can deduce that the proper solidification of all  solder balls will not be an issue at all for this component.


represent the topography that the component would show once back at room temperature, without being soldered to a PCB. Now a Note that this topography has been obtained before any external     (more or less) stiff PCB will certainly hinder the component to heat load on the component. It therefore represents the component   surface deformation due to internal stresses accumulated duringthe assembly.


IV. SUMMARY


adds a lot more information by giving detailed insight in the component variation for varying temperatures.


stress issues. The approach is based on surface topographyIn the second application example we demonstrated that even for a analysis of ICs and assemblies under thermal stress conditions. Anperfectly behaving IC package (without any out-of-plane warpage issue), an important reliability risk concerns itspossible CTE mismatch with the PCB it is soldered on. Thus the knowledge of


assembled on a PCB, neither for practical purposes of failure risk


minimization nor for numerical modeling of the assembly. Once the component is soldered on the PCB, the stiffer one of the two


parts (lower CTE) will retain the one with the higher CTE value


development and production cycle allows an early failure orwhen temperature is increasing, and an intermediate CTE value will govern the assembly.


importance of warpage variation with temperature for assessment of the quality of a IC package. In fact, the package presented here might be rejected for too high warpage when analysed at room  temperature. However it occurs that it becomes perfectly flat at the  is related to the quality (in terms of ability to withstand typical       solder solidification temperature. The knowledge of this  topography variation opens the way to answer the relevant


The measured deformations are related to the delamination riskquestion for this package: It does not concern the solderability, but the reliability of the solder joints once the solder process is done.


z)lrw(V


Longueur=15.8mm Pt=196 μm Echelle=600 μm


900


b00


300


200


100


0□


D12346678g101112131415 mm


topography variation constitutes an ideal complement to the


widely used SAM analysis of the components. However while


SAM acquisitions are only possible at room temperature, TDM A new failure analysis and reliability assessment approach has           been developed for assessing failure modes of ICs due to thermal


important application concerns the assessment of the ability of ICs        to withstand typical JEDEC type solder cycles without too strong stress accumulation in the components. The main advantage of the the CTE value of a specific component alone is not sufficient to new technology is its predictive power, i.e. delamination or other         describe accurately the behavior of this component once it is failure risks may be visualized before physical failure occurs.


Three examples have been discussed for application of TDM in  analysis of failures risks on ICs and assemblies. In each example,analysis of the different components in an early stage of the


failure risk recognition, successive design optimizations, and thus


shorter time to market as well as lower risk of customer returns.In the third application example we highlight once again the  In the first application example the surface topography variation with temperature caused by elastic and plastic deformations due to internal stress accumulations is the only way to differentiate good         and bad components. The topography variation with temperature


solder conditions) and the expected reliability of the component.        during the solder cycle. We can conclude that analysis of the


Fig. 10: 2D profiles extracted on the component topography as indicted by the arrows in fig. 9. The blue profile corresponds to the blue arrow, the red profile to the red arrow. The solder balls are clearly resolved. This profile is obtained on a component at room temperature.


Fig. 11: 2D profiles extracted on the component topography as indicted by the arrows in fig. 9. The blue profile


corresponds to the blue arrow, the red profile to the red arrow. The solder balls are clearly resolved. This profile is obtained on a component at 215C, in the temperature decreasing part of a JEDEC type lead free solder profile.


z(μm)↑


Longueur= 10 mm Pt= 223 pm Echelle=600 pm


600


500


490


0-


。12345e78。101112131415mm


Gradient Thermal Analysis by Induced Stimulus


FA Instruments, Inc.


2381 Zanker Rd. #150


San Jose, CA 95131


(408) 428-9353


E-mail: jim@fainstruments.com


Abstract


In the field of failure analysis of integrated circuits, diagnosing functional failures is a requirement.  Traditional  beam-based analysis techniques use a scanning laser or ebeam to induce a parametric shift, which is monitored through  changes in current or voltage driven to the device.  Deep  submicron technologies frustrate these analytical methods due  to the nearly immeasurable parametric shifts externally caused  by a small signal leakage path internally.  These internal  failures can be identified functionally by timing, temperature  or voltage dependencies but the exact location of the fault is  difficult to isolate.  SIFT (Stimulus Induced Fault Test), RIL (Resistive Interconnect Localization) and SDL (Soft Defect  Localization) can identify anomalies functionally using  induced thermal gradients to the metal but does not address  how to analyze embedded temperature sensitive defects  inaccessible to the laser.1,2,3,4  Stacked die and similar 3  dimensional (3D) devices complicate the analysis requiring  destruction/removal of one or more die.  This paper will show  how to create quantifiable thermal gradients to a defect and  triangulate the location of the defect in 1, 2, and 3 dimensions  as follows:


1.  Apply a differential temperature gradient across the  device in each of the X,Y, and Z-axes.  The defect is  localized based on its measured response in the gradient  as the gradient sweeps across.


2.  Induce a gradient with a laser and use the measurement  of DC power required to relate the distance to the defect  from various locations in relation to a heat sink.


3.  Measure the time of flight of the thermal propagation


Tester


to a defect from known laser positions to triangulate the


Stim


location of the defect.


Introduction


▼


Microscope


The Stimulus Induced Fault Test (SIFT) system is the basis for


0


Time of Flight (TOFSIFT) and thermal gradient


Microcontroller


development.5  Since the SIFT scanner does not use traditional  laser scanning microscope optics, the Device Under Test


Stage(DUT)


(DUT) scan area can be submicron to 12” or more, allowing  whole boards, packages and die to be analyzed since the  scanners are stepper-based rather than internal optics based.


Session 8: Photon Beam Based Techniques – 2


Picosecond Single-Photon and Femtosecond Two-Photon


Pulsed Laser Stimulation for IC Characterization and Failure Analysis .........................268


V. Pouget1, E. Faraud1, K. Shao1, S. Jonathas1, D. Horain2,  G. Haller3, V. Goubier3, B. Picart4, L. Forli4, and D. Lewis1


(1) University of Bordeaux, Talence, France;


(2) PULSCAN, Talence, France;


(3) STMicroelectronics, Rousset, France;


(4) ATMEL, Rousset, France


OBIC Measurements without Lasers or Raster-Scanning Based on


Compressive Sensing .........................................................................................................272


Ting Sun, Gary L. Woods, Marco F. Duarte,  Kevin Kelly, Chengbo Li, and Yin Zhang


Rice University, Houston, TX, USA


Development of Laser-Based Variation Mapping Techniques – Another Way to


Increase the Successful Analysis Rate on Analog & Mixed-Mode ICs ...........................278


Magdalena Sienkiewicz1,2, Kevin Sanchez1, Luigi Cattaneo1,


Philippe Perdu1, Abdellatif Firiti2, Olivier Crepel2, and Dean Lewis3


(1) CNES – French Space Agency, Toulouse, France;


(2) Freescale Semiconductor, Toulouse, France;


(3) Université de Bordeaux, Talence, France


xv


UV Emission Microscopy Development for High Band Gap Components .....................283


M. Bouya1,2, D. Carisetti1, J.C. Clement1, N. Malbert2, N. Labat2, and P. Perdu3


(1) Thales Research and Technology, Palaiseau, France;


(2) University of Bordeaux, Talence, France;


(3) CNES Laboratory, Toulouse, France


Session 9: Package and Assembly Level FA


Studies on a Qualification Method (OSAT) of


Microchip Al Bondpads in Wafer Fabrication ...................................................................289


Hua Younan, Nistala Ramesh Rao, Ng Adrian, and Tsai Tony  Chartered Semiconductor Manufacturing Ltd., Singapore


Degradation Analysis of Thick Film Chip Resistors .........................................................293


Bhanu Sood, Diganta Das, Michael H. Azarian and Michael Pecht  University of Maryland, College Park, MD, USA


Conductive Filament Formation in Printed Circuit Boards –


Effects of Reflow Conditions and Flame Retardants ........................................................301


Bhanu Sood and Michael Pecht


University of Maryland, College Park, MD, USA


Fracture Mechanisms for Silicon Dice ...............................................................................309


Roberto Dugnani and Ming Wu


Exponent Failure Analysis Associates, Menlo Park, CA, USA


Ultimate Resolution for Current Localization by


Means of  Magnetic Techniques .........................................................................................314


Fulvio Infante1, Mathieu Gabarrot1, Philippe Perdu1, and Dean Lewis2


(1) CNES, Toulouse, France;


(2) IMS Laboratory, Talence, France


Session 10: Failure Analysis Process


Failure Analysis of Stacked-Die Devices by Combining


Non-Destructive Localization and Target Preparation Methods .....................................319


Christian Schmidt1, Michél Simon1, Frank Altmann1, and Antoine Nowodzinski2


(1) Fraunhofer Institute for Mechanics of Materials, Halle, Germany;


(2) CEA-LETI Minatec, Grenoble, France


Challenges Facing the Detection of Leakage Current in


Integrated Circuit (IC) Devices ...........................................................................................324


S.L. Toh, E. Hendarto, J. Sudijono, P.K. Tan, Y.W. Goh, H.B. Lin, Q. Deng,  H. Tan, L. Zhu, Q.F. Wang, H.L. Li, R. He, J. Lam, and Z.H. Mai


Chartered Semiconductor Manufacturing Ltd., Singapore


xvi


Analysis of a Media Processor Functional Failure ...........................................................329


Alan Putman


Intel Corporation, Chandler, AZ, USA


Session 11: Advanced Metrology and System Level FA


Start up of a Dual Beam FIB for Automatic STEM Sample Preparation ..........................334


James J. Demarest1 and Zubin DeSouza2


(1) IBM, Albany, NY, USA;


(2) FEI, Hillsboro, OR, USA


The Helium Ion Microscope for High Resolution Imaging,


Materials Analysis, Circuit Edit and FA Applications .......................................................339


William B. Thompson1, John Notte1, Larry Scipioni1, Mohan Ananth1,  Lewis Stern1, Colin Sanford1, and Shinichi Ogawa2


(1) Carl Zeiss SMT, Peabody, MA, USA;


(2) Semiconductor Leading Edge Technologies, Inc., Tsukuba, Japan


Damage Induced Field Failures of Electrical Contacts ....................................................346


Aravind Munukutla, Randy Rahn, and J.S. Lewis  Intel Corporation, Hillsboro, OR, USA


Author Index ........................................................................................................................353


Analysis Approach to Thermal Stress Issues in IC Packages


An Advanced Reliability Improvement and Failure


Michael Hertl', Diane Weidmann', and Alex Ngai2


Insidix, 24 rue du Drac, F-38180 Grenoble/Seyssins, France


Phone:+33-(0)4-3812-4280 Fax:+33-(0)4-3812-0322 Email:michael.hertl@insidix.com 2 Teltec Semiconductor Pacific Ltd., 2802 Wing On House, 71 Des Voeux Rd. Central,Hong Kong Phone:(852) 25214213 Fax:(852)28106090 Email:teltecalexngai@gmail.com


Abstract - A new approach to reliability improvement and failure


for Topography and Deformation Measurement (TDM) under     The experimental set-up is shown in Figure 1. The electronics      package to be studied is illuminated by structured light (stripe     pattern) on the sample surface. The stripe pattern is more or lessJEDEC type reflow cycles.


deformed by the sample's surface structure. The resulting image is


I. INTRODUCTION


Thermal stress generation is available by top and bottom heating


Today developers of ICs are facing reliability demands frommonitored. User defined temperature profiles with heating customers asking for zero defect quality. Besides increasing costsgradients up to +3°C/s and cooling gradients down to -6°C/s may


and efforts to achieve this reliability level, even the classicalbe imposed to the component, within a temperature range from technologies for reliability assessment are challenged. The current-60°C up to +300C.


failure characterization technologies like X-ray imaging or


scanning acoustic microscopy all follow a post-mortem approach,


i.e. they only detect failure modes where the sample is already


of time and effort is wasted in waiting for the manifestation of


failures that are supposed not to happen.


An increasing number of failure risks are due to the strongly


increasing complexity of the assemblies rather than for example to


one single weak interface. The number of layers in one single


interfaces always well being known and understood. Therefore,thermocouple


Bottom of laminated materials. This phenomenon is particularly     thermocouple          problematic in case of stacked dies, which are assembled by a


number of successive solder processes, heating up the component


to 260°C each time that a new layer is added. Therefore new          Fig. 1: Sketch of the Topography and Deformation Measurement(TDM) set-up.related to the thermo-mechanical stress of the components.


II. EXPERIMENTAL


analysis on ICs is introduced, involving a specifically developed tool


thermal stress conditions. Applications are presented including         delamination risk or bad solderability assessment on BGAs duringcaptured by a CCD camera.


and cooling elements. The current sample temperature is


experimental tools are required for the assessment of failure risks


damages like delaminations are increasing due to CTE mismatch


Bottom heating


Top


physically damaged. Thus with decreasing failure probability, a lot


heating


Camera


Light source


Sample holder


component is increasing, without the exact behaviors or layers andTop


Bottom Cooling Top


Cooling


ISTFA™ 2009, Conference Proceedings from the


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 1-5


Copyright © 2009 ASM International®


All rights reserved.


maximum solder cycle temperature, and final room temperature after the solder cycle.


The primary obtained information consists of high resolution


3D topography images of the entire assembly. The high depth of


view (up to 32 mm) of the optical set-up allows to acquire all  relevant levels of virtually every component or assembly       simultaneously, as for example PCB, BGA substrate and BGA top  surface. For each pixel, the (x,y,z) coordinates are absolutely        known. After acquisition, software zoom on each level is possible and will reveal detailed surface information on a um scale.


III. APPLICATIONS


A. Production Process Qualification


Components are often produced by different sub-contractors,


resulting in strong dispersion in terms of failure risk and


reliability. Figure 2 presents SAM images obtained on 8


theoretically identical components produced by 2 differenttheoretically identical components from 2 different


manufacturers (say A and B), after soldering. Components frommanufacturers A(series 1 and 2) and B (series 3 and 4).


manufacturer A (series 1 and 2) behaved well, while those from


manufacturer B (series 3 and 4) show delamination.


Fig. 4: Topographies of one component out of each series shown in fig. 2. Topographies are shown at initial roon temperature, Series 1Series 2 Series 3Series 4


Fig. 2: Differences in delaminations detected on


comp1comp2comp3


comp4


is二**


inital


nMeJningrate z different


，H


z9olrw


0.20


等


Tmax


6法


245℃


Gw


TSM


L0


不、


T 25°C


列


final


00 20


0.1*


024


李感


T 25°℃


20 Fig. 3: Topography following on a BGA during a JEDEC type reflowprofile. This particular BGA is part of the series 3 in Fig. 2.


150°℃165 C 173C


157C *170℃*200C* 245℃


40 60


183 C


25°C


180


160 140 120


100 80


200C


25℃


143C


z [um]


240


220


Details of component behavior during the reflow process have


6.8877


been obtained by the TDM system. Figure 3 shows the TDM


p


X direction


analysis sequence for a BGA out of series 3. The BGA is initially


7 0877


slightly concave, and shows at the top temperature a strongly


convex topography. After cooling down again to room


X.1877△


temperature, residual deformation remains, indicating non elastic


122771"


deformation during the solder profile.


D


Figure 4 shows the topographies of 4 different components, one


3611x


out of each series as indicated in Fig. 2 (Comp. 1 is one component


78LL~


out of series I, and so on). The first observation is that


58776


immediately after production, at room temperature, all 4


6077


Il


components show the same topography. The same finding is true  for electrical tests or Scanning Acoustic Microscopy analysis:


7.7877


Directly after production, there is no detectable difference


V8877


However if we look at the topography measured by TDM at


component (not soldered on the underlying PCB), when heatingup the component from 25C to 145C.


show relatively low, and relatively homogeneousseries


deformation. The components become convex, and the height


5.5943


increases gradually from the component borders to the center. The


57943


deformation amplitude in the center of the components is in the


5 8943h


order of 60-80um. On the other hand, components out of the series


5.9943x


3 and 4 show a different type of deformation at maximum solder


temperature: They also become convex, but the deformation is


6.1943p


/6,0943


mainly concentrated to the center of the components, whereas a


Ix


large stripe along the borders stays more or less flat. Additionally,


06.2943


the deformation amplitude in the component center is much higher


2


6 3943


as for components out of series 1 and 2. Typical deformations at


6.4943Iμ


6.5943


maximum temperature are in the order of 250um for series 3 and 4


I


components.


When coming back to room temperature, the series I and 2


6 64


components show very little hysteresis, i.e. their topography afterFig. 6: In-plane iso-displacemnt lines (x-direction) of a PCB


the solder cycle is more or less the same as before the cycle. In(without any component soldered), when heating up from 25C to contrast, series 3 and 4 components show residual deformation of145C.


about 70 um in the component center.


The surface topography variation with temperature is caused by


pixel


elastic and plastic deformations due to internal stress


i0.4873


accumulations. It is therefore related to the quality (in terms of


10.5873


ability to withstand typical solder conditions) and the expected


reliability of the component. The measured deformations are


10.687313μmAX~0.8pix.~


related to the delamination risk during the solder cycle.


10/0/5


L088E


B. CTE Mismatch Induced IC Failure Risk


iU0 8LE


The evaluation of coefficients of thermal expansion (CTE) is


11U873


necessary for minimizing the CTE mismatch of materials to be assembled. Otherwise, if the CTE of components and PCB is not


11.1873


matched, permanent shear stress will be loaded on the solder joints


11.2873


between components and PCB during cooling down of the


11.3873


assembly (hardening of the solder paste) after the solder process.


The higher the permanent shear stress is, the higher will be the


11.4873


With TDM, in plane deformation (CTE) analysis is possible byFig. 7: In-plane iso-displacement lines (x-direction) of the


digital image correlation for images taken at differentcomponent shown in Fig. 5 soldered on the PCB shown in Fig. 6,temperatures.


between all 4 components, no matter what kind of test is applied.


Fig. 5: In-plane iso-displacement lines (x-direction) of a maximum temperature, a clear difference is seen between on the one side components out of series I and 2, and on the other side


components out of series 3 and 4. Components out of the first two


failure risk of the assembly during its life time in field.


when heating up the assembly from 25C to 145C.


For detailed analysis, 2D profiles along straight lines have been


in x-direction when the component is heated up from 25°C toextracted from the topography in fig. 9. Fig. 10 shows the profiles


145°C. It can be deduced that, for this temperature increase, thealong the red and blue arrows indicated in fig. 9, for room component expands by about 16 um in x-direction. Together withtemperature conditions (thus for the same conditions as those the known absolute size and the temperature increase, one can thusprevailing in fig. 9). It can be seen that the TDM equipment if able to resolve single solder balls. The height of a solder ball can be which is found to be 14x10-6 1/K.


deduced from fig. 10 to be about 350 um. It can also be seen that


the valleys of the profile extracted along the solder ball line overlap perfectly with the blue profile, extracted just besides the


solder ball line. This observation might prove the reliability of the


topography extracted on the solder ball line, along a quite complicated peak-valley structure.


1/K.


Finally fig. 7 shows the same in-plane deformation field for the


z(μm)


assembly, i.e. for the component shown in fig. 5 soldered on the PCB shown in fig. 6.  The experimentally obtained CTE value of


。


C


190T崩


the assembly is 11x1061/K.


4


This analysis shows that the CTE values of the component and


160


the PCB differ by about 40%, which is a quite important


140


mismatch. The CTE of the assembly is very close to the CTE of


6


120


the PCB alone, which means that the PCB governs the in-plane


8


deformation characteristics of the assembly. The components have


-100


to follow the deformation imposed by the PCB. From that it is


10


90


directly clear that the connectors of the component will face


0o


permanent shear stress during the entire assembly life time.


14


40


16


20


C. Flip Chip on Chip Solderability Analysis


mm


Fig. 9: Bottom side topography of the Flip Chip on Chip


component. In this representation, a software thresholding of the height scale is done in such a way to show details of the mould


compound topography. Other thresholdings allow to check the process.


analyzed by TDM.


difference between the central ball and the two balls on the outer


side of the lihe is in the order of 100 um. Therefore, when only


inspecting this part at room temperature, the question of its solderability would be an issue.


8: Bottom side of the Flip Chip on Chip component. ForFig.         time of the component on its PCB, we have to keep in mind theHowever, for the assessment of the solder reliability during the lifeoptimum solderability, all solder balls should be coplanar at all temperatures during the reflow cycle.


profiles obtained at room temperature (fig. 10). These profiles


come back to its usual room temperature shape, once the solder   being solid. Therefore, permanent pull stress will be applied to themanufacture of the component.central solder balls of the component during the entire life time of Fig. 5 shows the in-plane iso-displacement lines of a component


X-Y-Z


Field of view limitations of objectives on LSM (Laser Scan  Microscope) based equipment are eliminated with SIFT.  Data  output is to a PC via the microcontroller and contains data  from the scan for X, Y, Z and multi-channel data for each step  in the scan.  This data is coordinate data but can also be


displayed photographically.  Channel data consists of pass/fail  signals from the tester as well as analog information.  The  scan and step is user defined based on spot size.


Unlike LSMs, SIFT uses a stationary beam and moves either  the stage or the microscope head in a raster scan pattern.  Figure 1 is a block diagram of the apparatus.  A microscope  and stage are equipped with stepper motors to control the X, Y, and Z motion of the scan.  Z control is necessary to control  the spot size of the stimulus by either focus or proximity  control of the source.  Laser based SIFT uses a laser attached  to the top camera port of the microscope and can be any  wavelength compatible with the selected optics.  The selected  objective, aperture, and focus control spot size, in this case.


High power solid state or CO2 lasers are mounted in place of  the microscope and raster scanned over large areas for thermal  and TOFSIFT.  The stimulus can also be introduced over the  DUT with the raster applied to the stage.  This method of SIFT  can be thought of in the same way a probe is positioned over a  DUT by moving the stage.   The added requirement for  TOFSIFT is the ability to position the laser at predetermined  locations and modulate/raster the laser to determine the length  of time the defect “responds” to the thermal wave and the  corresponding length of time for the defect to cool.  These  time measurements are obtained at multiple locations to  triangulate in 3D the location of the defect akin to Global  Positioning System (GPS) trilateration methods.6,7


Figure 1.  Block Diagram of SIFT Scanner.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 6-15


Differential TLS Methods


Differential TLS builds the foundation for TOFSIFT and in its  own right simplifies the task of isolating the regions of  interest.  Figure 2 is a curve showing an unexpected jump in  Idd at 10 volts.  The hysteresis moves to lower voltages at  elevated temperatures with minimal change in Idd.  Two SIFT  scans at 1428nm were performed thermally similar to  TIVA/OBIRCH methods at 8 volts, for the lower and upper  portions of the loop.   The 2 scans were overlaid in green and  red with blue as the background.  Figure 3 shows the  differential areas in either green or red, with all yellow regions  indicative of a common mode response.  Unfortunately this  data does not clearly show which areas stimulated by the laser  improve or degrade the hysteresis loop.


Since the laser coordinates are known, the laser can be steered  to and parked on each of the regions of interest maintaining  constant power and focus.  Two related nodes are isolated in  figure 4 responsible for the threshold shift.  This example  illustrates the false positives created when a focused laser is  used to scan across the die.  Gradient SIFT and TOFSIFT  avoid these situations since the temperature differential is not  severely localized.


V(Volts)


Figure 2.  Idd curve showing unexpected hysteresis activating  at 10 Volts and relaxing at 6 volts.


Figure 3.  SIFT TLS scan of differential bandgap shift.  Green  and Red areas (arrows) show regions of shift associated with  the hysteresis loop.


Figure 4.  Locations responsible for shifting the hysteresis to  lower voltages from figure 3.


Thermal Stimulus


Parametric issues surrounding thermal management need to be  understood so that appropriate power levels can be chosen for  both frontside as well as backside analysis.  A simple way to


DUT Voltage=0.000V;DUT Curent=0.000mA


determine the required energy is to look at a diode to substrate


0.675157


on the device under test.  Generically, the substrate diode


0.540125


associated with a given input pin is a known temperature


2 0.405094


sensor.  Figure 5 shows the change in forward voltage for


二0.270063


0.1mA, 1mA, and 2mA respectively.


0.135031 0 0


3.953417.9068211.860215.813619.767


Diode Forward Vs Temp


400


0.1


0.2


武


100.3 3人


p0.4 0


60.5


面


0.6


0.7


0.8


50


150


￥0


Celcius


.1 mA


*


1 mA


，M


2 mA


.


Figure 5.  Typical diode forward drop versus temperature  relationships for 3 current drive levels.


Whereas the forward voltage may vary process to process, the  V can still be used to measure temperature excursions as  shown in equation 1.


Equation [1] V/2.0E-3  T  @0.1mA


V/1.6E-3  T @1mA


V/1.5E-3  T @2mA


V  = Change in diode forward voltage  T = Celsius change in temperature


The next parameter to evaluate is the thermal propagation in  silicon for frontside and backside.  For frontside, the excursion  in temperature is fairly small, on the order of 5 to 10 degrees, as shown in Figure 6.  Note the small fast waves are the on-off  pulses of the laser and the general slope downward represents  general die heating.  Since the substrate is tied to a copper  paddle, the general die heating is reliant on the paddle, which  is floating.  The temperature gradient is only 4 to 5 degrees  Centigrade due to the thermal conduction of the die and  paddle.


Figure 6.  Thermal excursions with a pulsed IR laser on the  frontside of silicon.  Signal is inverted.  Scale is Horz.: 2


sec./div., Vert.: 50 C/div.


For the backside, a die was thinned to 30 um remaining silicon  thickness in order to evaluate lateral heat spread with very thin  substrates.  Lateral effect vs. thickness and resolution will be  discussed in applicable sections later in the paper.  Note the  rapid ramp and gradient now better than 100 0C.  Since the  silicon is thin and has greatly reduced volume there is much  less lateral heat spread and a high differential thermal  gradient.


Figure 7.  Thermal excursions with a pulsed IR laser on the  backside of silicon.  30um thickness.  Signal is inverted. Scale  is Horz.: 1 sec./div,Vert.:100 0C/div.


Thermal Stimulus using CW lasers


Normally for thermal stimulus with a laser, wavelengths  outside the indirect bandgap of silicon are required, such as


1.3 um, to avoid generation of photocurrents.1,4  It is difficult  to get the power necessary in a large spot to heat significantly  at this wavelength due to numerous factors such as laser  power limitations.  The silicon doesn’t heat at this wavelength.  The primary heating is accomplished from absorption of the  laser energy by the metal, which typically scatters a significant  amount of the radiation.  As reported by Cole et al, the  temperature gradient at metal is roughly 10C/mW with typical  heating of the metal up to around 300C with a 1.3 um laser.1   Temperature excursion of the related silicon will be typically  less than 10C, inadequate for silicon based thermal analyses.


Ordinarily, shorter wavelength lasers generate too much  photocurrent to be useful thermally.  Several laser  wavelengths of importance, due to their ability to generate  higher power, are: 532nm, 808nm, 940nm, and 1064nm.  All  of these wavelengths will generate photocurrents unless they  are masked from the die.   This is accomplished by applying  high temperature flat black paint to the die surface by spray, brush or spin deposition.  The 532nm laser does not typically  need to be masked when used backside due to the absorption  of the laser by the silicon substrate.  Carbon sputtering or  carbon paint (preferred) can also be used backside or frontside  if the connections are passivated .  A 5 watt 808nm laser was  chosen to locally heat the surface with around 1 to 2 watts  depending on spot size and desired heating for the above  work.  For the remainder of the paper, a CO2 laser will be  used.


Gradient Thermal Analysis


A straightforward method to localize a thermally sensitive  region either parametrically or functionally is possible when  opposing ends of a copper paddle are held at two different  temperatures. A corresponding precise thermal gradient will  form across the surface.   With a quantifiable temperature  gradient across the device in X, Y, and optionally Z; the  location of the defect can be better localized.    Similar to


Magnetic Resonance Imaging except that the field gradient is  replaced with a thermal gradient and the defect is the  detector.8   Two precision temperature controllers are required  to control and “walk” the gradient across the wafer as shown  in figures 8 and 9.  The greater the gradient and the tighter the  tolerance of the defect to temperature change, the better the  triangulation of the defect.  The technique assumes the defects  are not distributed, however a cluster can still be localized.  Once the X position is approximately obtained with a low  level gradient, the differential is increased to more precisely  localize the defect while avoiding the continuity issues that  walking extreme differential temperatures across the wafer  create.  The wafer or Peltier elements are repositioned 90  degrees in order to localize the Y direction.  Since the  technique is effectively static, the test time is irrelevant.  Loop  testing or 1 shot testing can be performed for pass/fail with a  gradient scan or binary search for the threshold temperature at  which the gradient is locally at the fail temperature in  conjunction with the defect.  The probe card can be easily  positioned over the differential heating system.   Wafers that  dissipate heat while tested can still be analyzed, however, the  thermal offset will need to be factored into the gradient  measurements and/or a burst mode test will need to be  performed in order to minimize unwanted substrate heating.  Forcing a gradient across a thick metal plate of which the  wafer is attached and using closed loop control on the ends is  the best method to minimize these issues but takes  significantly more power from the controllers if large  gradients are desired. Heat load of the Peltier needs to be  considered for long term dissipation into the wafer chuck.  A  high power temperature controlled chuck  capable of cooling  serves well to obviate these issues.  Although 2 Peltier units  are shown here, a chuck could be used to control the cold side  of the gradient with a Peltier, liquid or resistive heater forcing  the other side.


Referring to equation 2, precision control of the gradient  means obtaining the best triangulation data in conjunction  with the   minimum temperature change required to detect the  defect.


Equation [2]


Resolution=Gradient*Precision/DChangeResolution=Gradient*Precision/Change


loo


If the minimum temperature change required to see a  transition from pass to fail ranges from 40.10C to 40.20C, then  the defect will be resolved (Precision/DChange) within athe defect will be resolved (Precision/Change) within a  gradient of 0.10C.  These assumptions are based on precise  temperature control and a single defect.  A chosen gradient of  10C/mm will yield a best-case resolution of 100um in X and  Y.  Correspondingly, the measurement precision of leakage as  a function of temperature and the slope of the induced gradient  define resolution.  If a device is characterized with a defect  which changes by 1 ohm/0C and the precision of the  measurement is 0.01 ohms then the thermal gradient inside


0.010C is within the range of error.  A gradient of 1000um/0C  will then infer the triangulation is within 10um in X and Y.


In order to minimize the impact of changing temperatures with  a sweeping thermal gradient, the defect can be characterized


with a few precise data points at various temperatures  resulting in a best fit line or curve applied to the data.  A static  gradient is then applied and the measured leakage matched to  the point on the curve.


Fig 8.  Wafer section across 2 Peltier temperature controlled  plates for differential temperature control.  The wafer was  thermally coupled using mineral oil for the experimental data.  Local vacuum on each brass plate may also be used to hold  the wafer edges.


|FA FA Instruments TCS|FA FA Instruments TCS|-0X|LAIFA Instrumenls TC5|sox|sox|
|---|---|---|---|---|---|

|UV Contal Themal Conhol| Opiona|UV Contal Themal Conhol| Opiona||UVControl ThemalCorhal Opions|||

||Heal/Cool Element DUT  Temp|XPoke:|HeaPCool Eletent- DuT  Temp|%Power||

||TECHea/Eool 22925|17.92|TECHeal/ Cool 21.923|0280|0280|

||HealCool|100%|He ekCool|||

||HealCool|100%|He ekCool|i-||

||||. .|Temp Control in degC||

|EnableP1DTemp Central|EnableP1DTemp Central||Enable FID Temp Control|||

|60.000 60.044|60.000 60.044|,|25.000÷ 24.952|, ,||

|Se lpoint Se rs o|Se lpoint Se rs o|"|Sespoint Sensor|. . .||

|Use ControlSensor|Use ControlSensor|0% 汁|CU se Con tral  Sense r|||

|Use Elemen: Senso:|Use Elemen: Senso:||Use Elemert  5ero|||

|Elnt Conent/Pai=059V7.0W|Elnt Conent/Pai=059V7.0W|厂|Elrr t  Durren: / Por-0.036/0.3W|||

Figure 9.  Differential temperature control panels (upper  image) and the controllers (lower image). Each panel can  control the forcing temperature, quickly within 50 mK.


Infrared investigation with an InSb camera as seen in figure 10  was used to measure the quality of the gradient generated  across the wafer.  Carbon paint was used to calibrate out  issues with black body radiation and pixel registration errors  during measurement.


05


1015


Distance (mm)


Fig 10.  350um thick wafer section with induced thermal  gradient.  Temperature gradient is 150C across a 25mm gap.  Carbon paint was used to validate the gradient while imaged  with an InSb thermal camera.  This step was only used to


10 mm


validate the gradient data and is not necessary for the actual  work.


Package devices are more problematic due to the differing  materials and hence thermal conductivities.  Additionally, the  socket fixturing must be customized with direct contact made  to the edges of the internal copper paddle of the device in  order to induce a decent thermal gradient.  Figures 12 through  14 illustrate the problem.  The package was backside milled  and the die thinned as in normal backside practice to 75um.  The reason for thinning was to better match the thermal  gradient of the plastic to that of the die since a thin die has less  lateral conduction.  Unfortunately, for a 150C spread across  the package the expected gradient across the die portion was


anticipated to be not much less than 120C and was found to  actually be 10C.  This method therefore requires direct thermal  connection to the conductive substrate or paddle using  machined fingers to make contact.  Package sockets can be  incorporated with this, especially in the case of flip chip or  bump chip technologies where either the back face is perfectly  accessible or a large area heat sink can be induced with a


40.00


thermal gradient in the case of power processors.


38.15


36.30


34.45


32.60


30.75


28.90


27.05


25.20


23.35


21.50


19.65


Fig 11.  TQFP package across the differential temperature  controller.  Double sided Kapton tape was used to temporarily  attach the package edges to the plates.  The die was backside  thinned to 75um.


40.69


35.81


30.93


台


26.05


n 8 0


21.17


he


习


30


Figure12.  InSb thermal image of the gradient across the  package.  Note the package has larger temperature steps  while the die has smaller steps.


Figure 13. 3D profile of figure 12 above.  The profile shows  even with the thinned die at 75 um, the silicon develops a  small gradient in relation to the package.


Figure14 Line profile from figure 13.  The slope illustrates a  10C gradient on the silicon in spite of a 120C gradient across  the package in that region.


Laser Induced Gradient Thermal Analysis


The thermal laser can be used in place of one of the 2 Peltier  controllers or opposite a heat sink where package complexities  obviate access.  A thin slot can be milled along the package  edge on angle to allow access with the laser to the die edge.  Carbon paint can be used to assist laser absorption as long as  the die edge has no delamination issues to allow the carbon  paint to wick into sensitive areas.  The laser serves as the heat  source vs. the heat sink.  The steady state power required to  reach the transition threshold is noted at known locations.  A  line scan can be used to uniformly inject higher levels of  average power along an entire edge to maintain and “walk” the gradient across the region of interest.  The power required  is recorded preferably for each of the 4 edges or at select  points appropriate to the geometry of the bulk region.  This  method allows the measured power of the laser required to  reach the trip point or threshold associated with the failure to  be related to the distance to the defect.  Select input pins  should be used for temperature calibration and validation of  the linearity of the gradient across the die.  Nonlinear effects  can be mathematically line fitted by utilizing the multiple pad  diodes available on the device before actual testing begins.  Optimization of the above techniques can be accomplished by  restricting the gap the gradient is applied.  The gradient can,


therefore, be large while avoiding excessive temperatures at  the edges.


Time of Flight Thermal Analysis (TOFSIFT)


2 200 150


All of the prior methods require a heat sink and source in


order to create the thermal gradient.  In the case of 3D


structures such as stacked die technologies, it is difficult to


contact the edges of the die since the individual die are


12


1620


typically of differing dimensions.  The apparatus for TOFSIFT (Time of Flight Stimulus Induced Fault Test) consists of a


24X/mm Y/mm


thermal laser, a programmable fast A/D or comparator to  detect the threshold from the part either as pass fail data or  analog change and the ability to control the hysteresis of the  on to off threshold point at which the laser is fired.  The laser  power is controllable for both the on power and the off power  states.  (Typically the off power is 0).  The local heating of the  device is controlled by the dwell time of the laser required to  trip from pass to fail.  Averaging for a matrix of locations  results in improved triangulation.


39 37


For this emerging technology, a 10 um CO2 laser was chosen


5 n


35


in order to heat a controlled spot with a diameter down to


533


100um.  The diameter of the spot is less important than the


3 031


damage threshold.  Accurate placement of the spot is key since


29


the triangulation is determined proportionately by the ratio of


27


the radius.  Identification of the locus or intercept of the


25


corresponding radii can be scaled proportionately to match the


15


physical distance even if the speed of the traveling thermal


wave is unknown. The ratio of the TOF between known  coordinates to the defect is scaled to best fit the locus in the  case where measuring the TOF is impractical.  The spot needs  to be large enough to heat the die without local damage.  If the  laser modifies the surface, the black body radiation absorption  will change affecting the measurements.  The power used was  1 to 1.5 Watts with a 0.5mm dia spot.  The laser range is from  100mW to 10 Watts and for larger spot sizes in pulse mode  the higher powers are indeed used.


Parametric issues surrounding thermal management need to be  understood so that appropriate power levels can be chosen for  both frontside as well as backside analysis.  A simple way to  determine the required energy is to look at a diode to substrate  on the device under test as explained above.  Generically, the  substrate diode associated with a given input pin is a  temperature sensor, which can be calibrated.  Figures 15 and  16 show the response of two input pins on opposite sides of a  5mm die.  The hysteresis of the trip point to turn the laser on  and off is determined experimentally.  If the trip points are too  close together, the laser can fire prematurely.  Ideally, the on  to off states should be chosen at around a 50% duty cycle  upon setup at the first laser injection site.  The cooling of the  die and heating by laser normalize out die temperature issues  and allow the die to act as a thermally stimulated oscillator.  The frequency of the oscillator changes in proportion to the  distance of the injection point to the defect or bond pad diode  monitor.  Candidates for this technique are devices that exhibit  either a repeatable temperature instability or a temperature  dependent resistance change.  A characterization of the failure  first is paramount to understanding the thermal gradient range


and hence laser power/hysteresis settings.   The montage in  figure 17 is a sequence of thermal images during the on  portion of the laser pulse.  The thermal propagation from the  corner of the square copper paddle is clearly shown.  The  cycle times were on the order of 500 to 900msec for this  particular sample to an input diode chosen as the “defect” hereafter.  The sample is a TQFP package 14mmx14mm with  an exposed copper paddle from the backside milled using the  ASAP-1.  The die is 500um thick and the Cu paddle is 250 um  thick.  The total Z distance to the die face is 750um.  Carbon  paint was applied to normalize the laser absorption.  The laser  was programmed for 4 corners of the paddle and the center in  micrometers, the results follow:


Site A: (5880,0,0) 680msec.  Site B: (0,0,0) 976msec.


Site C: (0,5260,0) 832msec.


Site D: (5880,5260,0) 512msec.


Center Site E: (2940,2630,0) 424msec.


Measured propagation time:895msec/5880um


16 Apr 200


12:38:03


Figure 15.  Thermal excursions with a pulsed IR laser on the  backside of silicon.  75um thickness.  Scale is Horz.: 2  sec./div.,Vert.:10C/div.  A clear difference can be seen between  the diodes.


Ch2 10.0mVM 2.00s A Ch1 广 3.38 V


C1310.0mV


16 Apr 2009


12:23:21


Figure 16.  Thermal excursions with a pulsed IR laser on the  plastic backside of the intact PQFP package.  The low thermal  conductivity of the plastic results in an inadequate difference  signal for the analysis.


Scale is Horz.: 2 sec./div.,Vert.: 1 0C/div.


Figure 17.  Montage of the thermal wave propagating for  one  on_cycle from the lower left corner.  Each frame is 1/30 sec. taken with an InSb camera.  Note the wave front gradient (slope) reduces as it propagates.


All the laser points are in the Z=0 plane.  The implications will  become clear later in the paper.  For now consider the 2  dimensional case.  Referring to figure 18, the 3 data points  furthest are chosen and overlaid with radial patterns  proportional to the measured laser period.  From this, the  propagation time is determined and the location of the defect


Ch2 10.0mVM 2.00s A Ch1  3.38V


is already approximately determined.   Triangulation is shown


10.0mV


in figures 19 and 20 by using 3 circles and calculating the  intercept points per the following formula in Equation [3]:


Equation [3]


X2+Y2=R2 (for sites A, B, C)


A-B=B-C (Intercept calculation for 3 circles A, B, C)


Sites D and E overlap the identified location.  Site E is in the  center and Site D is closest to the defect.  The Z plane has


been ignored up to this point but D and E have significant Z


angle with the opposite side of the triangle in Z at 750um


below Z=0.  Since the purpose is to triangulate in 3D, the 2D  case does a disservice to the acquired data.  Using the


intercept method is convenient but as shown in figure 20


unwanted measurement error results.  Additionally, since the  defect is not on the same z=0 plane, error compounds as the


slope of the z vector increases.


Figure 18. Radial spread patterns illustrating the propagation  of the thermal wave from 3 corners of the copper paddle in a  PQFP package accessed from the backside.  The actual fail  location is at the conjunction of the 3 arcs and is an emission  overlay aligned from an equivalent part to validate the  technique.  A CO2 laser was pulsed to induce the thermal  wave in conjunction with a feedback loop.


7804


Figure 19.  Triangulation in microns of the 3 thermal injection  points to the identified locus in 2D from figure 18 above using  intercepts.  The distant points must be used to minimize Z  error.


Figure 20.  Zoom view of the locus from figure 19 illustrating  the resultant error with the intercept.


Plotting the 3D case clarifies the remaining 2 issues.  Equation  set 2 is a 3D matrix set for all 5 data points.  The propagation  period for Z is longer than X-Y due to the die attach.  In this  case, the copper paddle is heated.  The  propagation takes


2.5X longer to reach the die through the die attach.  The ratio


1.104


is calculated by the Pythagorean theorem from the center point  to the identified locus in order to approximate the hypotenuse  length.  Applying equation set 4 yields a 3D view of the


J7500


spherical propagation waves as shown in figure 21.  The first 5  equations define the spheres where the center x,y,z location is  defined by xa,ya,,za for sphere a through xe,ye,,ze for sphere e.


5000


The radius of each sphere is the time amsec through emsec  divided by the propagation time constant smsecum in  milliseconds/micrometer.  Variables t and u define the


2500


continuous set of points to plot in 3D space defining a portion  or the entire sphere surface to be displayed.


00


-5000


-25000


75001.104


-2500


-500f


Equation set [4]


z[1900


Constants:


smsecum=895msec/5880um


amsec=680msec


bmsec=976msec


cmsec=832msec


dmsec=512msec


emsec=424msec


xa=5880um


ya=0um


za=0um


xb=0um


yb=0um


zb=0um


xc=0um


yc=5260um


zc=0um


xd=5880um


yd=5260um


zd=0um


xe=2940um


ye=2630um


ze=0um


The TOFSIFT method has been successfully used to localize  both leakage failures and functional failures.  Failures with


hysteresis or instability are problematic.  Hysteresis failures  must be analyzed 1 shot or with a reset to clear the hysteresis  for each new measurement cycle.  Unstable devices need


some repeatability to be analyzed.  The severity of the


instability dictates the resolution.   Errors in the Z model for  stacked die have been observed similar to the problem with


die attach in figure 21.  Different thermal conduction of the


die attach requires a compensator (multiplier) to be applied


depending on the die stack.  Currently, this is determined


experimentally by comparing the TOF data from several


additional locations roughly equidistant from the approximate  location of the defect.  Delamination/void issues can be


overcome with carefully milled access points along the die


x]xasint sinu


edges of the stacked array.


y=Ya+sint cosu1


cost


xXbsint sinu]yYb+sint cosubusecSmsecum)x7Xcsint sinuCmseey=Yc+sint cosuSmsecum )xXd


yYd+sint cosu'sint sinu(comsee[Z]ZdcostSmsecum xXe[sint sinu(emsecy=ye+sint cosu(Smsecum)zZelcost x7[480O][4800]


y


[z]1900


x7


y3870u,u=0...2


「4800]


[1900]3870=3870


,t=0...2π,u=0...Iπ,t=0...2x,u=0...1x


zZccost


),t=0...2x,u=0...1x


2Zbcost


J,t-0...2r,u-0...1x Smsecum


[z]_Za


amsec,t=0...2x,u=0...1x


Figure 21.  Error from the edge coordinate closest to the  defect.  The error is caused by the fact that the injection point  into the copper paddle is off the edge of the die by approx. 500um.  The thermal wave must couple up to the die further  from the stimulus laser causing the spherical pattern (red) to  appear too large in relation to the yellow dot (defect) at the  locus of (4800, 3870, 750).


Ongoing Work


GPS devices calculate position using a technique called “3-D  multilateration”, which is the process of figuring out where  several spheres intersect.7   In the case of GPS, each sphere  has a satellite at its center and for TOFSIFT the laser is at the  center; the radius of the sphere is the calculated distance from  the laser spot to the defect per equation 5.


Equation [5] d= sqrt((x2-x1) 2+(y2-y1)2+(z2-z1)2)


Ideally, these spheres would intersect at exactly one point, with one possible solution to the current location, but in  reality, the intersection is a culmination of near proximity  surfaces. The defect can be located within any point in the  proximal area compounding the error.  Precision is said to be “diluted” when the area grows larger,  dilution of precision or (DOP) is a measure of the error factor.  The same concepts  apply to TOFSIFT and as such, strikingly similar algorithms  are used to calculate position but on a considerably slower  timescale at shorter distances.  The process can be automated


to position and fire the laser as well as calculate the locus with  averaging to minimize error.  The (TOA) Time Of Arrival or (TDOA) Time Difference Of Arrival are two of multiple  algorithms available to provide a best-fit solution to  multilateration.  The chosen CO2 laser has poor power  stability and slow response since it is a gas discharge laser  requiring power control through pulse width modulation.  Trilateration improvements are being explored for both solid  state and gas discharge lasers.  Finite element models can be  incorporated to improve 3D triangulation in complex packages  and used in conjunction with CAD views.


Conclusions


An emerging method of failure analysis has been presented  which now allows buried defects to be triangulated using  thermal gradients. The gradient is either gradually walked  across the die while the device is tested or pulsed to determine  the propagation delay time to the defect.  Inducing a controlled  gradient either static or dynamic across each axis allows the  defect distance to be identified and matched to the gradient.  Once this is accomplished in X, Y, and Z; the embedded  location of the defect is known.  Triangulation to 10um has  been shown in 2D space with static thermal gradient methods  and 100um in 3D space with pulsed time of flight methods.  The coordinate data allows localization of failures in stacked  die as well as single die for localized small  access holes to be  milled.  Traditional techniques can then be used to triangulate  further, if required.  This technique works both with traditional  parametric measurements as well as thermally sensitive soft  defect test failures.  Existing input pins are used to assist in  calibrating the gradient for triangulation or the data may be  scaled for best fit of the trilateration data without benefit of  calibration points.


Acknowledgments


To my wife Mayra for her devotion and patience with my  continuing to burn the candle at both ends and my son  Christopher for helping assemble the video animation files.


References


1. U.S. Patent # 6,078,183 “Thermally-induced voltage  alteration for integrated circuit analysis,” Cole, Jr.; Edward I. Sandia Corporation (Albuquerque, NM)


2. Bruce et al., "Soft Defect Localization (SDL) on ICs", Proceedings From the 28th ... Symposium for Testing and  Failure Analysis (ISTFA), pp. 21-27, Nov. 3-7, 2002.


3. E.I. Cole, P. Tangyunyong, CF Hawkins, MR Bruce, VJ  Bruce, RM Ring, WL Chong “ Resistive Interconnect  Localization” ISTFA 2001 pp. 43-50.


4. J. Colvin,”Functional Failure Analysis by Induced  Stimulus” ISTFA/2002 Proceedings, pp. 623-630.


5. U.S. Patent # 7323888 B1 “System and Method for Use in  Functional Failure Analysis by Induced Stimulus,” Colvin; James B.


6. Ivan Stojmenovi,”Handbook of Sensor Networks: Algorithms and Architectures” p. 290.  Wiley


SBN: 978-0-471-68472-5 Hardcover 552 pages.


7.    R. Bucher and D. Misra,” A Synthesizable VHDL Model  of the Exact Solution for Three-dimensional Hyperbolic


Positioning System”


VLSI Design, 2002 Vol. 15 (2), pp. 507–520


8.    J. Hornak, ”The Basics of MRI”


http://www.cis.rit.edu/htbooks/mri/index.html


Measurement of Bit Leakages in a Functional SRAM


Xiaowei Deng, Wah Kit Loh, Beena Pious, Jayesh Raval, Bashar Khan, Larry Liu, Taylor Lowry, DB Yoon, Theodore W. Houston, Randy McKee, Abha Singh Kasper, Dan Corum


Texas Instruments Inc., Dallas, Texas, USA   x-deng@ti.com


A direct bit leakage measurement (DBLM) scheme is  proposed and implemented in 8Mb and 32Mb SRAM’s in  45nm and 28nm technologies. It allows, for the first time, direct and nondestructive measurement of various defect  induced leakages in each bit in a functional SRAM. It thus  enables collection of various defect induced bit leakage data  for low-cost and fast failure analysis. It also enables collection  of massive bit leakage data for statistical evaluation and  location sensitivity assessment.


With continued scaling in VLSI technology, SRAM bits  become increasingly susceptible to subtle defects caused by  process variation, etc. Consequently, the measurement of  defect induced bit leakages for failure analysis and variability  assessment becomes important. Traditional test structure  based bit leakage measurements, e.g., [1], provide limited  amount of data and are not linked to bit fails in a functional  SRAM. Therefore, they are generally not suitable for failure  analysis and accurate variability assessment. Nanoprobing  based bit leakage measurements, e.g., [2], although linked to  bit fails in a functional SRAM, are destructive and time  consuming, yet provide even less amount of data with which  fast failure analysis and variability evaluation are prohibitive. Direct bit line access [3] and direct bit transistor access [4] allows each bit or each bit transistor in a functional SRAM to  be characterized; however, direct measurement of defect  induced bit leakages is not available. In this paper, a direct bit  leakage measurement (DBLM) scheme is proposed. It allows, for the first time, direct and nondestructive measurement of  various defect induced leakages in each bit in a functional  SRAM.


Circuit Structure


As shown in Fig. 1, a DBLM SRAM is identical to a typical  functional SRAM except that it has direct bit line (BL) access  and independent control of array ground supply (VSSA), array  power supply (VDDA), array Nwell supply (VNWA), word  line (WL) driver power supply (VDDWL), and bit line precharge supply (VDDBL). Local bit lines, bit line true (BLT) and bit line bar/complement (BLB), are respectively  multiplexed to bond pads, BLT pad (PBLT) and BLB pad


(PBLB), through multiple levels of analog multiplexers to  allow direct bit line access, similar to [3] and [4]. VSSA, VDDA, VNWA, VDDWL, and VDDBL are directly supplied  from pads and are separated from core power supply (VDD) and chip ground (also tied to substrate; not shown).


古


Figure 1:  Schematic illustration of DBLM circuit structure. M1-6 are respectively the left pass gate, right pass gate, left  driver, right driver, left load, and right load transistors of a  6T SRAM cell. SNT and SNB are respectively the left and right  storage nodes of the cell. PREZ is a bit line pre-charge enable  signal (active low).


WL


PBLT


PBLB


VDDA


VDDWL


VDDBL


BLT


BLB


VDD


产


SNT


SNB


PREZ了可 WL Driver


Multiple levels of □


analog multiplexers


M1


M2


M3


M4 M5 lkdM6


VSSA VNWA


The DBLM scheme has been implemented in 8Mb and 32Mb  SRAM designs fabricated in 45nm and 28nm technologies. The die photo of an 8Mb DBLM SRAM fabricated in 45nm  CMOS technology is shown in Fig. 2.


131111


Figure 2:  Die photo of an 8Mb DBLM SRAM fabricated in  45nm CMOS technology.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 16-20


Test Methods


In DBLM test mode, the bit lines of the addressed bit are  multiplexed to PBLT/PBLB pads through analog multiplexers. Various bias voltages are applied to PBLT/PBLB and various  supply pads and then currents are measured from PBLT/PBLB  pads to allow measurements of various bit leakages. Methods  for some bit leakage tests are given below. Methods for other  bit leakage tests can be devised based on the same principles. In the following descriptions of test methods, a nominal  voltage of 1.2V is assumed. Each of this and other voltages  mentioned in these descriptions of test methods can be of a  slightly different value without affecting the test results.


Storage Node to VSSA Leakage Test


As shown in Fig. 3, to measure the storage node to VSSA  leakages, VDD and VDDWL are held at 1.2V. PBLT/PBLB  and other supply pads are held at 0V. WL is on. 1st and 2nd  PBLT/PBLB currents are measured with VSSA at 0V and


0.6V, respectively. The (1st–2nd) PBLT/PBLB currents are  calculated as the SNT-to-VSSA and SNB-to-VSSA leakages, respectively. The storage node to VDDA leakages, storage  node to VNWA leakages, and storage node to storage node  leakages are similarly measured.


Figure 3:  Schematic illustration of the DBLM bias conditions  for measuring storage node to VSSA leakages.


BL to WL Leakage Test


As shown in Fig. 4, to measure the BL to WL leakages, VDD  is held at 1.6V. PBLT/PBLB and other supply pads are held at


0.6V. 1st and 2nd PBLT/PBLB currents are measured with  WL off and on, respectively. The (1st–2nd) PBLT/PBLB  currents are calculated as the BLT-to-WL and BLB-to-WL  leakages, respectively.


Storage Node to WL Leakage Test


As shown in Fig. 5, to measure the storage node to WL  leakages, VDD and VDDWL are held at 1.2V. PBLT/PBLB  and other supply pads are held at 0V. 1st and 2nd  PBLT/PBLB currents are measured with WL off and on, respectively. The (1st–2nd) PBLT/PBLB currents are


calculated. The resulting two currents are then respectively  reduced by 2x of the corresponding BL to WL leakage  currents (see the previous sub-section) separately measured  from the same bit. These result in SNT-to-WL and SNB-toWL leakages.


WL(OFF,ON)


(0.6V)


VDDA(0.6V)


VDDWL(0.6V)


子


(1.6V)


VSSA(0.6V)VNWA(0.6V)


jo


Figure 4:  Schematic illustration of the DBLM bias conditions  for measuring BL to WL leakages.


(0V)


VDDA(0V)


VDDWL(1.2V)


(1.2V)


VSSA(0V)VNWA(0V)


WL(ON)


VSSA(0V,0.6V)


VNWA(0V)


jnrd[


Figure 5:  Schematic illustration of the DBLM bias conditions  for measuring storage node to WL leakages.


Storage Node to Substrate Leakage Test


As shown in Fig. 6, to measure the storage node to substrate  leakages, VDD is held at 1.6V. PBLT/PBLB and other supply  pads are held at 0.6V. 1st and 2nd PBLT/PBLB currents are  measured with VDDWL at 1.6V and 0.6V, respectively. VDD  and VDDWL are changed to 1V while other supply and BL  pads are changed to 0V (not shown). 3rd and 4th PBLT/PBLB  currents are measured with WL on and off, respectively. The [(1st–2nd)–(3rd–4th)] PBLT/PBLB currents are calculated as  the SNT-to-Substrate and SNB-to-Substrate leakages.


BL leakage from periphery circuits and non-selected bits  along the BL path could be significant, especially for  immature and high performance processes. Since each of the


above measured leakages results from the difference between  two leakage values measured from a BL pad (PBLT or  PBLB), the leakages not relating to the bit under test are  cancelled. This improves the measurement accuracy. In  addition, in these measurements VDDBL is biased at a low  voltage level or the same level as the PBLT/PBLB voltage, resulting in lowered BL leakage and hence reduced IR drop. This further improves the measurement accuracy.


Figure 6:  Schematic illustration of the DBLM bias conditions  for measuring storage node to substrate leakages.


Measured Results and Applications


DBLM scheme can find many useful applications. In a first  application, DBLM is used for fast failure analysis by quickly  narrowing down the cause of a bit fail. As an example, an  early failure rate (EFR) single hard fail bit (failing all  voltages) was identified. DBLM was conducted on this fail  bit, along with other 15 good bits on the same word. The left  storage node to substrate leakage of this bit was found to be  outstandingly high at about 0.7uA, as shown in Fig. 7.


6E-7


4E-7


2E-7


Current (A)


01■■□□-I■


■■■


051015


Figure 7:  Left storage node to substrate leakages of an EFR  hard fail bit and 15 good bits measured using DBLM. The  leakage of the fail bit is outstandingly high.


Subsequent nanoprobing on this bit confirmed that there is a  short from the shared drain of the left driver and pass gate  transistors to the substrate, as shown in Figs. 8 and 9.


1


o


点is


Current (uA)


00.2 0.4 0.6 0.81


Figure 8:  Nanoprobed I-V curves of the left driver of the fail  bit in Fig. 7. The data confirm that there is a short between  the drain and the substrate.


Vd (V)


Id


Ib


VDDWL(1.6V,0.6V)


uA)Current (-05


-1


Bit


Figure 9:  Nanoprobed I-V curves of the left pass gate of the  fail bit in Fig. 7. The data confirm that there is a short  between the drain and the substrate.


A final physical failure analysis (PFA) on this bit confirmed  that there is a NiSi pipe on the drain of the left driver  transistor, as shown in Fig. 10.


As another example, a single hard fail bit was identified and  DBLM was applied on the failing word. The left storage node  to VDDA leakage of this fail bit was found to be  outstandingly high at about 4.8uA, as shown in Fig. 11.


A subsequent PFA confirmed that the left storage node stretch  contact is shorting to VDDA metal 1, as shown in Fig. 12.


Figure 10:  PFA of the fail bit in Fig. 7. It confirms that there  is a NiSi pipe on the drain of the left driver transistor.


5E-6 Current (A)1E-62E-63E-64E-6 0-


Figure 11:  Left storage node to VDDA leakages of a hard fail  bit and 15 good bits measured using DBLM. The leakage of  the fail bit is outstandingly high.


Figure 12:  PFA of the fail bit in Fig. 11. It confirms that  there is a short between the left storage node stretch contact  and the VDDA metal 1.


As yet another example, DBLM was performed on a word  containing a single hard fail bit. The right storage node to WL  leakage of the fail bit was found to be outstandingly high at  about 8.5uA, as shown in Fig. 13.


to be outstandingly high at  about 8.5uA, as shown in Fig. 13.


|||I1|■■■■量||
|---|---|---|---|---|

8E-6


Current (A)2E-64E-66E-6


Figure 13:  Right storage node to WL leakages of a hard fail  bit and 15 good bits measured using DBLM. The leakage of  the fail bit is outstandingly high.


A subsequent PFA confirmed that there is a shot between the  right storage node contact and the WL gate poly, as shown in  Fig. 14.


Figure 14:  PFA of the fail bit in Fig. 13. It confirms that the  right storage node contact is shorting to the WL gate poly.


These measured results also validated the DBLM scheme. In a  second application, DBLM is used for variability assessment. As an example, DBLM leakage data from 4K bits in a 1Mb  SRAM instance were collected. Their statistical distributions  are plotted as shown in Fig. 15. Such data can be used to  analyze the defect leakage induced array IDDQ and potential  bit fails, as well as their changes over time.


||.1. .|1m|■■||
|---|---|---|---|---|

250


Count150


07.2E-101.44E-92.16E-9


Figure 15:  Statistical distributions of the storage node to  storage node leakages of 4K bits measured using DBLM.


As another example, the leakages of the 4K bits measured  using DBLM are plotted against rows and columns, as shown  in Fig. 16. Such data can be used to analyze sensitivity of  defect induced leakages on bit locations.


2800


3200


11.5E-9 1E-9 5E-10


2400  1E-9


2800 3200


5E-10


Figure 16:  Spatial distributions of the storage node to  storage node leakages of 4K bits measured using DBLM.


The proposed DBLM scheme enables fast failure analysis and  accurate variability assessment, such as statistical evaluation  and location sensitivity analysis, of defect induced bit


leakages in a functional SRAM. With this scheme, assessment  of defect induced bit leakage change over time (such as during  burn in) also becomes readily available. DBLM has been used  for efficient development of 45nm and 28nm SRAM cells and  processes.


[1] R. Venkatraman, R. Castagnetti, O. Kobozeva, F. L. Duan, et al., “The design, analysis, and development of  highly manufacturable 6-T SRAM bitcells for SoC  applications,” IEEE Trans. Electron Devices, Vol. 52, No. 2, pp. 218-226, February 2005.


[2] L. Liu, Y. Wang, H. Edwards, D. Sekel, and D. Corum, “Combination of SCM/SSRM analysis and Nanoprobing  technique for soft single bit failure analysis,” Proc. Int. Symp. Testing and Failure Analysis, November 2004, pp. 38-41.


[3] V. K. Wong, C. H. Lock, K. H. Siek, P. J. Tan, “Electrical analysis to fault isolate defects in 6T memory  cells,” Proc. Int. Symp. Physical and Failure Analysis of  Integrated Circuits, July 2002, pp. 101-104.


[4] X. Deng, W. K. Loh, P. Beena, T. W. Houston, et al., “Characterization of bit transistors in a functional  SRAM,” Symp. VLSI Circuits Digest of Technical  Papers, June 2008, pp. 44-45.


Row00


3600


Col


24602000000 200 300


元


2E-9八


400T2.5E-9500


Extended Circuit Edit, Analysis and Trimming Capabilities


based on the Backside Focused Ion Beam created Ultra Thin Silicon Platform


Rudolf Schlangen, Rainer Leihkauf, Uwe Kerst, Christian Boit


Department of Semiconductor Devices, Berlin University of Technology  Einsteinufer 19, Sekr. E2, D-10587 Berlin, Germany


Peter Egger


Infineon Technologies AG, Munich, Germany


Ted Lundquist


DCG Systems Inc., Fremont, CA, USA


Highly integrated microelectronic devices drive an ever increasing  effort in engineering, manufacturing and failure analysis. Almost  all established failure analysis techniques and conventional circuit  edit procedures are facing the severe challenges and limits of  aggressive downscaling. While device design and manufacturing  cooperate closely, failure analysis often is considered as an add-on  service upon request. If physical limitations are hard to overcome, extending the application of an established method to promote  synergy with other aspects of IC making is one option for future  progress. Traditionally circuit edit FIB is a post-fix procedure to  allow for fast design changes in the wiring of a chip. Device  performance remains unchanged. A different aspect is the  deposition of FIB probe pads which permits electrical probing in  locations difficult to reach. Probing results in critical regions of a  circuit provide tremendous value for general debug or first silicon  analysis. Device performance can be monitored. This paper adds a  another dimension with new CE and functional chip analysis  techniques where device performance can be directly monitored  and altered; therefore connecting integrated circuit design, device  development and failure analysis for shorter development cycles.


The microelectronics industry has reached a very highly


developed technical level. The cost for improvements and scaling


grow exponentially while physical limits in materials (e.g. need


new insulators) and resolution (implement deep UV lithography)


Stimulation, Probing入《1μm& Near Field Optics


FIB CE directly to FET actives


STI


ebackside EBP


need to be addressed. Of course the same limits apply in Failure


Analysis. However, prohibitive cost and additional constraints do  not allow for simply taking over the solutions developed for  manufacturing. The FA of highly integrated electronics therefore  needs to combine and optimize all existing methods for the  challenges of scaling. It must further extend its value by offering  new opportunities to the device developers and circuit designers. Those opportunities comprise better access to deep submicron  devices, highly resolved test, and direct device performance  control. The direct feedback between test result and device  performance adds a new aspect to FA.


Technically all extended FA options discussed in this paper are  based on backside FIB processing and adding optical and other  probing techniques as needed (Figure 1). The exposed ultra-thin  backside layer allows for backside CE [1], highly resolved  probing and device trimming. The ultra-thin silicon layer has a  depth of approximately 350 nm and is referred to as UTS. Especially for the application of scanning probe microscopy (SPM) related tools like atomic force probing or near-field  microscopy, UTS has to be created in wide areas requiring state of  the art trench floor planarity.


The utilized FIB tool is equipped with a coaxial IR-optical  microscope, allowing in-situ monitoring of the co-planarity  between trench bottom and the silicon/dielectric interface, concurrent with the actual FIB trenching. As illustrated in Figure  2, every interference maxima represents a certain thickness. The  fringes move during the ongoing FIB milling towards the thicker  region. By adjusting the beam pattern the co-planarity between  trench bottom and active device layer is assured [2].


Figure 1: Illustration of the proposed analysis and CE techniques, all based on backside FIB processing


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 21-26


Figure 2: IR-optical images subsequently captured during the FIB  trenching process


The fringes become visible below 40 μm of remaining thickness. The coarse milling is continued until the n-well level at  approximately 2 μm remaining thickness is reached [1]. Subsequently, the remaining bulk is removed in the area of  interest, until the well contrasting shallow trench isolation (STI) appears. Figure 3 shows a readily prepared test structure with a  slope of less than 100nm in the 80 x 45 μm2 wide targeted area (slope « 1%) based on the single fringe pattern. The high planarity


Opti FIB Il


Advantest E1380A EBP system


is mandatory for secure UTS formation in such wide areas. The  UTS serves as a platform for various probing and circuit-edit


inv,8


techniques as described in the next sections. An in-depth  invasiveness study of the FIB thinning procedure can prove its  nondestructive nature. The single transistors suffer a DC


p/nFE


inv.7


performance drop (~10%) whilst the RF performance of modified  gates can be increased by up to 20% [3]. Simulation results are in  good agreement with experimental data; the underlying device


2μm


physics are discussed later in the paper. The main drawback of  UTS for performance analysis is the lengthy procedure itself and  the self heating associated with the reduced substrate volume. Adequate cooling is mandatory.


AMndciniyAn


[45μm


Figure 3: IR-optical image (left) and two FIB images, showing a  test structure thinned to n-well and STI level


Backside Electron Beam Probing


[mV]


signal amplitude


E-beam probing (EBP) has been a well-established, very


successful and smart technique for contact-less measurements of  timing and voltage signals inside an integrated circuit (IC) [4].


These important parameters for circuit design can be extracted  without significant interaction with the circuit. The measurement


0core supply voltage


signal scales down linearly with the operating voltage compared


2.52


to a higher order reduction of signal intensity in competing IR  detection systems. The spatial resolution is also superior to IR  although the e-beam testers have not participated in the  improvement of SEM systems during the past 15 years.


However, due to the low penetration depth of the e-beam signal, the technique has been limited to few metal layer technology  generations, which are not widely used anymore [4]. Near infrared  optical techniques allow for better penetration even through the  backside of a chip but are limited in resolution. Cooling remains a  challenge in a vacuum system whereas IR techniques operate at  atmospheric pressure and allow more options [5].


Os


4s


Applying the proposed backside FIB thinning to any CMOS gate


Δz~630nm


of interest, the body of the device is exposed. As will be discussed  later, the body potential of the thinned device changes with the  operating conditions, which can be detected by backside EBP. A first proof of concept was demonstrated in [6] where EBP  signals were measured on FIB exposed 120 nm single FETs and  ROs. In [7], the functionality was tested on a logic test chip, fabricated in 90 nm bulk CMOS. Figure 4 shows two images of  one test location. The left part is the FIB image captured right  after trenching down to STI level (with CAD layout), whereas the  right image was captured using the e-beam probing system in  imaging mode. Note that an e-beam image features less material  contrast. This is compensated by biasing the part with regular  operating voltage thereby creating a voltage contrast.


Figure 4: SE images of 90 nm DUT, captured in FIB (left) and  EBP (right), with two subsequent inverters


p-FET inv. 7


IR-Optic


80x45μm2


N


5ns / DIV


34μm


0 ps


s F o


DIV


M-U


200mV /


U


nFET inv. 8


Figure 5: EBP measurement results on 90nm node inverter chain, with 50 MHz input signal, 128 averages and 150 ps e-beam pulse  width


1.5t0.5[V]0


Figure 6: EBP signal amplitude vs. core supply voltage, measured  at 180 nm inverter chain


The smallest printing gates of this process technology could be  resolved clearly and all measurements (Figure 5) could be done  without CAD assistance. The results show the expected phase  shift between two stages of an inverter chain. For narrower  transistors (e.g. inv. 7) the signal strength is about 30% reduced  since the pulsed e-beam diameter starts exceeding the transistor  dimensions. Still, the detected signal is strong and timing  resolution is assured. The EPB signal shows a linear dependency  to VDD (Figure 6), allowing this technique to be applied at very


low voltages, where acquisition times of optical techniques like  TRE are already excessively long [8].


Since the necessary FIB thinning alters the device performance, measurement points (MP) shall be selected based on circuit design  instead of exposing a large area down to STI level. Trenching  down to n-well level and subsequently opening small MPs to STI  enables a binary search approach with minor impact through the  analysis itself. Figure 7 illustrates the proposed analysis flow. Once the fail site is localized, a backside circuit edit can be  conducted within the same approach.


Figure 7: FIB image of trench to n-well level with an illustration  of the proposed order of EBP MPs and a typical backside CE (red  cut & green reconnection)


The main advantage of backside EBP compared to the established  optical tools is the clearly higher resolution potential. But also the  optical probing techniques can benefit from backside FIB  processing.


Optical Analysis Techniques on UTS level


The major drawback of optical analysis follow from the linear  dependence between resolution and wavelength. Without UTS the  residual silicon thickness absorbs light below the bandgap energy. That effectively limits the resolution to NIR wavelength  dimensions.


However, reducing the thickness to STI level allows  approximately double the resolution [9] when shorter wavelength  optics are used.


Beyond classical optics resolution limitations, Near Field  Scanning Optical Microscopy overcomes diffraction limited  classical optical systems at the cost of significant signal reduction. Again UTS permits the best performance because of the  minimized attenuation and improved signal to noise ratio.


CE & Nanoprobing on UTS


CE was the starting point for backside thinning. Initially the nwell level was considered as the working platform. That still holds  true if maximum safety against altering the device characteristic is  required. In that case STI and active area is partially exposed  around the desired CE position. The opening is aligned on n-well  level and after STI exposure the most accurate and strongly  visible alignment information to perform any circuit access is  available [1]. STI level aligns perfectly to device layers and lower  interconnect layers due to high resolution lithography.


To ease and accelerate complex CE larger areas of STI might be


exposed at the expense of more impacted devices.


In “traditional” backside CE circuit nodes are connected at metal  levels, e.g. by means of an access hole through STI. With  decreasing dimensions the aspect ratio of that hole can become  very large [10] and filling is a complicated task (see Figure 8). At  the same time any drift of the FIB operation can lead to  unintended shorts as illustrated with the circled dotted line.


Figure 8: Comparison between standard backside CE on metal  lines and the CtS approach


Generally FIB contacts can be deposited on many conductive  materials including silicides. All source/drain regions are covered  with silicide. Therefore a contact to silicide (CtS) is an option for  backside circuit access [11] which features a relaxed aspect ratio  and in addition the opportunity to connect internal nodes which  are not wired through the backend. A typical situation in CMOS  circuitry is the connection between the complementing p- and nFET.


Experimentally an ohmic characteristic of the contact has been  confirmed with a sheet resistance below 60 μm2 [12]. For the  circuit design community this offers to connect to any arbitrary  circuit node, even those which are not routed through the standard  backend. The modification depicted in the right part of Figure 8  would be impossible without CtS.


As an example the second n-FET (“in 2”) connnected in series in  the 3-way NAND of Figure 9 can be bridged directly with little  risk to the gates.


Figure 9: n-FET of a 3-way NAND gate with potential CtS


The low contact resistance in combination with minimum contact  dimensions permits single FETs to be fully contacted. This allows  for nano-probing solutions without the need of backend removal, hence preserving the circuit functionality. In [12], output  characteristics of single 120 nm transistors have successfully been  measured via CtS by using an atomic force prober on the FIB  thinned backside of a CMOS chip.


Invasiveness Evaluation of FIB Thinning


Trenching silicon down to STI level must have some impact on


the device performance. Various experiments in combination with  physical device simulations led to a comprehensive model of the  device performance alteration, being summarized in this  paragraph.


DGSn-well


Figure 10: Process Flow of backside CE


B9


10[uA]


Preparation Step


37μm


-G


n-well


片


心...


--


111111


0.67μm


in


-©


→to STI


local trench


(10MHz)IL□山L


163820out 20人


out 1


remaining Si &


250μm


STI exposure


1.6 VDS[M]exposed [ps]Regular FIB CE Process


Figure 11: Output-Characteristics of a 180 nm n-FET, measured 50 at different stages of the FIB thinning process


start with


milling todevice


FIB bulk removalSTI leveldegradation controlled


The backside procedure begins with decapsulation and


n Well


mechanical thinning, followed by coarse FIB milling down to


↓STI


~2 μm (see line a, in Figure 10). These initial steps are only of 30


~20%exposure


concern regarding reduced heat dissipation. The increased self


heating results in a DC performance drop (also indicated with a, in 20remaining Si [μm]


sTIEepth


Figure 11). Conservative backside edit approaches stop here and 8858492t↓


↓0.71


continue with very small sub-openings which never fully expose


an active region and therefore prevent floating body type effects


[13] by ensuring a reasonably small well resistance.


Following a less conservative strategy the well material is


removed (b) and the transistor body is affected. Further, the ion


beam induced surface damage leads to transistor performance


impact (mobility degradation and charge carrier density


redistribution) which is illustrated by the pink gradient. Finally the


device is gradually changed into an SOI like structure, where the


increase of Rwell initiates floating body effects [13]. With the


180 nm n-FET, the increased Rwell becomes clearly evident in the


form of the kink-effect when the FET is thinned to less than


500 nm (b, in Figure 11).


Moving forward (c) the surface degradation extends to the diode


junction depletion zone and enlarges the diode reverse leakage


current. Ultimately the device rapidly degrades and will be killed


at some point below STI height.


For a backside FIB debug procedure on STI level the question


remains to estimate how much net damage is exerted at the


different trenching levels and if any FIB induced effects may have


some interesting use.


After demonstrating the non-destructive nature of the proposed


FIB thinning on 120 nm technology ring oscillators (RO) [1], a  more quantitative evaluation of the RF performance alteration  used inverter chains (see  Figure 12) in a 180 nm process, characterized in situ with ps resolution [3]. Ten out of 20 inverters


Ga*(30kV)awere exposed simultaneously in order to demonstrate even small


FIB removed田


effects. Figure 13 depicts the measured results. At first the


bulk material


inverter speed steadily dropped during thinning to a remaining Si  thickness (tSI) of ~1.2 μm. Further material reduction increased  device speed with a maximum of +20% just where the STI  became visible (Figure 12 B). The proposed procedure ended


ST


here. Continuing the thinning decreased the performance and


350nm


ultimately destroyed the circuitry at ~150 nm as expected. A


OptiFIB image


Figure 12: A) FIB image, 4 inverter chains on n-well level with


0.49μm


FIB etch box (dotted red), B) enlarged view, 5 inverter stages with


***


-0.36μm


。00.40.81.2


STI partly60


年o


layout, thinned to STI, C) inverter chain schematic


0.360.34


0.230.190.15


Figure 13: Progressing of single inverter delay as a function of  the remaining Si thickness


Apparently the device thinning did not only have a detrimental  impact on the performance. Changes of the device geometry seem  to overcome any FIB induced performance degradation until the  trench undercuts the STI level.


Physical device simulations helped to deeper understand AC  charging effects. The structural differences between an initial  bulk-FET, the partially FIB thinned-FET, and a real SOI FET are  depicted in Figure 14. The body of the bulk FET is properly  grounded. This ground connection is turned very high ohmic for  the FIB-UTS FETs whereas the body of a real SOI FET is not  fixed to any potential at all (floating body). Unlike real SOI  devices, the drain space charge region capacitance (CDB) is still  present in the UTS devices and any potential variation on the  drain enforces a displacement current across the drain bulk  junctions. The simulations confirmed that the increased bulk  resistance Rwell substantially reduces this displacement current. Consequently, the bulk potential becomes a strong function of


time, as shown in Figure 15, and the effective capacitive load  caused by the drain bulk junction is strongly reduced. Additionally, the increased body potential at the beginning of a  switching event (start) lowers Vth, similar to the back-bias effect  in standard MOS, speeding up the switching process. For a full  description see [14].


Figure 14: Comparison between a bulk FET, a FIB thinned FET, once with VD = 0V, once with VD = VDD, and an SOI FET


Figure 15: Simulated bulk potential of an 180 nm n-FET, being  part of a CMOS inverter in dynamic operation


The dynamics of the charging effect can be nicely observed with  e-beam probing on UTS (see Figure 5).


As a net result, the measured DC performance drop is more than  compensated by dynamic charging effects due to a semi floating  body. Stopping at the right moment with the trenching procedure  permits to boost the performance of selected devices and adds a  new aspect to Circuit Edit.


FIB based Delay Reduction


Performance bottlenecks in certain circuit regions lead to soft-fails  and become a predominant limitation. Pre-designed fuses or  varactors may be used to fine-tune the internal timing. This comes  at the expense of overhead and requires a skilled prediction of  likely fails. The FIB induced delay reduction can help in  situations where failures occur at unexpected locations.


Figure 16 depicts a possible situation. A known delay (probed for  example on UTS) has to be compensated for. An appropriate subcircuit to be accelerated needs to be identified by the designer and  the net delay can be reduced, restoring pass condition (green).  Note that this FIB procedure modifies both p-FETs and n-FETs  such that it scales from single gates to whole circuit blocks.


Figure 16: Application example: a slow branch with additional  20 ps delay, either propagating unchanged, resulting in timing  conflict (red) or passing FIB enhanced gates, reducing the delay, restoring pass condition. (green)


Conclusion


Regarding ultra thin silicon as a platform several backside FIB  applications have been presented.


Those include unlimited access to any circuit node for  nanoprobing and connection, contactless probing with electron  beam and enhanced optical techniques. Highly resolving shorter  optical wavelengths can be finally used due to the reduced  absorption in ultra thin silicon.


A novelty is the proposed circuit tuning possibility due to change  in the device structure. The 20% performance boost can be  applied to any transistor, logic gate or full circuit block and opens  a new opportunity for fine-tuning critical signal paths without the  need for pre-designed tuning devices.


References:


[1] C. Boit, U. Kerst, R. Schlangen, A. Kabakow, E. Le Roy, T.


Lundquist, S. Pauthner, ”Impact of Backside Circuit Edit on


Active Device Performance in Bulk Silicon ICs”, Proc. 37th


IEEE ITC (2005) 48.2


[2] J Siebert, L Johri, D McCarty, S Voong, M Sengupta, H.


Wang, "Enhanced Scanning Control of Charged Particle


Beam Systems", US Patent 7,230,240


[3] R. Schlangen, R. Leihkauf, T. Lundquist, P. Egger, U.


Kerst, C. Boit, “Trimming of IC Timing and Delay by


Backside FIB Processing - Comparison of Conventional and


Strained Technologies”, Proc. IEEE IEDM (2008), pp. 439-


442


[4] W.T. Lee, “Engineering a Device for Electron Beam


Probing,” IEEE Design and Test of Computers (June 1989),


pp 36


[5] Rama R. Gorugunthu , Tom Crawford et al, Tahir Cedar,


“Spray Cooling for time Resolved Emission Measurements


of ICs, Proc. 30th ISTFA (2004) pp. 18


[6] R. Schlangen, R. Leihkauf, U. Kerst, C. Boit, ”Functional


Analysis Through Chip Backside with Nano Scale


Resolution”, Proc. 32nd ISTFA (2006) pp. 376


[7] R. Schlangen, R. Leihkauf, U. Kerst, C. Boit, K. Wilsher, T.


Lundquist et al., " Backside E-Beam Probing on Nano Scale


Devices" Proc. IEEE ITC (2007) pp. 23.2 1-9


[8] R. Jain. T. Malik, T. Lundquist, R. Schlangen et al., "Novel


Flip-Chip Probing Methodology Using Electron Beam


Probing" Proc. 14th IEEE IPFA (2007) pp. 39-43


[9] C. Boit, R. schlangen, U. Kerst, T. Lundquist "Physical


Techniques for Chip-Backside IC Debug in


Nanotechnologies" IEEE Design and Test of Computers


(June 2008), pp 250


[10] Q. Wang, M. Thompson, W. Schultz, T. Lundquist,


"Modeling Secondary Electron Emission from High Aspect


Ratio Holes", Proc. 29th ISTFA (2003) pp. 343


[11] R. Schlangen, P. Sadewater, U. Kerst, C. Boit “Contact to


Contacts or Silicide by use of Backside FIB Circuit Edit


allowing to approach every Active Circuit Node”Proc. 17th


ESREF (2006) pp. 1498


[12] R. Schlangen, U. Kerst, C. Boit, S. Schömann, B. Krüger,


T. Lundquist et al., “FIB Backside Circuit Modification on


Device Level Allowing to Access Every Circuit Node with


Minimum Impact on Device Performance by Use of Atomic


Force Probing”, Proc. 33rd ISTFA (2007), pp. 34-40


[13] A. Wei, M. Sherony, S. Antoniadis, "Effect of Floating


Body Charge on SOI MOSFET Design", Transactions on


Electron Devices, Vol. 45, No. 2 -430 (1998)


[14] R. Schlangen, R. Leihkauf, T. Lundquist, P. Egger, U.


Kerst, C. Boit," RF Performance Increase allowing IC


Timing Adjustments by use of Backside FIB Processing",


Proc. 16th IEEE IPFA (2009), pp. 33-36


Subsurface Imaging of Multi-level Integrated Circuits


using Scanning Electron Acoustic Microscopy


L. Meng1, A.G. Street2, J.C.H. Phang1


1Centre for Integrated Circuit Failure Analysis and Reliability (CICFAR),  National University of Singapore


2Qualcomm CDMA Technologies, San Diego, U.S.A


The capability of the Scanning Electron Acoustic Microscopy (SEAM) technique for high resolution non-destructive  subsurface imaging at different depths for a multi-level


dr =、oPC2K


integrated circuit is assessed. Experimental results using a


beveled DRAM IC sample are used to quantify the effect of


the electron beam energy and modulation frequency on


contrast, spatial resolution and depth of focus of SEAM where K is the thermal conductivity of the material, p is the amplitude and phase images.


density of the material, C is the specific heat and w/2t is the


frequency is 53.7 um and 13.4 um respectively. The primary


In integrated circuit (IC) failure analysis, the conventional  method of defect tracing after fault localization [1] is layer-bylayer deprocessing [2]. This technique is destructive and can  induce artifacts, particularly in low-k and ultra low-k  dielectric materials. The ability to image subsurface defects  with high resolution allows characterization that is noninvasive. Subsurface imaging of metal layers can also be  achieved with advanced X-ray tomography techniques [3], but  the technique is time consuming and not readily available.


Scanning Electron Acoustic Microscopy (SEAM) [4] has been  used to generate high resolution images of subsurface features [5,6] in ICs. In this paper, non-destructive high resolution  subsurface imaging of multi-level ICs using the SEAM  technique is described. This technique can be easily  implemented on an existing Scanning Electron Microscope (SEM) as an additional application.


SEAM Theory


SEAM is based on the detection of electron acoustic signals  that are generated within the sample by a periodic intensitymodulated electron beam. The heating effect is due to the  inelastic scattering of the primary electrons, which are  converted to  thermal waves  and which act as an intermediate  mechanism for the acoustic-wave generation [7]. The key  parameter in this model is the thermal diffusion length dT


which determines the region in which thermal waves convert  into acoustic waves and is expressed as [4]:


(1)


where K is the thermal conductivity of the material,  is the  density of the material, C is the specific heat and /2 is the  electron beam modulation frequency. The thermal diffusion  length for silicon and aluminium at 50 KHz modulation  frequency is 53.7 m and 13.4 m respectively. The primary  electron energy dissipation is treated as the source of the  SEAM signals since the thermal waves propagate no more  than a thermal diffusion length when most of the thermal  waves are converted into acoustic signals which propagate  through the sample [4]. The spatial resolution of the SEAM  depends on the thermal wave region, which extends from the  primary electron energy dissipation volume [8]. Hence,  the  SEAM spatial resolution is determined by the thermal  properties and the electron beam modulation frequency for the  linear SEAM mode.


Experimental Setup


Fig. 1 shows the block diagram of the SEAM setup. A  commercial SEM is modified to achieve an intensitymodulated electron beam using a function generator, amplifier  and blanking plates [5]. When the modulated electron beam  irradiates the sample surface, localized heating induces  acoustic waves that propagate through the sample and are  detected by a lead zirconate titanate (PZT) piezoelectric  transducer [9] attached to the back side of the sample as  shown in Fig. 2. The PZT transducer converts the acoustic  waves into electrical signals which are then amplified and fed  into a lock-in amplifier (LIA). The reference of the LIA is the  same signal that is used to drive the blanking plates of the  SEM. The imaging process is controlled by SEMICAPS  2200A Active Imaging System which synchronizes the scan  generator with the output of the LIA.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 27-32


Fig. 2: SEAM signal detection


Results and Discussions


Electron Beam


SEAM Amplitude Imaging of Multi-level IC


The sample is a fully passivated IC with six layers of  metallization and a thickness of 1 mm. Fig. 3 shows the  frontside images of the sample, which has been rotated 40° to  minimize artifacts caused by ac coupling of the pre-amplifier. Fig. 3a shows the secondary electron (SE) image of the die  surface taken at 30 KeV beam energy. This image clearly


Sample


shows the top metal layer and traces of the layer below.  Figs. 3b-3e show SEAM amplitude images taken at the same  location and the same electron beam energy with modulation  frequencies from 25 KHz to 200 KHz. Compared to the SE  image, the SEAM amplitude images clearly show both top  layer and subsurface details and discriminate different depths


PZT Detector


at different frequencies. It should also be noted that the  resolution of the SEAM amplitude images is comparable with  the SE image, which is approximately 1 μm at this


Pre-Amplifier


magnification.  ▼Electron Gun


FunctionV5Blanking


GeneratorAmplifier→ih


Condenser Lens


ScanScan GeneratorAmplifier


Final Lens


PZTDetector


Ref InR


Pre-AmplifierInAmplifierSignalsLock-inSEAM↓￥s


>00Deflection Coils


Beam Blanking Plates


Fig. 1: SEAM experimental setup


50 μm


(a) SE image


(b) SEAM amplitude image at  25 KHz


(c) SEAM amplitude image at  60 KHz


(d) SEAM amplitude image at


173.8 KHz


(e) SEAM amplitude image at  200 KHz


Fig. 3: (a) SE image and SEAM amplitude images of a multilevel IC at electron beam energy of 30 KeV and electron beam  modulation  frequency of (b) 25 KHz; (c) 60 KHz; (d) 173.8  KHz and (e) 200 KHz


In order to verify that the SEAM amplitude images are indeed  showing subsurface layers, the sample was deprocessed to  remove the top metal layer. Fig. 4a shows the SE image of the  deprocessed sample at the same location. Comparing the SE  and SEAM images in Fig. 4a and 4b respectively, it is clear  that the features in the SEAM image are indeed the subsurface  metal lines which are perpendicular to the top surface metal  lines.


(b) SEAM amplitude image at 173.8 KHz


Fig. 4:  (a) SE image with the top metallization layer removed  and (b) SEAM amplitude image at electron beam modulation   frequency of 173.8 KHz


SEAM Amplitude Imaging of Beveled DRAM IC Sample


A beveled IC sample was prepared to quantify the contrast, spatial resolution and depth of focus of the SEAM technique.  The sample is a commercial DRAM IC which is back-thinned  to a thickness of 80 μm. Part of the sample is then ground at  an angle of 1° until the front side of the sample is exposed at  the lowest point of the silicon bevel, as shown in Fig. 5a. Both  SEM and SEAM imaging are performed from the back side of  the beveled sample. The SE image with 10 KeV electron beam  energy in Fig. 5b shows the surface topography of the beveled  sample with the exposed first metal layer. The y-axis is the  interface between the backside silicon and the first metal  layer. The sample thickness increases at the rate of 2 um perlayer. The sample thickness increases at the rate of 2 m per  100 μm along the x-axis.100 m along the x-axis.


(a) Cross-section


Y,Z=0μm


5 μm


(b) SE image at 10 KeV electron beam energy


Z=10 μm


Fig. 5: (a) Cross-section and (b) SE image of the beveled


F£5μm


DRAM IC sample


200 μm


Fig. 6a(i), 6b(i), and 6c(i) show the SEAM amplitude (R) images at 10 KeV electron beam energy and electron beam  modulation frequencies of 25 KHz, 146 KHz and 316 KHz


respectively. Fig. 6a(ii), 6b(ii), and 6c(ii) show the


225 μm


corresponding SEAM amplitude images at 20 KeV electron  beam energy. The 10 KeV SEAM amplitude images show that


Z=10μm


the first metal layer is in focus over a sample thickness range


245μm


of approximately 2 um to 6 um, while the 20 KeV SEAMof approximately 2 m to 6 m, while the 20 KeV SEAM  amplitude images show the first metal layer in focus over a


wider backside thickness range from approximately 2 um towider backside thickness range from approximately 2 m to


12 m. This is expected as the depth of the electron energy


dissipation volume in silicon varies from 6 m for 10 KeV


electron beam energy to 12 m at 20 KeV. It shows that the


electrons penetrate deeper with a bigger interaction volume as


the electron beam energy increases from 10 KeV to 20 KeV


[10]. The depth of focus appears to be relatively independent


of the electron beam modulation frequency over this


frequency range, which differs from the frequency dependent


behavior noted in the previous experiment. This is because the


beveled sample is thinner than the theoretical thermal


diffusion length of silicon, which is 75.9 m and 20.8 m at


electron beam modulation frequencies of 25 KHz and 333


KHz respectively, while the range of thickness of the silicon


bevel is less than 20 m. This is consistent with the


observation that the thermo-elastic magnitude becomes


independent of frequency when the thermal diffusion length is corresponding SEAM phase (θ) images.


z


greater than the sample thickness [11]. There is also no


significant SEAM contrast variation at the electron beam


4000μm


energy of 10 KeV and 20 KeV over the electron beam  modulation frequency range. However, the spatial resolution


si


si80μm+x


is improved gradually as the electron beam modulation


PZT Transducer


frequency increases from 25 KHz to 316 KHz. The  improvement of spatial resolution with electron beam  modulation frequency is consistent with the observations in


Multi-level Integrated Circuits


ref [12].


'Y,Z=0μm


Y Z=0 μm


2= 5 μm


Z=5μm


(a) (i) SEAM amplitude image, 10 KeV, 25 KHz


(a) (ii) SEAM amplitude image, 20 KeV, 25 KHz


Y.Z=0μm


(b) (i) SEAM amplitude image, 10 KeV, 146 KHz


(b) (ii) SEAM amplitude image, 20 KeV, 146 KHz


12 um. This is expected as the depth of the electron energy


(c) (i) SEAM amplitude image,


dissipation volume in silicon varies from 6 um for 10 KeV


10 KeV, 316 KHz


(c) (ii) SEAM amplitude image, 20 KeV, 333 KHz


electron beam energy to 12 um at 20 KeV. It shows that the


Fig. 6: SEAM amplitude images of beveled DRAM IC sample at  various electron beam energies and modulation frequencies


SEAM Amplitude and Phase Imaging of Beveled DRAM  IC Sample


diffusion length of silicon, which is 75.9 um and 20.8 um at


Fig. 7a(i), 7b(i), and 7c(i) show the SEAM amplitude (R) images at 20 KeV electron beam energy and electron beam


bevel is less than 20 um. This is consistent with the


modulation frequencies of 25 KHz, 146 KHz and 333 KHz  respectively and Fig. 7a(ii), 7b(ii), and 7c(ii) show the  corresponding SEAM phase () images.


There is no significant change in the SEAM contrast, spatial  resolution and depth of focus between the SEAM amplitude  and phase images over the range of electron beam modulation  frequencies. However, the SEAM phase images show contrast  inversion as the electron beam modulation frequency increases  beyond 148 KHz, which indicates strong phase shifts of the  acoustic signals generated within the sample. These  observations are also reported in ref [12].


(a) (i) SEAM amplitude image, 25 KHz


(a) (ii) SEAM phase image,  25 KHz


(b) (i) SEAM amplitude image, 146 KHz


(b) (ii) SEAM phase image,  148 KHz


(c) (i) SEAM amplitude image,  333 KHz


(c) (ii) SEAM phase image,


330 KHz


Fig. 7: SEAM amplitude and phase images of beveled DRAM IC  sample at 20 KeV beam energy and various modulation  frequencies


The capability of the SEAM technique for high resolution  non-destructive subsurface imaging at different depths for a  multi-level IC sample has been demonstrated. Experimental  results using a beveled DRAM IC sample are used to quantify  the effect of the electron beam energy and modulation  frequency on the contrast, spatial resolution and depth of  focus of the SEAM amplitude and phase images.


The authors would like to acknowledge the support of the  staff at the Center for Integrated Circuit Failure Analysis and  Reliability (CICFAR) at National University of Singapore  where most of the initial work was performed. The authors  would also like to acknowledge Michael Campbell of  Qualcomm CDMA Technologies for funding and support.


[1] Kudva SM, Clark R, Vallett D, Ross D, Hasegawa T, Gilfeather G, Thayer M, Pabbisetty S, Shreeve R, Ash B, Serpiello J, Huffman K, Wagner L, Kazmi S, "The  SEMATECH Failure Analysis Roadmap", Int Symp  Testing & Failure Analysis (ISTFA 1995), 6-10 Nov 95, Santa Clara, California, USA, pg 1-5, 1995


[2] Wagner LC, "Failure Analysis of Integrated Circuits - Tools and Techniques", Kluwer Academic Publishers, pg  155-156, 1999


[3] Yun W, Wang S, Scott D, Nill KW, "X-ray  Nanotomography (XRMT) Tool for Non-Destructive  High Resolution Imaging of ICs", Int Symp Testing & Failure Analysis (ISTFA 2001), 11-15 Nov 01, Santa  Clara, California, USA, pg 1-8, 2001


[4] Balk LJ, "Scanning Electron Acoustic Microscopy", in  Hawkes PW (ed), "Advances in Electronics and Electron  Physics", Vol 71, pg 1-73, 1988


[5] Wong WK, Thong JTL, Phang JCH, Yin Q, Fang J, “Scanning Electron Acoustic Microscopy: A Novel Tool  for Failure Analysis and Microcharacterization”, Int  Symp Testing & Failure Analysis (ISTFA 2000), 12-16  Nov 2000, Bellevue, Washington, USA, pp 11-16, 2000


[6] Wong WK, Street AG, "Novel Acoustic Techniques for  Microelectronic Failure Analysis and Characterization", Int Symp Physical & Failure Analysis of Integrated  Circuits (IPFA 2005), 27 Jun 05 - 1 Jul 05, Singapore, pg  14-19, 2005


[7] Kultscher N, Balk LJ, "Signal Generation and Contrast  Mechanisms in Scanning Electron Acoustic Microscopy", Scanning Electron Microscopy 1986, Vol 1, pg 33-43, 1986


[8] Cargill GS, "Scanned Image Microscopy" (E.A. Ash, ed.), Academic Press (New York, 1980), pg 319, 1980


[9] Brandis E, Rosencwaig A, "Thermal-wave Microscopy  with Electron Beams", Appl Phys Lett, Vol 37, pg 98-100, 1980


[10]Goldstein JI, Newbury DE, Echlin P, Joy DC, Lyman CE, Lifshin E, Sawyer L, Michael JR, "Scanning Electron  Microscopy and X-Ray Microanalysis" (3rd ed.), Kluwer  Academic/ Plenum Publishers (New York, 2003), pg 68-69, 2003


[11]Domnik M, Balk LJ, “Quantitative Scanning Electron  Acoustic Microscopy of Silicon”, Scanning Microscopy, Vol 7, No 1, pg 37-48, 1993


[12]Balk LJ, Davies DG, Kultscher N, “The Dependence of  Scanning Electron Acoustic Microscopy (SEAM) Imaging on Chopping and Detection Frequency for Metal  Samples”, Physica Status Solidi (a), Vol 82, Issue 1, pg  23-33, 1984


Laser Timing Probe with Frequency Mapping for Locating Signal Maxima


L.S. Koh1, H. Marks2, L.K. Ross1, C.M. Chua1, J.C.H. Phang1,3


1SEMICAPS Pte Ltd, Singapore


2NVIDIA Corporation, Santa Clara, CA, USA


3Centre for Integrated Circuit Failure Analysis and Reliability (CICFAR), National University of Singapore


A Laser Timing Probe (LTP) system which uses a noninvasive 1.3 m continuous wave (CW) laser with frequency  mapping and single point measurement capabilities is  described.  The frequency mapping modes facilitate the  localization of signal maxima for subsequent single point  measurements. Measurements of waveforms with long delays  and 50 ps response time from NMOS and PMOS transistors  are also shown.


The capability of acquiring time resolved waveforms with  GHz bandwidth directly from silicon devices in integrated  circuits is critical for design verification, design debug and the  failure analysis of functional failures. High-frequency  electrical probes [1] have been demonstrated but the probes  are large compared to the internal nodes of the circuit. The EBeam Tester [2] is a non-contact, non-loading technique with  high spatial and temporal resolution but requires access to the  frontside of the chip. However, frontside analysis has become  impractical due to the increasing number of multi-level  metals. In addition, the use of array input-output connection  pads across the die for higher speed devices such as ball grid  array (BGA) and flip-chip packages do not allow frontside  access with full electrical functionality. These constraints have  led to the development of a new suite of backside failure  analysis techniques [3]. Time-Resolved Photon Emission [4] is a passive backside technique capable of GHz bandwidth  which is based on the collection of photons emitted by  switching transistors but suffers from the exponential drop in  emitted photons as supply voltage decreases with each  technology node [5]. Laser Voltage Probing [6] is an active  backside technique which is based on electro-optical effects in  silicon devices [7]. The technique uses a 1.064 m wavelength laser which is invasive due to electron hole pair  generation and a pulsed mode-locked laser which requires  complicated sampling signal processing systems that are not  compatible with the long loop times required by tester-based  applications.


This paper describes a Laser Timing Probe (LTP) system  which uses a non-invasive 1.3 m continuous wave (CW) laser with frequency mapping and single point measurement  capabilities. Experimental results to illustrate the localization  of signal maxima with frequency mapping and single point  measurements of waveforms with long delays are shown. The  ability of the LTP system to measure 50 ps response time from  NMOS and PMOS transistors are also shown.


System Setup


Since all of the work shown here was done as LADA, we refer  to this technique as time resolved LADA (TRLADA).  The  technique should be applicable to SDL keeping in mind that  the SDL technique relies on relatively slow (microsecond to  millisecond) thermal interaction with the sample rather than  the fast (picosecond) electron-hole generation and current  interaction of LADA [7].  Therefore, when using this time  resolution technique with SDL there will be reduced resolution  and accuracy.


Laser Raster


DUT


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 43-51


Figure 2.  Once the location of the interaction region is  known, functional probing is typically performed.   A typical  probe time window for TRE or other systems is on the order of  microseconds.  For test loop periods that are significantly  greater, it is not feasible to search the entire length of the test  for the small time window when the failure actually occurs.


Description of the Technique


The fundamental effect of the TRLADA technique has  probably been observed by many.  It appears as a shifted  LADA image when the failure analyst violates the rule of  dwelling on one pixel per test loop.   We have learned that this  shifted image contains valuable timing information.


As the scan rate is increased for a given test loop length, the  laser only dwells on a given pixel for a fraction of the test.  Effectively this pixel is illuminated by a laser “pulse,” from the  perspective of the test vectors that are executing during the  time the pixel is illuminated. Therefore when scanning at a rate  where the pixel dwell time is less than the length of the test  there is an effective modulation of the laser.  A faster scan rate  creates a shorter effective “pulse” per pixel.


The probability is low of illuminating the interaction region  during the correct interaction time with a fast scan.  In order to  generate a TRLADA image, the fast scanned image must be  summed or averaged for many frames.  This fast scanned  image contains valuable timing information about the failure.


TRLADA Process Flow


1.  Standard LADA analysis and imaging is performed, such  that the pixel dwell time of laser is greater than the test loop  period.


2.  A faster laser scan rate is used to perform the LADA  analysis and a frame averaged “fast” image is generated as  shown in Figure 3.   Note that the laser scan and test loop are  asynchronous.  An asynchronous setup simplifies the timing  analysis into image averaging and requires no effort at  synchronizing the LSM to the tester.


3.  The number of pixels that the LADA signal image shifted  between steps 1 and 2 is measured and used to calculate the  approximate delay between the interaction time and the time of  the pass/fail flag. (see Figure 4).


Figure 3. This diagram illustrates the result of scanning the  laser at a higher scan rate in violation of the standard  technique constraint of 1 pixel per test loop.  Many pixels are  illuminated during the execution of one test loop.  Many frame  images must be accumulated at the higher scan rate since the  test will not fail for every scan.  The shift in the LADA site  corresponds to the delay between the interaction time and the  tester generated pass/fail signal.


Figure 4.  A single line from overlay of the standard and fast  LADA images is shown here.   Each pixel that the spot shifts is  equivalent to the fast scan pixel dwell time.  This pixel shift  can therefore be converted to a time shift which can be used to  calculate the delay between the interaction time and the rising  edge of the pass/fail signal.


Initial Proof of Concept


During functional root cause analysis of a memory circuit  write timing sensitivity, a memory array built-in self test (BIST) exercised a failing memory array.  BIST patterns are  typically hundreds or thousands of microseconds long, with the  indication of a failure occurring at the end of the long test.


As shown in Figure 5, standard LADA analysis identified a  sensitive location on the device.  The TRLADA technique was  applied to find the interaction time.


Next Step: Where in time should the critical region be  probed?


卡


Start of test


Time window of probing  is about 1% of test period


Fail signal output  at end of test


Time


Fast Laser Scan


One test loop


corresponds to many


司 Time windowofprobingFail signal output


pixels


X Shift, in pixels, tells us the time of failure  relative to the fail signal timing that is output  at the end of the test


Slow scan LADA Location


Fast scan LADA  shifted location


Figure 5.  A slow scan LADA overlay identifies the location  of the suspect memory bits, (interaction region).


To find the interaction time, the pixel shift shown in the  TRLADA image in Figure 6 was measured with standard  image processing software.  The X-shift of the spots was 83  pixels.  The fast scan pixel dwell time was 806ns so this Xshift represents a 234.5s delay between the interaction time  and the tester-generated fail flag.


The tester fail flag output occurred at vector 4690 in the test  loop, and the tester loop period was 50ns per vector.  Therefore, the predicted interaction vector was vector 3352.


Figure 6.  A fast scan, at 0.806μs per pixel, shifts the leading  edge of the LADA spots 83 pixels to the right relative to the  slow scan in Figure 5.


Functional probing with TRE was performed and several TRE  time windows were selected near vector 3352.  The actual  interaction vector was found to be at vector 3450 indicating an  error of about 100 vectors (5s).  This initial case verified the


TRLADA method, but also demonstrated that there was room  for improvement.


Theory


A simplified one dimensional line scan of a LADA interaction  region is shown in Figure 7.  The same region is then shown as  it would appear with a faster laser scan.


Figure 7.  This diagram illustrates an averaged ideal line  scan of a LADA site.  The slow scan is taken with a pixel dwell  time greater than the test loop period, so the pixels between  XS1 and XS2 represent the true interaction region.  When the  pixel dwell time is decreased significantly for the fast scan, the  LADA spot shifts to the right and no longer represents the true  interaction region.


shift represents a 234.5us delay between the interaction time


In this analysis, the one-dimensional interaction region is  defined by XS1 and XS2.  The interaction time ranges between  t1 and t2, as illustrated in Figure 8.  The fail flag asserts at time  tF, and the fail flag is active for F vectors.  The fast scan pixel  dwell time is referred to as DF.


Figure 8.  This timing diagram shows an example of an  interaction time window overlaid to the tester pass fail signal.  The times t1 and t2 can be determined relative to tF by using  the Xshift data as described in Equations (1) through (6).


Referring to Figure 7, the pixel XF1 is the result of the laser  interaction at pixel XS1, and the difference in their position  contains the timing information needed to determine t2.  The  time t2 is the shortest time between the interaction time  window and the start of the fail flag.  This relationship is  shown below in Equation (1):


XF1 = XS1 + (tF – t2) / DF                  (1)


At pixel XF2 the amplitude of the fast scan becomes constant.  This point determines the longest time between the interaction  time and the start of the fail flag as shown in Equation (2):


XF2 = XS2 + (tF – t1) / DF                   (2)


error of about 100 vectors (5us). This initial case verified the


X shift  X shift


--XS1


XF1 XF2


XF3 XF4 -1


-


Slow Scan


Fast Scan


XS2


P/F Signal


尚


Vector 0


tF


t2


t1


Interaction time


XF3 and XF4 are simply determined by F, the length of the fail


flag, relative to XF1 and XF2, and don’t contain much added


information as shown in Equations (3) and (4) below:


|XF3 = XF1 + F / DF |(3) |
|---|---|

|XF4 = XF2 + F / DF |(4) |

Re-arranging (1) and (2) show how the line scans can be used


to calculate the times t1 and t2 of the laser interaction time


window.


|t2 = tF –DF (XF1 - XS1) |(5a) |
|---|---|

|t1 = tF –DF (XF2 - XS2) |(5b) |

Subtracting (2) from (1), we see that the distance between XF1


and XF2 is the width of the slow scan spot, stretched by


interaction time window (t2-t1):


XF2-XF1 = (XS2 – XS1) + (t2 – t1) / DF     (6)


The above equations show the simplified relationships


between the slow scan and fast scan image data.   In practice,


(t2-t1), the interaction time window, is typically small relative


to the test vector period.  Therefore, it is generally Equation


(5a) that is used to determine the probe window for TRE


analysis.  However, some of the case studies shown later scaling factor that guarantees 0 <= Q(Dx) <= 1. Only the illustrate longer interaction time windows


Time Resolved LADA Software Tool


As shown in the proof of concept, the interaction time can be  calculated using standard image manipulation software.  However, this method is not easy, and an ad-hoc process to  count the pixel shift could lead to inconsistent results.  We  have developed a software tool that helps the failure analyst  make the best measurement possible.


The tool was developed with a test case device and test pattern  that had a known LADA interaction time.  We exercised the  device with an at-speed scan test, in which a high speed clock  from the internal device PLL was active during the capture  cycle.  A slight shift in a data or clock edge induced by the  laser during the capture cycle causes a failure to be unloaded  at a later time, which is detected on the tester.  The capture  cycle is the known interaction time.  Since the number of test  pattern vectors between the capture cycle and the failing  unload vector is known, the at-speed scan test serves as a good  test of the TRLADA technique.


The software tool has a Reflected Images window and an  Interaction Images window.  The Reflected Images window  contains the reflected laser slow scan and fast scan images.  The Interaction Images window contains the grayscale LADA  slow scan and fast scan images.   Each window will be  described below.


The Reflected Images Window


Any drift or other x-shift in the reflected image between the  slow and the fast scan increases the error in the measured shift  of the LADA spot.  The Reflected Images window, shown in  Figure 9, allows the user to reliably measure this shift so it can  be subtracted out of the LADA spot shift.


Using the crosshairs, which can be locked together, the user  chooses a pixel just to the left of the slow scan LADA spot.  The cursors can be unlocked to choose similar y locations, if  there has been y-drift.  The graph below the images shows the  brightness along the horizontal line selected by the crosshairs.


The graph is used to find an x-shift at which the slow scan line  and fast scan line overlay best.  This operation can be done  manually, or automatically using the Best Shift button.


The Best Shift button searches for an integer pixel x-shift with  the best Match Quality value.  The match quality, Q, at a  particular x-shift Δx, is similar to the method of least squares:particular x-shift x, is similar to the method of least squares:


n-x n-Δx


Q(x) = 1 - M   (Fi – Si+x)Q(Δx)=1 -M∑(Fi-Si+ax)2 / (n-Δx-P+1)2 / (n-x-P+1)                           (7)


i=P


where P is the chosen pixel left of the LADA spot, n is the  number of pixels per line, F and S are the pixel brightness  values in the slow and fast scan respectively, and M is a  scaling factor that guarantees 0 <= Q(x) <= 1.  Only the  pixels to the right of chosen pixel P are considered since only  those pixels are considered when measuring the LADA spot  shift.


The typical x-shift for the Zeiss LSM 310 used for this work is  about 3 pixels, and is dominated by a natural shift between  slow scan rates and fast scan rates.


The Interaction Images Window


The Interaction Images window, shown in Figure 10, enforces  two requirements on the loaded LADA grayscale images.  First, JPEG images cannot be loaded, because the JPEG lossy  compression algorithm can cause a spread of the LADA spot.  The spread in the spot will increase the measurement error of  the shift.


The second enforced requirement is that the images contain the  full dynamic range of the original LADA data acquisition.  Any clipping caused by brightness and contrast enhancement  will change the shape of the LADA spot and increase the  measurement error of the shift.  In general, this requirement  might not be possible to enforce due to the image processing  capabilities of modern LSM software.  However, our custom  Zeiss LSM 310 software automatically saves the original, unmodified image with the full 12-bit dynamic range, and the  tool will only read this image type.


Both the slow scan and fast scan interaction images are  displayed.  The user selects either a horizontal line that


contains both spots with locked crosshairs, or selects a  rectangle that contains both spots.


The graph at the bottom of the window shows a simulated line  scan of the selected area, where the x-axis is x-pixel coordinate  and the y-axis is the brightness on a log scale.  With a  rectangle selection, the brightness value is averaged through  the height of the rectangle.   The line scan for the fast scan is  corrected with the measured shift from the Reflected Images  window prior to being plotted on the graph.


The brightness is shown on a log scale on the graph to  emphasize the leading edge of the line scan.  The user moves  the vertical cursors to leading edge of the line scans to define  XS1 and XF1.  The leading edge is defined as the last pixel from  the left that rises above the background noise. The buttons in  the middle section set the other parameters for equation (5).


The value of tF is set with the Fail Flag button, which sets the  test vector number of the fail flag, and the Vector: ns/MHz  number that sets the test vector period.  The dwell time DF is  set with the pulldown menu that selects the Zeiss LSM 310  scan mode.  The value of t2, the end of the laser interaction  time, is shown to the right and expressed as a test vector  number, with the values for +/- 1 pixel error.  The legend on  the x-coordinate of the graph also gives the user an indication  of the laser dwell time in terms of test vectors.


As shown in the figure, the tool calculates that the interaction  vector should be at vector -2523, if the fail flag goes high at  vector 0.  Although the fail flag was not actually at vector 0 in  the test case, the capture cycle was actually 2522 vectors prior  to the fail flag.  So the results were accurate to within 1 test  vector in this test case.


TRLADA Version 2009-04-30


L口


Reflected ImagesInteraction ImagesLoad/Save


☑Lock


Browse for Reflected Slow Scan Image...


Browse for Reflected Fast Scan Image...


):Profiles'ra0196My DocumentsVSTFA 2009data\GeminiLongTest'Vongtest_t64_attempt3.pngD:Profiles'ra0196My DocumentsVSTFA 2009data\GeminiLongTestdongtest_t2_attempt3.png


?


Shifted 3 Pixels


129


q125


brth


号75


O。2550751001251501752002252502753003253503754004254504755 Pixel X Coordinate


II


>


how


Best Shift96.7% Match Quality (pixel>163


Figure 9.  The Reflected Images window allows the user to measure any x-shift between the slow and fast scan reflected images. Throughout the tool, red represents the slow scan, and blue represents the fast scan.  The pixels along the horizontal yellow line are  shown as a line scan in the graph below.  The red crosshairs on the images move with the mouse and can be locked together, and are  used to select the location of yellow crosshairs.   These images, with the LADA spot overlaid in red, were taken from the test case  device.  The fast scan reflection image is naturally shifted by 3 pixels, due to the LSM itself.


Case Study 1


有STTH21


Column Write Circuit


With the development of the TRLADA software tool, the  technique was applied to an actual failure analysis case.  The  device failed a RAM sequential scan pattern, which contained  multiple ordered scan load and capture cycles prior to a final  unload of the scan cells.  As its name implies, a RAM  sequential scan pattern typically exercises logic paths nearby  and inside of memory arrays.


The multiple scan load and capture cycle pairs required to set  up the device created a 54μs test pattern loop.  Each capture


Failing Bitcell


cycle vector was a potential interaction vector.


Standard LADA analysis was performed, and a memory bit  and the associated column write circuitry were identified as  illustrated in Figure 11.


Figure 11. This standard LADA image was acquired while  looping on the test.  Red sites indicate interaction regions that  increase the failure rate.  Green sites are interaction regions  that increase the passing rate.


美TRLADA Version 2009-04-30


|Reflected Images|Interaction Images|Load/Save||
|---|---|---|---|

Browse for Interaction Slow Scan Image...


Browse for Interaction Fast Scan Image...


D:Profilesva0196My DocumentsISTFA 2009Wata\GeminiLongTestiLONGTEST_T64_ATTEMPT3_INT.SPE


D:Profileslra0196My DocumentsUSTFA 2009dataGeminiLongTestLONGTEST_T2_ATTEMPT3_INT.


Vector:36ns /28MHz


Leading Edge at Pixel 174


3e19106:0


Leading Edge at Pixel 193-/+1 pixel:-2656,-2390


60.000


50.000四40,000 6日


20,000 10,000。


150155160165170175180185190195200205210215220225230235240245 Pixe/ X Coordinale(133 veotors/pixel)


250255


30,000


912X9121=2▲


Fail event at vector-2523


卜


Figure 10.  The Interaction Images window allows the user to choose the LADA spots and measure the pixel shift between the slow  scan and fast scan interaction images.    Either a line, or as shown here, a rectangle can be selected.  The logarithmic pixel brightness  in the selected area is shown in the graph below the images.  The user moves the vertical graph cursors to the leading edge of each  curve to measure the pixel shift and compute the interaction time  Here, we set the fail flag to 0 in the software, so the fail time (interaction time)t is displayed as 2523 vectors prior to the fail flag.  The actual interaction time for this case was 2522 vectors prior  to the fail flag


TRLADA was employed as shown in Figure 12.  The fail flag  was asserted at vector 74787 with a 50ns test vector period.  The method predicted the interaction event occurred at vector


74016.  The closest scan capture cycle occurred at 74009.


SIOMs seu


Figure 12.  This TRLADA interaction graphic shows that the  interaction time was predicted to have occurred at vector


74016.  The LADA signature at the bit cell (top) was chosen  as the interaction region in this case.


A 500ns (10 vector) TRE window was used to collect  waveforms of the suspect circuit at this scan capture cycle  vector 74009.  The TRE waveforms showed that the column  write circuitry was malfunctioning at this time (Figure 13).  Therefore TRLADA predicted the time of the interaction event  to 7 vectors, well within the 96 vectors per pixel dwell time of  the fast scan.


Figure 13.  This graphic shows that the suspect circuit  malfunctioned at vector 74009, only 7 vectors away from the  predicted vector 74016.  The TRE waveforms show that both  WR and WRB, which should be mutually exclusive, assert  pulling down both bit lines.


Case Study 2


The TRLADA methodology was used in another failure  analysis case.  This device also failed a RAM sequential scan  pattern, as described in Case Study 1.   Standard LADA


Interaction Region


analysis was performed, and a fuse read circuit was identified (Figure 14). The fail was observed at vector 19440 and the fail  flag was asserted at 19463 which made a total test length of  970 μs.  This test length greatly exceeded the TRE loop length  requirement.


Figure 14. This LADA image was acquired while looping on  the entire test until the time of failure.  The test loop was  970μs.  This area is the interaction region of interest.


TRLADA was employed as shown in Figure 15.  The method


BL


predicted the interaction vector at 18788.  The test program


DIN "0"D


"0"


was set to jump back to the previous scan load to this vector at


WRB


18451, and the same pass/fail behavior was observed from the  device.  TRLADA therefore helped determine a guess for


BEN"1"NET191


where to start the loop, and the test time was reduced to 51 μs.


The nearest scan sample cycle occurred at vector 18771, which


ola


was off by 17 vectors from the predicted vector.


WR


▽


*2*0**7******


Figure 15. This TRLADA interaction graphic shows the  TRLADA analysis used to determine that the interaction time  occurred at vector 18788.


As shown in Figure 16, the fuse circuit read was not found  initially near vector 81771.  A search with TRE probing in the


NET191


MET191


Lungte a Poat 24Ite te/ lalg thE 3OMCH


XS1


号


XF1


V020 075125122□


80.000


60.000*8.000


20.000


10,000


o012reT0100


100 10 200 200 240


region of that vector located the fuse circuit read at  approximately vector 18779, within 9 vectors of the original  TRLADA prediction. The TRLADA methodology is not exact, but determines accurate starting points for an iterative probe  window search.


Figure 16.  The suspect faulty fuse circuit was enabled and  read as predicted by the TRLADA methodology.  The trigger  is set here at vector 18774, so the read event (READ_B) takes  place at approximately vector 18779 (the delay from the  trigger to the start of these waveforms is 100ns and the vector  period is 50ns).


Complex Interactions


The line scans in Figure 15 show more complexity than the


15.000


17.600 simple ideal scan of Figure 7.  The leading edge used to =10.000 calculate the interaction time in this case study is referred to as


7800


the primary interaction.  The data mixed into the tail to the


2.800


Tho


**


*20*


right of the leading edge contains complex interactions.  These


哈into


may be caused by one or more interaction regions with  different interaction times, or interaction regions with long  interaction times.


In the standard LADA image of this case, a passing interaction  region is to the left of the failing region that was used as the  primary interaction.   In the fast scan image, the tails of both  the passing and failing regions mix to create additional  features seen as slope changes in Figure 17.  Figure 18 shows  two TRLADA plots of the fast scan data which illustrates that  the fail site data (blue line) is riding on top of a more broad  passing site (red line).


In order to investigate this further, TRLADA analysis was  performed only in the passing region.  The passing data is  shown separately in Figure 19 where the data was analyzed  below the failing site so that only passing data is included.  This data indicates that the passing site has an interaction time  window from vector 18788 to vector 19367.


READ_B


FUSE


In summary further analysis of the original TRLADA data in


FUSE_IN


FUSEDET_OUT


Figure 15 indicates that there is a failing interaction time of  18788 and a passing interaction time window from vectors


READ


18788 to vector 19367.


Vdd。


ENABLE_B


Figure 17.  Case Study 2 has two additional complex  interactions in addition to the primary interaction. Note that  the primary interaction analysis (black and blue arrows)  indicates that t1=t2=18788.


 analysis (black and blue arrows)  indicates that t1=t2=18788.


|l=|l=|
|---|---|

100 125100170 20020825027830032838C 370 400 430 480 478800  Figure 18.  Case Study 2 has an interfering passing LADA  signal (red) that superimposes intensity slope changes on the  fail signal (blue) of Figure 17.  In actual fact the fail site  produces a simple interaction, but the passing site has a  longer interaction window.


Figure 19.  Further analysis of the passing signal shows that  the leading edge (solid vertical lines), while difficult to  interpret, indicates that t2 of the passing region is  approximately at vector 19367.  The trailing edge (dashed  vertical lines) was used to determine that the t1 of the passing  region was 18788.


立


|Delay:106ns||Logical READ Waveform|
|---|---|---|

|Timeldiv; 20ns in width.9.7656ps||READ|

|Timeldiv; 20ns in width.9.7656ps||READ_B|

|Timeldiv; 20ns in width.9.7656ps||ENABLE_B|

|lenable t enable||ENABLE|

McUr50ne|2MG1 FalFag8463 5125122


Leading Edge at Pand 246


LskE702+1piket 13385F Fail ewent abvecton t786


35,000 30,000


Intensity slope changes


6,000


0230 240250280270280290310310320 330 340 380 360 370 300390400410420430440450400 471 PlixelX Coordinate (96 vectors/poel)


800102Kf0o


sdsLACA209.t


Case Study 3


As a final example of a long interaction time window, a  voltage sensitive memory single bit failure was analyzed using  a fairly long memory BIST pattern.  The fail flag used for this  case was asserted at vector 181906 and held high for the  following test loop, as illustrated in Figure 20.


The pixels XF1 and XF2 were separated a significant amount on  this example as shown in Figure 19.   Also shown in Figure 21  is an overlay of the pass/fail signal that indicates how XF1 and  XF2 relate to the interaction time window.  In this case the  TRLADA data indicates that the beginning of the interaction  time t1 occurs in the previous test cycle (vector -20578).  The  end of the interaction window occurred at a t2 vector of 59301.  This data indicates that the failure mechanism has a long time  constant with respect to its recovery from a laser pulse.


Figure 20.  Timing diagram for Case Study 3 showing  relation between start of test, fail flag output vector, and the  locations of previous and next test boundaries.


Figure 21. This TRLADA data indicated that a single bit  failure had an interaction time window that extended to the  previous test cycle (calculated as vector -20578 by the  TRLADA software tool).  The overlaid P/F signal is the  pass/fail signal, illustrating the P/F envelope that builds the  averaged fast scan LADA image.  The long interaction time  stretches the rise time of the blue fast scan LADA signal.


The analysis of Case Study 3 was halted due to other priorities  and further TRE verification could not be performed.  However, the case was included here to show a straight  forward example of a long interaction time window that  actually began in the previous test cycle.


An LSM technique has been developed and shared that yields  valuable timing information about LADA (and SDL) laser  interactions in integrated circuits.  This timing information can  be obtained by simply acquiring LADA interaction images at  two different scan rates and then using image shift data to  determine the timing interaction window.  Accuracy and  usability of the technique are improved by the use of a custom  software interface that accounts for reflected image shifts and  handles conversions from pixel shift data to test vector  number.  Several case studies were presented that show that  the tool can be used to routinely determine the correct  placement of triggers for TRE probing.  Also shown in the  case studies were data sets that show that large interaction  windows can be detected and measured.


Fig. 1 shows the optical setup which is an extension of the  version proposed by Heinrich et al [8] without the use of a  reference beam.  A 1.3 m CW laser is used with a laser scan  module in an optical microscope with a refractive solid  immersion lens (RSIL) to achieve a focused scanned laser spot  size of better than 200 nm.  This technique relies on the  minute amplitude modulation (AM) due to refractive index  perturbation caused by electric field variations [7] from the  switching gates that is imparted to the CW laser beam after  reflection from the switching circuitry.  Although the  amplitude modulation is minute, it appears to be linear with  drain voltage [9] and can be detected with standard AM  demodulation techniques.


The use of a 1.3 m wavelength laser is minimally invasive  since it does not generate electron hole pairs that interfere  with device operation.  The 1.3 m wavelength increases the  AM as the free-carrier absorption and refraction is roughly  proportional to wavelength in doped silicon [10].


An analysis of the reflected beam energy in the frequency  domain can quickly identify regions within the circuit that are  operating at a known frequency while an analysis  in the time  domain can reproduce the amplitude waveforms occurring  within the switching circuitry.  In the frequency domain, the  reflected signal can be analyzed with Fast Fourier Transforms (FFT) for mapping the signal amplitude at a specified  frequency or multi-frequency mapping over a specified range  of frequencies. The reflected signal can also be processed  directly with a spectrum analyzer [9]. For single point  measurements in the time domain, the reflected signal is  displayed with a digitizing oscilloscope.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 33-37


Device Under Test


RSILY↑


Frequancy Mapping Image


Incident


umplittude


FFT


Deam


Procassor


Objective


Pholo-Dalector


lube


Timing Wevelorm


Scan Lans


Lans


1.3μmCWLasar


XY Scan曲Mirror


SM Fiber


Cube BSCollinaling lans FdM-W-WN


Digitizing Oscilloscopa


NOUUDNLNU hu


M口


Beam


Fig. 1:  Laser Timing Probe (LTP) system with frequency mapping


Principle of Operation


A conventional scanning optical microscope (SOM) is  modified to accept an additional optical input/output block for  the LTP.  The SOM raster scans the laser beam to produce an  image of the device layer with the field of view (FOV) determined by the objective in use. A 1.3 m wavelength CW  low noise laser is coupled via a single mode optic fiber to the  SOM via the LTP optical block.  The reflected signal from the  device layer is coupled by optical fiber to a photo-detector.


For frequency mapping, the photo-detector voltage output is  connected to a FFT Processor. The FFT Processor output is  mapped as the SOM raster scans the LTP laser beam across  the device.  The FFT Processor may be set either in singlefrequency mode in which the output is proportional to the  signal amplitude at the specified frequency or in multifrequency mode where the output corresponds to selected  frequencies. In single-frequency mode, the signal amplitude is  transformed into pseudo-colors and overlaid onto the reflected  laser image to represent the map of the signal amplitude at the  specified frequency.  In multi-frequency mode, the pseudocolors represent frequencies and the brightness of each color  represents the AM magnitude at the particular frequency.


The beam is then positioned at the point of highest relative  intensity around the transistor for timing measurement.  The  signal strength is sensitive to focus and the maximum signal  strength may not necessarily be at the best image focus [11].  In single-frequency mode, the FFT Processor is set to sweep  over a narrow frequency span centered at the specified


determined by the objective in use. A 1.3 um wavelength CW


frequency and the focus is adjusted to maximize the output  amplitude.  This is  the best position in location and focus for  single point timing measurement.


For single point timing analysis, the photo-detector output is  connected to a high-speed 50 GS/s digitizing oscilloscope.   The output from the oscilloscope undergoes noise reduction  signal processing to produce the timing waveforms. The  system jitter is better than 400 fs with a 10%-90% rise time of  better than 50 ps corresponding to a system bandwidth of at  least 7 GHz.


(a) 20X objective image


(b) 50X objective image


TO


Ngpdgw


Signal (au)g台


-60 50


51


52


53


54


Time (us)


(c) RSIL image


Fig. 2:  Frequency mapping images of graphics device with


(a) 20X, (b) 50X and (c) RSIL objectives


Experimental Results


A series of frequency-mapping images with 20X, 50X and  RSIL objectives obtained from an advanced graphics device  with backside thickness of 100 um is shown in Fig. 2.  Thewith backside thickness of 100 m is shown in Fig. 2.  The  scanned reflected signals are routed to a FFT processor set in  single-frequency mode of 27.5 MHz and resolution bandwidth  of 300 Hz. The frequency mapping images at increasing  magnifications allow the user to converge to the “sweet spot” for single point timing measurements.


Fig. 3 shows the single point timing measurements from the  point localized by the frequency mapping images.  Fig. 3a  shows the signal occurring after a delay of about 15 us. Fig.shows the signal occurring after a delay of about 15 s.  Fig. 3b shows the timing waveform triggered at 50us over a 10 us3b shows the timing waveform triggered at 50s over a 10 s range.  Fig. 4 shows a functional failure from another graphics  device with 4 states from a 3-state inverter.


吕


Signal (au)g


占


4060


80


(a) Triggered at time = 0


(b) (b)Triggered at time = 50 usTriggered at time = 50 s


Fig. 3:  Timing waveforms triggered at


(a) time = 0 and (b) 50 us(a) time = 0 and (b) 50 s


ro


统


以


a r g


s


L


-40


9


Driver1 PMOS


宫


M


PreDriver PMOS


a


Fig. 4: Timing waveform of a 3-state inverter showing 4 states


A frequency map of a 32 nm technology node ring oscillator


Signal (au)


Driver2 PMOS


ρ cn


is shown in Fig. 5.  Using this map, the timing waveforms  from the drivers of the PMOS and NMOS transistors are


w


easily and quickly obtained. The PreDriver PMOS waveform  demonstrates the LTP response of 50ps.


Driver2 NMOS


Driver3 NMOS


Fig. 5:  Reflected - frequency map overlay image of a ring  oscillator  acquired with a refractive SIL


Driver3 PMOS


80160240320400480560600 Time(ps)


Fig. 6:  Timing waveforms from PMOS and


NMOS transistors in the ring oscillator


For these measurements, two critical variables are the spot  size of the laser beam and the accurate placement of the spot.  While “estimating” a gate location is often used for photon  emission (PEM) applications, this estimation method is not  appropriate for timing measurements.  “Uncertainty” in the  placement of the laser combined with optical resolution limits, forces users to place the laser spot blindly near the gate, acquire waveforms, and repeat these tedious steps until the “sweet spot” is located where the signal strength is at a  maxima.  The time to locate the “sweet spot” is often more  than five times the measurement time.  Frequency mapping  virtually eliminates repetitive acquisitions to locate the “sweet  spot”. This process reduces the time required to search for  locations with specific timing signals significantly.


A Laser Timing Probe (LTP) system which uses a noninvasive 1.3 m continuous wave (CW) laser with frequency  mapping and single point measurement capabilities is  described.  The frequency mapping modes facilitate the  localization of signal maxima for subsequent single point  measurements. Measurements of waveforms with long delays  are shown. The ability of the LTP system to measure 50ps  response time from NMOS and PMOS transistors is also  shown.


[1] Ranieri VA, Deutsch A, Kopcsay GV, Arjavalingam G,


"A Novel 24 GHz Bandwidth Coaxial Probe", IEEE Trans


Instrum Meas, Vol 39, Iss 3, pg 504-507, 1990


[2] Thong JTL, "Electron Beam Testing Technology", Plenum


Press, New York, 1993


[3] Bruce MR, Bruce VJ, Prejean S, Huynh J, "Failure


Analysis Turned Upside Down:  A Review of Backside


Analysis Techniques", Electronic Device Failure Analysis,


Vol 5, No 4, pg 13-24, 2003


[4] Tsang JC, Kash JA, Vallett DP, "Time-Resolved Optical


Characterization of Electrical Activity in Integrated


Circuits", Proc IEEE, Vol 88, No 9, pg 1440-1459, 2000


[5] Rusu S, Seidel S, Woods G, Grannes D, Muljono H,


Rowlette J, Petrosky K, "Backside Infrared Probing for


Static Voltage Drop and Dynamic Timing Measurements',


IEEE Int Solid-State Circuits Conf (ISSCC 2001),  5-7 Feb


01, pg 276-277, 2001


[6] Paniccia M, Eiles T, Rao VRM, Yee WM, "Novel Optical


Probing Techniques for Flip Chip Packaged


invasive 1.3 um continuous wave (CW) laser with frequency


Microprocessors", International Test Conference (ITC


1998), 18-22 Oct 98, Washington DC, USA, pg 740-747,


1998


[7] Soref RA, Bennett BR, "Electrooptical Effects in Silicon",


IEEE J Quantum Elec, Vol QE-23, No 1, pg 123-129,


1987


[8] Heinrich HK, Hemenway BR, McGroddy KA, Bloom


DM, "Measurement of Real-Time Digital Signals in a


Silicon Bipolar Junction Transistor using a Noninvasive


Optical Probe", Elec Lett, Vol 22, No 12, pg 650-652,


1986


[9] Kindereit U, Woods G, Tian J, Kerst U, Leihkauf R,  Boit


C, "Quantitative Investigation of Laser Beam Modulation


in Electrically Active Devices as Used in Laser Voltage


Probing", IEEE Trans Dev Matl Rel, Vol 7, No 1, pg 19-


30, 2007


[10]Keldysh LV, "The Effect of a Strong Electric Field on the


Optical Properties of Insulating Crystals", Soviet Physics


JETP, Vol 34, pg 788-790, 1958


[11]Bruce M, Dabney G, McBride S, Mulig J, Bruce V,


Bachand C, Kasapi S,  Block JA, "Waveform Acquisition


from the Backside of Silicon Using


Electro-Optic Probing", Int Symp Testing & Failure


Analysis (ISTFA 1999), 14-18 Nov 99, Santa Clara,


California, USA, pg 19-25, 1999


Pseudo-Soft Defect Localization


Paiboon Tangyunyong, Rick McFarland, Richard S. Flores, Sean Pearson, and Marco O. Sanchez


Sandia National Laboratories, Albuquerque, NM USA  ptangyu@sandia.gov


In this paper, we describe a modified soft defect localization (SDL) technique, PSDL (pseudo-soft defect localization), to  localize pseudo-soft defects in integrated circuits (ICs).   Similar to soft defects, functional failures due to pseudo-soft  defects are sensitive to operating parameters (such as voltages, frequencies and temperatures) and/or laser exposures. Pass/fail  states in pseudo soft defect failures are, however, not fully  reversible after laser exposure or after changing operating  parameters. PSDL uses the methodology of conventional SDL  and/or TIVA in combination with a new scanning scheme for  defect localization.  An example will be shown to demonstrate  the use of this technique to localize pseudo-soft defects


Laser-based techniques such as thermally induced voltage  alteration (TIVA) [1] and soft defect localization (SDL) [2] are common failure analysis tools used to localize hard and  soft defects respectively.  Hard defects such as shorts and  opens are defects that cause failures in ICs at all operating  conditions (voltage, frequency, temperatures). High IDDS  and/or functional failures are the typical failure characteristics  of hard defects.  Soft defects are defects that primarily cause  functional failures when ICs are operated at certain conditions  that may be within or outside the normal operating limit of the  devices.


The pass/fail states of functional failures due to soft defects are  very sensitive to the operating parameters of voltages, frequencies and temperatures and these pass/fail states can be  altered by slightly adjusting these operating parameters.  One  of the examples of a soft defect is a resistive via or contact.  Devices with resistive vias or contacts normally function at  higher operating voltages and temperatures but fail at lower  operating voltages and temperatures [3].  In addition, the  pass/fail states are very sensitive to and can be altered by  exposure to a scanning laser. This sensitivity of pass/fail states  to laser illumination is the basis of  SDL.


During SDL measurements, the device is operated very close  to the pass/fail boundary and the stimulus provided by the  laser either in the form of heating or photo-current effect  changes these pass/fail states (e.g.  from 50/50 pass-fail to  30/70 pass-fail).   These changes are then mapped to form the  SDL images.


Another characteristic of soft defects is that changes in the  pass/fail states caused either by changes in operating  parameters or by laser exposure are fully reversible.   In other  words, the initial pass/fail state is restored when the operating  parameters are reset to the initial values or when the laser  stimulus is removed.  This reversibility in the pass/fail states is  important in SDL data acquisition since SDL images are  normally acquired by scanning a laser over the sample multiple  times for signal averaging.


Similar to soft defects, functional failures due to pseudo-soft  defects are also very sensitive to operating conditions and laser  exposures.  Unlike soft defects, the pass/fail states caused by  pseudo-soft defect failures are not reversible.  Once a  pass/fail states change as a result of laser exposure or changes  in the operating parameters, it will remain in that state and will  not be affected by subsequent laser exposure or subsequent  changes in operating parameters.  Restoring the initial pass/fail  state requires a power reset (turning the power to the device  off and turning it back on).  After the power reset, the device  reverts to its initial pass/fail state when operating with initial  parameters of voltage, frequency and temperature.


Conventional SDL data collection schemes are not effective in  localizing pseudo-soft defects due to the non-reversible  characteristic of the defects (described in the last paragraph).  In this paper, we describe a modified SDL technique, PSDL  that uses the methodology of conventional SDL or TIVA in  combination with a new scanning scheme. An example will be  used in the next three sections to describe and demonstrate the  use of PSDL to localize pseudo-soft defects.


Pseudo-soft Defects in Mixed-Signal ICs


In one of the new mixed-signal IC lots manufactured in  Sandia’s 0.35 μm, partially-depleted SOI technology, an  unusually high occurrence of functional failure was found.  The failure appeared to be randomly distributed across all the  wafers.   The functional failure occurred primarily in an onchip oscillator that failed to assert its output signal (OSCREADY).  The OSC-READY signal signifies that the  oscillator has reached a stable oscillation and the output clock  is ready for use.


Several “failed” and “good” reference devices were packaged  for failure analysis.  It was found the OSC-READY failure  could be duplicated in the failure analysis laboratory using a  relatively small and simple test vector set.   The OSC-READY


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 38-42


failure did not appear to be sensitive to operating voltages or  frequencies, but it responded to a 1340-nm laser illumination  but only at high laser intensity.   If the laser intensity was  below a certain threshold, no laser effect was observed on the  samples.


When a “failed” sample was scanned by a high-intensity 1340-nm laser, it no longer had the OSC-READY failure.  In fact, the “failed” samples behaved like “good” samples after highintensity laser exposure.   The sample would remain in the “passed” state after laser exposure until a power reset was  applied.


After the power reset, the sample would remain in the “failed” state until it was exposed again to the high-intensity laser.  These irreversible changes in the pass/failed states were  repeatable and observed in all “failed” samples.   The laser  exposure, however, did not affect the “good” samples.


The bandgap reference voltage output of the oscillator (output  pin VREFOUT) and the TIVA signals of the “failed” samples  change abruptly (Fig. 1) as a high-intensity laser scans in the x  direction from top to bottom.  The VREFOUT signal sees an  abrupt change from 0 to 1.1 V as the “failed” sample changes  from a “failed” to a “passed” state.   Correspondingly, the  power supply current changes from 1.9 mA to 2.4 mA.  The  large increase in power supply current results in a significant  change in TIVA signals (Fig. 1).


Figure 1: Abrupt change in VREFOUT signals (top) and TIVA  signals (bottom) when a ”failed” sample was exposed to a  high-intensity 1340-nm laser scanning in the x-direction from  top to bottom.


Figure 2 shows the comparison of TIVA images of a “good”


sample and a “failed” sample after high-intensity laser


exposure.  There are no discernible differences between these


two TIVA images, indicating that the “failed” sample behaves


like a “good” sample after high-intensity laser exposure.


Significant differences in TIVA signals were observed in a     “failed” sample when exposed to a low-intensity or a highintensity laser (Fig. 3).   At low laser intensity, the laser has no


effect on the pass/fail state of the “failed” device. After a highintensity exposure, the “failed” sample acts like a “good”


sample. The differences in TIVA images in Fig. 3 clearly


indicate different transistors are active when the device is in a


“failed” state or a “passed” state.


Figure 2: Overlayed TIVA images of a “good” device (top) and a “failed” device (bottom) after a  high-intensity laser  exposure.  The two TIVA images look identical, without any  discernible differences.


Figure 3: Overlayed TIVA image of a “failed” device after a  low-intensity (top) and a high-intensity (bottom) laser  exposure.


Low Laser Intensity exposure IDD = 1.9 mA


“Failed” Device After


High-Intensity Laser Exposure“Good” Device


Low Laser Intensity Exposure IDD = 1.9 mA


High Laser Intensity Exposure IDD = 2.4 mA


Abrupt change in


VREFOUT from 0 V to 1.1 V


“FAILED”


“PASSED”


Abrupt current


change from


1.9 mA to 2.4 mA


Defect Localization


Conventional SDL is not effective in localizing pseudo-soft  defect since it normally requires scanning a laser over the  samples multiple times for data collection. To accurately  localize the pseudo-soft defects, a new scanning scheme was  devised.  The new scanning scheme included:


1) Scan the laser in the x-direction and monitor the outputs  signals from VREFOUT and/or TIVA signals (Fig. 1).


2) Draw a line at the transition boundary between a “failed” state and a “passed” state (Fig. 4).


3) Apply a power reset to the sample.


4) Repeat the scanning in the y direction and draw a line at the  transition boundary  (Fig. 5).


5) Enhance the VREFOUT and/or TIVA images (e.g. changing the brightness/contrast/saturation) so that only the  boundary lines are visible in these images (Fig.  6).


6) Generate a composite image (Fig. 7) by overlaying the  reflected light image and the two images with x-direction and  y-direction boundary lines in Fig. 6.


The point where the two lines intersect in the composite PSDL  images in Fig. 7 indicates the location of a pseudo-soft defect.   Fig. 7 shows the composite PSDL images of two “failed  samples.  The locations of the defects are comparable in these  two “failed” samples.


Figure 4: Red lines were drawn in both VREFOUT  (top) and  TIVA (bottom) images of Fig. 1 to mark the transition  boundary between a “failed” state  and  a “passed” state.


Figure 5: Red lines were drawn in TIVA images of a “failed” sample to mark the boundary between a “failed” state and a “passed” state when a high-intensity laser scanned the sample  from top to bottom in the x-direction (top) and from left to  right in the y-direction (bottom).


Figure 6: Images in Fig. 5 were enhanced (e.g. changing the  brightness/contrast/saturation) so that only boundary lines  were  visible in these images.


Abrupt current  change from


Figure 7: Composite images of two “failed” samples. The  composite image was generated by overlaying the reflected  light image and the two modified boundary-line images in Fig


6.  The intersection of two red lines indicates the location of a  pseudo-soft defect.


The Effects of Laser Power and Scan Rate


The images in Fig. 7 were obtained by scanning the laser at a  rate of 8 seconds/frame over the sample.   Images with  different scan rates of 4 seconds/frame and 16 seconds/frame  were also obtained.  No significant differences in the locations  of the defects were observed with different scan rates.


In contrast, laser power was found to have a significant impact  on the locations of pseudo-soft defects.  Fig. 8 shows two  composite images of a “failed” sample.  The top composite  image in Fig. 8 was generated by carefully adjusting the laser  power so that the laser power was just slightly above the  threshold necessary to cause a change in the pass/fail states.   The bottom composite image was taken with laser power well  above the threshold.


There is a significant difference in the defect locations  identified with two different laser power schemes shown in  Fig. 8.  When the laser power is well above threshold power, it  can cause a change in the pass/fail state before the laser


reaches the “most sensitive” areas of the sample.  As the laser  power increases, the further away the intersection point will be  from the “real defect” location.  Using a laser power slightly  above threshold will ensure the laser only affects the “most  sensitive” areas of the samples


Figure 8: Composite images of a “failed” sample.  The top  image was obtained by using a laser power just slightly above  the threshold power necessary to cause a change in the  pass/fail states.  The bottom image was obtained by using a  laser power far exceeding the threshold power.


Corrective Actions


The area identified by PSDL in Fig. 7 corresponds to the area  of oscillator band-gap circuitry.  Subsequent detailed  simulation of the band-gap circuitry indicated a design  marginality that caused an  instability of the band-gap voltage  reference during the oscillator start-up.  The oscillator was  subsequently redesigned with more robust band-gap circuitry.


Laser Power ~ Threshold Power


Laser Power >> Threshold Power


Summary


We have described a modified SDL technique, PSDL (pseudosoft defect locations) that can be used to localize the pseudosoft defects.  Pseudo-soft defects are sensitive to changes in  operational parameters and/or laser exposure, but changes in  the pass/fail states are not fully reversible.   Pseudo-soft  defects require a power reset to restore the intial pass/fail state.   A new scanning scheme involving scanning the laser in both x  and y directions was used to localize these defects.  It was also  found that the laser powers just slightly above the threshold  power provided the most consistent and accurate localization  of pseudo-soft defects.


Sandia is a multiprogram laboratory operated by Sandia  Corporation, a Lockheed Martin Company for the United  States Department of Energy’s National Nuclear Security  Administration under contract DE-AC04-94AL85000.


[1] E. I Cole, Jr., P. Tangyunyong, D. A. Benson, and D. L.  Barton, “TIVA and SEI Developments for Enhanced  Front and Backside Interconnection Failure Analysis,” Microelectronics Reliabitlity 39 (1999), 991.


[2] M. R. Bruce, V. J. Bruce, D. H. Eppes, J. Wilcox, E. I. Cole, P. Tangyunyong, and C. F. Hawkin, “Soft Defect  Localization (SDL) on ICs,” Proceedings of 28th  International Symposium for Testing and Failure  Analysis, Phoenix, Arizona, November 2002, pp. 21-27.


[3] E. I. Cole, P. Tangyunyong, C. F. Hawkin, M. R. Bruce, V. J. Bruce, R. M. Ring, and W. L. Chong, “ Resistive  Interconnection Localization,” Proceedings of 27th  International Symposium for Testing and Failure  Analysis, Santa Clara, CA, November, 2001, pp. 43-50.


Software Enhanced Time Resolved Laser Assisted Device Alteration with a NonPulsed Laser Source


Kent Erington, John Asquith, Dan Bodoh


Freescale Semiconductor, Austin, Texas, USA


We describe a technique that is used to obtain timing  information from laser assisted device alteration (LADA).  The  technique uses a non-pulsed laser scanning microscope to  obtain timing information with a temporal resolution on the  order of microseconds.  Custom software is used to extract the  timing information from the LADA images.


Laser assisted device alteration (LADA) [1] and soft defect  localization (SDL) [2] both use the laser scanning microscope (LSM) for fault isolation of parametric sensitive functional  failures.  With a failing device that is sensitive to voltage, temperature or frequency, these techniques effectively locate  critical circuit elements in speed paths or suspect elements in  defective devices.   In this paper, we refer to a location  identified by standard LADA or SDL as an interaction region.   Figure 1 illustrates the standard LADA or SDL process.


Figure 1.   In standard LADA or SDL, the interaction image  shows a bright pixel if the test fails when the rastered laser  dwells at that pixel.  Over many averaged frames, regions that  fail more often than typical become bright, as indicated with  the red spot in this figure.  Standard LADA or SDL requires  that the laser dwells at each pixel for the entire test loop.


Once an interaction region is identified, functional waveforms  are acquired with time resolved emission (TRE) [3] or other


techniques to further diagnose the root cause.   The time span  of a probing tool such as TRE is practically limited to about 10  microseconds, so the acquisition trigger must be set such that  the failing circuit event falls within that limited time window.    As shown in Figure 2, a test loop much greater than 10  microseconds complicates the search for the failing event.


In the standard LADA and SDL techniques, the laser dwells at  a pixel for the entire length of the test.  However, it is likely  that the effect of the laser on the pass or fail status of the test  only occurs near the time of the failing event. In this paper, the  interaction time is defined as the time at which the laser  interacts with the sample, relative to the assertion of the tester  generated LADA or SDL pass/fail signal.   If expressed as in  terms of a vector in the tester pattern exercising the device, the  interaction time is called the interaction vector.


Setting the acquisition trigger of the probe tool near the  interaction time will very likely put the failing event into the  10 microsecond time span of the probe tool.


Laser pulsing and modulation schemes have been developed  by others to find the interaction time [4, 5].  However, many  LSM systems use continuous wave (CW) lasers and cannot  benefit from these techniques without modification.


We developed and implemented a technique for locating the  interaction time, with microsecond resolution, on a CW LSM  without modulation.  The technique uses a faster laser scan  rate and measures the resulting pixel shift of the LADA image  signal [6].  We also developed a software tool that reduces the  error in the technique and improves its effectiveness.


Fault injection versus low perturbation


Pulsed laser are also used to illuminate a very short portion of  the test pattern. It could be the rising or falling edge of the DUT  clock. It can also be a short pulse at anytime that can trigger an  electrical transient greater than the transistor threshold voltage. It requires high energy pulses and can be used for fault injection  purpose [18]. It can also simulate Single Event Upset (SEU) in  radiation application [20] as the effects are very similar to atmospheric neutrons or heavy ions in space environment. Fault  injection can also be used for security assessment of smart cards  or to increase device testability. In our case, we are more interested in low power perturbation and subset pattern illumination. Low perturbations are used for XVM techniques, or marginality


study. The aim of these techniques is to localize very small  variation in the operating parameter and we don’t want a high  laser power like for fault injection applications.


For all these raisons, we have chosen a modulated and low perturbation F_DLS approach..


Full Dynamic Laser Stimulation (F-DLS) Implementation


We implemented a modulated laser on our optical platform. The  F-DLS technique needs an optical and an electrical set up able  to control timing modulation in order to cover any kind of test  pattern subset. The aim is to be able to illuminate and perturb  only the vectors of interest.


To modulate the laser beam, we added an electro-optic modulator on the laser path (Figure 8). It is a Pockels cell composed of  a polarization controller consisting in a double LTA (LithiumTAntalate) crystal.


The polarization state transmitted by the biased electro-optic  crystal depends on the applied voltage. If the Pockels cell is  properly biased we have transmission, if not we have extinction. Optical setup control adjustment allows extinction ratio of 5‰. A preliminary setup was done with a fiber coupled modulator. In this case, optical losses were very important (60%) so we  embedded the modulator and the polarizer inside the laser box. The optical power loss is 27% only. It is due to the addition of  the Pockels cell and the polarizer.


Figure 8: F-DLS optical set up. A Pockels cell (electro-optic  modulator) is added on the laser path in order to modulate it. 100% of the laser beam power is transmitted when the Pockels


cell is biased and 0.5 % when it is not biased.


The main purpose of this work has been to demonstrate the ability of F-DLS to identify the right vector. This first setup was  done with an old Pockel cell not necessary well adapted to target ultimate timing performances. The main drawback is the  current frequency limitations: we work with a 10 MHz modulation so we are limited to a 100 ns illumination. Vector or test  pattern subset duration would be longer than this value. The  Pockels cell will soon be upgraded to GHz range Pockels. The  expected high frequency, fast rise time and fast fall time make  sense if the related phenomenon is at least as fast as the modulation. Using thermal laser stimulation will make us work with  vectors at millisecond duration whereas photoelectric is in  nanosecond range [21, 22]. Therefore our worked is focused on  photoelectric Laser Stimulation effects. Thermal Laser Stimula-


Pockels,


LTA crystal


Lens


Multimode


fiber


Laser  1064 nm


Bias voltage 150V


Analyzer aligned with  laser polarization


13


Pass vector


Fail vector


1st test


2nd test


3rd test


4th test


tion involves thermal time constants in the μs range which correspond to a maximum of hundred of KHz for frequency modulation. We have to bear in mind than the time to get a map is at  least the product of pixel time with pattern duration.


In order to perform a full dynamic analysis, the laser position, the laser modulation and the DUT test pattern must be perfectly  synchronized. Their commands are embedded in the test pattern. The tester controls the laser beam modulation and the laser  beam position in addition to the functional test. The laser modulation and the laser scan controls are directly embedded in the  test pattern as “additional vectors to command the laser” (Figure  9). “Device Test Pattern” will be used to run the device functional test. In the additional vectors to command the laser modulation a high level (“1”) is sent to bias the Pockels cell in order  to be in a transmission configuration. A low level (“0”) stands  for laser extinction.


Figure 9: F_DLS functional test pattern. “Device test pattern” is used to run the DUT. The first “additional vector to command  the laser” is the Pockels cell bias command. For a high level


(“1”) the Pockels cell is biased and the laser transmitted. For a  low level (“0”) the laser is not transmitted. The last vector


EleEdtVericalHoriz/Ace2Display CursorsMeasureMathesHeb


command the laser scan: a high level (“1”) makes the laser


TekRunAyerage


1s May0830 31:08


Bultore


beam move to the next location.


Curs1 Pos-11.2ns


In the figure 10 below we describe the general set up of our FCurs2 Pos


DLS method in a Pass-Fail methodology configuration.


272.0ms


The set up is composed of a tester, a laser scanning microscope


□29


(LSM), a modulator block (Pockels cell and Pockels cell ampliZero Fred(02)-H


fier). The tester is running a functional test on the DUT while


period


the laser is scanning its surface in order to locally perturb the


专利


device. The Pockels cell transmits the laser beam on specific  vectors in the test pattern so only vectors of interest are perturbed by the laser stimulation. The tester compares the DUT  output data with the expected output data. If they match, the test  is pass. Otherwise the test is fail. In any case the tester send a


Ch2500my


M 80.0ns 6.2535/hET 160ps/pt


signal to the acquisition card: it could be a high level if the test


Ch41.0Y


A 0h2 / 360mV


was pass and a low level if the test was fail. The functional test  result is correlated with the laser beam localization on the DUT  to provide F-DLS.


Figure 10: F-DLS set up. The tester controls the laser modulation (signal to the Pockels) and the laser scan (signal to the


LSM). The tester also runs the functional test (signal DUT input  and output signal). The functional test result is sent to the acquisition card and correlated with the laser beam localization


on the DUT in order to provide a F-DLS image.


To perform accurate analysis we need to determine the delay  between the tester trigger and the illumination. We used a photodiode and we monitored its output voltage and the tester trigger signal. On figure 11 we noticed that the shift between them  is 283 ns. This delay, as well as the other timing parameter, depends on Pockels, its amplifier and the set up (wires etc.). It  should be easily improved with our next Pockels. Even with this  relatively poor timing, we have been able to validate the interest  of F-DLS.


Figure 11: Timing characterization of the F_DLS set up.


F-DLS Application example


Set up


We work with a simple serial-in/parallel-out shift register perfectly functional. In this application example we use a Pass to  Fail mapping technique. First, we have determined the opera0 1 0 1 0 1 0 1  0 1 0 1


0 0 0 0 1 0 0 0 0 0 0  0


0 0 1  0 0 0


010101010111010


011101010111010


Laser


Scanning   Microscope


Acquisition


card


Pockels


F_DLS


TESTER


1 ￥0  1


0  0  0  1  0  1  0  1  0  0


0  1  0  0  0  0  0  0  0  0


0  1  0  1  0  1  0  1  0  0


0  1  0  0  1  0  0  0  1  0


0  1  0  0  0  1  0  1  0  0


0  0  0  1  0  0  0  1  0  0


0  1  0  1  1  1  0  0  0  0


0  0  0  0  0  1  0  1  0  0


0  1  0  1  0  0  0  1  0  0


Device test pattern


Additional vectors to command the laser


Tester trigger


Photodiode


tional conditions limits. We perform a shmoo plot showing the  functional test results for power supply versus the period (frequency). Based on this information we use the value 3,32V for  the power supply (nominal power supply value is 4,5V) and the  period is 304 ns. According to the shmoo below we are still in  the pass zone. The photoelectric stimulation perturbs the timing  propagation. We are in a low perturbation configuration and a


发


small amount of energy targeting sensitive area is enough to  induce fault.


[1] J Rowlette, T Eiles. “Critical Timing Analysis in  Microprocessors Using Near-IR Laser Assisted Device  Alteration” ITE International Test Conference, 2003, pp. 264-273.


[2] M Bruce, V Bruce, D Eppes, J Wilcox, E Cole, P  Tangyunyong, C Hawkins. “Soft Defect Localization (SDL) on ICs” Proc.28th International Symposium for  Testing &Failure Analysis, 2002, pp. 21-27.


[3]  D Bodoh, N Pakdaman, J Vickers, et al.  ”Defect Isolation  Using Time Resolved Photoemission on SOI Devices that  Fail Scan Tests” Proc.28th International Symposium for  Testing &Failure Analysis, 2002.


[4] J Shaw, C McMahon, Y Ng, F Beaudoin. “Dual Port RAM  MBIST Analysis using Time Resolved Dynamic Laser  Stimulation” ISTFA 2008: Proceedings from the 34th  International Symposium for Testing and Failure  Analysis, 2008, pp. 188-192


[5] P Perdu, R Desplats, F Beaudoin , P Vedagarbha, M  Leibowitz, KR Wilsher. “Spatial and Temporal Selective  Laser Assisted Fault Localization” US Patent #6,967,491, Nov-22-2005.


[6] Erington, Kent and Asquith, John.  “Time Resolved Laser  Assisted Device Alteration”.  Freescale Patent Filing  Docket number NC10101TH


[7] F.J. De la Hidalga, M. Jamal Deen, E.A. Gutierrez.  “Theoretical and Experimental Characterization of SelfHeating in Silicon Integrated Devices Operating at Low  Temperatures” IEEE Transactions on Electron Devices, Vol. 47, No. 5, May 2000.


XF2


From Static to Full Dynamic Laser Stimulation


A. Deyine, K. Sanchez, P. Perdu, F. Battistella


THALES & CNES  Laboratory, 18 Avenue Edouard Belin, 31401 Toulouse Cedex 9, FRANCE  phone: 33 5 61 28 14 32; fax: 33 5 61 27 47 32; e-mail: amjad.deyinebarth@thales-is.cnes.fr


H. Deslandes


DCGSystem, Fremont (CA), USA


D. Lewis


IMS Laboratory. Talence, FRANCE


Purpose


Limitations of backside optical techniques for failure analysis of  dynamically activated devices have underlined the need to extend the capabilities of Dynamic Laser Stimulation techniques (DLS). DLS techniques provide a precise localization of the  dynamically failing area, but it lacks timing information as the  fault is often related to a specific test vector. Optical probing  techniques such as TRE and LVP [1, 2] are hardly applicable on  cases with long test loop and for which no preliminary information is available on the time window of interest. Defect localization and electrical tests can be coupled in order to provide more  accurate information about the failure, especially vector information in addition to x and y localization.  We have developed a  Full Dynamic Laser Stimulation (F-DLS) approach based on  laser modulation by electro optic modulator to face this challenge. The purpose of this paper is to present DLS limitations, our motivations, comparisons with other DLS extensions, FDLS implementation on our system, application example and  future F-DLS developments.


Since integration in electronic component increases, integrated  circuit failure analysis becomes more and more complex and  failure analysis techniques have to continuously evolve to tackle  new challenges.


Optical techniques are currently used in failure analysis in addition to electrical tests in order to localize defects in a device. They are mandatory to perform backside analysis through silicon substrate. Unfortunately, Static and Dynamic Laser Stimulation techniques are no longer sufficiently accurate when fault  propagation in long test pattern shows several potential failure  sites.


After a brief reminder of Static and Dynamic Laser Stimulation  techniques currently used, we will discuss challenges associated  with long test pattern. To face complex VLSI devices analysis, we will show how adding temporal information in the dynamic  analysis of integrated circuit strongly extend DLS applications. Then we will present an implementation of this new Full Dynamic Laser Stimulation technique on a commercial system. Finally, preliminary result and further improvements that are  currently under development will be presented.


Laser Stimulation techniques background


Static Laser Stimulation (SLS)


The number of metal level in integrated circuit increases but  Laser Stimulation techniques are able to overcome this issue  since they are applicable from the device backside. Near Infrared Radiations (NIR) are used in order to go through the silicon  substrate using silicon transparency for NIR wavelengths. NIR  laser stimulation has physical effects on the integrated circuit  that are used to locally stimulate the device and localize defective sites.


Two infrared wavelengths are commonly used. 1064 nm wavelength laser induces local photoelectric stimulation by creating  electron-hole pairs, and so electrical current in the device.  The  associated techniques are OBIC (Optical Beam Induced Current) [3, 4] and LIVA (Light Induced Voltage Alteration). It  images junctions and other defects such as shorts, leakages or  any kind of expected or abnormal behavior enhanced by OBIC. 1340 nm wavelength laser beam carry photons that are not energetic enough to create electron-hole pairs. In this case, photons absorption locally heats the target. Related Thermal Static  Laser Stimulation techniques (TLS, [5, 6, 7]) are OBIRCh (Optical Beam Induced Resistance Change), TIVA (Thermally Induced Voltage Alteration) and SEI (Seebeck Effect Imaging).


These Static Laser Stimulation techniques (SLS) are very efficient to detect defects related to leakages. Nevertheless, failure  analysts have to deal with soft defects too [8]. Soft defects cause  abnormal behavior within a part of the device specification  range, and they occur when the IC is operated under defined  operating and environmental conditions (temperature, power  supply voltage, frequency, timing …). In addition to soft defects  at device test level, some soft defects appear only when the device is embedded in an application and they are very hardly  reproduced in laboratory for analysis. The same kind of issue  appear when environmental sub threshold stress address component robustness. Margin analysis performed by Dynamic Laser Stimulation (DLS) techniques [9, 10, 11, 12, 13] provide  solution to these issues.


Dynamic Laser Stimulation (DLS)


Soft defects are related to operating conditions, aging, environment or a combination of the three. To localize the sensitive  structures involved in these kinds of defects, we need to determine the conditions to reproduce them. The device structure


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 52-59


affected by a soft defect type of failure can be localized using  DLS techniques.


For DLS we need to have the device activated while the laser  beam is sweeping its surface. A pre-analysis should be carefully  done to extract electrical information about the failure and to  build the set up. Depending on the defect signature and the information we have from previous electrical and environmental


Laser stimulation


(temperature) characterization we can choose Thermal or PhoInput sequence


100010101010 011UU


0011110101


7C.I.


30000011010Expected output vectors toelectric Laser Stimulation. The localization set up will be built 00100101in accordance with this information but also taking in account 1100100110


00101110-


the environmental conditions. For instance, the temperature 1010100|1-U10


01010100


could play a key role in the device behavior. We also need to I0101110-↑0


01010101


determine which parameter sensitizes the most the soft defect.  个 Period (T)


FAIL


As an example, we test a device for different frequency and


PASS


Vector


power supply combination. Previous electrical observations lead  us to work on these operating parameters. We also know thanks


000011010


to a previous temperature test that temperature is a key parameSH1110101


ter in the device abnormal behavior. Functional test run for two


-0。201010 1、0711101


different temperatures are presented on a shmoo (Figure 1). In1010101001


crease temperature induces a shift of the limit between PASS  and FAIL. We know then that thermal laser stimulation could  provide local heating which may trigger an abnormal behavior  for sensitive areas. We then have the key tools to perform DLS  analysis on our device.


Figure 1: Shmoo representing the component frequency versus  the power supply. The fail area spread when the temperature  increases.


There are two main families in the Dynamic Laser Stimulation  techniques: the functional (Pass-Fail) mapping and the parametric mapping.


The Functional Mapping technique is a binary technique. We  use a tester which runs the device under defined conditions determined by previous characterizations (cf example above). In  the mean time a laser beam is sweeping the Device Under Test (DUT) surface inducing photoelectric or thermal perturbations. The tester sends vectors to the device which sends back output  data. These output data are compared with the expected output  vectors by the tester in order to determine if the device is functional or not. If expected output data and output data coming  from the DUT match, a pass signal is sent to the acquisition  card. Over while the card receives a fail signal (Figure 2). Pass  or fail signal are correlated with the laser beam position on the  DUT surface to provide a binary image highlighting the device  sensitive structures to external perturbations (laser stimulation). Then we obtain a Pass-Fail image (Figure 3).


A loop test is done for each laser beam position. This operation  is repeated until all the device surface is swept by the laser  beam. If we keep the example given on figure 1 the tester will  run the pattern at 8.3V and 0.6 MHz in the limit pass zone and  the thermal laser will locally increase the temperature. Sensitive  areas will become fail and highlighted on the Pass-Fail image.


Output signals


Figure 2:Pass-Fail Mapping electrical set up. The laser stimulation may induce errors in output signals if the structures  swept by the laser are sensitive. The tester compares expected


output vectors and actual output vectors coming from the DUT.


[MHz]1


0.9


在


人


0.7一


天之


之人人


0.6-


0.5


[MHz]


0.4


e


0.3?


0.3


0.1+。-


0.1↓


Figure 3: Example of a Pass-Fail binary image. White areas


8.18.28.38.48.588.18.28.38.48.5(Vbast [V]


show structures which become fail under photoelectric stimulation.


This functional mapping [11] is named SDL (Soft Defect Localization) [8] when a thermal effect is used or LADA (Laser Assisted Device Alteration) [10] when a photoelectric interaction  is used.


This functional (Pass-Fail) imaging technique is the simplest of  the dynamic imaging techniques and is still commonly used. It  only gives binary information. Even if it provides low complexity images, the threshold principle behind any binary technique  jeopardizes information.


In order to have more accurate information about the failure  mode and the integrated circuit robustness, parametric DLS tests  are being developed. Instead of a pass to fail or a fail to pass  information, variations induced by the laser stimulation are  mapped. Parameter variation can be data transfer timings, frequency, voltage etc. Parametric techniques could detect weak  variations in operating parameters. These techniques are known  as X Variation Mapping techniques [13], X standing for any  analog parameter (frequency, timing, voltage etc.). The variations between a reference signal and the signal coming from the  device under test are monitored while the tester is running the  device and the laser beam sweeping the DUT surface. The


Temperature increases


monitored operating parameter, the test pattern and localization  conditions are determined by previous characterization. The  laser beam position is correlated with the variation measured in  the device operating parameter which forms the XVM image.  As an example we show that thermal laser stimulation can highlight variations in signal propagation delay  (Figure 4). It is an  inverter chain made of 3 groups of inverters. The 256 grey levels in the XVM image represent variations in the delay propagation induced by the thermal laser stimulation. Figure 4 shows  that variation in the propagation delay trough this inverter chain  is different for the three groups of inverter.


Figure 4: Example of Delay Variation Mapping (DVM). Time  delay propagation under Thermal Laser Stimulation along an


inverter chain with 3 different groups of inverters. Propagation  delay decreases from left to right.


XVM is a very sensitive technique for identifying abnormal  variation in operating parameters. XVM techniques are very  useful for analog and mixed mode device [14]. With XVM techniques, we highlight variations in operational parameters so we  can localize both very sensitive areas and less sensitive areas. It  is important to be able to see the less sensitive areas too because  the most visible highlighted areas are not necessarily the failing  structures. On the image below, the thermal effect of a 1340 nm  laser is used to induce shift in the output signal phase. Grayscale  level is proportional to the difference between the signal output  value under thermal laser stimulation and a reference signal.


Figure 5: Frequency Variation Mapping performed on an analogue device [15].


XVM techniques is the most powerful and sensitive technique  among all DLS techniques. Their sensitiveness are used in failure analysis but it was demonstrated that these techniques could  also be efficiently embedded in qualification process to highlight marginalities due to aging [16, 17]. They also need low  perturbation levels compared to pass-fail techniques, up to one  order of magnitude.


DLS limitations


DLS techniques have already reached their limits. Indeed any  sensitive vectors in the test pattern under laser stimulation appear on the DLS image but we are not able to distinguish which  ones are related to the defect. Even with a simple counter we  have a “Christmas tree” (Figure 6). It is obviously worst with  long test pattern.


Figure 6: Classic DLS: Pass-Fail operated on a shift register.


To identify the effect of DLS on specific subset of vectors, we  need to be able to discriminate vectors in the test pattern. We  propose the Full Dynamic Laser Stimulation technique (F-DLS) to address this issue. By using a modulated laser instead of a  continuous one we are able to illuminate specific vectors or test  pattern subset. F-DLS provides temporal information in addition  to defect localization.


Fundamental choices for Full Dynamic Laser  Stimulation


Pulsed laser versus modulated laser


Previous works have been done on pulsed laser and fault injection. Our choice, low perturbation and laser modulation differ  from most previous literature. In fact, this choice is related to  key questions about full dynamic techniques. After a brief description of pulsed and modulated solutions, we will underline  some advantages of the modulation one.


Pulsed laser short description


In this mode the NIR laser is pulsed from 100 femtosecond  range to 10 ns second range. In the most recent publication [18] the DUT is driven by a tester. The laser pulse is triggered by an  Automatic Test Equipment (ATE) and it is synchronized with  the DUT clock. Pulse energy (picoseconds range) or Laser  power (nanosecond range) are challenging key factors. Repetition rate (usually less than 80 MHz) and pulse picker intrinsically reduce the sampling rate.


Modulated laser short description


The set up is almost the same as with a pulsed laser. The tester  drives the DUT and triggers the laser modulation. The laser  beam location is correlated to the DUT electrical pass-fail information and an imaging system integrates this value pixel per  pixel and converts it into a grayscale image. Instead of using a  short duration pulse, we will have the choice of different timing  parameters for the laser. Synchronously with the test pattern, we  can choose when the laser starts to illuminate the device, how  long it does it and when we stop it. Existing versatile laser


modulation system allows to choose from continuous (cw) to ns  range. The laser trigger and the modulation command are directly embedded into the DUT test pattern as we will explain in  the “Full Dynamic Laser Stimulation implementation” paragraph. Previous work was published about the implementation  of an electro-optic modulator to modulate the laser beam in order to discriminate read and write failure [19].


How to find the first failed vector?


Laser modulation as opposed to laser pulsing has been primarily  chosen to answer this question. With a pulsed laser we need to  test vector per vector, edge by edge from the test pattern beginning to the last vector in the worst case. Considering this, if we  have a 1024 vector test pattern then 1024 images are required  with the pulsed method to isolate temporally the fault. Whereas  using a modulated laser associated with a dichotomy methodology 10 images will be sufficent.


The example given in figure 7 is a 16 vector test pattern example. We first performed a simple DLS analysis with a continuous wave laser in order to determine the failing area of interest. We then modulate the laser in order to illuminate only from the  first vector to the 8th. If the test is pass then we know that the  first fail vector is between the 9th and the 16th so we can eliminate half of the pattern in one DLS acquisition. We illuminate  then from the 9th to the 12th. If we still have no failed vector we  illuminate the 13th and the 14th etc. In the worst case we have to  do 4 images to identify the failing vector of interest. More generally we need a maximum of N images for a 2N vectors test  pattern. Modulation easily allows this dichotomy approach since  device laser illumination can be adjusted for any number of vectors.


Figure 7: Example of the use of modulated laser associated with  a dichotomy methodology to find the first failed vector in a test  pattern.


periode


Figure 12:  Shmoo plot showing the shift register power supply  versus period.


A tester runs the shift register with this limit condition while the


TelkStopped


205225 Aces Tek Stopped


207684AC


photoelectric laser is synchronously sweeping the device under  test (cf “laser stimulation techniques background”). We present  the chronogram on figure 13 for 4 outputs on the eight.


Figure 13: Chronogram representing the shift register input, the  4 outputs (on 8), and the shift clock for 14 vectors.


We run the IC with a minimum period parameter. All the shift  register cells are sensitive. As soon as a signal goes through a  cell, a critical timing issue will be triggered by laser interaction. By illuminating all the sequence we perturb each vector in the  same way and highlight every possible fault propagation path (figure 14). So far, usual DLS approach did not allow us to discriminate the fault propagation path for each vector.


5. . .


4.6 42


Figure 14: Shift register laser sensitive areas obtained with a


3.8-


continuous laser scheme.


ID


Now we select the vector we want to illuminate. We will show


to


W3


that we are able to discriminate the fault propagation path for


e r2.0


each vector using the F-DLS technique.


F-DLS results


2.2


The shift register functional test is run by the tester while a pho1.8


toelectric laser beam is scanning its surface. The chronogram on  figure 15 represents the different monitored tester signals. The  top one is the pass-fail signal resulting from the functional test


11'*T111


and sent to the acquisition card. The middle signal represents


10n59n108n157n 206n255n 304n353n 402n451n 500n


the test pattern duration and the bottom signal is the command  to the Pockels cell. The high level is for laser beam transmission. Pulse width is 200 ns. The chronogram shows when the  laser stimulation occurs in the test pattern.


Figure 15:  Tester signals: pass fail signal (Top); test pattern  duration (middle); modulation command (bottom).Laser illumination occurs at the beginning of the pattern (left) and at the  end (right).


一--


一


--11I--------


I-The photoelectric laser is used to illuminate 6 specific vectors: N° 1, N° 4, N° 8, N° 10, N° 11, and N ° 14. When we illuminate  a vector we know that we induce a perturbation because of the  test operating conditions that we previously determined (pass to  fail limit). Figure 16 illustrates that we are able to identify  which sensitive flip-flops structures is perturbed at a given vector in the test pattern.


We highlight then the corresponding fault propagation path  among all possible paths we previously obtained on figure 14  with a continuous wave laser.


Pass_Fail signal


Modulation


E


Test pattern


一---


Vector 1      2      3     4       5     6     7     8      9     10   11    12   13   14


Clk


In


Out 1


Out 2  Out 3


Out 4


Figure 16:  Pass-Fail images for different illuminated vectors: N° 1, N° 4, N° 8, N° 10, N° 11, and N ° 14. Photoelectric laser  sensitive areas change with the stimulated vector.


There is not a permanent sensitive area on all 6 images. We can  conclude that we are perturbing vector propagation paths but not  the clock.


Based on the timing characterization we know that we actually  illuminate vector 2 and slightly vector 1 when we trigger the  illumination on vector 1 (figure 17). Therefore we illuminate the  transition between vector 1 and vector 2. As we are monitoring  timing issue, it is a very important condition to be sure we alternate them. It happens only during state change.


Figure 17:  Laser illuminates the vector N+1 if the illumination  trigger is set to “1” on vector N.


For a complex device with a test pattern performing different  function we are now able to correlate which part of the device is  activated by a specific set of vectors. This method helps following the fault propagation in the device and provides internal  fault vector information before fault propagation to the output. It allows x, y and vector localization for failure analysis purpose  but also a predefined timing window for subsequent optical  probing operations.


Discussion


The main benefit provided by synchronizing the laser beam  modulation with the functional test is that we can discriminate  faults propagation path. Classic DLS techniques using continuous wave laser can give several localizations which are not always linked to the electrically active defect. They increase the  analysis complexity so complementary tests are required to confirm which of those signal is defect related. F-DLS technique  target vectors or group of vectors responsible for the degraded  functionality.


Moreover, by embedding laser control commands in the test  pattern allows having a unique set up for all the dynamic and  static operating parameters characterization under laser stimulation. In the shift register example we work with a functional test  and use a Pass-Fail technique, but we can extend the F-DLS to  any X variation mapping techniques for parametric analysis.


The next limitation that we have to overcome is to improve the  modulation block response time. The Pockels we are using now  has 12 ns rising time and work at 10 MHz only. Some improvements will be made on our actual system in order to increase timing performances.


We also plan to post process data to simplify result interpretation. For instance we would like to have one F-DLS image  where the different illuminated vectors are referenced to their  corresponding localization as schematically illustrated in figure


18.


Figure 18:  Full Dynamic Laser Stimulation image. Different  illuminated vector and their corresponding sensitive structures  are represented.


Optical technique evolution is mandatory to maintain our ability  to perform efficient failure analysis. From Static Laser Stimulation to Dynamic Laser Stimulation technique, we gain the ability to deal with soft defects. Moreover DLS techniques such as  XVM techniques are very sensitive so the analysis accuracy was


Vector 11


Vector 1


Vector 4


Vector 8


Vector 14


Vector 10


Shift clock


Laser Command


304 ns


Laser ON


Vector N


Vector N+1


283 ns


considerably improved. But DLS techniques also reached their  limits when fault propagation in long test pattern demonstrates a  lot of potential failure sites and we cannot distinguish between  several possible defect locations.


In this paper we demonstrated that the Full Dynamic Laser  Stimulation technique can correlate laser stimulation sensitive  area locations and pattern vectors if the functional test and the  laser modulation are synchronized. Only one test is needed to  discriminate defective sites where several tests would be required with classic DLS techniques. Propagation fault in long  test pattern problems are overcame thanks to the addition of  modulation in Dynamic Laser Stimulation techniques.


Acknowledgements


The authors would like to thank F. Bourcier, F. Bereil, P. Le  Nouy (CNES) for their technical assistance.


[1]    R. Desplats et al. “Time Resolved Photon Emission Processing Flow For IC Analysis” Microelectronics reliability  vol 44, pp 1715-1720, 2004.


[2]   U. Kindereit, " Investigation of Laser Voltage Probing Signals in CMOS Transistor”, IRPS 2007.


[3]   Wilson and E. M. MacCabe, " Theory of optical beam induced current images of defects in  Semiconductors ", J. Appl. Phys. 61(1), 1987.


[4] K. Nikawa and S. Tozaki, “Novel OBIC observation  method for detecting defects in Al stripes under current  stressing”, ISTFA 1993, p303-309.


[5] K. Nikawa et al, “New Laser Beam Heating Methods Applicable to Fault Localization and Defect Detection in  VLSI Devices”, IRPS 1996, p346-354.


[6] F. Beaudoin et al, “Principles of thermal laser stimulation  techniques”, Microelectronic Failure Analysis Desk Reference, 2004, p417-425.


[7] K. Nikawa et al., “New capabilities of OBIRCh Method  for Fault Localization and Defect detection.” ATS 1997.


[8]    M. Bruce et al., “Soft Defect Localization (SDL) on ICs.” ISTFA 2002, p21-27.


[9]  F. Beaudoin et al., “Laser stimulation applied to dynamic  IC diagnostics.” ISTFA 2003, p371-377.


[10] Rowlette, J & T Eiles,  "Critical Timing Analysis in Microprocessors Using Near-IR Laser Assisted Device Alteration ITC 2003, p 264-273,


[11] K. Sanchez et al.,” Dynamic Thermal Laser Stimulation  Theory and Applications”, IRPS 2006.


[12] J. Colvin, “Functional Failure analysis by induced stimulus”, ISTFA 2002.


[13] K. Sanchez et al., “Delay variation mapping induced by  dynamic laser stimulation”. IRPS 2005


[14] S. Sienkiewizc et al. “Failure Analysis Enhancement by  Evaluating the Thermal Laser Stimulation Impact on Analog ICs” IPFA 2008.


[15] M. Sienkiewicz et al. «Failure Localization & Design Debug on Mixed-Mode ICs by using the Dynamic Laser  Stimulation Techniques », ISTFA 2007.


[16] A. Deyine et al, “Dynamic Laser Stimulation technique for  device qualification process”, ISTFA 2008.


[17] A. Deyine et al, “Improved IC qualification using a Dynamic Laser Stimulation technique on an EEPROM”, IRPS 2009.


[18] T. Kiyan, C. Boit, “Timing sensitivity of logical nodes in  scan design integrated circuits by pulsed diode Laser  Stimulation”.ISTFA 2008.


[19] J. Chaw, C. McMahon, Y. Shyang Ng, F. Beaudoin “Dual  Port RAM MBIST Failure Analysis using Time Resolved  Dynamic Laser Stimulation”, ISTFA 2008.


[20] A. Douin et al., “Influence of Laser Pulse duration in Single Event Upset testing”, IEEE transactions on Nuclear  Science, vol. 53,No 4, 2006.


[21] A. Douin IMS et al. "Picosecond Timing Analysis in Integrated Circuit with Pulsed Laser Stimulation.” IRPS 2007  pps 520 – 525.


[22] A. Reverdy et al., “Dynamic study of the thermal laser  stimulation response on advanced technology structures.” Microelectronics Reliability, Vol 48, Issue 10, 2008, pps  1689-1695.


Annular illumination and collection in solid immersion


Stephen Bradley Ippolito


IBM Semiconductor Research & Development Center Hopewell Junction, New York, USA


Hirotoshi Terada


Hamamatsu Photonics, Systems Division


Hamamatsu City, Japan


Tailoring  the  angular  spectrum  with  annular illumination  and  collection  can  significantly improve integrated circuit analysis with an optical microscope, when combined with solid immersion.


We  present  the  development,  testing,  and optimization of a simple and compact apparatus to implement annular illumination and collection in a Hamamatsu  iPHEMOS  system.  We  demonstrated improved  imaging  of  an  IBM  45nm  silicon-oninsulator  circuit,  with  annular  illumination  and collection in confocal scanning optical microscopy and widefield microscopy with an InGaAs camera.


Electrical  test  and  characterization  routinely identify deficiencies in the design and fabrication of integrated circuits.  Subsequent root cause analysis of  these electrical  deficiencies  provides  corrective actions  to  improve  the  integrated  circuit  yield.


Measurements by optical, scanning probe, electron beam, ion beam, and atom probe microscopes are necessary  to  reach  analytical  conclusions.  Optical microscopy measurements may range from simple visual inspection to more complex combinations of optical  and  electrical  interaction.  Both  the  spatial addressability of optical microscopy and generation of deficient electrical behavior are often necessary for analytical success.


In  optical  absorption  microscopy,  an  electrical response  in  the  circuit  is  generated  by  the absorption  of  focused  light  from  an  optical microscope through carrier generation and heating.


In practice, a confocal scanning optical microscope simultaneously acquires a confocal reflection and an absorption image. The confocal reflection image is required  for  focusing  and  laterally  registering  the absorption  image  to  the  circuit  layout.  In  optical


emission  microscopy,  light  emitted  by  the  circuit during  electrical  stimulation  is  collected  by  an optical  microscope.  In  practice,  a  widefield microscope  with  a  high  sensitivity  camera sequentially  acquires  a  widefield  reflection  image with illumination,  and an emission image without illumination.  The  widefield  reflection  image  is required  for  focusing  and  laterally  registering  the emission image to the circuit layout.


Optical  interaction  with  transistors,  through  the backside of the silicon substrate is often necessary,because opaque interconnect metal hinders frontside optical  microscopy.  Diffraction  limits  optical microscopy  through  the  substrate,  to  spatial resolutions  that  are  insufficient  to  resolve  the smallest  features  in  modern  integrated  circuits.


Furthermore, contribution to the images by multiple transistor  and  interconnect  layers  hinders longitudinal  localization  and  accurate  lateral registration  to  the  circuit  layout.  Thus,  improved lateral  and  longitudinal  spatial  resolution  will significantly  increase  the  information  gathered  by optical microscopy.


The optical fields in the substrate can be represented by  an  angular  spectrum  of  plane  waves.[1]  Each plane  wave  component  has  a  wave  vector,  ksub,composed of lateral and longitudinal wave vectors,kr-sub and  kz-sub,  respectively,  which  must  satisfy Equation  (1).  The  wavenumber,  ksub,  is  the magnitude  of  ksub and  is  equal  to  the  free  space wavenumber,  k0, multiplied by the refractive index of  the  silicon  substrate,  nsub.  The  lateral  and longitudinal  wavenumbers,  kr-sub and  kz-sub,respectively,  must  satisfy  Equation  (2)  due  to orthogonality.


ksub = kr-sub + kz-sub


kz-sub2 = nsub2 k02 − kr-sub2


(2)


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 60-64


Light  directly  coupled  into  a  planar  substrate contains only plane wave components with kr-sub less than  k0.  However,  light  coupled  through  a  solid immersion lens (SIL),  as illustrated in Figure 1(a),can also contain components with  kr-sub between  k0 and nsubk0. With a full angular spectrum, the ultimate limits in lateral  spatial resolution can be achieved with proper microscope and SIL design. The lateral


be achieved with proper microscope and SIL design. The lateral


|yellow|red|red|yellow|
|---|---|---|---|

spatial resolution of integrated circuit imaging with a SIL has been continually improved since the first experimental demonstration in 2000.[2-5] However,the  longitudinal  spatial  resolution  obtained  was never capable of resolving the individual layers in modern integrated  circuits.  Thus,  the images  with excellent spatial resolution were difficult to laterally


→


stop


SIL


substrate


register, due to the convolution of multiple layers.


interconnect→


(a)


(b)


Figure 1: Solid immersion lens (SIL) microscopy (a) without and (b) with annular illumination and collection.


In  bulk  technologies,  transistors  reside  in  the substrate,  but  in  silicon-on-insulator  (SOI)technologies, transistors reside in a thin silicon layer above  a  buried  oxide  on  the  substrate.  For  SOI technologies, the circuit can be approximated as a stratified medium, which permits calculation of the optical fields from each plane wave component by the  characteristic  matrix  method.[6]  Since  the lateral  wavenumber  in  the  buried  oxide,  kr-box,  is equal  to  kr-sub,  the longitudinal  wavenumber in the buried oxide,  kz-box,  must satisfy Equation (3). The refractive index of the buried oxide, nbox, near 1.5, is significantly  lower  than  nsub,  near  3.5.  Thus,components  with  kr-sub greater  than  nboxk0 yield imaginary values for  kz-box and therefore evanescent fields in the buried oxide.


kz-box2 = nbox2 k02 − kr-sub2


(3)


According to geometrical  optics, the position of a ray  intersecting  a  pupil  surface  of  an  imaging system is a function of the angle of the ray in the object space and is independent of the position of the ray in the object space. Therefore, spatial light modulation  at  a  pupil  surface  allows  angular


spectrum control throughout the full field of view in the object space. However, spatial light modulation at  any  other  non-imaging  surface  intersecting  the optical path also permits angular spectrum control,although within a more restricted field of view. A central  SIL  with  a  radius  of  curvature,  R,  has  a concentric  spherical  pupil  surface  at  a  radius  of nsubR/(nsub-1). An aplanatic SIL has the same pupil surface  within  the  paraxial  limit,  but  at  higher angles, parallel rays in the object space intersect at radii between R and nsubR/(nsub-1), if at all. Angular spectrum control  can  be  implemented  with  a  SIL that  is  fabricated  separately  or  on  the  substrate itself.[7-9]


Interconnect  metal  fabricated  on  the  frontside  of transistors is surrounded by transparent interconnect dielectric,  with  a  refractive  index,  ndie,  between 1 and 2. We approximate the circuit as a stratified medium,  due  to  its  material  and  geometrical complexity.  Under  this  approximation,  the  lateral wavenumber in the dielectric, kr-die, is equal to kr-sub,so  the  longitudinal  wavenumber  in  the  dielectric,kz-die, must satisfy Equation (4).


kz-die2 = ndie2 k02 − kr-sub2


(4)


The  interface  between  the  transistors  and interconnect  dielectric  is  a barrier  to  light,  with a critical  angle  of sin-1(ndie  /nsub).  Figure  1 illustrates sub-critical  and  super-critical  components  in  red and  yellow,  respectively.  Only  sub-critical components,  with  kr-sub less  than  ndiek0,  can propagate into the dielectric without first scattering from  fabricated  structures.  Super-critical components,  with  kr-sub greater  than  ndiek0,  yield evanescent  fields  in  the  dielectric,  and  are  only accessible with a SIL. Therefore, optical interaction with  the  interconnect  can  be  excluded  by  having only  super-critical  components  with  lateral wavenumbers high enough to yield short evanescent decay lengths in the dielectric. In SOI technologies,a  balance  must  be  reached  between  maximizing


evanescent  coupling  across  the  buried  oxide  and minimizing  the  evanescent  decay  length  in  the dielectric. A centered circular stop, as illustrated in Figure 1(b),  is a simple spatial  light  modulator to achieve  this  annular  illumination.  Annular collection, which also results from the stop, further improves  reflection  imaging,  by  blocking  the returning  light  that  was  scattered  from  the fabricated  structures  in  the  dielectric.  Annular collection  reduces  the  collection  efficiency  of emission imaging while improving the resolution by blocking  scattered  light.  Longitudinal  resolution enhancement  in  solid  immersion  microscopy with annular  illumination  and  collection  was  first experimentally  demonstrated  in  2008.[10]  Lateral resolution  enhancement  with  annular  illumination and collection followed shortly,[11] leading to new record resolutions since then.[12,13]


10μm


19


SUREER


(a) 0.0-2.5NA


(b) Si layout


(c) 1.9-2.5NA


(d) 1.1-2.5NA


(e) 1.4-2.5NA


(f)


1.7-2.5NA


UCCTE


Figure 2: (a) Conventional confocal reflection image compared with (b) silicon transistor layout and (c-f)annular illumination and collection images, with angular spectrum noted.


BHMNE


CRMAAS


CRRESS


shpe £n


BEMT


Figure 3: (a) Conventional widefield microscopy images from an InGaAs camera compared with (b) silicon transistor layout and (c-f) annular illumination and collection images, with angular spectrum noted.


Resolution enhancement  with annular  illumination and collection was demonstrated in the Hamamatsu iPHEMOS  system  while  imaging  an  IBM  45nm silicon-on-insulator chip at full substrate thickness.


We designed  a  set  of  interchangeable  stops  with varying  radii  that  are  slid  onto  the  mechanical mount  that  holds  the solid  immersion  lens  to  the 50X  objective.  The  central  solid  immersion  lens was  made of  silicon  and designed  for  a  substrate thickness  of  800m. Images  acquired  through the silicon substrate with the confocal scanning optical microscope  and  the  1300nm  laser  are  shown  in Figure  2.  Accurate  fault  isolation  requires  strong correlation between confocal reflection images and the physical  layout  of the silicon transistor device layer  and  associated  shallow  trench  isolation dielectric.  The  conventional  confocal  reflection


image,  shown  in  Figure  2(a),  exhibits  weak correlation with the smallest features of the silicon transistor  layout,  shown  in  Figure  2(b).  The conventional  confocal  reflection  image  was  taken with  a  full  angular  spectrum  between  zero  and


2.5NA. On the other hand, the confocal  reflection image  acquired  with  annular  illumination  and collection,  shown  in  Figure  2(c),  shows  strong correlation  with  the silicon  transistor  layout.  This image was taken under the same conditions, except with annular illumination and collection having an


thickness of 800um. Images acquired through the


angular spectrum between 1.9 and 2.5NA, with the light  below  1.9NA  blocked  by  the  stop.  Figure 2(d)-(f)  were  taken  under  the  same  conditions,except with different angular spectra resulting from stops with different radii.  The effect  of increasing radius can be seen by following the images counterclockwise around the layout, shown in Figure 2(b).


Similar  comparisons  between  conventional  and


annular illumination and collection images acquired via widefield microscopy with the InGaAs camera are  shown  in  Figure  3.  The  reduction  in  image intensity  between  Figure  3(a)  and  3(c)  was approximately  30%.  Improvements  in  correlation between  silicon/dielectric  layout  and  microscopy images were demonstrated in both experiments. The 300nm lateral  spatial  resolution obtained with the solid  immersion  lens  easily  resolves  the  650nm pitch fill shapes seen diagonally in all of the images.


Annular  illumination  and  collection  permits significantly  smaller  transistor  shapes  to  be resolved,  by  imaging  only  the  silicon  transistor layer,  as  opposed  to  a  convolution  of  all  of  the fabricated layers. Improvements were demonstrated in both confocal  scanning optical  microscopy and widefield  microscopy.  Thus,  significant improvement in fault isolation by optical absorption and  emission  microscopy  are  expected  with  this technique.  With  the  continuing  research  and development  in  the  field  of  solid  immersion microscopy,  fault  isolation  to  the  discrete  device level  has  been  maintained  in  optoelectronic microscopy, despite the scaling of integrated circuit features. The authors would like to thank the many groups  that  continue  to  contribute  to  this  area  of applied physics.[7-12]


[1] L. Novotny, B. Hecht, Principles of NanoOptics (Cambridge: Cambridge UP, 2006).


[2] S. M. Mansfield, G. S. Kino,  Applied Physics Letters 57, 2615 (1990).


[3] S. B. Ippolito, B. B. Goldberg, M. S. Ünlü,


Journal of Applied Physics, 97, 053105 (2005).


[4] S. B. Ippolito, B. B. Goldberg, M. S. Ünlü,


Applied Physics Letters, 78, 4071 (2001).


[5] S. Ippolito, Nature Photonics, 2, 273 (2008).


[6] M. Born, E. Wolf, Principles of Optics, 7th ed.


(New York: Cambridge UP, 1999).


[7] T. Koyama, E. Yoshida, J. Komori, Y. Mashiko,T. Nakasuji, H. Katoh, International Reliability


Physics Symposium (Piscataway: IEEE, 2003).


[8] F. Zachariasse, M. Goossens, International


Symposium for Testing and Failure Analysis


(Materials Park: ASM, 2005).


[9] S. H. Goh, C. J. R. Sheppard, A. C. T. Quah, C.


M. Chua, L. S. Koh, J. C. H. Phang, Review of


Scientific Instruments, 80, 013703 (2009).


[10] S. B. Ippolito, P. Song, D. L. Miles, J. D.


Sylvestri, Applied Physics Letters, 92, 101109


(2008).


[11] F. H. Köklü, S. B. Ippolito, J. I. Quesnel, B. B.


Goldberg, M. S. Ünlü, Lasers and Electro-Optics


Society Annual Meeting (Piscataway: IEEE, 2008).


[12] K. A. Serrels, E. Ramsay, D. T. Reid, Applied Physics Letters, 94, 073113 (2009).


[13] F. H. Köklü, S. B. Ippolito, B. B. Goldberg, M.


S. Ünlü, Optics Letters 34, 1261 (2009).


Backside IR Raman Temperature Measurements


R. Aaron Falk, Tram Pham


Quantum Focus Instruments Corp., OptoMetrix Division, Tukwila, WA, USA


Grant Albright


Quantum Focus Instruments Corp., Main Office, Vista, CA, USA


Spatial resolution limitations of IR thermal microscopy also  limit the temperature accuracy for small thermal sources. Use  of Raman temperature measurements significantly improves  spatial resolution and thereby temperature accuracy. Previous, visible-wavelength, Raman temperature measurements are  limited to top side measurements in silicon. This paper  describes the first ever IR Raman measurements in silicon and  demonstrates its use for backside temperature measurements.


Micro-temperature measurement in semiconductor devices  using IR thermal emission is a well known technique [1]. Careful calibration of the camera and emissivity effects can  result in temperature resolution of better than 0.1 K. However, temperature accuracy can be compromised by limited spatial  resolution. If the size of the temperature source is significantly  smaller that the optical spot size, then an average temperature  is measured. This average temperature is determined by the  convolution of the source spatial distribution with the optical  spatial response and is always less than the ture peak  temperature.


The use of Raman temperature measurements was introduced  to the FA community by M. Kuball, et al. in 2007 [2]. This  paper represented the culmination of nearly a decade of effort  for Raman temperature measurements in large bandgap  semiconductors, e.g. SiC. The advantage of Raman  temperature measurements over IR temperature measurements  is that the spatial resolution is determined by the probe laser  spot size. The laser wavelength (typically 488 or 532 nm) is  much shorter than the IR thermal wavelength (typical the band  from 2-4 micron). Diffraction limit indicates a spot size  reduction of a factor of ~ 6 for the laser probe. The effect of  this spot size reduction on temperature accuracy was clearly  demonstrated by Kuball, et al. An additional benefit (demonstrated by Kuball) of the Raman temperature  measurement approach is the ability to obtain depth  information.


The paper describes the extension of Kuball’s efforts to  silicon backside measurements through use of a near IR (1342


nm) laser probe. Several significant obstacles stood in the way  of obtaining this goal. Comparison with IR thermal emission  temperature measurements is made.


Affect of Spatial Resolution on Temperature Accuracy


The temperature response of any optical temperature sensor is  given by the spatial convolution of the point response of the  sensor, R(x,y,z) with the actual temperature distribution  T(x,y,z) over the spatial coordinates, with z the longitudinal  coordinate (the optical axis) and x, y the transverse  coordinates. Under the assumption of a thin heat layer, the z  coordinate can be ignored and the two functions can be  reduced to R(x,y) and T(x,y).


For most optical sensors (e.g. a thermal emission camera), the  imaging response and the temperature response are identical. In addition the response is generally symmetric about the two  transverse axis and must have a finite integral, e.g. it is a  Bessel function or a Gaussian function that depends only on  the radius, r = (x2 + y2)1/2. In this case, spatial resolution is  typically defined as some fraction of the width of the response  function.


By extension, NCVS at CA contact level can provide a means  to localize dopant defects, identify anomalous buried trench  capacitor leakage, resistive back end of line (BEOL) via  stacks, especially for silicon on insulator (SOI) substrates with  a buried oxide layer that isolates the Rx active silicon area  from the underlying silicon substrate.


Other applications for NCVS involve detection of capacitance  differences in via stacks associated with FEOL and BEOL  processing.


NCVS has been particularly successful for isolating defects in  high K gate structures that may not yield any anomalous DC  IV electrical characteristics.


Nano CV characterization offers opportunities for discrete  device localization, especially in SOI hardware.


Nanoprobe Capacitance Voltage Spectroscopy has  demonstrated the ability to detect buried trench capacitor  leakage in SOI embedded DRAM cells [2].


The further scaling in MOSFET gate length features enabled  by high k gate films underscores the importance of NCVS to  detect trapped charge, gate-drain overlap (Miller Capacitance), as well as dopant fluctuations in discrete devices.


NCVS is another powerful method for localization a defective  device in applications where discrete AFP probing would be  impractical.


A means is now available for AFP-assisted SCM or multiple  NCVS localization of junction defects and electrical C-V  measurements of gate oxide defects without the exacting and  time-consuming sample preparation steps of conventional  SCM analysis [6, 7, 8, 9, 10, and 11]. This approach permits  accumulation / inversion mode imaging and rapid localization  of the defect in the MOSFET (source or drain) device.  Multiple AFP probe tips permit independent biasing of  source/drain tungsten via level contacts simultaneously with  AFP contacts to the gate for discrete device C-V  measurements.


The authors wish to acknowledge the design and development  efforts of Atomic Force Probe NCVS by Andrew Erickson and  Peter Harris of Multiprobe. The authors also wish to  acknowledge the sample preparation contributions of Bruce  Redder employed in this paper. The authors also wish to  acknowledge helpful technical discussions with Stephen  Ippolito of IBM.


1. T.Kane, M. Tenney, A. Erickson, P. Harris, Calibration of


Nanoprobe Capacitance-Voltage Spectroscopy(NCVS),


ISTFA 2008, pp. 217-231 (2008)


2. T. Kane, M. Tenney, A. Erickson, S. Phan, Challenges of


Atomic Force Probe Characterization of Logic Based


Embedded DRAM for on-Processor Applications, ISTFA


2007,  pp. 46-51 (2007)


3. K. Ramanujachar, Scanning Capacitance Microscopy at        Transistor Contact Level, ISTFA 2004, pp. 482-486


4.  E.H. Nicollian, J.R. Brews, MOS (Metal Oxide


Semiconductor) Physics and Technology, “C-V Curves,       pp. 384-385, (1984)


5. Jean-Yves Rosaye, et. al. C-V and C-P Characterization


Sensitivities for Fast and Slow-State Traps in Very Thin


Oxide MOSFETS, Proceedings of International


Reliability Physics Symposium, pp. 353-35 (2004).


6. Matey, J.R. and Blanc, J.  Scanning Capacitance


Microscopy, J. Appl. Physics, 57 (5), 1 March 1985, pp.


1437-1444.


7. CC. Williams, J. Slinkman, W.P. Hough, H.K.


Wickramasinghe, “Lateral Dopant Profiling with 200nm


Resolution with Scanning Capacitance Microscopy”,


Appl. Phys. Lett. 55, 1662 (1989).


8. C.C. Williams, J. Slinkman, W.P. Hough, H. K.


Wickramasinghe, “Two Dimensional Dopant Profiling


using Scanning Capacitance Microscopy”, J. Vac. Sci.


Technol. B n. 8, 895 (1990)


9. V.V. Zavyalov, J. McMurray, C.C. Williams, Surface and


Tip Characterization for Quantitative Two Dimensional


Dopant Profiling by Scanning Capacitance Microscopy,


from Characterization and Metrology for ULSI


Technology: 1998 International Conference, American


Institute of Physics (AIP) Conference Proceedings, March


1998, pp 449-453 (1998).


10. T. Tong, A. Erickson: Current Image Atomic Force


Microscopy (CI-AFM) Combined with Atomic Force


Probing (AFP) for Location and Characterization of


Advanced Technology Nodes, ISTFA 2004, pp. 42-46 .


11. T. Kane, M. Tenney, Electrical Characterization of sub30nm Gatelength SOI MOSFETs, Proceedings


International Symposium for Test and Failure Analysis,


ISTFA 2004, pp. 33-37


The SRAM Soft failure analysis with SNM & TR characterization by Nanoprobing in sub 45nm


Jakyung Hong


Samsung Electronics Co., KOREA


jakyung.hong@samsung.com 82-31-209-5475


S.J. Cho, Y.W. Han,H.S. Choi, T.E. Kim, S.J. Son,H.S. Kim, S.D.Kwon, Y.S.Oh


Using the nanoprobe technique, transistor characteristics in an  actual SRAM cell can directly measured. To define the root  causes of a marginal soft failure, characterizing at the  transistor level has its limits in understanding cell stability and  failure mechanisms. Moreover, as shrinkage of SRAM cell  dimensions, the electron beam irradiation comes to an  important issue. When the electron beam is focused at an  SRAM cell for a time, it changes transistor characteristics, such as Vth shift and Idoff, Idsat swing.  Probing with a SEM  based nanoprober to get the correct data, electron beam  influence must be reduced. Probing at the metal1 layer, makes  it is possible to avoid electron beam influence; furthermore it  allows the coupled analysis of cell stability and TR  characteristics.


This paper presents the process of measuring SNM (static  noise margin), WNM (write noise margin) with 6 pin  nanoprober, and characterization & analysis of SRAM cell  stability through the case study of 45nm devices SRAM soft  failures.


Experimental setup


The SRAM cell made up of 6 transistors, two cross-coupled  inverters and two pass NMOS transistors connecting the cell to  the bit line and word line as shown in Fig [1a]. At the metal1  layer, SRAM is an isolated bit cell, allowing each cell’s SNM  measurement. Normally 8 prober pins are needed to measure  the read SNM. However, Most of the nanoprobers are  equipped with 6 pins. Due to the lack of probing pins, read  SNM cannot be tested at once in the actual cell. Therefore we  need to separate measuring conditions, such as PU-PD / PGPD / PU-PG (PU-pull up pFET, PD-pull down nFET, PG-pass  gate nFET) inverter pairs. Then, summarize their output data  of Vout node to calculate the SNM value. Each cell has 2 pairs  of PU-PD / PG-PD / PU-PG inverter set. Fig [1b] is shown as  the probing status of the PG-PD inverter in the metal1 layer. During the PU-PD inverter testing, Vdd and N-well are biased  at high voltage. Vss and P-well are at 0 volts. Sweep Vin while  measuring voltage on the Vout connection. The PG-PD


inverter testing condition is word line (WL) and bit line (BL) are based at operation voltage, P-well and Vss are at 0 volts. The PG-PS inverter testing condition is operation voltage at  WL, N-well and Vdd. 0 volts at BL and P-well. Vin and Vout  assignments are same.


The PU-PD, PG-PD inverters are able to be measure with 6  prober pins. However the PU-PG inverter needs 7 pins. Accordingly when the PU-PG inverter was measured, the rest  of the nodes are probed by pins, but P-well (P-sub) was  alternated to GND of sample loader chuck.


In 45nm devices the metal1 layer is made of tender copper, therefore tungsten pins are too strong to probe metal. It is easy  to make a shortage between metal lines by probing. It is  important that nanoprober pins are treated carefully.


Fig [1a]: Schematic layout of SRAM Cell


Fig [1b]: the PU-PD inverter probing in metal1


PU1


PD1


艺PU2


PD2


PG1


PG2


Vdd


Vss  Vin


Vout 申申Zπ 1a


INV1


INV2


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 76-80


A. Measuring SNM with 6 pins and the proof of reliability  through simulation


By collecting the SNM values for a bit cell, we can determine  the bit’s stability. For each inverter set’s output data’s  reliability, we first compare simulation with the good cell’s  Vout in actual 45nm SRAM devices.


Fig [2a] shows the simulation butterfly curves of the PU-PD  inverter, PG-PD inverter and their calculated read SNM curves  in series. Simulation data is regarded as 6 pins probing. Also, the read SNM is displayed by comparing Vout max of the PUPD inverter and the PG-PD inverter.


Fig [2a]: Simulation Vout curves of the PU-PD inverter / the  PG-PD inverter / the read SNM


The good cell butterfly curves are measured in the metal1  layer such as Fig [2b]. A shape of the good cell inverter and  SNM curves are similar to simulation data.


[


Fig [2b]: the good bit cell Vout curves of the PU-PD inverter / the PG-PD inverter / the read SNM


In the next step, by comparing simulation data, we determine  any differences between 6 pins measured read SNM and 8  pins. Fig [3] shows the read SNM curves under two  conditions, one is 8 pins measured read SNM and the other is  maximized Vout SNM value comparing the PU-PD inverter  and the PG-PD inverter. When two kind of read SNM curves  overlap in same axis, there is a little difference at the corner of  curve’s crossing point, between pink and yellow or green and  blue. However, the crossing point area-gray box- doesn’t mean  there is an error of SNM. Crossing points appear by  numerically calculated Vout values, with no correlation to  SNM value. Focusing on the SNM value, it is found that both  read SNM curves have the same size of rectangles. Therefore, we discovered that by using 6 pins, the read SNM can be  measured.


Fig [3]: Simulation data of read SNM under 2 conditions, one  is 8 pins probed curve and the other is maximized Vout SNM  value comparing PU-PD and PG-PD with 6 pins.


0.0


1.0


1.2


0.0 0.2 0.4 0.6 0.8 1.0 1.2


Vin[V]


PUPD INV1 PUPD INV2


:


n


o0.6


PGPD INV1 PGPD INV2


0.0 0.2 0.4 0.6 0.8 1.0 1.2 Vin[V]


PUPD + PGPD Vout Max INV1 PUPD + PGPD Vout Max INV2


m


Good Inv1 Good Inv2


A


]


o0.8


0.20.2


toGood Inv1 Good Inv2


/


PUPD+PGPD Vout MAX INV1 8Pin Read SNM INV1


PUPD+PGPD Vout MAX INV2 8Pin Read SNM INV2


B. Case study (Disturb and LVcc margin failure in 45nm  device)


1) SNM measurement in metal layer


The case study presents a single bit soft failure issue from


disturb failure at 1.1V. This sample was de-processed and


measured in the metal1 layer and the CA layer. There is no


abnormal PVC (passive voltage contrast) phenomenon in the


other samples with the same failure.


To compare the good and bad cell stability, for the first time,


measurements were made for each inverter pair (PU-PD/PGPD/PU-PG) in same layout. In Fig [4a~c] test conditions and


measured butterfly curves are shown in the actual cell. These


curves determine the Hold and read SNM with the Vdd held at


||Bad Inv1 Bad Inv2 |
|---|---|

1.1V. The square having the longest diagonal presents SNM,


and then the smaller of the two squares is used for determining


the SNM.


There is a 0.1V mismatch between 2 latches in the bad cell


PU-PD inverter. Fig [4a] shows the Hold SNM of the bad cell


is 0.32V, lower than good cell (0.44V). There is no difference A at the PG-PD inverter curves in Fig [4b]. Also the WNM


(Write noise margin) is able to measure using 6pins + GND.


There does not appear to be a significant gap in Fig [4c].


nA


AO


A[


]in


Fig [4a]: the bad/good cell Hold SNM (PU-PD inverter  curves)


n口


A0


A  1  A0


Fig [4b]: the bad/good cell (PG-PD inverter curves).


「 1A  0n


A[ n] A0


Fig [4c]: the bad/good cell WNM (PU-PG inverter curves)


To determine the read SNM, it is necessary to summarize the


PU-PD inverter and the PG-PD inverter curve. As mentioned


before, two curve’s crossing points – the gray box area doesn’t


affect any SNM value. As the Hold SNM reflects in the read


SNM, the read SNM of good cell is 0.15v, the bad cell is


0.05v. From the metal1 layer measuring data, it is possible to


infer that the bad cell inverter1 side’s stability is poor.


l


A C


Fig [4d]: the bad/good cell read SNM


Bad Inv1 Bad Inv2


Hold Vdd 1.1V  SNM = 0.32V


Hold Vdd 1.1V  SNM = 0.44V


0.4 n0.6[0.8


PD


PG


Vss=L  Vin


Vout


INV1 a


WL=H


BL=H


PW=L


Vin


000


PD  PU


Vss=L


Vdd=H


PW=L  NW=H


PU


INV1 宁


BL=L


1.0口


Read Vdd 1.1V  SNM = 0.05V


00.6


At


Read Vdd 1.1V  SNM = 0.15V


2) Transistor measurements in CA Layer


To obtain full electrical characteristics on 6 transistors, they  were measured under 1keV acceleration voltage SEM  conditions at the in CA layer. All the results were displayed in  table1. It was found that I-V characteristics of the good and  bad cell of PD, PS transistors were normal In Fig [5]. However, the PU1 saturation current in the bad cell was in -3.4uA, while in the good cell it was in -7.1uA.


Table1. Saturation current and threshold voltage comparisons  of the bad and good cell.


Fig [5a]: the I-V Characteristics of the bad/good PD  transistors. There is no difference between the bad and good  cell.


Fig [5b]: the I-V Characteristics of the bad/good PG  transistors. There is no difference between the bad and good  cell.


As shown in Fig [6], the bad cell PU1’s saturation current was  significantly lower than any other PU’s. There is a 57% of  saturation current difference within the bad cell PU transistors. Due to the bad cell PU1 weakness, the saturation current ratio


- alpha (PU/PD) is about 50% lower than the good cell, and  the gamma ratio (PG/PU) is over twice times higher. The PU1  of the bad cell performed weakly, and it induces asymmetrical  SRAM cell stability and causes disturb failure


Fig [6]: the I-V Characteristics of the bad/good PU  transistor. PU1 Idsat = -3.4uA, verses good PU1 Idsat=-7.1uA


The cross-section TEM image of the failing PU1 is shown in  Fig [7]. The PFA (physical failure analysis) results can also  explain the lower saturation current of PU1. This slightly  recess of the shared CA underneath was found to be the root  cause of a single bit soft failure. Such abnormal shared CA  caused the PU1 saturation current to be lower; more than half  and the bit cell instability.


0.E+00


2.E-05


4.E-05


6.E-05


8.E-05


-0.5


1.5


Vg[V]


Bad Cell PD1 Vd 0.05 Bad Cell PD1 Vd 1.1


Bad Cell PD2 Vd 0.05 Bad Cell PD2 Vd 1.1


Good Cell PD1 Vd 0.05 Good Cell PD1 Vd 1.1 Good Cell PD2 Vd 0.05 Good Cell PD2 Vd 1.1


Bad Cell PG1 Vd 0.05 Bad Cell PG1 Vd 1.1


Bad Cell PG2 Vd 0.05 Bad Cell PG2 Vd 1.1


Good Cell PG1 Vd 0.05 Good Cell PG1 Vd 1.1 Good Cell PG2 Vd 0.05 Good Cell PG2 Vd 1.1


-1.2E-05


-1.0E-05


-8.0E-06


-6.0E-06


-4.0E-06


-2.0E-06


0.0E+00


2.0E-06


-1.5


-1.0


Bad PU Vd -0.05 Bad PU Vd -1.1


Good PU Vd -0.05 Good PU Vd -1.1


-1.2


-0.8


-0.6


-0.4


-0.2


Vd[V]


Good Bad


Gate  PU1


Source


Drain


Fig [7]: Tilt-view SEM image and Cross-sectional TEM of  bad PU1 TR Shared CNT


Through this paper, we discovered that the local mismatch in  the bit cell caused by slight variation in the transistor  characteristics, such as Vth shift and Idsat, off variation, also  can easily induce a soft failure.


The analysis of the SNM & TR characteristic is successfully  demonstrated through the case study of 45nm SRAM devices. By testing the SNM at the metal1 layer, transistors are  protected from electron beam damage. Moreover, we  explained the act of the bit cell stability was linked with TR  characteristics.


Measuring SNM & TR characteristics are an important  methodology in understanding the stability of each bit cell and  failure mechanism depending on voltage, defects and other  factors. The next generation of nanoprobing analysis can be  expanded.


Acknowledgement


The author would like to thank the Physical Failure Analysis  group and TEM group for their assistance on the visual image.


[1] E. Hendarto, H.B. Lin, “Investigation of Soft Fail Issue in  Sub-Nanometer Devices Using Nanoprobing Technique”, Chartered Semiconductor, 15th IPFA. 2008


[2] Hung-Sung Lin, Chun-Ming Chen, “An Application of a  Nanoprobe Technique in the Characterization of  Advanced SRAM Devices”, UMC, 34thISTFA 2008, pp. 417~422


[3] S.L. Tho, P.K. Tan, “In-Depth Electrical Analysis to  Reveal the Failure Mechanisms With Nanoprobing”, IEEE Transaction on Device and Materials Reliability  2008, pp. 387 ~ 393


[4] S.L. Toh, Z.H. Mai, P.K. Tan, “Use of Nanoprobing as  the Diagnostic Tool for Nanoscaled Devices”, Chartered  Semiconductor, 14th IPFA. 2007, pp. 53~57


[5] Hung-Sung Lin, Wen-Tung Chang, “A Study of  Asymmetrical Behavior in Advanced Nano SRAM  Devices”, UMC, 13th IPFA. 2006, pp. 63~66


[6] S. Doering, R. Harzer, “Investigation on the Influence of  Focused Electron Beam on Electrical Characteristics of  Integrated Devices”, Qimonda, 33rd ISTFA.2007, pp. 210~213


Contact author information:


Samsung Electronics Co. LTD.


San #24 Nongseo-Dong, Giheung-Gu,


Yongin-City, Gyeonggi-Do, Korea 446-771


jakyung.hong@samsung.com


82-31-209-5475 Tel


82-11-600-5980 Mobile


82-31-209-0299 FAX


Bad  PU1


Good


Electrical Characterization of Different Failure Modes in sub-100 nm Devices  using Nanoprobing Technique


E. Hendarto, S.L. Toh*, J. Sudijono, P.K. Tan, H. Tan, Y.W. Goh, L. Zhu, Q. Deng, H.B. Lin, R. He, H.L. Li, Z.H. Mai, J. Lam


Chartered Semiconductor Manufacturing Ltd, Technology Development Department  60 Woodlands Industrial Park D Street 2, Singapore 738406


Phone: +65-6360-4923  Fax: +65-6362-2936  *Email: tohsl@charteredsemi.com


The Scanning Electron Microscope (SEM) based nanoprobing  technique has established itself as an indispensable failure  analysis (FA) technique as technology nodes continue to  shrink according to Moore’s Law [1-3]. Although it has its  share of disadvantages [4], SEM-based nanoprobing is often  preferred because of its advantages over other FA techniques  such as Focused Ion Beam (FIB) in fault isolation. Nanoprobing is a non-destructive approach to isolate defects, which continue to shrink in size as electronic devices become  smaller. This technique is often complemented by other nondestructive electrical FA techniques such as Conductive  Atomic Force Microscope (C-AFM) in order to identify  defective devices. This is true particularly when Vmin and  other related soft fail issues become prevalent in smaller nanodevices, thus increasing the frequency of “non-visible defect (NVD)” cases [5].


This paper presents the effectiveness of the nanoprobing  technique in isolating nanoscale defects in three different  cases. In two of these cases, the SEM Passive Voltage  Contrast (PVC) technique failed to identify the defective  location (Case A and C). Apart from identifying defective  nickel silicide (NiSi) and poly-contact short issues (Case A  and B respectively), nanoprobing also successfully isolated  the resistive contact location in a large Electrical Test (ET) structure (Case C). The nanoprobing technique greatly  assisted in the identification of failure mechanisms and thus  improved turnaround and device yield.


An SEM-based Zyvex sProber Nanomanipulator System was  used to perform nanoprobing on the defective samples. This  tool consists of a manipulator controlling the fine movements  of four tungsten nanoprobes which have tip diameter of 40 nm  and below. Figure 1 shows the four-prober manipulator  system in an SEM chamber. Two failed Static Random Access  Memory (SRAM) devices and one ET structure were  investigated.


A.  Soft-Fail Defect Caused by Asymmetrical NiSi  Formation


An SRAM single bit soft fail was identified from a wafer  suffering from zero yield. The sample was deprocessed and  inspected layer by layer from via 1 using the SEM PVC  technique, but no visible defect was found until the contact  layer. Before further deprocessing was carried out, nanoprobing was utilized at the contact level to further  understand the root cause of the soft fail.


Figure 2 shows the contact orientation of an SRAM cell with  the wafer notch at the right. A total of two pull-up (PU), two  pull-down (PD) and two pass-gate (PG) transistors makes up  one bit cell. With notch on the right, any transistor in the left  portion of the cell is denoted by the number “1” and any one  on the right is denoted by the number “2”.


Since the SEM PVC technique did not identify the failing  transistor within the fail bit, all six transistors were probed and  their electrical data obtained. A random nearby good bit was  selected and its six transistors probed so that their electrical  data could be compared with those of the bad bit.


Figure 1: Four-probe manipulator system in an SEM chamber


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 81-87


Figure 2: Contact orientation and the six transistors within a  bit cell with wafer notch on the right


Figure 3 tabulates the I-V characteristics of the PD1 transistor  in the bad and good SRAM cells. Figure 3(a) is the curve  obtained by sweeping the drain contact (drainsweep) of the  transistor PD1 in the bad SRAM cell, while figure 3(b) was  obtained by sweeping the source contact (sourcesweep) of the  same transistor. It is clear from these figures that the shapes of  the I-V curves were not identical, and the ION values of the  drainsweep and sourcesweep curves also differ. The ION  obtained by drainsweep is around 25 μA in contrast to 40 μA  obtained by sourcesweep.  Figure 4 tabulates the same data for  the PD2 transistor.  The shapes of the I-V curves of the bad  PD2 transistor are identical, be it drainsweep or sourcesweep, as shown in Figures 4(a) and 4(b). The ION is exceptionally  high at around 105 μA. This is a mismatch of approximately


120% between PD1 and PD2 transistor ION in the bad cell. There was no abnormality in ION values of PUs and PGs.


18


In comparison, the I-V characteristics of the PD1 and PD2


RT


transistors of the good SRAM cell shown in Figures 3(c,d) and 4(c,d) were similar whether the drain or source contacts  were swept. The ION value measured is around 85 μA resulting


商


in virtually no ION mismatch between PD1 and PD2.


Because of the asymmetrical nature of the I-V drainsweep and  sourcesweep curves in bad PD1 transistor, Transmission  Electron Microscope (TEM) was employed to perform a  cross-sectional cut along the source and drain contacts of PD1  shown in Figure 5(a).  The result shows abnormal NiSi  formation under the source contact as shown in Figure 4(b).  Nanoprobing played a pivotal role in identifying the defective  transistor, and it enabled us to perform a TEM cut along the  correct direction, targeting the defective transistor. It can be  concluded that the lack of symmetry of the bad PD1 I-V  drainsweep and sourcesweep curves is caused by the  asymmetrical formation of the NiSi below the contacts.


Transistor Measurement


||Bad SRAM Cell Good SRAM Cell |Bad SRAM Cell Good SRAM Cell |Bad SRAM Cell Good SRAM Cell |Bad SRAM Cell Good SRAM Cell |Bad SRAM Cell Good SRAM Cell |Bad SRAM Cell Good SRAM Cell |Bad SRAM Cell Good SRAM Cell ||||||
|---|---|---|---|---|---|---|---|---|---|---|---|---|

|Drainsweep |(a) ION ~25 μA (c) ION ~85 μA |(a) ION ~25 μA (c) ION ~85 μA |(a) ION ~25 μA (c) ION ~85 μA |(a) ION ~25 μA (c) ION ~85 μA |(a) ION ~25 μA (c) ION ~85 μA |(a) ION ~25 μA (c) ION ~85 μA |(a) ION ~25 μA (c) ION ~85 μA ||||||

||8.0E-05|8.0E-05|8.0E-05|8.0E-05|8.0E-05|8.0E-05|||||||

||7.0E-05|7.0E-05|7.0E-05|7.0E-05|7.0E-05|7.0E-05|||||||

||6.0E-05|6.0E-05|6.0E-05|6.0E-05|6.0E-05|6.0E-05|||||||

||5.0E-05 -----路 a 4.0E-05|5.0E-05 -----路 a 4.0E-05|5.0E-05 -----路 a 4.0E-05|5.0E-05 -----路 a 4.0E-05|5.0E-05 -----路 a 4.0E-05|5.0E-05 -----路 a 4.0E-05|||||||

As a concrete example, a radially symmetric, normalized  Gaussian response function of the sensor


R r


R


( )


exp


where R is a measure of the response width and a radially  Gaussian temperature distribution


T r T


T


Base


0222exp


where T is the measure of the temperature distribution width,  are assumed. Tbase is the baseline (ambient) temperature and T0 is the peak temperature difference from Tbase. After  performing the convolution, it can be shown that the measured


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 65-72


peak temperature difference, Tm is related to the actual peak  temperature difference T0 by


T TmOTT T


08


Tm=To0 √(a7+ak)2 2


Equation 3 indicates that the measured peak temperature will  always be less than the actual peak temperature, but will


OO0


日


approach it asymptotically as OR becomes small compared toapproach it asymptotically as R becomes small compared to  OTT


The Figures 1-4 below demonstrate this effect. The test device  is a standard digital IC with a ‘point-like’ hot spot along the  lower edge. The device is ‘flip-chip’ mounted, so is imaged  through the backside. The images were taken with our  standard IR temperature mapping system at three different  magnifications, 1X, 4X and 12X with image resolutions of 31, 8, and 2.8 microns respectively1. A strong localized signal is  seen at the short location. The peak temperature difference, Tm was determined for each magnification as 7 K, 24 K and 40 K  for the respective magnifications of 1X, 4X and 12X. Clearly, resolution significantly affects the measured temperature.


Figure 1: IR temperature map of silicon test device at 1X  magnification


1 The resolution limit of 1X and 4X magnifications is  primarily due to pixel size, whereas the 12X magnification is  diffraction limited.


Figure 2: Overlay of thresholded 1X IR temperature map onto  backside IR image of silicon test device.


Figure 3: Overlay of thresholded 4X IR temperature map onto  backside IR image of silicon test device.


Stokes


Anti-Stokes


Scatter


Figure 4: Overlay of thresholded 12X IR temperature map


Energy


onto backside IR image of silicon test device.


Photon


Phocon


Finad


InitialVibrational


Figure 5 plots peak temperature difference versus imaging


initial崔FinaiLevels


resolution. A fit to this data was made using Equation 3. The  fit is quite good and indicates a true peak temperature of ~ 57


K and a value of~ 3 micron for or. Clearly, even the highestK and a value of ~ 3 micron for T. Clearly, even the highest  resolution available produces a significant under estimate of  the true peak temperature.


Note that this fitting process works well enough to determine  the true peak temperature for a Gaussian temperature  distribution. However, it will not work for a general, nonGaussian distribution.


0 10 20 30 40 Temperature Difference (K)50 60


Image Resolution (micron)


Data Fit


Figure 5: Plot of measured temperature (blue diamonds) versus image resolution along with theoretical fit (solid red  line)


Raman Temperature Measurements


Raman Scattering in Semiconductors


Raman scattering is a process by which light gains or loses  energy when it scatters from a molecule [3]. The gain or loss  is via vibrational states in the molecule and a so called virtual  excited state (see Figure 6). Photon energy loss occurs when  the molecule starts in the ground state and ends up in the  excited state. Photon energy gain occurs when the molecule  starts in the excited state and ends up in the ground state. Thermal equilibrium determines the ratio of excited to ground  state molecules, and therefore the relative intensity of the two  components. Because the process is via a virtual excited state, it is a relatively rare event with only one photon in 1 to 100  million undergoing a Raman energy shift.


Virtual State


Figure 6: Energy diagram of Raman scattering illustrating  energy loss (Stokes scattering) and energy gain (anti-Stokes  scattering) from an incident photon.


Crystalline structures such as semiconductors also vibrate at  characteristic phonon frequencies, so also exhibit Raman  energy shifts. An example spectrum is shown Figure 7 using  our 532 nm Raman microscope with a silicon target. As is  typical with all Raman spectra, the x axis is plotted as a ‘frequency’ given in inverse centimeters, cm-1, where the  value is determined by


v=1/ho-1/h = 1/0 – 1/


where where λo is the incident photon (laser) wavelength and λ is the0 is the incident photon (laser) wavelength and  is the  resultant Raman wavelength (in centimeters). The importance  of this representation is the independence of v from the inputof this representation is the independence of  from the input  laser wavelength


1000


2000


3000


4000


Intensity5000


(nw)6000


7000


8000


9000


10000


700


Raman Shift (cm-1)


Figure 7: Graph of Raman spectral response of silicon target  showing laser line (at 0 cm-1) and Raman line (at ~518 cm-1).


Virtually all semiconductor materials exhibit Raman scattering  with a shift related to the material photon energy. Some  examples are given in Table 1 below.


)


Table 1: Raman shifts (at absolute zero) for several  semiconductor materials.


Application of Raman Scattering to Temperature  Measurements


The Raman energy shift in a semiconductor depends on  several factors


Material stoichiometry


● Stress


●Temperature


Separation of temperature from the other factors is  accomplished through a pair of measurements with device off  and then on. The Figure 8 shows a set of ‘on/off’ measurements of the Raman line in silicon for two different  substrate temperatures. The change in the Raman line center  ( ~ 0.02 cm-1/K) is clear. As seen in Figure 8, the intensity of  the Raman line also changes. This intensity change can be  used to measure temperature as well, however errors occur in  this approach due to other intensity factors (e.g. background  fluorescence). Less obvious is that the line width also  changes, however this is a much weaker effect than the line  shift.


Sophisticated computer algorithms are used to accurately  determine the Raman line center to better than 1% of the first  moment of the line distribution (e.g. the standard deviation). This analysis was performed in silicon producing the results  shown in Figure 9. A linear shift with temperature is observed  along with a temperature resolution demonstration of ~ 1 K.


|Material |Raman Shift (cm-1 |
|---|---|

|AlN |798 |

|BN (ZincBlend) |1046 |

|C (Diamond) |1287 |

|GaAs |282 |

|GaN (Wurtzite) |732 |

|GaN (ZincBlende) |700 |

|GaP |410 |

|GaSb |239 |

|Ge |298 |

|InAs |241 |

|InN |587 |

|InP |346 |

|InSb |201 |

|Si |507 |

|SiC |837 |

0 500 u1000 n1500


V人


u 8


510


520


530


540


550


560


Ramon Shift (cm-1)


145 C 22 C


Figure 8: Graph of Raman line in silicon for two different  substrate temperatures.


Silicon - Line Crossing


516.5


517


0517.5 5


518


518.5 519


60


70


Temperature (C)


Figure 9: Measurement of Raman line shift in silicon with  substrate temperature. Error bars are almost invisible at this  scale.


Kuball, et al. have demonstrated the use of Raman line shift in  temperature measurements for several high bandgap  semiconductors [1]. An example is shown in Figures 10 and


11. Figure 10 is take with our IR temperature mapping system, which indicates the hot area of interest. Figure 11 shows  results from a set of Raman measurements taken along a line  between the drain and source and compares them with the IR  measurements along that same line and a theoretical  calculation. Clearly the higher spatial resolution of Raman  probe (~ 0.4 um for diffraction limited laser probe versus 2.8  um for the thermal emission described above) yields a far  better estimate of the peak temperature in the source-drain  gap.


50μm50m


Prof. Kuball, University of Bristol, UK,


IEEE Trans. Electron Dev. 53, 2438 (2006).


Figure 10: IR temperature map of AlGaN/GaN HFET  showing high temperatures in drain-source gap.


45


60 Temperature()°C801


u


140 160 180


S


tegasource


drain


，


Raman


3D sim.


11 IR


Position (μm)Position (m)


G


Prof. Kuball, University of Bristol, UK, IEEE Electron Dev. Lett. 23, 7 (2002); IEEE Trans. Electron Dev. 53, 2438 (2006).


measured  through


Figure 11: Graph comparing IR temperature map results (red  bars), Raman temperature data (blue squares) and theoretical  simulation (black line) for AlGaN/GaN HFET.


Raman Microscopy Hardware


The original work of Kuball, et al. was performed with a  standard microscope coupled into a Raman spectrometer. Imaging was performed with a separate camera, which was  aligned to the laser spot. The target device was moved by  placing it onto an XY stage. Moving the device produces  obstacles for probing, so we reconfigured the system directly  into a scanning laser microscope. The scanner is then used to  point the laser at the measurement locations.


Figure 12 shows a block diagram of this Raman microscope  configuration. A sharp cutoff color beam splitter is used to  separate the input laser wavelength from the longer  wavelengths that result from the Raman shift. The filter pass  band is from 200 to 1200 cm-1. The resultant laser imaging  and spectrometer paths are co-aligned so that they both point  at the some spot on the target. Laser power on the target is  relatively low (< 20mW) to prevent excess self heating  effects.


In operation, the laser is raster scanned over the test circuit  and the reflected light recorded to produce an image of the test  circuit. Software then allows the user to select a point, line of  N points, or area of NxM points to be measured. Raman  spectra are obtained for each point with the device both on  and off. The line shifts are calculated and then converted into  temperatures.


|26.5|55.9 85.3|114.6|
|---|---|---|

||Temperature ("C)||

A 1 second integration time at each point results in a  temperature error of ~ 3K. 10 second integration time reduces  the error to ~ 1K. Clearly, Raman temperature measurements  are rather slow compared to IR temperature measurements (typically 10 frames/sec). Thus, both systems have been  combined, the IR measurements being used for search and the  Raman measurements used when high resolution is required.


Figure 12: Block diagram of Raman microscope integrated  into laser scanning microscope.


Obstacles to IR Raman Temperature Measurements


The requirements of optical penetration through the silicon  substrate and non-production of photo-carriers forces use of a  relatively long probe wavelength in silicon. A laser with  wavelength of 1342 nm is commercially available with good  frequency stability and reasonable output power, so was used  for this work. There are several obstacles associated with  backside IR Raman spectroscopy in this wavelength regime.


1. The Raman signal scales as one over the laser probe  wavelength to the fourth power.


2. High refractive index of silicon narrows the


collection solid angle, further reducing the signal.


3. Longer wavelength requires use of InGaAs detectors  which have increased dark current and readout noise  as compared to their silicon counterparts.


4. Longer wavelength reduces the spatial resolution


unless special optics (e.g. SILs) are used.


The first three obstacles affect the measurement signal-tonoise ratio, SNR. A high SNR is required to accurately  determine the Raman line shift, thus directly affecting the  temperature measurement accuracy.


The first obstacle results from the basic physics of Rayleigh  and Raman scattering and would seem to be insurmountable. A inverse forth power scaling between our original efforts at  532 nm and the IR effort at 1342 nm would indicate a signal  reduction of ~40.


The second obstacle results from Snell’s law and the very  high, 3.5, refractive index of silicon [4]. For a standard (air  gap) objective, this effect will reduce the signal by an  additional factor of ~ 12.


InGaAs detectors have very high quantum efficiency over


Scan


their total wavelength band as compared to a silicon detector.


Mirror


High-Resolution


Color Beam


Spectrometer


However, they have significantly higher dark current (orders


Splitter


of magnitude) and significantly higher readout noise (factors  of 10-20). Dark current can be mitigated by sufficient cooling (- 90 0C for the test system), but the readout noise only  changes slightly with cooling. In the worse case, this third


PBS


lmaging


obstacle would add another factor of 20 reduction in SNR for


Detector


IR versus visible Raman measurements.


5 3


The total SNR reduction for these three effects is a whopping


2 n


factor of ~ 9,600. At this point one might decide to pack up


ml L as


DAQ Electronics


and go home. However, physics has chosen to play some


S e


useful tricks in our favor. First, the wavelength of light is not  fixed, but depends on the refractive index of the media.


Test Circuit


Specifically, the wavelength & relates to the wavelength inSpecifically, the wavelength  relates to the wavelength in  vacuum λo by λ = λ0/n with n being the refractive index. Laservacuum 0 by  = 0/n with n being the refractive index. Laser  wavelengths are given as the vacuum wavelength, so the  effective wavelength of a 1342 nm laser in silicon is ~ 383  nm. Using the forth power scaling yields an actual net gain of ~ 4 from the wavelength scaling factor!


An additional advantage gained in backside imaging is that  silicon is a very good heat conductor. Thus it is possible to use  3-4 times the laser power levels without concern of excess self  heating2.


The final bit of serendipitous luck in that very high SNR (100  or better) is needed to accurately determine the Raman line  shifts. The noise part of the SNR is an RMS sum of the  detector read noise and the shot noise due to the counting  statistics of the detected photocarriers. The high SNR  requirement forces a high enough signal count that the shot  noise component dominates over readout noise in our  measurements. In the end, the visible and IR Raman systems  actually produce similar SNR.


The forth obstacle is spatial resolution when focusing through  a high refractive index interface [4]. This obstacle can be  overcome through use of liquid and solid immersion  objectives [5]. Resolutions as good as 166 nm have been  demonstrated using solid immersion objectives [6]. However, it is noted that immersion objectives can be quite lossy. As  light passes twice through the objective (once for the laser  probe and once for the Raman return), the total loss scales as  the square of the single pass loss. Although we plan to  investigate the improved resolution of solid immersion  objectives, this paper only has results for air gap and oil  immersion type objectives.


2 Small amounts of laser heating are removed via computer  processing. Large amounts of heating can affect the device  operating conditions, so must be avoided.


IR Raman Temperature Measurements


Oraph Temperature


81.600


ec0eh30 Oemo


were encoreconnuting con su


S AXD


61.810


Figure 13: Backside IR Raman temperature data on hot spot  in silicon device for 6x6 array with 2 micron step size.


The system shown in Figure 12 was modified with a 1342 nm


Oraph Tomperature Data


laser and an InGaAs detector based spectrometer. Test device  used was the same device used for the IR thermal  measurements shown in Figures 1-4. A high-transmission and  high-NA IR objective with a magnification of 40X was used. Expected resolution is ~ 1 micron.


Figure 13 shows results from a 6x6 sample array taken in the  region of a device hot spot. Integration time was 1 second for


44,399


each sample point. The measured peak temperature rise is ~61K with an error of +/- 3K. This result is somewhat higher  than the 57K rise predicted by fitting the IR thermal data but  within the expected measurement and fit errors. It is possible  that this slightly higher value is due differences in vertical  sectioning (the Raman system having higher vertical


www.encoreconouing.com.au


ccCraph10 Demo


rejection). The width of the peak is seen to be in reasonable  agreement with the IR thermal prediction. Unfortunately, the  width of this source was not sufficiently narrow to fully


44.391


demonstrate the resolution of the Raman system.


We examined an alternate ‘hot spot’ contained within the  white square shown in Figure 14 using a 1.2 NA oil  immersion objective. The expected resolution of this objective  is ~ 0.55 micron. The Raman temperature data shown in  Figure 15 displays a narrow line corresponding to the location  of the dark gap seen within the white square. The step size for  this data was set at 0.5 micron. The appearance of the single  pixel width line in the Raman temperature data seems to  confirm the expected resolution.


Figure 14: Laser reflected light image of test chip at 200X  and 1.2 NA. White square indicates location of Raman scan.


Figure 15: Raman temperature data taken within the white  square shown in Figure 14. Step size is 0.5 micron. Note  narrow line running from top to bottom of graph.


Some addition results are shown in Figure 16 for a low  resolution scan of a device with multiple closely spaced  hotspots. The rather curious negative temperatures seen are  quite reproducible and give rise to speculation of a localized  Peltier effect.


Figure 16: Backside IR Raman temperature data on multiple  hot spots in silicon device for 6x6 array with 10 micron step  size. Note negative temperatures (orange blocks near center) that may be due to a localized Peltier effect.


We have shown that image resolution and temperature  measurement accuracy are closely coupled for temperature  sources with size scales of the order of the image resolution. A  backside IR Raman temperature measurement system has been  assembled to overcome these resolution limits and  measurement results have been demonstrated.


Additional tests are planned to further define the capabilities  of backside IR Raman temperature measurements in silicon. These tests will include building a sub-micron heat source  with known thermal properties to determine resolution limits  and the use of solid immersion objectives to improve those  limits.


The authors would like to acknowledge Andor for the loan of  their DU490A-1.7 InGaAs camera and SR-163 spectrometer, without which these measurements could not have been made. We would also like to acknowledge Winfield Scott of EAG  Labs who supplied the test device.


[1] G. C. Albright, et al., “True Temperature Measurements  on Microscopic Semiconductor Targets,” SPIE Vol. 3700 (1999), pp. 245-50.


[2] M. Kuball, et al., “Integrated Raman – IR Thermography  for Reliability and Performance Optimization, and Failure  Analysis of Electronic Devices,” ISTFA 2007, pp. 1-5.


[3] J. R. Ferraro, Introductory Raman Spectroscopy,Academic Press (San Diego, 2003).


[4] R. A. Falk, “Optimizing Backside Image Quality,” ISTFA  2002, pp. 155-61.


[5] S. Ippolito, "Polarized high-resolution imaging," Nature  Photonics 2 (2008), pp. 273-4


[6] Ramsay, E. et al. “Three-Dimensional Nanoscale  Subsurface Optical Imaging of Silicon Circuits” Appl. Phys. Lett. 90, (2007) pp. 131101


Nanoprobe Capacitance-Voltage Spectroscopy (NCVS) Localization of 32nm SOI  SRAM Array Failure


IBM Systems and Technology Group, Hopewell Junction, New York, USA


The technique of Nanoprobe Capacitance-Voltage  Spectroscopy (NCVS) at contact level (CA) for identfication  of  FEOL defects in MOSFET devices, especially for silicon  on insulator applications  has been extensively detailed [1].


The introduction of Nanoprobe Capacitance Voltage  Spectroscopy (NCVS) of discrete MOSFET and SOI  embedded dynamic ramdon access memory devices  (eDRAM) without the time consuming delayering methods of  conventional scanning capacitance microscopy have also been  highlighted [2].


This paper is intended to describe the advantages of NCVS to  localize defects in specific MOSFET devices at CA level as  well as to identify resistive BEOL via interconnections and  FEOL defective high k metal gate structures without the  attendant time consuming delayering steps employed with  classical SCM methods.


Localization of a FEOL defect in a discrete 32nm SOI  MOSFET device in SRAM array causing a vertical pair cell  failure signature will be discussed.


MOSFET devices are routinely measured at the probe pad  level with conventional capacitance-voltage (CV) measurement instruments.  Such measurements are done at the  front end of line (FEOL) and back end of line (BEOL) process  completion levels.  The CV data is used to monitor the process  and verify certain parametrics such as effective oxide  thickness (EOT), Tox,  gate drain overlap capacitance (Miller  capacitance), trapped charge, source-drain leakages, halo  implant oxide leakage, doping concentration, threshold  implant level and many others.  This type of testing is treated  at length in the classic text of Nichollian and Brews [4].


Employment of Nanoprobe Capacitance Voltage Spectroscopy (NCVS) to localize defects in discrete MOSFET devices or to  pinpoint resistive BEOL via interconnects with less than one  femto amp current sensitivity levels far outperform legacy  methods of passive/active voltage contrast employing  scanning electron microscopy (SEM) or focused ion beam (FIB) microscopy.


Typically, Vdd levels of less than 1.0 volt associated with high  density SRAM arrays and embedded DRAM memory in 45nm  and beyond technologies require current sensiivity levels of  less than one femto amp.


NCVS localization of a discrete NFET transfer device in a   SRAM cell causing a vertical pair failure will be detailed.


Background


Nanoprobe Capacitance-Voltage Spectroscopy (NCVS) employs a resonant sensor in combination with an an atomic  force prober tool.


Figure 1 details this reasonat sensor and the its output signal.


Figure 1.  NCVS sensor and electronics block diagram.  The  curves can be extracted in two places: the “SCM” (as dC/dV  vs. V) and the “Sensor Output” (as C vs V.  The Lock in  Amplifier provides significant noise reduction for imaging, at  the expense of  losing the absolute value of capacitance.


Figure 2: Nanoprobe Capacitance NCVS localization image  associated with flat band voltage shift in defective SRAM  NFET transfer device in array cell.  The contrast is not due to  a smaller capacitance signal but due to a shift in the effective  flat band voltage


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 73-75


Figure 3: SRAM cell layout corresponding to defective NFET  transfer device (circled) that NCVS localized in Figure 2.


NCVS localization of this 32nm SOI failure involved  identifying a discrete device where the substrate has a buried  oxide layer isolating the Rx active area from the underlying  silicon substrate and therefore has no contact to the backside  of the die.  Such defects are tricky to locate using other  methods, but in the capacitance image, the CV flatband shift  associated with this defective device is easily measured.  There is sufficient capacitive coupling through the barrier  oxide (BOX) to allow the contrast mechanism shown.  The  contrast mechanism is explained by the acquisition of AC  capacitance (dC/dV vs V) curves from the bright contact and  its neighbor.


The image in Figure 2 is taken using the standard method of  applying an AC bias to the sample and demodulating the  resulting sensor signal using a lock-in-amplifier, the data  actually represent the derivative of the CV curve.


Figure4: TEM cross sectional image of NFET transfer device  localized by NCVS shown in Figure 2.


TEM cross sectional imaging of defective NFET transfer  device localized by NCVS showed a CA contact via that RIE  processing extended past the silicide level.


A series impedance (represented by this anomaly) coupled  with the AC capacitance signal is consistent with the NCVS  image shown in Figure 2.


The impedance associated with this CA RIE ‘punch through” of the silicide level did not produce an anomalous DC IV  measurement.


|||。 3.0E-05|。 3.0E-05|。 3.0E-05|。 3.0E-05|。 3.0E-05|。 3.0E-05||||||

|||*★ **★**自 2.0E-05 1.0E-05|*★ **★**自 2.0E-05 1.0E-05|*★ **★**自 2.0E-05 1.0E-05|*★ **★**自 2.0E-05 1.0E-05|*★ **★**自 2.0E-05 1.0E-05|*★ **★**自 2.0E-05 1.0E-05|**★**4|||||

|||||******1 ********4|******1 ********4|******1 ********4|******1 ********4|******1 ********4|||||

||0|0.2|0.4|0.6|0.8|1|0.0E+00|0.2 0.4 0.6 0.8 1|||||

||va/v|va/v||||-1.0E-05 0 va/v|-1.0E-05 0 va/v||||||

||(b) ION ~40 μA |(b) ION ~40 μA |(b) ION ~40 μA |(b) ION ~40 μA |(b) ION ~40 μA |(b) ION ~40 μA |||||||

||7.0E-05 6.0E-05|7.0E-05 6.0E-05|7.0E-05 6.0E-05|7.0E-05 6.0E-05|7.0E-05 6.0E-05|7.0E-05 6.0E-05|||||||

||a S.0E-05 4.0E-05|a S.0E-05 4.0E-05|a S.0E-05 4.0E-05|a S.0E-05 4.0E-05|a S.0E-05 4.0E-05|a S.0E-05 4.0E-05|||||||

||3.0E-05|3.0E-05|3.0E-05|3.0E-05|3.0E-05|3.0E-05|||||||

||2.0E-05 1.0E-05|2.0E-05 1.0E-05|2.0E-05 1.0E-05|2.0E-05 1.0E-05|2.0E-05 1.0E-05|2.0E-05 1.0E-05|||||||

||0.0E+00|0.0E+00|0.0E+00|0.0E+00|0.0E+00|0.0E+00|||||||

||(a) ION ~105 μA |(a) ION ~105 μA |(a) ION ~105 μA |(a) ION ~105 μA |(a) ION ~105 μA |(a) ION ~105 μA |(c) ION ~85 μA |(c) ION ~85 μA |(c) ION ~85 μA ||||

||(a) ION ~105 μA |(a) ION ~105 μA |(a) ION ~105 μA |(a) ION ~105 μA |(a) ION ~105 μA |(a) ION ~105 μA |8.0E-05 7.0E-05|8.0E-05 7.0E-05|||||

||★点 2*******|★点 2*******|★点 2*******|★点 2*******|★点 2*******|★点 2*******|6.0E-05 5.0E-05|6.0E-05 5.0E-05|||||

||★点 2*******|★点 2*******|★点 2*******|★点 2*******|★点 2*******|★点 2*******|< 4.0E-05 。|< 4.0E-05 。|||||

||★点 2*******|★点 2*******|★点 2*******|★点 2*******|★点 2*******|★点 2*******|3.0E-05|3.0E-05|||||

||-0- **************4|-0- **************4|-0- **************4|-0- **************4|-0- **************4|-0- **************4|2.0E-05 1.0E-05 0.0E+00|2.0E-05 1.0E-05 0.0E+00|********** . . . . . . . . . . . .||||

||0||0.2 0.4|0.2 0.4|0.6|0.6|0.8 1|0.8 1||||0.2 0.4 0.6|

||||||Va/v|Va/v|-1.0E-05 0|-1.0E-05 0|-1.0E-05 0|Va/v||0.2 0.4 0.6|

|PD2 Sourcesweep ||(b) |ION ~105 |ION ~105 |μA |μA |||(d) ION ~85 μA |(d) ION ~85 μA |(d) ION ~85 μA ||

||||||||||9.0E-05|9.0E-05|||

||||||||||8.0E-05|8.0E-05|||

||||||||||7.0E-05|7.0E-05|||

|||||||||6.0E-05 5.0E-05|6.0E-05 5.0E-05||||

|||||||||< 4.0E-05|< 4.0E-05||||

|||||||*********4|*********4|3.0E-05 2.0E-05|3.0E-05 2.0E-05|* * * *|||

||||||||0.8|0.8|1.0E-05|1.0E-05|. . . . . . . . . . . . 1||

||0|||0.2 0.4|0.2 0.4|0.6|0.6|0.8|0.0E+00 -1.0E-05 0|0.0E+00 -1.0E-05 0||8 0.2|

||||||v.Iv|v.Iv||||||v/v|

||||||||||||||

3.0E-05


2.5E-05


-*-Vg=1.0V


2.0E-05


---Vg=0.8V---Vg=0.6V


PI


--Vg=0.4V


5.0E-06


--Vg=0.2V--Vg=0V


-5.0E-06


1.0E-05


/V1.5E-05


Sourcesweep


4.5E-05


4.0E-05


3.5E-05


---Vg=0.8V


---Vg=0.6V


/i2.0E-05


--Vg=0.2V


1.5E-05


V


-→-Vg=OV


v./v


-5.0E-06 00.20.40.60.8


-1.0E-05 00.20.40.60.8


(d) ION ~85 μA


v./V


Figure 3: I-V characteristics of bad and good PD1 obtained by sweeping the drain (Drainsweep) and source (Sourcesweep).


Drainsweep


1.0E-04


8.0E-05


---Vg=0.6Vt


2.0E-OS


---Vg=0.2V


-→-Vg=0V


6.0E-05


1.2E-04


-2.0E-05


女


--Vg=0.4V---Vg=0.2V--Vg=OV


Figure 4: I-V characteristics of bad and good PD2 obtained by sweeping the drain (Drainsweep) and source (Sources


n-contact A


Unexposed poly beneath the oxide


CAREC B


Bright


TEM2X71000


Figure 5: (a) TEM cross-sectional cut direction along the  source and drain contacts of the PD1.  (b) TEM micrograph  showing abnormal NiSi under source contact.


B.  Hard-Fail Defect Caused by Abnormal NiSi Formation  Leading to Contact-Poly Short


02


The next case study involved a hard-fail defect which was  identified easily by the SEM PVC technique. Figure 6 shows  the SEM micrograph of the fail bit at contact level showing a  bright n-contact. This led to the conclusion that the hard-fail  could be due to a failed PG or PD transistor.


(a) G


Failbit


44.2mm


60.7nm


Figure 6: SEM micrograph showing a bright n-contact at the  fail bit using SEM PVC technique.  This led to the conclusion


08-19717Qingsiao/Wee Ming200 kv


that the hard-fail was due to a failing PG or PD transistor.


Because the I-V characteristics of the PG transistors in both  the bad and good SRAM cells were similar, it can be  concluded that the hard fail was caused by the failed PD. The  I-V characteristics of good PD and bad PD transistors were  compiled in Figure 7.


Measurement


||Bad PD transistor |Bad PD transistor |Bad PD transistor |Bad PD transistor |Bad PD transistor |Good PD transistor |Good PD transistor |
|---|---|---|---|---|---|---|---|

|Drainsweep |(a) |(a) |(a) |(a) |(a) |(c) |(c) |

||(a) |(a) |(a) |(a) |(a) |1.40E-04||

||(a) |(a) |(a) |(a) |(a) |1.20E-04 1.00E-04 8.00E-05 V||

||*******|*******|*******|*******|*******|1.20E-04 1.00E-04 8.00E-05 V||

||*******|*******|*******|*******|*******|1.20E-04 1.00E-04 8.00E-05 V|/ 6.00E-05|

||*******|*******|*******|*******|*******|1.20E-04 1.00E-04 8.00E-05 V|00000|

||*******|*******|*******|*******|*******||00000|

||||||2.00E-05|||

|||Va/v|Va/v|Va/v|Va/v|0.00E+00 -2.00E-05|**.....*...**************** 0 0.2 0.4 0.6 0.8 1 1.2 1.4|

|Sourcesweep |(b) |(d) |(d) |(d) |(d) |(d) |(d) |

|||||||||

||||||***************|***************|***************|

||0.2|0.4|0.6|0.6|0.8 1 1.2|0.8 1 1.2|0.8 1 1.2|

||0|0.2|0.4|0.6|0.8|1|1.2|

||v/v|v/v||||||

2.00E-04


→-Vg=1.4V


1.50E-04


--Vg=1.2V-Vg=1.0V--Vg=0.8V


V5.00E-05


-Vg=0.6V


P


→Vg=0.4V


0.00E+00


-5.00E-05


--Vg=0V


-1.00E-04-1.50E-04


1.00E-04


2.00E-05


--Vg=1.4V


1.00E-05


-■-Vg=1.2V---Vg=1.0V


0.00E+00--Vg=0.8V<-1.00E-05---Vg=0.6V>-2.00E-05--Vg=0.2V


-3.00E-05


-4.00E-05


1.4


---Vg=0.4V


Figure 7: I-V characteristics of bad and good PDs


The abnormal I-V characteristic of the bad PD transistor was  further investigated by performing a two-point electrical test  between the bright contact A and CAREC B as labeled in  Figure 6.  Figure 8 shows high current leakage between these  two contacts.


-1.2E-04


V/V


Figure 8: I-V characteristic of bright n-contact A and CAREC  B showing high leakage at failed bit.


The high leakage I-V characteristic led to the hypothesis that  the unexposed poly beneath the oxide had physically formed  an electrical short to the bright contact A.  A TEM cut was  proposed and the cross-section of the bad PD transistor is  shown in Figure 9.  A poly contact short can be seen in Figure  9(a).  A dark field image shown in Figure 9(b) further


confirms the existence of what may be a NiSi piping fail.  Further examination of the material was done using Energy  Dispersive X-ray (EDX).  The EDX micrograph is shown in  Figure 10.  Peaks can be seen corresponding to a NiSi piping  artifact. It is clear that NiSi piping caused the poly-contact  short, leading to a high leakage issue and causing the hard1.2E-04


fail.


-CAREC B


品


→-Bright n-contact A


V/


2.0E-20.


-1.4-1.2-1-0.8-0.6.04-0.200.2 0.4 0.6 0.8 1 1.2 1.4-4.0E-05


-8.0E-05


Figure 9: NiSi piping causing poly-contact short: (a) SEM  micrograph of the cross-section of the PD transistor; (b) Dark  field image of the cross-section;


Energy (arV)


Energy uk


(c)


Figure 10.  EDX Analysis confirming the presence of NiSi


C.  Isolation of Resistive Contact in a Large Electrical Test (ET) Structure


The last case study pertains to a large Electrical Test (ET) structure that spans 25 μm by 25 μm as shown in Figure 11.


Figure 11: (a) SEM micrograph showing a 25μm by 25 μm  ET structure.  There are a total of 50 columns with 100  CARECs at each column; (b) ET structure layout


HAADf Detector


There were a total of 50 columns with 100 CARECs along  each column, and one of the CARECs in this ET structure was  open or resistive. It would be extremely difficult and timeconsuming to isolate this defective CAREC by the SEM PVC  technique.


营


名


An iterative nanoprobing technique was employed to identify


onco


counts8


the resistive CAREC. Two probes (P1 and P2) were first


co10


-2-


landed at column 1 and column 25 and the I-V curve obtained


,BNBBAO NUa


8) HB(


(Figure 12(a)). Since the I-V curve shows ohmic behavior, the  resistive contact could have been anywhere along column 25


"


lshd


EOKHDF Dtr PUmE 4


to 50. To confirm this hypothesis, one probe was landed at  column 25 and the other at column 50 (Figure 12(b)). The


Counts


更


Counts名


non-ohmic characteristic confirmed that the resistive CAREC


1o


NG


was somewhere along column 25 to 50. This method was


repeated by eliminating half of the number of columns each  time. After multiple iterations it was identified that the  resistive CAREC was along column 26 (Figure 12(c)).


The iterative nanoprobing technique was then employed along  column 26 in a similar manner that was used for the entire  structure.  A probe was landed at one end of the column and a  second probe was landed in the middle of the column.  Again, half of the column was eliminated at a time to identify which  of the 100 CARECs was the resistive one.  It can be seen that  there is a partial open between CAREC 65 and 66 in Figure  12(d).  Further characterization between CAREC 66 and 67, shown in Figure 12(e), shows ohmic behavior and thus a good  contact.  It was concluded that CAREC 66 was electrically  open and the TEM cross-section micrograph in Figure 13  confirmed this finding. Nanoprobing greatly helped to reduce  the time needed in identifying the resistive CAREC in a large


25 μm


ET structure and improve turnaround.


勿


(b) D=mI=hndE


694


hadI'haundInITIIPboed--一-/mII-=====--一C11Ihim1一入、


2!11v=11thound1Ihaual'III=....91=I==joug=，-7-=jong=。=1"


1二二"Illham


ngI一


1""


三


|08-14289|Gek Li/CM|200kv|
|---|---|---|

|TEM2|X19500 1.0日||

-□"一JN-二工二


200 nm


一产1-


TI


TS1翔


mg--u


题)


23


国


1、年0


I"


72s3D0DO0


□-


1I


lunlI-山=F===. .====1-三-0三"一--一一"


IP4D


二


IE


n"


-N


月月


3111


Iuul=hulll-unll11


unl


II-=H=t


11unlullI..Il


Figure 13: TEM micrograph showing the cross-section of  physically unlanded CAREC 66


||(a) Column 1-25: Ohmic |(a) Column 1-25: Ohmic |(a) Column 1-25: Ohmic |(a) Column 1-25: Ohmic |(a) Column 1-25: Ohmic |(d) |Column 25 CAREC 65-66: Partially Open |Column 25 CAREC 65-66: Partially Open |Column 25 CAREC 65-66: Partially Open |Column 25 CAREC 65-66: Partially Open |Column 25 CAREC 65-66: Partially Open |Column 25 CAREC 65-66: Partially Open |Column 25 CAREC 65-66: Partially Open |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|

||0.0E+00|0.0E+00|-1 -0.8 -0.6 -0.4|-0.2 0||4.0E-06||2.0E-06||||||

||-5.0E-07|||3.5E-06||0.0E+00|-1|-0.8|-0.6|-0.4|-0.2|0|8.0E-06|

||-1.0E-06|||||0.0E+00|-1|-0.8|-0.6|-0.4|-0.2|0|8.0E-06|

||V|V|||||||V|V -2.0E-06|V -2.0E-06|V -2.0E-06||

||/|/|-1.5E-06|-1.5E-06|||2.5E-06|/|/ /|/ /|/ /|/ /|/ /|

||+ u|+ u|||||||子 u|子 u|子 u|子 u|子 u|

||||||u|||||||||

||0|0|-2.0E-06|-2.0E-06|||2.0E-06|8 1 n|a -4.0E-06 4.0E-06 d n|a -4.0E-06 4.0E-06 d n|a -4.0E-06 4.0E-06 d n|a -4.0E-06 4.0E-06 d n|a -4.0E-06 4.0E-06 d n|

||n 3|n 3||||||口|3|3||||

||T|T|-2.5E-06|-2.5E-06|||1.5E-06|乙 d|I|I||||

||d|d|-3.0E-06|-3.0E-06|||1.0E-06||d|d|-6.0E-06|-6.0E-06|-6.0E-06|

||d|d|-3.0E-06|-3.0E-06|||1.0E-06||||-8.0E-06|-8.0E-06|-8.0E-06|

||||-3.5E-06|-3.5E-06|||5.0E-07||||-1.0E-05|-1.0E-05|-1.0E-05|

|||0.0E+00|0.0E+00|0.0E+00||Voltage /V|Voltage /V|Voltage /V|Voltage /V|Voltage /V|Voltage /V|Voltage /V|Voltage /V|

||||Column 25-50: Non-ohmic (e) Column 25 CAREC 66-67: Ohmic |Column 25-50: Non-ohmic (e) Column 25 CAREC 66-67: Ohmic |Column 25-50: Non-ohmic (e) Column 25 CAREC 66-67: Ohmic |Column 25-50: Non-ohmic (e) Column 25 CAREC 66-67: Ohmic |Column 25-50: Non-ohmic (e) Column 25 CAREC 66-67: Ohmic |Column 25-50: Non-ohmic (e) Column 25 CAREC 66-67: Ohmic |Column 25-50: Non-ohmic (e) Column 25 CAREC 66-67: Ohmic |Column 25-50: Non-ohmic (e) Column 25 CAREC 66-67: Ohmic |Column 25-50: Non-ohmic (e) Column 25 CAREC 66-67: Ohmic |Column 25-50: Non-ohmic (e) Column 25 CAREC 66-67: Ohmic |Column 25-50: Non-ohmic (e) Column 25 CAREC 66-67: Ohmic |

||||5.0E-07 -1.0E-05|5.0E-07 -1.0E-05|5.0E-07 -1.0E-05|5.0E-07 -1.0E-05|5.0E-07 -1.0E-05|5.0E-07 -1.0E-05|-1 -0.8 -0.6 -0.4 -0.2 0|-1 -0.8 -0.6 -0.4 -0.2 0|-1 -0.8 -0.6 -0.4 -0.2 0|-1 -0.8 -0.6 -0.4 -0.2 0|-1 -0.8 -0.6 -0.4 -0.2 0|

||||4.0E-07 V / V -2.0E-05|4.0E-07 V / V -2.0E-05|4.0E-07 V / V -2.0E-05|4.0E-07 V / V -2.0E-05|4.0E-07 V / V -2.0E-05|4.0E-07 V / V -2.0E-05||||||

|||||||U /|U /|U /|U /|U /||||

||||3.0E-07 」||U|U|U|||||||

|n||8|8|-3.0E-05|-3.0E-05||||||||8|

|0||1|1|||||||||3.0E-05|1|

||||||||n|n||||||

||||||||n|n|||2|0|0|

||2.0E-07|2.0E-07|2.0E-07|d|I|I||||||||

||||d -4.0E-05|d -4.0E-05|d -4.0E-05|d -4.0E-05|d -4.0E-05|||||||

[3] Randal Mulder, Sam Subramanian, Tony Chrastecky, “Atomic Force Probe Analysis of Non-Visible Defects in  Sub-100nm CMOS Technologies” ISTFA 2006: Proceedings of the 32nd International Symposium for  Testing and Failure Analysis, pp. 503-511, November 12-16, 2006, Renaissance Austin Hotel, Austin, Texas, USA.


[4] Gunnar Zimmermann, Stefan Mueller   90nm  technology SRAM soft fail analysis using nanoprobing  and junction stain TEM 32nd International Symposium  for Testing and Failure Analysis, pp. 512-516, November  12-16, 2006, Renaissance Austin Hotel, Austin, Texas, USA.


[5] Peter Egger, Stefan Muller, Martin Stiftinger, “A New  Approach for SRAM Soft Defect Root Cause  Identification” ISTFA 2007:Proceedings of the 33rd  International Symposium for Testing and Failure Analysis, pp.214-218, November 4-8, 2007, McEnery Convention  Center, San José, California, USA.


[6] Randal Mulder, Sam Subramanian, Tony Chrastecky, “Low Voltage, Low Current AFP Characterization of NonVisible Soft Transistor Defects” ISTFA 2008: Proceeding  from the 34th International Symposium for Testing and  Failure Analysis.pp.417-422, November 2-6, 2008, Portland, Oregon USA.


FAMOS Fail Bit Verification /Characterization Via NanoProbe


Mark Dexter


Texas Instruments, Inc. Dallas, TX  m-dexter1@ti.com 972-995-1945


Richard Stallcup II


Zyvex Corp., Richardson, TX


rstallcup@zyvex.com 972-235-7881


Sarma Gunturi


Texas Instruments, Inc. Dallas, TX  s-gunturi@ti.com 972-995-1067


The nanoprobe technique has been widely adapted to many  circuit analyses from 6T SRAM bitcells to analog circuit  failure analysis. But among the applications widely reported, little has focused on the flash bitcell analysis. This is not so  surprising when one considers many flash cells consist of a 1T  storage cell. Physical failure analysis can proceed immediately  once the failing device has been unambiguously identified. This approach is generally effective for imaging defects and  determining root cause failure identification.


This paper presents the more unusual case where fail device  isolation is insufficient to determining the defect and/or the  root cause. In this case, we have established the nanoprobe  technique to understand the electrical signature of a customer  return 1T flash bit fail. This understanding supported  screening development to avoid test escapes.


The flash bitcell consists of a single floating gate transistor. This bit configuration uses a poly control gate (CG) separated  by an interpoly dielectric (IPD). The floating gate (FG) poly  acts as the storage medium. Program or charging of the cell  consists of injecting charge through a tunnel oxide by hot  carrier injection. These charges increase the threshold voltage  of the device and cause the cell to have a very low  conductivity compared to a reference cell.


Discharge or Erase of the cell forces charge off the floating  gate (FG) through the tunnel oxide. This causes threshold  voltage to fall, with a correspondingly high conductivity in  comparison to the reference cell. See Fig[1a] and [1b].


External connections are identical to those of a conventional  MOS transistor with drain (d), gate (g), source (s) and bulk (b) connections. The voltages used differ significantly from  typical ranges used at a similar technology due to the differing  mechanisms deployed. In characterizing these cells, dc  operation was initially verified. Specifically, we verified that


each cell could be programmed, erased and read normally. Additional I-V characteristics were also gathered for  comparison.


Contrasting these characteristics with those of traditional  MOS, we must be mindful of the fact that I-V are given in  terms of ‘apparent’ rather than actual Vgs. The actual  threshold voltage (Vt) would be given in terms of the floating  gate voltage. Floating gate bias is unknown, being determined  by a number of components including interface charges, coupling coefficients, capacitances, etc.


IPD


CG


FG


Tunnel Ox


Fig [1a]: TEM cross-section of the floating gate transistor


CG  FG


_  _  _  _  _  _  _  _


Erased


Pro


5


grammed


Fig [1b]: Erased versus programmed floating gate MOS  device. The Nch erased cell has minimal or know excess  charge on the floating gate (lot Vt state). The programmed


Cell has had charged injected onto the floating gate.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 93-96


203-0 993-9


Fig [1c]: Flash Bitcell Probing at Contact


A. Measuring Floating Gate bitcell characteristics


Initially, the fail and reference devices were compared against  the expected DC characteristics of the FG MOS devices.


The dc programming curves of passing and failing devices are  shown in 2a.


120E-6


100E-6


80E-6


60E-6


◆-Pass'---Fail


40E-6


yt


20E-6


00DE+0春


612345


Fig [2a]: DC programming curve of passing and failing  floating gate bitcell. Few differences were observed, with both  showing similar peak currents and injection voltages.


50.0E·6


45.CE-6


40.CE-6


025.0E-6


上了


C20.CE-6


15.CE-6


10.CE-6


5.CE-6


0DS


1.5225


00.0E+0*


Dran Vohage


Fig [2b]: Passing cell Id-Vd family of curves.


303-9


1539


F03-9


553-9


3203-9


TS3-9


T02-9


009


TS225


0003+0


Dran votage


Fig [2c]: Failing bitcell Id-Vd family of curves.


The passing cell’s family of curves (Id-Vd sweeps at various  CG voltages) is shown in Fig [2b]. The corresponding failing  cell’s family of curves is shown in Fig [2c].  The failing bitcell  was observed to be much weaker in comparison to the  reference cells. The drain current versus control gate sweep in  Fig [3] shows a large post-erase threshold voltage offset  between passing and failing devices. Several passing cells  showed a center around 2V with a maximum threshold  voltage spread of ~ 300mV. Clearly the failing unit is not  erasing as easily as the reference cells.


The difference does not explain the fail, however. The cell is  still read as being logically ON, i.e., erased.


7E-5


6E-5


56-6


46-5


3E


-d


Drain Qurre


dell


28-5


1E-6


COOE+O


0123456 Gate Votage


Fig [3]: Linear control gate (Vcg) sweep comparing failing  and reference bits. Post erase threshold voltage shows a  significantly higher net charge remaining on the failing  bitcell.


35.0E-0


830.CE-6


B. Understanding the fail  1) Customer Fail Mode


The customer return unit fail mode was post erase data gain. This means that the threshold voltage of the failing bit tended  to rise over some soak time. During the soak, the cell bias  conditions were fixed at levels consistent with a READ. The  observed voltage shift is consistent with charge injection onto  the floating gate, hence the term “data gain”.


The customer observed failure was confirmed upon retesting  of the unit under similar bias conditions.


Programming curves of all cells showed similar injection  points as shown in Fig [2a]. So there was no significant  difference in the drain side doping or tunnel oxide.


2) Soft Programming


No obvious differences between the bitcells were revealed in  the full dc programming curve. But since the fail mode was  determined to be a charge gain phenomenon, we decided to  examine the program characteristics more closely.


The so called soft programming sequence was targeted to  identify differences under bias conditions which are below  nominal. For this device, the nominal control gate to drain  bias during the program operation is ~4.5V, while the drain to  source bias is also about 4V. By reducing the lateral field, we  are providing fewer hot carriers for injection into the floating  gate, thus reducing programming efficiency.


||Pre-WLStress Const. Current |Pst-WLStress Vt (VTCC) [V] |
|---|---|---|

|Ref1 |1.80 |2.80 |

|Ref2 |1.75 |5.60 |

The injection point observed in the programming curves is  used as a reference for our drain bias. Drain bias (Vdrain) is  set 400mV below the experimentally determined injection  point (Vd = Vinj – 400mV). The control gate is then swept  and followed by a program verify. The target device is then  erased. The sequence is repeated using a slightly higher drain  voltage. Fig [4a] and [4b] show examples of the program  verify curves for a failing versus reference bit.


16 5-05


14 E-06


12 E-06


Reference Fail


10 E-06


C E-O6


a6 E-0B


*E-00


2 E-06


000 E+00


6vgs(v)8101214


Fig [4a]: Fail versus reference program verify curves. These  shifts were observed after a soft programming sequence. Both  the failing and an adjacent cell showed significantly higher  threshold voltage versus the reference cells.


In this paper, we documented an example of using the  nanoprobe methodology to understand a flash customer return. Unlike 6T or 8T SRAM bitcells, the failing transistor could be  identified immediately.  But numerous PFA efforts failed to  give sufficient understanding of the failure.


By using nanoprobe DC bit characterization, we were able to  determine that data gain failures were due to thin or


10E-6


9E-6-→-Fail 8E-6


---Reference1


Reference2


7E-6  36E-6


5E-6  C4E-6 3E-6


2E-6


★


00CE+0<


024681012 Gate Voltage


Fig [4b,c]: Fail versus reference cell program verify curves. These shifts were observed after a soft programming  sequence. The failing unit exhibited a significantly higher soft  program shift. The table summarizes pre and pst stress  constant current threshold voltage (VTCC).


compromised IPD (interpoly dielectric). This characterization  approach gave the necessary screen condition to eliminate test  escapes. The resulting single pulse program test successfully  identified die on the wafer which contained these very fast  programming bits. These were most like to become data gain  bits at the customer.


The author would like to thank the fab Physical Failure  Analysis group for their assistance on images.


[1] W. D. Brown and J. E. Brewer, “Nonvolatile  Semiconductor Technology,” Chapter 1, Basics of  Nonvolatile Semiconductor Devices, IEEE Inc., New  York, NY, 1997.


[2] Ibid., Chapter 2, Floating Gate Planar Devices, IEEE  Inc., New York, NY, 1997.


[3] Larry Liu, et. Al., “Combination of SCM/SSRM analysis  and Nanoprobing technique for soft single bit failure  analysis”, Texas Instruments, 30th ISTFA, 2004, pp. 38-41.


[4] Cha-Ming Shen, et.al., “Combine Nano-probing  technique with difference analysis to identify non-visual  failures,” TSMC, 32nd ISTFA, 2006, pp. 264 -267.


Fail


2.35


8.60


Contact author information: Mark Dexter


Texas Instruments, Inc.


MS  385


13020 TI Boulevard


Dallas, TX  75243


m-dexter1@ti.com


972-995-1945 Tel


972-877-2487 Mobile


972-927-1118 FAX


Methodologies for Quantifying FIB “Milling Acuity”


FEI Company, Hillsboro, Oregon, USA  chad.rue@fei.com


FIB column performance can be difficult to evaluate, and the  traditional metrics of imaging resolution and minimum spot  size give little indication of how a FIB system will perform its  intended daily tasks.  A series of supplemental FIB  performance tests is proposed to quantify “milling acuity” under real-world conditions.  A quantitative measuring  scheme for evaluating the quality of High Aspect Ratio (HAR) vias is proposed, and an example is shown in which  the HAR measuring scheme can be used for process  development.


Focused Ion Beam (FIB) tools are ubiquitous in Failure  Analysis (FA) and Circuit Edit (CE) labs throughout the  semiconductor industry.[1,2]  A wide variety of commercial  systems are available, and FIB users face a difficult task in  evaluating the performance of one system relative to another. FIB manufacturers typically specify ion column performance  in terms of imaging resolution or minimum spot size.[3]  From a user’s point-of-view, there are two problems with  these metrics.  First, the procedures (and even the definitions) of spot size and resolution may vary from manufacturer to  manufacturer, and users are not typically given any details  about how these numbers are derived.  This makes objective  comparisons between columns very difficult.


More importantly, imaging resolution and minimum spot size  measurements are always performed under ideal conditions: lowest possible vacuum base pressure, smallest possible beam  current, and a sample specifically chosen to provide optimal  results.  By contrast, “real world” conditions are dramatically  different: significant background gas pressure (for etching and  deposition, or even after a recent load cycle), larger beam  currents, and a wide variety of sample types.  These sets of  conditions are dramatically different, and resolution and  minimum spot size probably tell us little about how a FIB  system will perform its intended daily tasks.


The objective of this work is not to suggest that we  completely abandon imaging resolution and spot size tests.  They are still generally useful as indicators of theoretical  performance limits.  Rather, our goal is to propose


supplemental FIB column performance tests that provide  information about “milling acuity” under useful operating  conditions.  Ultimately, such tests would be beneficial to both  users and manufacturers.


What’s wrong with the current metrics?


Imaging resolution


Imaging resolution measurements are often performed by  imaging a sample with fine structure (such as graphite, goldon-carbon, or a “knife-edge”), and then digitally evaluating  the image to measure edge widths (that is, the minimum  number of pixels required to transition from dark to bright as  the beam scans over a small feature).  This is assumed to  represent the minimum feature size that can be observed with  a particular beam size.  There are several limitations to this  approach.  First, the definitions of “dark” and “bright” can  vary.  Different definitions will result in different edge widths  and therefore different resolution results.  Another limitation  of using this technique for FIB systems is that the ion beam  erodes the sample as it images, and features can be “smoothed-out” by the act of imaging, adversely affecting the  measured edge width.  Finally, the size of the sample features  themselves convolute the measurement.  For example, if a  feature size is larger than the probe size the transition from  dark to bright associated with that feature will not be an  accurate measure of the resolution limit.  For this reason, some analysts plot a distribution of numerous edge-width  measurements and extract the resolution from the lower-end  of the distribution.  Obviously it is difficult to know where to  draw a meaningful cut-off.  What part of the distribution is  due to legitimate experimental variations in the measured edge  widths, and what is due to different feature sizes on the  sample?  Some more sophisticated resolution analysis  techniques use Fourier methods to examine the data in  frequency space.[4]  However, at some point the same  problem arises, and a cut-off frequency must be chosen that  effectively throws our the remainder of the data.


Minimum spot size


The first and most obvious problem with estimating “spot  size” is that ion beams do not have well-defined edges, but  rather a smooth spatial distribution.  Therefore, all spot-size  estimates are derived from arbitrarily chosen boundaries along


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 97-105


this intensity distribution (which is not necessarily Gaussian).  Additionally, as noted in the Introduction section, manufacturers always perform spot size measurements under  the most favorable conditions possible, and these conditions  can be very different from those faced by users on a daily  basis.  Clearly a more “real-world” metric would be a helpful  supplement to users.


All of this leads to the obvious questions: What column  performance specifications are the most meaningful?  What  tests can be performed to measure them?


A New Metric: “Milling Acuity”


“Milling acuity,” or milling sharpness, is arguably more  critical to advanced CE than pure imaging resolution (although that is important, too).  This work concentrates  exclusively on defining milling acuity and proposes tests for  measuring it.  Ideally, these tests should conform to the  following four criteria:


1. Tests should be well-defined, such that they can be  performed on any FIB system by a competent user.


2. Tests should result in unambiguous, quantifiable  results.


3. Test procedure and evaluation methods should be  accepted by a consensus of FIB users.


4. Tests should probe column performance under useful (typical) operating conditions.


We acknowledge that many different performance criteria, definitions, and tests are possible.  What follows is merely a  starting point to initiate a dialogue between users and  manufacturers on the topic.  We encourage FIB users to share  their ideas and opinions.


Possible Tests of “Milling Acuity”


Line burns


Line burns on “chrome-on-glass” samples have been a staple  of column performance testing for many years.  To perform  this test, the user mills a one-dimensional line pattern (or  commonly, a cross with intersecting horizontal and vertical  lines) on an appropriate sample, and then measures the width  of the resulting features created by the FIB.  The sample  usually consists of a thin, grounded, blanket metal film (often  chromium) on an insulating substrate (often glass).  When the  ion beam penetrates the surface film, the underlying insulator  is exposed.  This creates a noticeable contrast between the  grounded surface film and the floating substrate which  facilitates subsequent width measurements.


Obviously, the duration of the line mill will affect the width of  the features created by the FIB.  Shorter mills will produce  narrower feature widths, and longer mills will result in wider  feature widths.  To remove this ambiguity, users typically  perform a series of mills with different “doses” to determine


the minimum amount of beam exposure required to break  through the metal coating.  “Dose” is a common measure of  the total number of ions delivered to the sample, and thus is  relatively independent of the total beam current.  Thus, even  though larger beam currents deliver more dose per unit time, the dose required to penetrate the metal film should be similar  for all beam currents (for purely sputtering processes, that is.  Gas-assisted processes do not necessarily follow this  generalization due to gas-depletion effects at large beam  currents).  It is also possible to determine the break-through in  terms of the number of raster passes.  In this case, we expect  that smaller beams will require more raster passes to break  through the metal film than large beams (because they deliver  less dose to the sample per raster pass).  Regardless of  whether dose or number of raster passes is used, however, the  minimum amount of beam exposure required to break-through  the metal film is considered the standard that is used for  measurement purposes.


As FIB currents have trended lower, feature widths have  become very small, and it is sometimes difficult to judge the  exact moment of breakthrough.[5]  Additionally, the effect of  gas pressure is typically ignored.  However, with slight  modifications the traditional chrome-on-glass experiment can  satisfy the test criteria described above, and can be very  informative.


Voltage contrast-based endpointing for line burns.  One  simple and unambiguous method for determining the exact  moment of breakthrough on the surface metal coating is to use  a modified pattern that results in voltage contrast at the  moment of breakthrough.  Instead of a simple cross consisting  of intersecting vertical and horizontal lines, we used a pattern  resembling a “tic-tac-toe” grid.  When the ion beam has  completely milled through the metal coating, the central  region inside the grid becomes electrically isolated from the  remainder of the grounded surface film and appears dark in a  FIB image.  This is illustrated in Figure 1.


This test can be made even more informative if it is performed  at various gas pressures.  In our experiments we inserted the  XeF2 gas nozzle and repeated the above experiment under a  range of different operating pressures and beam currents.  Each time the conditions were adjusted, a series of test burns  using the tic-tac-toe grid was performed to determine the dose  threshold for breakthrough.  Illustrative results are shown  below in Figure 2.


3:32:02 PM3 μs30.00kV 16.5mm5.50 μmV400 ACE 6/14/2009dwellHVWDHFW


Feature Width (nm)昆台台合


-93 pA


量


-■-28pA


Figure 1.  A series of line burn test patterns, milled for


-9.7pA


different amounts of time.  The number next to each pattern


represents the number of raster passes that were performed


0.0E+001.0E-052.0E-053.0E-054.0E-05


for each pattern.  The mill penetrated the thin, grounded


XeF2 Pressure (Torr)


surface film after approximately 12,000 passes (pattern in the  upper-right hand corner of the image), as indicated by the  voltage contrast in the center of the pattern.


Figure 2.  Voltage contrast thresholds (expressed as the  number of raster scans to penetrate the surface film) as a  function of XeF2 gas pressures.  Note that more rasters are  required to penetrate the metal film when higher gas  pressures are used.  This suggests a loss of milling acuity due  to gas scattering.


XeF2 was chosen as the background gas, because it is a  commonly-used etchant during normal FIB operation.[6]  XeF2 does not enhance removal of the chromium film, but can  cause gas-scattering that broadens the gallium beam profile  and reduces “milling acuity.”  It is appropriate to evaluate this  gas-scattering effect, because it is a real-world phenomenon  that affects all FIB systems during normal gas-assisted


operation.  The broadening effect due to gas-scattering is  evident in both Figures 2 and 3.  Figure 2 illustrates that more  raster passes are required to break through the chromium film


#井


七#井井##井


45 50


Line Burn Widths at First VC


as the XeF2 pressure increases.  This is consistent with


broadening due to gas scattering, which shifts beam intensity  from the center of the distribution to the tails.  In Figure 3, we  observe a corresponding increase in the measured feature  widths at higher pressures.


Figure 3.  Measured feature widths as a function of XeF2 gas  pressure.


Feature widths derived from experiments such as these are


VC Thresholds


one possible way to express “milling acuity.”  From a FIB


||||-93pA ---28 pA||
|---|---|---|---|---|

||||★ 9.7 pA||

||县||||

|0.0E+00 1.0E-05 2.0E-05 3.0E-05 4.0E-05 XeF2 Pressure (Torr)|0.0E+00 1.0E-05 2.0E-05 3.0E-05 4.0E-05 XeF2 Pressure (Torr)|0.0E+00 1.0E-05 2.0E-05 3.0E-05 4.0E-05 XeF2 Pressure (Torr)|0.0E+00 1.0E-05 2.0E-05 3.0E-05 4.0E-05 XeF2 Pressure (Torr)|0.0E+00 1.0E-05 2.0E-05 3.0E-05 4.0E-05 XeF2 Pressure (Torr)|

60000


user’s point of view, these trends in mill feature-width as a


50000


function of pressure should be more useful and informative  than a single-point resolution measurement performed under


40000


idealized conditions.


30000


Note that the purpose of the above experiment was to illustrate


20000


a methodology for evaluating the impact of gas pressure on  milling acuity.  The data are not intended as a performance


benchmark for any particular ion column.


CrPasses to break thru


Minimum printable feature size. A similar experiment can  also be performed on chrome-on-glass samples: determining  the “minimum printable feature size” for various gas  pressures.  In this experiment, a series of repair patterns are  created.  Each repair pattern has the same X pixel spacing, but  the Y pixel spacings vary to cover a large range of values, as  suggested by Figure 4.


At small Y pixel spacings, all of the chromium within the  repair zone is evenly sputtered away, as it would be in a  normal milling operation.  At very large Y pixel spacings, horizontal rows of un-milled chromium are left behind.  At  some critical intermediate Y pixel spacing, defined as the  minimum printable feature size, unbroken rows of chromium  appear for the first time in the series.  An example of this kind  of experiment is shown below in Figure 5.


Figure 4.  “Minimum printable feature size” can be  determined by milling a series of repair patterns with  gradually increasing Y pixel spacing on a chrome-on-glass  sample.  Note that the pattern in the middle is the first pattern  in the series that exhibits continuous horizontal lines.


Figure 5.  Three series of mills with gradually increasing Y  pixel spacing.  The gas pressure used for each series is  indicated on the left side of the image. The first mill in each  series with continuous chromium lines (highlighted in purple) corresponds to the minimum printable feature size as defined  above.


Within each series in Figure 5, the minimum printable feature  size is indicated by the purple outline.  Note that the minimum  printable feature size increases as the gas pressure increases.  This trend is described quantitatively in Figure 6.


This experiment is particularly convenient, because it is not  necessary to load the sample into a SEM and make  measurements of the line widths.  Instead, the user can simply  note the first appearance of the chromium lines in the FIB  image, and the minimum printable feature size can be  determined from the known Y pixel spacings of the repair


patterns.  Additionally, the series of repair patterns can be  saved as a template and used in later experiments.


Pressure (Torr)


Figure 6.  Minimum printable feature size at different gas  pressures.


8e-7 Torr


Finally, we mention for completeness that results from  experiments such as these should be “tagged,” or annotated, with enough specific information to repeat the experiment.  These details include: beam current, accelerating potential, gas  pressure (and type), and the thickness of the chromium layer.  Gas pressure is a detail that is currently not well-described.  In  the previous examples, “pressure” refers to the overall  chamber pressure as measured by a cold-cathode ionization  gauge (CCIG) located on the wall of the vacuum chamber.  Because the CCIG pressure sensor is relatively far away from  the outlet of the gas nozzle and the sample, it is not a good  quantitative indicator of the “local pressure” at the FIB edit  site.  Perhaps we should refer to the pressure in terms of the  maximum gas-load the FIB system’s vacuum chamber can  accommodate?  Suggestions on how to resolve this ambiguity  are welcome.


4e-6 Torr


1e-5 Torr


Minimum via sizes


Users and perspective customers often ask the following  question: “what is the minimum via size that can be made with  the FIB?”  Or, “what is the maximum aspect ratio that can be  achieved?”  The answer depends on several factors, including  beam current, gas pressure, and the scanning parameters that  are used.  In any case, minimum via size is another potential  vehicle for determining milling acuity.


Consider an array of repair patterns of different sizes, as  suggested by Figure 7 below.


Figure 7.  An array of patterns for milling vias of different  sizes.


This template of patterns results in a series of vias, such as  those shown in Figure 8 below.


Device level doping related defects are some of these “nonvisual” defects mentioned above. The doping issue, though  rather subtle, is critical for device function. Therefore, the  verification of doping issues is important for yield  improvement and SRAM stability for product’s lifetime. Recent References [1-3,5,6] had investigated the doping  anomaly induced failure by nano-probing alone or with other  methods. A junction stain TEM method to visualize the doping  region in 90nm also has been previously published [4]. However, a complete and thorough electrical signature  identification of a LDD doping induced Vt shift through nanoprobing and verification by means of junction stained TEM  analysis has not been reported before for 65nm node devices.


In this paper, nano-probing is used to carefully and fully  characterize the Vt shift failure to determine a specific  electrical signature for a specific failure mechanism and then  with junction stain Transmission Electronic Microscopy (TEM) to verify the subtle LDD doping defect affecting the  Static Random Access Memory function in the 65nm  generation node.


Experimental


The soft fail samples, in this paper are referred to those chips  fails below certain voltages. According to the random  distribution characteristic and Vcc minimum test result, a  majority of the soft fail chips are suspected to be defect  related. Failure analysis of an accelerated test chip fail with an  originally high Vcc shift, as shown in Fig.1, also suggests that  it might be a spacer defect induced blocked LDD doping issue.


Figure 1a): As arrow indicates, a subtle defect is observed  between the transistor and Tungsten contact. 1b): X-TEM  image of the particle. The spacer particle might be the cause  of the implantation defect.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 88-92


-2.00E-05


4.00E-05


Drain Current (A)6.00E-058.00E-05


-0.6 -0.4 -0.2


Source Drive Drain Drive Source Drive Drain Drive


-2.00E-05(A)Drain Current 0.00E+00


C4-PO


6.00E-05


8.00E-05


-0.6 -0.4


0 0.20.40.2 0.4 0.6


Gate Voltage (V)


Reference Vd=1.2V


Reference Vd=0.1V  Fail PD2 Vd=0.1V


Fail PD2 Vd=1.2V


a)


-5.00E-06


0.00E+00 CI5.00E-06 e1.00E-05


01.50E-05 A2.00E-05 u2.50E-05


V3.00E-05


3.50E-05


Drain Drive Source Drive


b)


Fail PD2, Vd =1.2V


c)


Reference PD2, Vd =1.2V


Reference PD2, Vd =0.1V


However, for the chips selected from the sorting out test with a  smaller Vcc shift, the success rate of failure analysis via the  conventional MOSAID fault bit isolation and following  physical analysis by SEM, FIB or TEM is significantly low. Single bit failure could possibly be caused by the malfunction  of any of the six transistors in a SRAM cell shown as Fig.2.


Figure 2: Schematic of a SRAM bit. It includes 2 pull down  gates (PD), 2 pass gates (PG) and 2 pull up gates (PU).


The physical evidence of a soft SRAM failure is often nonn


visual without detailed isolation and electrical characterization


especially in 65nm devices. Therefore, a careful and thorough


electrical characterization must be performed to identify the  most likely cause of the failure. Furthermore, in order to  directly observe the doping profile of the fault device, junction  stain TEM is explored. Thus, a combined method of nanoprobing and junction stain TEM is undertaken in this paper to  reveal the root cause of this soft failure.


The chip is polished to the contacts level to gain access to the  source (S), drain (D) and gate (G) nodes of the failing bit cell  transistors. Nano-probe was used to perform the electrical  characterization of the transistors and narrow down the fault  location to a single transistor. The probing tips are applied to  the individual contacts of each transistor. The voltages are set  to simulate the test conditions. A complementary junction stain  TEM analysis method is then utilized for the visualization of  the 2-D implantation doping profiles of transistors. The ultra  shallow junction with attenuated doping concentration in 65nm  transistors and the specific thin sample for TEM observation  required advance physical analysis techniques and skillful  operation. A junction stain TEM method has been previously  published [4]. However, the method that was chosen for  this case study uses a different sample preparation procedure. The junction stain TEM method in this paper is described as  below: The sample is first milled using a focused ion beam  tool (FIB) until a ~2um thick slice is left. The front side of this  slice is milled to the front edge of the fault transistor. Then the  sample is taken out and stained in a solution of HNO3, HF and  CH3COOH, which helps yield a delineation of silicon areas  with different doping levels. The sample is further thinned  down from the opposite side until a ~100nm thick lamella is  achieved.


FEI NanoSEM600 with Zyvex K100, FEI DB235 and FEI T20  are the major tools used to perform fault transistor isolation, sample preparation and TEM observation.


Result and Discuss


Figure 3 shows the complete electrical characterization results  for the fault transistor for the failing bit cell. Figure 3a) shows


Figure 3a): The I-V curve of PD2 in fault bit and pass bit. The  PD2 in the fail bit exhibits abnormal behaviors at Vd of 1.2V  and 0.1V. 3b): The Id-Vg curve for the transistor during  source drive and drain. The fault PD2 shows a significant Id  drop for source drive than for drain drive at Vd of 1.2V. 3c): Reference PD2 shows a symmetrical characteristic for both  drain drive and source drive.


Vcc


÷Vss


PU2


Fail bit PD2


Pass bit PD2  Source


↓


a) FT


LDD abnormality


Gate


Spacer1


LDD


Spacer2


Defect


a) LDD implant


b) Spacer2 formation


c) S/D implant


Doping abnormal


d)


7.7nm


8.3nm


e)


the drain current (Id) - gate voltage (Vg) curve for the fault  transistor and reference transistor under the same conditions. The failing pull down transistor (PD2) in failing bit exhibits a  lower drain current and higher threshold voltage (Vt) for the  same drain voltage (Vd) and gate voltage (Vg) values. Moreover, the I-V curves for evaluating the balance  characteristic of the drain and source for the failing transistor  are also measured by first biasing and driving the drain during  the sweep then repeating while biasing and driving the source. As shown in Fig.3b), the results for the failing transistor (PD2) are not symmetrical unlike the symmetrical characterization  results found for the normal reference transistors shown in  Fig.3c), The differences in Id and Vt values of PD2 between  source drive and drain drive are clearly observed. The Id while


the source is being driven is significant lower than when the  drain is biased and driven. According to the electrical signature  exhibited and previous FA results, a hypothesis of excessive  resistance caused by doping issue is proposed, and the doping  defect is expected to be located at drain site only.


The junction stained TEM results for the failing PD2 transistor  are shown in Fig.4. The results show that the lightly dope drain


Figure 4: Junction stain TEM image .4a): Doping profile of  fault PD2 and pass PD2. LDD region missing is observed. 4b): Zoom-in image of PD2 shows a spacer particle above the  LDD doping region. Sample is tilted for better observation.


(LDD) on the drain side of the fault transistor is partially  blocked by the spacer particle. As Fig.5a)-5c) indicates, the  LDD implantation is a self-aligned process based on the spacer  profile. The particle in the spacer will change the spacer  profile thus affecting the formation of the LDD doping region. Figure 5d)-5e) shows a spacer defect captured after spacer1  deposition. The particle is wrapped around the spacer1. A  spacer particle, which is too small to be identified by SEM or  FIB, is easily located at the fault transistor by nano-probing. Junction stain TEM results provide the physical evidence of  the missing LDD.


Figure 5a): A schematic of self- aligned implantation process. LDD implantation is performed after spacer1 formation. The  LDD region will be impacted when the spacer1 profile is  change by a particle. 5b): The original defect might become  more inconspicuous during the spacer2 formation. 5c):


160.nm


Source/Drain implantation is performed after the spacer2  formation. The tiny defect will not impacted the spacer2  profile, and thus not have an effect on the Source/Drain  profile. 5d)-5e): A spacer defect captured right after spacer1  deposition.


The partially blocked LDD region with reduced carrier  concentration will cause weak inversion or even depletion  under normal gate voltages and could be simplified as an  additional resistor. Therefore, the PD2 degrades with an  increase threshold voltage and decreased drain current.


The single side blocked LDD causes the asymmetrical  behavior and subsequent imbalance between source and drain  driver for the transistor. Figure 6 is the schematic of an N-type


20.mm


metal-oxide semiconductor field effect transistor (MOSFET). The grey line indicates that a rather large depletion region is  observed at the drain side compared to source side when 1.2V  bias is applied to drain. Therefore, the imbalance between  source drive and drain drive is severe when high positive bias  is applied which corresponds to the test result shown in  Fig.3b). The current during source drive is significantly lower


Vg +


Vd+


|Parameter |D:drain drive S:source drive |PD2 (F) |PD2 (P) |PD1 (F) |PD1 (P) |
|---|---|---|---|---|---|

|Vtlinear (V) |D |1.32 |0.37 |0.37 |0.33 |

|Vtlinear (V) |S |1.32 |0.38 |0.38 |0.34 |

|Vtsaturated (V) |D |0.39 |0.29 |0.3 |0.29 |

|Vtsaturated (V) |S |1.11 |0.31 |0.35 |0.27 |

|Idlinear (uA)|D |0.04 |22.5 |19.4 |22.1 |

|Idlinear (uA)|S |0.02 |22.7 |19 |22.1 |

|Id saturated (uA)|D |30.6 |75.3 |70.2 |76.2 |

|Id saturated (uA)|S |0.25 |76.2 |62.9 |77.9 |

Ground


0.1V 1.2V


Voltage will mainly drop on Pinch off area


-1.00E-08


1.00E-08


2.00E-08


3.00E-08


4.00E-08


5.00E-08


6.00E-08


7.00E-08


8.00E-08


||Fail PD2, Vd =0.1V |
|---|---|

||国 。 国 国|

Figure 6: Schematic of PD gate under different drain voltage. Grey line indicates the depletion layer of 1.2V Vd, voltage is  mainly dropped at the pinch off area. Red dash line indicates  the depletion layer when Vd is 0.1V.


than that seen when the drain is driven at saturated condition  due to the dual voltage drop on pinch off and additional  resistance in the LDD due to the defect and lack of implant, when source drive is applied [2]. However, when the positive  bias is as small as 0.1V, the depletion region shrinks, as shown  by the red dash line in Figure6, The pinch off is also unable to  happen. Thus a smaller difference in effective resistance is seen between the source side and drain side. Figure 7 shows  the asymmetry characteristic of fault PD2 under Vd of 0.1V  and Table1 also summaries the electrical values for PD2 and  PD1 (can also be a reference to PD2 for the symmetric design  layout in 6T cell) in the fault bit and pass bit for the linear  region and saturated region. Both indicate that the imbalance  between source and drain at lower drain voltage is less severe  than that of the higher drain voltage.


Figure 7: The asymmetry characteristic of the fault PD2  transistor when Vd is 0.1V. It is obvious that the difference  between source drive and drain drive is smaller at 0.1V Vd  than that at the Vd = 1.2V (as shown in Fig.3b).


Table I


Summary of the electrical parameter at saturated region & linear region


* PD (F) refers to PD gate in fault bit.


PD (P) refers to PD gate in pass bit


Generally, the fault PD2 will worsen the mismatch in a cell  circuit, and lead to a higher threshold voltage for this specific  SRAM cell. Since the cell could not be properly accessed  when the operating voltage fell below a specific voltage for the  specific SRAM bit, a marginal fail occurs. The spacer particles  were not only observed at PD transistors, but also observed at  PG, PU transistors in other fail samples. The particle will  change the behavior of the transistors leading to SRAM  failure. Therefore, the reduction of spacer particles is essential  and process splits were ran to solve this defect problem.


In current 65nm technology, the conventional method of direct  SEM inspection by de-process, FIB cross-section inspection, or TEM cross section analysis are no longer effective and  reliable ways to reveal tiny defects. SRAM marginal failures  induced by a partially missing LDD were characterized by  nano-probe analysis. Based on the electrical signature that  indicated a possible partially blocked LDD implant, junction  stained TEM method was used as the method of physical  analysis to verify the defect and the signature analysis results. The partially missing LDD implant, which is located by nano  probing, was directly visualized by the junction stained TEM  method. The proposed mechanism is that the non-perfect LDD  acting as an additional resistance resulted in the malfunction of  the bit thus inducing SRAM failure. This paper demonstrated  and verified the complete electrical signature for a partially  missing LDD implant by means of the combined method of  nano-probe analysis and junction stain TEM analysis.


[1] Hung-Sung Lin, Chun-Ming Chen, “An Application of a  Nanoprobe Technique in the Characterization of  Advanced SRAM Devices” ISTFA 2008: Proceeding from  the 34th International Symposium for Testing and Failure  Analysis.pp.417-422, November 2-6, 2008, Portland, Oregon USA.


[2] Cha-Ming Shen, Tsan-Chen Chuang and Shi-Chen Lin, “Combining the Nano-Probing Technique with  Mathematics to Model and Identify Non-Visual Failures” ISTFA 2007:Proceedings of the 33rd International  Symposium for Testing and Failure Analysis, pp.214-218, November 4-8, 2007, McEnery Convention Center, San  José, California, USA.


||||1.0E-07 -5.0E-05 0.0E+00|1.0E-07 -5.0E-05 0.0E+00|1.0E-07 -5.0E-05 0.0E+00|1.0E-07 -5.0E-05 0.0E+00|1.0E-07 -5.0E-05 0.0E+00|||||||

|||-0.8 -0.6 -0.4 -0.2 0 -6.0E-05|-0.8 -0.6 -0.4 -0.2 0 -6.0E-05|-0.8 -0.6 -0.4 -0.2 0 -6.0E-05|-0.8 -0.6 -0.4 -0.2 0 -6.0E-05|-0.8 -0.6 -0.4 -0.2 0 -6.0E-05|-0.8 -0.6 -0.4 -0.2 0 -6.0E-05|||||||

|||Voltage / V Voltage/V|Voltage / V Voltage/V|Voltage / V Voltage/V|Voltage / V Voltage/V|Voltage / V Voltage/V|Voltage / V Voltage/V|Voltage / V Voltage/V|Voltage / V Voltage/V|Voltage / V Voltage/V|Voltage / V Voltage/V|Voltage / V Voltage/V|Voltage / V Voltage/V|

|||||Column 25-26: Non-ohmic |Column 25-26: Non-ohmic |Column 25-26: Non-ohmic |P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|

||||||-0.8|-0.6|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|

|||||V|-5.0E-07||P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|

||||||/||P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|

||||||+||P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|

||||||u|-1.0E-06|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|

||||||a||P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|

||||||n J|-1.5E-06|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|

||||||I||P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|

||||||d -2.0E-06 -2.5E-06 -3.0E-06|d -2.0E-06 -2.5E-06 -3.0E-06|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|P1Current * P2 Current|

||Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |Figure 12: Iterative nanoprobing technique to identify the physically unlanded CAREC 66 in a large ET structure Conclusions The SEM based Nanoprobing technique greatly improved FA turnaround in identifying the root cause of device failures and reduced the number of NVD cases. It is particularly useful in identifying causes of soft-fails, but it also plays a very important role in investigating the cause of hard-fails and improving device yield. Acknowledgments The author and co-authors would like to thank Chartered Semiconductor Failure Analysis Department TEM team for the support and assistance in acquiring TEM and EDX data. References [1]  E. Hendarto, Z. Mai, P.K. Tan, B. Lau, J. Lam, W.K Chim, “Using Probing Techniques to Identify and Study High Leakage Issues in the Development of 90 nm Process and Below,” in 13th IEEE International Symposium on the Physical and Failure Analysis of Integrated Circuits (IPFA) 3-7 July 2006, Singapore, pp. 58-62. [2]  S.L. Toh, P.K. Tan, Y.W. Goh, E. Hendarto, J.L. Cai, H Tan, Q.F. Wang, Q. Deng, J. Lam, L.C. Hsia, Z.H. Mai, “In- depth Electrical Analysis to Reveal the Failure Mechanisms with Nanoprobing,” IEEE Trans. Device Mater. Rel., Volume 8 (2) (2008), pp. 387-393. 86 |

Voltage / V


-1E-07-2E-07-3E-07


-4E-07


CurrentP1/ A


-5E-07-6E-07


5.0E-07


,


[3]  S.L. Toh, Z.H. Mai, P.K. Tan, E. Hendarto, H. Tan, Q.F. Wang, J.L. Cai, Q. Deng, T.H. Ng, Y.W. Goh, J. Lam, L.C. Hsia, “Use of Nanoprobing as the Diagnostic Tool for  Nanoscaled Devices,” in 14th IEEE International Symposium  on the Physical and Failure Analysis of Integrated Circuits (IPFA), 11-13 July 2007, Bangalore, India, pp. 53-58.


[4]  S. Doering, R. Harzer, W. Werner, “Investigation on the  Influence of Focused Electron Beam on Electrical  Characteristics of Integrated Devices,” in 33rd International  Symposium for Testing and Failure Analysis (ISTFA), 4-8  November 2007, San Jose, CA, USA, pp. 210-213.


[5] J.H. Chuang, Jon C. Lee, “Conductive Atomic Force  Microscopy Application on Leaky Contact Analysis and  Characterization,” IEEE Trans. Dev. Mat. Reliability, vol. 4, no. 1, pp. 50-53, 2004.


b


Inconspicuous defect


Electrical Signature Verification of a Lightly Doped Drain Profile Abnormality in a  65nm Device via Nano-Probing and Junction Stain TEM


Jie Su, Sanan Liang, Yoyo Wen, May Yang; Linfeng Wu, Chorng Niou, Xianfeng Chen, Gary Zhao


Semiconductor Manufacturing International Corporation, 18 Wenchang Avenue, Beijing, P.R. China, 100176  Jie_Su@smics.com


Failures caused by threshold voltage (Vt) shifts in sub-100nm  technology transistors have become very difficult to both  analyze and determine the failure mechanism. The failure  mechanisms for Vt shifts are typically non-visible for  traditional physical analysis methods such as SEM inspection  or traditional TEM analysis. This paper demonstrates how  nano-probing was used to carefully and fully characterize the  Vt shift failure to determine a specific electrical signature for a  specific failure mechanism and then with junction stain  Transmission Electronic Microscopy (TEM) verify the subtle  doping defect affecting the Static Random Access Memory  function in the 65nm generation node. Device failure due to a  lack of Lightly Dope Drain (LDD) implant induced by an  inconspicuous spacer defect was determined to be the root  cause of the failure.


The quality and reliability for Static Random Access Memory (SRAM) with transistor scaling to 65nm nodes, has been  become challenging due to additional types of marginal failure  mechanisms. These marginal defects should be identified for  process optimization and yield improvement. However, as the  defect size decreases as the technology shrinks, the subtle  defects leading to marginal failures in semiconductor devices  have become more difficult for conventional FA tools such as  Scanning Electronic Microscopy (SEM), Focus Ion Beam (FIB) or even Transmission Electronic Microscopy (TEM) to  visualize.


Figure 8.  Vias resulting from an array of patterns having  different sizes.


After milling all of the patterns, a top-down image is obtained  for measuring purposes.  Starting with the largest via (upper  left hand corner of the image) we see that successively smaller  patterns result in correspondingly smaller vias, as expected.  However, this trend eventually plateaus, because it is  impossible to mill a via smaller than a given probe size.  Note  that all of the physical vias in the bottom row (and most of  those in the middle row) are approximately the same size, despite having used patterns of different sizes.  This behavior  is illustrated in Figure 9.


Figure 9.  Measured via sizes as a function of pattern size.  The open symbols correspond to measurements of the outer  diameter of the bright halo around the via, and the closed  symbols are measurements of the dark inner portion of the  vias.  The minimum via size corresponds to the Y-intercept (marked by the red arrow).


As with the other experiments suggested above, this exercise  could be repeated at different gas pressures and beam currents  to determine the minimum via size for different sets of  operating conditions (note that a range of aspect ratios will  also be measured, provided the oxide thickness does not vary  from via to via).  However, this experiment, while interesting, probably violates rule #2 above: Tests should result in  unambiguous, quantifiable results.  The problem lies in  measuring the size of the via from a top-down perspective.  It  is hard to judge exactly where the edges of each via lie, and it  is debatable whether one should measure the outside or the  inside of the bright halo surrounding each via.  If a particular  user is consistent with his or her measuring technique, a  qualitative assessment can be made using this approach.  However, it would be difficult to remove ambiguity if  different tools (run by different operators) were being  evaluated.  A more objective analysis of via milling acuity  requires a cross sectional analysis of the via profile.


High Aspect Ratio Vias


The subject of High Aspect Ratio (HAR) vias is somewhat  controversial in Circuit Edit.  Experienced FIB users avoid  working inside HAR vias as much as possible, because of the  well-known difficulties of poor signal-to-noise, poor  endpointing, and severe gas depletion that accompany HAR  vias.  There are many effective edit techniques that can relieve  aspect ratio in most edit situations,[7] and FIB operators  should use them whenever possible.  Nevertheless, HAR vias  can be a useful vehicle for examining milling acuity.


In the following section, we describe a methodology for  quantifying HAR via quality, and use the method to  demonstrate the effects of different operating conditions (such


as gas pressure, refresh time, etc.).  Thus, the proposed HAR  evaluation method can be used for internal process  development and for comparing the performance of one FIB  column to another.


Consider the via shown in Figure 10.  The broken orange lines  indicate the footprint of the user-requested repair pattern.  This also defines the sidewall profile of a theoretically perfect  via.  We can judge the quality of our actual via by its  deviations from this ideal.  Thus, we see that the via shown in  Figure 10 is significantly over-milled near the top surface, but  is under-milled at the bottom.


Figure 10.  Cross section of a FIB-milled via.  The size of the  repair pattern used to mill this via is shown by the broken  orange lines.  Note that the actual via is over-etched at the top  and under-etched at the bottom, relative the user-requested  dimension.


One way to quantify this observation is to measure the crosssectional area of the via relative to the theoretical ideal (derived from the dimension of the repair pattern).  In  practice, it is useful to separate the via into upper and lower  halves, and measure the two regions separately.  In this way, positive deviations at the top will not cancel-out the negative  deviations at the bottom (which would result in a number that  is artificially too “good” and does not tell the complete story).  An example of such an analysis is shown in Figure 11 below.


Figure 11.  Analysis of a HAR via profile.  The cross-sectional  areas of the physical via are compared to the ideal areas.  Deviations from the ideal are highlighted.


We can normalize the cross-sectional areas of the ideal  theoretical profile to values of 1.00 (for both the upper and  lower halves), and measure the actual via profiles accordingly.  The following notation is useful:


Via score = [U, L]


Where U is the cross sectional area of the upper half of the


via, and L is the cross sectional area of the lower half of the


via (normalized to the idealized cross sectional area derived


from the user-requested dimension).  Using this notation, we


have:


Ideal via score := [1.00, 1.00]     (by definition)  Actual via score = [2.20, 0.87]


At a glance, the score of [2.20, 0.87] for the via shown in  Figures 10 and 11 tells us a great deal.  The top section of the  via has a cross-sectional area 2.2 times larger than what we  asked for, which indicates rather severe over-etch in this case.  This may have been caused by too large a beam current, too  high of a gas pressure, poor milling parameters, or some  combination of all three factors.  By contrast, the bottom half  of the via tapered closed, and was only 0.87 times the ideal.  This suggests gas depletion.


As stated above for the line burn experiments, the profile  results for this particular via are not meant to illustrate the  capabilities of any particular ion column, but rather are


presented to illustrate a technique that can be used to  quantitatively assess via milling acuity.  This is important for  users to be able to objectively compare the performance of  different ion columns under real-world conditions.


This HAR via measuring method can also be useful for  process development, because it allows us to quantitatively  assess the “goodness” of different operating conditions.  In the  following section we examine a series of HAR vias performed  under a wide variety of operating conditions.  Each via is  scored according to the above convention. Finally, these  results are used to draw conclusions about the best conditions  for HAR via milling.


HAR Via Milling Optimization


Several series of High-Aspect Ratio vias were milled.  The  parameters for two of the series are listed in Table 1.  The first  series, comprising vias A-E, investigated the effect of refresh  time (the delay time between rasters to allow the etching gas  to replenish itself on the sample surface).  The second series  of vias, F-I, examined the effect of the XeF2 gas pressure.


Table 1: Experimental Details of HAR Vias*


Via


Refresh  Time (msec)


XeF2  Pressure (Torr)


Upper  Area Score (U)


Lower  Area Score (L)


1.1e-5


2.26


0.85


B


2.19


0.84


2.08


0.89


1.92


0.95


1.79


1.00


F


2.2e-6


1.70


0.78


5.0e-6


1.74


0.79


H


1.5e-5


2.13


1.10


2.1e-5


2.24


1.20


*Parameters common to all vias: Beam current = 102 pA (30  keV); Dwell time = 200 nsec; Pixel spacing = 24 nm.


Cross sectional images of vias A-E (refresh time series) and FI (pressure series) are shown in Figures 12 and 13, respectively.


Figure 12.  Cross sectional image of via series A-E, in which  the refresh time was varied.


F               G               D              H                I


Figure 13.  Cross sectional image of via series F-J, in which  the XeF2 gas pressure was varied.


Figure 12 illustrates that the via profiles improve as the  refresh time increases.  Moving left-to-right, we observe that  the over-etch at the top of the vias is reduced, and there is also  less tapering at the bottom of the vias.  Stated a different way, the via profiles more closely approximate the ideal profile at  longer refresh times.


Figure 13 reveals that higher gas pressures have a mixed  effect on the via profiles.  Moving left-to-right, the profiles at  the top of the vias clearly get worse (more over-etch), whereas  the profiles at the bottom of the vias improve (less underetch).  Both of these trends are expected with increasing XeF2  pressure.


These qualitative observations can be made quantitative by  applying the via measuring technique described.  The  calculated over-etch and under-etch for each via is plotted as a  function of refresh time and gas pressure in Figures 14 and 15, respectively.


2.0


Refresh Time (msec)


Bottom Ideal


A               B               C               D              E


Figure 14.  Quantitative evaluation of HAR vias as a function  of refresh time.


2.0E-05 XeF2 Pressure (Torr)


Figure 15.  Quantitative evaluation of HAR vias as a function  of XeF2 gas pressure.


Note in Figure 14 that at longer refresh times both curves  trend towards the ideal value (marked by yellow broken line), although the over-etch at the top of the via does not reach the  ideal value over the range evaluated in these experiments.  This suggests that some other factor besides refresh time is  limiting the via profile.  One possibility is that the beam  current that was used in these experiments was simply too  large for this particular via size.


By contrast, Figure 15 reveals that both curves are shifted  upwards (larger cross-sectional areas) at higher XeF2  pressures.  This is initially helpful for improving the slight  under-etch observed at the lowest pressures (note that the  purple curve approaches and then crosses the yellow broken  line at a pressure of about 1.2e-5 Torr).  However, there is  significant over-etch even at the lowest pressures, and  increasing the pressure only makes the matter worse.  Clearly, adjusting the gas pressure alone will not be able to improve  the overall via profile in this particular situation.


In addition to the refresh time and pressure series described  above, another series of vias was performed to examine the  effect of different combinations of dwell time and pixel  spacing.  The experimental parameters for this data series are  shown in Table 2.


Table 2: Experimental Details of “Iso-Loop Time” HAR


Vias*


Dwell  time (nsec)


Pixel  spacing (nm)


Loop  time (msec)


Upper  area score


(U)


Lower


area  score (L)


J


12.2


0.178


1.93


0.97


K


17.4


0.179


1.97


24.0


38.8


0.171


2.02


1.01


M 1000


55.7


0.164


1.06


*Parameters common to all vias: Beam current = 102 pA (30  keV); Refresh time = 4 msec, XeF2 gas pressure ~ 1.1e-5 Torr.


Note that longer dwell times are compensated by larger pixel  spacings, such that the “loop time” for each via was roughly  constant.  The loop time is defined as the time required for a  single raster pass.  By maintaining a constant loop time (referred to as “iso-loop time” conditions), the various vias  should be subject to similar gas-enhancement conditions.


A cross sectional image of vias J-M are shown in Figure 16.


J                K             D               L               M


Figure 16.  Cross sectional image of via series J-M, in which  different dwell time/pixel spacing combinations were  examined.


Note that the via profiles look very similar in all cases.  The  similarity of these conditions is confirmed quantitatively by  plotting the over-etch and under-etch for each via, as shown in  Figure 17.


800


Dwell Time (nsec)


Figure 17.  Quantitative evaluation of HAR vias performed  with different dwell time/pixel spacing combinations.  See  Table 2 for details.


Figures 16 and 17 suggest that for a given loop time, the HAR  via profile is insensitive to the specific combinations of dwell  time and pixel spacing.  This has interesting ramifications for  endpointing.  Longer dwell times result in better signal-tonoise ratios, whereas smaller pixel spacing results in higher  imaging resolution.  Therefore, the user can adjust the dwell  time/pixel spacing ratio to suit the demands of a particular  situation: higher dwell when S/N is important, and smaller  pixel spacing when imaging resolution is key.


None of the vias examined in this simple example yielded  particularly good results.  However, the data suggest  numerous adjustments that could be made in a second round  of experiments.  For example, an intermediate gas-pressure (~1e-5 Torr) combined with a refresh time of  4 msec and a  smaller beam current would likely improve the via profile.  Additionally, a combination of long dwell time (1000 nsec) and large pixel spacing (55.7 nm) would provide maximum  S/N for endpointing, without sacrificing gas enhancement.


Finally, although this section described how the HAR via  evaluation method can be applied to process development, it is  also possible to use the method to compare via milling acuity  between different FIB systems.


The existing FIB column performance metrics of imaging  resolution and minimum spot size are of limited use in  predicting how a system will perform under real-world  operating conditions.  Several additional tests are proposed  that attempt to define and measure “milling acuity,” which is  arguably a more critical parameter for advanced Circuit Edit. Line burn experiments on chrome-on-glass samples can still  be a useful way to probe milling acuity.  Slight modifications  to the traditional experimental procedures can remove  endpointing ambiguities.  Further, the effect of gas-scattering  effects on milling acuity can be easily examined by  performing line burns at various pressures.  This is desirable, because it more closely-simulates normal FIB operating  conditions.


Via milling acuity can be measured in a variety of ways.  Simple top-down imaging of vias provides useful qualitative  information, but milling acuity is difficult to quantify with this  type of approach.  However, cross-sectional analyses of HighAspect Ratio (HAR) vias are unambiguous and extremely  informative.


A quantitative measuring scheme for evaluating the quality of  HAR vias is proposed, having the following notation: [U, L], where U and L are the normalized cross-sectional areas of the  Upper and Lower halves of the via, respectively.  A via score  of [1.00, 1.00] represents a perfect, idealized via.  Numbers >


1.00 indicate over-etch, and numbers < 1.00 indicate underetch.


The [U, L] via scoring notation can also be useful for process  development, because the effect of individual milling  parameters on the via profile can be quantified.


Thanks to Tom Miller for useful discussions on the limitations  of imaging resolution measurements.  Thanks also to Ryan  Ross for helpful suggestions during the review process.


[1] Giannuzzi, L. A., Stevie, F. A. (Eds), Introduction to  Focused Ion Beams- Instrumentation, Theory, Techniques and  Practice, Springer (New York, 2005).


[2] Herschbein, S., Richardson, C., Rue, C., “Focused Ion  Beam: A Design Repair / Fault Isolation Tool,” Tutorial  Presentation at Int’l Symp for Testing and Failure Analysis (ISTFA), Portland, OR, November, 2008.


[3] Oroff, J., Utlaut, M., Swanson, L., High Resolution  Focused Ion Beams- FIB and Its Applications, Kluwer  Academic / Plenum Publishers (New York, 2003).


[4] Private Communication, Tom Miller, FEI Company, Hillsboro, Oregon.


[5] Private Communication, Roy Hallstein and Rick  Livengood, Intel Corporation, Santa Clara, California.


[6] Abramo, M., Hahn, L., Moszkowicz, L., “Gas-Assisted  Etching: An Advanced Technique for Focused Ion Beam  Device Modification,” Proc Int’l Symp for Testing and  Failure Analysis (ISTFA), 1994, pp. 439-446.


[7] Carleson, P., Rue, C., Skinner, K., “Rewiring Chips with  FIB Circuit Edit: Speed-Up Design Validation & Performance  Optimization,” Podcast originally aired April 9, 2008, available online from Semiconductor International at: http://www.semiconductor.net/webcast/Supplier_Webcasts/18 97-


Rewiring_Chips_with_FIB_Circuit_Edit_Speed_Up_Design_Validation_Performance_Optimization.php


Novel Dielectric Etch Chemistry for the next generation of Circuit Edit: Delicate  to Low-k Dielectrics and Silicon


Vladimir V. Makarov*, Leo Krasnobayev,


Tiza Lab, LLC, 1665 S. Main Street, Milpitas, California, USA


Sabina F. Misquitta


Advanced Circuit Engineers, LLC, 316 S. Abbott Avenue, Milpitas, California, USA


A novel solution is presented for dielectric and silicon etching  when using FIB for circuit edit. In contrast to commonly used  XeF2, the new solution has a significantly higher activation  threshold that allows it to be used for etching new sensitive  low-k dielectrics and even thin silicon without the risk of  damaging these materials spontaneously. Examples of  operations presented are: etching through ultra low-k  dielectrics on a front side device, exposure of a conductor  through shallow trench isolation (STI), and trimming active  silicon when performing circuit edit on a back side device. The advantages in comparison to XeF2 applications are  discussed.


Performing circuit edit (CE) using a FIB on an integrated  circuit (IC), is essential for design debug and failure analysis


[1].  Fragile, thin inter layer dielectrics and an increase in line  and device densities inside semiconductor ICs make CE using  the FIB challenging.  CE on ICs is performed either from the  front side, which is the metallization side, or through silicon  from the back side. In both cases, the removal of dielectric  and other non-metallic materials to expose the metal line(s) of  interest for further edit is one of the key CE operations. Currently, the most used FIB chemistry for dielectric and  Silicon removal is XeF2. This compound was used for decades  in the FIB as a reliable dielectric etchant. With the  introduction of “flip-chip” package technology and new low-k  dielectrics in the IC industry, XeF2 revealed some properties  that made its use difficult or, in some cases, impossible. Fluorine in the XeF2 molecule is connected to a noble gas  atom and this bonding is relatively weak. As a result, the  fluorine from XeF2 can attack some materials like silicon and  some low-k dielectrics either spontaneously or after a very  slight external push. Obviously, this makes the use of XeF2 in  the CE of flip-chip devices complicated, where the access to  the circuitry can only be obtained through the “active silicon”. Deposition of protective dielectrics and other precautions  must be taken to avoid deterioration of the active silicon by  XeF2, which makes CE more time-consuming and less


reliable. One can expect the same sort of problems to occur  with low-k dielectrics with weak Si-C bonds. When using  XeF2 through a stack of inter connects on a front side device,this “spontaneous” attack may lead to aggressive and  uncontrolled etching of the low-k dielectrics in the lateral  directions [2].  Unwanted lateral etching of dielectrics can  increase the complexity and difficulty of the subsequent CE  operations leading to lower yields.  Therefore, a new solution  is required to overcome these difficulties. This kind of  solution – Novel Dielectric Etch (NDE) is presented in this  paper.


Application of the New Dielectric Etch Solution  for CE on front side devices


In this section, the data for using XeF2 and NDE for etching  holes through multiple layers that include sensitive low-k  dielectric layers is compared. In Fig 1a, one can see two  examples of so-called “ballooning” – lateral broadening of the  etched holes when doing this operation using XeF2.


Obviously, the uncontrolled lateral etching occurs in the  layers of low-k dielectrics. Though the damage caused by this  unwanted etching is not extensive, from the view point of the  dimensions, it can potentially compromise the whole CE  operation.


Fig.1a, b Lateral broadening of the hole when coming  through sensitive low-k dielectrics using XeF2. In both  examples one can see that the broadening happens in the  dielectric layers while the intermediate thin delimiting layers (probably, etch stoppers) show good resistance to XeF2 aggression.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 106-109


As one can see from Fig.1c, application of the NDE on the  same structure as the two examples above does not show any  damage of low-k dielectric layers.


Fig.1c The new Dielectric Etch Solution does not show any  lateral uncontrollable etching when doing the same operation  on the same structure as in Fig.1a, b.


Application of the New Dielectric Etch Solution  for CE on flip-chip devices


In the case of CE on flip-chip devices, the first operation  requires a fast and coarse etching of large (about 200x200m) trenches through thick Silicon [3]. In this case, the aggressive  formation of the SiF4 (gas) is beneficial for the fast removal of  Silicon.  The trenching operation is followed by an etch  operation to access the active silicon. At this point, XeF2 cannot be used since it is very aggressive to Silicon, and  exposure of the active silicon to XeF2 may compromise the  operation of active elements of the circuitry. Currently, the  normal practice is to use an Iodine-based chemistry to expose  the area of interest down to the STI level. Once the STI level  is reached (and active silicon is exposed), one needs to expose  conducting lines (usually copper lines) beneath STI. At this  point, one cannot use the XeF2 (which is damaging to the  active silicon) or Iodine (which corrodes the copper).  To  overcome this problem, the trench floor and the surrounding  areas are covered with FIB deposited insulator prior to  accessing the metal line of interest [4]. Not only does this  operation make the backside CE process longer, but, in cases  where the access hole is to come through spatially dense  active silicon, the CE becomes impossible. Figure 2 illustrates  a scenario in which damage occurs when etching an access  hole to a metal line, which is too close to the active silicon.


Area of possible


corrosion caused by  lateral over-etch


FIB Access


holes


FIB deposited


protective


dielectric


Fig. 2 Illustra


Fig. 2 Illustration of possible risk of active silicon damage  when using XeF2 to access a line that is too close to the active  silicon. Note that FIB deposited protective dielectric cannot  resolve the issue.


Line 1 is accessed safely, but the access hole to line 2 is too  close to the active silicon and a lateral spontaneous over-etch  occurs on the active silicon when XeF2 is used.  Such  unwanted corrosion of active silicon will destroy the device  and jeopardize the CE operation.


Application of the NDE instead of XeF2 resolves these  problems. As NDE is benign to bare silicon, there is no need  to put protective dielectric over the exposed active silicon. The lines of interest can be accessed directly. Figure 3 shows  copper metallization exposed through STI in between two  uncovered silicon areas using XeF2 and the new etchant. Lateral spontaneous etch of the active silicon by XeF2 damages the neighboring active silicon, Fig 3a. The new  dielectric etchant is used in a similar location where the  spontaneous etching of Silicon is absent and the access hole is  clean, Fig 3b.


Si


Metal Lines to be


exposed


Fig.3. a) Etch using XeF2 to expose copper lines in between  two active silicon areas causes damage to the neighboring  active silicon. b) Same procedure as in a) but using NDE  which is benign to the neighboring active silicon.


Moreover, in case the CE plan requires, the NDE allows  cutting through active silicon as it is shown in Figs.4a, b. Fig.4a demonstrates a cut through the diffusion area and the  exposure of tungsten contacts to this area from the M1 layer. This sort of operation is absolutely impossible when XeF2 is  used because of its aggressiveness to silicon. Besides, the  tilted view of this area in Fig.4b, demonstrates significant  selectivity of the etching process using the NDE for tungsten  and silicon: note the high pillars of the tungsten contacts after  silicon removal. This means that one can expect also a serious  advantage of SiO2 (and other dielectrics) etching rate(s)  compared to tungsten etching rate when using NDE, which  could be very beneficial for the CE on ICs with fully tungsten  metallization like some memory microchips.  However, additional characterization will be necessary to confirm this  expectation.


Fig.4. Removal of active silicon using NDE to expose tungsten  contacts to M1: a) top view, b) tilted view (45 degrees).


This advantage of the NDE over XeF2 and Iodine –the  possibility of cutting through thin (0.5um or less) diffusion  layers to access copper metallization, - was demonstrated, in  this work, on a flip-chip with 40nm technology.


Case Study: Shorting of inverter input/output  contacts to copper M1 on a flip-chip device


This work was done in several steps on two FIB instruments: The flip-chip device was etched through Silicon to create a  large trench (~200x200um). The trenching process was


stopped after n-well contrast had been revealed (see Fig. 5).


Fig.5 Trench for the case study on NDE application.


In the second step CAD navigation was used to find and  expose the area of interest (the inverter) and to create  landmarks (Fig.6). Up to this point, the operations were done  on the DCG OptiFIB instrument.


Fig. 6 Locally opened STI and active Silicon show target  points of the inverter (arrows). Top and bottom arrows show  location of the inverter outputs. The middle arrow shows  where M1 must be opened to contact the gate.


After the opening above had been created, the device was  relocated to the instrument equipped with NDE chemistry. The etching of the STI and active Silicon was done in a one  box operation (150nm x 650nm) to expose contacts to the  inverter outputs and to expose M1 in between (Fig.7). After  that the device was returned back to the OptiFIB to finish the  edit with conductor deposition to short the exposed contacts. Prior to the deposition on the OptiFIB, the exposed contacts  were cleaned with raw beam sputtering and a picture of the  area of interest was taken (Fig.7. Occasionally the area of  interest is turned 90 degrees clockwise with respect to Fig.6)


Fig. 7 Tungsten contacts to inverter outputs and M1 in  between are successfully exposed through diffusions and SiO2 using NDE. No corrosion on the exposed adjacent Silicon is  observed.


The whole CE operation was completed with the deposition of  low resistivity conductor to short three exposed contact. Successful electrical verification of the (expected) device  functionality was established.


This work has shown that NDE can be used to trim diffusion  structures vertically or laterally for CE or device analysis [5].


Definitely, these abilities of the new solution will be  beneficial for newer CE methodologies [6].


In this work, a new FIB dielectric etch solution is proposed.  Compared to the commonly used XeF2, this solution shows no  signs of uncontrolled etching of silicon and the newest  sensitive ultra low-k dielectrics. Obviously, for CE on front  side devices, this solution has a significant advantage over  XeF2 in those cases where new sensitive dielectrics are  involved. Regarding CE on back side devices, this advantage  becomes even more significant as the new Dielectric Etch  solution not only allows CE operations on STI with  unprotected active silicon, but also allows trimming diffusions – an operation that cannot be done with XeF2 in principle. Apparently, one should expect a significant increase in the  number of reports on successful use of the NDE as it will  definitely expand the common practice of CE on back side  devices.  Promising data were obtained on significant  selectivity of the new dielectric etch process over tungsten, which can be another advantage of the NDE over XeF2 for CE  on ICs with tungsten metallization.


[ln(


initial


thin


ultra


a a


ultraT


was computed for each ultra-thin unit and the  arithmetic mean was computed.  (There was no significant  variation in the mean calibrated ultra-thin temperature between  speed groups.)  Table 5 shows the calibrated ultra-thin  temperatures for each temperature at which the units were initially  tested. The suggested reduction in test temperature for ultra-thin  units is significant, nearly 20 C for an initial test temperature of 50  C. Because the unit performance exponentially decays with  temperature, the ultra-thin calibration temperature offset decreases  with higher initial test temperatures.


10RST control FF 35607467B0334


10RST 10um FF 35607467B0327


Initial 10um FF 35607467B0327


Initial control FF 35607467B0334


Expon. (Initial 10um FF


35607467B0327)


Expon. (10RST 10um FF


Expon. (10RST control FF


35607467B0334)


Expon. (Initial control FF


Table 5:  The ultra-thin calibrated temperature (“Average 10” =


ultraT ) is list for each temperature tested.  The calibrated  temperatures for the control units are listed for comparison.


The computed ultra-thin calibration temperatures are similar to the  temperatures we tested. Using the same data we were able to  confirm our calibration technique by comparing the initial data  taken at 85C and 70C to the ultra-thin data taken at 70C and 50C  respectively.


Temp-Cal results with Ultra-Thin temperature Calibration


Figure 8 shows the results of the ultra-thin temperature calibration  for two FF units which are representative of the overall results. Notice that with the calibration the performance of the ultra-thin  unit is nearly identical to its pre-prep performance in both cases, similar to control.


Schmoo results with Ultra-thin temperature Calibration


The shmoo data was also re-analyzed with the ultra-thin  temperature calibration. Each unique unit-test taken at 85C and  70C initially was compared the unit-test taken at 70C and 50C, respectively. Figure 9 shows an example of a unit-test comparison  with the ultra-thin calibrated temperature. In this example, the first


fail clock period of the shmoo taken at the ultra-thin calibrated  temperature is equal to the first fail clock period of the initial  shmoo.


TSearch_PSMI TSearch_Fmax vs Setpoint @ 1.19036 FF - Initial & 10RST w/ Control


3.02


3.07


3.12


3.17


3.22


68


72


74


76


78


82


84


86


Temperature Setpoint (C)


Figure 8: Plot of FMAX vs  temperature taken at 1.19036 V of two  units.  Data collected at the calibrated  ultra-thin temperature ( data points) is nearly identical to pre-prep data (data points) for both units, similar to  control(blue).


Initial 10um FF


35607467B0310


35607467B0327


calibrated 10RST 10um FF 35607467B0310


calibrated 10RST 10um FF 35607467B0327


10RST control FF


35607467B0334


Initial control FF


Figure 9: Line shmoos taken at 85 C with tuple test type g0745007 initially, before ultra-thinning (initial) and after ultra-thinning at 70C (10RST)


PMOS transistors very apparent  and crisp in ultra-thin, in normal  thickness the emission is barely  visible and blurred.


Capacitor structures are clearly  visible in ultra-thin, barely


visible at all at normal thickness.


When tested at the ultra-thin calibrated temperature 47% of the  unit-tests had a first fail clock period equal to the pre-prep first fail  clock period, 31% speed up and 22% slowed down, as shown in  Fig. 10 and Table 6. Of the unit-tests that speed up, 28% were  within 100ps of the initial first fail clock period and of the unittests that slowed down, 20% were within 100ps of the initial first  fail clock period.  A total of 95% of the unit-tests taken at the ultrathin calibrated temperature were within 100ps of the initial first  fail clock period.


Ultra-Thin Data (Round2)


After Temperature Calibration


0 5 10 15 20 25 30 35 40 45 50


UP


EQ


DOWN


Change in First Fail Clock Period


Figure 10: Plot shows % of shmoo ultra-thin unit-tests with a first  fail clock period less than the initial value (speed-up), equal to the  initial value, and greater than the initial value (slowed down) when tested at the ultra-thin calibrated temperature.


95%


Calibrated Ultra-thin temperature


% of unit-tests w/ First Fail clock period w/in  100ps of initial value


65%


Un-calibrated Ultra-Thin temperature


89%


Control


Table 6: % of ultra-thin unit-tests with a first fail clock period  within 100 ps of the initial value when tested with and without the  ultra-thin calibrated temperature.


As we determined from the control data, with no changes to the  device or the test setup, we can expect that approximately 10% of  the unit-tests will change in performance by more than 100ps. Therefore, with 95% of ultra-thin unit tests changing in  performance by 100ps or less, we have successfully calibrated the  test temperature for ultra-thin units.


A similar Temp-Cal data set has been collected on PNR family  products. The ultra-thin calibrated temperature has been  determined with the method presented here and was used to  collect post-FIB data for speed path debug. Due to the sensitivity  of power, thermal, and speed data on the 1266 process lead  vehicle product, further detail cannot be shared at this time.


Impact of Ultra-Thin of Physical Si Debug


Optical Probing  IREM


IREM analysis was performed on a Intel Core 2 Duo unit thinned  to 100um RST with traditional sample preparation process. The  unit was then ultra-thinned to 10um RST and the IREM analysis  was repeated.  The ultra-thin process substantially improves the  clarity of IREM images compared to the traditional preparation  process (see Fig.11).


Traditional Process, 100um RST


Ultra-thin process, 10um RST


Figure 11: IREM images of the same device at 100 um RST  (left)and 10 um RST (right).  Images courtesy of Dan Bockelman.


EMI-Scope III (TRE)


At first Si for one Intel product, the DCC settings of the IC were  off, preventing tail analysis and speed path identification. To solve  this problem, over 100 high precision waveforms were collected  for duty cycle characterization around the chip. From this data the  proper DCC settings were determined.  The data collection time  for each wave was 10 minutes on a device thinned with the ultrathin process to 10um RST.  This data collection would have taken  three times as long with a device 100um RST.  The ultra-thin  process created a total time savings of over 33 hours enabling path  id and tail analysis to begin nearly a week earlier that it would  have with the traditional sample preparation process.


Circuit Edit


We said in the introduction that the ultra-thin process was  revolutionary to the overall debug process of backside devices. One of the most powerful developments that the ultra-thin process  brings to debug is the creation of iterative FIB and probe work  possibilities - a concept that had not been considered before the


development of ultra-thin. Optical probe can sometimes be the  only way to localize a speedpath. This was the case with a shmoo  crack issue. The shmoo crack was root caused to 2 instances of a  series of two inverters. These inverters existed in four latch clock  timers of 8 data banks. To verify that these inverters were indeed  the cause of the problem, a FIB edit was defined to remove the  total of 64 inverters per core, a total of 128 edits. Though there  was no test that could isolate the four inverters within one latch  clock timer, within 1 data bank, the LADA could be used to  analyze the localized signal of one such instance. Because of ultrathin, we were able to define the edit such that only one instance of  the four inverter cuts was done. The LADA tool confirmed that  the edit resolved the issue by measuring the localized signal of the  edited circuit (See Fig. 12). The minimum TPT of this edit was ~1  hour using the OptiFIB.


FIB Work


LADA Signal


Figure 12: LADA data of FIB edited unit, used to resolve B3  shmoo crack issue.


With the traditional sample prep technique, a minimum of 64 edits  would have been required taking a minimum of 64 hours to  confirm this ECO. With the ultra-thin process to issue could be  resolved in 2 hours or less.


As demonstrated in this paper more predictable thermal control, improved overall optical probing quality, and increase in the  flexibility of circuit edit are the key enhancements this process  gives to the debug environment. The ultra-thin process, developed  for Intel Core 2 Duo products has reduced the overall time to  market of many products and reduced the cost of the debug  operation.


Development work is in progress to enable ultra-thin on all  devices, including large die products and products with die side  components, using a CNC. If successful, we will be able to  eliminate the need for LCE.


This body of work was made possible with the help of many  contributors. Jason Shumway provided design validation expertise  and aided in driving data collection as well as in data analysis that  lead to the development of the ultra-thin temperature calibration. Jeff Robinson contributed by providing his expertise in speedpath  debug and tail analysis to help define the testing parameters used  in the certification DOE. Jerry Fortier provided insight into the  parameters important for optical probing. He and his team  collected and analyzed the LADA and TRE data presented here. Dan Bockelman collected and analyzed the IREM data presented  here. Senthil Singaravelu provided thermal consultation. Craig  Berscheidt wrote scripts that aided in the shmoo data analysis. Dane Scott and Ken Watrobski had the vision to drive the  development of this process.


1. C-C Tsao, E LeRoy, S Saha, L Ansorge, M E Potter,


“Reliability of Ultra Thinning of Flip Chips for ThroughSilicon Analyses” IEEE-IRPS 2002.


2. C-C Tsao, Q S Wang, P Bouchet, P Sudraud, “Coaxial


Ion-Photon System”, Micro-Rel (2001) 1483.


A Versatile Design of Solid Immersion Lenses in Bulk Silicon   Using Focused Ion Beam Techniques


P. Scholz, U. Kerst, C. Boit


Berlin University of Technology, D-10587 Berlin, Germany  philipp.scholz@tu-berlin.de, +49-30-314-26803


C.-C. Tsao*, T. Lundquist


DCG Systems, Fremont, CA 94538, USA


* currently with Solyndra, Fremont, CA 94538, USA


The topic of this work is the sequential use of Solid Immersion  Lenses (SILs), created in bulk silicon in less than 20 minutes of  processing time, using a focused ion beam and a bitmap milling  process. Fibbed SILs can be removed by polishing, and the  silicon back surface resumes a perfect planar shape for further  backside analysis or the creation of more SILs. The influence of  the progressively thinner sample thickness on the magnification  of the SIL was analyzed. As fibbed SILs in this work are about


1.4 μm thick and have an additional magnification of 2.4, a  second process after removal has been found to decrease  magnification not more than 20%. The presence of interference  rings in the SIL image could be almost completely removed by  anti-reflective coating. Photon emission microscopy, performed  using fibbed SILs, allowed to clearly distinguish between sources  that were separated by 240 nm wide structures.


Our previous work [1] showed that for the backside analysis of  semiconductor devices a homogeneously shaped refractive Solid  Immersion Lens (SIL) can be created in bulk silicon using a  Focused Ion Beam (FIB). The SIL shape remains in the bulk  material after a certain amount of silicon (light gray area in  Fig. 1) is precisely removed by the FIB process. The parameters  of the SIL are the sample thickness t, the radius of curvature r, the height of the SIL h and the Radius of the SIL R.


Figure 1:  Construction of a SIL in bulk silicon with t=r.


Experiments and Results


Removing and recreating the SIL


One advantage of the presented SIL is the fast processing time of  less than 20 minutes, which is also due to the small height of the  SIL of about 1.4 μm. This gives the opportunity to remove the  SIL by chemical-mechanical polishing (CMP) and to recreate a  smooth back surface for further analysis like a new SIL on the  same spot or close by. Removing a SIL created in bulk silicon  was so far only mentioned for diffractive SILs [2], which need a  longer processing time, a larger area and the combination of FIB  implantation and plasma etch. The ability to remove this SIL  makes the described method more flexible. Until now, the  creation of a SIL with a FIB permanently altered the sample in  the SIL region and could not be applied twice to the same area. Figure 2 illustrates the individual steps of a) the SIL creation  using the FIB process, b) the removal of the SIL by polishing and  c) the creation of a new SIL on the same sample. A series of  experiments was carried out to analyze the effect of the changed  sample thickness on the SIL parameters and is used for a further  development of this technique.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 119-125


Figure 2:  a) SIL creation using the FIB process


Figure 2:  b) Removal of the SIL by polishing


Figure 2:  c) Creation of a new lens on the same sample


Laser scanning images of these experiments that correspond to  the illustration of Fig. 2 are shown in Fig. 3. The FIB created SIL  with a constant radius of curvature on a decreasing sample  thickness (t < r) can be seen in Fig. 3 a), c), e) (comparable to  Fig. 2 a) and 2 c)) and the recreated flat surface in Fig. 3 b) and  d) (comparable to Fig. 2 b)). It is observed, that the magnification  of the SIL slightly decreases on a thinner sample. In the  presented experiments, the thickness was reduced by about  10 μm with every polishing step to get a wide range of thickness  values. Polishing away only 3 μm of material would be enough  to remove the SIL, and would change the performance of the SIL  even less. The flat surface achieves its initial qualities, in terms  of roughness and transparency. All the images of Fig. 3 show the  same area of the sample.


Figure 3 a)


Figure 3 b)


Figure 3 c)


Figure 3 d)


Figure 3 e)


Figures 3:  1064 nm laser scanning images of the same optical  test structure - a),c),e) with the SIL created by FIB processing (scale is adjusted to the magnification of the SIL: 2.6, 2.1, 1.8) and b), d) after being removed by polishing.


Influence of the sample thickness


Apart from the small height, it is also the small area (radius of  SIL R  16 μm) that makes a quick SIL creation possible using  the presented method. In addition, it gives the opportunity to  fully remove the SIL and create a new surface on a slightly  thinner sample. The sample thickness t and the radius of SIL R  create the opening angle  (see Fig. 4 and Fig. 6). The question  is, how much does the opening angle  limit the performance of  the SIL? The radius of the SIL R and the radius of curvature r (r  95 μm) remain constant for the following experiments. The  previous work suggested the transverse magnification MT to be  equal to the improvement in resolution [1]. In this case of a  hemispherically shaped refractive SIL a large sample thickness  close to the radius of curvature (see Fig. 4) MT can reach values  close to the refractive index of silicon n  3.5 [3] according to  Eq. 2 from [4] using the parameters described in Fig. 5.


Figure 4:  SIL on a sample with a sample thickness t close to the  radius of curvature r. This condition leads to greater  magnification according to the lens formula Eq. 2, but creates a  smaller opening angle  (which did not have a negative effect on  lens performance for the sample thicknesses used in the  presented experiments).


n1 / so + n2 / si = (n2 – n1) / r


MT = – (n1 · si) / (n2 · so)


n1: index of refraction in object space (3.5 in this case)


n2: index of refraction in image space (1 in this case)


so: object distance (= t in this case)


si: image distance


r: radius of curvature (negative in this case)


MT: transverse magnification


Figure 5:  Spherical lens setup used to calculate MT for t  r. Object A not being in the center of curvature B.


Fig. 6 illustrates the same SIL (radius of curvature remains the  same) on a thinner sample with the sample thickness t being  much smaller than the radius of curvature r. This creates a larger  opening angle, which does not yield a higher resolution or  magnification in this case, because the rays are refracted more  than in Fig. 4 and can reach total internal reflection. The  common rule of a larger opening angle leading to a higher  resolution can be used if rays from the center of the object plane  can pass from silicon to air at a perpendicular angle, and is  therefore not directly applicable to the SIL discussed here (t  r).


In this case, the higher magnification was reached for samples  with a t closer to r, rather than samples with a large opening  angle (with t much smaller than r). The not optimized opening  angle did not have a significant influence on the performance of  the lens. The distance between t and r had the greater influence  for the given lens setup with t < r (see final results in Fig. 8).


Figure 6:  SIL on a thin sample. This condition leads to smaller  magnification according to the lens formula Eq. 2, but creates a  large opening angle .


The influence of the sample thickness on the transverse  magnification can be analyzed by solving Eq. 1 for the image  distance si (see Eq. 3) and inserting it into Eq. 2. Taking the  negative sign of the MT formula in Eq. 2 (which was neglected in  the previous work) and the negative radius of curvature r into  account, leads to Eq. 4. This formula shows the dependency of  the transverse magnification MT on the sample thickness t (equal  to the object distance so). For the calculation it is assumed, that a  small opening angle does not have a significant effect on MT. The  radius of curvature r is negative by definition, because it has its  center of curvature on the object side and not on the image side. Fig. 7 shows a graph of Eq. 4. Looking at the graph, one might  expect the magnification of the SIL to rise continuously with  increasing sample thickness, which is not the case. A small  opening angle can no longer be neglected for a t close to r and  larger than r. In addition, corresponding MT values can not be  measured, because reflective laser scanning images of a SIL  could not be brought into focus for a SIL setup with t > r.


si = n2 / ((n2 – n1) / r – n1 / so)


MT = r · n1 / (r · n1 – t (n1 – n2))


(4) The MT(t) results of the series of experiments from Fig. 2 can be  seen in Fig. 8. The process has demonstrated a good  reproducibility. It shows that, within the range of the analyzed t  values, a not optimized opening angle (for t closer to r) does not  have a significant negative influence on the SIL performance. An  additional magnification of more than 2.4 could be realized  repeatedly (the previous work only reached 1.8). This value of


2.4 was also reached for a SIL on an active device (see Fig. 9).


Figure 7: Calculated dependency of the transverse magnification  MT on the sample thickness t (using a radius of curvature r of  95 μm).


The transverse magnification was analyzed in the presented  experiments, because it can be efficiently measured by  comparing image features with and without SIL. The  improvement in resolution is, of course, the true benefit of a SIL. The transverse magnification can be used as an indicator for the  improvement in resolution if t < r, as suggested in the previous  work [1] and is therefore the parameter of the analysis.


Comparing the calculated dependency of the transverse  magnification MT on the sample thickness t to the measured  values (Fig. 8) illustrates, that the results are within the range of  the expected values. For a sample thickness close to the radius of  curvature, the values of MT are slightly below the calculated  values, because of the not optimized opening angle of the lens, which is not considered by the simple model created in Eq. 4.


Figure 8:  Results of experiments compared to the calculated  dependency of the transverse magnification MT on the sample  thickness t (using a constant radius of curvature r  95 μm).


Creating the SIL on an active device


The SIL was created on the backside of a microchip with a ring  oscillator to test the possible benefit for photon emission  microscopy (PEM). The four long black horizontal stripes in the  LSM image of Fig. 9 a) are the diffusion areas of the transistors. Fig. 9 b) shows part of the ring oscillator underneath the SIL, which is magnified by a factor of about 2.4. The 1.36 μm wide  diffusion areas appear dark. The space between them is 240 nm  wide according to the layout data and becomes visible using the  SIL (see Fig. 9 b)).


Other SIL techniques using fibbed diffractive SILs in bulk  silicon [2] even managed to show image features of 120 nm. The  creation of these diffractive SILs, however, requires a longer  processing time, a larger area and the combination of FIB  implantation and plasma etch. The fast creation of the presented  SILs in less than 20 minutes of processing time, using only the  FIB tool, is a promising solution to enhance the performance of  optical backside analysis tools.


a)                                             b)


Figure 9:  1340 nm laser scanning images using 100x objective  showing part of a ring oscillator a) without and b) with the SIL (scale is adjusted to the magnification of the SIL). The 1.36 μm  wide diffusion areas appear dark. The 240 nm wide spacing  between them becomes visible using the SIL (b). Emission  analysis is performed in Fig. 10 on the areas marked by the  white dotted squares.


While working under the same conditions, the photon emission  of the ring oscillator in Fig. 9 was measured with and without  SIL (see Fig. 10). The equipment used for this analysis was a  Phemos 1000, which uses a cooled CCD camera to do integrative  emission measurements of a running circuitry. Further  information on photon emission microscopy (PEM) can also be  found in [5]. The overall emission signal did not increase using  the SIL, due to the relatively small opening angle of the SIL. The  emission image, however, was also magnified just like the LSM  image. The SIL enhanced the resolution and gave the ability to  distinguish between the individual devices (see Fig. 10 b)).


Figure 10:  Photon emission images of the areas marked by the  white dotted squares in Fig. 9, taken with a 100x objective. Showing part of the ring oscillator a) without the SIL and b) with  the SIL (scale is adjusted to the magnification of the SIL). The  SIL gives the ability to distinguish between the individual  devices. The clearly visible spaces are marked by arrows.


The emission image without SIL from Fig. 10 a) is enlarged up  to the same scale as the image with SIL, to directly compare the  emission data measured without and with SIL. The previously  mentioned consistently recurring gaps between the areas of  strong emission can be identified with the SIL, but not without. Horizontal line scans were performed in the marked area of  Fig. 11 b) for further analysis of the measured emission. The  average values of theses scans can be seen in Fig. 12. The  regions of lower emission between the devices are clearly  visible.


Figure 11:  Photon emission data without the SIL from Fig. 10 a) enlarged and brought to the same scale as b) with the SIL. The  direct comparison shows how the image b) with the SIL presents  consistently recurring gaps between areas of strong emission, which can not be identified in a) without the SIL. The area  marked by a dotted rectangle in b) is used for horizontal line  scans of the emission values. The corresponding average values  can be seen in Fig. 12.


Figure 12:  Average values of horizontal line scans from the  area marked in Fig. 11 b). Regions of lower emission between  the devices are clearly visible.


Anti-reflective coating an a SIL


So far, most of the reflective images that were taken by a laser  scanning microscope (LSM) showed strong interference rings (see Fig. 3 a), c), e) and Fig. 14 a)). The analysis of the lens’ surface using an atomic force microscope (AFM) [1] could prove  that it was an optical effect and not an irregular geometry of the  surface. These interference rings or fringes can also be used for a  3D analysis of the surface [6]. An anti-reflective coating (ARC) was applied to the SIL to reduce the interference rings for better  image quality (see Fig. 13).


Figure 13:  An anti-reflective coating is applied to the SIL to  improve the image quality. The 142 nm thin layer of silicon  nitride is created by plasma enhanced chemical vapor  deposition.


A thin layer of silicon nitride (Si3N4 – exact stoichiometry  unknown) causes the rays that are reflected on the surface of the  ARC to interfere destructively with the rays that are reflected at  the bottom of the ARC (above the silicon). This reduces the  overall reflection on the sample surface (see also [7]). Thereby  the LSM image consists mostly of reflections from the structures  on the object plane at the bottom of the silicon.


Fig. 14 shows the effect of a 142 nm thin silicon nitride (Si3N4) layer, created by plasma enhanced chemical vapor deposition (PECVD) for the use with a 1064 nm laser wavelength. Fig. 14 b) with ARC has much better contrast and fewer  interference rings. This proves that an ARC on a SIL is a


promising solution for further image quality improvement. A  double-layer ARC consisting of tantalum pentoxide and silicon  dioxide (Ta2O5 and SiO2) was also tested, but didn’t have an  effect as good as the single-layer Si3N4 ARC. Present  experiments are analyzing the possibility to create a silicon  dioxide (SiO2) ARC directly in the FIB as part of the SIL  creation process.


Figure 14:  Laser scanning images of a SIL a) without antireflective coating and b) with a layer of Si3N4 (scale is adjusted  to the magnification of the SIL).


Being able to put a series of fibbed SILs on the same sample by  creating and removing them, increases the usability of the  presented process. A flat sample surface can be restored for  further analysis by polishing the sample. It also offers the  developers a more flexible analysis of test structures for further  experiments. The additional magnification using the SIL was  increased to a factor of 2.4 (the previous work [1] only reached


1.8) and the dependency of the magnification on the thickness of  the sample was analyzed. The creation of the SIL on an active  device made 240 nm wide image features visible and gave the  ability to distinguish between individual devices of a ring  oscillator in a photon emission image. Anti-reflective coatings  showed a great benefit for the image quality of reflective LSM  images.


All the results presented in this paper prove, that FIB processes  can be used to produce high quality SILs even in several  sequences, expanding the options of backside failure analysis  considerably.


Special thanks to Rudolf Schlangen (TU Berlin) for teaching FIB  and for continuous support. Further thanks go to Reiner Güther (FBH Berlin) for support in optics and lens questions. Thanks to  Evelin Brose, Jürgen Bruns and Chris Scharfenorth (TU Berlin) for support in anti-reflective coatings. Thanks to Ultra Tec for  sample preparation support.


[1] P. Scholz et al., “Creation of Solid Immersion Lenses in  Bulk Silicon Using Focused Ion Beam Backside Editing  Techniques”, Proc. 34th ISTFA, 2008, pp. 157-62


[2] F. Zachariasse, M. Goossens, “Diffractive lenses for high  resolution laser based failure analysis”, Proc. 31st ISTFA, 2005, pp. 1-7


[3] H.-G. Wagemann, Grundlagen der optoelektronischen  Halbleiterbauelemente, B. G. Teubner (Stuttgart 1998), p. 228


[4] E. Hecht, Optics, Addison-Wesley (2nd Ed., 1974), p.134. p.144, p. 507


[5] C. Boit, “Fundamentals of Photon Emission (PEM) in  Silicon - Electroluminescence for Analysis of Electronic  Circuit and Device Functionality”, Microelectronics Failure  Analysis Desk Reference 5th Edition, 2004, pp. 356-368


The authors would like to thank Jeff Large, Texas  Instruments, and Rajesh Jain, DCG Systems, for their inputs, discussions and assistance.


[1] T. Malik, R. Jain, R. Nicholson, T. Lundquist “Role of


Circuit Edit in Post-Silicon Debug and Diagnosis”,


presentation at 2nd  IEEE Silicon Debug & Diagnosis


Workshop,  November 2005, Austin, TX


[2] C. Richardson, LSI Logic and Jeff Large, TI, Dallas –Private Communication, 2008


[3] C. Rue, S. Herschbein, C. Scrudato, “Backside Circuit


Edit on Full-Thickness Silicon Devices”, presentation at  12th European FIB Users Group Meeting (EFUG),


September 2008, Maastricht, the Netherlands


[4] R Lee, N Antoniou, “FIB Micro-surgery on Flip Chips


from the Backside”, Proc 24th Int’l Symp for Testing and  Failure Analysis, Dallas, TX, November 1998, pp. 455-


459.


[5] Boit, C. et al., “Impact of Backside Circuit Edit on Active  Device Performance in Bulk Silicon ICs”, Proc 36th IEEE Int’l Test Conf, Austin, TX,  November 2005, pp. 1236 - 1244


[6] R. Schlangen, P.Sadewater, U. Kerst, C. Boit “Contact to  Contacts or Silicide by Use of Backside FIB Circuit Edit  allowing to approach every Active Circuit Node”


Microelectronics Reliability 46 (2006) 1498–1503


Global Die UltraThin Silicon for Backside Diagnostics and Circuit Edit


Dane Scott, Erin O’Donnell


Intel Corporation, Folsom, CA, USA  Tahir Malik, Rajesh Jain


DCG Systems, Inc, Fremont, CA, USA


For more than 10 years, silicon thinning techniques have  been relegated to an art form of mere necessity to enable  complex optical probing and circuit edit analysis. Silicon  thinning is a fundamental aspect of diagnostic analysis and  while it is well-understood that limitations in the area of  silicon thinning can severely limit high-quality diagnostic  results, poor thinning results have generally been accepted as  standard environmental operating conditions with which  optical probe and circuit edit engineers must cope.  Presented  here is a scientific approach to thinning silicon to enable  predictable high-precision, high-quality results.


Remaining silicon thickness (RST) has been debated  throughout the years because it was uncertain how much  thinning was excessive.  Primary perceived limitations  included mechanical constraints (package / die warping) and  post-thinning thermal control.  Adding to the complexity of  the discussion has been the fact that RST has been largely  uncertain because analysis usually involved determining how  much silicon was removed rather than how much silicon  remains.  All of these challenges have been overcome.


A novel process has been developed to ultra-thin bulk Si to as low  as 10um remaining Si thickness, eliminating the need for the  Laser Chemical Etcher for circuit edit and improving optical  emission probing considerably. This sample preparation process  has been used on Intel Core2 Duo products with a success rate of  98%. Post FIB unit testing is a critical step in this debug process. A technique was developed to calibrate the change in thermal  resistivity of the ultra-thin unit such that it will remain within  100ps of its original FMax performance in 90% of tests.


Sample preparation is a critical aspect of the physical Si debug of  backside devices as it is a key enabler for optical probing and  circuit edit [1]. Often a circuit edit is necessary to validate an ECO (Engineering Change Order) and the FIB work is in the critical  path of the product release to market. Minimizing the total time to  complete any FIB edit and maximizing the usefulness of any one  FIB edit directly effects product time to market.


Once a circuit edit is defined the IHS (Integrated Heat Sink), if  there is one, is detached from the die and package. The unit is then  thinned using a polishing wheel and diamond lapping films.


Traditionally the unit would be thinned to 100um RST then loaded  into a Laser Chemical Etcher (LCE) for bulk Si removal. With  both the traditional method and the ultra-thin processes, the  remaining bulk Si in the edit location is removed with the FIB  tool. The ideal thickness to mill through with the FIB is ~10um. Milling through thicker material is possible, but increases the FIB  edit TPT.


With the ultra-thin process the unit is thinned to as low as 10um  RST. Because of the scale there are some subtleties that need to be  included in the process that are not necessary when thinning to  100um RST. First, it is crucial that the RST measurement is  accurate within +/- 1um of the actual value to ensure the highest  success rate, whereas when thinning to 100um a measurement  accuracy of +/-10um is sufficient. Second, it is important that the  Si thickness be uniform across the die. Planarity of the die on an  ultra-thin unit is important to minimize the FIB edit TPT and  maximize device preparation success rate. Planarity on a global  level is not a critical parameter when using the LCE for bulk Si  removal because the LCE has end pointing tools which allow the  operator to stop the Si removal process with 10um RST. Once the  unit is prepared for FIB it may or may not be tested to recharacterize its performance before FIB.


Once the FIB edit is complete, successful testing of the unit on a  tester or system validation board is critical. An extensive  experiment was done to test the reliability of ultra-thin devices and  certify the process.  Trends in the data collected were found and a  method was developed to compensate for changes in device  performance due to changes in Si thickness and thermal stack-up.   The ultra-thin process presented here is revolutionary to the debug  process of backside devices increasing the overall efficiency of the  debug operation. It reduces product cost and time to market in  three major ways. The overall cost of the debug operation is  reduced by eliminating the LCE. The TPT of the sample  preparation process, and circuit edit using the OptiFIB is also  reduced, thereby reducing the time taken to solve any issue being  resolved with a circuit edit and/or optical probing. Most  significant is the improvement to efficiency that the ultra-thin  process provides by enabling a high degree of flexibility in using  circuit edits to solve problems. The ultra-thin process enables  iterative, unplanned FIB work, maximizing the usefulness of an  edited device.  With the ultra-thin process a new root cause  technique has been developed, using iterative FIB work and  optical probing.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 110-118


Ultra-Thin Process


Polishing Process


A process has been developed to ultra-thin FCBGA (Flip Chip  Ball Grid Array) and FCPGA (Flip Chip Pin Grid Array) devices  with die sizes ranging from approximately 10.5x13.8 mm to


8.9x12.3 mm and packages that do not have die-side components. This process is being implemented on most Intel Core 2 Duo  products, including quad-core products.  With both the traditional  and the ultra-thin process the package is seated into the polish  puck, a fixture designed by Intel’s internal mechanical engineering  team. The puck is designed in compliance with the Allied  polishing wheel head. The puck is fixed on the polishing head and  the packaged unit is placed face down on polishing wheel. The  wheel rotates between 100 and 250rpm, the head rotates around  the puck axis and around the arm axis.


Figure 1: Packaged CPU device seated in polishing puck (left).  Allied polishing wheel (right).


The die and the package are not planar, but warped in a convex  shape. This deformation occurs during thermal cycling processes  involved in C4 assembly because of the mismatch of the  coefficient of expansion of Si and the substrate. To compensate for  this the head of the polisher is tilted at an angle with a shim.


A diamond lapping film, ranging from 30um grit to 1um grit, adhered to the wheel with water, is used to etch the bulk Si.  (The  surface tension of the water forms a sufficient bond between the  film and the wheel.) Traditionally larger grit diamond lapping  films were used to remove the majority of the material (~600 um) and polycrystalline diamond suspension slurries and polishing  cloths were used to remove the remaining 30um of material above  the thinning target. The polishing cloth on the wheel does not  create a rigid surface and thereby reduces the effect of the shim. This causes material to be removed from the center of the die  faster than material is removed from the edges of the die. This  effect is not significant enough to be observed when thinning to  100um with a measurement system with precision of +/-10um, but is noticeable with ultra-thin process. Using lapping films in  conjunction with the shim to remove all of the Si necessary, we  are able to maintain the crown on the die throughout the process. In this way, the smaller grit films are used to achieve planarity as  well as to polish the surface of the Si.  (The Si removal rates of the  films range from 85um/min for bulk removal steps to less than  1um/min for polish steps.) For FIB, the surface of the Si must be


polished to ensure even etch rates in the localized area of the edit  location. When thinning to 100um in preparation for LCE the  finest grit generally used is 3um as the LCE does not require a  polished surface for even etch. The LCE provides a finish smooth  enough for FIB work.


Because of the scale, the ultra-thin process requires tight  tolerances on all of the mechanical components used. The head of  the Allied polisher is parallel to the wheel to within +/-2um. The  polishing puck is parallel lapped with a tolerance of +/-2.5 um.  Small imperfections in the planarity of the puck and polishing  head can be compensated for by rotating the die in the puck. A  spread sheet was developed that calculates removal times based  on removal rate of each film and suggests rotation angle based on  the measurements after each step to enable quick TPT with good  success rate.


Removing Si with CNC milling to obtain RSTs of ~10um with +/- 2um accuracy is in development.


Measurement System


As mentioned in the introduction, the ultra-thin process requires a  measurement tool that provides accurate RST measurements with  a high degree of precision. A tool was developed in a joint effort  between Intel and VarioScale called VarioMetric®. With a  broadband multi channel tunable laser, this tool shines light  through the Si and detects the light that is reflected from the  surface of the Si and the light that is reflected from the dielectric  layer of the IC and refracted through the Si. The total reflected  light is collected with 1mm InGaAs PIN diode, which measures  the total reflected intensity. The light reflected from the two  surfaces will interfere constructively or destructively depending  on the wavelength of the light and the thickness of the Si, as with  all thin films. With the intensity measurement for a particular  wavelength the tool calculates the thickness of the bulk Si. The  tool is used in a light saturated environment so basing the Si  measurement on one intensity measurement could be very noisy. To compensate for this the laser scans across >250nm of  wavelengths and measures the intensity of the reflected light for  each wavelength. From the power spectrum, the thickness is  accurately calculated.


The total amount of light reflected is the sum of the light reflected  from the Si surface and the light reflected from the surface of the  dielectric.  The total power of the reflected light is given by,


01


t


ik


d


i


total


where d = Si thickness, n = index of refraction, k = extinction  coefficient, l = wavelength and other terms as in Fig. 2.  The  exponential terms account for the phase of the light and the  attenuation of the signal in the Si.  It is assumed here that the light  is normally incident on the IC.  Measurement time of the tool is  less than 1 sec with a measurement error of <1um when the RST  is between 10um and 250um.


Air


Dielectric


no


n1 n2


t01


r12


Figure 2: Image courtesy of Varioscale


Traditionally, when thinning to 100um the RST is calculated by  measuring the height of the die with respect to the puck after  removing Si and taking the difference to determine the amount of  material removed. The total amount of material removed is  subtracted from the initial Si thickness to calculate the RST. It is  assumed that the initial thickness is the original wafer thickness (775um for CWM and PNR) across the die. The measurements  are done with a micrometer (Mitutoyo Corp IDC Digimatic  Indicators with Absolute Series 543). This measurement technique  yields RST results of +/-10 um of the target RST.


Circuit Edit Flow


The ultra-thinning process can be completed in 0.75 hours to 1.0  hours for single die products and 1 to 2 hours for dual die  products. The total sample preparation time to thin a device to  between100um and 150um RST in preparation to use the LCE for  bulk Si removal is 0.6 hours for single die products. The TPT for  LCE trenching depends on the tool used and number of trenches  necessary. The number of LCE trenches will vary depending on  the edit definition. Typically LCE TPT ranges from 0.5 hours to


1.5 hours. The minimum TPT for sample preparation with the  traditional method is 1.1 hours and is 0.75 hours with the ultra-thin  process. This difference of 0.35 hours may not seem significant, but when this number is propagated throughout the debug process, from first Si to product release, this is a difference of 140 hours for  a typical 400 circuit edits.


The ultra-thin process also provides some key benefits to circuit  edit TPT using the OptiFIB. In the OptiFIB a nIR light source is  coaxial to the ion beam [2]. The IR microscope is used for through  Si imaging of metal and diffusion layers of the IC.  (Before  loading the unit into the FIB an anti-reflective coating is applied to  the surface. This protects the Si surface outside of the edit location  area from the reactive chemistries used in the FIB and enhances  the signal to noise of the IR microscope.) The OptiFIB tool, like  other FIB and Probe tools is linked to the CAD database of the  microprocessor.


Ultra-thin Si reduces the signal attenuation resulting higher signal  to noise ratio and less signal distortion than 100um Si. The high  resolution, coaxial IR image enables highly precise global optical  CAD alignment on the OptiFIB in 5 minutes or less with no  adjustment for signal distortion necessary. This is a considerable


TPT reduction for FIB edits on the OptiFIB in comparison to  100um RST due to increased signal to noise ratio and less signal  distortion.


Figure 3: The high quality IR signal from ultra-thin Si enables a  fast and precise 3 point CAD alignment in OptiFIB.


With the traditional sample preparation process the circuit edit  must be fully defined before milling LCE trenches. Trenches are  milled with a step down method with a maximum angle of 80  degrees as demonstrated in figure 4. With the proper planning  most edits can be accommodated with LCE trench sizes but  possibly not all proposed edit definitions. Though the risk that a  potential edit definition may not be possible to do with LCE  trenching is relatively small, the possibility that an LCE trench  may obstruct a future, un-planned edit opportunity is a problem.


500 um 400 um 300 um 250 um


LCE Trench


10um RST


Edit Location


80°


Figure 4: A typical LCE trench in 100 um RST Si.  Note that the  bottom of the trench is typically 200 to 250 um wide at the edit  location.  If a second edit was defined after this trench had been  milled within ~300 um of the original edit, it could not be done  due to the obstruction of the first trench.


The nature of the debug environment requires a high degree of  flexibility. LCE trenches significantly limit the flexibility of circuit  edit. Often a circuit edit fixes a bug that limits visibility into other  problems, such as a boot up bug or a limiting speedpath.  When  this is this case, the FIB edited unit can be used to collect data on  other logic bugs or speedpaths that could not otherwise be  collected. When another problem is found and a circuit edit is  defined it is often most beneficial and efficient to edit the already  FIB edited unit. With the traditional method, there is always a risk  that the new edit cannot be accommodated due to an LCE trench  obstruction. If this is the case, it is conceivable that all of the data  previously collected on the unit with the first circuit edit would  need to be re-collected. With the ultra-thin process this is never a  problem. Because the die is thinned globally to 10um, a FIB  edited device can go straight from test to FIB. This reduces the


TPT of such an edit. More importantly, ultra-thin enables a level  of flexibility that creates a more efficient debug process overall.  Also note that quality IR images cannot be obtained inside LCE  trenches. With the traditional sample preparation method the  typical distance between the edit location and probe data  acquisition is ~250um whereas with the ultra-thin process, probe  data can be acquired within 6 to10um of the edit location.


Once a unit is modified with a circuit edit on the FIB tool, testing  the unit to determine if the circuit modification defined solves the  problem of interest is a critical aspect of the circuit edit process. It  is also important that the unit performance not be fundamentally  changed due the device preparation process so that the circuit edit  fix is a realistic representation of the proposed ECO.


Unit Testing


FIB edited units may be tested in several different ways depending  on the problem the circuit edit is meant to resolve. For speed path  circuit edits the unit is generally tested on a tester with a hand  clamp used to socket the device. For logic edits the units are often  tested in system validation. Thermal control is an important aspect  of all microprocessor testing and even more important when  finding and resolving bugs, as they can be temperature dependent. Most CPUs are standard with an IHS attached, though mobile  products do not have an IHS. The standard thermal interface  material (TIM) between the IHS and die is solder. After  preparation it is not practical to restore the original thermal stackup in the debug lab environment because the solder TIM will  cause electrical shorting in the FIB trenches and the original IHS  is designed for Si 775um thick and will not make sufficient  contact to the thinned die.  A modified IHS has been developed for  thinned Si. The modified IHS is made of nickel plated copper, similar to the original, but is thick enough to make contact with  the thin die. The tolerance specification for the contact surfaces is +/-10um. To ensure that there are no thermal gaps between the  IHS and die a thin layer of thermal grease is applied to the IHS  and a layer of indium foil is placed between the grease and the die. The foil conforms to the Si surface to ensure good thermal contact  between die and IHS and serves to protect the FIB trenches from  becoming filled with thermal grease and potentially limiting  further work. For many applications the IHS is temporarily  attached during testing, meaning pressure is applied to the IHS  with the handsocket to achieve thermal contact between die and  IHS during test but there is no attachment between IHS and  package outside of the socket. The modified IHS can also be  permanently attached. To do this positive pressure is applied to the  die/IHS interface while an adhesive, applied to the perimeter of  IHS and package cures at high temperature.


Preparing a device for circuit edit with either the traditional  method or the ultra-thin process causes the thermal profile of the  device to change. With the ultra-thin process this change is due to  the global change in Si thickness and the change in thermal  resistivity of the IHS and TIM. Like the ultra-thin process the  traditional method changes the thermal profile of the device  globally with the removal ~600um of bulk Si and change in


thermal stack-up.  However, the LCE trench also changes the Si  locally in the edit location so the change in the thermal profile of  the device is more complex. The thermal solution is applied  globally across the die and not locally to the edit location. The  change in the thermal profile of a device prepared with the  traditional method cannot be calibrated therefore the device must  be re-characterized before continuing with the circuit edit. The  LCE trench introduces a risk that the circuit problem in question  will be influenced by the uncontrolled change in the thermal  profile and is not representative of the ECO. Because the change  in thermal profile of an ultra-thin device is global across the die it  can be measured and compensated for in a systematic way.


Certification and Reliability


An aggressive test flow was deployed to certify the ultra-thin  process and ultra-thin devices as reliable.  With this data a method  was developed to compensate for any change in performance due  to the change Si thickness and thermal stack-up.


Intel Core 2 Duo units (1264 process material) were used to  certify the ultra-thin process. The units were tested with two  different test flows. Line and column shmoos were collected to  determine the impact of changes in the performance due to  thinning for an on speed path debug. A Temp-Cal test flow was  also used to get a comprehensive dataset reflecting the correlation  between the device performance and setpoint temperature of the  thermal solution. This test flow included deep sleep current  measurements (SICC), dynamic current measurements (DICC), and TSearch FMax measurements using PSMI patterns. The  SICC and DICC tests measure the current the device draws when  it’s in a very low power state and in a very high power state, respectively. The TSearch test uses a binary search algorithm to  find the last passing frequency, or FMax of the device for a group  of patterns. Before and after each test a thermal diode reading is  collected. This reading gives valuable insight into the performance  of the thermal solution.


The tests were done on an s9k tester with an ETC1K thermal  solution with power following enabled. (The ETC1K responds to  current draw from the device for cooling. The system was  calibrated with the same calibration as for the production ATE  thermal solution for Conroe B0; ktheta =0.16.) The ETC1K  delivers the cooling solution through a hand-clamp. The units  were tested, ultra-thinned, and retested with the same test plan, tester, TIU and ETC1K. Temporarily attached modified IHS’s  were used with the standard thermal stack-up of indium foil and  thermal grease for testing the ultra-thinned units. Data was  collected on a total of 12 units; eight units were ultra-thinned and  four units were used as control. (A total of 11 units were ultrathinned, 2 were hard failures after prep due to user error, 1 was  thrown out because it failed on s9k during test, but later passed on  all patterns on IMS.) No changes were made to the control units  throughout the test flow. The control units were used to capture  any changes in the tester or thermal solution over the test plan. The units were chosen based on their IDVP (In Die Variation  Probe) value collected in sort such that the distribution across  speeds was nearly uniform for both the ultra-thin and control unit


sets.  (IDVP value is an indicator of the processor leakage and  overall device performance. Values are binned in Fast-Fast (FF), Fast (F), Typical (T), Slow (S), and Slow-Slow (SS) for each  processor stepping.)


Results


Certification Test Plan Details


In Tables 1 - 3 the test parameters are defined. The temperature set  points were chosen based on the most common test temperatures  used for path-id and probe work for a speed path debug. The  shmoo patterns were chosen because each hit speed paths on most  of the units, and some were found to have been sensitive to LCE  trenches during product debug. The Vcc used for the shmoo data  collection was within the range of stable Vcc for the products.  (It  was our intent to collect shmoos at multiple vcc’s, however there  was an error in the test script that was not caught until after the  experiment was complete.)  The shmoo resolution is the same as  the resolution most commonly used for tail analysis and speedpath  debug, which is fine enough to catch the pass to fail point without  introducing much noise. The shmoo range was set wide enough  that the pass to fail region on any functional unit would be  measured. Both column and line shmoos were collected because  both tests are used for path id in speedpath debug and because  there is a slight difference in DUT time between the two test types.  (The DUT time is longer for column shmoos than line shmoos  because the device is tested at a particular clock period, T, for each  pattern, then tested at T + 50ps for each pattern, whereas the line  shmoo tests the unit for each pattern one at a time.)


Each unique shmoo test will be called a unit-test for the remainder  of this paper. For example a column shmoo of unit B0334 tested  with pattern g0725012, at 50C is one unique unit-test.


The temp-cal SICC, DICC, and TSearch PSMI patterns were the  same as the patterns used for design validation of the products  tested.  The shmoo resolution used for the TSearch is the finest  possible and the range was set so as to measure the pass to fail  point on any functional unit.


EXB


0.16


Ktheta


50C, 70C, 85C


ETC1K Temperature Setpoints


Table 1. General test parameters


Column Shmoo and Line Shmoo


Test types


Number of unique tests per unit


Total number of tests per unit


40min


Test Time


8ns – 14ns


Range (core clock per)


50ps


Resolution (core clock per)


g0725012, g0729029, g0741444, g0745007, g0734746


Tuples


0.999V


Table 2. Shmoo test parameters


1.24401, 1.19036, 1.13633, 1.05445, .99916


Vcc (V)


75


n/a


13.33ns, 15.00ns, 17.15ns


20ns


Core CLCK_Per


d0672675


DICC


5min


d0691527


SICC


10ps


35 patterns


TSearch_PSMI


Resolution


Test type


Total Test Time Tuples


Table 3. Temp-Cal test parameters


Shmoo results


The first fail core clock period of each unique unit-test was  compared before and after ultra-thinning. Figure 5 shows an  example of a unique unit-test comparison. In this case the unit-test  slows down by 150 ps after thinning.


Compared to control, a significant number of ultra-thin unit-tests  slowed down after sample prep, as can be see in Fig. 6 and Table


4.  The change in performance of the ultra-thin units is  considerable, with 35% of unit-tests having changed in the first  fail clock period by more than 100 ps compared to only 10% of  control units changing by that magnitude. (1 tester tick, 50 ps, can  sometimes be noisy; a change of two tester ticks 100 ps is  significant as it should be outside tester noise.) Control unit data  confirms that changes in performance of the ultra-thin units are  directly related to physical changes in the device and thermal  stack-up and were not related to the tester or thermal solution (ETC1K). Control unit data also gives an idea of the noise  expected in these tests. With no changes to the device or the test  setup, approximately 10% of the unit-tests can be expected to  change in performance by more than 100 ps.


Figure 5: Line shmoos taken at 85C with tuple test type g0745007 initially, before ultra-thinning (Initial), and after ultra thinning (10RST).


Ultra-Thin Data (Round 2)


0 10 20 30 40 50 60 70 80 90


Initial-10umRST Control


Figure 6: Plot shows the % of shmoo ultra-thin unit-tests (blue) and control unit-tests (purple) with a first fail clock period less  than the initial value (speed-up), equal to and greater than the  initial value (slowed down).


% of unit-tests w/ FF clck_per w/in  100ps of initial value


Ultra-Thin


Table 4: % of ultra-thin and control unit-tests with a first fail clock  period within 100 ps of the initial value.


Temp-Cal Data Analysis


We evaluated the correlation between the unit performance and  thermal set point with the TSearch PSMI data as this was the most  aggressive performance test done in the temp-cal test suite. The  SICC and DICC test data were used to gauge the thermal stability  of the unit and thermal solution. Figure 7 shows a representative  plot of the TSearch PSMI data for ultra-thin and control units. The  FMax data for each unit was plotted against the temperature set  point and the exponential curve fit was calculated. The FMax of  the units decreases with the increase of temperature, as expected.  Notice that the FMax of the ultra-thin unit is significantly reduced  from its initial value, consistent with the shmoo data, but that the  relationship between the FMax and temperature is similar before  and after ultra-thin.  Notice also that the FMax of the control unit  does not change significantly between the two rounds of testing, confirming that any changes in the ultra-thin units are due to  sample preparation and not the test setup.


y = 3.3713e-0.0007x


R2 = 0.9969


y = 3.3219e-0.0007x


R2 = 0.9911


y = 3.3437e-0.001x R2 = 1


y = 3.3182e-0.0009x


R2 = 0.9998


3


3.1


3.2


3.3


55


65


85


Figure 7: The TSearch FMax vs. temperature set point data taken  at 1.19036 V of two FF (FastFast, based on the IVDP value >11700) is plotted. The FMax of  the control unit (blue) is  relatively constant over both  rounds of testing.  The FMax of  the ultta-thin unit (yellow) is  significantly slower after ultrathin ( data points) than initially ( data points), but that curve fit  is nearly identical.


Each data set fit nicely to the curve:


mT


FMax *


By constraining the FMax of the ultra-thin unit to equal to the  unit’s original FMax, we could calculate the test temperature  which should return the unit to its original performance.


[6] R. K. Jain et al., “Advanced Fringe Analysis Techniques in  Circuit Edit”, Proc. 32nd ISTFA, 2006, pp. 79-85


[7] J. Aguilar et al., “Optical mismatch in double AR coated   c-Si, a simple theoretical and experimental correlation”, 3rd  World Conference on Photovoltaic Energy Conversion, 2003, pp. 1001-1004


Localized Epoxy Layer Formation on Surface Defect Using a Micro-brush in a  Plucking System


Kun-Lin Lin, Jian-Shing Luo, Hsiu-Ting Lee, and Jeremy D. Russell


Physical Failure Analysis Department, Inotera Memories Inc., Taoyuan, Taiwan kenlin@inotera.com


Focused ion beam (FIB) milling has been increasingly applied  in sample preparation for transmission electron microscopy (TEM) with device shrinkage in the Integrated Circuit (IC) industry. There are several advantages for TEM specimen  preparation using FIB, for example, complex heterogeneous  structures with different sputtering rates can be thinned  uniformly and specific regions of interest can be located  precisely for defect analysis [1-5]. In general, a protection  layer, such as platinum (Pt), tungsten (W) metal or carbon, is  deposited onto a target area using FIB ion-beam assisted  deposition to avoid excessive Ga ion damage. However, a  damage or amorphous layer, about 20 to 30nm thick for a 30  KeV beam is formed at the interface between the protection  layer and sample surface [6-9]. This damage layer makes tiny  feature analysis very difficult or impossible. From previous  studies [10-12], an intermediate buffer layer, such as metal or  polymer, was added between the Pt protection layer and the  sample surface using plasma or sputter deposition to avoid  damage for surface defect analysis. For instance, Rubanov and  Munroe [10] investigated the effect of gold sputter-coated  films in minimizing damage in FIB-produced TEM  specimens. They found the gold film was either locally absent  or of low thickness (< 15 nm), and ion beam damage of the  near surface region was evident. Kato et al. [11] used a  plasma-polymerized protective film with a thickness of 100  nm instead of ion-beam deposited Pt, showing no amorphous  layer. However, using an intermediate buffer layer creates a  localization problem for site-specific defect analysis. Kwong  and Zhang [12] have recently developed a method to address  the above issues using two deposition steps, first electronbeam assisted Pt deposition followed by ion-beam deposited  Pt, for surface defect analysis [12]. Unfortunately, there is still  a problem due to the poor step coverage of electron-beam  assisted Pt deposition for some defect analysis cases. Fig. 1  shows a typical image taken using the method described in


[12]. It can be seen that in this case, a thin damage or mixing  layer was also found on the defect surface and sample surface, as denoted by the arrows, after electron-beam assisted Pt  deposition.


Plucking systems are widely used in ex-situ lift-out TEM  sample preparation [13]. For this technique, the sample is  extracted from a FIB system and loaded onto a standard  plucking system after FIB thinning. The plucking system is  used to lift out the thinned sample by electrostatic attraction  and then place it on carbon-coated copper grids for TEM


analysis using a glass needle. We developed a novel method  to cover a tiny epoxy layer as an intermediate buffer on the  site-specific surface defect using a micro-bush on the tip of a  glass needle in a plucking system without sample surface  damage and localization problems. This method was applied  successfully for surface defect analysis. In this paper, the  details of the method and some real cases are described. The  microstructures were investigated using an FEI Tecnai TF20  field emission gun TEM equipped with high angle annular  dark field (HAADF) detector, energy dispersive X-ray  spectroscopy (EDS) and Gatan image filter (GIF) systems.


Figure 1 A bright field (BF) TEM image shows a poor step  coverage around a surface defect’s bottom and the damage or  mixing layers, indicated by arrows, formed after e-beam  assisted Pt deposition.


Methods and Results


Micro-brushes and buffer layer preparation  Different kinds of fibre were selected to attach to the tip of a  glass needle to form micro-brushes. They were: cotton thread, human hair, paintbrush, and cat’s hair, as shown in Fig. 2. Their tip sizes are about 330, 120, 30, and 10m in diameter, respectively. The different micro-brushes were applied to  different sizes of surface defects.  The cotton thread and  human hair micro-brushes are suitable for hundreds of micron


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 126-129


size defects. For the paintbrush and cat’s hair micro-brushes, they are best for sub-micron size defects.


Figure 2 OM images show different kinds of micro-brushes, including (a) cotton thread (b) human hair (c) paintbrush, and


(d) cat’s hair.


Fig. 3 shows the procedure of covering an epoxy micro-layer, such as M-bond 610, Allied High Tech Products, Inc., USA. on a site-specific area of the sample surface using a microbrush on the tip of a glass needle controlled by the plucking  system. Using this method, it is easy to locate exactly the sitespecific defect on the sample surface without any damage or  localization problems.


Examples


Fig. 4 shows a real case demonstrating our new micro-bush  method. Surface defects were initially found by an inline  inspection system that creates a KLA results file which is  subsequently imported into Knights Camelot navigation  software to locate the defects using a high resolution imaging  system, in this case a full wafer dual-beam FIB. Specific  surface defects were localized using the navigation system  with the defect map and then marked using ion beam milling  for subsequent detailed analysis. In order to avoid damage of  the defect’s surface during FIB marking, only one low current  ion beam scan was done to indicate the locations of markers  around the defect, as shown in Fig. 4(a). An alternative  approach is using a full wafer DUV OM with laser marker. After FIB marking, the defect was covered by a droplet of  epoxy as intermediate buffer layer using our micro-brush  method, as shown in Fig. 4(b). Then, the sample was cured at  10  on a hot plate for 15 minutes. After curing, the defect  location was covered by a Pt protection layer in a DB FIB  system, as shown in Fig. 4(c). Next step is to slice the surface  defect sample using a dicing saw and then glue the slice to a  half copper ring with epoxy. The sample is cleaned in acetone  solution. The final step is to use a DB FIB system to thin the


pre-thinned sample down to a proper thickness for TEM  analysis.


Figure 3 A schematic diagram illustrating the micro-brush  method. (a) A micro-brush is moved to the target with a  micro-droplet of epoxy by a plucking system (b) The epoxy  droplet is painted covered onto the target by touching (c) After covering the epoxy on the target, the micro-brush is  moved away.


(d)


Figure 4 (a) OM image of surface defect marked by a DB FIB  system with low beam current (b) OM image of an epoxy  micro-droplet on the surface defect using micro-brush (c) Ion  beam image of the surface defect after the ion-beam Pt  deposition.


Fig. 5 shows the resulting TEM/energy filtering TEM (EFTEM) images. A surface defect is covered by a micro-size  epoxy protective layer using our micro-brush method, as  shown in Fig. 5(a). It reveals that the step coverage of epoxy  is better than that of electron-beam assisted Pt deposition. In  addition, no damage was caused to the surface defect during  sample preparation. The zero energy loss peak (ZLP)/EFTEM  image of the circle region in Fig. 5(a) is shown in Fig. 5(b), indicating a thin layer was found on the surface of the defect. Figs. 5(c-f) show the maps of C, Si, Fe elements and a RGB (red-green-blue) composite color map, in Fig, 5(b), indicating  that the thin layer is pure Si. Therefore, it can be concluded  that the defect fell on to the wafer surface before Si  deposition. In addition, the defect consisted of Fe, Ni and Cr  from EDS/TEM analysis. Fig. 6(a) shows a ZLP image of


another surface defect. The defect was successfully covered  by a micro-size intermediate buffer layer using micro-brush  method.  Figs. 6(b-f) display elemental distribution maps of C, Si, N, O, and Al, respectively.  From the maps of element  distribution, it reveals that the surface defect consists of an  oxynitride hard mask layer residue and an Al particle.  This  surface defect would have then blocked the metal line  patterning at the defect addresses.  From above analysis  results; the micro-brush method has succeeded in avoiding  damage to the defect surface, which is a common source of  artifacts in this kind of defect analysis.


Figure 5(a) A cross-sectional BF TEM image shows a surface  defect is well covered by an epoxy protective layer using the  micro-brush method. (b) ZLP image of the circle region in  Fig. 5(a); (c)-(f) Elemental distribution maps of C, Si, Fe, and  RGB image of Fig. 5(b), respectively.


(d)(b)


(e)(c)(a)


Target


Mark


Epoxy


Pt


Figure 6(a) A cross-sectional ZLP image shows a surface  defect is well covered by an epoxy protective layer using the  micro-brush method. (b)-(f) Elemental distribution maps of C, Si, N, O, and Al of Fig. 6(a), respectively.


A novel micro-brush method to cover a defect with a microlayer on the target’s surface using a standard plucking system  has been introduced and successfully applied in the  application of surface defect analysis without any damage or  localization problem. Various sizes of micro-brushes, ranged  between 10 and 330 m, were chosen to deal with different  sizes of surface defects. The micro-brush method can be used  for both in-film and on-surface defects.


The authors would like to thank all their colleagues in Inotera  Memories Inc. for their help in this work, particularly the  transmission electron microscopy and surface analysis (TEMSA) and secondary electron microscopy (SEM) sections  in the physical failure analysis department. The authors are


grateful to Lang-Yu Huang for her support on preparing  defect samples.


[1] L. A. Giannuzzi and F. A. Stevie, “A review of Focused  Ion Beam Milling Techniques for TEM Specimen  Preparation”, Micron, 30, 197-204, 1999.


[2] R. M. Langford and A. K. Petford-Long, “Preparation  of Transmission Electron Microscopy Cross-section  Specimens Using Focused Ion Beam Milling”, J. Vac. Sci. Technol., A19(5), 2186-2193, 2001.


[3] K. Yabusaki and H. Sasaki, “ Specimen Preparation  Technique for a Microstructure Analysis Using the  Focused Ion Beam Process, FuruKawa Review, No 22, 1-6, 2002.


[4] B. Yao and K. R. Coffey, “A high-throughput Approach  for Cross-sectional Transmission Electron Microscopy  Sample Preparation of Thin Films”, Journal of Electron  Microscopy, 1-6, 2008.


[5] H. Sasaki, T. Matsuda, T. Kato, T. Muroga, Y. Iijima, T. Saitoh, F. Iwase, Y. Yamada, T. Izumi, Y. Shiohara and  T. Hirayama, “ Specimen Preparation for Highresolution Transmission Electron Microscopy Using  Focused Ion Beam and Ar Ion Milling”, Journal of  Electron Microscopy, 53(5), 497-500, 2004.


[6] S. Rubanov and P. R. Munroe, “FIB-induced Damage in  Silicon,” Journal of Microscopy, Vol. 214, 213-221,


2003.


[7] S. Rubanov and P. R. Munroe, “Investigation of the  Structure of Damage Layers in TEM Samples Prepared  Using a Focused Ion Beam,” J. Mater. Sci. Lett., 20(13), 1181-1184, 2001.


[8] J. P. McCaffrey, M. W. Phaneuf, and L. D. Madsen, “Surface Damage Formation During Ion-Beam  Thinning of Samples for Transmission Electron  Microscopy”, Ultramicroscopy, 87, 97-104, 2001.


[9] T. Ishitani, K. Umemura, T. Ohnishi, T. Yaguchi, and T. Kamino, “Improvement in Performance of Focused Ion  Beam Cross-sectioning: Aspects of Ion-Sample  Interaction”, Journal of Electron Microscopy, 53(5), 443-449, 2004.


[10] S. Rubanov and P. R. Munroe, “The Effect of the Gold  Sputter-coated films in Minimising Damage in FIBproduced TEM Specimens”, Materials Letters 57, 2238-2241, 2003.


[11] N. I. Kato, N. Miura, and N. Tsutsui, “ A Plasmapolymerized Protective Film for Transmission Electron  Microscopy Specimen Preparation by Focused Ion  Beam Etching”, J. Vac. Sci. Technol., A16(3), 1127-1130, 1998.


[12] W. Y. Kwong and W. Y. Zhang, “Electron-Beam  Assisted Platinum Deposition As a Protective Layer for  FIB and TEM Applications”, Semiconductor  Manufacturing, IEEE International Symposium, 13-15, 469-471, 2005.


[13] R. M. Langford and C. Clinton, “In situ lift-out using a  FIB-SEM system”, Micron, 35, 607–611, 2004.


(e)


Deterministic Polishing


Applications in Failure Analysis


Principal Member of Technical Staff  Maxim Integrated Products


7250 Evergreen Parkway


Hillsboro, OR 97124


Development of a reliable mechanical decapsulation procedure  for an IC process incorporating Cu and organic passivation  layers resulted in a better understanding of the polishing  process. The improved polishing technique --Deterministic  Polishing-- is an adaptation of an advanced polishing  technology employed by the optics industry to fabricate highly  accurate optical elements.  These results can be applied to a  broad class of polishing applications


Devices fabricated with copper metallization can present  significant problems with regard to failure analysis, particularly when it is necessary to decapsulate them.  Acids  used to perform chemical decapsulation can attack copper  circuit metallization and organic low-K dielectrics.  Mechanical decapsulation can work, but we have found that  sample preparation issues and inherent limitations in the  polishing process can lead to less than optimum results.  Investigations into the polishing problem, with emphasis on  rastered (XY) polishing tools (such as the ASAP-1) were  performed.  Theoretical modeling using a variation on  Preston’s Equation was used to help optimize the polishing  process.  Deterministic Polishing, a technique derived from the  Optics industry, was investigated as a way to address some of  these problems.   Theoretical and real-world results have  shown that Deterministic Polishing (DP) can give improved  polishing results.  These improvements are not confined to  copper or low-K devices.  Guidelines for achieving optimal  results are provided, some of which are also applicable to  currently-available (non-DP-based) tools.


Polishing Issues


Polishing problems can be separated into two categories:   nonuniform polishing effects, and planarity problems due to  sample mounting and tool setup.  The former problem is most  apparent on polishing systems that raster the sample in an X-Y


fashion underneath a polishing tool, and planarity problems are  common to all types of polishing systems.


Nonuniform Polishing Problems


Polishing tools that raster the sample underneath a rotating  polishing tip can exhibit nonuniform polishing.  This is  particularly true for tools that use a mechanically rastered XY  table, where the “slow” axis is driven by a reduction gear  connected to the “fast” axis.  In this type of tool, the tool traces  out a Lissajous figure.  See Figure 1.


Figure 1  Lissajous pattern drawn by the ASAP.  This was  traced out by placing a pencil lead in the tool while its XY  table was in motion.  The sinusoidal table motion leads to  repetitive variations in the tool step size and dwell time, which, in turn, results in nonuniform polishing.


Since the table motion is sinusoidal, in addition to variations in  the effective coverage of the polishing bit, the velocity of the  table varies across the sample:  it moves fastest near the center  and slowest at the edges.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 130-134


Another effect common to all types of rastered polishing  systems can impact the quality of the polish.  As the tool  approaches the edge of the sample, its contact area decreases.   As a result, the polishing pressure increases.  This also causes  nonuniform polishing.


Sample Planarity Problems


In our experience, it is very difficult to achieve perfect sample  planarity.  In the case of performing parallel lap on packaged  devices, we have observed that dice are not assembled exactly  parallel to the external plane of the package.  This is most  likely due to thickness variations in the die attach material.  It  also is difficult to mount parts on sample holders and get them  exactly flat.  For relatively large devices, a tilt of just a few  microns across the span of a die can result in the exposure or  removal of different metal layers across the die, so this can be  a significant problem.  Many polishing tools have adjustments  which are designed to address this problem, but in our  experience it is difficult to exactly compensate for sample tilt.  Some tools have an optical alignment system that can improve  the situation, but they require additional sample preparation; or  that system may not be available or applicable to a particular  sample.


We began addressing these problems by modeling the  polishing process.


Modeling the Polishing Process


Although many theoretical approaches have been taken to  model the polishing process, in most cases they reduce to  variations on Preston’s Equation [1].  Time integration of  Preston’s equation results in


T(x,y) = K*V(x,y)*P(x,y)*t(x,y)   (Eq’n 1)


Where


T(x,y) = Thickness of material removed at each x,y point.


K = A polishing constant, dependant on the materials present. V(x,y) = Velocity of the polishing medium at each sample  point.


P(x,y) = Pressure between the sample and polishing medium  over each sample point.


t(x,y) =  Elapsed time over each sample point.


In this derivation, it is assumed that T(x,y), V(x,y) and P(x,y) are independent of time.


It can be seen that nonuniform velocity V(x,y) and variable  dwell time t(x,y) results in a nonuniform polishing rate.  In  addition, pressure variations (which occur when the tool  approaches the edges of the sample) also contribute to  polishing nonuniformity.


A computer program was written to simulate polishing using  this equation.  See Figure 2 for an example of the program  output.


Figure 2.  Polishing uniformity vs. position, using mechanical  XY table.


In this simulation, the polishing uniformity of a single die is  shown.  The peaks at each corner of the sample are caused by  variations in pressure as the polishing tool moves over the  corners of the die:  pressure increases as the contact area  decreases.  Also, note the higher-frequency variations across  the die .  This is a consequence of the nonuniform sinusoidal  motion of the mechanical XY table.


We have found that Deterministic Polishing can eliminate, or  at least improve, polishing artifacts caused by these problems.


Deterministic Polishing is a technique used in the optics  industry to produce highly accurate optical surfaces [2, 3].  In  its typical application a small polishing tool is used to  interactively finish a larger glass surface.  Deviations from the  desired shape are periodically measured, fed into a computer, and a special program controls the tool.  The tool spends more  time over the highest regions and thus selectively polishes the  surface until the desired shape is achieved.  This approach has  yielded surfaces that can deviate from the desired shape by  only a few nanometers [2].


Computer simulations of samples polished using a uniform  velocity have indicated that DP can produce good results -- with some caveats.  See Figure 3.


Figure 3.  Computer simulation of Deterministic Polishing.


The simulation shows that, for the most part, the polishing  uniformity should be very good.  It only degrades near the  edges and corners of the sample, where two effects come into  play.  The first is the expected pressure variation, which causes  the ridges and peaks near (but not at) the edges and corners of  the die.  The second effect causes the steep drop-off in  polishing rate at the edges of the sample.  This is due to the  polishing tool’s greatly reduced dwell time (i.e., t(x,y) in  Equation 1) at the edges.  At the extremes of the tool position, the tool approaches its maxim (or minimum) and then  immediately reverses its motion, so the time spent at the edge  of the die is much lower, compared to the center.  Attempts to  address this by increasing the tool dwell time near the edges of  the sample were not successful, leading to exaggerated  polishing rates in other locations.  It should be noted that this  problem would apply to all rastered polishing tools, regardless  of the XY table design.


The extent of the nonlinear zone at the edges of the sample can  be reduced by reducing the diameter of the polishing tool.  Mechanically-rastered systems have a lower size limit that is  established by the ratio of the X and Y axes’ motion.  If the  ratio is N, the absolute minimum tool diameter is:


Min-tool-Diameter = Ss/N.


(Eq’n 2)


Where Ss is the sample dimension along the slow axis of the  polishing tools’ XY table.


If the tool is any smaller, it will not hit portions of the sample.  This limitation does not apply to DP because the XY stage’s  step size can be set to whatever is necessary to ensure good  tool coverage.  However, since rastered polishing systems only  polish a small location at any one time, the time needed to  process a sample will go up as the tool diameter decreases.


We also simulated an “edge protection” scheme, where the die  is surrounded by an encapsulation material -- either by the  molding compound that is around the die in its package, or by


material that is added later (for instance, a 2-part epoxy).  Mechanical decapsulation of acid-sensitive devices would  naturally result in edge protection.   The expected result of  adding edge protection was to eliminate pressure variations  near the edge of the die and therefore improve polish  uniformity.  The dwell-time problem can be addressed by  ensuring that the edge protection “zone” is wide enough for the  polishing tool to travel all the way across the sample, rather  than reversing at the sample edges.  If edge protection is used, along with extending the tool motion, the result can be very  good.  See Figure 4.  Although the dwell-time effect is still  present, the sample is located inside the flattest region.


Since dwell time effects apply to all types of rastered polishing  systems, edge protection is universally applicable to them.  If  we find it necessary to use epoxy, the polishing rate of the  epoxy glue is adjusted to more closely match that of the die.  We accomplish this by adding a filler to the epoxy -- either  alumina powder or fine glass beads (i.e., fine sandblasting  media).  If using alumina powder, be sure to use a grit that is at  least as fine as the smallest polishing grit you will use.  Otherwise the epoxy will become a source of larger particles  that will scratch the sample.  The concentration of alumina or  glass beads does not appear to be critical.


Figure 4.  Simulated polishing rate for sample with edge


protection.  The optimum sample processing "window" is in  the central region.


Compensating for Sample Tilt


Simulations have shown that DP should be able to compensate  for tilted samples, by varying the dwell time in a linear fashion  across the sample.  See Figure 5.  Figures 6 and 7 illustrate a  real-world example of tilt compensation using DP.


Figure 5.  Simulation showing polishing variation across a


sample.  The tool dwell time increased as it moved to the right.  This simulation assumes that edge protection is also used.


Figure 6.  Photo of sample prior to DP procedure.  It would


be very difficult to prevent over-polishing in the lower left


region of the die using conventional polishing techniques.


Figure 7.  Sample at end of DP procedure.


Implementation


The prototype DP hardware is shown in Figure 8.  Each axis of  the XY stage is driven by an RC servo motor and a rack and  pinion gear. Many parts were purchased at hobbyist robotics  supply stores.  The programmable stage is mounted on a  commercially-available milling/polishing machine.  A small  microcontroller is used to convert commands from the PC to  the PWM-modulated signals used to control the R/C servos.  Not shown:  a PC running the user interface.


Figure 8.  DP hardware installed on an ASAP-1.  No


modifications to the tool are required to use the DP hardware.


As implemented here, DP cannot achieve the nanometer-level  precision reported by optics workers [2].  This probably is not  a fundamental limitation so there is room for improvement, if  needed.  The “measurement” portion of the process is a simple  microscopic examination of the sample, so adjustments to the  dwell time are made by editing the job file based on  observation and experience.  Currently there is no automation  of the measurement-correction sequence.  However, in our  experience, visual inspection and subsequent adjustments of  the polishing parameters in an iterative fashion can yield very  good results.  Figs 6 and 7 illustrate this point.


Modeling the polishing process has shown that there are a  number of effects that affect all rastered polishing systems.  Simulation and real world results have shown that polishing  uniformity is best when the dwell time over each portion of the  sample is uniform, and when the edges of the sample are  protected -- either by the package molding compound, or with  epoxy that is placed around the die as part of the sample  mounting procedure. Edge protection was found to be a useful  sample preparation technique for all types of rastered polishing  systems (it also works very well for more traditional parallellap techniques).  Deterministic Polishing addresses a number  of polishing uniformity issues and permits the use of smaller  polishing bits. In addition, DP can compensate for sample tilt.  These improvements are particularly applicable to devices that  would be damaged by the acids used to perform chemical  decapsulation.


All computer-rendered images were generated using openDX, an open source scientific visualization program running on  Cygwin.  The microcontroller is from the Arduino open source  project.


All references to commercially offered products are © their  respective owners.


[1]  Preston, F. W., “The Theory and Design of Glass Plate


Polishing Machines”, J. Soc. Glass Technology, 11, 247


(1927)


[2] Arkwright J. et al, “A Deterministic Optical Figure


Correction Technique That Preserves Precision-Polished


Surface Quality”, Optics Express Vol 16 No. 18 (2008)


[3] Yutaka Uda et al, “Digital Polishing Method for CMP


System Using a Smaller Diameter Polishing Pad”  Nikon webpublished article.


Near-Infrared Microscopy in Semiconductor Failure Analysis Applications


Thomas B. Davis, Robert Reagan, Yangyang Sun, and Tom Jiang  Micron Technology Inc., Boise, Idaho USA


Results have demonstrated that a low temperature O2 plasma  process will provide an oxide of sufficient quality to produce


good scanning capacitance measurements. The process can be  used to prepare samples for top down analysis or epoxy potted  polished cross sections. In the latter case, the plasma process  resulted in minimal alteration of the epoxy resin eliminating  the need for additional sample clean up. It is necessary to  adjust the plasma power and process pressure to minimize  surface contamination caused by sidewall sputtering. The  optimal process conditions using a PlasmaTherm 790 etch  system were determined to be a 15 minute plasma treatment at  20sccm O2, 100W, and 1000mTorr pressure. The best results  were obtained by placing the samples on a bare silicon wafer  after performing an O2 chamber clean. Although this process  results in some trace fluorine and carbon surface  contamination, this appeared to have no impact on the SCM  signal.


[1] Maria Virginia Stangoni, “Scanning Probe Techniques for  Dopant Profile Characterization”, PHD Dissertation, Swiss Federal Institute of Technology, 2005.


[2] Hal Edwards, Rudye McGlothlin, Richard San Martin, Elisa U, Michael Gribelyuk, Rachel Mahaffy, C. Ken  Shih, R. Scott List and Vladimir A. Ukraintsev, “Scanning  capacitance spectroscopy: an analytical technique for pnjunction delineation in silicon devices,” Applied Physics  Letters, Volume 72, Number 6, 9 February 1998.


[3] Didier Goghero, Vito Raineri, and Filippo Giannazzo, “Study of interface states and oxide quality to avoid  contrast reversal in scanning capacitance microscopy,” Applied Physics Letters, Volume 81, Number 10, 2  September 2002.


Non-destructive Failure Analysis in Organic Thin-film Transistors


Shih-Ting Liu, Tao-Chi Liu, Ming-Lun Chang, King-Ting Chiang, Su-Ping Chiu, Jandel Lin


Integrated Service Technology Inc., No.19, Pu-ding Rd., Hsin-chu 30072, Taiwan (R.O.C.)   selena_liu@istgroup.com


Po-Yuan Lo, Pei-Wen Li


Department of Electrical Engineering, National Central University, Taoyuan 32001, Taiwan (R.O.C.) PYLO@itri.org.tw


Contrary to conventional Si-based device, organic thin-film  transistors (OTFTs) constituting organic semiconductors are  easily destroyed. Investigating failures using traditional FA  techniques like electron microscopy or cross section is hard to  procure. Therefore, the purpose of this paper attempts to  develop approaches for failure analysis of OTFTs. We  successfully demonstrate a non-destructive technique for  defect inspection and localization, exactly specifying the  failure of OTFT with a void existing in the organic dielectric. Application of optical beam induced resistance change (OBIRCH) in current leakage localization is shown. Non-distorted cross-section sample preparation and analysis of  internal structure by electron microscopy are also developed. Moreover, the failure of OTFT induced by high driving  voltage punch-through is analyzed using techniques  established in the article. Particular elongation of the gate  metal was found to be the failure mode.


Organic thin-film transistors (OTFTs) have attracted much  attention recently due to their low-cost and low-temperature  fabrication process. Because of the flexibility of organic  materials, OTFTs are more compatible with a polymeric  substrate compared with conventional Si-based TFT. The use  of OTFTs has been successfully demonstrated as backplanes  in active matrix organic light emitting diodes (AMOLEDs) [1-2], electronic paper [3-7], radio-frequency identification (RFID) tags [8] and smartcards. Organic semiconductor  materials and fabrication technology of OTFTs have been  widely investigated since the first organic field-effect  transistor was fabricated in 1986 [9]. However, very little  attention has been given to failure analysis of organic-based  electronics.


The performance of OTFTs has steadily progressed because of  the continuing improvements in organic materials. Early  OTFTs had very low field effect mobility, often ranging  between 10-4 and 10-6 cm2/V-s [10-11]. In current years, the  mobility values ranged from 0.21 to 0.17cm2/V-s [4]. Although growing numbers of researchers have improved the


performance of OTFTs, the mobility is still lower than  Si-based TFT. Typically, the field effect mobility is between


0.5 to 1.0 cm2/V-s for hydrogenated amorphous silicon (a-Si:H) TFT, most of which are used in AMLCD [1]. Therefore, high driving voltage for OTFTs is required if the  switching speed becomes tolerable. Even though the  low-temperature fabrication process reduces a great quantity  of cost and enables OTFTs to have great potential for wide  variety applications, the deposition conditions strongly  influence morphology and uniformity of dielectric layer. Research on the effect of dielectric roughness in the  performance of OTFTs has been reported [12-13]. The  properties of dielectric strongly dominate the mobility of  transistors. Generally speaking, poor quality of organic thin  film and high driving voltage may result in considerably  violent failures seldom discovered in conventional Si-based  devices.


Since organic materials are easily damaged, the failure  analysis by observation of a cross-section specimen is hard to  obtain. Investigating the defect of organic dielectric and the  leakage and failure mode of OTFTs is an arduous task. No  research, however, has been done on this issue. The  requirement of applicable technologies for analysis on organic  device is urgent. Thus, this paper aims to develop  non-destructive techniques to analyze the failure modes of  OTFTs, which are explicitly discussed in this study. Such  research is still in its infancy, but it may have a contribution to  the failure analysis of devices and packages comprising  organics and flexible substrate.


The first section of this article analyzes electrical deviation, addressing both detection and sited estimation of void defects  existing in organic dielectric thin-film. This is followed by  cross-section sample preparation of the OTFT. Observation of  void defect by electron microscopy is carried out. Then, we  demonstrate two analytic techniques for the failure resulting  from high driving voltage punch-through. One is current  leakage localization and the other is cross-section specimen  preparation mentioned in the previous section. Finally, failures  of OTFTs are expressly defined and analyzed by the  techniques established in this paper.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 144-148


Experiment


Sample Preparation and Electrical Stress


In this experiment, we fabricated an OTFT device as shown in  Fig. 1 which consists of a gold electrode, a polyethylene  naphthalate (PEN) substrate, and an organic dielectric  thin-film. The device configuration was a top-gate structure  with 510nm thick gate insulator and 40nm thick source/drain (S/D) electrode. Perfluorinated polymer was utilized for the  dielectric layer and fabricated by a spin-coating method at a  rate of 500 rpm. The electrical stressing was achieved under  the cyclic bumping gate voltage from 40 to -40 at VD = -10 V. The serious drain leakage became a significant issue at this  point.


Measurement and Analysis


The electrical characteristics of OTFTs were measured using a  semiconductor parameter analyzer  AGILENT HP4156 at  room temperature. An OLYMPUS BX51 Optical Microscope (OM) was used for general imaging of the device. The void  defects of organic dielectric thin-films were observed by  scanning acoustic microscopy (SAM), using a SONIX  Quantum 350 in C-Scan mode with a UHF (3nm) transducer. This technique was used for localization of void defects in  A-Scan mode by estimating the time difference of the echo of  the acoustic wave. Cross-section specimens were prepared by  mechanical polishing and ion beam respectively. Ion beam  cross-section polishing (CP) was performed on a JEOL  SM-09010, and preparations were accomplished at an  acceleration voltage of 6 kV under a pressure of 1x10-4 Pa. A  dual beam focused ion beam (DB-FIB), SII FEI NOVA 200, was also applied to the cross-section sample in order to  specify the failure at an ultra-low ion beam energy of 10kV. Cross-section image of the OTFT, prepared by mechanical  polishing, was acquired to use a HITACHI S-4800 scanning  electron microscope (SEM) with an acceleration voltage at 10  kV. The SEM image was formed by means of secondary  electrons. The images of transmission electron microscopy (TEM) were provided by a JEOL JEM-2100F microscope. Photon emission analysis (PEA) is a well-known method used  for localization of silicon failures resulting from current  leakage. Because the sensitivity in I-V variation, optical beam  induced resistance change (OBIRCH) performed on a  HAMAMATSU AMOS-200 apparatus was chosen to detect  leakage of OTFTs. The thermal stimulus was achieved with a  1340nm laser by supplying voltage of 0.1 V at gate and S/D  probing point.


Figure 1: (a) Schematic cross-section and (B) optical  micrograph of a single OTFT device on flexible PEN  substrate.


Results and Discussion


The drain and gate current vs. gate voltage characteristics for  an OTFT device is depicted in Fig. 2. Noticing that the gate  current continuously increased as the device was off. This  result undoubtedly indicates that leakage exists through the  channel region. We first observed the organic dielectric  deposited on PEN substrate by optical microscopy. Fig. 3(a) shows the OM image of the organic dielectric thin-film. However, no defects were optically discovered. In order to  figure out the reason for this failure, the inspection with  technique called SAM is applied, as shown in Fig. 3(b). Two  circles are discovered and indicated with white arrows. According to the principle of the SAM instrument, the circles  probably reveal the rise and fall of the dielectric. In other  words, there is an existence of a void defect within the organic  dielectric. These findings in Fig. 3 clearly suggest that the  void defect within organic dielectric can be detected without  destruction by using SAM rather than optical microscopy. Fig. 4 is the A-Scan image that represents the reflected acoustic  waves gathered from the circumference (dash line) and the  surface of dielectric (solid line). The time deviation, as small  as 3 ns, obtained from dash line (5.097 s) and solid line (5.094 s) in Fig. 4. The result has shown that the depth of  voids can be exactly specified by estimating the time  difference of echo in A-Scan mode of SAM [14].


Figure 2: Drain current and gate voltage characteristics for  OTFT with void defect in organic dielectric thin film. Red line  is gate current and gate voltage characteristics.


It is widely believed that important information about the  interlayer structure and defects can be obtained through  cross-sectional observation. The analysis of cross-section  structure of OTFTs is performed in Fig. 5. Fig. 5(a) shows  SEM images with sample preparation by using mechanical  polishing. Even though the composition can be examined  easily, the S/D thickness is measured as 167 nm. Compared to  the schematic structure in Fig. 1(a), S/D thickness  dramatically increases. These findings propose that  mechanical polishing causes the Au electrode to extend. To  solve this problem, cross section sample preparation using an  ion beam (CP) is shown in Fig. 5(b). However, our data  provides possible evidence that ion beam heating led the  polymer of OTFT to evaporate and further distort the device. Apparently, neither mechanical polishing nor CP is a suitable  preparation method for OTFTs. DB-FIB method with  ultra-low voltage is presented in Fig. 5(c). The data shows a


perfect cross sectional image and the S/D thickness is  measured as 50.46 nm. Consequently, cross-section  preparation of OTFTs without acute distortion and metallic  elongation is revealed by using ultra-low voltage DB-FIB. Table 1 offers the comparison of the above three methods, including S/D thickness, the deviation percentage of S/D  thickness between observation and design, and cost. As shown  in the third row of Table 1, the deviation can be achieved as  small as 26.15% by DB-FIB. Even though this technique has  the undeniable merit of offering great cross-section  preparation for device consisting of organic materials, it has  some limitations. A preparation of a wide surface area of a  specimen and high cost are presumably considerable  problems.


(a)                      (b)


Figure 3: (a) OM image of organic dielectric thin film. The  white circle is a hand-made marker. No defect is shown on the  region where voids are discovered in Fig 3b, which is pointed  with white arrow. (b) C-scan SAM image in the same area as  Fig. (a). The white arrow point toward the discovered voids.


Figure 4: A-scan SAM image of organic dielectric thin film. Solid line indicates reflected echo wave of thin film surface. Dash line represents the sub-surface in which voids exist.


Based on previous works in cross-section sample preparation, void defects inspected using SAM can be analyzed by electron  microscopy. For instance, multiple voids within an OTFT are  observed by using SAM in C-scan mode, as shown in Fig. 6(a). The upper left area pointed by white arrow is analyzed  by TEM, which is shown in Fig. 6(b). Existence of voids in  organic dielectric thin-film is clearly illustrated in the scheme  image. These reported experiments have demonstrated that a  non-destructive technique called SAM is a powerful  instrument for void defect localization applied to organic  electronics.


Figure 5: A cross-section sample of OTFT prepared (a) mechanical polishing, (b) CP and (c) ultra-low voltage  DB-FIB, observed using OM, SEM and TEM respectively.


Table 1: Comparision of the three preparation methods for  cross-section sample of OTFTs mentioned in this paper.


Method


Mechanical  polishing


CP


Ultra-low  voltage   DB-FIB


S/D


thickness (nm)


167


N/A


50.46


Deviation (%) 317.5


26.15


low


middle


expensive


As was mentioned above, high driving voltage of OTFTs may  result in considerable failures, especially when void defects  are in the dielectric. Analysis of device damage resulting from  high driving voltage punch-through can be shown in the  following section. Firstly, an approach for quickly specifying  leakage faults of an OTFT device is completed by OBIRCH,


(a)                       (b)


Figure6: (a) C-scan SAM image of OTFT device. The white  arrow points toward the void location for analysis. (b) TEM  image of cross-sectional void observation for the void location  pointed in Fig. (a).


which is a common practice in current leakage localization for  Si-based devices. The application of OBIRCH discovers the  leakage site by detecting the signal of current change as shown  in Fig. 7(a). The arrowed site in Fig. 7(a) is the exact location  of current leakage. To observe the failure mode induced by  high driving voltage for OTFTs, DB-FIB is used to prepare the  specimen at the arrowed site. Fig. 7(b) demonstrates the  cross-section observation by TEM. The data, showing the gate  metal rolling and penetration into the dielectric, is completely  a new discovery. The vital findings from this data suggest that  high driving voltage contributes to acute transformation of the  Au electrode of OTFTs.


Figure 7: (a) OBIRCH picture for the current-induced failure  of an OTFT. The white arrow points toward a green hot spot  location. (b) TEM image shows gate metal rolling and  penetration into dielectric layer at the arrowed site in Fig. (a).


To conclude, several research were addressed in this study and  the principle results indicated that (1) SAM is an effective and  non-destructive technique for inspection and exact localization  of intra-structure void defects; (2) successful leakage  metrology observation of OTFTs is revealed by OBIRCH; (3) ultra-low voltage DB-FIB showed a wonderful cross-section  sample preparation; and (4) we demonstrated that the failure  mode of OTFT induced by high driving voltage was a  particular extension and rolling of gate metal. Although the  present study has yielded findings that have practical  implication, it still has some limitations. This paper is offering


preliminary results of analytic approaches that will be further  analyzed and explored. The topics to be explored in future  research can be listed as follows: (1) Optimum fabrication  conditions prohibit void defects from producing within  dielectric; and (2) The mechanism of OTFTs’ failure resulting  from high driving voltage. We hope that further studies will  provide more detailed results.


This research was funded by project 7301XSY2X0 from the  Industrial Technology Research Institute (ITRI) in Taiwan, R.O.C. I am grateful to whole research participants for their  interest and time.


[1] Jackson, T. N., et al., “Organic Thin Film Transistor for  Organic Light-Emitting Flat-panel Display Backplanes,” IEEE Selected Topics in Quantum Electronics Vol. 4, No. 1 (1998), pp. 100-104.


[2] Rogers, J. A., et al., “Organic smart pixels and  complementary inverter circuits formed on plastic  substrates by casting and rubber stamping,” IEEE  Electron Device Lett. Vol. 21, No. 3 (2000), pp. 100-103.


[3] Rogers, J. A., et al., “Paper-like electronic displays: Large-area rubber-stamped plastic sheets of electronics  and microencapsulated electrophoretic inks,” Proc. Nat. Acad. Sci., Vol. 98, No. 9 (2001), pp. 4835-4840.


[4] M. W. Lee, et al., “Flexible OTFT-Backplane for Active  Matrix Electrophoretic Display Panel,” IMID '07 DIGEST,


pp. 159-161.


[5] Sheraw, C. D., et al., “Organic Thin-film  Transistor-Driven Polymer-dispersed Liquid Crystal  Displays on Flexible Polymeric Substrates,” Appl. Phys. Lett. Vol. 80, No. 6 (2002), p. 1088.


[6] Gelinck, G. H., et al., “Flexible Active-matrix Displays  and Shift Registers Based on Solution-processed Organic  Transistors,” Nat. Mater. Vol. 3, No. 6 (2004), pp.


106-110.


[7] Burns, S. E.,  et al., “A Flexible Plastic SVGA e-Paper  Display,” Disp Devices  No. 44 (2006), pp. 19-20.


[8] Colin Reese, et al., Materialstoday (2004), p. 20.


[9] Tsumura, A., et al., “Macromolecular Electronic Device: Field-effect Transistor with a Polythiophene Thin Film,” Appl. Phys. Lett. Vol. 49, No. 18 (1986), p. 1210.


[10] Burroughes, J. H., et al., “New Semiconductor Device  Physics in Polymer Diodes and Transistors,” Nature Vol. 335 (1988), pp. 137-141.


[11] Tsumura, A., et al., “Polythiophene Field-effect  Transistor: Its Characteristics and Operation Mechanism,” Synth. Meth. Vol. 25, No. 1 (1988), pp. 11-23.


[12] Soren Steudel, et al., “Influence of the Dielectric  Roughness on the Performance of Pentacene Transistors,” Appl. Phys. Lett. Vol. 85, No. 19 (2004), pp. 4400-4402.


[13] F.-J. Mayer zu Heringdorf, et al., “Growth dynamics of  pentacene thin films,” Nature Vol. 412 (2001), pp. 517-520.


[14] Weiss, E.C., et al., “Mechanical Properties of Single Cells  by High-Frequency Time-Resolved Acoustic


Microscopy,” IEEE. Vol. 54, No. 11 (2007), pp. 2257-2271.


Comparative Failure Analysis of Photovoltaic Devices


2381 Zanker Rd. #150 San Jose, CA 95131


Photovoltaic devices (PV) or more commonly “solar cells” are analyzed using LBIC/LBIV (Light Beam Induced Current/Voltage) PL (Photoluminescence) and EL(Electroluminescence) as well as INSB thermal Methods.


This paper will show the advantages and pitfalls of the techniques as well as a novel way to perform EL imaging without a dark box and thermal imaging through glass panels.


Photovoltaic cells are effectively large area diodes with metal electrodes spaced to minimize the loss of fill factor from the light. Popular cell materials are: Silicon, Cadmium Telluride,Copper Indium Selenide, GaAs, Light absorbing dyes (DSSC)and Organic/polymer based cells. [1] Since these cells are covered only minimally by metal, EL imaging can be performed on both crystalline and amorphous versions of the cells. Certain specialized organic thin film cells may not generate an EL or PL signal and can only be mapped thermally to look for ohmic shorts or map the interconnections while biased. LBIC is useful as the local conversion efficiency of the thin film can be mapped but near bandgap light must be used for subsurface defect detection and mapping in the presence of significant shunt resistance may be difficult. Normal (LSM) Laser Scan Microscopes are not very useful, as large areas cannot be readily mapped and the power varies dependent on the scan angle through the optics. The solution is to raster the laser using SIFT (Stimulus Induced Fault Test)[2,3] The SIFT scanner is a large area X, Y, Z positioner that allows the laser to be rastered and positioned over a large area similar to an engraving machine. Since the spot is at a constant location internal to the optics, the power is also constant. Tilt is compensated in all three axes to insure constant power distribution with a constant spot size. This is especially important with laser excited PL imaging and thermal laser injection methods. The raster, spot size, and scan rate are controlled to produce an LBIC or TLS (Thermal Laser Stimulus) scan of the array in a similar but larger scale to OBIRCH or TIVA methods.[4,5]


Sensor and System Considerations


The 3 most common imaging sensors for analysis of photovoltaic technology for EL and PL techniques are Si CCD, MCT and InGaAs. Figure 1 compares typical response characteristics in relation to Si in order to show the small


overlap enabling CCD sensors to be used for EL imaging.


Note the Depletion CCD reaches into the active indirect bandgap region of Si at 1.1 eV or around the 1000nm to 1100nm region. Clearly for EL and PL imaging, the InGaAs or MerCad (MCT) cameras are superior from a performance perspective however the price differential favors CCD as the low cost solution. Typical performance differences place the InGaAs at 60 times more sensitive than CCD making CCD a poor choice for PL imaging, whereas EL imaging is acceptable using longer integration times. Sensor resolution must not be dismissed. Higher resolution is not necessarily better. The system must be matched to the capabilities of the optics in the system. The optics define ultimate resolving power, whereas the sensor array size dictates field of view,NOT resolution. Sensitivity and resolution are inversely proportional. A 500x500 pixel array is 4 times more sensitive than a 1000x1000 pixel array. The light is further subdivided amongst a higher pixel count decreasing sensitivity. This fact is often overlooked resulting in the purchase of megapixel cameras that perform poorly.


Sensor Comparison


400nm500nm600nm700nm800nm900nm1000nm1100nm1200nm1300nm1400nm1500nm1600nm1700nm1800nm


Wavelength (nm)


MerCad


InGaAs QE


Depletion CCD CCD


Si Transmittance


Figure 1. Graph of typical sensor spectral response for CCD,MCT and InGaAs cameras.


Two typical setups are shown for plan view imaging. Figure 2 is a probe station setup on a vibration isolation table with CCD, InGaAs, and SIFT laser scan capabilities. This type setup is useful for analyzing individual cells and smaller modules especially where the electrical connections are missing or require probing. Figure 3 operates from the same control platform with the camera head and interchangeable lenses attached to a portable stand. The stand is motorized for precise control of all 3 axes and can do SIFT scans. This portable configuration can rest on top of a solar panel for close inspection work. The entire microscope head can be mounted on this stand to perform similar work to the probe station but without the benefit of vibration isolation. Dark box environments can be achieved by draping a light blocking


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 149-156


cloth around the setup or using stabilized differential methods described later in the paper. A third configuration is to use a standard tripod for camera positioning.


Fig 2. Probe station equipped with InGaAs integrating camera and scanning laser sources for LBIC and Thermal stimulus.


Fig 3. Portable InGaAs system for cell, module and panel inspection.


Basic Electroluminescence Imaging


Electroluminescence occurs when current flows across a forward biased diode. When the minority carriers recombine,photons are emitted with an energy of 1.1 eV (silicon). The resulting light from the activity of the minority carriers can be collected and imaged. A light emitting diode (LED) is an efficient EL device whereas silicon is not, due to the indirect bandgap. Radiative recombination of electrons and holes is a low probability event due to the large mismatch of momentum between the available electron and hole states. In spite of the inefficiency, EL signals are obtainable with integrating CCD or InGaAs type cameras. Areas where the field is reduced such as proximal to a shunt or a resistive to open interconnect


will result in a corresponding reduction in the EL signal as will surface trap sites (Dangling bonds, contamination, or other lattice defects). The cell or module is biased forward to force current flow through the cell or module. The chosen bias is dependent on the desired effect. For the monocrystalline Si cell in figures 4 and 5, a crack is easily identified that is not seen with visible illumination, the arrows additionally show local areas of missing backside contact to the anode and the top metal finger shows a greatly reduced EL signal for figures 5 and 7. Figure 6 is a magnified view of the scratch resulting in a discontinuity. Note the reduced EL signal along the length of the top finger in figures 4-6.


Fig. 4. Screen shot of InGaAs image with curve for a crystalline photovoltaic. The Photovoltaic has a vertical crack as well as a discontinuity in the upper horizontal finger.


Figure 5. InGaAs EL image taken with 1 second integration.


The cell drive current is 50mA. The arrows show local areas of missing backside anode contact. The top finger has a reduced EL signal due to a discontinuity in the metal finger.


Although the identified crack does not show with visible light,it is easily seen when illuminated in the NIR spectrum. Figure 8 illustrates the effect of illumination off axis (darkfield).


Since Si is relatively transparent at 1064nm, the crack can easily be observed without bias.[6]


Figure 6. Location of scratched cathode finger on the surface of the cell.


Fig. 7: The EL image of dark circle on the left center side of fig 5 is shown magnified here. The EL image is reduced within this zone due to a locally etched backside electrode during processing. The increased resistance results in less recombination in the “hole”.


Fig. 8. Portion of the vertical crack imaged with a ringlight at 1064nm to enhance.


Light Beam Induced Current/Light Beam Induced Voltage


The setup to obtain an LBIC/LBIV (also known as OBIC:Optical Beam Induced Current) image using SIFT will allow a comparison and facilitate an explanation of the scanner. The SIFT scanner does not use traditional laser scanning microscope optics. DUT scan area can be submicron to 7” or more, allowing large areas to be analyzed since the scanners are stepper-based rather than internal optics based. Field of view limitations of objectives on LSM (Laser Scan Microscope) based equipment are eliminated with SIFT as are issues with varying beam power across the raster. The system can be based on either a motorized probe station or microscope stand for field applications. Unlike LSMs, SIFT uses a stationary beam and moves either the stage or the microscope head in a raster scan pattern. Figure 9 is a block diagram of the apparatus. A microscope and stage are equipped with stepper motors to control the X, Y, and Z motion of the scan. Obviously, servo motors or similar linear positioning devices can be used in place of stepper motors. Z control is necessary to control the spot size of the stimulus by focal point methods. Laser based SIFT uses a laser attached to one of the beam ports of the microscope and can be any wavelength compatible with the selected optics. The selected objective, aperture, and focus control spot size.


precision measurements to be taken.


Figure 11 - X, Y, Z measurements


Discussion and conclusion


There is a significant amount of literature discussing the use of  NIR microscopy in materials analysis and medical fields and  of late, there has been growing interest in using these


techniques to view MEMS devices. What has been missing is  a look at the failure analysis and manufacturing verification


possibilities that stem from the application of NIR technology  in the semiconductor industry. The advent of laser scanning


confocal NIR microscopy opens doors for inspection and


failure analysis work viewing features through the backside of  silicon die. With proper sample preparation and the use of


laser scanning confocal NIR microscopy opportunities are


presented allowing the backside viewing of silicon features


without disturbing those features with the more familiar cross  section sample preparation. The backside viewing also opens  doors to delayering and viewing of single die exposed in a


multi-die stack without disturbing underlying materials or


features.


In conclusion, we have affirmed the critical steps needed in


sample preparation for use of NIR microscopy. We have also  demonstrated that, contrary to the majority of the current


literature, silicon samples of 700um plus thickness can be


prepared and successfully imaged using backside laser


scanning confocal NIR microscopy. Finally, with the


advanced 2D and 3D imaging now available using confocal


laser scanning NIR microscopy, we can clearly image and


accurately capture X, Y, and Z and angular measurements


from backside imaged samples.


[1] A. Trigg, “Applications of Infrared Microscopy to IC and  MEMS Packaging,” IEEE Transactions on Electronics


Packaging Manufacturing, Vol. 26 No. 3 (2003)


[2]  V. Lakshminarayanan, “Failure Analysis Techniques for  Semiconductors and other Devices,” retrieved online Jan  2009 from, RF semiconductors,


http://mobiledevdesign.com/hardware_news/radio_failure_analysis_techniques/ (2001)


[3]  M. S. N. Murthy, M. G. Jones, J. Kulka, J. D. Davies, M. Halliwell, P. C. Jackson, D. R. Bull, and P. N. T. Wells, “Scanning Confocal Near-Infra-red Microscopy: a new


microscopy technique for three-dimensional


histopathology,” Engineering Science and Education


Journal, Vol. 240 (1995)


[4]  M. Hazel, and M. Karpman, “Measuring MEMS though  Silicon Caps,” SPIE  Photonics West 2008 (2008)


[5]  T. Hazeldine, K. Duong, “Microsurgery for Microchips – new techniques for sample preparation,” Materials World, Vol. 11 (2003)


[6]  S. Chen, B. Shinseki, C. Barutha, and T. Kha, “Infrared


Imaging and Backside Failure Analysis Techniques on


Multilayer CMOS Technology,” Proceeding of 6th IPFA ’97, Singapore (1997)


Low Temperature O2 Plasma Process for Scanning Capacitance Sample  Preparation.


Donald W. Schulte, Terry McMahon, David D. Hall, Mark Johnson, William Stickle, Craig Sanders, Greg Long, Gary  DeHaan, Ruhua Cai.


Hewlett Packard Company, Corvallis, Oregon, USA.


A novel SCM oxide preparation technique using a low  temperature O2 plasma treatment is presented. Experimental  results demonstrated that oxides of sufficient quality for  scanning capacitance measurement analysis can be obtained on  both top down and epoxy potted polished cross sections. SCM  results obtained from samples processed using the plasma  process were comparable to those obtained using more  common thermal oxide growth techniques.


Introduction (Required)


Sample preparation for Scanning Capacitance Measurement (SCM) requires forming a thin high quality oxide on the  sample surface, typically via a thermal or a wet H2O2 process. A wide range of thermal processes have been successfully used  to grow the oxide, typically requiring temperatures ranging  between 200-400 °C and times ranging from 10 to 60 minutes


[1] [2] [3]. Since the glass transition temperature of many  potting epoxies is well below 200 °C, the high temperatures  used in these thermal treatments can cause difficulty in the  preparation of polished cross section samples due to  deformation of the epoxy and creation of undesirable odors. Care must also be used in the wet H2O2 process since any  exposed conductive epoxy may be etched and re-deposited on  the sample surface [1]. To overcome these issues this paper  presents a novel SCM oxide preparation technique using a low  temperature O2 plasma treatment.


Initial Screening Experiments and Results


To investigate the use of a low temperature plasma treatment  for growth of an SCM oxide, screening experiments were done  to compare the oxide thickness and cleanliness of various  processes. Films grown using typical thermal and wet H2O2 processes were compared with several O2 plasma treatments. Thermal treatments were all carried out on a 400 °C hotplate  in atmosphere under UV illumination and H2O2 treatments  were carried out at room temperature in a wet chemical hood  with a 10 minute UV exposure after processing. The UV  exposure is generally required to reduce trapped charge in the  grown oxide [1]. Plasma treatments were performed using two  different plasma etch systems. The first plasma system tested  was a Techniques MicroRIE Series 800 plasma etcher using an  O2 plasma ash recipe of 15sccm O2 at 350mTorr and 200W.


The second plasma system tested was a PlasmaTherm 790  reactive ion etcher using an O2 plasma ash recipe of 10sccm  O2 at 100mTorr and 150W.


Table 1 – Summary of initial oxide preparation treatment  conditions and results. The plasma treatments grew useful  oxide thicknesses, but resulted in trace metal contamination  on the sample surface.


Initial Treatment Conditions and Oxide Thickness


Treatment


Time (min.)


Oxide  Thick. (Å)


Comments


None


< 2


Hotplate


(400 °C in


atmosphere under  UV Illumination)


900(15 hr)


21


H2O2 Wet Chemical  Soak.


1080(18 hr)


50 Trace Metal  Contamination


82 Trace Metal  Contamination


O2 Ash –


Techniques


(15 sccm O2,


350mTorr, 200W.)


150 Trace Metal  Contamination


12 Trace Metal  Contamination


30 Trace Metal  Contamination


O2 Ash -


PlasmaTherm


(10sccm O2, 100  mTorr, 150W)


30 Trace Metal


Contamination Samples were prepared by clipping coupons from a bare  silicon wafer and then stripping the native oxide with a 30  second dip in 49% HF. Oxides were then grown on each  sample using the treatment conditions and times detailed in  Table 1. After oxidation the samples were analyzed using a  Physical Electronics QUANTERA Scanning ESCA to evaluate  the oxide thickness and look for the presence of surface  contamination. Oxide thickness values listed in the report were  estimated from the ESCA measurements using a simple  overlayer model. For reference the oxide thickness values


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 140-143


obtained by ESCA were compared with variable angle  spectroscopic ellipsometry (VASE) on a few samples. Results  showed similar trends in oxide thickness using each method, but indicated that the oxide thickness measured by the ESCA  was approximately 8-9Å lower than the thickness measured  using VASE.


Results from the initial screening experiment are detailed in  Table 1. The results showed that the 400 °C 60 minute thermal  process produced a clean oxide of approximately 9Å in  thickness. The wet H2O2 treatments also produced clean  oxides, but resulted in thinner oxide layers than the thermal  process. Each plasma treatment condition tested produced an  oxide that was thicker than the 9Å oxide produced by the  thermal process. For most cases the plasma treatment time  required to grow the oxide was significantly shorter than the  standard 60 minute thermal process time. Although the plasma  oxide thickness results were promising, in each case the  plasma treatments also incorporated trace amounts of metallic  contamination on the surface. This indicated that the plasma  processes were sputtering small amounts of material off of the  chamber sidewalls and re-depositing the material on the  sample surface.


Given the promising results from the initial screening  experiment, further experiments were run to optimize the  plasma process parameters to reduce the sidewall sputtering  and minimize surface contamination. The experiments  indicated that the trace metallic contaminants could be  eliminated through a combination of plasma etch chamber  cleaning, reduced etch power and increased plasma process  pressure. Although this eliminated the metallic contamination, there still were small amounts of residual carbon and fluorine  present on the surface.


Table 2 – Carbon and Fluorine contamination and oxide  thickness as a function of plasma processing power. All  samples were processed for 15 min. at 1000mTorr and 20sccm  O2  flow rate.


Oxide Thickness and Contamination as a Function  of Plasma Process Power and Electrode.


Process Conditions


ESCA Analysis Results


Contaminants


Bottom  Electrode


Power (W)


Oxide


Thick. (Å) C (%) F (%)


Si Wafer


5.4


5.9


Si Wafer 100


17


2.4


Graphite


7


11


7.5


Graphite 100


4.3


To minimize the carbon and fluorine contamination two final  sample test runs were done. Each sample was processed at the  1000mTorr chamber pressure with etch power varying  between 25W and 100W as detailed in Table 2. The first set of  samples was processed on the standard graphite bottom  electrode in the system. For the second set of samples, a 20


minute O2 chamber clean process was run with a clean bare  silicon wafer in the chamber to attempt to coat the chamber  sidewalls with a clean oxide. Samples were then placed in the  center of the silicon wafer and processed to help reduce  sputtering from the bottom electrode surface. Table 2 shows that the carbon contamination increased slightly  with increasing etch power and indicated that the presence or  absence of the silicon wafer had no effect on the carbon  contamination. The fluorine contamination was found to be  minimized for the 100W plasma etch condition when the  sample was process on the silicon wafer.


Based on the experimental results, the 100W, 20sccm  1000mTorr process using the silicon wafer on the bottom  electrode produced the least surface contamination and was  chosen as the best candidate for SCM sample preparation. Using these process conditions a final series of samples was  prepared with different processing times to generate a curve of  oxide thickness versus plasma treatment time. The results are  shown in the chart in Figure 1. Figure 1 indicates that a plasma  processing time of ~3-5 minutes under these conditions will  produce an oxide thickness similar to that obtained from our  default thermal process described in Table 1.


Figure 1: Oxide thickness versus plasma process time. Plasma  process parameters used: 100 W, 1000 mTorr, 20 sccm O2.


To determine whether the plasma grown oxide was sufficient  to obtain a good SCM signal, samples were prepared for SCM  analysis with the selected plasma treatment. Samples were  stripped to silicon using 49% HF and rinsed for 30 seconds in  DI water. Samples were then placed in the center of a bare  silicon wafer in the plasma etcher for SCM oxide growth. The  SCM oxide was grown using a 5 minute plasma treatment at  100W, 20sccm O2 and 1000mTorr pressure to approximate  our standard thermal process oxide thickness. After plasma  treatment, the samples were placed under UV light for 10  minutes to help eliminate trapped charge from the oxide. SCM  analysis results showed that reasonable signal and  measurements could be obtained from the samples. Although  the SCM signal was sufficient to provide useful results, it was  somewhat lower than optimal.


To attempt to improve the signal, samples were processed for  an additional 10 minutes in the O2 plasma followed by a 10  minute UV light exposure. The SCM results from the  reprocessed samples showed a strong signal, but indicated that  some trapped charge was still present in the oxide. The  samples were submitted to a 20 minute UV ozone treatment  and re-analyzed. The results showed a strong SCM signal with  no evidence of trapped charge and provided results consistent  with those that could be obtained with our thermal oxidation  process. It should be noted that the additional plasma  processing was done without removing the sample and silver  epoxy from the stainless steel AFM mount, demonstrating the  improved sample processing capability as compared to the wet  and thermal processes.


Analysis of n-type IMEC Calibration Standard.


To provide a more quantitative measurement of the oxide  growth processes, an N-type IMEC SCM calibration sample  was obtained for characterization of the plasma oxide growth  process. Figure 2 shows the dynamic SIMS doping level data  provided with the IMEC calibration standard for reference. The IMEC sample was cleaved in half and each piece was


Level Name


Resistivity (-cm) Standard Dev.


T9L1


4.12e-3


21.28%


T9L2


2.17e-2


9.40%


T9L3


8.64-2


4.82%


T9L4


9.81e-1


4.73%


T9L5


1.05e1


4.31%


Figure 2: SIMS Data provided with n-type <100> T9 IMEC  calibration structures.


mounted to a glass slide with epoxy in preparation for  precision cross section. The epoxy mounted samples were  mechanically polished using an Allied precision cross section  tool. After polish one of the samples was prepared for SCM  analysis by placing it on a 400 °C hotplate for 60 minutes  under UV illumination. The other sample was prepared using  the 15 minute plasma treatment process, followed by a 10  minute UV light exposure.


Figure 3: Optical micrograph showing one n-type IMEC  calibration sample after cross section and thermal SCM oxide  formation. The thermal treatment results in significant  charring and distortion of the epoxy, necessitating additional  sample clean up prior to SCM analysis.


Figure 4: Optical micrograph showing the second n-type  IMEC calibration sample after cross section and plasma SCM  oxide formation. The plasma process results in no apparent  damage to the epoxy, eliminating the need for additional  sample clean up prior to analysis.


Figure 3 shows an image of the sample processed using the  thermal SCM oxide growth process. The image shows the  significant charring and distortion of the epoxy resin that  occurs during the thermal treatment. Due to this, thermally  prepared cross sections typically require additional clean up to  remove the epoxy residue prior to SCM analysis. The charring  of the epoxy resin also results in significant odor during the  thermal treatment, making it preferable to process the samples  in a fume hood or exhaust vent.


Figure 4 shows an image of the other IMEC sample after cross  section and plasma treatment. The image shows that the epoxy  resin is still transparent and appears unaffected by the plasma  treatment. The lack of damage to the epoxy allows the SCM  analysis to be performed without the need for further sample  clean up.


Line scan SCM measurements were made on each sample  using a Veeco Dimension 3100 AFM. Measurements were all  performed using the same bias conditions, frequency and Pt/Ir  AFM probe type. Results from the SCM measurements are  shown in Figure 5. The graph shown in Figure 5 shows that the  data from each sample was well correlated with the doping  levels in the IMEC sample shown earlier in Figure 4. Additionally the data shows that the measurements from each  sample have a similar signal to noise level. Some slight  difference in signal strength is observed on each sample. This  difference is likely due to a combination of tip wear during  analysis, and minor differences in sample roughness, oxide  thickness and oxide properties.


IMEC T9 n-Doped Staircase Standard


-1 1 3 5 7 9 11


Depth, micrometers


Thermal Oxidation


O2 Plasma


Figure 5: SCM analysis results from Silicon n-doped <100> T9 IMEC staircase calibration standard. The O2 Plasma and  thermal oxide growth techniques both produced similar  results.


There has been ample discussion concerning the use of nearinfrared microscopy (NIR) in fields such as medical, materials  science, and more recently in applications aimed toward


micro-electro-mechanical systems (MEMS); however, little


attention has been paid to the application of NIR microscopy  in the verification and failure analysis of semiconductor


memory devices. This paper will present a discussion of NIR  and laser scanning confocal near-infrared microscopy, sample  preparation for NIR microscopy, and emphasize examples of  laser scanning confocal NIR microscopy in the measurement  and failure analysis of silicon samples typical to the


semiconductor industry.


NIR microscopy is successful because silicon is


characteristically transparent to infrared wavelengths longer


than 1100nm. This transparent nature is reduced by factors


such as the thickness and surface finish of the silicon sample  and by the presence of dopants, although only very heavily


doped silicon presents a problem [1, 2]. The silicon


transparency to near infrared wavelengths allows the relatively  clear viewing of features such as under fill or die attach voids, metal layers on the silicon, thru silicon via alignment, and


patterned alignment marks though the silicon. The serendipity  of this method is that targets such as these can generally be


seen without cross sectioning or otherwise disturbing the


objects of interest. This allows an object of interest to be


viewed without the risk of induced secondary damage during  sample preparation.


While standard near-infrared microscopy adds value to the


inspection and failure analysis process, the application of


newer types of equipment and particularly the addition of laser  scanning confocal NIR microscopy opens the door to


additional applications. Standard NIR microscopy offers a two  dimensional or flat view of an object through silicon; laser


scanning confocal NIR adds three-dimensional imaging and


measurement options to the microscopes tool set.


Confocal microscopy makes use of a pinhole filter positioned  in front of the microscope’s photo detector in such a way that  reflected light outside of the focal plane is filtered eliminating  glare issues. Tighter control of the light source, by using a


laser, also reduces sidewall shadowing [3, 4]. The use of


confocal NIR microscopy enables the “ability to make


quantitative measurement of features through the silicon cap ….with an advertized lateral resolution of 0.55um and a


vertical resolution of better than 0.1um” [4]. The improved  resolution allows the accurate measurement of X, Y, and Z  features.


Sample preparation


Since NIR microscopy is more effective if the sample has


been properly prepared, a brief discussion concerning sample  preparation is warranted. While Hazeldine and Duong [5]


discuss the need to thin silicon samples to 80um or less for


viewing with NIR systems, it is our experience that properly


polished silicon samples of greater than 700um thickness will  yield good results using laser confocal NIR microscopy. Chen, Shinseki, Barutha, and Kha [6] point out that substrate


thickness is a significant variant in resolution clarity and


suggest that the silicon thickness is a more important


consideration than doping. While we would not contest these  statements, we would point to our in-house results as reason to  attempt NIR viewing and measurements on thicker silicon


samples.


In the realm of semiconductor manufacturing, silicon die


prepared for encapsulation are typically seen in thicknesses


ranging from greater than 150um to 50um or less. The lower  end of this range places the sample well within a typically


defined vision range for near-infrared microscopy. The upper  end of the silicon thickness range (from 150um to perhaps


750um) is often present in manufacturing and warrants


consideration for viewing using current NIR capabilities. In all  cases, the die preparation often calls for polishing the backside  of the silicon to enhance the through silicon image. After


opening the package to the silicon level, it has proven useful  to use a CMP approach, as described by Hazeldine and


Duong. A relatively hard zero-nap polyurethane pad is used to  avoid edge rounding and retain flatness while polishing


slurries down to 0.1um may be used to produce the necessary  mirror-like, scratch-free final finish.


In practice, a Logitech polishing system is used (other grinders  could be successfully used following the same principles) with  the following steps to expose and polish silicon for backside


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 135-139


near IR imaging (Figure 1 shows preparation area for bottom  die exposure) :


• Remove material using course grind methods to the  level of the die attach material (milling, laser


ablation, or chemical methods might also be used in   this step). If you are planning on thinning the silicon  using a coarse grind method would serve well to


remember that the coarser the grit used in removing  material, the longer the polish procedure will take


when removing scratches from the silicon.


• Mount sample on a fixturing device capable of


adjustment for planer correction as well as total zheight movement of the sample. (If available, the use  of a Moiré leveling device, optical flat or flat edge


parallel strip may speed setup and assist in


maintaining planarity.)


• Remove die attach material and expose the backside  of the silicon die using 15um (or coarser) slurry on a  metal plate. Removal at this point may also be


accomplished using a variety of grinding or milling  techniques. Care should be taken not to extend this  process into the silicon die.


• Remove expose and clean the backside of the silicon  die using 3 micron cerium-oxide on a hard


polyurethane pad as described above.


• Final polish the die with a 0.5 micron cerium oxide  polishing agent.


Figure 1 – Sample prep area for bottom die exposure


Throughout this process, care must be taken to maintain a


reasonable degree of die planarity, which ultimately relates to  a uniform focal plane across the silicon. It is also advisable to  restrict down pressure during the polishing process. Excess


down pressure may cause material to be removed at a more


rapid rate than had been intended and could lead to


preparation caused damage to the silicon. The polishing


process produces a sample that can be viewed with minimal  defocus across the die. It also minimizes the occurrence of


secondary damage to the sample caused by the sample


preparation process.


Sample imaging and measurement


A novel imaging opportunity is found using the confocal laser  scanning NIR microscope to look through some types of die


attach materials. (Several NIR instruments are available for


failure analysis type work. The images shown in this paper


were captured using an Olympus LEXT-OLS3000-IR scope.) While this is not possible with all materials, it is certainly


worth consideration when using one of the more transparent


die attach tapes or compounds.


Figure 2 demonstrates the clarity of this view and


demonstrates it visibility with the scope looking through


~30um of die attach material at the top surface of a patterned  die. This capability may open a path for delayering stacked die  by removing unwanted layers and stopping at the die attach


level immediately above the die of interest. Using this method, we are able to view features on the target die with minimal


disturbance of the silicon and metal layers. Also of interest for  failure analysis work is the right side of the image showing air  bubbles trapped in under the die attach to silicon layer.


Figure 2 - Imaged through ~30um die attach material


The image in Figure 3 shows traces and bond pad sites and is  viewed through a thin surface layer of oxide material and


750um of silicon die material. This image demonstrates the


functional use of NIR scanning laser microscopy when


viewing thick silicon samples and oxide materials.


Figure 3 - Bond Pads - 750um silicon with oxide


The view in Figure 4 shows the same sample with the oxide


layer removed by polishing with a 0.5um cerium oxide slurry  as described in the sample preparation portion of this paper. A  comparison of the two images demonstrated the capability of  the NIR microscope to image through thick silicon samples


and suggests that while other variables (i.e., the addition of


dopant materials to the silicon) will affect the imaging


capability, attempts at viewing through thick silicon may be


rewarding for the user.


Figure 4 - Bond Pads - 750um silicon no oxide


Figure 5a and 5b demonstrate the 3D imaging capability of the  NIR scanning laser microscope. This view shows a trace to via  area captured using a 50x lens through the polished 750um


thick silicon sample. This magnification level allows larger


surface areas to be viewed while still allowing for an


appropriate amount of detail in the captured image.


Figure 5a - 3D via features - 750um no oxide


Figure 5b – 3D image


Figure 6 is a backside scanning view of metal layers viewed  through a 150um thick silicon die polished with 3um diamond  compound. The mirror finish allows good visibility of the


feature even through silicon thicknesses that are often


described in literature as being undesirable [1].


Figure 6 - 150um die polished with 3um diamond


Figure 7 shows metal layer features viewed through a 70um  silicon wafer. The sample has been prepaired by polishing


with .5um cerium oxide on a hard polypropolene pad. Just


right of center, this view also shows an obvious die crack


extending full thickness through the die.


A compairison of image quality between figure 5 and figure 6  demonstrates the improved imaging capability that results


from a more finely polished surface.


Figure 7 - 70um die showing features and die crack


Figure 8 is a 90x magnification, 3D view of the die crack also  seen in 2D image Figure 6. Of particular interest with this 90x  lens is the inclusion of an adjustable focus ring on the lens.


This feature allows the lens to be focused to matched to the


thickness of the silicon material be viewed. The focus feature  allows clearer imaging at high magnification and reduces or  eliminates the occurrence of fringing in the image.


Figure 8 - 70um die showing features and die crack


Figure 9 demonstrates the ability to view die attach voids, or  air bubbles, trapped in die attach material located between two  silicon die. The voids are clearly visible and are seen in both  image figures 8 and 9 as circular features. (It is important to


remember that voiding may also appear in any irregular


patterned image.) Depending on the process step, the use of


NIR confocal laser microscopy offers alternative or secondary  approaches to determining die attach material coverage and/or  voiding. Where applicable, NIR microscopy offers a less time  consuming method of inspection than acoustic microscopy.


Figure 9 – die attach voiding.


Figure 10 shows a 50x view of alignment marks on an upper  and lower silicon sample and is used to verify x and y


alignment during equipment setup. While this is the same


view often available from equipment NIR alignment sensors, the addition of measurement capabilities allows engineers to  verify the distance of x and y alignment offset and facilitates  program correction to correct the offset problem. In Figure 8, a 20x view was first captured then the measurement option


was used to create distances 1, 2, 3, and 4, which are used to  calculate the existence and amount of x and y offset


Figure 10 – Die on wafer alignment verification


Figure 11 demonstrates typical X, Y, Z measurement


capabilities using the NIR laser confocal microscope. This


image was captured looking through the backside silicon of a  packaged sample with 150um die. The package was ground  open from the backside and the die was then mirror polished. 3D image capture capabilities and clear imaging allows


The microcontroller handles X-Y-Z positioning, stimulus,sensor feedback and communicates with the tester. The controller also optionally manages the bias circuit. Scans are initiated by selecting start and end corners and the step interval for the scan. The smaller the step interval, the greater the resolution of the scan generated mage. Laser spot size is managed by the diffraction limit of the selected objective in conjunction with the focus. Scan time is then calculated as the total number of steps multiplied by the step delay (settle time).


As a side note, gas CO2 lasers can be mounted in place of the microscope (glass optics are not compatible) and raster scanned over large areas for thermal SIFT. CO2 lasers are chosen due to low cost, power and desired wavelength for thermal stimulus. The laser does not generate recombination in common photovoltaic materials and is a long enough wavelength (low energy photons) to be more readily absorbed by the substrate than the more traditionally used 1340nm laser for silicon. The change in resistance, voltage, or current of the cell, as desired, is monitored during the scan and overlaid with the reflected image. Thermal laser mapping is beyond the scope of this paper but is mentioned here for follow on work in relation to the SIFT scanner description.


The stimulus can also be introduced over the DUT with the raster applied to the stage. This method of SIFT can be thought of in the same way a probe is positioned over a DUT by moving the stage.


accumulated camera frames. Typically gains of up to 60X can be realized with typical 12 bit InGaAs cameras.


Shunts can be identified in series/parallel wired panels by imaging at different drive current levels. The panel is an 18x42 inch monocrystalline panel rated at 4 amps and 60 Watts with a Voc of 20V. The panel slipped past production into the field. In figure 18, top image, the panel was imaged at 2A using 1/30 sec integration and a simple background subtract. Note the 2 cells 1 weak and 1 dead at location 4,0 and 4,1 (8 cells across by 9 cells high). The current was reduced further to 1A for the center image. Now the 2 cells at 4,0 and 4,1 are both dead with all the cells above in the same column appearing brighter. The dead cells must have shunts causing greater current to flow in column 4 and less in parallel wired column 3. Note column 3 is indeed darker and location 8,4 is suspect. Reducing the current down to 140 mA in the bottom image the lower level shunt leakages begin to dominate in several areas. The intensity is too low to acquire without increasing the integration time but the sensor will saturate due to ambient light conditions. To solve this, the stabilized mode was used for acquisition with 256 frames and 16 frames per state at 1/30 second integration time.


Fig 18. 18x42 inch solar panel InGaAs EL image. Top image is with 2A drive current and 1/30 second integration time.


Middle image is with 1A drive current and 1/30 second integration time. Bottom panel is with 140mA drive current and 1/30 second integration time with 256 frames


accumulated in stabilize mode to extract the signal. Each column has 9 cells wired in series. Each column pair is wired in parallel with the parallel pairs wired in series. In EL mode the current will divide between the pairs as becomes evident at 140mA. The middle module from the rightmost column is cracked.


Figure 19. EL image of cracked adjacent cells identified in the rightmost column (8,5) from figure 18. Note the edge shunt leakage on the lower cell from contamination.


Figure 20. Magnified view of the crack in EL mode from figure 19. Note the mating piece where the crack originates has an irregular cut. The dicing operation is to blame for this failure.


Unfortunately, the original sites in column 4 are not understood at this point and visual inspect is negative for the root cause. The goal is not to destroy the panel until the data is understood. The suspected shunts should show up thermally, as will be shown in the next section.


InSb Investigation of the Solar Panel


The panel was set up and imaged from across the room with the InSb camera on a tripod. The panel is complete with a glass faced window and upon imaging the warm vertical panel, the image in figure 21 was obtained. Not surprising since glass absorbs fairly well in the 3um to 5 um band.


Stabilized thermal imaging will not work unless the frame rate is reduced to about 0.1 Hz due to the slow thermal diffusion anticipated through the glass to the surface. In this case, only a differential approach was required based on the strength of the signal, however, stabilized would have been used if warranted. The thermal image is now clear where the shunts are located. The shunt at (8,4) is due to edge contamination as correlated by the EL image in figure 19. Note the crack is not the shunt. The 3 sites at the bottom of column 4 are caused by the series interconnect strap touching the cell edge between the 2 cells.


Figure 21. 18x42 inch solar panel imaged with an InSb camera at ambient. The hot end of the panel on the left is actually the top part where heat is rising. Note the cells cannot be seen behind the glass and removal of the glass would be destructive. Units are Celsius.


Figure 22 Differential thermal image in degrees C of the 18x42 inch solar panel imaged with an InSb camera after applying 1A for 5 seconds. Compare the identified shunt leakage to Figures 18 and 19. Note the cells can now be“seen” behind the glass since the difference image is being collected on the glass face from heat injected below.


Several case studies of photovoltaic cell and module failures have been shown with emphasis on cross correlation to obtain corrective action. Stabilized imaging has been used to identify low level thermal shunts and has demonstrated how to obtain EL signals without a dark box. Different power levels allow identification/understanding of the nature of the leakage. PL mode can be used to characterize unfinished product. Dopant profiles can be calibrated to the PL signal and minority lifetimes characterized locally. LBIV was shown with constant power, tilt corrected scans on large area panels to


obtain QE surface data. Finally, InSb 3um to 5um imaging technology was demonstrated through glass with differential thermal analysis.


To my wife Mayra for her devotion and patience with my continuing to burn the candle at both ends.


1. http://www.solarserver.de/wissen/photovoltaik-e.html


2. J. Colvin,”Functional Failure Analysis by Induced


Stimulus” ISTFA/2002 Proceedings, pp. 623-630.


3. U.S. Patent # 7323888 B1 “System and Method for Use in Functional Failure Analysis by Induced Stimulus,”Colvin; James B.


4. R. Aaron Falk,”Advanced LIVA/TIVA Techniques”ISTFA/2001 Proceedings, pp. 59-65.


5. U.S. Patent # 6,078,183 “Thermally-induced voltage alteration for integrated circuit analysis,” Cole, Jr.;Edward I. Sandia Corporation (Albuquerque, NM)


6. J.B. Colvin United States Patent US6134365: Coherent Illumination System and Method.


7 O. Breitenstein, et al, “Fault Localization and Functional Testing of ICs by Lock-in Thermography”, Proc. 28th ISTFA, pp. 29-36, 2002.


8. D.L. Barton, “Thermal Defect Detection Techniques”,ASM Microelectronic Desk Reference Fifth Edition,pp.378-397, 2004.


9. J. Colvin,”Moire Stabilized Thermal Imaging”,IPFA/2005 Proceedings, pp. 163-166.


Analysis of poly-Si thin film solar cells by IR-LBIC


M. Boostandoost, H.-P. Lin, U. Kerst, C. Boit


Berlin University of Technology, Institute of Radio Frequency and Semiconductor System Technologies  Section Semiconductor Devices


Einsteinufer 19, Sekretariat E2 D - 10587 Berlin, Germany


mahb@mikro.ee.tu-berlin.de, Tel.: +49-30-314-29947


S. Gall


Helmholtz-Zentrum Berlin für Materialien und Energie  Institute Silicon Photovoltaics


Kekuléstrasse 5, 12489 Berlin, Germany


The carrier collection properties of polycrystalline Si (poly-Si) thin film solar cells on glass with interdigitated mesa structure  have been locally analysed with Infrared Light Beam Induced  Current (IR-LBIC) and compared to LBIC measurements  using visible light. The low absorption of IR light leads to a  low current level when the light is coupled vertically into the  active volume. An enhanced carrier collection has been  detected at the corners of the mesa because the etch allows to  couple the light horizontally into the solar cell, This  investigation shows that IR-LBIC is sensitive to light trapping  structures in silicon based thin film solar cells.


1) Introduction


The photovoltaic market is still dominated by wafer-based Si  solar cells (mono- and multi-crystalline Si). So far the well  established Si thin film technologies are based on amorphous  Si (a-Si:H) and microcrystalline Si (μc-Si:H). Polycrystalline  Si (poly-Si) thin film solar cells on glass feature the potential  to combine the advantages of both Si wafer technology (i.e. high material quality) and Si thin film technology (i.e. low  costs) [1].


In this paper, IR-LBIC (Infrared Light Beam Induced  Current), which is well established technique in the  community of microelectronic devices, is applied for  investigating poly-Si thin film solar cells on glass.


In LBIC, a laser beam is scanned over the device and the  photocurrent induced by the laser beam is monitored. The  variations in the current collection are correlated with the  position of the laser leading to current map (LBIC image). In  Integrated Circuits, this image can display the location of  buried diffusion on the sample or can also result from defects  associated with the junction [2]. In the solar cell community, LBIC is used for profiling the cell performance, e.g. caused by  diffusion length variations. Since it is performed under short  circuit conditions, the dark I–V characteristic of the sample  does not influence the result.


For IR-LBIC measurements a laser beam with the wavelength  in IR range but below the wavelength of the bandgap energy  of silicon (1.1eV) is used. We have used the wavelength of  1064nm to implement IR-LBIC measurement. The IR-LBIC  measurement provides the information about the solar cell  spectral response for photons close to the silicon band gap, which is especially interesting in thin film cells because of the  low absorption rate. We will show in this paper that IR-LBIC  can provide information about the light trapping structures in  Si thin film solar cells.


2) Setup


Light Beam Induced Current (LBIC) measurement has been  performed using two different wavelengths, 532nm and  1064nm to investigate the thin film solar cells and obtain  information about their properties and the surface texture. Hamamatsu PHEMOS 1000 has been used for implementing  IR-LBIC measurement as depicted in figure 1. Main  components of this setup include laser scanning microscope (LSM), DC power supply, and current monitoring unit  including amplifier, laser light source, image processor and  display. The solar cell sample has been placed on the sample  stage and its terminals have been contacted using microprobe  heads and needles.


The PHEMOS 1000 combines laser (1064nm) stimulation and  light emission microscope with a silicon cooled CCD camera  as a detector for acquisition of extremely faint emission in  range of visible and infrared wavelength [3]. Table 1 shows  the measured laser power, spot size of laser (1064nm) and  laser power density depending on the objective. Laser power  can be varied from 0.1-100% of maximum power using the  PHEMOS 1000 software. The maximum output power for all  the lens magnifications have been measured using a power  meter. Spot size of laser is calculated numerically, considering  the numerical aperture (NA) of the optical system and the  laser wavelength. Current changes caused by IR-LBIC are  usually very weak and therefore need to be amplified before it  can be used for imaging purposes. This is the main function of  OBIRCH amplifier to amplify the signals. The PHEMOS


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 157-161


1000 system has the signal amplifying unit consisting of  voltage and current sources and amplifier and can provide up  to 100x voltage amplification.


Figure 1: Measurement setup used to perform IR-LBIC  technique


Objective   agnification


Measured  Laser Power


[mW]


Laser  Spot Size


[m]


Power density


[mW/m2]


5x


31,6 – 36


9,3


0,46 – 0,52


20x


21,9 – 24,3


3,2


2,7 – 3,02


100x


2,9 – 3,3


2,6


0,54 – 0,62


Table 1: Measured laser power, laser spot size and laser  power density depending on the objective


The Laser Scan Controller, as the basic component of the  image processing unit in the PHEMOS 1000 system, controls  the scanning procedure of the laser beam via line and frame  signals. A laser scanning microscope (LSM) micrograph can  be superimposed to the light emission or laser stimulation  image.


The LBIC measurement of 532nm stimulation wavelength has  been performed at the Helmholtz Zentrum Berlin. The Laser  power is about 50mW and the laser spot can be focused to  5m area using a reflective lens. The reflective objective  x36/0.5 has been used which provides 36X magnification.


We have also used FEI 830 DualBeam equipment to perform  cross sectioning and trenches for investigation of the sample  structure and material characterization. The dual beam  incorporates both a Focused Ion Beam (FIB) column and a  Scanning Electron Microscope (SEM) in a unit.  This  combination enables to view the cross section face using the  electron beam while the ion beam mills normal to the sample  surface.


3) Devices


The poly-Si thin film solar cells under investigation are  formed as it is depicted in figure 2.


The preparation of the poly-Si thin film solar cells starts with  the formation of a thin (about 200nm) large-grained poly-Si  seed layer on glass (Borofloat 33 from Schott) using the  aluminum-induced layer exchange (ALILE) process [4].


Subsequently the highly doped poly-Si seed layer (p+-type) is  thickened epitaxially by high-rate e-beam evaporation [4].  The thickness of the epitaxially grown p-type poly-Si absorber  layer is about 2μm. Then a plasma hydrogenation step is  applied to passivate defects [5]. The p-n-junction is formed by  the deposition of a thin (about 10nm) n+-type a-Si:H emitter  layer using plasma enhanced chemical vapor deposition (PECVD).


Figure2: Preparation of poly-Si thin-film solar cell on glass


To improve the lateral current transport a 80nm aluminumdoped zinc oxide (ZnO:Al) layer is deposited as a transparent  conductive oxide (TCO) onto the a-Si:H emitter. No Light  trapping structures are included, i.e. the solar cell surface is  smooth. The area of the solar cell is defined by photolithography and subsequent mesa etching. During wet  chemical mesa etching the ZnO:Al layer, the n+-type a-Si:H  emitter and (partly) the p-type poly-Si absorber are removed. Due to the high etching rate the ZnO:Al layer is not only  etched off in the areas which are not protected by the  photoresist but also partly below the photoresist (undercut of  the photoresist). Finally interdigitated front (emitter) and rear (base) contacts are formed (Al). The cross section of the final  solar cell structure is shown schematically in figure 3.


Figure 3: Schematic structure of a poly-Si thin-film solar cell  on glass (cross section)


Figure 4 shows an optical micrograph (in reflection mode) of  the solar cell surface taken with PHEMOS 1000. The size of  the solar cell is 4mm*4mm. The bright bands aligned in  horizontal direction in figure 4 are the front contact fingers (Al), which are electrically connected to ZnO:Al layer. These  fingers are surrounded by a dark area (the p-n junction  covered with the TCO layer) and a gray area (the p-n junction


without TCO layer). The interdigitated rear contact fingers (Al) are also at the front side. The red vertical line in this  figure marks the position of the cross section in figure 3.


Figure 4: Optical micrograph (in reflection mode) of a poly-Si  thin film solar cell (Top view)


The current-voltage (I-V) characteristic of a poly-Si thin film  solar cell is shown in figure 5. The low current in forward bias  and relatively high current in reverse bias indicate that the p-n  junction has relatively weak electrical characteristics.


-5,E-03 0,E+00 5,E-03 1,E-02 2,E-02 2,E-02 3,E-02 3,E-02 4,E-02


-3 -2,6 -2,2 -1,8 -1,4 -1 -0,6 -0,2 0,2 0,6 1 1,4


Voltage[v]


Figure 5: I-V characteristics of a poly-Si thin film solar cell


4) Results


A typical LBIC measurement at a wavelength of 532nm is  shown in figure 6.


Figure 6: LBIC map of a poly-Si thin film solar cell (Laser wavelength: 532nm)


The inhomogeneous signal distribution is representing the  variations of the carrier collection in the part which is covered  with the TCO layer.


The IR-LBIC measurements using a laser with a wavelength  of 1064nm show a much weaker signal response from the area  covered with the TCO layer as expected for poly-Si thin film  solar cells using a laser with a wavelength of 1064nm. However, in contrast to the LBIC measurement, relatively  strong IR-LBIC signals are observed at the mesa corners (see  Fig.7).


Figure7: IR- LBIC map of a poly-Si thin film solar cell


(Laser wavelength: 1064nm). The IR-LBIC map is


superimposed to a micrograph using objective with 5x  magnification.


Using 20x magnifications (Fig.8), the inhomogeneous  distribution of the weak IR-LBIC signal over the TCO  covered area is clearly visible. This picture also shows in more  detail that at the mesa corner, the IR-LBIC signal is much  stronger than from the area that is covered with TCO.


Figure 8: IR- LBIC signal (laser wavelength: 1064nm)


superimposed to an optical micrograph using objective with  20x magnification. The corresponding cross section is also  shown.


In order to investigate the origin of the strong IR-LBIC signal  at the mesa corner, an SEM (Scanning Electron Microscopy) micrograph (Fig. 9) has been taken, providing a better view at  the sample surface at the mesa corner. This picture is taken  using the DualBeam system when the sample is tilted to 52°.


The rough surface on the bottom part of the picture is the pdoped poly-Si region (obtained by mesa etching) and the  smooth surface on the top part is the highly n-doped  amorphous silicon surface. The wet etching process has led to  the relatively rough surface of the poly-Si film.


Figure 9: SEM image of the surface of the poly-Si thin film  solar cell. The sample is tilted by 52°


Figure 10 shows cross section of the transition from a-Si top  to etched poly-Si after FIB preparation, in order to investigate  the etching profile. The position of the cross section is  indicated with a yellow vertical line in figure 4. g A more  precise image of the etching profile is shown in the cross  section of this area that is shown.


For FIB cross sectioning, protection of the sample surface has  been provided by a local platinum deposition, visible as a  bright top layer on the cross section, around 1μm thick. As the  sample is tilted, the gray line within is indicating the corner  from vertical to horizontal surface orientation. Above that  line, the top down view is showing the surface structure  visible in figure 9 now with higher magnification.  The rough  surface of the poly-Si can be seen on the right side of the  picture and the smooth surface of amorphous silicon on the  left.


Figure 10: FIB processed cross section using E Beam  imaging with 52° for the poly-Si thin film solar cell


The next layer with the thickness of 2438nm at the left side of  the picture in figure 10 shows the poly-Si layer. At the mesa  corner its thickness reduces smoothly and reaches the final  thickness of 1402nm at the right side. Therefore the etching  profile is not as ideal as is shown in figure 3; it rather shows a  continuous thickness variation in the length of about 10m to  reach the final thickness. The gray line, which is shown with  red arrow in figure 10, is indicating the transition from poly-Si  layer to the glass substrate.


This cross section is also evidence of a very rough poly-Si  surface after etching.


The reason of the IR-LBIC signals at the mesa corner can be  explained by the geometrical profile of the light trapping  property of the poly-Si surface after etching process, which  allows light to be diffracted into horizontal direction while  hitting the etched surface. The absorption coefficient of  silicon decreases with increasing the wavelength. The  absorption coefficient of silicon at the wavelength of 1064nm  is about 67cm-1 and for the wavelength of 532nm is about  10197cm-1 [6]. As it is depicted in figure 11, the scattered  light can travel in horizontal direction up to 440m and in  vertical direction just up to 2m.


Figure 11: Light scattering at the mesa corner of a poly-Si  thin film solar cell


Therefore according to Beer–Lambert law for 1064nm, the  maximum light absorption in horizontal direction along the pn junction can be about 99.5% and in vertical direction, there  is almost no light absorption. These two parameters, the rough  profile at the mesa corner after etching process and small  absorption coefficient at this wavelength (1064nm) allow the  incident light to penetrate the structure horizontally and  generate many more electrons and holes along the absorption  path than in vertical direction. By stimulating with visible  light (532nm), the absorption is very effective even at very  short vertical path, about 87%, whereas the coupling from the  side will not lead to increased signals at the mesa corner, as it  is shown in figure 6.


We have performed the LBIC measurement in IR range with a  wavelength of 1064nm and compared the result with a typical  LBIC measurement (532nm). The main difference using IR  light is the low absorption rate due to photon energies only  slightly above the semiconductor bandgap. In thin film solar  cells, this results in a very low current induction when light  transmission is vertical. Light trapping structures are  diffracting the light into horizontal direction which has a large  dimension also in thin film cells. This leads to a comparably


large induced current as overall absorption is high. This makes  IR-LBIC an excellent indicator of light trapping properties in  thin film solar cells.


The authors thank Hamamatsu KK Japan and Germany for  support; many thanks go to Thomas Unold and Markus Wendt  of Helmholtz Zentrum Berlin (HZB) for performing the LBIC  measurement and Pinar Dogan from HZB for providing the  poly-Si thin film solar cell.


[1] “Crystalline Silicon on Glass (CSG) Thin-Film Solar Cell  Modules”, M.A. Green et al., Solar Energy 77, pp.857-863, 2004


[2] “Failure Analysis of Integrated Circuits Tools and


Techniques Series”; Lawrence C. Wagner, The Springer  International Series in Engineering and Computer


Science, ISBN. 978-0-412-14561-2, Vol. 494, pp.216,


1999


[3] PHEMOS series General catalogue, Emission Microscope  PHEMOS Series, Cat. No. SSMS0003E07, 2008


[4] “Polycrystalline silicon thin-film solar cells on glass“, S. Gall, C. Becker, E. Conrad, P. Dogan, F. Fenske, B. Gorka, K.Y. Lee,B. Rau, F. Ruske, B. Rech, Solar Energy  Materials & Solar Cells 93 , pp.1004–1008, 2009


[5] “Hydrogen passivation of polycrystalline Si thin films by  plasma treatment”, B. Gorka, B. Rau, K.Y. Lee, P. Dogan, F. Fenske, E. Conrad, S. Gall, B. Rech, Proc.of  the 22nd European Photovoltaic Solar Energy Conference, Milan, Italy, pp. 2024-2027, 2007


Figure 9. Block Diagram of SIFT Scanner.


Image reconstruction is obtained as the sample is scanned point by point. There are 8 amplifiers available to measure signals such as the reflected laser signal for the background image formation and the modulated voltage or current signal from the DUT. These signals are superimposed on the reflected signal data, if desired, during the scan. Typically LBIC is a measure of the small signal voltage developed across a resistor tied between the anode and cathode of a cell.


The value of the resistor needs to be large and properly chosen. In many instances the cell leakage is considered the resistor and the developed voltage is measured directly at the terminals with a high impedance amplifier (LBIV). This has the advantage of providing shunt leakage information from series wired cells. Compare the LBIC signal in figure 10 to the EL data obtained in figures 4-7. Note the crack is the only surface anomaly shown at the 654nm wavelength.


Fig 10. LBIC scan of a Monocrystalline Si cell at 654nm.


Note the crack running up the cell above the micron scale bar,the other subsurface anomalies are not revealed from figure 5.


An amorphous Si panel on a glass substrate was investigated with EL and LBIV methods. EL imaging revealed anomalies with the backside electrode in figure 11. The LBIV scan shows the actual cell-to-cell local conversion efficiencies as shown in figure 12. Figure 13 is an averaged line plot profile from figure 12. When performing LBIV on series cells, the impedance load is of a rather high impedance, otherwise the adjacent series cells will reverse bias. Under these conditions,any local leakage within the specific cell in the chain will reduce the signal and as such serves as the built in shunt for the LBIV signal. With a high impedance measurement, all other cells will appear as a short, since the measured voltage associates only with the cell being stimulated. If an external resistive shunt is used, the cells must be connected individually rather than in series for LBIC mode.


Fig. 11. EL image of a forward biased amorphous Si panel at 22V and 8mA of forward current. Note the holes in the signal near the center due to backside electrode disparities.


Compare to the LBIV image in figure 12.


Fig. 12. Large area LBIV scan of an amorphous silicon module on glass photovoltaic. The LBIC signal reveals the cells with the best conversion efficiency and highlights local surface disparities. Backside contact issues are not revealed.


Figure 13. Profile graph from figure 12 of a large area LBIV scan on an amorphous silicon module on glass photovoltaic.


The LBIV plot reveals the cells with the best conversion efficiency.


Stabilized Luminescent and Thermal Imaging


Traditional thermal imaging methods typically utilize a background reference image with no bias, and then a subsequent biased image is acquired and compared. The length of time to acquire is typically seconds, resulting in thermal propagation across the cell during signal acquisition diluting a useful result. Using stabilized mode, sensitivity will be shown to be far superior to IR camera imaging methods and does not suffer the sqrt(2) noise increase and hence 2X amplitude loss inherent in lock in thermography systems(LIT). [7,8]


This method of acquisition controls synchronously to the camera frame rate the thermal propagation, (stabilizes the substrate temperature with interleaved bias pulses) while building up the thermal signal to enhance the thermal sensitivity. This work was originally published for Moiré pattern thermal mapping. [9]


Referring to equation (1) the difference signal is built up using a summed sequence of frames from state 1 and state 0. For Stabilize 1x, the Device Under Tests (DUT) alternates between States 1 and 0 for every frame. For Stabilize 2x, the DUT alternates between States 1 and 0 every 2 frames, and so on. Stabilize can run any binary multiple. The absolute value is used as a “catch all” for both 0 and 180 phase situations.


Thermal shifts increasing or decreasing are mapped but the polarity is, of course, lost. The flags controlling absolute value and polarity: (state 1 sum – state 0 sum) or (state 0 sum– state 1 sum) can be toggled during acquisition to force a recalculate and display.


Equation (1)


Using Stabilize 4x as an example, at 30 frames/second it becomes apparent that the thermal propagation will be 4/30 second on and 4/30 second off for a cycle time of 3.75 Hz.


The frame groups of on and off (State 1 and State 0) are accumulated in an interlaced fashion and displayed to allow the analyst to watch the signal grow and to stop the acquisition


at sufficient intensity. The end result will be N accumulated frames in packets of 4. The interface can trigger with a test sequence in slave mode or drive the modulated power directly to the device. This stabilize method of acquisition is also compatible with FMI (Fluorescence Microthermal Imaging).


The ability to visualize and control the propagation per unit time gives insight as to the location and nature of the defect and its surroundings.


A normal polycrystalline cell was investigated to demonstrate the sensitivity of the technique for figures 14-17. Compare the EL image in figure 14 to the high gain thermal image in forward and reverse bias for figure 16. The 2 spots in the center are diffusion anomalies based on their presence restricted to forward bias modes. The PL image, in figure 17,was obtained using a 670nm excitation source with the InGaAs camera and a longpass filter close to the bandgap of silicon to reject the 670nm signal component to the camera.


Note the similarities to the EL signal from figure 14. PL data yields information on the minority carrier lifetime. Trap sites such as dangling bonds are revealed with PL imaging.


Experimental material without electrodes can be evaluated with PL since the “bias” is the high-energy photon beam impinging on the surface generating hole electron pairs and subsequently recombination at the bandgap of the material studied. The n or p material can be examined individually during process development making PL a powerful process development/monitor technique.


Fig. 14. EL image taken with the InGaAs camera. 500msec.


at 200mA drive current.


Figure15. Curve in reverse bias mode to identify low-level hot spots using the InSb camera in stabilized thermal mode. See figure 16.


Figure16. INSB thermal images of a typical cell with 1024 frames and 256 gain at 3.75 Hz modulation (4X Stabilize).


Upper Image is Reverse bias at 734mv and 5ma. Lower image is forward bias 735ma at 352ma. The shunt is weak in the enhanced upper image.


Figure17. Photo luminescent image taken with the InGaAs camera using a flood source of 670nm to irradiate the surface of the unbiased cell. A longpass filter was used to minimize leakage. Note the similarity to the EL image in figure 14.


Large area solar panel analysis


One of several challenges with EL and thermal imaging is the size of the area to be investigated. A dark box is not necessarily practical for solar panels. The stabilized luminescent method above is implemented using frame acquisition with modulating power to the panel. By capturing frames in alternating on and off states, the background illumination can be differentially removed allowing the remaining EL signal to be viewed and quantified. Since the integration times for the camera are shorter, camera requirements are less stringent since camera defects are differentially removed from the image, a fringe benefit of the technique. The upper limit is based on the S/N of the


The RBD approach is powerful, as it allows a block diagram to  be created with deeper and deeper levels based on the level of  failure data available.  Figure 3 demonstrates the third of six  levels currently in the RBD model for the system of interest.


Figure 3: RBD of PV Array, level 3 of 6.


O&M data are collected from the field, including component  failure, failure mode (if known), date of failure, time to repair, etc.  The data are then sorted by component and failure type, and the failure statistics are determined. Two basic  approaches to PV Life Data Analysis are employed:


Life Data Analysis


o Ranks goodness-of-fit to common life distributions


o For components that are replaced (PV Modules, fuses, etc.)


o Failures are independent


Parametric Recurrence Data Analysis


o Power law & repair effectiveness factor


o Components that are repaired (Inverter)


o Failures may not be independent


Life data are fitted to five distributions: Exponential one  parameter, Exponential two parameter, Weibull two parameter, Weibull three parameter, Lognormal. The life distribution  selection criteria used include:


goodness of fit (the p-value from the Kolmogorov-Smirnov  test), the maximum absolute difference between the  hypothesized and empirical cumulative distribution functions (cdfs)


a likelihood ratio,  the value of the log likelihood of the  hypothesized distribution with the estimated parameters  evaluated with the given data set, and


plot fit, the mean absolute difference between the  hypothesized and empirical cdfs.


Maintenance and repair data are similarly analyzed. The  failure and repair distributions are then fed into the RBD and  component and system reliability predictions can be made. Table 2 provides a summary of the time to failure analysis  for components that are replaced as an example of the analysis  used.


Table 2. Time to Failure Analysis for Replaced Components


Repair  Results


PV Comp/   RBD Block


Distribution


Beta or  Log SD (Shape)


Eta or


Log


Mean or  Lambda  (Scale)


Gamma


AC disconnect Weibull 3-RRX


0.35


11000


3.9


Lightning


Exponential 1-RRX


0.00022


Row Box


Weibull 2-RRX


0.51


1.2E+06


PV Module


Weibull 3-RRX


0.28


5.2E+12


480/34.5 KV Weibull 2-RRX


0.58


7100


208/480


Transformer Weibull 3-RRX


0.15


1.3E+10


28


Marshalling  Box


Lognormal 2-RRX


2.3


Figure 4 is an example of the calculated reliability of each  component and the ultimate system reliability predictions  based on one year of data for this system.


Figure 4: Modeled PV array component and system reliability  as a function of time for 5 MWdc grid-connected photovoltaic  systems


In this system, the inverter has the lowest reliability, which  drives the system reliability.  However, the inverters are  repairable and were well-maintained. Figure 5 shows the  cumulative and instantaneous mean time between failures for  the inverters for five years in the field, demonstrating  predictable reliability growth is occurring with field repair by  finding problems and applying fixes to all the inverters.


Although the field failure and maintenance data are necessary  for predicting system-level reliability, the uncertainty in the  predictions is large when no accelerated life test data or  component degradation data are included.  The system-level  reliability and lifetime predictions can be greatly enhanced by  including component-level failure data generated as described  in the component section.


Figure 5: Modeled inverter MTBF as a function of time for 5  MWdc grid-connected photovoltaic systems


Understanding reliability of PV components and systems is  currently a focus area for DOE and the PV community.  The  long life times required (20-30 years), the conditions (outdoors  in extreme climates), the rapid changes in technology and the  cost of PV systems make gathering quantitative reliability  statistics challenging.  Expanding reliability assessment and  failure analysis techniques for components and systems can  enhance the reliability of PV systems, which is necessary for  large-scale deployment of PV as a power generation source.


Sandia is a multiprogram laboratory operated by Sandia  Corporation, a Lockheed Martin Company, for the United  States Department of Energy’s National Nuclear Security  Administration under contract DE-AC04-94AL85000.  Sandia  acknowledges the support of the DOE Solar Energy  Technologies Program in particular for the work presented  here.


[1] King, D. L., et al., “Photovoltaic Array Performance  Model,” Sandia internal document SAND 2004-3535.


[2] Cameron, C. P., et al., “Comparison of PV System  Performance-Model Predictions with Measured PV  System Performance,” Proc 33rd IEEE Photovoltaic  Specialists Conference, San Diego, CA, May 2008.


[3] International Standard IEC 61215, “c-Si Terrestrial  Modules Design Qual and Type Approval,” 2005


100.00


1000.00


10.00


10000.00


ReliaSoft's RGA 6 PRO - RGA.ReliaSoft.com


Cum. and Instant. MTBF vs Time


5/6/2009 11:24 Sandia Labs


Mike Mundt


Power Law


Data 1


Fielded-Repair MLE


CMTBF IMTBF


CB[C] 90%


1-Sided-B [T2]


Beta=0.7471, Lambda=0.0186


Time [hours]


PV System Reliability vs. Time


Expected


reliability of


components and


the system


based on utility


PV data


[4] International Standard IEC 61646, “Thin Film terrestrial  photovoltaic (PV) modules – Design qualification and  type approval,” 2008


[5] International Standard IEC 62108, “Concentrator Module  Qualification Standards,” 2008


[6] UL1741, “UL Standard for Safety for Static Converters  and Charge Controllers for Use in Photovoltaic Power  Systems,” Underwriters Laboratories, First Edition, May  7, 1999, Revised Jan 2001


[7] Bower, W., et al., “Performance Test Protocol for  Evaluating Inverters Used in Grid-Connected Photovoltaic  Systems”,


available


for


download


at


http://www.bewengineering.com


[8] Wohlgemuth, J. H. et al., “The Effect of Cell Thickness  on Module Reliability,” Proc 33rd IEEE Photovoltaic


Specialists Conference, San Diego, CA, May 2008.


[9] Granata, J. E., et al., “Long-term Performance and


Reliability Assessment of 8 PV Arrays at Sandia National  Laboratories,” Proc. 34th IEEE Photovoltaic Specialists


Conference, Philadelphia, PA, June 2009.


[10] Gonzalez, S., et al., “Long-term Inverter Operation


Demonstration at Sandia National Laboratories,” Proc


34th IEEE Photovoltaic Specialists Conference, Philadelphia, PA, June 2009.


[11] Sorensen, N. R, et al., “The Effect of Metal Foil Tape  Degradation on the Long-Term Reliability of PV  Modules,” Proc. 34th IEEE Photovoltaic Specialists  Conference, Philadelphia, PA, June 2009.


[12] Kempe, M. D. et al., “Accelerated Stress Testing of  Hydrocarbon-Based Encapsulants for MediumConcentration CPV Applications,” Proc 34th IEEE  Photovoltaic Specialists Conference, Philadelphia, PA, June 2009.


[13] Moore, L. M. et al., “Five Years of Operating Experience  at a Large, Utility-Scale Photovoltaic Generating Plant,” Prog. Photovolt: Res. Appl, (2007)


[14] Collins, E., et al., “Reliability and Availability Analysis of  a Fielded Photovoltaic System,” Proc. 34th IEEE  Photovoltaic Specialists Conference, Philadelphia, PA, June 2009.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 171-176


•


• •


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 177-181


(α)


(β)


μμ μ


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 182-188


Ω


μ


≥


=


Ε


∫


⏐  ⏐


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 189-192


Case Study: Failure Analysis of Functional Shmoo Hole with Laser Voltage  Probing


SH Lee, YW Lee, KT Lee, CY Choi


Samsung Electronics Co. Ltd., Ki-hung, South Korea  Sukho.lee@samsung.com 82-17-341-1407


HW Shin


NEOSEM Inc., Su-won, South Korea


Yin S Ng, TR Lundquist


DCG Systems, Inc., Fremont, CA, USA


Innovations in semiconductor fabrication processes have  driven process shrinks partly to fulfill the need for low power, system-on-chip (SOC) devices. As the process is innovated, it  influences the related design debug and failure analysis which  have gone through many changes.  Historically for signal  probing, engineers analyzed signals from metal layers by  using e-beam probing methods [1]. But due to the increased  number of metal layers and the introduction of flip chip  packages, new signal probing systems were developed which  used time resolved photon emission (TRE) to measure signals  through the backside. However, as the fabrication process  technology continues to shrink, the operating voltage drops as  well. When the operating voltage drops below 1.0V, signal  probing systems using TRE find it harder to detect the signals


[2]. Fortunately, Laser Voltage Probing (LVP) technology [3] is capable of probing beyond this limitation of TRE. In this  paper, we used an LVP system to analyze and identify a  functional shmoo hole failure. We also proposed the design  change to prevent its reoccurrence.


With the development of SOC techniques, an increasing  number of different and complicated functions can be  integrated into a single device solution, creating an entire  system within a chip, hence System-on-Chip. But as a result, it  has been difficult to proceed with the related design debug and  failure analysis because of the resulting complexity in the  device. In recent years, EDA design tools and design  engineering skills have rapidly improved such that it is very  rare that one encounters an outright device malfunction or  gross functional failure. Instead, parametric failures or soft  failures in which the device only fails at certain parameters are  prevalent, and these types of failures are hard to detect using  simulation tools. Low or high Vcc fails are examples of these  parametric failures and are seen as an anomaly in shmoo plots.


It is due to these types of failures that design debug techniques  have evolved to supplement certain limitations of simulation  tools. In this paper, we mainly discuss the method of approach  to the failure analysis of a parametric failure seen at low Vcc  and the result of this analysis.


In general, there are two types of test patterns for verifying  functionality.


1.  In Built-In-Self-Test (BIST), inputs (data and control  signal) to a functional block can be generated  internally, and outputs of the functional block are  synthesized into test result which then can be sent out  through flag signals.


2. In a full functional test, input signals are externally  generated and can be fed through the data path and  output signals can be compared to the expected data  from simulation result


In the former case, failure analysis involves a more  complicated procedure as knowledge of the BIST synthesis  algorithm is required. In an SOC where many blocks of  circuitry are integrated together, it is common to have a 3rd party BIST in which this knowledge may not be readily  available. However, in the latter case, the failure analysis is  easier as the data path and its simulated signals to, along and  from the functional block of interest is known. Focus can be  immediately put into tracing the data path of the functional  block in question. Fortunately for this paper, the latter test  pattern can be used for verification. By probing of the data  path of this functional block in question using the binary  search method, the localization to source of the failure can be  done. Once localized, further analysis of the signals can  provide insight to the electrical root cause of the failure.


LVP is a backside optical probing technique used to extract  waveforms from internal transistors. A pulsed laser is directed  at the transistor under measurement, and the changing charge  density due the electrical activity modulates the laser as it  passes through the active and gate regions of the transistor. The laser is reflected back to the LVP system by the various  layer interfaces within the DUT. As a result, the reflected laser


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 193-197


contains timing information directly related to the electrical  activity in the DUT.


Problem description


The device used in the paper was from a 65 nm process  technology SOC solution for mobile Digital TV (DTV) applications in a variety of mobile devices. Fig 1 shows the  functional blocks under analysis. The operation of these  blocks was tested by using full-path functional test. There  were no constraints requiring BIST implementation such as  limited I/O pins and low-cost testers. Additionally, the data  port in each of the functional blocks in Fig. 1 must interface  with another functional block. It is for these reasons that the  full path functional test was implemented. Other  considerations for implementing full-path functional test were  test time reduction for mass production and also to best  simulate the device in actual operation.


Demodulator


Mode Detector


Equalizer


TPS


FEC


CSI


Phase rotate


Data in


Data out


Figure 1: Diagram of Functional Block under evaluation


It was during this full-path testing with a production tester that  the problem was first observed. An anomaly in the shape of a  hole was observed in a 1-dimensional search of operating  voltage.  Later, with a shmoo plot, it was found that the hole  was 2-dimensional as it occurred as a function of frequency as  well as voltage.  This same shmoo hole happened on about  80% of the devices in 2 or 3 different lots so we could assume  that this shmoo hole failure was possibly a design issue. Further, 65 nm has been a stable process for mass-production; there had been no particular fab yield issues.


The first hurdle in the debug is narrowing the problem to a  specific high-level functional block. Since each functional  block under investigation could be directly stimulated  externally, specific test vectors for debugging purposes were  generated to independently test each block with the intention  of observing the shmoo plot of each of these tests. A Catalyst  Tester, the same tester used for production, enabled specific  test vectors to be readily generated for our LVP analysis. From  the results of these tests, it was observed that the demodulator  block shared the same anomaly (hole) in the shmoo plot as the  full-path functional test. The shmoo plot of the other  functional blocks did not contain any anomalies.


The demodulator functions to demodulate an RF signal  modulated by a carrier frequency. An external transmitter


transmitting the RF signal (consisting both video and audio  data) needs to modulate this RF signal with a carrier frequency  to preserve signal integrity and prevent signal distortion. The  internal RF receiver receives this modulated RF signal, and an  internal ADC digitizes it. The demodulator then converts this  digital modulated signal to the original RF signal. In this  analysis, using the specific test vector for debugging the  demodulator, the input to the demodulator was sent from I/O  pins rather than the ADC.


As per the required design target, the demodulator should  operate at 80 MHz within the operating voltages of 1.08 V to


1.32 V. However, as operating voltage was reduced towards


1.08 V, functional fails started occurring for a certain range  before the functional fails stopped, causing the hole in the  shmoo plot. The range of operating voltages, in which the  functional fails occurred, varied with the operating frequency, creating a 2-dimensional hole in the shmoo plot as shown in  Fig. 2.


80MHz


1.08V


Figure 2: Shmoo plot with anomaly (hole) for both full  functional test & demodulator test.


Failure Analysis


With additional tests, it was possible to confirm that the source  of the failure was within this demodulator block. The failure  analysis then proceeded to backside signal probing, using LVP  technology, in order to pinpoint the source of this shmoo hole  failure.


Backside analysis required some sample preparation. The  original production package type was a front-side BGA, which  could not be used for backside analysis. A special LQFP  package had been developed for the purpose of these backside  analyses. Additionally, since a Solid Immersion Lens (SIL) [4] was being used in the backside analysis, the silicon had to be  thinned down to 100 m; this thinning was done in the wafer  production line prior to the LQFP packaging.


U_CORE


U _DEMOD _MUX


U_DEMOD _IN _MUX


U_DEMOD _TOP


inst _7


inst _8


inst_80


inst_87


inst _83 inst _1726


1,250 n


2,200n


under 300 n


inst _95


inst_82


Ins t 87


B H D


Figure 3: Block diagram of demodulator


The demodulator block consists of instances shown in Fig. 3. The goal was to trace the signals along the data path of the  demodulator. However, if the signals along the data path are  traced sequentially forward from its beginning or backwards  from its end, the amount of time spent would be long  depending on where the source of the failure actually was. Therefore, as the source of the failure was unknown and hard  to guess, a binary search along the data path reduced the  analysis time.


The cells in the data path consist of both D flip-flops and  buffers. Wherever possible signal acquisition was taken at a  buffer due to its relatively large size and its strong modulation  of the LVP’s probing laser. However, as the binary search  narrows, there may not be an option to choose between a D  flip-flop or a buffer. At 65 nm process technology, the  transistors within a D flip-flop are spatially dense, requiring  high spatial resolution probing. It is for this reason that a LVP  system with a SIL is used for this analysis. Fig. 4 below shows  an image of a D flip-flop and its LVP signals.


Figure 4: LSM image of the CLK input inverter and Q output  driver and their corresponding Signal Acquisitions of a 65nm  D flip flop


At each point of the search, signals were acquired in both  passing (1.2 V) and failing (1.08 V) operating voltages. The


data signal at 1.08V is compared to the data signal at 1.2V to  determine if the data signal at 1.08V is failing or passing at  that particular point. Starting the search of the data path at  point A, a failing signal was acquired, while at point B, the  signal was what would be expected. This indicated that there  was no need to analyze the data path before point B. Narrowing down the search, signals were then acquired after  point B.  At point D, a failing signal was detected. It was then  obvious that the source of the failure was located between  points B and D. Continuing the search, the source of the  failure was localized in the data path between points B and H, (see Fig. 5) in which there was a single instance of a D Flipflop.


Figure 5: Signal Acquisition at points B & H in the  demodulator’s data path


Once localized to a single cell instance, all inputs to the cell  were validated. In this case of a D Flip-flop, with the input  data already validated during the binary search at point B, the  next input to validate was the clock signal. As shown in Fig. 6, signals were acquired at the D & CLK inputs and Q output of  the flip flop and an extra pulse was detected in the CLK signal. At 1.08V, the extra pulse on the CLK signal latches the low  level of the D input, hence causing the output Q to drop to low  prematurely. With the device set to a passing operating  voltage of 1.2V, and observing the non-existence of the extra  pulse in the CLK signal, it was determined from the failure  analysis thus far that the functional shmoo hole failure was  caused by the extra pulse at the CLK signal of this flip-flop in  the demodulator block.


1.2V Pass


1.08V Fail


POINT H


POINT CB


1.2V Pas s


CLK


Q


Figure 6: Signal Acquisition at source of failure in the  demodulator’s data path.


In order to trace the root cause of this extra pulse, the analysis  moved to the source of the CLK; the clock generation block. The CLK signal is a gated clock being controlled by a flip-flop (Gated CLK F/F) at the clock generation block. Focusing the  analysis on this Gated CLK F/F, a glitch was observed at the  D input as shown in Fig. 7. The failure happened when the  glitch occurred in the proximity (in time) of the rising edge of  the Gated CLK F/F’s clock. The clock latches the erroneous  glitch at the D input and consequently, the generated clock  contained an extra pulse.


From Fig. 7, the glitch at the D input existed even in higher  passing operating voltages. As the operating voltage was  lowered, the glitch shifted left towards the clock’s rising edge  till the failure occurred. Further reduction in the operating  voltage would further shift the glitch to the left to a point  where the glitch moved away from the rising edge—hence the  cause of the ‘hole’ in the shmoo.


1.12V_pass  D


1.08V_fail D


1.06V_fail D


1.04V_pass  D


1.12V_pass  CK


1.08V_FAIL CK


1.06V_fail CK


1.04V_pass  CK


400ps


Figure 7: Signal Acquisition at the clock generation flip-flop (Gated CLK F/F).


The results shown in Fig. 7 show that the failing signals  exactly matched the identified anomaly (hole) of the shmoo. These results were fed-back to the design team.


Design Review


The D signal for the Gated CLK F/F is generated by an “OR” operation of SYM_EN and Counter signals as shown in Fig 8. The falling edge of SYM_EN occurs slightly before the rising edge of the Counter signal, causing a condition a race condition between these 2 signals. The glitch happens at this  time.


Gated Clock F/F D :


SYM_EN + Orignal Clock


Glitch!!


Gated Clock F/F CK Counter


SYM_EN


SYM _EN


Counter


Gated LK F/F D Gated LK F/F CK


Figure 8:  Timing diagram of the clock generation block


As a solution to this problem, a delayed SYM_EN signal is ‘OR’ed together with the original signal at the D input  containing the glitch. This removes the glitch to the Gated  CLK F/F D input as illustrated in Fig. 9.


Gated Clock F/F D


Gated Clock F/F CK Counter SYM_EN


Delayed SYM_EN  New Gated Clock F/F D


Figure 9:  Timing diagram of the corrected clock generation  block


Ideally, timing simulation needs to be done for each critical  path implemented in the design. However, when a certain  design is implemented several times within a device, the  timing simulation may only be done for a single  implementation. All other implementations would assume the  same timing simulation. In this case, the design of the ‘OR’-ed  SYM_EN and Counter signals was implemented in both a different functional block and the clock generation block  within the demodulator functional block. The timing  simulation was done for the other functional block and this  glitch was observed. However, no errors were flagged because  in this timing simulation, the glitch was relatively far from the  rising edge of the clock. An assumption was made that this  timing simulation applied to the demodulator function as well. However, based on the results of the failure analysis, the  timing simulation of this design implementation in the  demodulator functional block was then done, and the results  showed a glitch occurring near the rising edge of the clock; an  exact match to the results of this analysis.


Using the LVP system, signals were probed from transistors  operated at ~1.0 V. With these signals, we were successful in  completing the functional shmoo hole failure analysis. What  were critical to the success of this failure analysis were the  ability to measure the signals at low operating voltages within  a short amount of time, the ability to achieve the spatial  resolution required to probe within a 65nm flip-flop and the  ability to detect a 400 ps glitch which was the root cause of the  failure.


The LVP technology should continue to provide signal  probing solutions as fabrication process technologies  continues to shrink to 45 nm and 32 nm where operating  voltages are even lower. The high bandwidth performance of  the LVP systems provides for analyzing signals like the “glitch” reported on here.


[1]  J. L. T. Thong, Electron Beam Testing Technology. New  York: Plenum, 1993.


[2] Chi-Lin Young, Paul Ng, “Ultra low voltage probing on  45nm CMOS by Time Resolved Emission (TRE) Technology”, ASM-ISTFA 2007, p.161


[3] Yin S Ng, W Lo, K Wilsher, “ Next Generation Laser  Voltage Probing”, ASM-ISTFA 2008, p. 249


[4] “Aplanatic Microlens and Method for Making Same” US  Patent 5,282,088, granted 1/25/1994; “Bi-Convex Solid  Immersion Lens”, US Patent 6,594,086, granted  1/15/2003; “Bi-Convex Solid Immersion Lens”, US  Patent 6,778,327, granted 8/17/2004; “Bi-Convex Solid  Immersion Lens”, US Patent 7,227,702, granted 6/5/2007.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 198-201


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 202-207


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 208-213


−


μ        − =


=    =    =


±


= ⋅


= + +


−   −


−  −


μ×


− +


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 214-216


° °


°


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 217-221


In a solar module about 36 cells are connected in series in socalled strings. The current flowing through all cells is the  same, but the cell biases are floating. Only if all cells have the  same illuminated current-voltage (I-V) characteristics, they are  all operating at the same working point and their generated  voltages simply add up. However, if one of these cells should  be shadowed or broken, leading to a reduced photocurrent of  this cell, the other cells may bias this one in reverse direction  to up to -18 V. If then a large reverse current flows, which may  be as large as the short circuit current of the other cells (typically 7 A), this cell dissipates a lot of heat and the module  may be destroyed thermally. According to its base doping  concentration of 1016 cm-3, a solar cell should undergo  avalanche breakdown at -60 V. However, in reality breakdown  may occur already at -10 to -15 V. Therefore the electric  breakdown behavior of solar cells is an important reliability  aspect and must be studied in detail.


The two breakdown mechanisms discussed in literature are  avalanche breakdown (impact ionization) and internal field  emission (Zener breakdown) [1]. Avalanche breakdown is the  generation of electron-hole pairs by the impact of accelerated  carriers. It is characterized by the multiplication of  photocurrents in the breakdown sites. It shows a negative  temperature coefficient (TC) of the current for a fixed bias, since at high temperature phonon scattering quenches the


impact efficiency. Zener breakdown, on the other hand, is  direct tunneling of carriers through the energy gap. It shows no  multiplication of photo-induced carriers and its TC is positive, since the gap shrinks with increasing temperature. This  mechanism is more probable than avalanche only at high  doping concentrations above 1018 cm-3, where the breakdown  voltage is in the order of -6 V. The probability of all  breakdown mechanisms increases with increasing net doping  concentration. For a base doping concentration of 1016 cm-3 as  in our solar cells, breakdown should occur by avalanche at  voltages beyond -60 V. However, it is well-known that local  breakdown may occur already at lower reverse bias if the p-n  junction is not flat but curved, leading to a local increase of the  electric field.


In this investigation the dominant breakdown sites in industrial  multicrystalline Si solar cells are localized by lock-in  thermography (LIT) under reverse bias. Special LIT  techniques allow us to image the temperature coefficient, the  slope (steepness) of the breakdown current variation with  voltage, and the avalanche multiplication factor locally. The  distribution of grown-in recombination-active crystal defects is  obtained by electroluminescence (EL) imaging. By using  different electron microscopy techniques, the physical origin  of the dominating breakdown mechanism in the investigated  cells is identified.


Typical Breakdown Characteristics


Fig. 1 shows the reverse dark current-voltage characteristic of  the investigated cell at two temperatures. For this investigation  a typical 156x156 mm2 sized industrially produced solar cell  made from solar-grade multicrystalline silicon was selected, which was free of significant ohmic shunts. Weak (soft) breakdown starts already at -6 V and hard breakdown occurs  beyond -13 V. As Fig. 1 shows, in the hard breakdown regime  the current shows a negative temperature coefficient (TC), as it  is known from avalanche breakdown, whereas in the soft  breakdown regime (below -13 V) the TC is positive. Already  this observation points to the presence of different breakdown  mechanisms acting in different bias ranges.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 162-165


-14 -12 -10 -8 -6 -4 -2


0 200 400 600 800 1000 1200


25°C  80°C


reverse bias  [V]


Figure 1: Reverse bias I-V characteristic of the investigated  cell at two temperatures.


Electroluminescence Imaging and Bias-Dependent Lock-in  Thermography


In the forward-bias electroluminescence (EL) image Fig. 2 (a) regions containing recombination-active crystal defects are  visible as dark areas, which are mainly grain boundaries and  dislocations. Four interesting regions are labeled by 'A', 'B', 'C', and 'D'. In lock-in thermography (LIT) the locally dissipated  heat in a device is imaged [2]. The two LIT images Fig. 2 (b) and (c), taken at reverse biases of -12 and -15 V, show that at  different biases different breakdown sites dominate. At -12 V


(b) the breakdown sites strongly correlate with dark regions of  recombination-active defects in (a), see e.g. in regions 'A' and 'B'. It can be noted that, on the average, in regions with a  strong dark EL contrast also stronger breakdown occurs and  vice versa. At -15 V, however, new breakdown sites appear in  regions without recombination-active defects, see regions 'C' and 'D'. Note that Fig. 2 (c) is scaled very insensitively, hence  the currents in (c) are much higher than in (b).


Figure 2: (a) Forward-bias EL image of this cell, (b) reversebias LIT image at -12 V, (c) reverse-bias LIT image at -15 V. Note the different scaling ranges in (b) and (c).


Imaging Physical Breakdown Parameters


If the LIT signal being -90° phase shifted to the bias pulses is  displayed and the cell has no series resistance problems, the  LIT signal is a quantitative measure of the locally flowing  current density and can be scaled in units of mA/cm2 [2]. Then, by subtracting two current density images taken at  different biases at the same temperature, or at different  temperatures at the same bias, respectively, and dividing by  the bias / temperature difference, images of the local biasdependence (slope) or of the local temperature coefficient (TC) of the local current can be obtained. Since these values  are still dependent on the absolute magnitude of the current  flowing, it is useful to relate them to the mean values of the  local currents. In this way images of the relative slope (steepness, given in % current change per Volt) and the  relative TC (given in % current change per Kelvin) are  obtained, which allow to image the basic physical parameters  of breakdown sites quantitatively [3].


Figure 3: (a) Slope at -12 V, scaled from 0 to 100 %/V, (b) slope at -13.5 V, scaled from 0 to 150 %/V, (c) temperature  coefficient, measured at -14 V, scaled from -3 %/K to +3 %/K,


(d) avalanche multiplication factor at -15 V, scaled from 1 to


3. (a), (b)  taken at 60 °C, (c) at 70 °C. (d) at room  temperature.


Fig. 3 (a) shows such a slope image belonging to a bias of  -12 V, scaled from 0 (black) to 100 %/V (white, see color bar). This image again correlates well with the EL image Fig. 2 (a) in that regions 'A' and 'B' appear bright. Note that at this bias  the breakdown site 'C' is not visible yet but site 'D' is. Fig. 3 (b) shows a slope image belonging to a higher bias of -13.5 V, scaled to 150 %/V. Here also the site 'C' appears, but 'A' and 'B' appear relatively weaker, since their slope is lower (soft  breakdown). In the TC image Fig. 3 (c) taken at -14 V all sites  of steep breakdown (e.g. 'C' and 'D') appear dark, hence they  show a negative TC. However, breakdown sites 'A' and 'B'


(b) -12 V, 15 mK


(c) -15 V, 800 mK


(a) slope -12 V


(b) slope -13.5 V


(c) TC -14 V


(d) MF -15 V


show a close-to-zero TC (red), hence here obviously another  breakdown mechanism is active. This becomes obvious in Fig. 3 (d) which shows the local avalanche multiplication factor (MF) at -15 V, scaled from MF = 1 to 3. For obtaining this  image, the bias of -15 V was permanently applied to the cell  and the cell was illuminated homogeneously in a pulsed  manner. Then the lock-in signal is a measure of the locally  flowing photocurrent and also can be scaled in units of  mA/cm2. Note that the dark breakdown current, which is  visible in Fig. 2 (b) and (c), does not influence this  photocurrent image, since it is steady-state. It turns out that, at  reverse biases between zero and -13 V, the photocurrent image  is nearly homogeneous, but at higher reverse bias regions of  avalanche multiplication appear bright. By dividing the  photocurrent image taken at a certain bias V (here -15 V) to  one taken at a lower bias (here -13 V), a quantitative local  image of the avalanche multiplication factor MF at bias V can  be obtained [3]. The MF image Fig. 3 (d) shows that only the  regions with the steepest slope at -13.5 V (e.g. 'C' and 'D') show significant avalanche multiplication, but the regions of  defect-induced breakdown (e.g. 'A' and 'B') do not.


Electron Microscopy


The question is: What are the different physical mechanisms of  breakdown in these different regions? For answering this  question, scanning electron microscopy (SEM) has been  applied at the interesting sites, including lock-in EBIC (electron beam-induced current) imaging under high reverse  bias [4]. For this investigation only lock-in EBIC is  appropriate, which is working with a pulsed beam and an a.c.-coupled current amplifier, since any d.c.-coupled amplifier  would be overloaded by the strong steady-state breakdown  current. While in regions 'A' and 'B' nothing special could be  seen, in region 'C' at a reverse bias above -13 V lines and spots  of bright EBIC signal appear, see Fig. 4 (a). Such sites are  traditionally called microplasma sites. In these regions fieldinduced avalanche multiplication of beam-generated minority  carriers occurs. In the SE image Fig. 4 (b) in these sites black  spots are visible (see arrows), which in higher magnification


(c) can be identified as conical etch pits. Note that this cell was  acidically textured, which is standard for modern solar cells  since this texturization works independent of crystal  orientation. The recipe of this texture is actually chosen to  avoid the appearance of etch pits, but obviously some types of  defects still generate them.


In Fig. 4 (c) a pair of etch pits is shown which obviously is  connected by a planar defect, maybe a stacking fault. The  region between the arrows in (c) was processed into a TEM  lamella by focused ion beam (FIB) preparation. The resulting  TEM image is shown in (d). Here we see that the tips of the  etch pits are really sharp (radius about 20 nm) and that they are  indeed caused by dislocation-like defects. The exact type of  this defect is yet under investigation. Since in these cells the pn junction is lying about 300 nm below the surface, at these  tips the junction should be bowl-shaped with a radius of 300  nm. Sze and Gibbons [5] have calculated the avalanche  breakdown voltage for bowl-shaped p-n junctions and have  found that, for a net doping concentration of p = 1016 cm-3 and


a radius of 300 nm, the avalanche breakdown voltage indeed  reduces from about -60 V (for a flat junction) to -13 V, which  was also found by us for breakdown in regions 'C' and 'D'. Hence, by these investigations we have successfully identified  the mechanism being responsible for the "hard" breakdown  e.g. in regions 'C' and 'D' as an avalanche breakdown, with the  field being enhanced by the tip effect at the bottom of the  observed etch pits. The measured negative TC of this  breakdown current fits to this interpretation. It is  understandable that this effect is observed mainly in regions  where no high density of recombination-active defects is  observed, since for avalanche effect clean material is necessary  for enabling a large scattering path length of the carriers.


Figure 4: (a) Lock-in-EBIC image at -15 V in region 'C' showing microplasma sites, (b) corresponding SE image, (c) detailed SE image of single microplasma sites, (d) TEM cross  section of this site after FIB preparation between arrows in (c).


Discussion and Conclusions


The origin of the defect-induced breakdown e.g. in sites 'A' and 'B' is less clear yet. It has been shown by Lausch et al. [6] that this type of breakdown also occurs at a flat surface. Many  authors have discussed the influence of defects like  dislocations on the avalanche breakdown voltage, but this  influence was meant to be basically due to a field increase by  the presence of charged defects. Then also the defect-induced  breakdown should show a negative TC and should lead to  avalanche multiplication, which, however, was not observed in  regions 'A' and 'B'. Therefore, we believe that for this  breakdown electronic gap states of the defects are responsible. This hypothesis is supported by our observation that there is a  correlation between the recombination activity of these defects  and the magnitude of the breakdown current. It was also  observed that only weak defect-induced breakdown sites show  some 1.55 μm defect-induced luminescence, but strong ones  do not [7]. This can be explained by a different degree of  contamination of the defects, leading to different densities of  deep defect states. One of our hypotheses is that trap-induced


tunneling might be the mechanism responsible for defectinduced breakdown. This mechanism is physically related to  internal field emission (Zener effect, tunneling through the  gap), which is actually improbable at a doping concentration  as low as 1016 cm-3. However, if the tunneling occurs not  through the whole gap but in two steps via mid-gap states, this  mechanism would become much more probable. Actually, as  for the Zener effect, we would expect a positive TC for this  mechanism, since the gap energy reduces with increasing  temperature. However, in Fig. 3 (c) we have measured a closeto-zero TC in regions 'A' and 'B', which is not completely  understood yet. Therefore another hypothesis is that the  mechanism is a kind of "trap-assisted avalanche". Since a gap  level may be occupied either by an electron or a hole, in a trapassisted avalanche process the impact should lead to  subsequent electron and hole emission with a certain delay  time in between. This might be the reason why this process  shows no significant multiplication of photo-generated  carriers. At least it seems to be clear that this defect-induced  breakdown becomes stronger with increasing degree of  contamination of the defects. Therefore it may become the  dominant breakdown mechanism if upgraded metallurgical  grade (UMG) material is being used instead of gas-phase  purified silicon for solar cells in future.


This work was financially supported by the German Federal  Ministry for the Environment, Nature Conservation and  Nuclear Safety and all the industry partners within the research  cluster SolarFocus (0327650 D). The content of this  publication is the responsibility of the authors.


[1] Mahadevan, S., Hardas, S.M., Suryan, G., "Electrical  Breakdown in Semiconductors", Physica Status Solidi (a) Vol. 8 (1971), pp. 335-374


[2] Breitenstein, O., Langenkamp, M.: Lock-in  Thermography - Basics and Use for Functional  Diagnostics of Electronic Components, Springer (Berlin / Heidelberg / New York 2003), ISBN 3-540-43439-9


[3] Breitenstein, O., Bauer, J., Wagner, J.-M., Lotnyk, A., "Imaging Physical Parameters of Pre-Breakdown Sites by  Lock-in Thermography Techniques", Prog. Photovolt: Res. Appl., Vol. 16 (2008), pp. 679-685


[4] Bauer, J., Wagner, J.-M., Lotnyk, A., Blumtritt, H., Lim, B., Schmidt, J., Breitenstein, O., "Hot spots in  multicrystalline silicon solar cells: avalanche breakdown  due to etch pits", Physica Status Solidi RRL Vol. 3 (2009), pp. 40-42


[5] Sze, S.M., Gibbons, G., "Effect of junction curvature on  breakdown voltage in semiconductors", Solid-State  Electronics Vol. 9 (1966), pp. 831-845


[6] Lausch, D., Petter, K., v. Wenckstern, H. Grundmann, M., "Correlation of Pre-Breakdown Sites and Bulk Defects in  Multicrystalline Solar Cells", Physica Status Solidi RRL, Vol. 3 (2009), pp. 70-72


[7] O. Breitenstein, J. Bauer, J.-M. Wagner, H. Blumtritt, A. Lotnyk, M. Kasemann, W. Kwapil, W. Warta: Physical  mechanisms of breakdown in multicrystalline silicon solar  cells, presented at IEEE Photovoltaic Specialists  Conference (PVSC), Philadelphia, June 2009, proceedings in preparation.


Approaches to Photovoltaic Systems Reliability


Jennifer E Granata, Elmer Collins, Mike Mundt, N. Robert Sorensen and Michael A. Quintana


Sandia National Laboratories, Albuquerque, NM, USA   jegrana@sandia.gov


The increasing demand for clean energy, renewable energy, and energy independence has generated a rapid expansion in  the photovoltaic (PV) industry in the last 3-5 years.  Although  crystalline silicon PV technology has been in use for more than  30 years, PV has remained a “cottage industry” until the recent  expansion.  Thin film and concentrating PV technologies have  added to the market. Overall component and system  performance levels have risen.  What is missing in this  expanding industry, with 20-30 year lifetime expectations in  harsh outdoor environments, is a solid understanding of  component and system-level reliability.  This paper will  provide an introduction to the current issues of reliability in  the PV field and the work the Department of Energy’s Solar  Energy Technologies Program (DOE SETP) is focused on to  address these issues.  In particular, the work of the Reliability  Programs at both Sandia National Laboratories and the  National Renewable Energy Laboratory (NREL) are reviewed  with several examples of recent results included and sited.


Definition of Reliability


Sandia National Laboratories is DOE’s primary Systems  Engineering laboratory.  As such, Sandia brings a systems  approach to PV reliability.  This means that to adequately  understand the reliability of a component it is necessary to  understand the end use.  For the majority of photovoltaic  devices, the end use is in a PV array, outdoors for 30 years  providing power to the grid or to an off-grid customer.  This  provides the most basic requirement for PV reliability.


The following definition of reliability is being used within  Sandia’s PV Reliability Program and will be used in this  paper:


Reliability is the probability of simultaneously satisfying the  performance requirement in a specified environment at a  particular time.


PV System Overview


The components and structure of a system, the expected  operating conditions, expected performance, definition of  failure, and expected failure modes must be understood before  even a qualitative reliability assessment is possible.  The  primary components of PV systems are summarized in Table


1.  A typical PV system is designed with multiple PV modules  connected in series to generate the desired voltage (a “string”); several strings are combined into a combiner or marshalling


box in series or parallel to generate the desired voltage/current  combination (PV Row); the DC disconnect and fuse allow  each string or row to be isolated if needed; rows can be  combined into an inverter which converts DC power to AC  power.  Note that micro inverters can also be used at the  module level.  The power lines then go through a power meter  and into a transformer and AC disconnect for grid-tied  systems.  Stand-alone systems include a storage component, such as a battery bank.


Table 1. PV System Components for a typical


Component Materials


Use/Purpose


PV Modules Semiconductor devices, metal  interconnects, substrate and  superstrate (glass, tevlar,


metal foil, polymer), diodes, EVA (encapsulant), wires


DC power  generation


Junction  Box


Wires, diodes


Module


Interconnect


Wires, connectors


Series or parallel  string; carries


current


Blocking  Diode


Si diode


Prevent power  backflow


Fuses, terminals


Combine PV


strings together, protect against  power surges


DC


disconnect


Mechanical switch, metal box, DC wires


Allow PV strings  to be isolated


Inverter


Capacitors, semiconductor  devices, wires, LED display, metal box


Convert to AC


power


Power Meter Mechanical or digital output Monitor power


generation


To assess and test for failure, the expected use environment  must be understood.  PV arrays operate outdoors, throughout  the year, in nearly every climate.  Operating temperature  extremes can range from below freezing to well above 80°C, with an expected number of thermal cycles of 10000-50000, depending on expected cloud coverage and shading  conditions.  Humidity in various operating conditions can  range from desert climates (<10% RH) to tropical climates (>90% RH).  Systems must be able to survive high winds, snow loading, and hail impact.  Electronics need to survive  dust, dirt, and bug accumulation.  Glass and electronic  components must survive vibration and other transport  conditions in tact.  Plastics and polymers must survive  extended UV exposure.  String-level voltages can reach 600 V  in the US, 1000 V in Europe, and even higher if the array is  protected from public contact (behind a utility “fence”).


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 166-170


The expected performance of a PV system can be modeled  based on weather, solar insolation, and expected component  performance [1].  Different models can differ in performance  predictions by as much as 10% from each other, and from  measured data [2 and references therein].


Designing reliability test and analysis techniques requires an  understanding of the expected failure modes and a definition  of failure. Currently the definition of failure within the PV  community is inconsistent and application-dependent.  For  example, system failure may be defined as the point when the  system is providing 80% of its original power.  Others may  define a system to be failed only when it is not providing any  power at all.  This variation can have drastic effects on the  calculation of reliability.


Failure mode information for PV modules has been collected  over the last 20 years through anecdotal evidence, papers, and  presentations.  Recently, NREL and Sandia compiled a list of  the top failure modes observed and documented for PV  systems (http://www.nrel.gov/pv/performance_reliability/).  Such a list can be used to focus in on the areas to test.  What is  missing is the extended list of failure modes for the combined  system, including the inverters, disconnects, etc.


PV Reliability and Failure Analysis


The approach to calculating reliability and failure statistics of  components in general is fairly well understood, if not always  applied.  How is the reliability of a system determined?  For a  PV system, by determining the probability that it will be  producing the expected power at a given time.  The reliability  of the system is also determined by the least reliable  component in the system, and it is therefore important to test, analyze and calculate reliability of the components separately, as well as in the system.  Full failure analysis techniques are  required to determine and hence, mitigate failure mechanisms.  The use of full failure analysis for failed components and  systems is inconsistent in the PV industry, and more complete  application could provide great benefit.


Failure Analysis of Components


The best way to improve the reliability of the system is to  improve the reliability of each component and then to address  any unreliable interactions between the components within the  system.  An initial series of accelerated life tests (ALTs) is in  place for PV modules through international qualification  standards [3-5]. The primary tests include thermal cycling, damp heat exposure, humidity-freeze cycles, ice ball impact (hail), and mechanical load [3].  These tests are primarily  pass/fail tests. The pass/fail for performance is typically set at  no more than 5% power loss after a given test and no more  than 8% after the test sequence.  These are only initial ALTs  and the results cannot be used at this point in time to predict  module lifetime.  Inverters must pass a safety standard [6] and  an efficiency rating [7], but there is no reliability-type  qualification equivalent for inverters at this time.


There are five areas pertaining to reliability not addressed by  these standards: 1) test to failure; 2) quantitative assessment of  failure and failure statistics at the component level; 3) calculation of transport equations such as activation energies  to transfer results of these tests to expected lifetime under  operating conditions; 4) comparison of ALT results to failures  observed in the filed under use conditions; and 5) consistent  failure analysis on failed (or passed) components to enable  reliability growth.  Such testing and analysis is needed to  determine acceleration factors for failure modes, generate  failure probabilities, and predict reliability. There are some PV  manufacturers that are very good at addressing these missing  links (see for example reference [8]), but many are just  developing expertise in these areas.


Both Sandia and NREL are expanding the reliability  knowledge and test technology at the component level.  Sandia  is assessing the performance and failure of fielded modules  and inverters to add to the statistical data available [9-10]. Sandia is also conducting accelerated life tests on new module  components to support design for reliability.  Some module  designs are using conductive tapes for carrying current in the  module instead of soldering ribbons or wires. A Failure Modes  and Effects Analysis (FMEA) of one particular module type  demonstrated a high occurrence and severity for failure of the  conductive tape. To address this, Sandia performed  accelerated life testing using three environmental conditions  and two interface configurations. Resistance was monitored in  situ. Figure 1 provides an example of change in resistance with  thermal cycling of conductive tapes [11].  It is not enough to  determine the effects on the component; it must be brought  into the systems perspective to understand system-level  reliability.  In ref. 11, Sorensen et al calculated the reduction  in power for a “typical” module expected with the increase in  series resistance for each scenario tested.  A 20% drop in  module power was chosen as failure and the data were then  modeled to a failure distribution. This data set could then be  included in a system-level reliability prediction model (see  next section).


Figure 1: Initial results of an accelerated test developed to  quantify failure risk of conductive tapes in PV modules


NREL is also performing accelerated testing on both modules  and module components. With regard to modules, for example, NREL is performing extended damp heat testing on modules


Cu-Sn Tape at 60° C, 70% RH Short Time


1.E-03


1.E-02


1.E-01


1.E+00


1.E+01


1.E+02


0.00


5.00


15.00


20.00


Time (hrs.)


tape # 1 tape # 2 tape # 3 tape # 4 tape # 5


15mm overlap, 30mm long 1mm overlap, 30mm long


control, 30mm long


Open


and comparing the degradation observed in the current-voltage  curves with long term field testing of similar modules in a hot  and humid climate.  This will serve to demonstrate adequacy  or lack of adequacy of the qualification tests as well as provide  calculated activation energy for failure due to damp heat. NREL is also instituting a module test-to-failure protocol using  thermal cycling and damp heat to assess how far modules can  be stressed before failure is observed.


With regard to component accelerated testing, NREL has been  studying degradation of encapsulants under both accelerated  UV [12] and humidity, since these are weak links in the  module lifetime.


There are still many areas yet to be addressed, including the  specific failure mechanisms of inverters and other balance of  systems components, such as the AC disconnects.  Generating  failure statistics and incorporating the failure data into the  system model is also an area of continued work.


Failure Analysis of PV Systems


Sandia has been working to address PV systems reliability for  many years. System-level reliability requires good  documentation of failures in the field.  The system-level  failures are documented in operations and maintenance (O&M) data logs. Unfortunately, the accuracy and consistency  of these data logs is sporadic, creating greater challenges to  assessing the current state of PV systems reliability.


Figure 2 is taken from a paper by Moore and Post [13], outlining system-level failures observed during five years of  operations of 5 MWdc of grid-connected photovoltaic systems.


Figure 2: Unscheduled maintenance events by component for  5 MWdc grid-connected photovoltaic systems [from ref. 13]


Note that the inverters failed most often in these array fields, followed by the AC disconnects and then by the PV modules.  This level of data provides a guide to components designers  and manufacturers to address weak points.  However, calculating failure statistics requires an additional level of data  and analysis.


Sandia is currently addressing the systems-level failure  analysis through the development of a PV systems reliability  and availability predictive model using a reliability block  diagram (RBD) approach.  The detailed systems design and  O&M data upon which Figure 2 is based have been used for  the initial development [14].


[6]  “Handbook of optical constants of solids”, Edward D. Palik, Gorachand Ghosh, Academic Press, ISBN  0125444230, 9780125444231, 1998


Failure Analysis of Breakdown Sites in Silicon Solar Cells


Otwin Breitenstein, Jan Bauer, Jan-Martin Wagner, Horst Blumtritt, Nikolai Zakharov


Max Planck Institute of Microstructure Physics, Halle, Germany   breiten@mpi-halle.mpg.de, +49-345-5582740


Andriy Lotnyk


Christian-Albrecht-University, Kiel, Germany


In this contribution the use of electroluminescence imaging, bias-dependent lock-in thermography, special dark and  illuminated lock-in thermography techniques, and electron  microscopy techniques is demonstrated for investigating the  physical mechanism of breakdown in multicrystalline silicon  solar cells. Two dominant breakdown mechanisms are  identified, which are breakdown at recombination-active  crystal defects, showing a relatively soft breakdown, and  avalanche breakdown at dislocation-induced etch pits, which  occurs very steep (hard breakdown) and dominates in our cells  at high reverse bias.


°    °


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 222-229


A Novel Technique of Device Measurement after Cross-Sectional FIB in  Failure Analysis


Chih-Chung Chang, Jian-Chang Lin, Wen-Sheng Wu, Chih-Ying Tasi , Ching-Lin Chang


United Microelectronics Corporation, Tainan, Taiwan, ROC (James_CC_Chang@umc.com)


A dual beam FIB (Focused Ion Beam) system which provides  the ion beam (i-beam) and electron beam (e-beam) function  are widely used in semiconductor manufacture for  construction analysis and failure cause identification. Although FIB is useful for defect or structure inspection, sometimes, it is still difficult to diagnose the root cause via  FIB e-beam image due to resolution limitation especially in  products using nano meter scale processes. This restriction  will deeply impact the FA analysts for worst site or real failure  site judgment. The  insufficient e-beam resolution can be  overcome by advanced TEM (Transmission Electron  Microscope) technology, but how can we know if this  suspected failure site is a real killer or not when looking at the  insufficient e-beam images inside a dual beam tool? Therefore, a novel technique of device measurement by using C-AFM (Conductive Atomic Force Microscope) or Nano-Probing  system after cross-sectional (X-S) FIB inspection has been  developed based on this requirement.


This newly developed technology provides a good chance for  the FA analysts to have a device characteristic study before  TEM sample preparation. If there is any device characteristic  shift by electrical measurement, the following TEM image  should show a solid process abnormality with very high  confidence. Oppositely, if no device characteristic shift can be  measured, FIB milling is suggested to find the real fail site  instead of trying TEM inspection directly.


A dual beam FIB system providing i-beam and e-beam  technologies are widely used in semiconductor manufacture  for construction analysis and failure cause identification. The  FIB uses a Gallium i-beam to bombard the surface of the  sample and allows the milling of small holes at well localized  sites, so that cross-sectional images of the structure at precise  layout site can be observed by e-beam inspection. [1-3]


When the processes shrink into the nano meter scale, some  failure mechanisms are difficult to diagnose the root cause via  X-S FIB inspection due to the limitation of image resolution  from the e-beam. Real failure site confirmation is a big  challenge without sufficient e-beam resolution. In the  semiconductor field, the most familiar solution is to utilize  TEM technology to provide a high resolution image. But  sometimes, TEM images cannot provide us the root cause if  the suspected failure site is not the real fail site. In order to


overcome this problem, a novel technique of device  measurement after X-S FIB will be presented later in this  paper.


The FIB milled sample will be covered by an epoxy coating, and then manually polished to the contact layer. In this way, highly reliable electrical measurements can be obtained by  C-AFM or Nano-Probing. The C-AFM or Nano-Probe can   diagnose if the suspected failure site is the real failure site or  not. Furthermore, the sample can continuously be analyzed by  following TEM without any impact.


Sample Preparation Procedure


A typical X-S FIB image with structure diagram is shown in  Fig.1. As the pictures show, the salicide is partially missing  under bit line (BL) contact.


Fig.1 (a)A typical X-S FIB with partial salicide missing under  BL contact, (b)A structure diagram of failure sample after FIB  milling.


The sample preparation procedure is as below


Step 1: Fill up the FIB hole with epoxy coating, as Fig.2(a).


Step 2: Parallel lapping this sample till contact layer by


manual polish, as Fig.2(b).


Step 3: Device measurement


, as Fig.2(c).


Following the above procedure, the electrical characteristic of  the suspected failing device could be measured by either  C-AFM or Nano-Probing.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 230-233


Fig.2 (a) Fill up the FIB hole with epoxy coating, (b) Manual  polish this sample till contact layer, (c) device measurement by  C-AFM


Case Study


I. The first example using nano-probing measurement


In this case, an SRAM dual bit failure using nano meter  processes will be investigated. In Fig.3, the X-S FIB results  show salicide is partially missing under the suspected failing  BL contact. But how can we know if this partially missed  salicide is a killer or not at this dual bit failure site? Although  advanced X-S TEM inspection can give us clear images of the  missing  salicde with high enough resolution, the TEM result  cannot provide us the information about contact resistance  change or impact level due to abnormal salicide processing.


Fig.3 Salicide partial missing under BL contact by FIB


In order to eliminate this concern, device measurement using a  Nano-Probing system is applied here. The FIB milled sample  of interest is covered by an epoxy coating. Without this  coating, there is a risk of sample or probe tip damage when we  do manual polish or Nano-Probing directly.


Using a Nano-Probing system, one tip probes the suspected


failed BL contact and the other tip probes the bulk contact, as  shown in  Fig.4(a). In Fig.4(b), the I-V curve reveals that the  n+ to P-Well junction current at the suspected failing BL  contact is much lower than that at a nearby good BL contact. Both areas were milled by FIB. This means the partially  missing salicide will cause BL contact high resistance and  result in an SRAM dual bit failure.


We also have a junction current comparison between nearby  good BL contacts with and without FIB milling. As seen in  Fig.4(b) the junction current of an FIB milled good BL contact  is a little lower than that of a no FIB milled good BL contact. Smaller contact size after FIB milling will induce higher  contact resistance and cause lower junction current.


Fig.4(a) The suspected failure BL contact is probed by using  Nano-Probing system, (b)


I-V curve of the suspected failure BL contact, nearby good BL  contact with FIB milling, and good BL contact without FIB  milling.


II. The Second example using C-AFM measurement


In case 2, another sample with a similar failure mechanism can  be found as case 1. Salicide is missing under the Vdd contact  as observed by X-S FIB, see Fig.5.


Fig.5 Salicide missing under Vdd contact by FIB


The same sample preparation procedure using the newly  developed epoxy coating and manual polish combined with   C-AFM is applied in this study. By using the C-AFM, n+ to  P-Well junction current can be detected through the suspected  failing contact and good Vdd contacts. In the Veeco CP-II  model, one tip is applied to the ground and the sample  backside is activated by a DC bias. The feedback Z-axis signal  generates AFM topography image. The current path from tip  to sample is measured and generates the C-AFM signal.


As Fig.6 shows, a dark signal by C-AFM with –0.5V DC  biased voltage is detected at the suspected failing Vdd contact. It means the junction current through the Vdd contact is much  lower than a good Vdd contact. This electrical result matches  our postulation that salicide is missing causing high Vdd  contact resistance and results in an SRAM dual bit functional   failure.


Fig.6. Dark signal at suspected failure Vdd contact is detected  by using C-AFM as DC biased voltage -0.5V. It means lower  junction current through failing Vdd contact.


After electrical measurement, further TEM analysis can still  be done in the same sample without any impact. X-S TEM  result is shown in Fig.7.


Fig.7 Salicide missing is found by TEM


III. The third example using nano-probing measurement  for not real failure position


In case 3, a reliability test failure will be discussed. After fault  isolation by electrical failure analysis, the X-S FIB image in  Fig.8 indicates salicide migration into the poly gate and  substrate layer.


Fig.8 Salicide migrates into poly gate and substrate layer


Device measurements are made using a nano-probing system. As Fig.9(a) shows, one tip probes the suspected failing poly  contact and the other tip probes the bulk contact. The I-V  curve reveals fully open behavior at the poly contact as seen in  Fig.9(b). This electrical behavior is inconsistent to X-S FIB  result with salicide migration and the nearby good poly  contacts. He small leakage current at the nearby good poly  contact is believed to be poly gate damag during FIB milling. According to this result, this salicide migrated poly gate  should not be the real failure site. Therefore, more FIB milling  is executed and finally, the real fail site is proved to be a poly  gate burned-out instead of salicide migration only, see Fig.10.


Fig.9 (a)Poly contact I-V curve is measured by using  nano-probing system, (b) I-V curve shows poly contact  fully  open but small current in nearby good poly contact


Fig.10 Poly gate burned-out is confirmed after FIB more  milling


A novel technique of device measurement after X-S FIB  by using C-AFM and Nano-Probing is presented in this paper. Using this newly developed technique, device characteristics  can be measured without any permanent damage. This result is  helpful for failure mechanism or root cause judgment. Although the electrical characteristic might slightly change  due to structureal damage by FIB milling, it is still worthy to  compare I-V curves between the suspected failure and a  nearby good site for root cause confirmation. Furthermore, the  same sample can be analyzed by advanced FIB, TEM, or other  element analysis without any impact.


Reference


[1] Verkleij D, “The Use of the Focused Ion Beam in  Failure Analysis”, Microelectronics Reliability, Volume 38, Issues 6-8, June-August 1998, Pages 869-876.


[2] Gunnar Zimmermann, Richard Chapman, “In-situ  Dual Beam (FIBSEM) Techniques for Probe Pad Deposition  and Dielectric Integrity Inspection in 0.2 μm Technology  DRAM Single Cells” ISTFA '99 , Pages: 311-316


[3] Stevie F.A., T.C. Shane, P.M. Kahora, R. Hull, D. Bahnck, V.C. Kannan, E. David, “Applications of Focused Ion  Beams in Microelectronics Production, Design and  Development”, Surface and Interface Analysis, Volume 23, Page 61~68 (1995)


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 234-241


The method for retaining an Intermittent Electrical Failure signature during the  Interconnect Immobilization process throughout Failure Analysis


Julie Schuchman, Intel Corporation


Intel Corporation, Hillsboro, Oregon USA  Julie.schuchman@intel.com


Julie Willis, Intel Corporation


Intel Corporation, Hillsboro, Oregon USA  Julia.k.willis@intel.com


With the ever increasing need for cost reduction in the  computer industry, motherboard manufacturers are relying  more and more on timely, actionable data from Failure  Analysis methods, thus it is essential to promptly and  correctly identify the exact root cause, and incorporate  corrective actions to avoid these failures. We developed a  method of sample preparation for material analysis, which  enables us to maintain an electrical failing signature  throughout the preparation stage, making it possible to  perform electrical fault isolation up to the pivotal point before  the destructive phase of the process begins.


Due to their finicky nature, intermittent failures are, logically, challenging to perform failure analysis on. Given the fragility  of the failing signature, often times, the slightest movement  caused by an individual can not only induce additional  defects, but it has been known to cause the faulty electrical  signal to disappear completely. This renders subsequent  material analysis, or any further electrical analysis  investigations unneccessary, unreliable, or both. Thus, special  handling and processing may be required.


In our case study, we were tasked with the challenge of  performing material analysis on a board with a bank of 16  fully populated DIMM connectors. Adding to the complexity  of the request, we needed to maintain the electrical failure  signature throughout, and up to the point where the sample  preparation enters the destructive phase. The DIMM  connectors’ close proximity board design, coupled with the  heat spreaders mass on the DIMMS, when installed in the  board, presented us with a space constraint issue. Industry  standard cross sectional preparation methods did not cover  this particular challenge.


Fault Isolation, identifying and pinpointing the root cause of  the failure, is the ultimate purpose of Electrical Failure  Analysis. Using various electrical diagnostic tools at their  disposal, an engineer will isolate the failing signature to a  specific location on a motherboard. However, for many failure


analysis undertakings, mere identification of an electrical  short or open will not be sufficient, and a further in depth  investigation is warranted. This is where advanced material  analysis techniques come in handy in identification of process  irregularities, design marginalities or material property  defects.


Relative to fine focus of typical material analytical techniques  and the complexity associated with instrumentation and  sample handling, it is essential to have accurate electrical  isolation of the failing location. In general, maintaining the  failing signature is of primordial importance. In cases where  the failing signature is fragile and intermittent, a technician  may find it necessary to fashion some unique material sample  preparation techniques to freeze the failing signature before  any further electrical isolation is performed.


Outlined in the next section of this document, we will cover  the various materials and methods used for the study, highlighting the advantages or disadvantages of each one. Also covered will be the techniques that we tried, ultimatly  leading to our successful outcome. The benefit of following  this process is the ability to capture failing electrical  signatures, and then prove the failing symptom through  material analysis cross section methodology. The  disadvantages could include the potential to displace an  interfering material artifact, thus altering the analysis results. Included in this manuscript are photographs resulting from  Optical and Scanning Electron Microscopy inspection, supporting the use of this process by representing evidence of  the failing signature.


The purpose of our experiment was to develop a sample  preparation method for immobilizing failing symptoms. In our  case study, these were specifically intermittent failures  associated with DIMM and socket interconnects. Our  objectives were (1) to handle the board the minimum amount  necessary, (2) determine the optimum materials to be used  based on ease of use, functionality and overall efficiency, (3) evaluate the electrical function of the board after each  handling.


In our first experiment, we found no evidence that there was  debris interferring at the interface level. Since this is what we  believed was causing the failure, we considered that, if there


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 242-246


had been debris, the pouring of the epoxy could have caused  the debris to float away; or, during the curing phase of the  epoxy, the pins pulled away from the inserted memory  module. Therefore no obvious conclusions could be drawn  regarding our initial fault failure analysis attempt.  An  additional contributing factor could have been improper  handling that jarred the interface, causing the failure to  disappear/dislodge. Our hypothesis was that if we froze the  failure early on in the sample preparation process, we could  find conclusive evidence that debris was the source of the  failure.


Material/Methods


Fig.1: This is the board which presented the cross section  sample preparation challenge. Note the close proximity of  DIMM connectors and inserted memory modules.


Fig.2: 3M Scot-Weld Adhesive DP-460 used to secure the  locking mechanism and center retention features of DIMM  connector to the inserted memory module.


Fig.3: Image of the epoxy mixing tube. Attached to the mixing  tube is the long fine tipped needle (Monoject 16mm X


25.4mm) required to enable epoxy placement without  bumping anything.


Fig.4: Dispensing 3M epoxy to secure center keyed notch of  memory module to DIMM connector.


Fig.5: Secured memory module using 3M Scot-Weld Adhesive  DP-460. This picture shows the DIMM connector and memory  module end latching mechanism and center retention feature  secured with the use of 3M Scot-Weld Adhesive DP-460.


Fig.6: Close-up view of end latching mechanism.


Fig.7: Close-up view of center key.


Fig.8: Our first attempt was using the Flex Mask material to  plug the through in an attempt to stop any epoxy leakage on  the bottom of the board. We needed to move the board as little  as possible, so we had one technician carefully stand the  board up on its side, while another technician applied the  Flex Mask to the areas that could pose leakage issues.


Fig.9: This is an OM darkfield image showing the pin pulling  away from the gold contact on the DIMM module, induced by  pouring the epoxy too quickly.


Fig.10: This is the QuickSet Epoxy used in the next trial.


Fig.11: Our next attempt at preventing epoxy leakage was to  plug the holes with quick set epoxy, applied with the same  care taken in the initial trial.


Fig.12: This picture represents Mylar film cut in a manner to  surround and create a barrier to encapsulate the area of  interest for Material Analysis. Also depicted in this picture is  a mixture of QuickSet Acrylic Powder and QuickSet Acrylic  Liquid poured onto the Mylar film. This Acrylic is fast drying (15 minutes) and partners with the Mylar film to support the  encapsulation of the area of interest.


Fig.13: Carefully positioning the Mylar creating a self  engineered dam to secure a wall to control the flow and  application of EpoxySet.


Fig.14: This picture represents Mylar film coupled with two  part QuickSet Acrylic Powder and QuickSet Acrylic Liquid  creating a walled barrier (Dam) to support epoxy  encapsulation note the corners of the dam are not sealed.


Fig.15: Sealing corners with QuickSet epoxy.


Fig.16: This is the slow cure EpoxySet used. Note it cures at  ambient temperature in eight hours.


Fig.17: Notice the position of epoxy stream. Careful flow  placement and speed is critical. The purpose of this slow and  careful technique is to minimize the opportunity to displace  any potential artifacts or oxidization.


Fig.18: A Cross Sectioned Optical Microscope image of the  DIMM Connector coupled with a DIMM module. The arrows  are pointing to a Nickel Oxide layer that had formed between  the DIMM connector and DIMM memory module, the root  cause of the failing symptom.


Fig.19: A magnified optical microscope image of a nickel  oxide layer.


Fig.20: A SEM (Scanning Electron Microscope) Sectioned  image of the DIMM Connector coupled with a DIMM module  post cross section analysis. The arrows are pointing to a  Nickel Oxide layer that had formed between the DIMM  connector and DIMM memory module the root cause of the  failing symptom.


The sample preparation methodology described secures the  intermittent failure throughout the process which greatly  increases the ability to overcome the limitations and  challenges presented with obscure component types and sizes  for cross sectional analysis. Process improvements are still  being investigated. Our intent is to devise a better dam  technique coupled with researching other epoxy encapsulating  products which could have less shrinkage issues during the  curing progression.


Thanks to Randy Rahn, Aravind Munukutla, and Pete  Nicholas for all of their guidance and support during the  experiments. Thanks to Aravind again, along with JS Lewis, and Anil Kurella for their assistance in providing reference  materials, reviewing of our documents, and offering timely  and instrumentally productive feedback.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 247-253


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 254-260


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 261-267


Picosecond Single-Photon and Femtosecond Two-Photon Pulsed Laser  Stimulation for IC Characterization and Failure Analysis


V. Pouget1, E. Faraud1, K. Shao1, S. Jonathas1, D. Horain2, G. Haller3, V. Goubier3, B. Picart4, L. Forli4, D. Lewis1


1 IMS, University of Bordeaux, 33405 Talence, France


2 PULSCAN, 351 cours de la Libération, 33405 Talence, France 3 STMicroelectronics, 13106 Rousset, France 4 ATMEL, 13106 Rousset, France


This paper presents the use of pulsed laser stimulation with  picosecond and femtosecond laser pulses. We first discuss the


resolution improvement that can be expected when using  ultrashort laser pulses. Two case studies are then presented to  illustrate the possibilities of the pulsed laser photoelectric  stimulation in picosecond single-photon and femtosecond twophoton modes.


The growing complexity of modern VLSI devices  continuously brings new challenges for design debug and


failure analysis [1]. Classical laser stimulation techniques  which have become standard tools during the last decade are  now facing some resolution limitations for defect localisation


at nanometer scale. The development of so-called dynamic  techniques, based on the association of static laser stimulation


with dynamic testing has considerably improved the coverage  of soft defects [2,3]. Recently, modulation in the millisecond  to nanosecond range was introduced in order to perform timeresolved laser stimulation, for example for targeting a specific  time window within a test sequence. Pulsed laser techniques


with picosecond and femtosecond pulse duration have been  around for several years for radiation testing or metrology  applications [4].


In this work, we present several results of applications of


pulsed laser techniques for IC characterization and failure  analysis obtained recently thanks to the implementation of a


new pulsed laser scanning microscope on a backside probing  station at the ATLAS laser facility. First, we summarize the  benefits that can be expected and the specific aspects that must


be considered when using ultra-short laser pulses. We then  present two stimulation techniques using respectively


picosecond and femtosecond laser pulses.


Specificity of using ultra-short laser pulses


Pulsed laser stimulation with ultrashort laser pulses has  several interesting aspects including negligible thermal stress  and improved resolutions.


a. Time-resolution


The first clear benefit of using ultra-short laser pulses, i.e.


pulses with duration shorter than 100ps, is the improved time  resolution that allows illuminating shorter portions of the test  pattern. This capability is required for testing fast devices at


frequencies high enough for being representative of real  operating conditions. Coupled with low jitter testers,


picosecond laser pulses can be used to target a single  transition in the test pattern. Time-resolved analysis has  already been used for sensitive time windows characterization


for single-event effects or fault injection attacks [4].


b. Lateral resolution


The spatial resolution of laser stimulation techniques is a


complex function of the laser spot size and of the laser-device  interaction mechanisms. Defect localisation may also rely on a  specific interaction of the laser beam with the defect itself. For  photoelectric techniques like Optical Beam Induced Current (OBIC) imaging, resolution is governed by charge collection


mechanisms involved in the generation of the photocurrent, including drift, diffusion, parasitic bipolar activation... On  modern technologies with long pulses or cw lasers, resolution


is often limited by diffusion due mainly to the slow dynamics  involved in the detection. Using picosecond pulses and


adapted instrumentation, the drift contribution can become  predominant in the image formation. This is particularly  interesting in terms of resolution because the spatial extension


of the drift collection is much more limited than the collection  by diffusion.


This resolution enhancement was confirmed by TCAD


simulation of OBIC scans as presented in Fig.1. A realistic  model of the laser-induced electron-hole generation rate was


introduced into the TCAD simulation of a pair of bulk NMOS


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 268-271


transistors. Figure 1 presents the amplitude of the transient  OBIC current as a function the position of the center of the  1μm diameter laser beam. Long laser pulses don’t allow  distinguishing between the contributions of both transistors  whereas they are clearly resolved with picosecond pulses.


c. 3D resolution with non-linear interaction


Ultrashort laser pulses focused on small spot sizes allows to


reach a regime of extremely high optical intensities in which  the optical response of the material is not linear anymore with  respect to the optical intensity. In silicon, non-linear  interaction can be exploited to perform photoelectric  stimulation by two-photon absorption (TPA). Because this


mechanism depends quadratically on the intensity, it will be  significant only in the confocal section of the beam. This


implies that the stimulation has a limited in-depth extension  and can be positioned within the thickness of the device by


moving the focal plane of the beam, providing 3D resolution


[5]. TPA has also been confirmed to provide improved lateral  resolution [6].


Picosecond laser stimulation


a. Set-up


The experiment was performed at the ATLAS laser facility  with the Time-Resolved Laser Stimulation (TRLS) setup [7]. We used a double-side probing station with a backside Laser  Scanning Microscope (LSM). A cw laser at 1300nm is used  for backside reflectivity imaging and a laser source delivering  30ps pulses at 1064 nm is used for photoelectric pulsed laser  stimulation. The device under test (DUT) is made of several  chains of inverters in 130nm bulk CMOS technology, operating at 1.2V.


b. Results


Figure 2 presents typical results obtained by monitoring the


output voltage of an inverter chain during a pulsed laser scan. In this case, the chain input is set to a constant value and a  single laser pulse is triggered for each position of the LSM.


The laser energy was adjusted to be high enough to induce  transients in the chain. The transients on Fig.2a) were  generated by laser pulses impacting at different positions in  the chain. Transients observed later (i.e. on the right side of  the graph) correspond to upstream positions in the chain, i.e.


generated further away from the measuring point at the output  of the chain. The output transient duration clearly increases as


1200


-1,0-0,5 0,0 0,5 1,0 1,5 2,0


Time (ns)


2 4 6


8 10 12 14 16 18


Figure 2: a) Pulsed laser induced transients at the output of the laser chain for different impact position, b) transient amplitude mapping In gray levels LSM image of bulk Chain 130nm backside and global SET mapping. b) Measured SETs in the bulk chain, under laser irradiation, for a “high” input state(Vdd).


Figure 1: profile of the transient signal amplitude obtained by


TCAD simulation of the scan of two transistors with long


(100μs) and ultrashort (1ps) laser pulses showing a resolution  enhancement.


the transient is generated far from the output. This result  allows characterizing the propagation-induced broadening


effect of transients. Fig.2b) presents a 2D mapping of output  transient amplitude (in blue) for laser energy closer to the


commutation threshold, superimposed with an LSM image of  the structure. Multiple spots are observed that correspond to  the different inverters that were commuted by the laser pulses.


The lack of homogeneity of these areas is so far mainly  explained by noisy measurement conditions.


The broadening effect observed above, which is a bulk version


of the well-known floating body history effect in SOI  technologies, can be characterized dynamically by delaying  the laser pulse with respect to a transition applied at the input


of the chain.


Figure 3 presents the broadening effect, expressed in terms of


transient width increase per gate, versus the preset time of the  laser impacted gate. This curve allows direct extraction of at  least the short and long-term time constants for the


phenomena. Such characterization, when performed only by a  conventional electrical testing approach, would require a quite


sophisticated electrical setup, whereas a simple tester-based  delay sweep was necessary using pulsed laser stimulation.


Femtosecond two-photon laser stimulation


a. Setup


We operate with the same prober setup as above except that  the pulsed laser now emits 130fs pulses at 1300nm. At this  wavelength, only the simultaneous absorption of two photons  can induce a photoelectric stimulation. This mechanism is  enhanced by using femtosecond pulses and is only significant


in the immediate vicinity of the focal point. In this section, the  device under test is an amplifier AD9617.


Figures 4a) and 4b) present 2D mappings at two different  magnifications of the amplitude of two-photon laser induced


transients observed at the output of the chip configured as a  non-inverting amplifier with a constant input voltage. Blue


and red areas correspond to structures giving rise to negative  and positive transients, respectively. The polarisation regime  of the different zones can be immediately verified.


Figures 4c), d) and e) present the results of the detailed


scanning of a particular bipolar transistor in the DUT obtained  for three different positions along the z-axis of the sample


with respect to the focal plane of the microscope. The origin  of the z-axis is taken at the position corresponding to the best  LSM image quality, with positive direction toward the bulk.


One can observe that the transient amplitude is merely  constant in the collector diffusion when the beam is focused a


few micron below the front surface. The base and emitter  regions disappear on Fig.4d) probably due to a current  compensation mechanism between the different junctions of


the transistor. Finally, when the beam is focused above the  surface, the response seems to be dominated by reflection on


metal layers (Fig.4e). These results illustrate the potential of  the two-photon stimulation technique for 3D characterization  of future 3D-ICs.


We have presented new results based on the evolution of  pulsed laser stimulation techniques to picosecond and


femtosecond pulses durations. These approaches provide  interesting tools for advanced characterization and failure  analysis of all devices technologies including the most recent  ones, while offering new possibilities and significant  resolution improvements in the lateral, depth, and time


dimensions.


[1] C. Burmer, S. Görlich, “Failure analyses for debug and


ramp-up of modern IC's”, Microelectronics Reliability 46


pp. 1486–1497, 2006


[2] F. Beaudoin, K. Sanchez, P. Perdu, « Dynamic laser


stimulation techniques for advanced failure analysis and


design debug applications”, Microelectronics Reliability


47, pp. 1517-1522, 2007.


[3] A. Rowlette, T. Eiles “Critical timing analysis in


microprocessors using near-IR laser assisted device


200 300 400 500 600


PRESET (ms)


Figure 3 : broadening vs preset time. The preset time refers to  the time during which the chain input has been preset to a  given bias state, before the laser pulse.


alteration (LADA)”, International Test Conference 2003,


p264-273.


[4] V. Pouget, D. Lewis, P. Fouillat, “Time-Resolved


Scanning of Integrated Circuits with a Pulsed Laser :


Application to Transient Fault Injection in an ADC”, IEEE


Trans. Inst. and Meas, vol 53, No. 4, pp 1227-1231, 2004.


[5] D. Wan, V. Pouget, A. Douin, P. Jaulent, D. Lewis, P.


Fouillat, “In-depth resolution for LBIC technique by twophoton absorption”, Semiconductors, vol 41, pp.371-375,


2007


[6] K. Serrels, E. Ramsay, D. Reid, “70 nm resolution in


subsurface optical imaging of silicon integrated-circuits


using pupil-function engineering”, Appl. Phys. Let. 94,


073113, 2009


[7] A. Douin, V. Pouget, D. Lewis, P. Fouillat, P. Perdu,


“Picosecond Timing Analysis in Integrated Circuits with


Pulsed Laser Stimulation”,  Proc. of IEEE International


Reliability Physics Symposium (IRPS) 2007, Phoenix


(Etats-Unis), 15-19 avril 2007


X5


X20


Z=7μm


Z=1μm


Z=3μm


[Volts]


[μm]


Zone1


X50


CBEB


Figure 4 : Mappings of the amplitude of transients induced by Femtosecond Two-Photon pulsed laser stimulation in an AD9617.


OBIC Measurements without Lasers or Raster-Scanning Based on Compressive  Sensing


Ting Sun, Gary L. Woods, Marco F. Duarte, Kevin Kelly


Department of Electrical & Computer Engineering, Rice University, Houston TX 77005 USA   kkelly@rice.edu


Chengbo Li, Yin Zhang


Department of Computational and Applied Mathematics, Rice University, Houston TX 77005 USA


Laser-based failure-analysis techniques such as optical beaminduced current (OBIC) or optical beam-induced resistance  change (OBIRCH) involve scanning a focused laser beam  across a sample by means of a laser scanning microscope (LSM). In this paper, we demonstrate a new method of  obtaining OBIC data without requiring a laser or an LSM. Instead, we employ new techniques from the field of  compressive sensing (CS). We use an incoherent light source  and a spatial light modulator in an image plane of the device  under test, supplying a series of pseudo-random on/off  illumination patterns (structured illumination) and recording  the resulting electrical  (photocurrent) signals from the device. Advanced algorithms allow us to reconstruct the signal for the  entire die. We present results from OBIC measurements on a  discrete transistor and discuss extensions of CS techniques to  OBIRCH. We also demonstrate static emission images  obtained using CS techniques in which the incoherent light  source is replaced with a single-element infrared photon  detector so that no detector array is required.


Introduction to Compressive Sensing (CS)


In this paper, we discuss our approach to the challenge of  building a simpler and smaller optical probing system that is  useful for obtaining OBIC data and also static emission data. Our approach fuses a new architecture based on a digital  micromirror device (DMD) with the new mathematical theory  and algorithms of Compressive Sensing (CS). CS combines  sampling and compression into a single nonadaptive linear  measurement process. Rather than measuring pixel samples of  the device under test, we measure inner products between the  device and a set of measurement basis functions. Interestingly, randomized basis functions play a key role, making each  measurement a random sum of pixel values taken across the  entire image. When the scene under view is compressible, CS  theory shows that we can stably reconstruct an image of the  scene from far fewer measurements than the number of  reconstructed pixels (sub-Nyquist acquisition). For a review of  CS theory see [1] below. Compressive sensing has been  applied to a number of imaging situations, including singlepixel cameras, hyper-spectral imaging, etc. [2, 3].


Fig. 1. Image of DUT with (a) 100% illumination and (b) a  32 x 32 pseudo-random illumination pattern.


The standard approach to optical measurements such as OBIC  and OBIRCH is the time-tested raster scan. If using a laser, this means just stepping the laser beam to each pixel  sequentially. When using a DMD, one would accomplish a  raster scan simply by illuminating the entire DMD with a light  source and scanning one mirror at a time onto the sample. The  light source could be a lamp or a suitably expanded and despeckled laser beam. Of course, performing a raster scan in  this way would throw away most of the light and would hence  require unacceptably long integration times in real-world  cases.


An alternative to the raster scan using a DMD is the so-called “basis scan.” In this case, the entire die is illuminated with a  series of patterns that comprise a complete basis set. If there  are M pixels then M patterns are required. For each pattern the  corresponding electrical signal is recorded, as illustrated in  Fig. 2.


In CS, one uses not a complete set of basis functions but a  smaller set of random illumination patterns. This is  advantageous because the theory of CS tells us that if our  imagery is compressible, then we can take many fewer  random measurements than the number of raster-scanned  pixels or basis-scan functions. If there are M pixels in the  image, then typically we can make L measurements, where  L/M is on the order of 10% or less, with only a small SNR  penalty compared to basis scan. This is analogous to the  familiar JPEG compression of images – although the  compression is lossy, most of the information in the image is


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 272-277


retained even though the file size is much smaller than the  original.


Theory of CS applied to OBIC/ OBIRCH


We analyze the signal to noise ratio performance of OBIC  using raster scan, basis scan, and CS. For modest optical  power levels, OBIC signals are quite linear in the optical  power. In principle the same analysis applies to OBIRCH  although the optical power levels required are much higher, and the SNR significantly lower, due to the weaker effects. We assume an array of M pixels and denote by i m( )  the  value of the image to be sensed at the mth pixel. We can  express the image values in a vectorized representation   i = i 1( )…i M( )[ ]T .


To measure the image, we shine a series of light intensity  patterns  am= am1( )…amM( )[ ] ,  m = 1…M , which provides  us with measurements


(1) x m( ) = amm( ) i m( )


m =1 M


= am i .


Note the measured values are by assumption linear in the  optical power. If we stack the M row vectors am into a matrix  A of size M  M , then this measurement process can be  represented as the matrix equation x = Ai . We also assume  zero-mean white noise inm( )  is added to each obtained


measurement x m( ) ; by collecting the noise values into a


vector  in= in1( )…inM( )[ ]T, our measurements then


correspond to x = Ai + in. When A  is a basis (or more  generally a full rank matrix), an estimate of the image data is  obtained as


i = A-1x = A-1 Ai + in( ) = i + A-1in.


Thus the signal to noise ratio at the mth pixel, defined as a  ratio of voltages, becomes


(3) SNR m( ) =i m( )


î m( )  i m( )


i m( )


am-1in


where am-1 denotes the mth  row of the matrix A-1 . We first  evaluate the Euclidean norm of the rows   am= am1( )…amM( )[ ]  of the matrix A , defined as


am= amm( )2


for the different techniques; the SNR will be proportional to  this norm.


In raster scan with optical power P, the row   am= 0…0 P 0…0[ ] , with the P at index m; the Euclidean  norm of this vector is am= P .


In basis scan with optical power P per non-zero pixel (and  hence M 2  times higher total power incident on the sample),


the row am corresponds to the mth  Walsh pattern with entries


0 and P. Its Euclidean norm is am= P M 2 .


In basis scan with optical power P distributed equally among


the M pixels, the row am corresponds to the mth Walsh pattern  with entries 0 and P M . Its Euclidean norm is


am= P 2M .


We now calculate the SNR for each methodology, accounting  for the estimation process. We take the signal at the pixel of  interest to be unity: i m( ) = 1 , and the variance of the noise to


be  2 : E in2[ ] = 2 .


In raster scan we set the matrix A = P  I  where P is the  optical power and I  is the identity matrix, so that only one  pixel is measured at a given time. In this case,


am-1in= inm( ) P .  The expectation value of the SNR becomes


(5)


SNRrasterm( ) =i m( )inm( )=P.


In basis scan with total optical power P distributed uniformly  over all M pixels of the modulator, we set the matrix  A = P W , where W  is the Walsh matrix with entries 1 M


and 0. The matrix B = A-1  will have entries bmm( )  of  magnitude 2 P  (save for a single entry of magnitude


M  2


( ) P , which represents a DC offset and can be  ignored). One can show that the expected value of the  denominator of the SNR is


(6)


E am1in[ ] = 2 M P .


In the basis scan with optical power P per nonzero pixel so  that the total optical power is MP 2 , we set the matrix


Fig. 2. Optical setup showing random DMD illumination  pattern focused onto DUT. The resulting photocurrent is  measured by the ADC. A computer records the series of  measurements and reconstructs the image using advanced  algorithms.


A = MP W , and so the matrix A-1= B MP , with entries of  magnitude 2 MP , save for a single entry of magnitude  M  2


( ) MP . One can show that the expected value of the  denominator of the SNR is


(7)


E am1in[ ] = 2 MP


So


we


obtain


expectation


that  SNRbasism( ) = SNRrasterm( ) 2 M  under the assumption of  constant


optical


P,


and  SNRbasism( ) = MSNRrasterm( ) 2  when we assume optical  power P per pixel. This implies that for basis scan to  outperform raster scan, we will need an amplification of the  total optical power by a factor of at least 2 M .


In CS, the measurements follow the same formulation as in  basis scan. CS recovery introduces an amplification in the  noise power by a constant Cn, which has been shown  experimentally to be approximately 4 [4]; thus we can say  roughly that  SNRCS SNRbasis2 , where now we refer to the  SNR averaged over the entire image. The advantage of CS  over basis scan is that we only need  L  M  measurements. Thus the acquisition time is reduced by a factor L M , which  could be 10x or more depending on the image. For further  discussion of basis scan and CS theory, see refs. [5-6].


Fig. 6 shows numerical simulations of the relative scaling of  SNR for CS vs. raster-scanned images. A series of 128 x 128  images with up to 10 nonzero data points was used. The  amplitude of each nonzero  point within an image was set to 1, 10, 100, or 1000.  Gaussian noise of rms value 1 was then  added. Each image was reconstructed with raster scan (using  the full 16K measurements) and CS (using 100 measurements) and the expectation value of the SNR, averaged over the entire  image, was calculated. The CS measurements used 128 times   as much total optical power incident on the sample as the  raster measurements; in this limit the SNR values are  approximately equal as expected, over a range of about 3  orders of magnitude.


Interestingly, for low SNR and small number of nonzero  pixels, the CS measurement performs somewhat better than  raster. This is because the CS technique only required 100  measurements (vs. 16K for raster) and so the signal was  extracted without adding in an enormous number of noise  measurements. At higher SNR and higher number of nonzero  pixels, the raster scan shows some improvement over the CS. This is due to the heavier weighting of the high-signal pixels  when averaged over the whole image.  In the high-SNR  regime either image would be sufficiently clean to be useful, but the CS measurement in this (extremely sparse) case  required less than 1% of the measurements required for the  raster scan.


OBIC results


To demonstrate CS applied to OBIC, we constructed a simple  experimental setup. A visible/ near-IR white-light beam (from  an arc lamp source) was collimated onto a Texas Instruments


digital micromirror device (DMD). This is the same type of  spatial light modulator used in conference-room projectors. The DMD has an array of 1024 x 768 independentlyaddressable pixels and is capable of 8000 frames per second in  the DLI Discovery 1100 package. The DMD was imaged onto  the DUT to create structured illumination matching the digital  pattern applied to the DMD. A representative pseudo-random  illumination pattern on the DUT is shown in Fig. 1.


(a) CS 50%


(b) CS 30%


(c) CS 20%


(d) CS 15%


(e) CS 10%


(f) Raster with 10x gain


Fig. 3. OBIC measurements of DUT with constant optical power  per pixel, 256 x 256 resolution. (a)-(e): CS measurements with  specified level of compression. (f) Raster data with 10x extra  gain to boost SNR.


The DUT was a large discrete NPN power transistor with the  base & emitter terminals connected to a transimpedance  amplifier (TIA). The OBIC signal from the DUT was  converted to a voltage level by the TIA and recorded by an  analog to digital converter (ADC). Fig. 2 shows the optical  setup. A series of pseudo-random illumination patterns with  256 x 256 effective pixels was applied to the DMD and  imaged onto the DUT. A series of patterns up to 50% of the  full 64K patterns was recorded.


The raw data from the measurements was inverted using an  advanced algorithm based upon a fast total variation  minimization routine (TVAL3: TV minimization by  Augmented Lagrangian and ALternating direction


ALgorithms) developed by two of the authors, Zhang and Li


[7]. Development of such algorithms is a topic of active  research. Somewhat slower-performing algorithms are already  available in the public domain [8-10]. The algorithms typically  take from a few seconds up to about 1 minute to execute  running in Matlab. Optimized/ complied code could run much  faster if necessary.


In reconstruction one need not use all of the patterns. Fig. 3(a)-(e) shows reconstruction using varying fractions of  the total potential 64K patterns. In practice one would only  record the required fraction of the total patterns, leading to an  acquisition time advantage. The flexibility to trade off SNR  directly for acquisition time is an advantage of CS techniques  over raster scan: if one terminates an OBIC scan 10% of the  way through a measurement, one only obtains data for 1/10 of  the field of view rather than obtaining a somewhat noisy but  useful image of the entire field of view.


Fig. 3(f) shows a raster scan measurement taken with the same  power per pixel as the CS measurements. In this case the  signal was so small as to be limited by quantization noise in  the ADC. The gain of the TIA was increased by 10x to  compensate. Even in this case some of the weaker features (such as the outer contact ring due to the collector-base  junction) are completely missing. The constant power per  pixel assumption reflects cases in which there is a maximum  allowed intensity one can apply to the DUT. This would be  relevant when limited by optical damage to the DUT or by the  need to avoid latchup.


We also performed a series of experiments with constant total  power. This is analogous to expanding a laser beam from a  raster-scanning measurement to fill the entire die and  performing CS instead. We used 128 x 128 resolution and  attenuated the white-light source by approx. 1e4 during the CS  measurements to achieve roughly constant total power. The  results are shown in Fig.4. In this case, as predicted by theory, the raster measurement is cleaner, although the OBIC data is  still quite good.


Emission results


Compressive sensing is also relevant for emission images  from integrated circuits. Instead of acquiring emission images  using expensive focal-plane array (FPA) detectors, one can  use a single-pixel photon detector and spatial light modulator. This is the basis of the original “single-pixel camera” idea [1-2]. The advantage in this case is the greatly reduced cost and  complexity of a single-pixel emission microscope compared to  an FPA-based system. Scientific-grade InGaAs FPAs with  liquid-nitrogen cooling cost much more than $20K and are not  commercially available everywhere in the world. On the other  hand, a single-element photodiode along with a DMD could  cost significantly less and achieve comparable levels of  performance in some cases.


In Fig. 5 we demonstrate a 256 x 256 emission image taken  from a similar transistor to the OBIC device above using CS  techniques. The light source from the OBIC measurements  was replaced by a TE-cooled InGaAs detector. The baseemitter junction of the DUT was forward-biased, causing  emission due to electron-hole recombination. The light  emitted by the DUT was imaged onto the DMD. The pseudorandom intensity patterns reflected by the DMD were  collected onto the detector and then digitized. The image looks  somewhat noisy due mostly to the very low numerical aperture (NA) optics used for collection of the light and the unoptimized detection electronics. The exact scaling of emission  performance using CS compared to array detectors is beyond  the scope of this paper.  However, with suitable optics and  electronics, CS can perform quite well for emission and in  some practical cases may outperform (in SNR, acquisition  time, or cost) emission measurements from array detectors.


(b) CS 40%


Fig. 4. OBIC measurements  at constant total optical  power, 128 x 128 resolution. (a)-(b) CS with specified  levels of compression. (c) raster scan.


(c) Raster


Fig. 5. Emission data taken from a bipolar power transistor  with forward-biased B-E junction. 256 x 256, 20% compression.


While the above example (OBIC on a single macroscopic  transistor) is rather simplistic, the CS techniques we have  demonstrated are readily extensible, at least in principle, to  more-relevant problems such as OBIRCH on microscopic  devices.


In general OBIRCH requires the use of high optical intensity  not too far below the damage threshold of the device. A  ballpark number is 100 mW focused into a 1um spot. As  discussed above, to achieve the same SNR using CS in a  1MPix image, one would require about 100W optical power  spread over the entire field of view. This is impractical.


However, we speculate that CS-OBIRCH could find  application in the new field of volume optical diagnostics for  yield enhancement at the wafer level. In this scenario, the goal  is to localize gross defects with high throughput. CS is in  principle easier to automate than laser raster scanning, and  some subset of defects that require lower optical power could  be found. Using the above numbers, a defect that required  1 mW to find using raster-OBIRCH could be found using 1W  over the field of view, in perhaps 10% of the time required for  a full raster scan.


Some OBIC measurements are also intensity-limited. For  latchup avoidance in OBIC, one is often limited to a few W  optical power in single spot. Many commercial OBIC systems  cannot accurately generate such a small power level. Using  CS, a few mW spread over the DUT would suffice to obtain  an OBIC image in less time than possible with rasterscanning.


We point out that CS is not directly applicable to dynamic  laser stimulation (DLS) techniques. This is because CS  assumes the measurements are linear, whereas the digital  pass/fail measurements from DLS techniques are highly nonlinear. Conceivably one could bias the DUT near the 50%-failure point and track the pass/fail statistics vs. the applied  pattern, although this would be difficult in practice.


Emission images taken with CS may find a commercial niche  due to the rather low expected cost of single-pixel systems  compared to high-performance near-IR imaging detector  systems. We also point out that CS techniques could improve  the performance of PICA (Picosecond Imaging Circuit  Analysis) systems. In this scenario, one could obtain timecorrelated photon counting images (with x,y, and t resolution) from a single-element photon-counting detector and a DMD.


We have demonstrated OBIC measurements taken without the  need for a laser or a laser-scanning microscope. Using a digital  micromirror device and compressive sensing techniques, we  are able to acquire OBIC data using a simple optical system. Under some circumstances a CS-OBIC system can outperform  a comparable raster-OBIC system or be more suitable for  automated measurements. We also have demonstrated using  CS to obtain static emission data from a discrete transistor  using a single-element detector. We have also speculated on  the extension of CS techniques to measurements as diverse as  OBIRCH and PICA. It is too soon to predict whether CS will


find any commercial application in FA, but we hope this paper  will encourage further work in this field.


Fig. 6. Numerical simulation OBIC/ OBIRCH measurements, with M = 128 x 128 resolution. Horizontal axis is SNR of  acquired raster images (full 16K measurements). Vertical axis  is SNR of CS (100 measurements). The optical power for the


CS measurements was M = 128  higher than the raster  measurements.


The authors acknowledge diligent and useful critiques from  Aaron Falk.


[1] Marco Duarte, Mark Davenport, Dharmpal Takhar, Jason  Laska, Ting Sun, Kevin Kelly, Richard Baraniuk, “Single-Pixel Imaging via Compressive Sampling,” IEEE  Signal Processing Magazine, 25(2), pp. 83 -91, March


2008.


[2] Dharmpal Takhar, Jason N. Laska, Michael B. Wakin, Marco F. Duarte, Dror Baron, Shriram Sarvotham, Kevin  F. Kelly and Richard G. Baraniuk, “A New Compressive  Imaging Camera Architecture using Optical-Domain  Compression,” Proceedings of Computational Imaging IV  at SPIE Electronic Imaging, 2006, San Jose, CA. pp. 43-52.


[3] Ting Sun’s Master Thesis, ECE Department, Rice  University, Houston, TX 77005 USA.


[4] Richard G. Baraniuk, Volkan Cevher, Marco F. Duarte and  Chinmay Hegde, "Model-based Compressive Sensing," submitted for publication, 2008; revised, 2009.


[5] Brady, D. J., “Multiplex imaging and the constant radiance  theorem,” Optics Letters, 2002, 27(1):16-19.


[6] Gustave L Davis, Mauro Maggioni, Frederick J Warner, Frank B Geshwind,  Andreas C Coppi, Richard A  DeVerse, Ronald R Coifman, “Spectral Analysis of  normal and Malignant Microarray Tissue Sections using a  novel micro-optoelectrialmechanical system,” Mod. Pathol., vol. 17 no. 1:358A (2004).


[7] TVAL3: TV minimization by Augmented Lagrangian and  ALternating direction ALgorithm.  See: http://www.caam.rice.edu/~optimization/L1/TVAL3/.


[8] Elaine Hale, Wotao Yin and Yin Zhang, “A Fixed-Point  Continuation Method for L1 Regularized Minimization  with Applications to Compressed Sensing,” CAAM  Technical Report TR07-07, Rice University.


[9] Emmanuel Candes, Justin Romberg “L1-magic: Recovery  of Sparse Signals via Convex Programming”, User’s  guide of L1-magic code, Caltech, 2005.


[10] Emmanuel Candes, Terence Tao “Decoding by Linear  Programming”, IEEE Transactions on Information  Theory, 2005.


Development of laser-based Variation Mapping techniques – another way to increase the  successful analysis rate on analog & mixed-mode ICs


Magdalena SIENKIEWICZ1,2, Kevin SANCHEZ1, Luigi CATTANEO1, Philippe PERDU1, Abdellatif FIRITI2, Olivier  CREPEL2, Dean LEWIS3


1: CNES – French Space Agency, 18, avenue Edouard Belin, 31401 Toulouse, France  2: Freescale Semiconductor, 134, avenue Général Eisenhower, 31023 Toulouse, France  3: IMS, Université de Bordeaux 1, 33405 Talence, France


PURPOSE


The failure localization on analog & mixed mode ICs in  functional mode (AC signals) has become more and more  challenging in the last few years. Due to an increasing  integration and complexity of these devices, the number of  defects, especially those named “soft”, raised considerably. The classical Dynamic Laser Stimulation (DLS) techniques  showed some limitations when applied to analog & mixedmode ICs. The SDL (Soft Defect Localization) technique [1] based on binary output signal allows us to localize only the  most sensitive areas. The defect in this type of circuits, which  are very sensitive to the laser beam [2], is often characterized  by a weaker sensitivity than that of “healthy” regions. Hence, xVM (Variation Mapping) techniques were introduced to map  some parameters in an analog way (the different sensitivity  levels are visualized). To date, the T-LSIM technique [3], the  Delay and the Phase Variation Mapping techniques were  published [4, 5]. We have already had some interesting results  by using these techniques [6] but not every “soft” defect case  study could be resolved in that way.


In this paper we propose to look at some different parameters  which characterize an analog signal and can be used as an  input for laser mapping. By applying a simple setup, without  any additional sophisticated tool, we show on a “golden” commercial IC the added value of this analysis. We also deal  with amplifying the weak signal variations induced by the  laser beam scan which often are hidden by the high signal  variations in analog or mixed-mode ICs.


BACKGROUND


Failure localization by using Laser Stimulation Techniques


In order to accurately localize a failure, laser stimulation  techniques use two major phenomena. A thermal  phenomenon, which allows us the localization of resistive  issues (resistance variation [7] and Seebeck effect [8]), is  often implemented by the use of a laser wavelength of  1340nm. A photoelectric phenomenon is induced by a laser  wavelength of less than 1100nm1. For this wavelength the


1 In reality a thermal phenomenon is also induced but is much  weaker compared to the photoelectric phenomenon.


photon energy is higher than the silicon band gap. Part of the  photons is absorbed by the silicon, resulting in free carrier  generation. Due to existing electric field (intrinsic electric  field of a p-n junction) the electrons and the holes generated  by the laser separate from each other. Hence, an additional  photocurrent will be generated at silicon level.


Many thermal (IR-OBIRCh [9], SEI [8], TIVA [8], RIL [10], SDL, xVM [4, 5]) and photoelectric (OBIC [11], LIVA [12], LADA [13], xVM [4, 5]) techniques were introduced to date. They can be performed from the frontside or from the  backside of the circuit with an easier access to the active  areas. Figure 1 shows a general failure localization setup when  using one of the above techniques. While the IC is electrically  stimulated, we perform a step by step laser scan above it to  locally introduce electrical changes through the desired  phenomenon: photoelectric or thermal. The correlation  between the laser position and the electrical response of the  DUT results in a mapping of failing or sensitive areas.


Figure 1: Failure localization principle by using Laser  Stimulation techniques.


Limitations of available xVM techniques applied on Analog & Mixed-Mode ICs


The defect sensitivity to the laser beam scan is visualized as a  variation in the device output signal. Depending on the signal  variation, an appropriate parameter should be observed and  used for the mapping. Among possible Variation Mapping  techniques, only two parameters have been measured up to  now: delay and phase of the signal. Our experience shows that  those parameters are sometimes not sufficient to find the  defect. For example, there are some devices where the most  suitable parameter to analyze is related to the frequency  domain, e.g. FFT (Fast Fourier Transform). First, high  frequency signals are easier to analyze in the frequency  domain. Second, different kinds of signal distortion can be


Laser beam


Laser Scanning  Microscope


Electrical


emulation


Sensitive/failing  zones mapping


INs


Signal


processing


OUT


Image processing & Control Unit


Correlation: laser  position (x,y) & DUT  output


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 278-282


detected through the measurement based on FFT, e.g. power  spectrum. This point will be described in the next section.


Another limitation of the existing xVM techniques is due to  the intrinsic sensitivity of the analog ICs, which is much  higher than that of digital ICs. This results in a mapping with  plenty of sensitive areas, especially when many blocks of the  dynamically stimulated circuit are operating. In such  mappings the areas with weak sensitivity will be hidden by  those with higher sensitivity. We thought that in certain cases  it would be interesting to highlight these weak spots.


In the next paragraph we will explain how we can overcome  the above limitations.


EXPERIMENTATION


Device & setup description


The analyzed IC, opened from the front side, is an operational  amplifier placed in a high gain configuration. The bias voltage  is V+ = 1.5V, V- = -1.5V. The input, a sinusoidal signal, has an  amplitude of 50mVp-p and a frequency of 1kHz. These  settings and the temperature of the amplifier are controlled  and maintained at the same values for all the measurements.  The general purpose is to localize sensitive areas which  correspond to some elementary structures like transistors, resistors, etc. by using xVM techniques, as shown in figure 2. The only difference with figure 1 is the use of an oscilloscope  as a signal processing tool. This oscilloscope is able of  measuring a wide range of parameters of the signal (e.g. rising  edge duration, falling edge duration, RMS (Root Mean  Square) etc.) and also applying mathematic functions (filtering, rescaling, FFT etc.). We use the AUX OUT  connector to send in real time the desired parameter, calculated from the waveform (IC output), to the failure  localization tool. In order to perform such operation, we have  developed a specific C++ application that converts in real time  the extracted parameter into a voltage value between 0V and  1V and sends this signal through the AUX OUT connector.


Figure 2: xVM setup by using Laser Stimulation techniques.


During the experimentation, the only laser used is a  photoelectric laser (wavelength: 1064nm), for which power is  fixed for all measurement at 0.35mW. A 2.5x zoom lens is  chosen to have a global view of the device. No  synchronization is applied between the laser scanning above  the DUT and the device OUT signal. The pixel dwell time is  fixed at 7ms (mean time to process the measured data by  oscilloscope and convert the result to the voltage level), and  image resolution is 512x512.


Analyzed parameters


Rising edge duration: this parameter is measured between


20-80% level of the signal transition.


RMS (Root Mean Square): measured on a voltage signal, it  represents its efficient value.


RMS


(


Where vi denotes measured sample values, and N is the  number of data points within the periods measured.


The Power Spectrum (PS) is the square of the magnitude  spectrum and shows how the average power is distributed as a  function of frequency. It is often represented on a logarithmic  scale.


2 2


logMMrefn


PS


Where Mn is the magnitude of a complex vector calculated  from a FFT of the signal and Mref is a reference value.


Such choice of the analyzed parameters is directly related to  the different distortions in the electrical signal induced by the  laser beam scan. Table 1 shows the sensitivity of the chosen  parameters to the different kinds of distortion.


Measured


parameter


Distortion in


tRISE_20-80% RMS PSMA X


PSNOISE_LEVEL


Amplitude  high level


+


Amplitude  low level


Amplitude  offset


Frequency


Duty cycle*


Table 1: Sensitivity of some measurable parameters to  different sinusoidal signal distortions.


* for square signal.


Figure 3 shows the results obtained by using the xVM setup  described before. Each image represents a mapping of an  entire device. The black color corresponds to the decrease of  the parameter value (compared to its average value), e.g. the  rising edge duration is shorter. The white color corresponds to  the increase of the chosen parameter value, e.g. the rising edge  duration is longer. These results show that depending on the  measured parameter we do not necessarily observe the same  sensitive areas (e.g. Fig.3b versus Fig. 3d).


Moreover, the sensitivity level is not the same when different  parameters are measured (e.g. Fig. 3a versus Fig. 3b). These  findings confirm that complementary information is brought  by the different parameters mapping.


Oscilloscope


a: trise 20-80%


b: RMS


c: PSMAX at 1kHz


d: PS noise level


Figure 3: xVM results for different mapped parameters:        a. 20-80% rise time, b. RMS, c. max of the 1st harmonic PS, d. noise level in PS.


The following step consists in extracting only weak variations  of the signal which are often hidden by high signal variations, all induced by the laser beam scan. For this purpose we  developed an algorithm which was applied in real time to the  parameter measured by the oscilloscope, before sending it to  the failure localization tool. We still use the C++ application  described before to send data to the failure localization tool. Through this application we fix the range of the parameter  values, supposed to vary under the Laser beam Scan (LS). This range is converted to a voltage value between 0V and  1V.


Equations 1 & 2 describe mathematically the algorithm. Equation 2 provides a better filtering for noise, which could  be particularly high, especially in analog or mixed mode  circuits.


LS


NO


RAW


_


Eq.1


p - value of the processed parameter used to create the  mapping (simulation in Fig. 4b).


pv_RAW - value of the parameter measured when an IC is  scanned with a laser beam (raw data).


pv_NO_LS - value of the parameter measured when no laser  stimulation is applied to the circuit (or no sensitivity to the LS  is detected).


'


No


Eq.2


p’ - value of the processed parameter used to create the  mapping (simulation in Fig. 4b’).


Figure 4 shows the simulation of our algorithm. Figure 4a  shows the raw data of the parameter values which can vary


when the laser beam scans above the sensitive areas (this kind  of data was used to create the mappings from figures 3a,b,c,d). This variation is detected for all pixels except pixel no. 3, which is our reference pixel (the part of the circuit which  corresponds to this pixel is not sensitive to the LS). It can be  noticed that the different variations were chosen in terms of  value and sign. The goal is to amplify the pixels 2 and 5 and  attenuate the pixels 1 and 4. Figure 4b & 4b’ are obtained by  applying respectively equation 1 & 2. When the variation of  the signal decreases, the calculated value p (in Fig. 4b) or p’ (in Fig. 4b’) increases. By fixing the measurement range (dashed line in Fig. 4b & 4b’) we can obtain the mapping of  the smallest variation induced by the laser beam.


Parameter changes under LS for different pixels


a: Raw data of the parameter variation for 5 pixels when the


IC is scanned by the laser beam. Only the 3rd pixel is not


sensitive to the laser beam scan.


b: Real time processing of raw data from Fig. 4a according to


equation 1. The dashed lines determine the measurement


range (noise as well as signal with no variation or high


variation are excluded).


b’: Real time processing of raw data from Fig. 4a according  to equation 2. The dashed lines determine the measurement


Figure 4: Simulation of an algorithm used to highlight the  smallest variation in the OUT signal induced by the laser  scan.


As an example, figure 5 shows the comparison between two  mappings where the raw data was used (Fig. 5a) and where  our algorithm was applied (Fig. 5b). In figure 5b the colour  varies depending on the signal variations (white=low, black=high) for the specified range (dashed line from Fig. 4b’). The arrows point at the low sensitivity areas which were  hardly visible in the original figure 5a and are highlighted  thanks to our algorithm in figure 5b.


4a


4b


Noise & signal with no variation


High signal variation


4b’


Figure 5: Comparison of xVM acquisition (PSMAX at 1kHz). a: Raw data, b: Raw data treated in real time to highlight  faint signal variation induced by the laser beam.


DISCUSSION


The advantage of such xVM acquisition setup is the possibility  to map various parameters in real time (one by one) by using  only one easy tool: an oscilloscope (no need to change the  setup). As we have seen in figure 3, different parameters are  used to image a specific signal distortion(s) when the  photoelectric laser stimulation is applied to the IC. An  important advantage asset to map different parameters is the  complementary information about the sensitive areas (Fig.3a  versus Fig.3d). There are also parameters, such as RMS, which allow us to detect many different kinds of signal  distortions (Tab.1). This results in mappings with many  sensitive areas (Fig.3b), sometimes complex to analyze. However, comparative analysis between good & failing ICs  can be performed. Another advantage asset is the frequencyrelated parameters mappings, such as power spectrum, which  are suitable to analyze RF ICs.


To save time it is also possible to map, just with one scan, a  few parameters, and display these mappings in real time (on  going).


Beside, the innovating point of this article is the extraction of  the smallest signal variations. As showed in figure 5b, the  small variations can be highlighted by applying the algorithm  described before. As a typical consequence, in analog or  mixed-mode ICs, in addition to these small variations, we will  also visualize the outline of the highly sensitive areas (Fig. 5b). This is due to the gradual sensitivity decrease from high  sensitive areas to those with no sensitivity to the laser beam  scan. For instance, on order to make the difference between  low and high sensitive areas we scan the DUT twice: with and  without applying the algorithm. We also have to notice that in  these kinds of treatments we amplify the lowest signal  variation at the cost of losing all the information about the sign  variations.


CONCLUSIONS


In this paper we presented a new way to characterize analog  or mixed-mode ICs. Few examples of parameters (trise, RMS, PS), measured at the output of a commercial IC, were used to  map the sensitivity of this circuit under photoelectric laser  stimulation. Each of these parameters highlighted specific  areas, and not necessarily the same, inside our IC. The  relationship between the chosen parameters and some  distortions induced by the laser beam scan has been explained. In this way we have proven that by measuring different  parameters during laser stimulation, it is possible to obtain  additional information about the device sensitivity. Moreover, all these mappings can be done by using one tool which  probably every Failure Analysis (FA) laboratory owns - an  oscilloscope. Besides measurements and several kinds of data  processing, this tool is flexible to develop some application  under C++ or other programming languages.  In this paper we  have also treated the issue of amplifying the weak variations  of the signal induced by the laser beam scan which can  correspond to the faulty transistor or to the abnormal region in  analog or mixed-mode ICs.


REFERENCES


[1] Michael R. Bruce et al, “Soft Defect Localization (SDL) on


ICs”, ISTFA, 2002, p21-27.


[2] M.Sienkiewicz et al, “Methodology to support laser-localized


soft defects on analog and mixed-mode advanced ICs”, IRPS,


2009.


[3] R. A. Falk et al., ”New Application of Thermal Laser   Signal


Injection Microscopy (T-LSIM)”, ISTFA, 2003,  p25-35.


[4] K. Sanchez et al, “Delay Variation Mapping induced by


dynamic laser stimulation”, IEEE, 2005,  p305-311.


[5] K. Sanchez et al., “Phase Variation Mapping, a Dynamic


Laser Stimulation Technique with Picosecond Timing


Resolution“, IRPS, 2007, p534-541.


[6] M.Sienkiewicz et al, “Failure localization & design debug on


mixed-mode ICs by using the Dynamic Laser Stimulation


techniques”, ISTFA, 2007, p86-91.


[7] F. Beaudoin, Thesis dissertation Localisation de défaut par la


face arrière des circuits intégrés.2002, N° d’ordre 2605.


[8] E.I. Cole Jr. et al., “TIVA and SEI Developments for


Enhanced Front and Backside Interconnection Failure


Analysis”, Microelectronic Reliability, 1999, Vol.39, p991-


996.


[9] K. Nikawa and S. Inoue, “New Capabilities of OBIRCH


Method for Fault Localization and Defect Detection”, ATS,


1997, p214-219.


[10] E.I. Cole et al., “Resistive Interconnection Localization”,


ISTFA, 2001, p43-57.


[11] T. Wilson and E. M. MacCabe, “Theory of optical beam


induced current images of defects in Semiconductors”, J.


Appl. Phys. 61(1), 1987, p191-195.


[12] E. I. Cole, Jr. et al., "Novel Failure Analysis Techniques


Using Photon Probing With a Scanning Optical Microscope",


IRPS, 1994, p388-398.


[13] J. A. Rowlette et al., “Critical Timing Analysis in


Microprocessors Using Near-IR Laser Assisted Device


Alteration (LADA)”, ITC, 2003, p264-273.


35th International Symposium for Testing and Failure Analysis  November 15–19, 2009, San Jose, California, USA, p 283-288

